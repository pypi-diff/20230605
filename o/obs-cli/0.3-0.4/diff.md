# Comparing `tmp/obs-cli-0.3.tar.gz` & `tmp/obs-cli-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.3.tar", last modified: Mon Jun  5 15:17:35 2023, max compression
+gzip compressed data, was "obs-cli-0.4.tar", last modified: Mon Jun  5 15:52:17 2023, max compression
```

## Comparing `obs-cli-0.3.tar` & `obs-cli-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:17:24.000000 obs-cli-0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 15:17:24.000000 obs-cli-0.3/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 15:17:24.000000 obs-cli-0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 15:17:24.000000 obs-cli-0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 15:17:24.000000 obs-cli-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:17:35.291198 obs-cli-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 15:17:24.000000 obs-cli-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-05 15:17:24.000000 obs-cli-0.3/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-05 15:17:24.000000 obs-cli-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:17:35.291198 obs-cli-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:52:17.365801 obs-cli-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:52:17.365801 obs-cli-0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:52:07.000000 obs-cli-0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:52:17.365801 obs-cli-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 15:52:07.000000 obs-cli-0.4/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 15:52:07.000000 obs-cli-0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 15:52:07.000000 obs-cli-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 15:52:07.000000 obs-cli-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:52:17.365801 obs-cli-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 15:52:07.000000 obs-cli-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:52:17.365801 obs-cli-0.4/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:52:17.000000 obs-cli-0.4/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:52:17.000000 obs-cli-0.4/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:52:17.000000 obs-cli-0.4/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 15:52:17.000000 obs-cli-0.4/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 15:52:17.000000 obs-cli-0.4/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 15:52:17.000000 obs-cli-0.4/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-05 15:52:07.000000 obs-cli-0.4/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-05 15:52:07.000000 obs-cli-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:52:17.365801 obs-cli-0.4/setup.cfg
```

### Comparing `obs-cli-0.3/.github/workflows/release.yaml` & `obs-cli-0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.3/LICENSE` & `obs-cli-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.3/PKG-INFO` & `obs-cli-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.3
+Version: 0.4
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.3/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.4/obs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.3
+Version: 0.4
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.3/obs_cli.py` & `obs-cli-0.4/obs_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import argparse
 import logging
+import os
 import re
 import sys
 
 import obsws_python as obs
 from rich import print, print_json
 from rich.console import Console
 from rich.table import Table
@@ -15,15 +16,17 @@
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("-D", "--debug", action="store_true", default=False)
     parser.add_argument("-H", "--host", help="host name", default="localhost")
     parser.add_argument(
         "-P", "--port", help="port number", type=int, default=4455
     )
-    parser.add_argument("-p", "--password", help="password")
+    parser.add_argument(
+        "-p", "--password", required=False, help="password ($OBS_API_PASSWORD)"
+    )
     parser.add_argument("-j", "--json", action="store_true", default=False)
 
     subparsers = parser.add_subparsers(dest="command")
 
     scene_parser = subparsers.add_parser("scene")
     scene_parser.add_argument(
         "-e", "--exact", action="store_true", default=False, help="Exact match"
@@ -62,14 +65,24 @@
         default="show",
         help="list/show",
     )
     input_parser.add_argument("INPUT", nargs="?", help="Input name")
     input_parser.add_argument("PROPERTY", nargs="?", help="Property name")
     input_parser.add_argument("VALUE", nargs="?", help="Property value")
 
+    filter_parser = subparsers.add_parser("filter")
+    filter_parser.add_argument(
+        "action",
+        choices=["list", "toggle", "enable", "disable", "status"],
+        default="list",
+        help="list/toggle/enable/disable/status",
+    )
+    filter_parser.add_argument("INPUT", nargs="?", help="Input name")
+    filter_parser.add_argument("FILTER", nargs="?", help="Filter name")
+
     return parser.parse_args()
 
 
 def switch_to_scene(cl, scene, exact=False, ignorecase=True):
     regex = re.compile(
         f"^{scene}$" if exact else scene,
         re.IGNORECASE if ignorecase else re.NOFLAG,
@@ -151,38 +164,61 @@
     return cl.get_input_settings(input).input_settings
 
 
 def set_input_setting(cl, input, key, value):
     return cl.set_input_settings(input, {key: value}, overlay=True)
 
 
+def get_filters(cl, input):
+    return cl.get_source_filter_list(input).filters
+
+
+def is_filter_enabled(cl, source, filter):
+    return cl.get_source_filter(source, filter).filter_enabled
+
+
+def enable_filter(cl, source, filter):
+    return cl.set_source_filter_enabled(source, filter, True)
+
+
+def disable_filter(cl, source, filter):
+    return cl.set_source_filter_enabled(source, filter, False)
+
+
+def toggle_filter(cl, source, filter):
+    enabled = is_filter_enabled(cl, source, filter)
+    return cl.set_source_filter_enabled(source, filter, not enabled)
+
+
 def main():
     console = Console()
     logging.basicConfig()
 
     args = parse_args()
     LOGGER.setLevel(logging.DEBUG if args.debug else logging.INFO)
     LOGGER.debug(args)
 
+    password = args.password or os.environ.get("OBS_API_PASSWORD")
+
     try:
-        cl = obs.ReqClient(
-            host=args.host, port=args.port, password=args.password
-        )
+        cl = obs.ReqClient(host=args.host, port=args.port, password=password)
 
         cmd = args.command
         if cmd == "scene":
             if args.action == "current":
                 print(get_current_scene_name(cl))
             elif args.action == "list":
                 res = cl.get_scene_list()
                 print(
                     *sorted([x.get("sceneName") for x in res.scenes]), sep="\n"
                 )
+                LOGGER.debug(res)
             elif args.action == "switch":
-                switch_to_scene(cl, args.SCENE, exact=False)
+                res = switch_to_scene(cl, args.SCENE, exact=False)
+                LOGGER.debug(res)
             else:
                 print(get_current_scene_name(cl))
 
         elif cmd == "item":
             if args.action == "list":
                 # print(*get_items(cl, args.scene), sep="\n")
                 scene = args.scene or get_current_scene_name(cl)
@@ -199,19 +235,23 @@
                 for item in data:
                     item_id = str(item.get("sceneItemId"))
                     name = item.get("sourceName")
                     enabled = "✅" if item.get("sceneItemEnabled") else "❌"
                     table.add_row(item_id, name, enabled)
                 console.print(table)
             elif args.action == "toggle":
-                toggle_item(cl, args.ITEM, args.scene)
+                res = toggle_item(cl, args.ITEM, args.scene)
+                LOGGER.debug(res)
             elif args.action == "show":
-                show_item(cl, args.ITEM, args.scene)
+                res = show_item(cl, args.ITEM, args.scene)
+                LOGGER.debug(res)
             elif args.action == "hide":
-                hide_item(cl, args.ITEM, args.scene)
+                res = hide_item(cl, args.ITEM, args.scene)
+                LOGGER.debug(res)
+
         elif cmd == "input":
             if args.action == "list":
                 data = get_inputs(cl)
                 if args.json:
                     print_json(data=data)
                     return
 
@@ -229,15 +269,47 @@
                     print(data.get(args.PROPERTY))
                 else:
                     # TODO Implement rich table output
                     print_json(data=data)
             elif args.action == "set":
                 if not args.INPUT or not args.PROPERTY or not args.VALUE:
                     raise ValueError("Missing input name, property or value")
-                set_input_setting(cl, args.INPUT, args.PROPERTY, args.VALUE)
+                res = set_input_setting(
+                    cl, args.INPUT, args.PROPERTY, args.VALUE
+                )
+                LOGGER.debug(res)
+
+        elif cmd == "filter":
+            if args.action == "list":
+                data = get_filters(cl, args.INPUT)
+                if args.json:
+                    print_json(data=data)
+                    return
+                table = Table(title=f"Filters for {args.INPUT}")
+                table.add_column("Kind")
+                table.add_column("Name")
+                table.add_column("Enabled", justify="center")
+                for filter in data:
+                    kind = filter.get("filterKind")
+                    name = filter.get("filterName")
+                    enabled = "✅" if filter.get("filterEnabled") else "❌"
+                    table.add_row(kind, name, enabled)
+                console.print(table)
+            elif args.action == "toggle":
+                res = toggle_filter(cl, args.INPUT, args.FILTER)
+                LOGGER.debug(res)
+            elif args.action == "enable":
+                res = enable_filter(cl, args.INPUT, args.FILTER)
+                LOGGER.debug(res)
+            elif args.action == "disable":
+                res = disable_filter(cl, args.INPUT, args.FILTER)
+                LOGGER.debug(res)
+            elif args.action == "status":
+                res = is_filter_enabled(cl, args.INPUT, args.FILTER)
+                LOGGER.debug(res)
 
         return 0
     except Exception:
         console.print_exception(show_locals=True)
         return 1
```

### Comparing `obs-cli-0.3/pyproject.toml` & `obs-cli-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "obsws-python",
   "rich"
 ]
-version = "0.3"
+version = "0.4"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

