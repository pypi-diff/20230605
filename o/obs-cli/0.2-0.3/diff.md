# Comparing `tmp/obs-cli-0.2.tar.gz` & `tmp/obs-cli-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.2.tar", last modified: Mon Jun  5 15:06:36 2023, max compression
+gzip compressed data, was "obs-cli-0.3.tar", last modified: Mon Jun  5 15:17:35 2023, max compression
```

## Comparing `obs-cli-0.2.tar` & `obs-cli-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.272909 obs-cli-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.268909 obs-cli-0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:06:19.000000 obs-cli-0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.268909 obs-cli-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 15:06:19.000000 obs-cli-0.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 15:06:19.000000 obs-cli-0.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 15:06:19.000000 obs-cli-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 15:06:19.000000 obs-cli-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:06:36.272909 obs-cli-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 15:06:19.000000 obs-cli-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:06:36.268909 obs-cli-0.2/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 15:06:36.000000 obs-cli-0.2/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-05 15:06:19.000000 obs-cli-0.2/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-05 15:06:19.000000 obs-cli-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:06:36.272909 obs-cli-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:17:24.000000 obs-cli-0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 15:17:24.000000 obs-cli-0.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 15:17:24.000000 obs-cli-0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 15:17:24.000000 obs-cli-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 15:17:24.000000 obs-cli-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:17:35.291198 obs-cli-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 15:17:24.000000 obs-cli-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:17:35.291198 obs-cli-0.3/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 15:17:35.000000 obs-cli-0.3/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-05 15:17:24.000000 obs-cli-0.3/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-05 15:17:24.000000 obs-cli-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:17:35.291198 obs-cli-0.3/setup.cfg
```

### Comparing `obs-cli-0.2/.github/workflows/release.yaml` & `obs-cli-0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.2/LICENSE` & `obs-cli-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.2/PKG-INFO` & `obs-cli-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.2
+Version: 0.3
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.2/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.3/obs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.2
+Version: 0.3
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.2/obs_cli.py` & `obs-cli-0.3/obs_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("-D", "--debug", action="store_true", default=False)
     parser.add_argument("-H", "--host", help="host name", default="localhost")
     parser.add_argument(
         "-P", "--port", help="port number", type=int, default=4455
     )
     parser.add_argument("-p", "--password", help="password")
+    parser.add_argument("-j", "--json", action="store_true", default=False)
 
     subparsers = parser.add_subparsers(dest="command")
 
     scene_parser = subparsers.add_parser("scene")
     scene_parser.add_argument(
         "-e", "--exact", action="store_true", default=False, help="Exact match"
     )
@@ -181,45 +182,57 @@
             else:
                 print(get_current_scene_name(cl))
 
         elif cmd == "item":
             if args.action == "list":
                 # print(*get_items(cl, args.scene), sep="\n")
                 scene = args.scene or get_current_scene_name(cl)
+
+                data = get_items(cl, args.scene)
+                if args.json:
+                    print_json(data=data)
+                    return
+
                 table = Table(title=f"Items in scene '{scene}'")
                 table.add_column("ID")
                 table.add_column("Name")
                 table.add_column("Enabled", justify="center")
-                for item in get_items(cl, args.scene):
+                for item in data:
                     item_id = str(item.get("sceneItemId"))
                     name = item.get("sourceName")
                     enabled = "✅" if item.get("sceneItemEnabled") else "❌"
                     table.add_row(item_id, name, enabled)
                 console.print(table)
             elif args.action == "toggle":
                 toggle_item(cl, args.ITEM, args.scene)
             elif args.action == "show":
                 show_item(cl, args.ITEM, args.scene)
             elif args.action == "hide":
                 hide_item(cl, args.ITEM, args.scene)
         elif cmd == "input":
             if args.action == "list":
+                data = get_inputs(cl)
+                if args.json:
+                    print_json(data=data)
+                    return
+
                 table = Table(title="Inputs")
                 table.add_column("Kind")
                 table.add_column("Name")
-                for input in get_inputs(cl):
+                for input in data:
                     kind = input.get("inputKind")
                     name = input.get("inputName")
                     table.add_row(kind, name)
                 console.print(table)
             elif args.action == "show":
                 data = get_input_settings(cl, args.INPUT)
                 if args.PROPERTY:
                     print(data.get(args.PROPERTY))
                 else:
+                    # TODO Implement rich table output
                     print_json(data=data)
             elif args.action == "set":
                 if not args.INPUT or not args.PROPERTY or not args.VALUE:
                     raise ValueError("Missing input name, property or value")
                 set_input_setting(cl, args.INPUT, args.PROPERTY, args.VALUE)
 
         return 0
```

### Comparing `obs-cli-0.2/pyproject.toml` & `obs-cli-0.3/pyproject.toml`

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
-version = "0.2"
+version = "0.3"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

