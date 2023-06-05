# Comparing `tmp/obs-cli-0.1.tar.gz` & `tmp/obs-cli-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.1.tar", last modified: Mon Jun  5 14:15:57 2023, max compression
+gzip compressed data, was "obs-cli-0.2.tar", last modified: Mon Jun  5 15:06:36 2023, max compression
```

## Comparing `obs-cli-0.1.tar` & `obs-cli-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:15:57.637608 obs-cli-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:15:57.633607 obs-cli-0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 14:15:46.000000 obs-cli-0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:15:57.633607 obs-cli-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 14:15:46.000000 obs-cli-0.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 14:15:46.000000 obs-cli-0.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 14:15:46.000000 obs-cli-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 14:15:46.000000 obs-cli-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 14:15:57.637608 obs-cli-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 14:15:46.000000 obs-cli-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:15:57.637608 obs-cli-0.1/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 14:15:57.000000 obs-cli-0.1/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 14:15:57.000000 obs-cli-0.1/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:15:57.000000 obs-cli-0.1/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 14:15:57.000000 obs-cli-0.1/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 14:15:57.000000 obs-cli-0.1/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:15:57.000000 obs-cli-0.1/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-05 14:15:46.000000 obs-cli-0.1/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-05 14:15:46.000000 obs-cli-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:15:57.637608 obs-cli-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.272909 obs-cli-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.268909 obs-cli-0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:06:19.000000 obs-cli-0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.268909 obs-cli-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 15:06:19.000000 obs-cli-0.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 15:06:19.000000 obs-cli-0.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 15:06:19.000000 obs-cli-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 15:06:19.000000 obs-cli-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:06:36.272909 obs-cli-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 15:06:19.000000 obs-cli-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.268909 obs-cli-0.2/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-05 15:06:19.000000 obs-cli-0.2/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-05 15:06:19.000000 obs-cli-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:06:36.272909 obs-cli-0.2/setup.cfg
```

### Comparing `obs-cli-0.1/.github/workflows/release.yaml` & `obs-cli-0.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.1/LICENSE` & `obs-cli-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.1/PKG-INFO` & `obs-cli-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.1
+Version: 0.2
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.1/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.2/obs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.1
+Version: 0.2
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.1/obs_cli.py` & `obs-cli-0.2/obs_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 import argparse
 import logging
 import re
 import sys
 
 import obsws_python as obs
-from rich import print
+from rich import print, print_json
 from rich.console import Console
 from rich.table import Table
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("-D", "--debug", action="store_true", default=False)
     parser.add_argument("-H", "--host", help="host name", default="localhost")
     parser.add_argument(
         "-P", "--port", help="port number", type=int, default=4455
     )
     parser.add_argument("-p", "--password", help="password")
 
     subparsers = parser.add_subparsers(dest="command")
+
     scene_parser = subparsers.add_parser("scene")
     scene_parser.add_argument(
         "-e", "--exact", action="store_true", default=False, help="Exact match"
     )
     scene_parser.add_argument(
         "-i",
         "--ignorecase",
@@ -49,14 +50,25 @@
         "action",
         choices=["list", "show", "hide", "toggle"],
         default="toggle",
         help="show/hide/toggle",
     )
     item_parser.add_argument("ITEM", nargs="?", help="Item to interact with")
 
+    input_parser = subparsers.add_parser("input")
+    input_parser.add_argument(
+        "action",
+        choices=["list", "show", "set"],
+        default="show",
+        help="list/show",
+    )
+    input_parser.add_argument("INPUT", nargs="?", help="Input name")
+    input_parser.add_argument("PROPERTY", nargs="?", help="Property name")
+    input_parser.add_argument("VALUE", nargs="?", help="Property value")
+
     return parser.parse_args()
 
 
 def switch_to_scene(cl, scene, exact=False, ignorecase=True):
     regex = re.compile(
         f"^{scene}$" if exact else scene,
         re.IGNORECASE if ignorecase else re.NOFLAG,
@@ -126,14 +138,26 @@
     return cl.set_scene_item_enabled(scene, item_id, not enabled)
 
 
 def get_current_scene_name(cl):
     return cl.get_current_program_scene().current_program_scene_name
 
 
+def get_inputs(cl):
+    return sorted(cl.get_input_list().inputs, key=lambda x: x.get("inputName"))
+
+
+def get_input_settings(cl, input):
+    return cl.get_input_settings(input).input_settings
+
+
+def set_input_setting(cl, input, key, value):
+    return cl.set_input_settings(input, {key: value}, overlay=True)
+
+
 def main():
     console = Console()
     logging.basicConfig()
 
     args = parse_args()
     LOGGER.setLevel(logging.DEBUG if args.debug else logging.INFO)
     LOGGER.debug(args)
@@ -173,14 +197,35 @@
                 console.print(table)
             elif args.action == "toggle":
                 toggle_item(cl, args.ITEM, args.scene)
             elif args.action == "show":
                 show_item(cl, args.ITEM, args.scene)
             elif args.action == "hide":
                 hide_item(cl, args.ITEM, args.scene)
+        elif cmd == "input":
+            if args.action == "list":
+                table = Table(title="Inputs")
+                table.add_column("Kind")
+                table.add_column("Name")
+                for input in get_inputs(cl):
+                    kind = input.get("inputKind")
+                    name = input.get("inputName")
+                    table.add_row(kind, name)
+                console.print(table)
+            elif args.action == "show":
+                data = get_input_settings(cl, args.INPUT)
+                if args.PROPERTY:
+                    print(data.get(args.PROPERTY))
+                else:
+                    print_json(data=data)
+            elif args.action == "set":
+                if not args.INPUT or not args.PROPERTY or not args.VALUE:
+                    raise ValueError("Missing input name, property or value")
+                set_input_setting(cl, args.INPUT, args.PROPERTY, args.VALUE)
+
         return 0
     except Exception:
         console.print_exception(show_locals=True)
         return 1
 
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `obs-cli-0.1/pyproject.toml` & `obs-cli-0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "obsws-python",
   "rich"
 ]
-version = "0.1"
+version = "0.2"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

