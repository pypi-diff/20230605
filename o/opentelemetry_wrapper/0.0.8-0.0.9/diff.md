# Comparing `tmp/opentelemetry_wrapper-0.0.8.tar.gz` & `tmp/opentelemetry_wrapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_wrapper-0.0.8.tar", last modified: Tue Nov 29 07:55:44 2022, max compression
+gzip compressed data, was "opentelemetry_wrapper-0.0.9.tar", last modified: Tue Nov 29 10:18:45 2022, max compression
```

## Comparing `opentelemetry_wrapper-0.0.8.tar` & `opentelemetry_wrapper-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     2311 2022-09-27 08:12:51.286165 opentelemetry_wrapper-0.0.8/.gitignore
--rw-r--r--   0        0        0     9229 2022-09-28 02:55:55.816861 opentelemetry_wrapper-0.0.8/LICENSE
--rw-r--r--   0        0        0     2396 2022-11-29 07:54:03.131763 opentelemetry_wrapper-0.0.8/README.md
--rw-r--r--   0        0        0     3775 2022-11-28 10:31:15.575275 opentelemetry_wrapper-0.0.8/TODO.md
--rw-r--r--   0        0        0       60 2022-09-27 08:12:51.287162 opentelemetry_wrapper-0.0.8/aaaa/bbbb.py
--rw-r--r--   0        0        0     3237 2022-09-27 08:12:51.287162 opentelemetry_wrapper-0.0.8/experiment_otel_logging.py
--rw-r--r--   0        0        0     2486 2022-09-27 08:12:51.288159 opentelemetry_wrapper-0.0.8/fastapi_main.py
--rw-r--r--   0        0        0     1055 2022-11-29 07:55:33.604997 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/__init__.py
--rw-r--r--   0        0        0     1067 2022-11-29 07:46:41.010115 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/config/config.py
--rw-r--r--   0        0        0     4644 2022-11-29 07:48:49.311472 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/config/service_name.py
--rw-r--r--   0        0        0     1277 2022-11-29 07:53:02.319884 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_dataclasses.py
--rw-r--r--   0        0        0     8818 2022-11-29 07:53:02.283982 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_decorator.py
--rw-r--r--   0        0        0     2656 2022-11-29 07:53:02.335844 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_fastapi.py
--rw-r--r--   0        0        0     4438 2022-11-29 07:53:02.354200 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_logging.py
--rw-r--r--   0        0        0      605 2022-11-29 07:53:02.303929 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_requests.py
--rw-r--r--   0        0        0    14550 2022-11-29 03:14:30.775550 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/introspect.py
--rw-r--r--   0        0        0     7512 2022-09-28 03:30:31.950785 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/json_encoder.py
--rw-r--r--   0        0        0     6002 2022-09-28 03:29:48.386634 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/logging_json_formatter.py
--rw-r--r--   0        0        0     1819 2022-11-29 07:40:56.218872 opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/tracers.py
--rw-r--r--   0        0        0      889 2022-11-29 07:31:46.479401 opentelemetry_wrapper-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      299 2022-11-29 07:31:46.497354 opentelemetry_wrapper-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1496 2022-09-27 08:12:51.295142 opentelemetry_wrapper-0.0.8/setup_otel_logging.py
--rw-r--r--   0        0        0     3189 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2311 2022-09-27 08:12:51.286165 opentelemetry_wrapper-0.0.9/.gitignore
+-rw-r--r--   0        0        0     9229 2022-09-28 02:55:55.816861 opentelemetry_wrapper-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2501 2022-11-29 10:18:17.706896 opentelemetry_wrapper-0.0.9/README.md
+-rw-r--r--   0        0        0     3775 2022-11-28 10:31:15.575275 opentelemetry_wrapper-0.0.9/TODO.md
+-rw-r--r--   0        0        0       60 2022-09-27 08:12:51.287162 opentelemetry_wrapper-0.0.9/aaaa/bbbb.py
+-rw-r--r--   0        0        0     3237 2022-09-27 08:12:51.287162 opentelemetry_wrapper-0.0.9/experiment_otel_logging.py
+-rw-r--r--   0        0        0     2486 2022-09-27 08:12:51.288159 opentelemetry_wrapper-0.0.9/fastapi_main.py
+-rw-r--r--   0        0        0     1055 2022-11-29 10:18:33.859577 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/__init__.py
+-rw-r--r--   0        0        0     1433 2022-11-29 09:50:36.908078 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/config.py
+-rw-r--r--   0        0        0     1024 2022-11-29 09:49:22.064362 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/log_level.py
+-rw-r--r--   0        0        0     5882 2022-11-29 10:17:05.115821 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/service_name.py
+-rw-r--r--   0        0        0     1277 2022-11-29 07:53:02.319884 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_dataclasses.py
+-rw-r--r--   0        0        0     8818 2022-11-29 07:53:02.283982 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_decorator.py
+-rw-r--r--   0        0        0     2656 2022-11-29 07:53:02.335844 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_fastapi.py
+-rw-r--r--   0        0        0     4477 2022-11-29 10:17:51.984560 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_logging.py
+-rw-r--r--   0        0        0      605 2022-11-29 07:53:02.303929 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_requests.py
+-rw-r--r--   0        0        0    14550 2022-11-29 03:14:30.775550 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/introspect.py
+-rw-r--r--   0        0        0     7512 2022-09-28 03:30:31.950785 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/json_encoder.py
+-rw-r--r--   0        0        0     6002 2022-09-28 03:29:48.386634 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/logging_json_formatter.py
+-rw-r--r--   0        0        0     2117 2022-11-29 10:05:37.035599 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/tracers.py
+-rw-r--r--   0        0        0      889 2022-11-29 07:31:46.479401 opentelemetry_wrapper-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      299 2022-11-29 07:31:46.497354 opentelemetry_wrapper-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1496 2022-09-27 08:12:51.295142 opentelemetry_wrapper-0.0.9/setup_otel_logging.py
+-rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.0.9/PKG-INFO
```

### Comparing `opentelemetry_wrapper-0.0.8/.gitignore` & `opentelemetry_wrapper-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/LICENSE` & `opentelemetry_wrapper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/README.md` & `opentelemetry_wrapper-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 ## usage
 
 todo: write stuff here
 
 ## env vars
 
-| Variable Name                 | Description                                              | Default (if not set)                                                |
-|-------------------------------|----------------------------------------------------------|---------------------------------------------------------------------|
-| `OTEL_SERVICE_NAME`           | Sets the value of the `service.name` resource attribute. | f'{username}@{hostname}.{namespace or domain}:<{filename of main}>' |
-| `OTEL_RESOURCE_ATTRIBUTES`    | Key-value pairs to be used as resource attributes.       | *NA*                                                                |
-| TODO: `OTEL_LOG_LEVEL`        | Log level used by this logging instrumentor              | `NOTSET`                                                            |
-| `OTEL_WRAPPER_DISABLED`       | Set to `true` to disable everything globally             | `false`                                                             |
-| `OTEL_EXPORTER_OTLP_ENDPOINT` | Looks like `http://tempo.local:4317`                     | *NA*                                                                |
+| Variable Name                 | Description                                                             | Default (if not set)                                                |
+|-------------------------------|-------------------------------------------------------------------------|---------------------------------------------------------------------|
+| `OTEL_SERVICE_NAME`           | Sets the value of the `service.name` resource attribute.                | f'{username}@{hostname}.{namespace or domain}:<{filename of main}>' |
+| `OTEL_RESOURCE_ATTRIBUTES`    | Key-value pairs to be used as resource attributes.                      | *NA*                                                                |
+| `OTEL_LOG_LEVEL`              | Log level used by this logging instrumentor                             | `NOTSET`                                                            |
+| `OTEL_WRAPPER_DISABLED`       | Set to `true` to disable everything globally (e.g. when running pytest) | `false`                                                             |
+| `OTEL_EXPORTER_OTLP_ENDPOINT` | Looks like `http://tempo.local:4317`                                    | *NA*                                                                |
 
 
 ## read the original docs
 
 * [OpenTelemetry](https://opentelemetry.io/docs)
 * [OpenTracing](https://opentracing.io/docs)
 * [SkyWalking](https://skywalking.apache.org/docs/skywalking-python/latest/readme/)
```

### Comparing `opentelemetry_wrapper-0.0.8/TODO.md` & `opentelemetry_wrapper-0.0.9/TODO.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/experiment_otel_logging.py` & `opentelemetry_wrapper-0.0.9/experiment_otel_logging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/fastapi_main.py` & `opentelemetry_wrapper-0.0.9/fastapi_main.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/__init__.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 """
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 from opentelemetry_wrapper.config.config import OTEL_WRAPPER_DISABLED
 from opentelemetry_wrapper.instrument_dataclasses import instrument_dataclasses
 from opentelemetry_wrapper.instrument_decorator import instrument_decorate
 from opentelemetry_wrapper.instrument_fastapi import instrument_fastapi
 from opentelemetry_wrapper.instrument_logging import instrument_logging
 from opentelemetry_wrapper.instrument_requests import instrument_requests
```

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/config/config.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import os
+from typing import Optional
 
+from opentelemetry_wrapper.config.log_level import get_log_level
 from opentelemetry_wrapper.config.service_name import get_default_service_name
+from opentelemetry_wrapper.config.service_name import get_k8s_namespace
 from opentelemetry_wrapper.config.service_name import getenv_otel_service_name
 
 # global flag to override opentelemetry and not do anything
 # because opentelemetry is too verbose in tests
 # naming / terminology based on:
 # https://opentelemetry.io/docs/reference/specification/sdk-environment-variables/#:~:text=OTEL_SDK_DISABLED
 OTEL_WRAPPER_DISABLED: bool = os.getenv('OTEL_WRAPPER_DISABLED', 'false').casefold().strip() == 'true'
 
-# tries these 3 things, in order:
+# tries these things, in order:
 # 1. `OTEL_SERVICE_NAME` env var
 # 2. `service.name` property from `OTEL_RESOURCE_ATTRIBUTES` env var
-# 3. `get_default_service_name()` (which technically breaks OpenTelemetry spec)
-# if all the above fails, falls back to 'unknown_service'
+# 3. if running in k8s, returns {namespace}/{pod_name}
+# 4. otherwise, f'{_username}{_hostname}{_namespace}{_filename}' (which technically breaks OpenTelemetry spec)
+# 5. if all the above fails, falls back to 'unknown_service'
 OTEL_SERVICE_NAME: str = getenv_otel_service_name() or get_default_service_name() or 'unknown_service'
+OTEL_SERVICE_NAMESPACE: Optional[str] = get_k8s_namespace() or None
 
 # enable exporting to tempo for visualization in grafana
 OTEL_EXPORTER_OTLP_ENDPOINT: str = os.getenv('OTEL_EXPORTER_OTLP_ENDPOINT', '').strip()
+
+OTEL_LOG_LEVEL: int = get_log_level()
```

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/config/service_name.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/service_name.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,49 +18,88 @@
     except Exception:
         return ''
 
 
 @lru_cache
 def get_hostname() -> str:
     out = ''
+
+    # os-specific hostname env vars
     if not out:
         out = os.getenv('HOSTNAME', '').strip()  # linux
     if not out:
         out = os.getenv('COMPUTERNAME', '').strip()  # windows
+
+    # k8s-specific hostname path
+    if not out:
+        k8s_hostname_path = Path('/etc/hostname')
+        if k8s_hostname_path.is_file():
+            # noinspection PyBroadException
+            try:
+                hostname = k8s_hostname_path.read_text().strip()
+                if hostname.count('-') >= 2:
+                    return hostname.rsplit('-', 2)[0]
+            except Exception:
+                pass
+
+    # linux-specific, based on uname
     if not out:
         # noinspection PyBroadException
         try:
             out = platform.node().strip()
         except Exception:
             pass
+
+    # something network related
     if not out:
         # noinspection PyBroadException
         try:
             out = socket.gethostname().strip()
         except Exception:
             pass
     return out
 
 
 @lru_cache
-def get_namespace() -> str:
-    # get k8s namespace
+def get_k8s_namespace() -> str:
     # https://kubernetes.io/docs/tasks/run-application/access-api-from-pod/#directly-accessing-the-rest-api
     namespace_path = Path('/var/run/secrets/kubernetes.io/serviceaccount/namespace')
     if namespace_path.is_file():
         # noinspection PyBroadException
         try:
             namespace = namespace_path.read_text().strip()
             if namespace:
                 return namespace
         except Exception:
             pass
+    return ''
 
-    # not in k8s, try to get domain by removing hostname from fqdn
+
+@lru_cache
+def get_k8s_pod_name() -> str:
+    # does the file exist
+    k8s_hostname_path = Path('/etc/hostname')
+    if not k8s_hostname_path.is_file():
+        return ''
+
+    # noinspection PyBroadException
+    try:
+        hostname = k8s_hostname_path.read_text().strip()
+        if hostname.count('-') >= 2:
+            return hostname.rsplit('-', 2)[0]
+    except Exception:
+        pass
+    return ''
+
+
+@lru_cache
+def get_domain() -> str:
+    # try to get domain by removing hostname from fqdn
     hostname = get_hostname()
+
     # noinspection PyBroadException
     try:
         fqdn = socket.getfqdn()
         if fqdn.strip().casefold().startswith(f'{hostname.casefold()}.'):
             return fqdn[len(hostname) + 1:].strip()
     except Exception:
         pass
@@ -77,14 +116,24 @@
     # todo: also try getting the primary dns suffix from the dns suffix search list
 
     # everything failed, return nothing
     return ''
 
 
 @lru_cache
+def get_namespace() -> str:
+    # get k8s namespace
+    if get_k8s_namespace():
+        return get_k8s_namespace()
+
+    # not in k8s, try to get domain instead
+    return get_domain()
+
+
+@lru_cache
 def get_main_filename() -> str:
     if getattr(__main__, '__file__', None):
         main_full_path = Path(__main__.__file__)  # can be undefined, e.g. C modules or Jupyter notebooks
         if main_full_path.is_file():  # should always be true
             return main_full_path.name
 
     return ''
@@ -103,14 +152,18 @@
 
     it would be more correct to just return the namespace instead,
     but my preference (for now at least) is to isolate the instance for further debugging
 
     :return: {username}@{hostname}.{namespace or domain}:<{filename of main}> or an empty string
     """
 
+    # try return just namespace/pod by default
+    if get_k8s_namespace():
+        return f'{get_k8s_namespace()}/{get_k8s_pod_name()}'
+
     # formatting
     _username = f'{get_username()}@' if get_username() else ''
     _hostname = get_hostname()
     _namespace = f'.{get_namespace()}' if get_namespace() else ''
     _filename = f':<{get_main_filename()}>' if get_main_filename() else ''
 
     # if at least one of the above succeeded, then make sure hostname is not blank
@@ -121,15 +174,15 @@
 
     # format the output nicely
     return f'{_username}{_hostname}{_namespace}{_filename}'
 
 
 def getenv_otel_service_name() -> str:
     """
-    tries these 3 things, in order:
+    tries these 2 things, in order:
     1. `OTEL_SERVICE_NAME` env var
     2. `service.name` property from `OTEL_RESOURCE_ATTRIBUTES` env var
-    3. `get_default_service_name()` (which technically breaks OpenTelemetry spec)
-    if all the above fails, falls back to 'unknown_service'
+
+    otherwise, returns an empty string
     """
     otel_detected_service_name = OTELResourceDetector().detect().attributes.get('service.name', '') or ''
     return str(otel_detected_service_name).strip()
```

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_dataclasses.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_dataclasses.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_decorator.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_decorator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_fastapi.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_fastapi.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_logging.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import wraps
 from pathlib import Path
 from typing import Optional
 from typing import TextIO
 
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 
+from opentelemetry_wrapper.config.config import OTEL_LOG_LEVEL
 from opentelemetry_wrapper.config.config import OTEL_WRAPPER_DISABLED
 from opentelemetry_wrapper.instrument_decorator import instrument_decorate
 from opentelemetry_wrapper.utils.logging_json_formatter import JsonFormatter
 
 # write IDs as 0xBEEF instead of BEEF so it matches the trace json exactly
 LOGGING_FORMAT_VERBOSE = (
     '%(asctime)s '
@@ -31,15 +32,15 @@
     '[%(name)s:%(module)s:%(funcName)s] '
     '%(message)s'
 )
 
 
 @lru_cache  # avoid creating duplicate handlers
 def get_json_handler(*,
-                     level: int = logging.NOTSET,
+                     level: int = OTEL_LOG_LEVEL,
                      path: Optional[Path] = None,
                      stream: Optional[TextIO] = None,
                      ) -> logging.Handler:
     if path is not None and stream is not None:
         raise ValueError('cannot set both path and stream')
 
     if path is not None:
@@ -52,15 +53,15 @@
     handler.setFormatter(JsonFormatter())
     handler.setLevel(level)
     return handler
 
 
 @instrument_decorate
 def instrument_logging(*,
-                       level: int = logging.NOTSET,  # todo: support env var
+                       level: int = OTEL_LOG_LEVEL,
                        print_json: bool = True,
                        verbose: bool = True,
                        force_reinstrumentation: bool = False,
                        ) -> None:
     """
     this function is (by default) idempotent; calling it multiple times has no additional side effects
```

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/instrument_requests.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_requests.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/introspect.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/introspect.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/json_encoder.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/logging_json_formatter.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/logging_json_formatter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/opentelemetry_wrapper/utils/tracers.py` & `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/tracers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from functools import lru_cache
 from typing import Optional
 
 from opentelemetry import trace
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.resources import SERVICE_NAME
+from opentelemetry.sdk.resources import SERVICE_NAMESPACE
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace import Tracer
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter
 
 from opentelemetry_wrapper.config.config import OTEL_EXPORTER_OTLP_ENDPOINT
 from opentelemetry_wrapper.config.config import OTEL_SERVICE_NAME
+from opentelemetry_wrapper.config.config import OTEL_SERVICE_NAMESPACE
 
 
 @lru_cache  # only run once
 def init_tracer():
-    if OTEL_SERVICE_NAME:
-        tp = TracerProvider(resource=Resource.create({SERVICE_NAME: OTEL_SERVICE_NAME}))
+    if OTEL_SERVICE_NAMESPACE:
+        tp = TracerProvider(resource=Resource.create({SERVICE_NAME:      OTEL_SERVICE_NAME,
+                                                      SERVICE_NAMESPACE: OTEL_SERVICE_NAMESPACE}))
     else:
-        tp = TracerProvider()
+        tp = TracerProvider(resource=Resource.create({SERVICE_NAME: OTEL_SERVICE_NAME}))
 
     # noinspection PyProtectedMember
     trace._set_tracer_provider(tp, log=False)  # try to set, but don't warn otherwise
     if trace.get_tracer_provider() is tp:  # if we succeeded in setting it, set it up
         def format_span(span: ReadableSpan) -> str:
             return f'{span.to_json(indent=None)}\n'
```

### Comparing `opentelemetry_wrapper-0.0.8/pyproject.toml` & `opentelemetry_wrapper-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/setup_otel_logging.py` & `opentelemetry_wrapper-0.0.9/setup_otel_logging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.8/PKG-INFO` & `opentelemetry_wrapper-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry_wrapper
-Version: 0.0.8
+Version: 0.0.9
 Summary: a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 Author-email: Avery Khoo <averykhoo@gmail.com>
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: asgiref
 Requires-Dist: fastapi
@@ -41,21 +41,21 @@
 
 ## usage
 
 todo: write stuff here
 
 ## env vars
 
-| Variable Name                 | Description                                              | Default (if not set)                                                |
-|-------------------------------|----------------------------------------------------------|---------------------------------------------------------------------|
-| `OTEL_SERVICE_NAME`           | Sets the value of the `service.name` resource attribute. | f'{username}@{hostname}.{namespace or domain}:<{filename of main}>' |
-| `OTEL_RESOURCE_ATTRIBUTES`    | Key-value pairs to be used as resource attributes.       | *NA*                                                                |
-| TODO: `OTEL_LOG_LEVEL`        | Log level used by this logging instrumentor              | `NOTSET`                                                            |
-| `OTEL_WRAPPER_DISABLED`       | Set to `true` to disable everything globally             | `false`                                                             |
-| `OTEL_EXPORTER_OTLP_ENDPOINT` | Looks like `http://tempo.local:4317`                     | *NA*                                                                |
+| Variable Name                 | Description                                                             | Default (if not set)                                                |
+|-------------------------------|-------------------------------------------------------------------------|---------------------------------------------------------------------|
+| `OTEL_SERVICE_NAME`           | Sets the value of the `service.name` resource attribute.                | f'{username}@{hostname}.{namespace or domain}:<{filename of main}>' |
+| `OTEL_RESOURCE_ATTRIBUTES`    | Key-value pairs to be used as resource attributes.                      | *NA*                                                                |
+| `OTEL_LOG_LEVEL`              | Log level used by this logging instrumentor                             | `NOTSET`                                                            |
+| `OTEL_WRAPPER_DISABLED`       | Set to `true` to disable everything globally (e.g. when running pytest) | `false`                                                             |
+| `OTEL_EXPORTER_OTLP_ENDPOINT` | Looks like `http://tempo.local:4317`                                    | *NA*                                                                |
 
 
 ## read the original docs
 
 * [OpenTelemetry](https://opentelemetry.io/docs)
 * [OpenTracing](https://opentracing.io/docs)
 * [SkyWalking](https://skywalking.apache.org/docs/skywalking-python/latest/readme/)
```

