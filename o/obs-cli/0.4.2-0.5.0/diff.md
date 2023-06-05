# Comparing `tmp/obs-cli-0.4.2.tar.gz` & `tmp/obs-cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.4.2.tar", last modified: Mon Jun  5 16:31:34 2023, max compression
+gzip compressed data, was "obs-cli-0.5.0.tar", last modified: Mon Jun  5 16:43:46 2023, max compression
```

## Comparing `obs-cli-0.4.2.tar` & `obs-cli-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:31:34.085409 obs-cli-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:31:34.085409 obs-cli-0.4.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 16:31:18.000000 obs-cli-0.4.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:31:34.085409 obs-cli-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 16:31:18.000000 obs-cli-0.4.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 16:31:18.000000 obs-cli-0.4.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 16:31:18.000000 obs-cli-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:31:18.000000 obs-cli-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:31:34.085409 obs-cli-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 16:31:18.000000 obs-cli-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:31:34.085409 obs-cli-0.4.2/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:31:34.000000 obs-cli-0.4.2/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:31:34.000000 obs-cli-0.4.2/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:31:34.000000 obs-cli-0.4.2/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:31:34.000000 obs-cli-0.4.2/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:31:34.000000 obs-cli-0.4.2/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:31:34.000000 obs-cli-0.4.2/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-06-05 16:31:18.000000 obs-cli-0.4.2/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 16:31:18.000000 obs-cli-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:31:34.085409 obs-cli-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.097232 obs-cli-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.093232 obs-cli-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.093232 obs-cli-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:43:32.000000 obs-cli-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:43:46.097232 obs-cli-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 16:43:32.000000 obs-cli-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.097232 obs-cli-0.5.0/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-06-05 16:43:32.000000 obs-cli-0.5.0/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 16:43:32.000000 obs-cli-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:43:46.097232 obs-cli-0.5.0/setup.cfg
```

### Comparing `obs-cli-0.4.2/.github/workflows/release.yaml` & `obs-cli-0.5.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.4.2/LICENSE` & `obs-cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.4.2/PKG-INFO` & `obs-cli-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.4.2
+Version: 0.5.0
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.4.2/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.5.0/obs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.4.2
+Version: 0.5.0
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.4.2/obs_cli.py` & `obs-cli-0.5.0/obs_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,23 @@
         choices=["list", "toggle", "enable", "disable", "status"],
         default="list",
         help="list/toggle/enable/disable/status",
     )
     filter_parser.add_argument("INPUT", nargs="?", help="Input name")
     filter_parser.add_argument("FILTER", nargs="?", help="Filter name")
 
+    hotkey_parser = subparsers.add_parser("hotkey")
+    hotkey_parser.add_argument(
+        "action",
+        choices=["list", "trigger"],
+        default="list",
+        help="list/trigger",
+    )
+    hotkey_parser.add_argument("HOTKEY", nargs="?", help="Hotkey name")
+
     return parser.parse_args()
 
 
 def switch_to_scene(cl, scene, exact=False, ignorecase=True):
     regex = re.compile(
         f"^{scene}$" if exact else scene,
         re.IGNORECASE if ignorecase else re.NOFLAG,
@@ -185,14 +194,22 @@
 
 
 def toggle_filter(cl, source, filter):
     enabled = is_filter_enabled(cl, source, filter)
     return cl.set_source_filter_enabled(source, filter, not enabled)
 
 
+def get_hotkeys(cl):
+    return cl.get_hot_key_list().hotkeys
+
+
+def trigger_hotkey(cl, hotkey):
+    return cl.trigger_hot_key_by_name(hotkey)
+
+
 def main():
     console = Console()
     logging.basicConfig()
 
     args = parse_args()
     LOGGER.setLevel(logging.DEBUG if args.debug else logging.INFO)
     LOGGER.debug(args)
@@ -303,14 +320,28 @@
             elif args.action == "disable":
                 res = disable_filter(cl, args.INPUT, args.FILTER)
                 LOGGER.debug(res)
             elif args.action == "status":
                 res = is_filter_enabled(cl, args.INPUT, args.FILTER)
                 LOGGER.debug(res)
                 print("enabled" if res else "disabled")
+        elif cmd == "hotkey":
+            if args.action == "list":
+                data = get_hotkeys(cl)
+                if args.json:
+                    print_json(data=data)
+                    return
+                table = Table(title="Hotkeys")
+                table.add_column("Name")
+                for hk in data:
+                    table.add_row(hk)
+                console.print(table)
+            elif args.action == "trigger":
+                res = trigger_hotkey(cl, args.HOTKEY)
+                LOGGER.debug(res)
 
         return 0
     except Exception:
         console.print_exception(show_locals=True)
         return 1
```

