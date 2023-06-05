# Comparing `tmp/line_async_webhook-0.2.0.tar.gz` & `tmp/line_async_webhook-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line_async_webhook-0.2.0.tar", max compression
+gzip compressed data, was "line_async_webhook-0.2.1.tar", max compression
```

## Comparing `line_async_webhook-0.2.0.tar` & `line_async_webhook-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-0.2.0/README.md
--rw-r--r--   0        0        0     2189 2023-06-04 14:57:04.780473 line_async_webhook-0.2.0/line_async_webhook/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:59:34.886600 line_async_webhook-0.2.0/line_async_webhook/py.typed
--rw-r--r--   0        0        0      421 2023-06-04 15:02:05.112825 line_async_webhook-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-0.2.1/README.md
+-rw-r--r--   0        0        0     2422 2023-06-05 14:10:11.480793 line_async_webhook-0.2.1/line_async_webhook/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:59:34.886600 line_async_webhook-0.2.1/line_async_webhook/py.typed
+-rw-r--r--   0        0        0      421 2023-06-05 14:10:22.310829 line_async_webhook-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-0.2.1/PKG-INFO
```

### Comparing `line_async_webhook-0.2.0/LICENSE` & `line_async_webhook-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `line_async_webhook-0.2.0/line_async_webhook/__init__.py` & `line_async_webhook-0.2.1/line_async_webhook/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,7 +54,14 @@
             function_return = func(event)
         else:
             function_return = func()
         ## END: copy from WebhookHandler.__invoke_func, but added function_return capture
 
         await function_return
 
+    @staticmethod
+    def __get_args_count(func):
+        return WebhookHandler.__get_args_count(func)
+
+    @staticmethod
+    def __get_handler_key(event, message=None):
+        return WebhookHandler.__get_handler_key(event, message)
```

