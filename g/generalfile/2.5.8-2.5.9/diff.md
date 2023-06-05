# Comparing `tmp/generalfile-2.5.8.tar.gz` & `tmp/generalfile-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalfile-2.5.8.tar", last modified: Thu Sep  1 04:56:53 2022, max compression
+gzip compressed data, was "generalfile-2.5.9.tar", last modified: Thu Sep  8 17:53:30 2022, max compression
```

## Comparing `generalfile-2.5.8.tar` & `generalfile-2.5.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 04:56:53.680245 generalfile-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-01 04:56:24.000000 generalfile-2.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-01 04:56:29.000000 generalfile-2.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    19934 2022-09-01 04:56:53.680245 generalfile-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18231 2022-09-01 04:56:51.000000 generalfile-2.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 04:56:53.676245 generalfile-2.5.8/generalfile/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5910 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/configfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 04:56:53.676245 generalfile-2.5.8/generalfile/optional_dependencies/
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/optional_dependencies/_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/optional_dependencies/path_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/optional_dependencies/path_pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     6144 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/optional_dependencies/path_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/optional_dependencies/path_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 04:56:53.676245 generalfile-2.5.8/generalfile/path_bases/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path_bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path_bases/path_diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path_bases/path_envs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path_bases/path_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)    16786 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path_bases/path_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path_bases/path_scrub.py
--rw-r--r--   0 runner    (1001) docker     (121)     8755 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/path_bases/path_strings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 04:56:53.680245 generalfile-2.5.8/generalfile/test/
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/setup_workdir.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)    11127 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/test_configfile.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/test_generalfile.py
--rw-r--r--   0 runner    (1001) docker     (121)    25073 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/test_path.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/test_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-09-01 04:54:03.000000 generalfile-2.5.8/generalfile/test/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 04:56:53.676245 generalfile-2.5.8/generalfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19934 2022-09-01 04:56:53.000000 generalfile-2.5.8/generalfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-09-01 04:56:53.000000 generalfile-2.5.8/generalfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 04:56:53.000000 generalfile-2.5.8/generalfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-01 04:56:53.000000 generalfile-2.5.8/generalfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-01 04:56:53.000000 generalfile-2.5.8/generalfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-01 04:56:24.000000 generalfile-2.5.8/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-01 04:56:53.680245 generalfile-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-09-01 04:56:29.000000 generalfile-2.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 17:53:30.828871 generalfile-2.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-08 17:52:56.000000 generalfile-2.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-08 17:53:00.000000 generalfile-2.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    20275 2022-09-08 17:53:30.828871 generalfile-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18516 2022-09-08 17:53:29.000000 generalfile-2.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 17:53:30.824871 generalfile-2.5.9/generalfile/
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5910 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 17:53:30.824871 generalfile-2.5.9/generalfile/optional_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/optional_dependencies/_extension.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/optional_dependencies/path_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/optional_dependencies/path_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6144 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/optional_dependencies/path_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/optional_dependencies/path_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 17:53:30.824871 generalfile-2.5.9/generalfile/path_bases/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path_bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path_bases/path_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path_bases/path_envs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path_bases/path_lock.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16786 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path_bases/path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3282 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path_bases/path_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8921 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/path_bases/path_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 17:53:30.828871 generalfile-2.5.9/generalfile/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/setup_workdir.py
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11127 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/test_configfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/test_generalfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25734 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/test_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-09-08 17:50:37.000000 generalfile-2.5.9/generalfile/test/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 17:53:30.824871 generalfile-2.5.9/generalfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    20275 2022-09-08 17:53:30.000000 generalfile-2.5.9/generalfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-09-08 17:53:30.000000 generalfile-2.5.9/generalfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 17:53:30.000000 generalfile-2.5.9/generalfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-08 17:53:30.000000 generalfile-2.5.9/generalfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-08 17:53:30.000000 generalfile-2.5.9/generalfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-08 17:51:13.000000 generalfile-2.5.9/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 17:53:30.828871 generalfile-2.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-09-08 17:53:00.000000 generalfile-2.5.9/setup.py
```

### Comparing `generalfile-2.5.8/LICENSE` & `generalfile-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/PKG-INFO` & `generalfile-2.5.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,145 +1,152 @@
 Metadata-Version: 2.1
 Name: generalfile
-Version: 2.5.8
+Version: 2.5.9
 Summary: Easily manage files cross platform.
 Home-page: https://github.com/ManderaGeneral/generalfile
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Description: # generalfile
         Easily manage files cross platform.
         
-        This package and 3 other make up [ManderaGeneral](https://github.com/ManderaGeneral).
-        
-        ## Information
-        | Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                    | Cover   |
-        |:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:--------------------------------------------------------|:--------|
-        | [generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.8](https://pypi.org/project/generalfile/) | 2022-09-01 06:56 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [4](https://github.com/ManderaGeneral/generalfile#Todo) | 73.1 %  |
-        
         ## Contents
         <pre>
         <a href='#generalfile'>generalfile</a>
-        ├─ <a href='#Information'>Information</a>
         ├─ <a href='#Contents'>Contents</a>
+        ├─ <a href='#Examples'>Examples</a>
         ├─ <a href='#Installation'>Installation</a>
+        ├─ <a href='#Information'>Information</a>
         ├─ <a href='#Attributes'>Attributes</a>
+        ├─ <a href='#Contributions'>Contributions</a>
         └─ <a href='#Todo'>Todo</a>
         </pre>
         
+        
         ## Installation
         | Command                   | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   | <a href='https://pypi.org/project/send2trash'>send2trash</a>   | <a href='https://pypi.org/project/appdirs'>appdirs</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   | <a href='https://pypi.org/project/dill'>dill</a>   |
         |:--------------------------|:-----------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------|:-------------------------------------------------------|:---------------------------------------------------|
         | `pip install generalfile` | Yes                                                                    | Yes                                                            | Yes                                                      | Yes                                                    | Yes                                                |
         
+        ## Information
+        | Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                    | Cover   |
+        |:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:--------------------------------------------------------|:--------|
+        | [generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.9](https://pypi.org/project/generalfile/) | 2022-09-08 19:53 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     2 | [4](https://github.com/ManderaGeneral/generalfile#Todo) | 72.8 %  |
+        
         ## Attributes
         <pre>
-        <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/__init__.py#L1'>Module: generalfile</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/errors.py#L6'>Class: CaseSensitivityError</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L109'>Class: ConfigFile</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L139'>Method: exists</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L94'>Method: get_custom_serializers</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L102'>Method: get_field_dict_serializable</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L168'>Method: halt_getattr</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L15'>Method: read_hook_post</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L14'>Method: read_hook_pre</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L148'>Method: safe_equals</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L56'>Method: write_config</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L17'>Method: write_hook_post</a> <b>(Untested)</b>
-        │  └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L16'>Method: write_hook_pre</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/errors.py#L10'>Class: InvalidCharacterError</a>
-        └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path.py#L20'>Class: Path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path.py#L20'>Class: Path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L32'>Method: absolute</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_lock.py#L123'>Method: as_working_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_cfg.py#L13'>Property: cfg</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L426'>Method: contains</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L97'>Method: copy</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L158'>Method: copy_to_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L237'>Method: create_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L311'>Method: delete</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L343'>Method: delete_folder_content</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L216'>Method: empty</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L268'>Method: encode</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L94'>Method: endswith</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L204'>Method: exists</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L24'>Method: from_alternative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L40'>Method: get_active_venv</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L283'>Method: get_cache_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L399'>Method: get_differing_files</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L293'>Method: get_lock_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L302'>Method: get_lock_path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L25'>Method: get_parent_package</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L32'>Method: get_parent_repo</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L18'>Method: get_parent_venv</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L255'>Method: get_working_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L59'>Method: is_absolute</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L174'>Method: is_file</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L180'>Method: is_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L381'>Method: is_identical</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L10'>Method: is_package</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L66'>Method: is_relative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L14'>Method: is_repo</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L186'>Method: is_root</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L6'>Method: is_venv</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_lock.py#L114'>Method: lock</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L261'>Method: match</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L73'>Method: mirror_path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L166'>Method: move</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L153'>Method: name</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L247'>Method: open_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L31'>Method: open_operation</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L446'>Method: pack</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L145'>Method: parts</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_pickle.py#L12'>Property: pickle</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L64'>Method: read</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L42'>Method: relative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L120'>Method: remove_end</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L103'>Method: remove_start</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L73'>Method: rename</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L195'>Method: root</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L136'>Method: same_destination</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_scrub.py#L10'>Method: scrub</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L360'>Method: seconds_since_creation</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L368'>Method: seconds_since_modified</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L274'>Method: set_working_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L375'>Method: size</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L20'>Method: spawn_children</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L11'>Method: spawn_parents</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_spreadsheet.py#L13'>Property: spreadsheet</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L85'>Method: startswith</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L169'>Method: stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L201'>Method: suffix</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L245'>Method: suffixes</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_text.py#L12'>Property: text</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L16'>Method: to_alternative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L332'>Method: trash</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L352'>Method: trash_folder_content</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L185'>Method: true_stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L465'>Method: unpack</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L7'>Method: view_paths</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L160'>Method: with_name</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L176'>Method: with_stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L209'>Method: with_suffix</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L252'>Method: with_suffixes</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L192'>Method: with_true_stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L228'>Method: without_file</a>
-           └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L51'>Method: write</a>
+        <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/__init__.py#L1'>Module: generalfile</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/errors.py#L6'>Class: CaseSensitivityError</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L109'>Class: ConfigFile</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L139'>Method: exists</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L94'>Method: get_custom_serializers</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L102'>Method: get_field_dict_serializable</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L168'>Method: halt_getattr</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L15'>Method: read_hook_post</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L14'>Method: read_hook_pre</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L148'>Method: safe_equals</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L56'>Method: write_config</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L17'>Method: write_hook_post</a> <b>(Untested)</b>
+        │  └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L16'>Method: write_hook_pre</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/errors.py#L10'>Class: InvalidCharacterError</a>
+        └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path.py#L20'>Class: Path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path.py#L20'>Class: Path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L32'>Method: absolute</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_lock.py#L123'>Method: as_working_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_cfg.py#L13'>Property: cfg</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L426'>Method: contains</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L97'>Method: copy</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L158'>Method: copy_to_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L237'>Method: create_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L311'>Method: delete</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L343'>Method: delete_folder_content</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L216'>Method: empty</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L275'>Method: encode</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L94'>Method: endswith</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L204'>Method: exists</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L268'>Method: forward_slash</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L24'>Method: from_alternative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L40'>Method: get_active_venv</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L283'>Method: get_cache_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L399'>Method: get_differing_files</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L293'>Method: get_lock_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L302'>Method: get_lock_path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L25'>Method: get_parent_package</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L32'>Method: get_parent_repo</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L18'>Method: get_parent_venv</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L255'>Method: get_working_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L59'>Method: is_absolute</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L174'>Method: is_file</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L180'>Method: is_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L381'>Method: is_identical</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L10'>Method: is_package</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L66'>Method: is_relative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L14'>Method: is_repo</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L186'>Method: is_root</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L6'>Method: is_venv</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_lock.py#L114'>Method: lock</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L261'>Method: match</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L73'>Method: mirror_path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L166'>Method: move</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L153'>Method: name</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L247'>Method: open_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L31'>Method: open_operation</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L446'>Method: pack</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L145'>Method: parts</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_pickle.py#L12'>Property: pickle</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L64'>Method: read</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L42'>Method: relative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L120'>Method: remove_end</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L103'>Method: remove_start</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L73'>Method: rename</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L195'>Method: root</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L136'>Method: same_destination</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_scrub.py#L10'>Method: scrub</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L360'>Method: seconds_since_creation</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L368'>Method: seconds_since_modified</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L274'>Method: set_working_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L375'>Method: size</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L20'>Method: spawn_children</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L11'>Method: spawn_parents</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_spreadsheet.py#L13'>Property: spreadsheet</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L85'>Method: startswith</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L169'>Method: stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L201'>Method: suffix</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L245'>Method: suffixes</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_text.py#L12'>Property: text</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L16'>Method: to_alternative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L332'>Method: trash</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L352'>Method: trash_folder_content</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L185'>Method: true_stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L465'>Method: unpack</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L7'>Method: view_paths</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L160'>Method: with_name</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L176'>Method: with_stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L209'>Method: with_suffix</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L252'>Method: with_suffixes</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L192'>Method: with_true_stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L228'>Method: without_file</a>
+           └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L51'>Method: write</a>
         </pre>
         
+        ## Contributions
+        Issue-creation and discussion is most welcome!
+        
+        Pull requests are **not wanted**, please discuss with me before investing any time.
+        
         ## Todo
         | Module                                                                                                                                               | Message                                                                                                                                                                                   |
         |:-----------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L1'>path_spreadsheet.py</a> | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L112'>Support DataFrame and Series with spreadsheet.append()</a> |
-        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L1'>path_lock.py</a>                          | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L12'>Lock the optional extra paths.</a>                                            |
         | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path.py#L1'>path.py</a>                                               | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path.py#L27'>Binary extension.</a>                                                                         |
         | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/configfile.py#L1'>configfile.py</a>                                   | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/configfile.py#L117'>Handle custom serializers within iterable for ConfigFile.</a>                          |
+        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L1'>path_lock.py</a>                          | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L12'>Lock the optional extra paths.</a>                                            |
+        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L1'>path_spreadsheet.py</a> | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L112'>Support DataFrame and Series with spreadsheet.append()</a> |
         
         <sup>
-        Generated 2022-09-01 06:56 CEST for commit <a href='https://github.com/ManderaGeneral/generalfile/commit/e054043'>e054043</a>.
+        Generated 2022-09-08 19:53 CEST for commit <a href='https://github.com/ManderaGeneral/generalfile/commit/ae8d109'>ae8d109</a>.
         </sup>
         
 Platform: UNKNOWN
 Classifier: Topic :: Desktop Environment :: File Managers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: generalfile Version: 2.5.8 Summary: Easily manage
+Metadata-Version: 2.1 Name: generalfile Version: 2.5.9 Summary: Easily manage
 files cross platform. Home-page: https://github.com/ManderaGeneral/generalfile
 Author: Rickard "Mandera" Abraham Author-email: rickard.abraham@gmail.com
-License: mit Description: # generalfile Easily manage files cross platform.
-This package and 3 other make up [ManderaGeneral](https://github.com/
-ManderaGeneral). ## Information | Package | Ver | Latest Release | Python |
-Platform | Lvl | Todo | Cover | |:---------------------------------------------
-----------------|:-----------------------------------------------|:------------
-----------|:-------------------------------------------------------------------
-------------------------------------------------------|:----------------|-----
--:|:--------------------------------------------------------|:--------| |
-[generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.8](https://
-pypi.org/project/generalfile/) | 2022-09-01 06:56 CEST | [3.8](https://
-www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/
-downloads/release/python-390/) | Windows, Ubuntu | 1 | [4](https://github.com/
-ManderaGeneral/generalfile#Todo) | 73.1 % | ## Contents
+License: mit Description: # generalfile Easily manage files cross platform. ##
+Contents
         generalfile
-        ââ Information
         ââ Contents
+        ââ Examples
         ââ Installation
+        ââ Information
         ââ Attributes
+        ââ Contributions
         ââ Todo
 ## Installation | Command | generallibrary | send2trash | appdirs | pandas |
 dill | |:--------------------------|:------------------------------------------
 -----------------------------|:------------------------------------------------
 ---------------|:---------------------------------------------------------|:---
 ----------------------------------------------------|:-------------------------
 --------------------------| | `pip install generalfile` | Yes | Yes | Yes | Yes
-| Yes | ## Attributes
+| Yes | ## Information | Package | Ver | Latest Release | Python | Platform |
+Lvl | Todo | Cover | |:--------------------------------------------------------
+-----|:-----------------------------------------------|:----------------------
+|:-----------------------------------------------------------------------------
+--------------------------------------------|:----------------|------:|:-------
+-------------------------------------------------|:--------| | [generalfile]
+(https://github.com/ManderaGeneral/generalfile) | [2.5.9](https://pypi.org/
+project/generalfile/) | 2022-09-08 19:53 CEST | [3.8](https://www.python.org/
+downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/
+python-390/) | Windows, Ubuntu | 2 | [4](https://github.com/ManderaGeneral/
+generalfile#Todo) | 72.8 % | ## Attributes
         Module:_generalfile
         ââ Class:_CaseSensitivityError
         ââ Class:_ConfigFile
         â  ââ Method:_exists
         â  ââ Method:_get_custom_serializers
         â  ââ Method:_get_field_dict_serializable (Untested)
         â  ââ Method:_halt_getattr (Untested)
@@ -52,22 +53,23 @@
            ââ Method:_create_folder
            ââ Method:_delete
            ââ Method:_delete_folder_content
            ââ Method:_empty
            ââ Method:_encode
            ââ Method:_endswith
            ââ Method:_exists
+           ââ Method:_forward_slash
            ââ Method:_from_alternative
            ââ Method:_get_active_venv (Untested)
            ââ Method:_get_cache_dir
            ââ Method:_get_differing_files
            ââ Method:_get_lock_dir
            ââ Method:_get_lock_path
            ââ Method:_get_parent_package (Untested)
-           ââ Method:_get_parent_repo (Untested)
+           ââ Method:_get_parent_repo
            ââ Method:_get_parent_venv (Untested)
            ââ Method:_get_working_dir
            ââ Method:_is_absolute
            ââ Method:_is_file
            ââ Method:_is_folder
            ââ Method:_is_identical
            ââ Method:_is_package (Untested)
@@ -114,21 +116,23 @@
            ââ Method:_with_name
            ââ Method:_with_stem
            ââ Method:_with_suffix
            ââ Method:_with_suffixes
            ââ Method:_with_true_stem
            ââ Method:_without_file
            ââ Method:_write
-## Todo | Module | Message | |:------------------------------------------------
+## Contributions Issue-creation and discussion is most welcome! Pull requests
+are **not wanted**, please discuss with me before investing any time. ## Todo |
+Module | Message | |:----------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------|:-------------------------------------------------------
+------------|:-----------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------| | path_spreadsheet.py |
-Support_DataFrame_and_Series_with_spreadsheet.append() | | path_lock.py | Lock
-the_optional_extra_paths. | | path.py | Binary_extension. | | configfile.py |
-Handle_custom_serializers_within_iterable_for_ConfigFile. | Generated 2022-09-
-01 06:56 CEST for commit e054043. Platform: UNKNOWN Classifier: Topic ::
-Desktop Environment :: File Managers Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: Microsoft ::
-Windows Classifier: Operating System :: POSIX :: Linux Requires-Python: >=3.8,
-<3.10 Description-Content-Type: text/markdown
+------------------------------------------| | path.py | Binary_extension. | |
+configfile.py | Handle_custom_serializers_within_iterable_for_ConfigFile. | |
+path_lock.py | Lock_the_optional_extra_paths. | | path_spreadsheet.py | Support
+DataFrame_and_Series_with_spreadsheet.append() | Generated 2022-09-08 19:53
+CEST for commit ae8d109. Platform: UNKNOWN Classifier: Topic :: Desktop
+Environment :: File Managers Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux Requires-Python: >=3.8, <3.10
+Description-Content-Type: text/markdown
```

### Comparing `generalfile-2.5.8/README.md` & `generalfile-2.5.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,138 @@
 # generalfile
 Easily manage files cross platform.
 
-This package and 3 other make up [ManderaGeneral](https://github.com/ManderaGeneral).
-
-## Information
-| Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                    | Cover   |
-|:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:--------------------------------------------------------|:--------|
-| [generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.8](https://pypi.org/project/generalfile/) | 2022-09-01 06:56 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [4](https://github.com/ManderaGeneral/generalfile#Todo) | 73.1 %  |
-
 ## Contents
 <pre>
 <a href='#generalfile'>generalfile</a>
-├─ <a href='#Information'>Information</a>
 ├─ <a href='#Contents'>Contents</a>
+├─ <a href='#Examples'>Examples</a>
 ├─ <a href='#Installation'>Installation</a>
+├─ <a href='#Information'>Information</a>
 ├─ <a href='#Attributes'>Attributes</a>
+├─ <a href='#Contributions'>Contributions</a>
 └─ <a href='#Todo'>Todo</a>
 </pre>
 
+
 ## Installation
 | Command                   | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   | <a href='https://pypi.org/project/send2trash'>send2trash</a>   | <a href='https://pypi.org/project/appdirs'>appdirs</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   | <a href='https://pypi.org/project/dill'>dill</a>   |
 |:--------------------------|:-----------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------|:-------------------------------------------------------|:---------------------------------------------------|
 | `pip install generalfile` | Yes                                                                    | Yes                                                            | Yes                                                      | Yes                                                    | Yes                                                |
 
+## Information
+| Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                    | Cover   |
+|:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:--------------------------------------------------------|:--------|
+| [generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.9](https://pypi.org/project/generalfile/) | 2022-09-08 19:53 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     2 | [4](https://github.com/ManderaGeneral/generalfile#Todo) | 72.8 %  |
+
 ## Attributes
 <pre>
-<a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/__init__.py#L1'>Module: generalfile</a>
-├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/errors.py#L6'>Class: CaseSensitivityError</a>
-├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L109'>Class: ConfigFile</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L139'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L94'>Method: get_custom_serializers</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L102'>Method: get_field_dict_serializable</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L168'>Method: halt_getattr</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L15'>Method: read_hook_post</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L14'>Method: read_hook_pre</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L148'>Method: safe_equals</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L56'>Method: write_config</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L17'>Method: write_hook_post</a> <b>(Untested)</b>
-│  └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L16'>Method: write_hook_pre</a> <b>(Untested)</b>
-├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/errors.py#L10'>Class: InvalidCharacterError</a>
-└─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path.py#L20'>Class: Path</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path.py#L20'>Class: Path</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L32'>Method: absolute</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_lock.py#L123'>Method: as_working_dir</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_cfg.py#L13'>Property: cfg</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L426'>Method: contains</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L97'>Method: copy</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L158'>Method: copy_to_folder</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L237'>Method: create_folder</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L311'>Method: delete</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L343'>Method: delete_folder_content</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L216'>Method: empty</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L268'>Method: encode</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L94'>Method: endswith</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L204'>Method: exists</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L24'>Method: from_alternative</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L40'>Method: get_active_venv</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L283'>Method: get_cache_dir</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L399'>Method: get_differing_files</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L293'>Method: get_lock_dir</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L302'>Method: get_lock_path</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L25'>Method: get_parent_package</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L32'>Method: get_parent_repo</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L18'>Method: get_parent_venv</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L255'>Method: get_working_dir</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L59'>Method: is_absolute</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L174'>Method: is_file</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L180'>Method: is_folder</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L381'>Method: is_identical</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L10'>Method: is_package</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L66'>Method: is_relative</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L14'>Method: is_repo</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L186'>Method: is_root</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L6'>Method: is_venv</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_lock.py#L114'>Method: lock</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L261'>Method: match</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L73'>Method: mirror_path</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L166'>Method: move</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L153'>Method: name</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L247'>Method: open_folder</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L31'>Method: open_operation</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L446'>Method: pack</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L145'>Method: parts</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_pickle.py#L12'>Property: pickle</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L64'>Method: read</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L42'>Method: relative</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L120'>Method: remove_end</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L103'>Method: remove_start</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L73'>Method: rename</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L195'>Method: root</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L136'>Method: same_destination</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_scrub.py#L10'>Method: scrub</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L360'>Method: seconds_since_creation</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L368'>Method: seconds_since_modified</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L274'>Method: set_working_dir</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L375'>Method: size</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L20'>Method: spawn_children</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L11'>Method: spawn_parents</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_spreadsheet.py#L13'>Property: spreadsheet</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L85'>Method: startswith</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L169'>Method: stem</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L201'>Method: suffix</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L245'>Method: suffixes</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_text.py#L12'>Property: text</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L16'>Method: to_alternative</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L332'>Method: trash</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L352'>Method: trash_folder_content</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L185'>Method: true_stem</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L465'>Method: unpack</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L7'>Method: view_paths</a> <b>(Untested)</b>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L160'>Method: with_name</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L176'>Method: with_stem</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L209'>Method: with_suffix</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L252'>Method: with_suffixes</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L192'>Method: with_true_stem</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L228'>Method: without_file</a>
-   └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L51'>Method: write</a>
+<a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/__init__.py#L1'>Module: generalfile</a>
+├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/errors.py#L6'>Class: CaseSensitivityError</a>
+├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L109'>Class: ConfigFile</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L139'>Method: exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L94'>Method: get_custom_serializers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L102'>Method: get_field_dict_serializable</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L168'>Method: halt_getattr</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L15'>Method: read_hook_post</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L14'>Method: read_hook_pre</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L148'>Method: safe_equals</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L56'>Method: write_config</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L17'>Method: write_hook_post</a> <b>(Untested)</b>
+│  └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L16'>Method: write_hook_pre</a> <b>(Untested)</b>
+├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/errors.py#L10'>Class: InvalidCharacterError</a>
+└─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path.py#L20'>Class: Path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path.py#L20'>Class: Path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L32'>Method: absolute</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_lock.py#L123'>Method: as_working_dir</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_cfg.py#L13'>Property: cfg</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L426'>Method: contains</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L97'>Method: copy</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L158'>Method: copy_to_folder</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L237'>Method: create_folder</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L311'>Method: delete</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L343'>Method: delete_folder_content</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L216'>Method: empty</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L275'>Method: encode</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L94'>Method: endswith</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L204'>Method: exists</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L268'>Method: forward_slash</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L24'>Method: from_alternative</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L40'>Method: get_active_venv</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L283'>Method: get_cache_dir</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L399'>Method: get_differing_files</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L293'>Method: get_lock_dir</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L302'>Method: get_lock_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L25'>Method: get_parent_package</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L32'>Method: get_parent_repo</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L18'>Method: get_parent_venv</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L255'>Method: get_working_dir</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L59'>Method: is_absolute</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L174'>Method: is_file</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L180'>Method: is_folder</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L381'>Method: is_identical</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L10'>Method: is_package</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L66'>Method: is_relative</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L14'>Method: is_repo</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L186'>Method: is_root</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L6'>Method: is_venv</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_lock.py#L114'>Method: lock</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L261'>Method: match</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L73'>Method: mirror_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L166'>Method: move</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L153'>Method: name</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L247'>Method: open_folder</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L31'>Method: open_operation</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L446'>Method: pack</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L145'>Method: parts</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_pickle.py#L12'>Property: pickle</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L64'>Method: read</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L42'>Method: relative</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L120'>Method: remove_end</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L103'>Method: remove_start</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L73'>Method: rename</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L195'>Method: root</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L136'>Method: same_destination</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_scrub.py#L10'>Method: scrub</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L360'>Method: seconds_since_creation</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L368'>Method: seconds_since_modified</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L274'>Method: set_working_dir</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L375'>Method: size</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L20'>Method: spawn_children</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L11'>Method: spawn_parents</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_spreadsheet.py#L13'>Property: spreadsheet</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L85'>Method: startswith</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L169'>Method: stem</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L201'>Method: suffix</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L245'>Method: suffixes</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_text.py#L12'>Property: text</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L16'>Method: to_alternative</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L332'>Method: trash</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L352'>Method: trash_folder_content</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L185'>Method: true_stem</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L465'>Method: unpack</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L7'>Method: view_paths</a> <b>(Untested)</b>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L160'>Method: with_name</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L176'>Method: with_stem</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L209'>Method: with_suffix</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L252'>Method: with_suffixes</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L192'>Method: with_true_stem</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L228'>Method: without_file</a>
+   └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L51'>Method: write</a>
 </pre>
 
+## Contributions
+Issue-creation and discussion is most welcome!
+
+Pull requests are **not wanted**, please discuss with me before investing any time.
+
 ## Todo
 | Module                                                                                                                                               | Message                                                                                                                                                                                   |
 |:-----------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L1'>path_spreadsheet.py</a> | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L112'>Support DataFrame and Series with spreadsheet.append()</a> |
-| <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L1'>path_lock.py</a>                          | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L12'>Lock the optional extra paths.</a>                                            |
 | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path.py#L1'>path.py</a>                                               | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path.py#L27'>Binary extension.</a>                                                                         |
 | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/configfile.py#L1'>configfile.py</a>                                   | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/configfile.py#L117'>Handle custom serializers within iterable for ConfigFile.</a>                          |
+| <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L1'>path_lock.py</a>                          | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L12'>Lock the optional extra paths.</a>                                            |
+| <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L1'>path_spreadsheet.py</a> | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L112'>Support DataFrame and Series with spreadsheet.append()</a> |
 
 <sup>
-Generated 2022-09-01 06:56 CEST for commit <a href='https://github.com/ManderaGeneral/generalfile/commit/e054043'>e054043</a>.
+Generated 2022-09-08 19:53 CEST for commit <a href='https://github.com/ManderaGeneral/generalfile/commit/ae8d109'>ae8d109</a>.
 </sup>
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-# generalfile Easily manage files cross platform. This package and 3 other make
-up [ManderaGeneral](https://github.com/ManderaGeneral). ## Information |
-Package | Ver | Latest Release | Python | Platform | Lvl | Todo | Cover | |:---
-----------------------------------------------------------|:-------------------
-----------------------------|:----------------------|:-------------------------
--------------------------------------------------------------------------------
------------------|:----------------|------:|:----------------------------------
-----------------------|:--------| | [generalfile](https://github.com/
-ManderaGeneral/generalfile) | [2.5.8](https://pypi.org/project/generalfile/) |
-2022-09-01 06:56 CEST | [3.8](https://www.python.org/downloads/release/python-
-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows,
-Ubuntu | 1 | [4](https://github.com/ManderaGeneral/generalfile#Todo) | 73.1 % |
-## Contents
+# generalfile Easily manage files cross platform. ## Contents
 generalfile
-ââ Information
 ââ Contents
+ââ Examples
 ââ Installation
+ââ Information
 ââ Attributes
+ââ Contributions
 ââ Todo
 ## Installation | Command | generallibrary | send2trash | appdirs | pandas |
 dill | |:--------------------------|:------------------------------------------
 -----------------------------|:------------------------------------------------
 ---------------|:---------------------------------------------------------|:---
 ----------------------------------------------------|:-------------------------
 --------------------------| | `pip install generalfile` | Yes | Yes | Yes | Yes
-| Yes | ## Attributes
+| Yes | ## Information | Package | Ver | Latest Release | Python | Platform |
+Lvl | Todo | Cover | |:--------------------------------------------------------
+-----|:-----------------------------------------------|:----------------------
+|:-----------------------------------------------------------------------------
+--------------------------------------------|:----------------|------:|:-------
+-------------------------------------------------|:--------| | [generalfile]
+(https://github.com/ManderaGeneral/generalfile) | [2.5.9](https://pypi.org/
+project/generalfile/) | 2022-09-08 19:53 CEST | [3.8](https://www.python.org/
+downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/
+python-390/) | Windows, Ubuntu | 2 | [4](https://github.com/ManderaGeneral/
+generalfile#Todo) | 72.8 % | ## Attributes
 Module:_generalfile
 ââ Class:_CaseSensitivityError
 ââ Class:_ConfigFile
 â  ââ Method:_exists
 â  ââ Method:_get_custom_serializers
 â  ââ Method:_get_field_dict_serializable (Untested)
 â  ââ Method:_halt_getattr (Untested)
@@ -49,22 +49,23 @@
    ââ Method:_create_folder
    ââ Method:_delete
    ââ Method:_delete_folder_content
    ââ Method:_empty
    ââ Method:_encode
    ââ Method:_endswith
    ââ Method:_exists
+   ââ Method:_forward_slash
    ââ Method:_from_alternative
    ââ Method:_get_active_venv (Untested)
    ââ Method:_get_cache_dir
    ââ Method:_get_differing_files
    ââ Method:_get_lock_dir
    ââ Method:_get_lock_path
    ââ Method:_get_parent_package (Untested)
-   ââ Method:_get_parent_repo (Untested)
+   ââ Method:_get_parent_repo
    ââ Method:_get_parent_venv (Untested)
    ââ Method:_get_working_dir
    ââ Method:_is_absolute
    ââ Method:_is_file
    ââ Method:_is_folder
    ââ Method:_is_identical
    ââ Method:_is_package (Untested)
@@ -111,16 +112,18 @@
    ââ Method:_with_name
    ââ Method:_with_stem
    ââ Method:_with_suffix
    ââ Method:_with_suffixes
    ââ Method:_with_true_stem
    ââ Method:_without_file
    ââ Method:_write
-## Todo | Module | Message | |:------------------------------------------------
+## Contributions Issue-creation and discussion is most welcome! Pull requests
+are **not wanted**, please discuss with me before investing any time. ## Todo |
+Module | Message | |:----------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------|:-------------------------------------------------------
+------------|:-----------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------| | path_spreadsheet.py |
-Support_DataFrame_and_Series_with_spreadsheet.append() | | path_lock.py | Lock
-the_optional_extra_paths. | | path.py | Binary_extension. | | configfile.py |
-Handle_custom_serializers_within_iterable_for_ConfigFile. | Generated 2022-09-
-01 06:56 CEST for commit e054043.
+------------------------------------------| | path.py | Binary_extension. | |
+configfile.py | Handle_custom_serializers_within_iterable_for_ConfigFile. | |
+path_lock.py | Lock_the_optional_extra_paths. | | path_spreadsheet.py | Support
+DataFrame_and_Series_with_spreadsheet.append() | Generated 2022-09-08 19:53
+CEST for commit ae8d109.
```

### Comparing `generalfile-2.5.8/generalfile/configfile.py` & `generalfile-2.5.9/generalfile/configfile.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/decorators.py` & `generalfile-2.5.9/generalfile/decorators.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/optional_dependencies/_extension.py` & `generalfile-2.5.9/generalfile/optional_dependencies/_extension.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/optional_dependencies/path_cfg.py` & `generalfile-2.5.9/generalfile/optional_dependencies/path_cfg.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/optional_dependencies/path_pickle.py` & `generalfile-2.5.9/generalfile/optional_dependencies/path_pickle.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/optional_dependencies/path_spreadsheet.py` & `generalfile-2.5.9/generalfile/optional_dependencies/path_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/optional_dependencies/path_text.py` & `generalfile-2.5.9/generalfile/optional_dependencies/path_text.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/path.py` & `generalfile-2.5.9/generalfile/path.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/path_bases/path_diagram.py` & `generalfile-2.5.9/generalfile/path_bases/path_diagram.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/path_bases/path_envs.py` & `generalfile-2.5.9/generalfile/path_bases/path_envs.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/path_bases/path_lock.py` & `generalfile-2.5.9/generalfile/path_bases/path_lock.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/path_bases/path_operations.py` & `generalfile-2.5.9/generalfile/path_bases/path_operations.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/path_bases/path_scrub.py` & `generalfile-2.5.9/generalfile/path_bases/path_scrub.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/path_bases/path_strings.py` & `generalfile-2.5.9/generalfile/path_bases/path_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,20 +261,26 @@
     def match(self, *patterns):
         """ Get whether this Path matches any given filter line.
 
             :param generalfile.Path self: """
         return match(self.path, *map(self._replace_delimiters, patterns))
 
     @deco_cache()
+    def forward_slash(self):
+        """ Return string path with forward slashes.
+
+            :param generalfile.Path self: """
+        return self.path.replace("\\", "/")
+
+    @deco_cache()
     def encode(self):
         """ Return a URL encoded string from this Path.
 
             :param generalfile.Path self: """
-        url = self.path.replace("\\", "/")
-        return quote(url)
+        return quote(self.forward_slash())
```

### Comparing `generalfile-2.5.8/generalfile/test/test_cfg.py` & `generalfile-2.5.9/generalfile/test/test_cfg.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/test/test_configfile.py` & `generalfile-2.5.9/generalfile/test/test_configfile.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/test/test_path.py` & `generalfile-2.5.9/generalfile/test/test_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 
 class PathTest(unittest.TestCase):
     def setUp(self):
         """Set working dir and clear folder. Set path delimiter to '/' for testing."""
         setup_workdir()
 
+    @classmethod
+    def tearDownClass(cls):
+        """Set working dir and clear folder. Set path delimiter to '/' for testing."""
+        setup_workdir()
+
 
 class FileTest(PathTest):
     """ Skipped: open_folder, view, scrub"""
     def test_path(self):
         self.assertRaises(InvalidCharacterError, Path, "hello:there")
         self.assertRaises(InvalidCharacterError, Path, "hello<")
         self.assertRaises(InvalidCharacterError, Path, "hello>")
@@ -445,14 +450,22 @@
         self.assertEqual(True, Path("foo/bar/hi").match("/bar/"))
         self.assertEqual(True, Path("foo/bar/hi").match("\\bar\\"))
 
         self.assertEqual(False, Path("hello/there").match("x"))
         self.assertEqual(False, Path("hello/there").match("*x*"))
         self.assertEqual(False, Path("hello/there").match("there/"))
 
+    def test_forward_slash(self):
+        self.assertEqual("foo/bar", Path("foo\\bar").forward_slash())
+        self.assertEqual("foo/bar", Path("foo/bar").forward_slash())
+        self.assertEqual("foo bar", Path("foo bar").forward_slash())
+        self.assertEqual("foo/bar/hi there", Path("foo/bar\\hi there").forward_slash())
+        self.assertEqual("_hello/there_now.py", Path("_hello/there_now.py").forward_slash())
+        self.assertEqual("foo/_bar_now", Path("foo\\_bar_now").forward_slash())
+
     def test_encode(self):
         self.assertEqual("foo/bar", Path("foo\\bar").encode())
         self.assertEqual("foo/bar", Path("foo/bar").encode())
         self.assertEqual("foo%20bar", Path("foo bar").encode())
         self.assertEqual("foo/bar/hi%20there", Path("foo/bar\\hi there").encode())
         self.assertEqual("_hello/there_now.py", Path("_hello/there_now.py").encode())
         self.assertEqual("foo/_bar_now", Path("foo\\_bar_now").encode())
```

### Comparing `generalfile-2.5.8/generalfile/test/test_pickle.py` & `generalfile-2.5.9/generalfile/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/test/test_spreadsheet.py` & `generalfile-2.5.9/generalfile/test/test_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile/test/test_text.py` & `generalfile-2.5.9/generalfile/test/test_text.py`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/generalfile.egg-info/PKG-INFO` & `generalfile-2.5.9/generalfile.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,145 +1,152 @@
 Metadata-Version: 2.1
 Name: generalfile
-Version: 2.5.8
+Version: 2.5.9
 Summary: Easily manage files cross platform.
 Home-page: https://github.com/ManderaGeneral/generalfile
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Description: # generalfile
         Easily manage files cross platform.
         
-        This package and 3 other make up [ManderaGeneral](https://github.com/ManderaGeneral).
-        
-        ## Information
-        | Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                    | Cover   |
-        |:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:--------------------------------------------------------|:--------|
-        | [generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.8](https://pypi.org/project/generalfile/) | 2022-09-01 06:56 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [4](https://github.com/ManderaGeneral/generalfile#Todo) | 73.1 %  |
-        
         ## Contents
         <pre>
         <a href='#generalfile'>generalfile</a>
-        ├─ <a href='#Information'>Information</a>
         ├─ <a href='#Contents'>Contents</a>
+        ├─ <a href='#Examples'>Examples</a>
         ├─ <a href='#Installation'>Installation</a>
+        ├─ <a href='#Information'>Information</a>
         ├─ <a href='#Attributes'>Attributes</a>
+        ├─ <a href='#Contributions'>Contributions</a>
         └─ <a href='#Todo'>Todo</a>
         </pre>
         
+        
         ## Installation
         | Command                   | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   | <a href='https://pypi.org/project/send2trash'>send2trash</a>   | <a href='https://pypi.org/project/appdirs'>appdirs</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   | <a href='https://pypi.org/project/dill'>dill</a>   |
         |:--------------------------|:-----------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------|:-------------------------------------------------------|:---------------------------------------------------|
         | `pip install generalfile` | Yes                                                                    | Yes                                                            | Yes                                                      | Yes                                                    | Yes                                                |
         
+        ## Information
+        | Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                    | Cover   |
+        |:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:--------------------------------------------------------|:--------|
+        | [generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.9](https://pypi.org/project/generalfile/) | 2022-09-08 19:53 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     2 | [4](https://github.com/ManderaGeneral/generalfile#Todo) | 72.8 %  |
+        
         ## Attributes
         <pre>
-        <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/__init__.py#L1'>Module: generalfile</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/errors.py#L6'>Class: CaseSensitivityError</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L109'>Class: ConfigFile</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L139'>Method: exists</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L94'>Method: get_custom_serializers</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L102'>Method: get_field_dict_serializable</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L168'>Method: halt_getattr</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L15'>Method: read_hook_post</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L14'>Method: read_hook_pre</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L148'>Method: safe_equals</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L56'>Method: write_config</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L17'>Method: write_hook_post</a> <b>(Untested)</b>
-        │  └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/configfile.py#L16'>Method: write_hook_pre</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/errors.py#L10'>Class: InvalidCharacterError</a>
-        └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path.py#L20'>Class: Path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path.py#L20'>Class: Path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L32'>Method: absolute</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_lock.py#L123'>Method: as_working_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_cfg.py#L13'>Property: cfg</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L426'>Method: contains</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L97'>Method: copy</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L158'>Method: copy_to_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L237'>Method: create_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L311'>Method: delete</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L343'>Method: delete_folder_content</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L216'>Method: empty</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L268'>Method: encode</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L94'>Method: endswith</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L204'>Method: exists</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L24'>Method: from_alternative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L40'>Method: get_active_venv</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L283'>Method: get_cache_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L399'>Method: get_differing_files</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L293'>Method: get_lock_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L302'>Method: get_lock_path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L25'>Method: get_parent_package</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L32'>Method: get_parent_repo</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L18'>Method: get_parent_venv</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L255'>Method: get_working_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L59'>Method: is_absolute</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L174'>Method: is_file</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L180'>Method: is_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L381'>Method: is_identical</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L10'>Method: is_package</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L66'>Method: is_relative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L14'>Method: is_repo</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L186'>Method: is_root</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_envs.py#L6'>Method: is_venv</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_lock.py#L114'>Method: lock</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L261'>Method: match</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L73'>Method: mirror_path</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L166'>Method: move</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L153'>Method: name</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L247'>Method: open_folder</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L31'>Method: open_operation</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L446'>Method: pack</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L145'>Method: parts</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_pickle.py#L12'>Property: pickle</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L64'>Method: read</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L42'>Method: relative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L120'>Method: remove_end</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L103'>Method: remove_start</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L73'>Method: rename</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L195'>Method: root</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L136'>Method: same_destination</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_scrub.py#L10'>Method: scrub</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L360'>Method: seconds_since_creation</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L368'>Method: seconds_since_modified</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L274'>Method: set_working_dir</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L375'>Method: size</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L20'>Method: spawn_children</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L11'>Method: spawn_parents</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_spreadsheet.py#L13'>Property: spreadsheet</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L85'>Method: startswith</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L169'>Method: stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L201'>Method: suffix</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L245'>Method: suffixes</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/optional_dependencies/path_text.py#L12'>Property: text</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L16'>Method: to_alternative</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L332'>Method: trash</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L352'>Method: trash_folder_content</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L185'>Method: true_stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L465'>Method: unpack</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_diagram.py#L7'>Method: view_paths</a> <b>(Untested)</b>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L160'>Method: with_name</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L176'>Method: with_stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L209'>Method: with_suffix</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L252'>Method: with_suffixes</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_strings.py#L192'>Method: with_true_stem</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L228'>Method: without_file</a>
-           └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/e054043/generalfile/path_bases/path_operations.py#L51'>Method: write</a>
+        <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/__init__.py#L1'>Module: generalfile</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/errors.py#L6'>Class: CaseSensitivityError</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L109'>Class: ConfigFile</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L139'>Method: exists</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L94'>Method: get_custom_serializers</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L102'>Method: get_field_dict_serializable</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L168'>Method: halt_getattr</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L15'>Method: read_hook_post</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L14'>Method: read_hook_pre</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L148'>Method: safe_equals</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L56'>Method: write_config</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L17'>Method: write_hook_post</a> <b>(Untested)</b>
+        │  └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/configfile.py#L16'>Method: write_hook_pre</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/errors.py#L10'>Class: InvalidCharacterError</a>
+        └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path.py#L20'>Class: Path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path.py#L20'>Class: Path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L32'>Method: absolute</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_lock.py#L123'>Method: as_working_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_cfg.py#L13'>Property: cfg</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L426'>Method: contains</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L97'>Method: copy</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L158'>Method: copy_to_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L237'>Method: create_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L311'>Method: delete</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L343'>Method: delete_folder_content</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L216'>Method: empty</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L275'>Method: encode</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L94'>Method: endswith</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L204'>Method: exists</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L268'>Method: forward_slash</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L24'>Method: from_alternative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L40'>Method: get_active_venv</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L283'>Method: get_cache_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L399'>Method: get_differing_files</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L293'>Method: get_lock_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L302'>Method: get_lock_path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L25'>Method: get_parent_package</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L32'>Method: get_parent_repo</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L18'>Method: get_parent_venv</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L255'>Method: get_working_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L59'>Method: is_absolute</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L174'>Method: is_file</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L180'>Method: is_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L381'>Method: is_identical</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L10'>Method: is_package</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L66'>Method: is_relative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L14'>Method: is_repo</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L186'>Method: is_root</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_envs.py#L6'>Method: is_venv</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_lock.py#L114'>Method: lock</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L261'>Method: match</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L73'>Method: mirror_path</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L166'>Method: move</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L153'>Method: name</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L247'>Method: open_folder</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L31'>Method: open_operation</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L446'>Method: pack</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L145'>Method: parts</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_pickle.py#L12'>Property: pickle</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L64'>Method: read</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L42'>Method: relative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L120'>Method: remove_end</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L103'>Method: remove_start</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L73'>Method: rename</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L195'>Method: root</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L136'>Method: same_destination</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_scrub.py#L10'>Method: scrub</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L360'>Method: seconds_since_creation</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L368'>Method: seconds_since_modified</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L274'>Method: set_working_dir</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L375'>Method: size</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L20'>Method: spawn_children</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L11'>Method: spawn_parents</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_spreadsheet.py#L13'>Property: spreadsheet</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L85'>Method: startswith</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L169'>Method: stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L201'>Method: suffix</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L245'>Method: suffixes</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/optional_dependencies/path_text.py#L12'>Property: text</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L16'>Method: to_alternative</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L332'>Method: trash</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L352'>Method: trash_folder_content</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L185'>Method: true_stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L465'>Method: unpack</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_diagram.py#L7'>Method: view_paths</a> <b>(Untested)</b>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L160'>Method: with_name</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L176'>Method: with_stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L209'>Method: with_suffix</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L252'>Method: with_suffixes</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_strings.py#L192'>Method: with_true_stem</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L228'>Method: without_file</a>
+           └─ <a href='https://github.com/ManderaGeneral/generalfile/blob/ae8d109/generalfile/path_bases/path_operations.py#L51'>Method: write</a>
         </pre>
         
+        ## Contributions
+        Issue-creation and discussion is most welcome!
+        
+        Pull requests are **not wanted**, please discuss with me before investing any time.
+        
         ## Todo
         | Module                                                                                                                                               | Message                                                                                                                                                                                   |
         |:-----------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L1'>path_spreadsheet.py</a> | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L112'>Support DataFrame and Series with spreadsheet.append()</a> |
-        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L1'>path_lock.py</a>                          | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L12'>Lock the optional extra paths.</a>                                            |
         | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path.py#L1'>path.py</a>                                               | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path.py#L27'>Binary extension.</a>                                                                         |
         | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/configfile.py#L1'>configfile.py</a>                                   | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/configfile.py#L117'>Handle custom serializers within iterable for ConfigFile.</a>                          |
+        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L1'>path_lock.py</a>                          | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/path_bases/path_lock.py#L12'>Lock the optional extra paths.</a>                                            |
+        | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L1'>path_spreadsheet.py</a> | <a href='https://github.com/ManderaGeneral/generalfile/blob/master/generalfile/optional_dependencies/path_spreadsheet.py#L112'>Support DataFrame and Series with spreadsheet.append()</a> |
         
         <sup>
-        Generated 2022-09-01 06:56 CEST for commit <a href='https://github.com/ManderaGeneral/generalfile/commit/e054043'>e054043</a>.
+        Generated 2022-09-08 19:53 CEST for commit <a href='https://github.com/ManderaGeneral/generalfile/commit/ae8d109'>ae8d109</a>.
         </sup>
         
 Platform: UNKNOWN
 Classifier: Topic :: Desktop Environment :: File Managers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: generalfile Version: 2.5.8 Summary: Easily manage
+Metadata-Version: 2.1 Name: generalfile Version: 2.5.9 Summary: Easily manage
 files cross platform. Home-page: https://github.com/ManderaGeneral/generalfile
 Author: Rickard "Mandera" Abraham Author-email: rickard.abraham@gmail.com
-License: mit Description: # generalfile Easily manage files cross platform.
-This package and 3 other make up [ManderaGeneral](https://github.com/
-ManderaGeneral). ## Information | Package | Ver | Latest Release | Python |
-Platform | Lvl | Todo | Cover | |:---------------------------------------------
-----------------|:-----------------------------------------------|:------------
-----------|:-------------------------------------------------------------------
-------------------------------------------------------|:----------------|-----
--:|:--------------------------------------------------------|:--------| |
-[generalfile](https://github.com/ManderaGeneral/generalfile) | [2.5.8](https://
-pypi.org/project/generalfile/) | 2022-09-01 06:56 CEST | [3.8](https://
-www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/
-downloads/release/python-390/) | Windows, Ubuntu | 1 | [4](https://github.com/
-ManderaGeneral/generalfile#Todo) | 73.1 % | ## Contents
+License: mit Description: # generalfile Easily manage files cross platform. ##
+Contents
         generalfile
-        ââ Information
         ââ Contents
+        ââ Examples
         ââ Installation
+        ââ Information
         ââ Attributes
+        ââ Contributions
         ââ Todo
 ## Installation | Command | generallibrary | send2trash | appdirs | pandas |
 dill | |:--------------------------|:------------------------------------------
 -----------------------------|:------------------------------------------------
 ---------------|:---------------------------------------------------------|:---
 ----------------------------------------------------|:-------------------------
 --------------------------| | `pip install generalfile` | Yes | Yes | Yes | Yes
-| Yes | ## Attributes
+| Yes | ## Information | Package | Ver | Latest Release | Python | Platform |
+Lvl | Todo | Cover | |:--------------------------------------------------------
+-----|:-----------------------------------------------|:----------------------
+|:-----------------------------------------------------------------------------
+--------------------------------------------|:----------------|------:|:-------
+-------------------------------------------------|:--------| | [generalfile]
+(https://github.com/ManderaGeneral/generalfile) | [2.5.9](https://pypi.org/
+project/generalfile/) | 2022-09-08 19:53 CEST | [3.8](https://www.python.org/
+downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/
+python-390/) | Windows, Ubuntu | 2 | [4](https://github.com/ManderaGeneral/
+generalfile#Todo) | 72.8 % | ## Attributes
         Module:_generalfile
         ââ Class:_CaseSensitivityError
         ââ Class:_ConfigFile
         â  ââ Method:_exists
         â  ââ Method:_get_custom_serializers
         â  ââ Method:_get_field_dict_serializable (Untested)
         â  ââ Method:_halt_getattr (Untested)
@@ -52,22 +53,23 @@
            ââ Method:_create_folder
            ââ Method:_delete
            ââ Method:_delete_folder_content
            ââ Method:_empty
            ââ Method:_encode
            ââ Method:_endswith
            ââ Method:_exists
+           ââ Method:_forward_slash
            ââ Method:_from_alternative
            ââ Method:_get_active_venv (Untested)
            ââ Method:_get_cache_dir
            ââ Method:_get_differing_files
            ââ Method:_get_lock_dir
            ââ Method:_get_lock_path
            ââ Method:_get_parent_package (Untested)
-           ââ Method:_get_parent_repo (Untested)
+           ââ Method:_get_parent_repo
            ââ Method:_get_parent_venv (Untested)
            ââ Method:_get_working_dir
            ââ Method:_is_absolute
            ââ Method:_is_file
            ââ Method:_is_folder
            ââ Method:_is_identical
            ââ Method:_is_package (Untested)
@@ -114,21 +116,23 @@
            ââ Method:_with_name
            ââ Method:_with_stem
            ââ Method:_with_suffix
            ââ Method:_with_suffixes
            ââ Method:_with_true_stem
            ââ Method:_without_file
            ââ Method:_write
-## Todo | Module | Message | |:------------------------------------------------
+## Contributions Issue-creation and discussion is most welcome! Pull requests
+are **not wanted**, please discuss with me before investing any time. ## Todo |
+Module | Message | |:----------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------|:-------------------------------------------------------
+------------|:-----------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------| | path_spreadsheet.py |
-Support_DataFrame_and_Series_with_spreadsheet.append() | | path_lock.py | Lock
-the_optional_extra_paths. | | path.py | Binary_extension. | | configfile.py |
-Handle_custom_serializers_within_iterable_for_ConfigFile. | Generated 2022-09-
-01 06:56 CEST for commit e054043. Platform: UNKNOWN Classifier: Topic ::
-Desktop Environment :: File Managers Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: Microsoft ::
-Windows Classifier: Operating System :: POSIX :: Linux Requires-Python: >=3.8,
-<3.10 Description-Content-Type: text/markdown
+------------------------------------------| | path.py | Binary_extension. | |
+configfile.py | Handle_custom_serializers_within_iterable_for_ConfigFile. | |
+path_lock.py | Lock_the_optional_extra_paths. | | path_spreadsheet.py | Support
+DataFrame_and_Series_with_spreadsheet.append() | Generated 2022-09-08 19:53
+CEST for commit ae8d109. Platform: UNKNOWN Classifier: Topic :: Desktop
+Environment :: File Managers Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux Requires-Python: >=3.8, <3.10
+Description-Content-Type: text/markdown
```

### Comparing `generalfile-2.5.8/generalfile.egg-info/SOURCES.txt` & `generalfile-2.5.9/generalfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generalfile-2.5.8/setup.py` & `generalfile-2.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 
-
 from setuptools import setup, find_namespace_packages
 from pathlib import Path
 
 try:
     long_description = (Path(__file__).parent / 'README.md').read_text(encoding='utf-8')
 except FileNotFoundError:
     long_description = 'Readme missing'
 
 setup(
     name="generalfile",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="2.5.8",
+    version="2.5.9",
     description="Easily manage files cross platform.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'generallibrary',
         'send2trash',
         'appdirs',
```

