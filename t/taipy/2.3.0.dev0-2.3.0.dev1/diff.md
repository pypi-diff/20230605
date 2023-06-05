# Comparing `tmp/taipy-2.3.0.dev0.tar.gz` & `tmp/taipy-2.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-2.3.0.dev0.tar", last modified: Mon Jun  5 16:13:40 2023, max compression
+gzip compressed data, was "taipy-2.3.0.dev1.tar", last modified: Mon Jun  5 16:45:22 2023, max compression
```

## Comparing `taipy-2.3.0.dev0.tar` & `taipy-2.3.0.dev1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.515587 taipy-2.3.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_cli/_help_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_cli/_scaffold_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/gui_core/
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/gui_core/GuiCoreLib.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/gui_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.515587 taipy-2.3.0.dev0/src/taipy/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/
--rw-r--r--   0 runner    (1001) docker     (123)   411212 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:13:33.000000 taipy-2.3.0.dev0/src/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.013620 taipy-2.3.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.017620 taipy-2.3.0.dev1/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.017620 taipy-2.3.0.dev1/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/_cli/_scaffold_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.017620 taipy-2.3.0.dev1/src/taipy/gui_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/gui_core/GuiCoreLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/gui_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/src/taipy/gui_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   657107 2023-06-05 16:45:15.000000 taipy-2.3.0.dev1/src/taipy/gui_core/lib/taipy-gui-core.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.013620 taipy-2.3.0.dev1/src/taipy/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   411212 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/src/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.017620 taipy-2.3.0.dev1/src/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-05 16:45:22.000000 taipy-2.3.0.dev1/src/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-05 16:45:22.000000 taipy-2.3.0.dev1/src/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:45:22.000000 taipy-2.3.0.dev1/src/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-05 16:45:22.000000 taipy-2.3.0.dev1/src/taipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:45:15.000000 taipy-2.3.0.dev1/src/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 16:45:22.000000 taipy-2.3.0.dev1/src/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:45:22.000000 taipy-2.3.0.dev1/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:45:22.021620 taipy-2.3.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-05 16:44:05.000000 taipy-2.3.0.dev1/tests/test_run.py
```

### Comparing `taipy-2.3.0.dev0/LICENSE` & `taipy-2.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/PKG-INFO` & `taipy-2.3.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.0.dev0
+Version: 2.3.0.dev1
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-2.3.0.dev0/README.md` & `taipy-2.3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/setup.py` & `taipy-2.3.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/__init__.py` & `taipy-2.3.0.dev1/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/_cli/__init__.py` & `taipy-2.3.0.dev1/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/_cli/_help_cli.py` & `taipy-2.3.0.dev1/src/taipy/_cli/_help_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/_cli/_scaffold_cli.py` & `taipy-2.3.0.dev1/src/taipy/_cli/_scaffold_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/_entrypoint.py` & `taipy-2.3.0.dev1/src/taipy/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/_run.py` & `taipy-2.3.0.dev1/src/taipy/_run.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/gui_core/GuiCoreLib.py` & `taipy-2.3.0.dev1/src/taipy/gui_core/GuiCoreLib.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/gui_core/__init__.py` & `taipy-2.3.0.dev1/src/taipy/gui_core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg` & `taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}` & `taipy-2.3.0.dev1/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy/version.py` & `taipy-2.3.0.dev1/src/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev0/src/taipy.egg-info/PKG-INFO` & `taipy-2.3.0.dev1/src/taipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.0.dev0
+Version: 2.3.0.dev1
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-2.3.0.dev0/src/taipy.egg-info/SOURCES.txt` & `taipy-2.3.0.dev1/src/taipy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,12 +16,13 @@
 src/taipy.egg-info/requires.txt
 src/taipy.egg-info/top_level.txt
 src/taipy/_cli/__init__.py
 src/taipy/_cli/_help_cli.py
 src/taipy/_cli/_scaffold_cli.py
 src/taipy/gui_core/GuiCoreLib.py
 src/taipy/gui_core/__init__.py
+src/taipy/gui_core/lib/taipy-gui-core.js
 src/taipy/templates/taipy-default-template/cookiecutter.json
 src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
 src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
 src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
 tests/test_run.py
```

### Comparing `taipy-2.3.0.dev0/tests/test_run.py` & `taipy-2.3.0.dev1/tests/test_run.py`

 * *Files identical despite different names*

