# Comparing `tmp/object-settings-4.0.5.tar.gz` & `tmp/object-settings-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object-settings-4.0.5.tar", last modified: Mon Apr 10 16:35:08 2023, max compression
+gzip compressed data, was "object-settings-4.1.tar", last modified: Mon Jun  5 18:27:46 2023, max compression
```

## Comparing `object-settings-4.0.5.tar` & `object-settings-4.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.766898 object-settings-4.0.5/
--rw-r--r--   0 samu      (1000) samu      (1000)     5602 2023-04-10 16:35:08.766898 object-settings-4.0.5/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)     4755 2023-03-09 17:49:33.000000 object-settings-4.0.5/README.md
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.760898 object-settings-4.0.5/object_settings.egg-info/
--rw-r--r--   0 samu      (1000) samu      (1000)     5602 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)     1223 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/SOURCES.txt
--rw-r--r--   0 samu      (1000) samu      (1000)        1 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/dependency_links.txt
--rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/requires.txt
--rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/top_level.txt
--rw-r--r--   0 samu      (1000) samu      (1000)     1136 2023-04-10 16:33:53.000000 object-settings-4.0.5/pyproject.toml
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.760898 object-settings-4.0.5/settings/
--rw-r--r--   0 samu      (1000) samu      (1000)      389 2023-03-04 19:26:29.000000 object-settings-4.0.5/settings/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.761898 object-settings-4.0.5/settings/backend/
--rw-r--r--   0 samu      (1000) samu      (1000)      114 2023-03-09 16:08:28.000000 object-settings-4.0.5/settings/backend/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1909 2023-03-09 17:10:15.000000 object-settings-4.0.5/settings/backend/config.py
--rw-r--r--   0 samu      (1000) samu      (1000)      835 2023-04-10 16:29:41.000000 object-settings-4.0.5/settings/backend/datatype_loader.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1494 2023-03-09 16:08:28.000000 object-settings-4.0.5/settings/backend/main.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.762898 object-settings-4.0.5/settings/backend/parsers/
--rw-r--r--   0 samu      (1000) samu      (1000)      235 2023-03-09 16:25:34.000000 object-settings-4.0.5/settings/backend/parsers/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)      848 2023-03-09 14:41:43.000000 object-settings-4.0.5/settings/backend/parsers/_template.py
--rw-r--r--   0 samu      (1000) samu      (1000)      839 2023-03-09 16:10:26.000000 object-settings-4.0.5/settings/backend/parsers/cli.py
--rw-r--r--   0 samu      (1000) samu      (1000)      812 2023-03-09 14:41:43.000000 object-settings-4.0.5/settings/backend/parsers/env.py
--rw-r--r--   0 samu      (1000) samu      (1000)     2213 2023-03-10 16:44:26.000000 object-settings-4.0.5/settings/backend/parsers/files.py
--rw-r--r--   0 samu      (1000) samu      (1000)     3373 2023-03-09 17:10:15.000000 object-settings-4.0.5/settings/base.py
--rw-r--r--   0 samu      (1000) samu      (1000)     4411 2023-03-03 16:47:09.000000 object-settings-4.0.5/settings/types.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.762898 object-settings-4.0.5/settings_gui/
--rw-r--r--   0 samu      (1000) samu      (1000)      231 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)      338 2022-12-16 13:11:05.000000 object-settings-4.0.5/settings_gui/_tk_abstractor.py
--rw-r--r--   0 samu      (1000) samu      (1000)      279 2023-03-04 22:40:29.000000 object-settings-4.0.5/settings_gui/config.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.763898 object-settings-4.0.5/settings_gui/tkinter/
--rw-r--r--   0 samu      (1000) samu      (1000)      343 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/tkinter/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.764898 object-settings-4.0.5/settings_gui/tkinter/icons/
--rw-r--r--   0 samu      (1000) samu      (1000)      206 2015-11-19 10:52:05.000000 object-settings-4.0.5/settings_gui/tkinter/icons/checkmark-black.png
--rw-r--r--   0 samu      (1000) samu      (1000)     4826 2022-10-23 18:33:29.000000 object-settings-4.0.5/settings_gui/tkinter/icons/checkmark-white.png
--rw-r--r--   0 samu      (1000) samu      (1000)      333 2015-11-19 10:51:50.000000 object-settings-4.0.5/settings_gui/tkinter/icons/error.png
--rw-r--r--   0 samu      (1000) samu      (1000)      301 2015-11-21 05:08:04.000000 object-settings-4.0.5/settings_gui/tkinter/icons/folder-black.png
--rw-r--r--   0 samu      (1000) samu      (1000)     5036 2022-10-23 16:12:53.000000 object-settings-4.0.5/settings_gui/tkinter/icons/folder-white.png
--rw-r--r--   0 samu      (1000) samu      (1000)     1417 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/tkinter/main.py
--rw-r--r--   0 samu      (1000) samu      (1000)      708 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/tkinter/section_frames.py
--rw-r--r--   0 samu      (1000) samu      (1000)     7619 2023-03-09 14:26:09.000000 object-settings-4.0.5/settings_gui/tkinter/type_frames.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.764898 object-settings-4.0.5/settings_gui/ttk/
--rw-r--r--   0 samu      (1000) samu      (1000)      719 2022-12-16 20:12:38.000000 object-settings-4.0.5/settings_gui/ttk/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)       38 2023-04-10 16:35:08.766898 object-settings-4.0.5/setup.cfg
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.766898 object-settings-4.0.5/tests/
--rw-r--r--   0 samu      (1000) samu      (1000)      923 2023-03-09 16:25:34.000000 object-settings-4.0.5/tests/test_cli.py
--rw-r--r--   0 samu      (1000) samu      (1000)      797 2023-03-09 15:35:21.000000 object-settings-4.0.5/tests/test_datafiles.py
--rw-r--r--   0 samu      (1000) samu      (1000)      791 2023-04-10 16:31:09.000000 object-settings-4.0.5/tests/test_datatype_loader.py
--rw-r--r--   0 samu      (1000) samu      (1000)      821 2023-03-09 16:25:34.000000 object-settings-4.0.5/tests/test_endurance.py
--rw-r--r--   0 samu      (1000) samu      (1000)      830 2023-03-09 14:52:24.000000 object-settings-4.0.5/tests/test_env.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1715 2023-03-04 11:54:10.000000 object-settings-4.0.5/tests/test_gui_(manual).py
--rw-r--r--   0 samu      (1000) samu      (1000)     1108 2022-10-27 17:39:38.000000 object-settings-4.0.5/tests/test_v1_definitions.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1466 2022-11-03 11:24:05.000000 object-settings-4.0.5/tests/test_validation.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.295534 object-settings-4.1/
+-rw-r--r--   0 samu      (1000) samu      (1000)     5600 2023-06-05 18:27:46.295534 object-settings-4.1/PKG-INFO
+-rw-r--r--   0 samu      (1000) samu      (1000)     4755 2023-03-09 17:49:33.000000 object-settings-4.1/README.md
+-rw-r--r--   0 samu      (1000) samu      (1000)      969 2023-06-05 18:27:20.000000 object-settings-4.1/pyproject.toml
+-rw-r--r--   0 samu      (1000) samu      (1000)       38 2023-06-05 18:27:46.296534 object-settings-4.1/setup.cfg
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.284535 object-settings-4.1/src/
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.286535 object-settings-4.1/src/object_settings.egg-info/
+-rw-r--r--   0 samu      (1000) samu      (1000)     5600 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/PKG-INFO
+-rw-r--r--   0 samu      (1000) samu      (1000)     1343 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 samu      (1000) samu      (1000)        1 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/requires.txt
+-rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/top_level.txt
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.288534 object-settings-4.1/src/settings/
+-rw-r--r--   0 samu      (1000) samu      (1000)      427 2023-06-05 16:38:50.000000 object-settings-4.1/src/settings/__init__.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.289535 object-settings-4.1/src/settings/backend/
+-rw-r--r--   0 samu      (1000) samu      (1000)      114 2023-03-09 16:08:28.000000 object-settings-4.1/src/settings/backend/__init__.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     3004 2023-06-05 17:19:56.000000 object-settings-4.1/src/settings/backend/config.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      855 2023-06-05 14:08:02.000000 object-settings-4.1/src/settings/backend/datatype_loader.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1494 2023-06-05 17:28:50.000000 object-settings-4.1/src/settings/backend/main.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.290535 object-settings-4.1/src/settings/backend/parsers/
+-rw-r--r--   0 samu      (1000) samu      (1000)      263 2023-06-05 14:30:05.000000 object-settings-4.1/src/settings/backend/parsers/__init__.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      935 2023-06-05 14:50:54.000000 object-settings-4.1/src/settings/backend/parsers/_template.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      853 2023-06-05 14:30:30.000000 object-settings-4.1/src/settings/backend/parsers/cli.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      826 2023-06-05 14:30:55.000000 object-settings-4.1/src/settings/backend/parsers/env.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     2214 2023-06-05 17:16:10.000000 object-settings-4.1/src/settings/backend/parsers/files.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     3620 2023-06-05 17:31:48.000000 object-settings-4.1/src/settings/base.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     4472 2023-06-05 16:26:58.000000 object-settings-4.1/src/settings/types.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.290535 object-settings-4.1/src/settings_gui/
+-rw-r--r--   0 samu      (1000) samu      (1000)      231 2023-03-04 11:44:09.000000 object-settings-4.1/src/settings_gui/__init__.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      338 2023-06-05 15:03:20.000000 object-settings-4.1/src/settings_gui/_tk_abstractor.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      279 2023-03-04 22:40:29.000000 object-settings-4.1/src/settings_gui/config.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.292534 object-settings-4.1/src/settings_gui/tkinter/
+-rw-r--r--   0 samu      (1000) samu      (1000)      343 2023-03-04 11:44:09.000000 object-settings-4.1/src/settings_gui/tkinter/__init__.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.293535 object-settings-4.1/src/settings_gui/tkinter/icons/
+-rw-r--r--   0 samu      (1000) samu      (1000)      206 2015-11-19 10:52:05.000000 object-settings-4.1/src/settings_gui/tkinter/icons/checkmark-black.png
+-rw-r--r--   0 samu      (1000) samu      (1000)     4826 2022-10-23 18:33:29.000000 object-settings-4.1/src/settings_gui/tkinter/icons/checkmark-white.png
+-rw-r--r--   0 samu      (1000) samu      (1000)      333 2015-11-19 10:51:50.000000 object-settings-4.1/src/settings_gui/tkinter/icons/error.png
+-rw-r--r--   0 samu      (1000) samu      (1000)      301 2015-11-21 05:08:04.000000 object-settings-4.1/src/settings_gui/tkinter/icons/folder-black.png
+-rw-r--r--   0 samu      (1000) samu      (1000)     5036 2022-10-23 16:12:53.000000 object-settings-4.1/src/settings_gui/tkinter/icons/folder-white.png
+-rw-r--r--   0 samu      (1000) samu      (1000)     1505 2023-06-05 17:48:09.000000 object-settings-4.1/src/settings_gui/tkinter/main.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      723 2023-06-05 16:49:45.000000 object-settings-4.1/src/settings_gui/tkinter/section_frames.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     7620 2023-06-05 16:49:23.000000 object-settings-4.1/src/settings_gui/tkinter/type_frames.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.293535 object-settings-4.1/src/settings_gui/ttk/
+-rw-r--r--   0 samu      (1000) samu      (1000)      719 2022-12-16 20:12:38.000000 object-settings-4.1/src/settings_gui/ttk/__init__.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.295534 object-settings-4.1/tests/
+-rw-r--r--   0 samu      (1000) samu      (1000)      923 2023-03-09 16:25:34.000000 object-settings-4.1/tests/test_cli.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      797 2023-03-09 15:35:21.000000 object-settings-4.1/tests/test_datafiles.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      791 2023-04-10 16:31:09.000000 object-settings-4.1/tests/test_datatype_loader.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      821 2023-03-09 16:25:34.000000 object-settings-4.1/tests/test_endurance.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      830 2023-03-09 14:52:24.000000 object-settings-4.1/tests/test_env.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1811 2023-06-05 17:47:04.000000 object-settings-4.1/tests/test_gui_(manual).py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1108 2022-10-27 17:39:38.000000 object-settings-4.1/tests/test_v1_definitions.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1466 2022-11-03 11:24:05.000000 object-settings-4.1/tests/test_validation.py
```

### Comparing `object-settings-4.0.5/PKG-INFO` & `object-settings-4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-settings
-Version: 4.0.5
+Version: 4.1
 Summary: Simple object-oriented config library, where your settings are objects
 License: MIT License
 Project-URL: Homepage, https://github.com/SamuLumio/object-settings
 Keywords: settings,setting,config,OOP,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `object-settings-4.0.5/README.md` & `object-settings-4.1/README.md`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/object_settings.egg-info/PKG-INFO` & `object-settings-4.1/src/object_settings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-settings
-Version: 4.0.5
+Version: 4.1
 Summary: Simple object-oriented config library, where your settings are objects
 License: MIT License
 Project-URL: Homepage, https://github.com/SamuLumio/object-settings
 Keywords: settings,setting,config,OOP,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `object-settings-4.0.5/object_settings.egg-info/SOURCES.txt` & `object-settings-4.1/src/object_settings.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 README.md
 pyproject.toml
-object_settings.egg-info/PKG-INFO
-object_settings.egg-info/SOURCES.txt
-object_settings.egg-info/dependency_links.txt
-object_settings.egg-info/requires.txt
-object_settings.egg-info/top_level.txt
-settings/__init__.py
-settings/base.py
-settings/types.py
-settings/backend/__init__.py
-settings/backend/config.py
-settings/backend/datatype_loader.py
-settings/backend/main.py
-settings/backend/parsers/__init__.py
-settings/backend/parsers/_template.py
-settings/backend/parsers/cli.py
-settings/backend/parsers/env.py
-settings/backend/parsers/files.py
-settings_gui/__init__.py
-settings_gui/_tk_abstractor.py
-settings_gui/config.py
-settings_gui/tkinter/__init__.py
-settings_gui/tkinter/main.py
-settings_gui/tkinter/section_frames.py
-settings_gui/tkinter/type_frames.py
-settings_gui/tkinter/icons/checkmark-black.png
-settings_gui/tkinter/icons/checkmark-white.png
-settings_gui/tkinter/icons/error.png
-settings_gui/tkinter/icons/folder-black.png
-settings_gui/tkinter/icons/folder-white.png
-settings_gui/ttk/__init__.py
+src/object_settings.egg-info/PKG-INFO
+src/object_settings.egg-info/SOURCES.txt
+src/object_settings.egg-info/dependency_links.txt
+src/object_settings.egg-info/requires.txt
+src/object_settings.egg-info/top_level.txt
+src/settings/__init__.py
+src/settings/base.py
+src/settings/types.py
+src/settings/backend/__init__.py
+src/settings/backend/config.py
+src/settings/backend/datatype_loader.py
+src/settings/backend/main.py
+src/settings/backend/parsers/__init__.py
+src/settings/backend/parsers/_template.py
+src/settings/backend/parsers/cli.py
+src/settings/backend/parsers/env.py
+src/settings/backend/parsers/files.py
+src/settings_gui/__init__.py
+src/settings_gui/_tk_abstractor.py
+src/settings_gui/config.py
+src/settings_gui/tkinter/__init__.py
+src/settings_gui/tkinter/main.py
+src/settings_gui/tkinter/section_frames.py
+src/settings_gui/tkinter/type_frames.py
+src/settings_gui/tkinter/icons/checkmark-black.png
+src/settings_gui/tkinter/icons/checkmark-white.png
+src/settings_gui/tkinter/icons/error.png
+src/settings_gui/tkinter/icons/folder-black.png
+src/settings_gui/tkinter/icons/folder-white.png
+src/settings_gui/ttk/__init__.py
 tests/test_cli.py
 tests/test_datafiles.py
 tests/test_datatype_loader.py
 tests/test_endurance.py
 tests/test_env.py
 tests/test_gui_(manual).py
 tests/test_v1_definitions.py
```

### Comparing `object-settings-4.0.5/pyproject.toml` & `object-settings-4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "object-settings"
-version = "4.0.5"
+version = "4.1"
 description = "Simple object-oriented config library, where your settings are objects"
 readme = "README.md"
 keywords = ["settings", "setting", "config", "OOP", "GUI"]
 urls = {"Homepage"="https://github.com/SamuLumio/object-settings"}
 license = {text="MIT License"}
 
 dependencies = [
@@ -23,23 +23,10 @@
     "Topic :: Utilities",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces"
 ]
 
-
-
 [tool.setuptools]
-
-packages = [
-    "settings",
-    "settings.backend",
-    "settings.backend.parsers",
-
-    "settings_gui",
-    "settings_gui.tkinter",
-    "settings_gui.ttk",
-]
-
 include-package-data = true
-package-data = {'settings_gui.tkinter'=['icons/*']}
+package-data = {'settings_gui.tkinter'=['icons/*']}
```

### Comparing `object-settings-4.0.5/settings/backend/config.py` & `object-settings-4.1/src/settings/backend/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,44 +19,59 @@
 	return cls()
 
 
 
 @_instance
 @_dataclass
 class values:
-	"""Call this to configure the library to better suit your app.
+	"""Call this or set attributes to configure the library to better suit your app.
 	Only app_name is required, all other values are optional."""
 
-	app_name: str = None
-	"""The name/id of your app - used to generate paths for config files and keys for environment variables 
+	app_name: str = ""
+	"""REQUIRED: The name/id of your app - used to generate paths for config files and keys for environment variables 
 	(this is the only required option)"""
 
 	custom_dir: str | None = None
 	"""Custom directory to store config files in instead of the one generated with app_name"""
 
+	default_section_name: str = "Settings"
+	"""Title for the default section that settings are placed under. Defaults to 'Settings'."""
+
 	use_environment: bool = True
-	"""Allow loading setting values from the enviroment
-	(like env vars and command line options)"""
+	"""Allow loading setting values from the enviroment (like env vars and command line options). \n
+	If a setting's value has been set from the environment, it takes priority over any stored configurations, 
+	and it can't be changed on runtime. 
+	You can still set new values for settings, 
+	but they will be saved to storage and the get() method will keep returning the environment value."""
 
-	storage_parsers: list[type[parsers.StorageParser]] = _field(
+	storage_parsers: list[type[parsers.StorageParserTemplate]] = _field(
 		default_factory=parsers.storage_parsers.copy)
+	"""Select which storage sources and file formats to get setting values from. 
+	By default all builtin ones are selected. \n 
+	If you want to implement custom ones, subclass backend.parsers.StorageParserTemplate, 
+	implement all the methods, and add your own parser classes to this list."""
 
-	environment_parsers: list[type[parsers.EnvironmentParser]] = _field(
+	environment_parsers: list[type[parsers.EnvironmentParserTemplate]] = _field(
 		default_factory=parsers.environment_parsers.copy)
+	"""Select which environment sources to get setting values from (these take priority over the storage parsers). 
+	By default all builtin ones are selected. \n 
+	If you want to implement custom ones, subclass backend.parsers.EnvironmentParserTemplate, 
+	implement all the methods, and add your own parser classes to this list."""
+
 
 
 	def __getattribute__(self, item):
 		value = super().__getattribute__(item)
-		if item == 'app_name' and value is None:
+		if item == 'app_name' and value == "":
 			raise NotSetupError
 		else:
 			return value
 
 
-# Aliases because the class serves as both of these things
+# Aliases because the values class serves as both of these things
 setup = values
 config = values
```

### Comparing `object-settings-4.0.5/settings/backend/datatype_loader.py` & `object-settings-4.1/src/settings/backend/datatype_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import configparser
+import configparser, typing
 
 str_converter_functions = {
 	str: str,
 	int: int,
 	float: float,
 	bool: lambda string: configparser.ConfigParser.BOOLEAN_STATES[string.lower()],
 	list: lambda string: string.removeprefix("['").removesuffix("']").split("', '")
 }
 
-def get(data, output_type: type[str | int | float | bool | list]):
+def get(data: typing.Any, output_type: type[str | int | float | bool | list]):
 	if isinstance(data, output_type):
 		return data
 	elif isinstance(data, float) and output_type == int:
 		return int(data)
 	elif isinstance(data, str) and output_type in str_converter_functions:
 		function = str_converter_functions[output_type]
 		return function(data)
```

### Comparing `object-settings-4.0.5/settings/backend/main.py` & `object-settings-4.1/src/settings/backend/main.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/settings/backend/parsers/_template.py` & `object-settings-4.1/src/settings/backend/parsers/_template.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-class EnvironmentParser:
+import typing
+
+
+class EnvironmentParserTemplate:
 	"""Controller/parser for a read-only config source"""
 
 	@classmethod
 	def generate_key_name(cls, setting_name: str) -> str:
 		"""Generate a key name that a setting can be found with"""
 		return str(setting_name)
 
 	@classmethod
-	def get(cls, option: str) -> str:
+	def get(cls, option: str) -> typing.Any:
 		"""Reload and get value"""
 
 	@classmethod
 	def exists(cls, option: str) -> bool:
 		"""Check if option is defined"""
+		return False
 
 
 
 
-class StorageParser:
+class StorageParserTemplate:
 	"""Controller/parser for a config file"""
 
 	def __init__(self, header="Settings"):
 		self.header = header
 
-	def get(self, option: str) -> str:
+	def get(self, option: str) -> typing.Any:
 		"""Reload and get value"""
 
 	def set(self, option: str, value):
 		"""Set a value and write to storage"""
 
 	def exists(self, option: str) -> bool:
 		"""Check if option is defined"""
+		return False
 
 	@property
 	def active(self) -> bool:
-		"""Check if target path exists"""
+		"""Check if a stored configuration exists"""
 		return False
```

### Comparing `object-settings-4.0.5/settings/backend/parsers/cli.py` & `object-settings-4.1/src/settings/backend/parsers/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys, argparse
 
-from . import _template
+from . import EnvironmentParserTemplate
 
 
 
-class CliOptionParser(_template.EnvironmentParser):
+class CliOptionParser(EnvironmentParserTemplate):
 
 	@classmethod
 	def generate_key_name(cls, setting_name: str):
 		"""Generates a cli option name in the form --setting-name,
 		with dashes, lowercase letters and no spaces or special characters"""
 		name = setting_name.lower()
 		for index, char in enumerate(name):
```

### Comparing `object-settings-4.0.5/settings/backend/parsers/env.py` & `object-settings-4.1/src/settings/backend/parsers/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
-from . import _template
+from . import EnvironmentParserTemplate
 
 
 
-class EnvVarParser(_template.EnvironmentParser):
+class EnvVarParser(EnvironmentParserTemplate):
 
 	@classmethod
 	def generate_key_name(cls, setting_name: str):
 		"""Generates an envvar key in the form APPNAME_SETTING_NAME,
 		with underscores, capital letters and no spaces or special characters"""
 
 		def convert(string: str):
```

### Comparing `object-settings-4.0.5/settings/backend/parsers/files.py` & `object-settings-4.1/src/settings/backend/parsers/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import appdirs, os, configparser, json, yaml
 
-from . import _template
+from . import StorageParserTemplate
 
 
 
-class _FileParser(_template.StorageParser):
+class _FileParser(StorageParserTemplate):
 	ext: str
 
 	def __init__(self, header="Settings"):
 		super().__init__(header)
 		self.values: dict = {}
 
 	@property
 	def path(self):
 		from .. import config
 		if isinstance(config.custom_dir, str):
 			dir = config.custom_dir
 		else:
-			# noinspection PyTypeChecker
 			dir = appdirs.user_config_dir(config.app_name, False)
 		return os.path.join(dir, self.header + self.ext)
 
 	def _read(self):
 		"""Load values from file"""
 		# Subclass
 
@@ -55,25 +54,23 @@
 
 
 class CfgParser(_FileParser):
 	ext = '.cfg'
 
 	def __init__(self, header="Settings"):
 		super().__init__(header)
-
 		# Initialize lower-level config parser
 		self._parser = configparser.ConfigParser()
-		self._parser.optionxform = str  # For preserve case
-
-		# Make sure that section exists
-		if self.header not in self._parser.sections():
-			self._parser.add_section(self.header)
+		self._parser.optionxform = str  # For preserve case    # type: ignore
 
 	def _read(self):
 		self._parser.read(self.path)
+		# Make sure that header section exists
+		if self.header not in self._parser.sections():
+			self._parser.add_section(self.header)
 		self.values = dict(self._parser[self.header])
 
 	def _write(self):
 		super()._write()
 		self._parser[self.header] = {str(key): str(value) for key, value in self.values.items()}
 		with open(self.path, 'w') as f:
 			self._parser.write(f)
```

### Comparing `object-settings-4.0.5/settings/base.py` & `object-settings-4.1/src/settings/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import threading, typing
 
-from . import backend
+from . import backend, config
 
 
 
 
 class Section:
-	"""A group of settings that is also represented by one file.
-	Usage of these is optional, settings defined without sections will use the default one."""
+	"""A group of settings that is also represented by one config file.
+	Usage of these is optional – settings defined without sections will use the default one."""
 	def __init__(self, name: str):
 		self.name = name
 		self.settings = []
 		self._storage = None
-		# self._environment = None
 		self.environment = backend.Environment()
 		all_sections.append(self)
 
 	@property
 	def storage(self):
 		if self._storage is None:
 			self._storage = backend.Storage(self.name)
 		return self._storage
+	
+	def is_default(self):
+		"""Check if this section is the default section"""
+		return self == default_section
 
-	# @property
-	# def environment(self):
-	# 	if self._environment is None:
-	# 		self._environment = backend.Environment()
-	# 	return self._environment
 
+all_sections: list[Section] = []
 
 
 
-all_sections: list[Section] = []
-default_section = Section('Settings')
+class _DefaultSection(Section):
+
+	@property
+	def name(self):
+		return config.default_section_name
+	
+	@name.setter
+	def name(self, value):
+		pass
+	
+default_section = _DefaultSection('')
 
 
 
 
-class Setting:
-	"""Base setting class - can be effectively subclassed to create custom setting types"""
+
+class BaseSetting:
+	"""Base setting class - can be safely subclassed to create custom setting types"""
 	def __init__(self, datatype, name: str, default, section: Section = default_section):
 		self.datatype = datatype
 		self.name = name
 		self.default = default
 		self.section = section
 		self.listeners = []
 
@@ -67,16 +76,16 @@
 
 	def check_validate(self, value):
 		"""Call validate() and raise ValueError if value is not valid"""
 		if not self.validate(value):
 			raise ValueError
 
 
-	def get(self):
-		"""Return stored value, or the default if invalid or missing"""
+	def get(self) -> typing.Any:
+		"""Return the set value, or the default if invalid or missing"""
 		try:
 			if self.set_externally:
 				value = self.section.environment.get(self.name, self.datatype)
 			else:
 				value = self.section.storage.get(self.name, self.datatype)
 			self.check_validate(value)
 			return value
@@ -89,15 +98,16 @@
 			raise ValueError(f"New setting value {new_value} is invalid")
 		self.section.storage.set(self.name, new_value)
 		for listener in self.listeners:
 			threading.Thread(target=listener).start()
 
 	@property
 	def set_externally(self):
-		return backend.config.use_environment and self.section.environment.exists(self.name)
+		"""See if the value is set from the environment (like env vars or cli params)"""
+		return config.use_environment and self.section.environment.exists(self.name)
 
 	def reset(self):
 		"""Sets the setting back to its default value"""
 		self.set(self.default)
 
 
 	@property
@@ -116,11 +126,14 @@
 
 	def __iter__(self):
 		return self.value.__iter__()
 
 
 	def __eq__(self, other):
 		"""Supports comparing with actual types (and other settings)"""
-		if isinstance(other, Setting):
+		if isinstance(other, BaseSetting):
 			return (other.name == self.name) and (other.section == self.section)
 		elif isinstance(other, self.datatype):
 			return self.value == other
+
+
+Setting = BaseSetting  # for backwards compatibility
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `object-settings-4.0.5/settings/types.py` & `object-settings-4.1/src/settings/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
-from . import base
+from . import base, BaseSetting as _BaseSetting
 
 
 # Yes, all of these overlayed methods have to exist for IDE features to work,
 # one does not simply re- type hint an inherited variable
 
 
-class Toggle(base.Setting):
+class Toggle(_BaseSetting):
 	"""A boolean True/False"""
 	def __init__(self, name, default: bool, section=base.default_section):
 		super().__init__(bool, name, default, section)
 
 
 	def get(self) -> bool:
-		return super().get()
+		return bool(super().get())
 
 	def set(self, new_value: bool):
 		super().set(new_value)
 
 
 	@property
 	def value(self) -> bool:
@@ -34,25 +34,25 @@
 	def __bool__(self):
 		return self.value
 
 
 
 
 
-class Choice(base.Setting):
+class Choice(_BaseSetting):
 	"""Choose an option (str) from a list"""
 	def __init__(self, name, options: list[str], default: str, section=base.default_section):
 		self.options = options
 		super().__init__(str, name, default, section)
 
 	def validate(self, value):
 		return super().validate(value) and (value in self.options)
 
 	def get(self) -> str:
-		return super().get()
+		return str(super().get())
 
 	def set(self, new_value: str):
 		super().set(new_value)
 
 
 	@property
 	def value(self) -> str:
@@ -62,15 +62,15 @@
 	def value(self, new_value: str):
 		self.set(new_value)
 
 
 
 
 
-class Multichoice(base.Setting):
+class Multichoice(_BaseSetting):
 	"""Choose multiple options (str) from a list"""
 	def __init__(self, name, options: list[str], default_choices: list[str], section=base.default_section):
 		self.options = options
 		super().__init__(list, name, default_choices, section)
 
 
 	def validate(self, value):
@@ -79,15 +79,15 @@
 			all((item in self.options) for item in value),
 			all((type(item) == str) for item in value)
 		]
 		return all(conditions)
 
 
 	def get(self) -> list[str]:
-		return super().get()
+		return list(super().get())
 
 	def set(self, new_value: list[str]):
 
 
 		for value in new_value:
 			if value not in self.options:
 				raise ValueError(f"New value {new_value} not in options ({self.options})")
@@ -114,36 +114,36 @@
 		value.remove(item)
 		self.set(value)
 
 
 
 
 
-class Text(base.Setting):
+class Text(_BaseSetting):
 	"""Just normal text"""
 	def __init__(self, name, default: str, section=base.default_section):
 		super().__init__(str, name, default, section)
 
 	def get(self) -> str:
-		return super().get()
+		return str(super().get())
 
 	def set(self, new_value: str):
 		super().set(new_value)
 
 	@property
 	def value(self) -> str:
 		return self.get()
 
 	@value.setter
 	def value(self, new_value: str):
 		self.set(new_value)
 
 
 
-class Path(base.Setting):
+class Path(_BaseSetting):
 	"""A file path. Automatically converted between Windows and Unix paths."""
 	def __init__(self, name, default: str, has_to_exist: bool = False, section=base.default_section):
 		self.has_to_exist = has_to_exist
 		super().__init__(str, name, default, section)
 
 
 	def validate(self, value):
@@ -151,15 +151,15 @@
 		if self.has_to_exist:
 			return valid and os.path.exists(value)
 		else:
 			return valid
 
 
 	def get(self) -> str:
-		return super().get()
+		return str(super().get())
 
 	def set(self, new_value: str):
 		if os.name == 'nt':
 			new_value = new_value.replace('/', '\\')
 		else:
 			new_value = new_value.replace('\\', '/')
 		super().set(new_value)
@@ -171,15 +171,15 @@
 	@value.setter
 	def value(self, new_value: str):
 		self.set(new_value)
 
 
 
 
-class Number(base.Setting):
+class Number(_BaseSetting):
 	"""A number (int) that can be incremented and decremented"""
 	def __init__(self, name, default: int, lower_limit: int = 0, upper_limit: int = 100,
 	             section=base.default_section):
 		self.lower_limit = lower_limit
 		self.upper_limit = upper_limit
 		super().__init__(int, name, default, section)
 
@@ -188,15 +188,15 @@
 		if type(value) == int:  # The base method does check for this, but the size check could crash
 			return super().validate(value) and (self.lower_limit <= value <= self.upper_limit)
 		else:
 			return False
 
 
 	def get(self) -> int:
-		return super().get()
+		return int(super().get())
 
 	def set(self, new_value: int):
 		super().set(new_value)
 
 
 	@property
 	def value(self) -> int:
```

### Comparing `object-settings-4.0.5/settings_gui/tkinter/icons/checkmark-white.png` & `object-settings-4.1/src/settings_gui/tkinter/icons/checkmark-white.png`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/settings_gui/tkinter/icons/folder-white.png` & `object-settings-4.1/src/settings_gui/tkinter/icons/folder-white.png`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/settings_gui/tkinter/main.py` & `object-settings-4.1/src/settings_gui/tkinter/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import settings, tkinter
+import settings, tkinter, typing
 
 from ..config import config
 from . import section_frames, a
 
 
-class SettingsFrame(a.layer.Frame):
-	def __init__(self, master, autosave=True, save_button: str = None):
+class SettingsFrame(a.layer.Frame): # type: ignore
+	def __init__(self, master, autosave=True, save_button: typing.Optional[str] = None):
 		super().__init__(master)
 		self.sections = []
-		for section in settings.all_sections:
 
-			if section != settings.base.default_section:
-				a.layer.Frame(self).pack(pady=config.padding)  # padding
+		for section in settings.all_sections:
+			if section.settings != []:
+				a.layer.Frame(self).pack(pady=config.padding)  # for padding
 				a.layer.Label(self, text=section.name, font='big').pack(padx=config.padding)
-
-				self.sections.append(section_frames.SectionFrame(self, section, autosave=autosave))
-				self.sections[-1].pack(fill='x', expand=True, padx=2*config.padding, pady=3*config.padding)
+				section_frame = section_frames.SectionFrame(self, section, autosave=autosave)
+				section_frame.pack(fill='x', expand=True, padx=2*config.padding, pady=3*config.padding)
+				self.sections.append(section_frame)
 
 		if isinstance(save_button, str):
 			button = a.layer.Button(self, command=self.save_settings, text=save_button)
 			if a.is_ttk():
-				button.configure(style='Accent.TButton')
+				button.configure(style='Accent.TButton')  # type: ignore
 			button.pack(pady=config.padding*3)
 
 	def save_settings(self):
 		for section_frame in self.sections:
 			section_frame.save_settings()
 		if isinstance(self.master, SettingsWindow):
 			self.master.destroy()
 
 
 
 class SettingsWindow(tkinter.Toplevel):
-	def __init__(self, master, title="Settings", autosave=True, save_button: str = None):
+	def __init__(self, master, title="Settings", autosave=True, save_button: typing.Optional[str] = None):
 		super().__init__(master)
 		SettingsFrame(self, autosave, save_button).pack(padx=config.padding*2, pady=config.padding*2, fill='both')
 
 		self.title(title)
 	#	self.minsize(self.winfo_width(), self.winfo_height())
 		self.resizable(False, False)
```

### Comparing `object-settings-4.0.5/settings_gui/tkinter/section_frames.py` & `object-settings-4.1/src/settings_gui/tkinter/section_frames.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ..config import config
 from . import type_frames, a
 
 
 
 
-class SectionFrame(a.layer.Frame):
+class SectionFrame(a.layer.Frame): # type: ignore
 	def __init__(self, master, section: settings.Section, autosave=True):
 		super().__init__(master)
 		self.settings = []
 		self._pad()
 		for setting in section.settings:
 			for type, type_frame in type_frames.types.items():
 				if isinstance(setting, type):
```

### Comparing `object-settings-4.0.5/settings_gui/tkinter/type_frames.py` & `object-settings-4.1/src/settings_gui/tkinter/type_frames.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import tkinter as tk
 
 from ..config import config, strings
 from . import a
 
 
 
-
-class _Base(a.layer.Frame):
-	def __init__(self, master, setting: settings.base.Setting, autosave: bool, width_limit=30):
+class _Base(a.layer.Frame): # type: ignore
+	def __init__(self, master, setting: settings.BaseSetting, autosave: bool, width_limit=30):
 		super().__init__(master)
+		settings.BaseSetting
 		self.setting = setting
 		self.variable = tk.Variable()
-		self.widget: a.layer.Widget | None = None
+		self.widget: a.layer.Widget | None = None # type: ignore
 		self.autosave = autosave
 		self.width_limit = width_limit
 
 		self.error_photoimage = tk.PhotoImage(file=_icon_path('error'))
 		self.error_icon = _AppearingWidget(a.layer.Label(self, image=self.error_photoimage))
 
 		a.layer.Label(self, text=setting.name).pack(side='left', padx=config.padding)
@@ -25,15 +25,15 @@
 		self.init()
 
 		# Settings set from envvars can't be changed
 		if self.setting.set_externally:
 			self.widget = a.layer.Label(self, text=strings.set_from_env, foreground='gray')
 
 		if isinstance(self.widget, a.layer.Widget):
-			self.widget: a.layer.Widget
+			self.widget: a.layer.Widget # type: ignore
 			self.widget.pack(side='right', padx=config.padding)
 
 		if isinstance(self.widget, (a.layer.Entry, a.layer.Spinbox, a.layer.OptionMenu)):
 			self.variable.trace_add('write', self.update_width)
 			self.variable.trace_add('write', self.validate)
 
 		self.variable.set(self.setting.get())
@@ -80,24 +80,26 @@
 
 	def save_from_widget(self, *args):
 		if self.autosave:
 			self.save()
 
 
 
+
 class Toggle(_Base):
 	"""A checkbutton, or a switch if available from ttk theme"""
 	def init(self):
 		self.variable = tk.BooleanVar()
 		self.widget = a.layer.Checkbutton(self, variable=self.variable, command=self.save_from_widget)
 		if a.is_ttk():
 			self.widget.configure(style='Switch.TCheckbutton')
 
 
 
+
 class Choice(_Base):
 	"""A horizontal radiobutton-row or an expandable menu, depending on the number of options"""
 	def init(self):
 		self.setting: settings.Choice
 		self.variable = tk.StringVar()
 		if _options_size(self.setting) <= self.width_limit:
 			frame = a.layer.Frame(self)
@@ -107,14 +109,15 @@
 			self.widget = frame
 		else:
 			self.widget = a.layer.OptionMenu(self, self.variable, self.setting.value, *self.setting.options,
 			                                 command=self.save_from_widget)
 
 
 
+
 class Multichoice(_Base):
 	"""Either a horizontal or vertical checkbutton-row, depending on the number of options"""
 	def init(self):
 		self.setting: settings.Multichoice
 		self.variable = self.MultichoiceVar(self.setting.options)
 		self.widget = a.layer.Frame(self)
 		direction = 'left' if (_options_size(self.setting) <= self.width_limit) else 'top'
@@ -165,15 +168,15 @@
 		super().save_from_widget(*args)
 		self.done_button.hide()
 
 
 	def icon_button(self, icon: str, command: typing.Callable):
 
 		if a.is_ttk():
-			hex = a.layer.Style().lookup('TButton', 'background')
+			hex = a.layer.Style().lookup('TButton', 'background') # type: ignore
 			hex = str(hex).removeprefix('#')
 			rgb = tuple(int(hex[i:i + 2], 16) for i in (0, 2, 4))
 			hls = colorsys.rgb_to_hls(*rgb)
 			brightness = hls[1]
 			if brightness > 50:
 				icon += '-black'
 			else:
@@ -185,14 +188,15 @@
 
 		icon_image = tk.PhotoImage(file=path)
 		self.icons.append(icon_image)
 		return a.layer.Button(self, image=icon_image, command=command)
 
 
 
+
 class Path(Text):
 	"""Like Text, but with a button to open a file chooser"""
 	def init(self):
 		super().init()
 		if not self.setting.set_externally:
 			self.icon_button('folder', self.browse).pack(side='right', padx=config.padding)
 
@@ -204,36 +208,61 @@
 				self.variable.set(dir)
 		except FileNotFoundError:
 			def open(func):
 				dir = func(initialdir=os.path.expanduser('~'))
 				if dir:
 					self.variable.set(dir)
 			popup = tk.Menu(self, tearoff=False)
-			popup.add_command(label=strings.file, command=lambda: open(tk.filedialog.askopenfilename))
-			popup.add_command(label=strings.dir, command=lambda: open(tk.filedialog.askdirectory))
+			popup.add_command(label=strings.file, command=lambda: open(tkinter.filedialog.askopenfilename))
+			popup.add_command(label=strings.dir, command=lambda: open(tkinter.filedialog.askdirectory))
 			popup.tk_popup(*self.winfo_pointerxy())
 
 
 
 
-
 class Number(_Base):
 	"""Spinbox that allows to increment/decrement (or manually type in)"""
 	def init(self):
 		self.setting: settings.Number
 		self.variable = tk.IntVar()
 		self.widget = a.layer.Spinbox(self, textvariable=self.variable,
 		                              from_=self.setting.lower_limit, to=self.setting.upper_limit)
 		self.variable.trace_add('write', self.save_from_widget)
 
 
 
 
 
 
+
+
+
+types = {
+	settings.Toggle: Toggle,
+	settings.Text: Text,
+	settings.Choice: Choice,
+	settings.Multichoice: Multichoice,
+	settings.Path: Path,
+	settings.Number: Number
+}
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 def _icon_path(icon: str):
 	if '.' not in icon:
 		icon += '.png'
 	return os.path.join(os.path.dirname(__file__), 'icons', icon)
 
 
 def _options_size(setting):
@@ -241,39 +270,20 @@
 	icons = len(setting.options) * 3
 	return text + icons
 
 
 
 
 class _AppearingWidget:
-	def __init__(self, widget: a.layer.Widget):
+	def __init__(self, widget: a.layer.Widget): # type: ignore
 		self.widget = widget
 		self.visible = False
 
-	# def isvisible(self):
-	# 	try:
-	# 		self.widget.pack_info()
-	# 		return True
-	# 	except tk.TclError:
-	# 		return False
-
 	def show(self):
 		if not self.visible:
 			self.widget.pack(side='right', padx=config.padding*2)
 			self.visible = True
 
 	def hide(self):
 		if self.visible:
 			self.widget.forget()
 			self.visible = False
-
-
-
-
-types = {
-	settings.Toggle: Toggle,
-	settings.Text: Text,
-	settings.Choice: Choice,
-	settings.Multichoice: Multichoice,
-	settings.Path: Path,
-	settings.Number: Number
-}
```

### Comparing `object-settings-4.0.5/settings_gui/ttk/__init__.py` & `object-settings-4.1/src/settings_gui/ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/tests/test_cli.py` & `object-settings-4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/tests/test_datafiles.py` & `object-settings-4.1/tests/test_datafiles.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/tests/test_datatype_loader.py` & `object-settings-4.1/tests/test_datatype_loader.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/tests/test_endurance.py` & `object-settings-4.1/tests/test_endurance.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/tests/test_env.py` & `object-settings-4.1/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/tests/test_gui_(manual).py` & `object-settings-4.1/tests/test_gui_(manual).py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 def test_tkinter():
 
 	import tkinter
 	window = tkinter.Tk()
 	window.title("Check that tkinter GUI looks right")
 
 	import settings_gui.tkinter
+	settings.base.default_section.settings.clear()
 	frame = settings_gui.tkinter.SettingsFrame(window)
 	assert isinstance(frame, tkinter.Frame)
 	frame.pack(padx=5, pady=5, fill='both')
 
 	window.mainloop()
 
 
@@ -41,14 +42,15 @@
 
 	import sv_ttk
 	sv_ttk.set_theme('dark')
 
 	import settings_gui.ttk
 	settings_gui.config.config(padding=4)
 	tkinter.ttk.Frame(window).pack(pady=2)
+	settings.base.default_section.settings.clear()
 	frame = settings_gui.ttk.SettingsFrame(window)
 	assert isinstance(frame, tkinter.ttk.Frame)
 	for section in frame.sections:
 		section.configure(style='Card.TFrame')
 	frame.pack(padx=5, pady=5, fill='both')
 
 	window.mainloop()
```

### Comparing `object-settings-4.0.5/tests/test_v1_definitions.py` & `object-settings-4.1/tests/test_v1_definitions.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.5/tests/test_validation.py` & `object-settings-4.1/tests/test_validation.py`

 * *Files identical despite different names*

