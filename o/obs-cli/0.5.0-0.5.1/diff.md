# Comparing `tmp/obs-cli-0.5.0.tar.gz` & `tmp/obs-cli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.5.0.tar", last modified: Mon Jun  5 16:43:46 2023, max compression
+gzip compressed data, was "obs-cli-0.5.1.tar", last modified: Mon Jun  5 16:50:42 2023, max compression
```

## Comparing `obs-cli-0.5.0.tar` & `obs-cli-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.097232 obs-cli-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.093232 obs-cli-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.093232 obs-cli-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 16:43:32.000000 obs-cli-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:43:32.000000 obs-cli-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:43:46.097232 obs-cli-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 16:43:32.000000 obs-cli-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:46.097232 obs-cli-0.5.0/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:43:46.000000 obs-cli-0.5.0/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-06-05 16:43:32.000000 obs-cli-0.5.0/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 16:43:32.000000 obs-cli-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:43:46.097232 obs-cli-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.587804 obs-cli-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.583804 obs-cli-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.583804 obs-cli-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:50:30.000000 obs-cli-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:50:42.587804 obs-cli-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 16:50:30.000000 obs-cli-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.587804 obs-cli-0.5.1/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-05 16:50:30.000000 obs-cli-0.5.1/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 16:50:30.000000 obs-cli-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:50:42.587804 obs-cli-0.5.1/setup.cfg
```

### Comparing `obs-cli-0.5.0/.github/workflows/release.yaml` & `obs-cli-0.5.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.0/LICENSE` & `obs-cli-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.0/PKG-INFO` & `obs-cli-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.5.0/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.5.1/obs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.5.0/obs_cli.py` & `obs-cli-0.5.1/obs_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from rich.console import Console
 from rich.table import Table
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("-D", "--debug", action="store_true", default=False)
+    parser.add_argument("-q", "--quiet", action="store_true", default=False)
     parser.add_argument("-H", "--host", help="host name", default="localhost")
     parser.add_argument(
         "-P", "--port", help="port number", type=int, default=4455
     )
     parser.add_argument(
         "-p", "--password", required=False, help="password ($OBS_API_PASSWORD)"
     )
@@ -319,14 +320,16 @@
                 LOGGER.debug(res)
             elif args.action == "disable":
                 res = disable_filter(cl, args.INPUT, args.FILTER)
                 LOGGER.debug(res)
             elif args.action == "status":
                 res = is_filter_enabled(cl, args.INPUT, args.FILTER)
                 LOGGER.debug(res)
+                if args.quiet:
+                    sys.exit(0 if res else 1)
                 print("enabled" if res else "disabled")
         elif cmd == "hotkey":
             if args.action == "list":
                 data = get_hotkeys(cl)
                 if args.json:
                     print_json(data=data)
                     return
```

### Comparing `obs-cli-0.5.0/pyproject.toml` & `obs-cli-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "obsws-python",
   "rich"
 ]
-version = "0.5.0"
+version = "0.5.1"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

