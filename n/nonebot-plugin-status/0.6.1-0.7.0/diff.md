# Comparing `tmp/nonebot_plugin_status-0.6.1.tar.gz` & `tmp/nonebot_plugin_status-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_status-0.6.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_status-0.7.0.tar", max compression
```

## Comparing `nonebot_plugin_status-0.6.1.tar` & `nonebot_plugin_status-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rwxr-xr-x   0        0        0     3430 2022-11-15 15:40:15.000000 nonebot_plugin_status-0.6.1/README.md
--rwxr-xr-x   0        0        0     2394 2022-11-15 15:40:15.000000 nonebot_plugin_status-0.6.1/__init__.py
--rwxr-xr-x   0        0        0      589 2022-11-15 15:40:15.000000 nonebot_plugin_status-0.6.1/common.py
--rwxr-xr-x   0        0        0     1337 2022-11-15 15:40:15.000000 nonebot_plugin_status-0.6.1/config.py
--rwxr-xr-x   0        0        0     2157 2022-12-17 08:45:10.000000 nonebot_plugin_status-0.6.1/data_source.py
--rwxr-xr-x   0        0        0      657 2022-11-15 15:40:15.000000 nonebot_plugin_status-0.6.1/helpers.py
--rwxr-xr-x   0        0        0     1058 2022-11-15 15:40:15.000000 nonebot_plugin_status-0.6.1/onebot_v11.py
--rwxr-xr-x   0        0        0     1018 2023-01-26 03:37:25.000000 nonebot_plugin_status-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 nonebot_plugin_status-0.6.1/setup.py
--rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 nonebot_plugin_status-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     3430 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/README.md
+-rw-r--r--   0        0        0     3204 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/common.py
+-rw-r--r--   0        0        0     1921 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/config.py
+-rw-r--r--   0        0        0     2530 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/data_source.py
+-rw-r--r--   0        0        0      679 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/helpers.py
+-rw-r--r--   0        0        0     1218 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/onebot_v11.py
+-rw-r--r--   0        0        0     1007 2023-06-05 08:15:10.223629 nonebot_plugin_status-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4637 1970-01-01 00:00:00.000000 nonebot_plugin_status-0.7.0/PKG-INFO
```

### Comparing `nonebot_plugin_status-0.6.1/README.md` & `nonebot_plugin_status-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_status-0.6.1/__init__.py` & `nonebot_plugin_status-0.7.0/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-09-18 00:00:13
 @LastEditors    : yanyongyu
-@LastEditTime   : 2022-10-25 07:35:00
-@Description    : None
+@LastEditTime   : 2023-03-30 19:58:02
+@Description    : Status plugin
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
 import contextlib
 from typing import Any, Dict
 
 from jinja2 import Environment
 from nonebot import get_driver
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
+from nonebot.plugin import PluginMetadata
 from jinja2.meta import find_undeclared_variables
 
 from .config import Config
 from .helpers import humanize_date, relative_time, humanize_delta
 from .data_source import (
     get_uptime,
     get_cpu_status,
@@ -28,14 +29,28 @@
     per_cpu_status,
     get_swap_status,
     get_memory_status,
     get_bot_connect_time,
     get_nonebot_run_time,
 )
 
+__plugin_meta__ = PluginMetadata(
+    name="服务器状态查看",
+    description="通过戳一戳获取服务器状态",
+    usage=(
+        "通过QQ私聊戳一戳或拍一拍头像获取机器人服务器状态\n"
+        "或者通过发送指令 `status/状态` 获取机器人服务器状态\n"
+        "可以通过配置文件修改服务器状态模板"
+    ),
+    type="application",
+    homepage="https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status",
+    config=Config,
+    supported_adapters=None,
+)
+
 global_config = get_driver().config
 status_config = Config.parse_obj(global_config)
 status_permission = (status_config.server_status_only_superusers or None) and SUPERUSER
 
 _ev = Environment(
     trim_blocks=True, lstrip_blocks=True, autoescape=False, enable_async=True
 )
@@ -56,30 +71,34 @@
     "memory_usage": get_memory_status,
     "swap_usage": get_swap_status,
     "disk_usage": get_disk_usage,
     "uptime": get_uptime,
     "runtime": get_nonebot_run_time,
     "bot_connect_time": get_bot_connect_time,
 }
+"""Available variables for template rendering."""
 
 
 def _solve_required_vars() -> Dict[str, Any]:
+    """Solve required variables for template rendering."""
     return (
         {k: v() for k, v in KNOWN_VARS.items() if k in _t_vars}
         if status_config.server_status_truncate
         else {k: v() for k, v in KNOWN_VARS.items()}
     )
 
 
 async def render_template() -> str:
+    """Render status template with required variables."""
     message = await _t.render_async(**_solve_required_vars())
     return message.strip("\n")
 
 
 async def server_status(matcher: Matcher):
+    """Server status matcher handler."""
     await matcher.send(message=await render_template())
 
 
 from . import common
 
 with contextlib.suppress(ImportError):
     import nonebot.adapters.onebot.v11
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_status-0.6.1/common.py` & `nonebot_plugin_status-0.7.0/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-09-18 00:00:13
 @LastEditors    : yanyongyu
-@LastEditTime   : 2022-10-15 09:39:14
-@Description    : None
+@LastEditTime   : 2023-03-30 18:26:14
+@Description    : Common text matcher for status plugin
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
 from nonebot import on_command
 
 from . import server_status, status_config, status_permission
@@ -18,7 +18,8 @@
     command = on_command(
         "status",
         aliases={"状态"},
         permission=status_permission,
         priority=10,
         handlers=[server_status],
     )
+    """`status`/`状态` command matcher"""
```

### Comparing `nonebot_plugin_status-0.6.1/config.py` & `nonebot_plugin_status-0.7.0/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-10-04 16:32:00
 @LastEditors    : yanyongyu
-@LastEditTime   : 2022-10-25 07:34:07
-@Description    : None
+@LastEditTime   : 2023-03-30 18:17:09
+@Description    : Config for status plugin
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
 
 from pydantic import Extra, BaseModel
 
-CPU_TEMPLATE = "CPU: {{ '%02d' % cpu_usage }}%"
+CPU_TEMPLATE = r"CPU: {{ '%02d' % cpu_usage }}%"
+"""Default CPU status template."""
+
 # PER_CPU_TEMPLATE = (
 #     "CPU:\n"
 #     "{%- for core in per_cpu_usage %}\n"
 #     "  core{{ loop.index }}: {{ '%02d' % core }}%\n"
 #     "{%- endfor %}"
 # )
-MEMORY_TEMPLATE = "Memory: {{ '%02d' % memory_usage.percent }}%"
+
+MEMORY_TEMPLATE = r"Memory: {{ '%02d' % memory_usage.percent }}%"
+"""Default memory status template."""
+
 SWAP_TEMPLATE = (
-    "{% if swap_usage.total %}Swap: {{ '%02d' % swap_usage.percent }}%{% endif %}"
+    r"{% if swap_usage.total %}Swap: {{ '%02d' % swap_usage.percent }}%{% endif %}"
 )
+"""Default swap status template."""
+
 DISK_TEMPLATE = (
     "Disk:\n"
     "{% for name, usage in disk_usage.items() %}\n"
     "  {{ name }}: {{ '%02d' % usage.percent }}%\n"
     "{% endfor %}"
 )
+"""Default disk status template."""
+
 UPTIME_TEMPLATE = "Uptime: {{ uptime | relative_time | humanize_delta }}"
+"""Default uptime status template."""
+
 RUNTIME_TEMPLATE = "Runtime: {{ runtime | relative_time | humanize_delta }}"
+"""Default runtime status template."""
 
 
 class Config(BaseModel, extra=Extra.ignore):
     server_status_enabled: bool = True
+    """Whether to enable the server status commands."""
     server_status_truncate: bool = True
+    """Whether to render the status template with used variables only."""
     server_status_only_superusers: bool = True
+    """Whether to allow only superusers to use the status commands."""
 
-    # template
     server_status_template: str = "\n".join(
         (CPU_TEMPLATE, MEMORY_TEMPLATE, RUNTIME_TEMPLATE, SWAP_TEMPLATE, DISK_TEMPLATE)
     )
+    """Default server status template.
+
+    Including:
+
+    - CPU usage
+    - Memory usage
+    - Runtime
+    - Swap usage
+    - Disk usage
+    """
```

### Comparing `nonebot_plugin_status-0.6.1/data_source.py` & `nonebot_plugin_status-0.7.0/data_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-09-18 00:15:21
 @LastEditors    : yanyongyu
-@LastEditTime   : 2022-12-17 16:45:10
-@Description    : None
+@LastEditTime   : 2023-03-30 18:23:38
+@Description    : Getting status of the bot and the mechine
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Dict, List, Optional
 
@@ -43,52 +43,59 @@
 
 @driver.on_bot_disconnect
 async def _(bot: Bot):
     _bot_connect_time.pop(bot.self_id, None)
 
 
 def get_nonebot_run_time() -> datetime:
+    """Get the time when NoneBot started running."""
     try:
         return _nonebot_run_time
     except NameError:
         raise RuntimeError("NoneBot not running!") from None
 
 
 def get_bot_connect_time() -> Dict[str, datetime]:
+    """Get the time when the bot connected to the server."""
     return _bot_connect_time
 
 
-# mechine status
 def get_cpu_status() -> float:
+    """Get the CPU usage status."""
     return psutil.cpu_percent(interval=0.3)  # type: ignore
 
 
 def per_cpu_status() -> List[float]:
+    """Get the CPU usage status of each core."""
     return psutil.cpu_percent(interval=0.3, percpu=True)  # type: ignore
 
 
 def get_memory_status():
+    """Get the memory usage status."""
     return psutil.virtual_memory()
 
 
 def get_swap_status():
+    """Get the swap usage status."""
     return psutil.swap_memory()
 
 
 def _get_disk_usage(path: str) -> Optional["sdiskusage"]:
     try:
         return psutil.disk_usage(path)
     except Exception as e:
         logger.warning(f"Could not get disk usage for {path}: {e!r}")
 
 
 def get_disk_usage() -> Dict[str, "sdiskusage"]:
+    """Get the disk usage status."""
     disk_parts = psutil.disk_partitions()
     return {
         d.mountpoint: usage
         for d in disk_parts
         if (usage := _get_disk_usage(d.mountpoint))
     }
 
 
 def get_uptime() -> datetime:
+    """Get the uptime of the mechine."""
     return datetime.fromtimestamp(psutil.boot_time(), tz=CURRENT_TIMEZONE)
```

### Comparing `nonebot_plugin_status-0.6.1/helpers.py` & `nonebot_plugin_status-0.7.0/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2022-10-15 08:08:41
 @LastEditors    : yanyongyu
-@LastEditTime   : 2022-10-15 12:00:21
-@Description    : None
+@LastEditTime   : 2023-03-30 18:24:49
+@Description    : Template rendering helpers
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
 
 from datetime import datetime, timedelta
```

### Comparing `nonebot_plugin_status-0.6.1/pyproject.toml` & `nonebot_plugin_status-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "nonebot-plugin-status"
-version = "0.6.1"
+version = "0.7.0"
 description = "Check your server status (CPU, Memory, Disk Usage) via nonebot"
 license = "MIT"
-authors = ["yanyongyu <yanyongyu_1@126.com>"]
+authors = ["yanyongyu <yyy@nonebot.dev>"]
 readme = "README.md"
 homepage = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status"
 repository = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status"
 documentation = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status#readme"
 keywords = ["nonebot", "nonebot2", "server", "status"]
 packages = [
     { include = "nonebot_plugin_status/*.py", from = ".." }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 psutil = "^5.7.2"
 Jinja2 = "^3.0.0"
 humanize = "^4.0.0"
-nonebot2 = "^2.0.0-beta.1"
+nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = { version = "^2.0.0-beta.1", optional = true }
 
 [tool.poetry.extras]
 onebot = ["nonebot-adapter-onebot"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_status-0.6.1/setup.py` & `nonebot_plugin_status-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,133 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-status
+Version: 0.7.0
+Summary: Check your server status (CPU, Memory, Disk Usage) via nonebot
+Home-page: https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status
+License: MIT
+Keywords: nonebot,nonebot2,server,status
+Author: yanyongyu
+Author-email: yyy@nonebot.dev
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: onebot
+Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
+Requires-Dist: humanize (>=4.0.0,<5.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0) ; extra == "onebot"
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: psutil (>=5.7.2,<6.0.0)
+Project-URL: Documentation, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status#readme
+Project-URL: Repository, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status
+Description-Content-Type: text/markdown
+
+<!--
+ * @Author         : yanyongyu
+ * @Date           : 2020-11-15 14:40:25
+ * @LastEditors    : yanyongyu
+ * @LastEditTime   : 2022-11-05 16:13:36
+ * @Description    : None
+ * @GitHub         : https://github.com/yanyongyu
+-->
+
+<!-- markdownlint-disable MD033 MD036 MD041 -->
+
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
+
+<div align="center">
+
+# nonebot-plugin-status
+
+_✨ NoneBot 服务器状态（CPU, Memory, Disk Usage）查看插件 ✨_
+
+</div>
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">
+    <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-status">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-status.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
+</p>
+
+## 使用方式
+
+通用:
+
+- 发送 Command `状态` 或者 `status`
+
+OneBot:
+
+- 向机器人发送戳一戳表情
+- 双击机器人头像戳一戳
+
+## 配置项
+
+> **warning**
+> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.org/project/nonebot-plugin-status/) 上的文档。
+
+配置方式：直接在 NoneBot 全局配置文件中添加以下配置项即可。
+
+### server_status_enabled
+
+- 类型：`bool`
+- 默认值：`True`
+- 说明：是否启用服务器状态查看功能
+
+### server_status_truncate
+
+- 类型：`bool`
+- 默认值：`True`
+- 说明：是否启用模板变量按需注入功能（节约时间）
+
+### server_status_only_superusers
+
+- 类型: `bool`
+- 默认: `True`
+- 说明: 是否仅允许超级用户使用
+
+> 超级用户需在配置文件中如下配置:
+>
+> ```dotenv
+> SUPERUSERS=["your qq id"]
+> ```
+
+### server_status_template
+
+- 类型: `str`
+- 默认: 请参考示例
+- 说明：发送的消息模板，支持的方法、变量以及类型如下：
+  - relative_time (`Callable[[datetime], timedelta]`): 获取相对时间
+  - humanize_date (`Callable[[datetime], str]`): [人性化时间](https://python-humanize.readthedocs.io/en/latest/time/#humanize.time.naturaldate)
+  - humanize_delta (`Callable[[timedelta], str]`): [人性化时间差](https://python-humanize.readthedocs.io/en/latest/time/#humanize.time.precisiondelta)
+  - cpu_usage (`float`): CPU 使用率
+  - per_cpu_usage (`List[float]`): 每个 CPU 核心的使用率
+  - memory_usage (`svmem`): 内存使用情况，包含 total, available, percent, used, free(, active, inactive, buffers, cached, shared) 属性
+  - swap_usage (`sswap`): 内存使用情况，包含 total, used, free, percent, sin, sout 属性
+  - disk_usage (`Dict[str, psutil._common.sdiskusage]`): 磁盘使用率，包含 total, used, free, percent 属性
+  - uptime (`datetime`): 服务器运行时间
+  - runtime (`datetime`): NoneBot 运行时间
+  - bot_connect_time (`Dict[str, datetime]`): 机器人连接时间
+
+配置文件示例（默认模板）
+
+```dotenv
+SERVER_STATUS_TEMPLATE='
+CPU: {{ "%02d" % cpu_usage }}%
+Memory: {{ "%02d" % memory_usage.percent }}%
+Runtime: {{ runtime | relative_time | humanize_delta }}
+{% if swap_usage.total %}Swap: {{ "%02d" % swap_usage.percent }}%{% endif %}
+Disk:
+{% for name, usage in disk_usage.items() %}
+  {{ name }}: {{ "%02d" % usage.percent }}%
+{% endfor %}
+'
+```
 
-package_dir = \
-{'': '..'}
-
-packages = \
-['nonebot_plugin_status']
-
-package_data = \
-{'': ['*'], 'nonebot_plugin_status': ['dist/*']}
-
-install_requires = \
-['Jinja2>=3.0.0,<4.0.0',
- 'humanize>=4.0.0,<5.0.0',
- 'nonebot2>=2.0.0-beta.1,<3.0.0',
- 'psutil>=5.7.2,<6.0.0']
-
-extras_require = \
-{'onebot': ['nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-status',
-    'version': '0.6.1',
-    'description': 'Check your server status (CPU, Memory, Disk Usage) via nonebot',
-    'long_description': '<!--\n * @Author         : yanyongyu\n * @Date           : 2020-11-15 14:40:25\n * @LastEditors    : yanyongyu\n * @LastEditTime   : 2022-11-05 16:13:36\n * @Description    : None\n * @GitHub         : https://github.com/yanyongyu\n-->\n\n<!-- markdownlint-disable MD033 MD036 MD041 -->\n\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot-plugin-status\n\n_✨ NoneBot 服务器状态（CPU, Memory, Disk Usage）查看插件 ✨_\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">\n    <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-status">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-status.svg" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">\n</p>\n\n## 使用方式\n\n通用:\n\n- 发送 Command `状态` 或者 `status`\n\nOneBot:\n\n- 向机器人发送戳一戳表情\n- 双击机器人头像戳一戳\n\n## 配置项\n\n> **warning**\n> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.org/project/nonebot-plugin-status/) 上的文档。\n\n配置方式：直接在 NoneBot 全局配置文件中添加以下配置项即可。\n\n### server_status_enabled\n\n- 类型：`bool`\n- 默认值：`True`\n- 说明：是否启用服务器状态查看功能\n\n### server_status_truncate\n\n- 类型：`bool`\n- 默认值：`True`\n- 说明：是否启用模板变量按需注入功能（节约时间）\n\n### server_status_only_superusers\n\n- 类型: `bool`\n- 默认: `True`\n- 说明: 是否仅允许超级用户使用\n\n> 超级用户需在配置文件中如下配置:\n>\n> ```dotenv\n> SUPERUSERS=["your qq id"]\n> ```\n\n### server_status_template\n\n- 类型: `str`\n- 默认: 请参考示例\n- 说明：发送的消息模板，支持的方法、变量以及类型如下：\n  - relative_time (`Callable[[datetime], timedelta]`): 获取相对时间\n  - humanize_date (`Callable[[datetime], str]`): [人性化时间](https://python-humanize.readthedocs.io/en/latest/time/#humanize.time.naturaldate)\n  - humanize_delta (`Callable[[timedelta], str]`): [人性化时间差](https://python-humanize.readthedocs.io/en/latest/time/#humanize.time.precisiondelta)\n  - cpu_usage (`float`): CPU 使用率\n  - per_cpu_usage (`List[float]`): 每个 CPU 核心的使用率\n  - memory_usage (`svmem`): 内存使用情况，包含 total, available, percent, used, free(, active, inactive, buffers, cached, shared) 属性\n  - swap_usage (`sswap`): 内存使用情况，包含 total, used, free, percent, sin, sout 属性\n  - disk_usage (`Dict[str, psutil._common.sdiskusage]`): 磁盘使用率，包含 total, used, free, percent 属性\n  - uptime (`datetime`): 服务器运行时间\n  - runtime (`datetime`): NoneBot 运行时间\n  - bot_connect_time (`Dict[str, datetime]`): 机器人连接时间\n\n配置文件示例（默认模板）\n\n```dotenv\nSERVER_STATUS_TEMPLATE=\'\nCPU: {{ "%02d" % cpu_usage }}%\nMemory: {{ "%02d" % memory_usage.percent }}%\nRuntime: {{ runtime | relative_time | humanize_delta }}\n{% if swap_usage.total %}Swap: {{ "%02d" % swap_usage.percent }}%{% endif %}\nDisk:\n{% for name, usage in disk_usage.items() %}\n  {{ name }}: {{ "%02d" % usage.percent }}%\n{% endfor %}\n\'\n```\n',
-    'author': 'yanyongyu',
-    'author_email': 'yanyongyu_1@126.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,57 +1,55 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': '..'}
-packages = \ ['nonebot_plugin_status'] package_data = \ {'': ['*'],
-'nonebot_plugin_status': ['dist/*']} install_requires = \
-['Jinja2>=3.0.0,<4.0.0', 'humanize>=4.0.0,<5.0.0', 'nonebot2>=2.0.0-
-beta.1,<3.0.0', 'psutil>=5.7.2,<6.0.0'] extras_require = \ {'onebot':
-['nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0']} setup_kwargs = { 'name':
-'nonebot-plugin-status', 'version': '0.6.1', 'description': 'Check your server
-status (CPU, Memory, Disk Usage) via nonebot', 'long_description': '\n\n\n\n
-                                \n [nonebot]\n
-\n\n
-\n\n# nonebot-plugin-status\n\n_â¨ NoneBot æå¡å¨ç¶æï¼CPU, Memory, Disk
-                         Usageï¼æ¥çæä»¶ â¨_\n\n
-\n\n
-                 \n \n_[license]\n\n \n_[pypi]\n\n [python]\n
-\n\n## ä½¿ç¨æ¹å¼\n\néç¨:\n\n- åé Command `ç¶æ` æè
-`status`\n\nOneBot:\n\n- åæºå¨äººåéæ³ä¸æ³è¡¨æ\n-
-åå»æºå¨äººå¤´åæ³ä¸æ³\n\n## éç½®é¡¹\n\n> **warning**\n> GitHub
-ä»åºä¸­çææ¡£ä¸ºææ° DEV çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://
-pypi.org/project/nonebot-plugin-status/
-) ä¸çææ¡£ã\n\néç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
-å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã\n\n###
-server_status_enabled\n\n- ç±»åï¼`bool`\n- é»è®¤å¼ï¼`True`\n-
-è¯´æï¼æ¯å¦å¯ç¨æå¡å¨ç¶ææ¥çåè½\n\n###
-server_status_truncate\n\n- ç±»åï¼`bool`\n- é»è®¤å¼ï¼`True`\n-
-è¯´æï¼æ¯å¦å¯ç¨æ¨¡æ¿åéæéæ³¨å¥åè½ï¼èçº¦æ¶é´ï¼\n\n###
-server_status_only_superusers\n\n- ç±»å: `bool`\n- é»è®¤: `True`\n- è¯´æ:
-æ¯å¦ä»åè®¸è¶çº§ç¨æ·ä½¿ç¨\n\n>
-è¶çº§ç¨æ·éå¨éç½®æä»¶ä¸­å¦ä¸éç½®:\n>\n> ```dotenv\n> SUPERUSERS=
-["your qq id"]\n> ```\n\n### server_status_template\n\n- ç±»å: `str`\n-
-é»è®¤: è¯·åèç¤ºä¾\n-
-è¯´æï¼åéçæ¶æ¯æ¨¡æ¿ï¼æ¯æçæ¹æ³ãåéä»¥åç±»åå¦ä¸ï¼\n
-- relative_time (`Callable[[datetime], timedelta]`): è·åç¸å¯¹æ¶é´\n -
+Metadata-Version: 2.1 Name: nonebot-plugin-status Version: 0.7.0 Summary: Check
+your server status (CPU, Memory, Disk Usage) via nonebot Home-page: https://
+github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status
+License: MIT Keywords: nonebot,nonebot2,server,status Author: yanyongyu Author-
+email: yyy@nonebot.dev Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: onebot
+Requires-Dist: Jinja2 (>=3.0.0,<4.0.0) Requires-Dist: humanize (>=4.0.0,<5.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0) ; extra ==
+"onebot" Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: psutil
+(>=5.7.2,<6.0.0) Project-URL: Documentation, https://github.com/cscs181/QQ-
+GitHub-Bot/tree/master/src/plugins/nonebot_plugin_status#readme Project-URL:
+Repository, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/
+nonebot_plugin_status Description-Content-Type: text/markdown
+                                   [nonebot]
+   # nonebot-plugin-status _â¨ NoneBot æå¡å¨ç¶æï¼CPU, Memory, Disk
+                           Usageï¼æ¥çæä»¶ â¨_
+                           [license] [pypi] [python]
+## ä½¿ç¨æ¹å¼ éç¨: - åé Command `ç¶æ` æè `status` OneBot: -
+åæºå¨äººåéæ³ä¸æ³è¡¨æ - åå»æºå¨äººå¤´åæ³ä¸æ³ ## éç½®é¡¹
+> **warning** > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
+çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.org/project/nonebot-plugin-
+status/) ä¸çææ¡£ã éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
+å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### server_status_enabled -
+ç±»åï¼`bool` - é»è®¤å¼ï¼`True` -
+è¯´æï¼æ¯å¦å¯ç¨æå¡å¨ç¶ææ¥çåè½ ### server_status_truncate -
+ç±»åï¼`bool` - é»è®¤å¼ï¼`True` -
+è¯´æï¼æ¯å¦å¯ç¨æ¨¡æ¿åéæéæ³¨å¥åè½ï¼èçº¦æ¶é´ï¼ ###
+server_status_only_superusers - ç±»å: `bool` - é»è®¤: `True` - è¯´æ:
+æ¯å¦ä»åè®¸è¶çº§ç¨æ·ä½¿ç¨ >
+è¶çº§ç¨æ·éå¨éç½®æä»¶ä¸­å¦ä¸éç½®: > > ```dotenv > SUPERUSERS=
+["your qq id"] > ``` ### server_status_template - ç±»å: `str` - é»è®¤:
+è¯·åèç¤ºä¾ -
+è¯´æï¼åéçæ¶æ¯æ¨¡æ¿ï¼æ¯æçæ¹æ³ãåéä»¥åç±»åå¦ä¸ï¼
+- relative_time (`Callable[[datetime], timedelta]`): è·åç¸å¯¹æ¶é´ -
 humanize_date (`Callable[[datetime], str]`): [äººæ§åæ¶é´](https://python-
-humanize.readthedocs.io/en/latest/time/#humanize.time.naturaldate)\n -
+humanize.readthedocs.io/en/latest/time/#humanize.time.naturaldate) -
 humanize_delta (`Callable[[timedelta], str]`): [äººæ§åæ¶é´å·®](https://
-python-humanize.readthedocs.io/en/latest/time/#humanize.time.precisiondelta)\n
-- cpu_usage (`float`): CPU ä½¿ç¨ç\n - per_cpu_usage (`List[float]`): æ¯ä¸ª
-CPU æ ¸å¿çä½¿ç¨ç\n - memory_usage (`svmem`): åå­ä½¿ç¨æåµï¼åå«
-total, available, percent, used, free(, active, inactive, buffers, cached,
-shared) å±æ§\n - swap_usage (`sswap`): åå­ä½¿ç¨æåµï¼åå« total,
-used, free, percent, sin, sout å±æ§\n - disk_usage (`Dict[str,
+python-humanize.readthedocs.io/en/latest/time/#humanize.time.precisiondelta) -
+cpu_usage (`float`): CPU ä½¿ç¨ç - per_cpu_usage (`List[float]`): æ¯ä¸ª CPU
+æ ¸å¿çä½¿ç¨ç - memory_usage (`svmem`): åå­ä½¿ç¨æåµï¼åå« total,
+available, percent, used, free(, active, inactive, buffers, cached, shared)
+å±æ§ - swap_usage (`sswap`): åå­ä½¿ç¨æåµï¼åå« total, used, free,
+percent, sin, sout å±æ§ - disk_usage (`Dict[str,
 psutil._common.sdiskusage]`): ç£çä½¿ç¨çï¼åå« total, used, free,
-percent å±æ§\n - uptime (`datetime`): æå¡å¨è¿è¡æ¶é´\n - runtime
-(`datetime`): NoneBot è¿è¡æ¶é´\n - bot_connect_time (`Dict[str,
-datetime]`):
-æºå¨äººè¿æ¥æ¶é´\n\néç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼\n\n```dotenv\nSERVER_STATUS_TEMPLATE=\'\nCPU:
-{{ "%02d" % cpu_usage }}%\nMemory: {{ "%02d" % memory_usage.percent
-}}%\nRuntime: {{ runtime | relative_time | humanize_delta }}\n{% if
-swap_usage.total %}Swap: {{ "%02d" % swap_usage.percent }}%{% endif %}\nDisk:\n
-{% for name, usage in disk_usage.items() %}\n {{ name }}: {{ "%02d" %
-usage.percent }}%\n{% endfor %}\n\'\n```\n', 'author': 'yanyongyu',
-'author_email': 'yanyongyu_1@126.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/cscs181/QQ-GitHub-Bot/
-tree/master/src/plugins/nonebot_plugin_status', 'package_dir': package_dir,
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'extras_require': extras_require, 'python_requires':
-'>=3.8,<4.0', } setup(**setup_kwargs)
+percent å±æ§ - uptime (`datetime`): æå¡å¨è¿è¡æ¶é´ - runtime
+(`datetime`): NoneBot è¿è¡æ¶é´ - bot_connect_time (`Dict[str, datetime]`):
+æºå¨äººè¿æ¥æ¶é´ éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv
+SERVER_STATUS_TEMPLATE=' CPU: {{ "%02d" % cpu_usage }}% Memory: {{ "%02d" %
+memory_usage.percent }}% Runtime: {{ runtime | relative_time | humanize_delta
+}} {% if swap_usage.total %}Swap: {{ "%02d" % swap_usage.percent }}%{% endif %}
+Disk: {% for name, usage in disk_usage.items() %} {{ name }}: {{ "%02d" %
+usage.percent }}% {% endfor %} ' ```
```

