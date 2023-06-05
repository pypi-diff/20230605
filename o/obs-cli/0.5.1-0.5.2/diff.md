# Comparing `tmp/obs-cli-0.5.1.tar.gz` & `tmp/obs-cli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.5.1.tar", last modified: Mon Jun  5 16:50:42 2023, max compression
+gzip compressed data, was "obs-cli-0.5.2.tar", last modified: Mon Jun  5 16:57:16 2023, max compression
```

## Comparing `obs-cli-0.5.1.tar` & `obs-cli-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.587804 obs-cli-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.583804 obs-cli-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.583804 obs-cli-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 16:50:30.000000 obs-cli-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:50:30.000000 obs-cli-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:50:42.587804 obs-cli-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 16:50:30.000000 obs-cli-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:50:42.587804 obs-cli-0.5.1/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:50:42.000000 obs-cli-0.5.1/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-05 16:50:30.000000 obs-cli-0.5.1/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 16:50:30.000000 obs-cli-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:50:42.587804 obs-cli-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:57:01.000000 obs-cli-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-06-05 16:57:16.441636 obs-cli-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-05 16:57:01.000000 obs-cli-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-05 16:57:01.000000 obs-cli-0.5.2/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 16:57:01.000000 obs-cli-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:57:16.441636 obs-cli-0.5.2/setup.cfg
```

### Comparing `obs-cli-0.5.1/.github/workflows/release.yaml` & `obs-cli-0.5.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.1/LICENSE` & `obs-cli-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.1/PKG-INFO` & `obs-cli-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,8 +700,23 @@
 pipx install obs-cli
 ```
 
 ## Usage
 
 ```
 obs-cli --help
+usage: obs_cli.py [-h] [-D] [-q] [-H HOST] [-P PORT] [-p PASSWORD] [-j]
+                  {scene,item,input,filter,hotkey} ...
+
+positional arguments:
+  {scene,item,input,filter,hotkey}
+
+options:
+  -h, --help            show this help message and exit
+  -D, --debug
+  -q, --quiet
+  -H HOST, --host HOST  host name
+  -P PORT, --port PORT  port number
+  -p PASSWORD, --password PASSWORD
+                        password ($OBS_API_PASSWORD)
+  -j, --json
 ```
```

### Comparing `obs-cli-0.5.1/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.5.2/obs_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,8 +700,23 @@
 pipx install obs-cli
 ```
 
 ## Usage
 
 ```
 obs-cli --help
+usage: obs_cli.py [-h] [-D] [-q] [-H HOST] [-P PORT] [-p PASSWORD] [-j]
+                  {scene,item,input,filter,hotkey} ...
+
+positional arguments:
+  {scene,item,input,filter,hotkey}
+
+options:
+  -h, --help            show this help message and exit
+  -D, --debug
+  -q, --quiet
+  -H HOST, --host HOST  host name
+  -P PORT, --port PORT  port number
+  -p PASSWORD, --password PASSWORD
+                        password ($OBS_API_PASSWORD)
+  -j, --json
 ```
```

### Comparing `obs-cli-0.5.1/obs_cli.py` & `obs-cli-0.5.2/obs_cli.py`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.1/pyproject.toml` & `obs-cli-0.5.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "obsws-python",
   "rich"
 ]
-version = "0.5.1"
+version = "0.5.2"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

