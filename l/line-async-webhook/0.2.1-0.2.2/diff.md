# Comparing `tmp/line_async_webhook-0.2.1.tar.gz` & `tmp/line_async_webhook-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line_async_webhook-0.2.1.tar", max compression
+gzip compressed data, was "line_async_webhook-0.2.2.tar", max compression
```

## Comparing `line_async_webhook-0.2.1.tar` & `line_async_webhook-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-0.2.1/README.md
--rw-r--r--   0        0        0     2422 2023-06-05 14:10:11.480793 line_async_webhook-0.2.1/line_async_webhook/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:59:34.886600 line_async_webhook-0.2.1/line_async_webhook/py.typed
--rw-r--r--   0        0        0      421 2023-06-05 14:10:22.310829 line_async_webhook-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-0.2.2/README.md
+-rw-r--r--   0        0        0     2925 2023-06-05 14:39:00.204760 line_async_webhook-0.2.2/line_async_webhook/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:59:34.886600 line_async_webhook-0.2.2/line_async_webhook/py.typed
+-rw-r--r--   0        0        0      421 2023-06-05 14:39:14.165614 line_async_webhook-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-0.2.2/PKG-INFO
```

### Comparing `line_async_webhook-0.2.1/LICENSE` & `line_async_webhook-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `line_async_webhook-0.2.1/line_async_webhook/__init__.py` & `line_async_webhook-0.2.2/line_async_webhook/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,14 +39,27 @@
                     LOGGER.info('No handler of ' + key + ' and no default handler')
                 else:
                     if inspect.iscoroutinefunction(func):
                         task_group.soonify(self.__invoke_func_async)(func, event, payload)
                     else:
                         self.__invoke_func(func, event, payload)
 
+    def __add_handler(self, func, event, message=None):
+        return super().__add_handler(func, event, message)
+
+    def add_handler(self, func, event, message=None):
+        if isinstance(message, (list, tuple)):
+            for it in message:
+                self.__add_handler(func, event, message=it)
+        else:
+            self.__add_handler(func, event, message=message)
+
+    @classmethod
+    def __invoke_func(cls, func, event, payload):
+        super().__invoke_func(func, event, payload)
 
     @classmethod
     async def __invoke_func_async(cls, func, event, payload):
         ## START: copy from WebhookHandler.__invoke_func, but added function_return capture
         (has_varargs, args_count) = cls.__get_args_count(func)
         if has_varargs or args_count == 2:
             function_return = func(event, payload.destination)
```

