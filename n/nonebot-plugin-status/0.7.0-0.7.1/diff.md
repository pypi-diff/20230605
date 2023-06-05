# Comparing `tmp/nonebot_plugin_status-0.7.0.tar.gz` & `tmp/nonebot_plugin_status-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_status-0.7.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_status-0.7.1.tar", max compression
```

## Comparing `nonebot_plugin_status-0.7.0.tar` & `nonebot_plugin_status-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3430 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/README.md
--rw-r--r--   0        0        0     3204 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/__init__.py
--rw-r--r--   0        0        0      666 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/common.py
--rw-r--r--   0        0        0     1921 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/config.py
--rw-r--r--   0        0        0     2530 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/data_source.py
--rw-r--r--   0        0        0      679 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/helpers.py
--rw-r--r--   0        0        0     1218 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/onebot_v11.py
--rw-r--r--   0        0        0     1007 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4637 1970-01-01 00:00:00.000000 nonebot_plugin_status-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3430 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/README.md
+-rw-r--r--   0        0        0     3608 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/common.py
+-rw-r--r--   0        0        0     1921 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/config.py
+-rw-r--r--   0        0        0     2634 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/data_source.py
+-rw-r--r--   0        0        0      679 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/helpers.py
+-rw-r--r--   0        0        0     1218 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/onebot_v11.py
+-rw-r--r--   0        0        0     1007 2023-06-05 08:54:25.901338 nonebot_plugin_status-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4637 1970-01-01 00:00:00.000000 nonebot_plugin_status-0.7.1/PKG-INFO
```

### Comparing `nonebot_plugin_status-0.7.0/README.md` & `nonebot_plugin_status-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_status-0.7.0/__init__.py` & `nonebot_plugin_status-0.7.1/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-09-18 00:00:13
 @LastEditors    : yanyongyu
-@LastEditTime   : 2023-03-30 19:58:02
+@LastEditTime   : 2023-06-05 16:43:31
 @Description    : Status plugin
 @GitHub         : https://github.com/yanyongyu
 """
+
 __author__ = "yanyongyu"
 
+import inspect
 import contextlib
 from typing import Any, Dict
 
 from jinja2 import Environment
 from nonebot import get_driver
+from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
 from jinja2.meta import find_undeclared_variables
 
 from .config import Config
 from .helpers import humanize_date, relative_time, humanize_delta
@@ -74,26 +77,39 @@
     "uptime": get_uptime,
     "runtime": get_nonebot_run_time,
     "bot_connect_time": get_bot_connect_time,
 }
 """Available variables for template rendering."""
 
 
-def _solve_required_vars() -> Dict[str, Any]:
+if not set(_t_vars).issubset(KNOWN_VARS):
+    raise ValueError(
+        f'Unknown variables in status template: {", ".join(set(_t_vars) - set(KNOWN_VARS))}'
+    )
+
+
+async def _solve_required_vars() -> Dict[str, Any]:
     """Solve required variables for template rendering."""
     return (
-        {k: v() for k, v in KNOWN_VARS.items() if k in _t_vars}
+        {
+            k: await v() if inspect.iscoroutinefunction(v) else v()
+            for k, v in KNOWN_VARS.items()
+            if k in _t_vars
+        }
         if status_config.server_status_truncate
-        else {k: v() for k, v in KNOWN_VARS.items()}
+        else {
+            k: await v() if inspect.iscoroutinefunction(v) else v()
+            for k, v in KNOWN_VARS.items()
+        }
     )
 
 
 async def render_template() -> str:
     """Render status template with required variables."""
-    message = await _t.render_async(**_solve_required_vars())
+    message = await _t.render_async(**(await _solve_required_vars()))
     return message.strip("\n")
 
 
 async def server_status(matcher: Matcher):
     """Server status matcher handler."""
     await matcher.send(message=await render_template())
```

### Comparing `nonebot_plugin_status-0.7.0/common.py` & `nonebot_plugin_status-0.7.1/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_status-0.7.0/config.py` & `nonebot_plugin_status-0.7.1/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_status-0.7.0/data_source.py` & `nonebot_plugin_status-0.7.1/data_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-09-18 00:15:21
 @LastEditors    : yanyongyu
-@LastEditTime   : 2023-03-30 18:23:38
+@LastEditTime   : 2023-06-05 16:40:35
 @Description    : Getting status of the bot and the mechine
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
+import asyncio
 from datetime import datetime
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 import psutil
 from nonebot import get_driver
 from nonebot.log import logger
 from nonebot.adapters import Bot
@@ -55,22 +56,26 @@
 
 
 def get_bot_connect_time() -> Dict[str, datetime]:
     """Get the time when the bot connected to the server."""
     return _bot_connect_time
 
 
-def get_cpu_status() -> float:
+async def get_cpu_status() -> float:
     """Get the CPU usage status."""
-    return psutil.cpu_percent(interval=0.3)  # type: ignore
+    psutil.cpu_percent()
+    await asyncio.sleep(0.5)
+    return psutil.cpu_percent()
 
 
-def per_cpu_status() -> List[float]:
+async def per_cpu_status() -> List[float]:
     """Get the CPU usage status of each core."""
-    return psutil.cpu_percent(interval=0.3, percpu=True)  # type: ignore
+    psutil.cpu_percent(percpu=True)
+    await asyncio.sleep(0.5)
+    return psutil.cpu_percent(percpu=True)  # type: ignore
 
 
 def get_memory_status():
     """Get the memory usage status."""
     return psutil.virtual_memory()
```

### Comparing `nonebot_plugin_status-0.7.0/helpers.py` & `nonebot_plugin_status-0.7.1/helpers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_status-0.7.0/onebot_v11.py` & `nonebot_plugin_status-0.7.1/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_status-0.7.0/pyproject.toml` & `nonebot_plugin_status-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-status"
-version = "0.7.0"
+version = "0.7.1"
 description = "Check your server status (CPU, Memory, Disk Usage) via nonebot"
 license = "MIT"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 readme = "README.md"
 homepage = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status"
 repository = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status"
 documentation = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status#readme"
```

### Comparing `nonebot_plugin_status-0.7.0/PKG-INFO` & `nonebot_plugin_status-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-status
-Version: 0.7.0
+Version: 0.7.1
 Summary: Check your server status (CPU, Memory, Disk Usage) via nonebot
 Home-page: https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status
 License: MIT
 Keywords: nonebot,nonebot2,server,status
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-status Version: 0.7.0 Summary: Check
+Metadata-Version: 2.1 Name: nonebot-plugin-status Version: 0.7.1 Summary: Check
 your server status (CPU, Memory, Disk Usage) via nonebot Home-page: https://
 github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status
 License: MIT Keywords: nonebot,nonebot2,server,status Author: yanyongyu Author-
 email: yyy@nonebot.dev Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

