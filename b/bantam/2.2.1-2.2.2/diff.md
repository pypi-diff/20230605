# Comparing `tmp/bantam-2.2.1.tar.gz` & `tmp/bantam-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.2.1.tar", last modified: Sun Jun  4 16:08:02 2023, max compression
+gzip compressed data, was "bantam-2.2.2.tar", last modified: Mon Jun  5 00:33:32 2023, max compression
```

## Comparing `bantam-2.2.1.tar` & `bantam-2.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 16:08:02.367650 bantam-2.2.1/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.1/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.1/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-04 16:08:02.367650 bantam-2.2.1/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-04 16:07:54.000000 bantam-2.2.1/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.363650 bantam-2.2.1/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.1/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10356 2023-06-04 16:03:49.000000 bantam-2.2.1/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.1/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.1/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    18406 2023-06-04 16:03:49.000000 bantam-2.2.1/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.1/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4399 2023-06-04 13:45:48.000000 bantam-2.2.1/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    44538 2023-06-04 16:03:49.000000 bantam-2.2.1/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.1/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.1/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.1/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.2.1/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4517 2023-06-04 02:21:15.000000 bantam-2.2.1/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4573 2023-06-04 14:26:39.000000 bantam-2.2.1/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.1/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.1/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.1/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.2.1/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.2.1/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-05 00:33:32.454154 bantam-2.2.2/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.2/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.2/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-05 00:33:32.454154 bantam-2.2.2/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-05 00:23:53.000000 bantam-2.2.2/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.450154 bantam-2.2.2/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.450154 bantam-2.2.2/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.2/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10547 2023-06-04 23:41:07.000000 bantam-2.2.2/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.2/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.2/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    19764 2023-06-04 23:29:54.000000 bantam-2.2.2/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.2/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.2.2/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    45348 2023-06-05 00:08:58.000000 bantam-2.2.2/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.2/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.2/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.2/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.2.2/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4636 2023-06-05 00:12:39.000000 bantam-2.2.2/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4573 2023-06-04 14:26:39.000000 bantam-2.2.2/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.2/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.2/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.2/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.2.2/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.2.2/test/test_js_async.py
```

### Comparing `bantam-2.2.1/PKG-INFO` & `bantam-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.1
+Version: 2.2.2
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.1
+Download-URL: https://github.com/bantam/dist/2.2.2
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.1/setup.py` & `bantam-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.2.1"
+VERSION = "2.2.2"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.2.1/src/bantam/__init__.py` & `bantam-2.2.2/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/src/bantam/api.py` & `bantam-2.2.2/src/bantam/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 
 
 class API:
 
     def __init__(self, clazz, func, method: RestMethod, content_type: str, is_instance_method: bool,
                  is_class_method: bool,
                  is_constructor: bool,
+                 on_disconnect: Optional[Callable[[], None]] = None,
                  timeout: Optional[ClientTimeout] = None,
                  expire_on_exit: bool = False, uuid_param: Optional[str] = None):
         annotations = func.__annotations__
         self._clazz = clazz
+        self._on_disconnect = on_disconnect
         self._is_class_method = is_class_method
         self._is_instance_method = is_instance_method
         self._is_static = not self._is_class_method and not self._is_instance_method
         self._expire_obj = expire_on_exit
         self._func = func
         self._real_func = func
         self._method = method
@@ -97,14 +99,18 @@
         return self._real_func.__doc__
 
     @property
     def method(self):
         return self._method
 
     @property
+    def on_disonnect(self):
+        return self._on_disconnect
+
+    @property
     def is_instance_method(self) -> bool:
         return self._is_instance_method
 
     @property
     def content_type(self) -> str:
         return self._content_type
```

### Comparing `bantam-2.2.1/src/bantam/autogen/main.py` & `bantam-2.2.2/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/src/bantam/client.py` & `bantam-2.2.2/src/bantam/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,30 +207,42 @@
             rest_method = api._func._bantam_web_api.method
             if rest_method.value == RestMethod.GET.value:
                 url_args = cls._generate_url_args(kwargs=kwargs)
                 url = f"{base_url}{url_args}"
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.get(url) as resp:
                         resp.raise_for_status()
+                        buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             if data:
-                                if api.return_type == str and data[-1] == 0:
-                                    data = data[:-1]
-                                data = data.decode('utf-8')
-                                yield conversions.from_str(data, api.return_type)
+                                if api.return_type == str:
+                                    buffer += data.decode('utf-8')
+                                    *data_items, buffer = buffer.split('\0')
+                                    for datum in data_items:
+                                        yield conversions.from_str(datum, api.return_type)
+                                else:
+                                    data = data.decode('utf-8')
+                                    yield conversions.from_str(data, api.return_type)
             else:
                 payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
                                       for k, v in kwargs.items()})
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.post(base_url, data=payload) as resp:
+                        buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             resp.raise_for_status()
                             if data:
-                                data = data.decode('utf-8')
-                                yield conversions.from_str(data, api.return_type)
+                                if api.return_type == str:
+                                    buffer += data.decode('utf-8')
+                                    *data_items, buffer = buffer.split('\0')
+                                    for datum in data_items:
+                                        yield conversions.from_str(datum, api.return_type)
+                                else:
+                                    data = data.decode('utf-8')
+                                    yield conversions.from_str(data, api.return_type)
 
         setattr(clazz, name, class_method_streamed)
 
     @classmethod
     def _add_instance_method(cls, clazz: Type, impl_name: str, end_point: str, method,
                              common_headers: dict):
         # class/static methods
@@ -296,33 +308,43 @@
             rest_method = api.method
             if rest_method == RestMethod.GET:
                 url_args = cls._generate_url_args(self_id=self.self_id, kwargs=kwargs_)
                 url = f"{base_url}{url_args}"
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.get(url) as resp:
                         resp.raise_for_status()
+                        buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             if data:
-                                if api.return_type == str and data[-1] == 0:
-                                    data = data[:-1]
-                                data = data.decode('utf-8')
-                                yield conversions.from_str(data, api.return_type)
+                                if api.return_type == str:
+                                    buffer += data.decode('utf-8')
+                                    *data_items, buffer = buffer.split('\0')
+                                    for datum in data_items:
+                                        yield conversions.from_str(datum, api.return_type)
+                                else:
+                                    data = data.decode('utf-8')
+                                    yield conversions.from_str(data, api.return_type)
             else:
                 url = f"{base_url}?self={self.self_id}"
                 kwargs_['self'] = self.self_id
                 payload = json.dumps({k: conversions.to_str(v) for k, v in kwargs_.items()})
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.post(url, data=payload) as resp:
                         resp.raise_for_status()
+                        buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             if data:
-                                if api.return_type == str and data[-1] == 0:
-                                    data = data[:-1]
-                                data = data.decode('utf-8')
-                                yield conversions.from_str(data, api.return_type)
+                                if api.return_type == str:
+                                    buffer += data.decode('utf-8')
+                                    *data_items, buffer = buffer.split('\0')
+                                    for datum in data_items:
+                                        yield conversions.from_str(datum, api.return_type)
+                                else:
+                                    data = data.decode('utf-8')
+                                    yield conversions.from_str(data, api.return_type)
         setattr(clazz, name, instance_method_streamed)
 
     # noinspection PyPep8Naming
     @classmethod
     def Client(cls: C, end_point: str, impl_name: Optional[str] = None,
                common_headers: Optional[dict] = None) -> C:
         if cls == WebInterface:
```

### Comparing `bantam-2.2.1/src/bantam/conversions.py` & `bantam-2.2.2/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/src/bantam/decorators.py` & `bantam-2.2.2/src/bantam/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 PreProcessor = Callable[[Request], Union[None, Dict[str, Any]]]
 PostProcessor = Callable[[Union[Response, StreamResponse]], Union[Response, StreamResponse]]
 
 
 def web_api(content_type: str, method: RestMethod = RestMethod.GET,
             is_constructor: bool = False,
             expire_obj: bool = False,
+            on_disconnect: Optional[Callable[[], None]] = None,
             timeout: Optional[ClientTimeout] = None,
             uuid_param: Optional[str] = None,
             preprocess: Optional[PreProcessor] = None,
             postprocess: Optional[PostProcessor] = None) -> Callable[[WebApi], WebApi]:
     """
     Decorator for class async method to register it as an API with the `WebApplication` class
     Decorated functions should be static class methods with parameters that are convertible from a string
@@ -41,14 +42,16 @@
     http://<host>:port>/MyRestAPI?name=Jill
 
 
     :param content_type: content type to disply (e.g., "text/html")
     :param method: one of MethodEnum rest api methods (GET or POST)
     :param is_constructor: set to True if API is static method return a class instnace, False oherwise (default)
     :param expire_obj: for instance methods only, epxire the object upon successful completion of that call
+    :param on_disconnect: callback if client disconnects unexpectedly
+    :param timeout: optional timeout value for response to request to timeout
     :return: callable decorator
     """
     from .http import WebApplication
     if not isinstance(content_type, str):
         raise Exception("@web_api must provide one str argument which is the content type")
 
     def wrapper(func: Union[WebApi, staticmethod, classmethod]) -> Union[WebApi, staticmethod, classmethod]:
@@ -78,12 +81,13 @@
                                             timeout=timeout,
                                             is_instance_method=not is_static and not is_class_method,
                                             is_class_method=is_class_method,
                                             method=method,
                                             content_type=content_type,
                                             is_constructor=is_constructor,
                                             expire_on_exit=expire_obj,
+                                            on_disconnect=on_disconnect,
                                             uuid_param=uuid_param,
                                             preprocess=preprocess,
                                             postprocess=postprocess)
 
     return wrapper
```

### Comparing `bantam-2.2.1/src/bantam/http.py` & `bantam-2.2.2/src/bantam/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 import os
 import sys
 import traceback
 import types
 import uuid as uuid_pkg
 
 import logging
-from aiohttp import ClientTimeout
+from aiohttp import ClientTimeout, ClientConnectionError
 from aiohttp import web
 from aiohttp.web import (
     Application,
     Request,
     Response,
     StreamResponse,
 )
+from asyncio import CancelledError
 from contextlib import suppress
 from pathlib import Path
 from ssl import SSLContext
 from typing import (
     Any,
     Awaitable,
     Callable,
@@ -538,27 +539,28 @@
     def _func_wrapper(cls, clazz, func: WebApi,
                       is_instance_method: bool,
                       is_class_method: bool,
                       is_constructor: bool,
                       expire_on_exit: bool,
                       method: RestMethod,
                       content_type: str,
+                      on_disconnect: Optional[Callable[[], None]] = None,
                       timeout: Optional[ClientTimeout] = None,
                       uuid_param: Optional[str] = None,
                       preprocess: Optional[PreProcessor] = None,
                       postprocess: Optional[PostProcessor] = None) -> WebApi:
         """
         Wraps a function as called from decorators.web_api to set up logic to invoke get or post requests
 
         :param func: function to wrap
         :param clazz: if function is instance method, provide owning class, otherwise None
         :return: function back, having processed as a web api and registered the route
         """
         api = API(clazz, func, method=method, content_type=content_type, is_instance_method=is_instance_method,
-                  is_class_method=is_class_method,
+                  is_class_method=is_class_method, on_disconnect=on_disconnect,
                   is_constructor=is_constructor, expire_on_exit=expire_on_exit, uuid_param=uuid_param, timeout=timeout)
         func._bantam_web_api = api
         if hasattr(func, '__func__'):
             func.__func__._bantam_web_api = api
             func = func.__func__
         if is_instance_method:
             cls._instance_methods.append(api)
@@ -596,14 +598,22 @@
                 try:
                     postprocess = postprocess or app.postprocessor
                     postprocess(response) if postprocess else response
                 except Exception as e:
                     text = traceback.format_exc()
                     return Response(status=400, text=f"Error in post-processing of response: {e}\n{text}")
                 return response
+            except (CancelledError, ConnectionResetError, ClientConnectionError):
+                if api.is_instance_method:
+                    self_id = request.query['self']
+                    instance = cls.ObjectRepo.instances.get(self_id)
+                    api.on_disonnect(instance)
+                else:
+                    api.on_diconnect()
+                raise
             except BaseException as e:
                 text = traceback.format_exc()
                 return Response(status=500, reason=f"Server error: {e}",
                                 body=f"Server error: {e}\n{text}", content_type="test/plain")
 
         invoke.clazz = WebApplication._instance_methods_class_map.get(api) if is_instance_method else None
         if method == RestMethod.GET:
@@ -840,19 +850,23 @@
                 async_q = asyncio.Queue()
                 content_type = "text/streamed; charset=x-user-defined"
                 response = StreamResponse(status=200, reason='OK', headers={'Content-Type': content_type})
                 await response.prepare(request)
                 try:
                     # iterate to get the one (and hopefully only) yielded element:
                     # noinspection PyTypeChecker
+                    count = 0
                     async for res in awaitable:
                         serialized = _serialize_return_value(res, encoding)
                         if isinstance(res, str):
                             serialized += b'\0'
                         await response.write(serialized)
+                        count += 1
+                except (CancelledError, ConnectionResetError, ClientConnectionError):
+                    raise
                 except Exception as e:
                     print(str(e))
                     await async_q.put(None)
                     raise RuntimeError(f"Exception in server-side logic: {e}") from e
                 await response.write_eof()
             else:
                 #################
@@ -881,14 +895,16 @@
                 return Response(status=200, body=result if result is not None else b"Success",
                                 content_type=content_type)
 
         except TypeError as e:
             return Response(status=400, text=f"Improperly formatted query: {str(e)}")
         except HTTPException as e:
             return Response(status=e.status_code, text=str(e))
+        except (CancelledError, ConnectionResetError, ClientConnectionError):
+            raise
         except Exception as e:
             text = f"Exception: {e}\n {traceback.format_exc()}"
             return Response(status=500, text=text)
         finally:
             # noinspection PyUnresolvedReferences,PyProtectedMember
             del cls._context[sys._getframe(0)]
```

### Comparing `bantam-2.2.1/src/bantam/js.py` & `bantam-2.2.2/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/src/bantam/js_async.py` & `bantam-2.2.2/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/src/bantam/pythonclient.py` & `bantam-2.2.2/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/src/bantam.egg-info/PKG-INFO` & `bantam-2.2.2/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.1
+Version: 2.2.2
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.1
+Download-URL: https://github.com/bantam/dist/2.2.2
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.1/src/bantam.egg-info/SOURCES.txt` & `bantam-2.2.2/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/test/test_client_get.py` & `bantam-2.2.2/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/test/test_client_post.py` & `bantam-2.2.2/test/test_client_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import sys
 if True:
     sys.path.insert(0, str(Path(__file__).parent / 'example'))
 from pathlib import Path
 
 import pytest
 from bantam.http import WebApplication
-from class_rest_post import RestAPIExampleAsyncPostInterface
+from class_rest_post import RestAPIExampleAsyncPostInterface, RestAPIExampleAsyncPost
+
+PORT = 8237
 
 
 @pytest.mark.asyncio
 async def test_client_class_method(tmpdir):
-    PORT = 8237
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
         client: RestAPIExampleAsyncPostInterface = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
         response = await client.api_post_basic(42, True, 992.123)
         assert response == f"Response to test_api_basic 1.0 2"
@@ -26,15 +27,14 @@
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_constructor(tmpdir):
-    PORT = 8237
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
         client: RestAPIExampleAsyncPostInterface = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
         response = await client.explicit_constructor(42)
         assert response.self_id is not None
@@ -42,15 +42,14 @@
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_instance_method(tmpdir):
-    PORT = 8237
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
         Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
         instance = await Client.explicit_constructor(4242)
         response = await instance.my_value()
@@ -59,15 +58,14 @@
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_class_method_streamed(tmpdir):
-    PORT = 8237
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
         client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
         count = 0
         async for item in client.api_post_stream(42, True, 992.123, "They're here..."):
@@ -78,15 +76,14 @@
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed(tmpdir):
-    PORT = 8237
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
         Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
         instance = await Client.explicit_constructor(29)
         count = 0
@@ -95,25 +92,28 @@
             count += 1
         assert count == 200
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
+
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed_str(tmpdir):
-    PORT = 8237
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
         Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
         instance = await Client.explicit_constructor(29)
         count = 0
         async for item in instance.my_value_repeated_string(200):
-            assert item == str(29)
+            assert item == str(29)*65537
             count += 1
-        assert count == 200
+            if count == 121:
+                break  # disconnects client
+        await asyncio.sleep(1)  # give server time to process disconnect
+        assert RestAPIExampleAsyncPost.disconnected
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
```

### Comparing `bantam-2.2.1/test/test_client_post_inherited_apis.py` & `bantam-2.2.2/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/test/test_conversions.py` & `bantam-2.2.2/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/test/test_decorators.py` & `bantam-2.2.2/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/test/test_js.py` & `bantam-2.2.2/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.1/test/test_js_async.py` & `bantam-2.2.2/test/test_js_async.py`

 * *Files identical despite different names*

