# Comparing `tmp/taipy-config-2.3.0.dev0.tar.gz` & `tmp/taipy-config-2.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-config-2.3.0.dev0.tar", last modified: Tue May 23 11:54:05 2023, max compression
+gzip compressed data, was "taipy-config-2.3.0.dev1.tar", last modified: Mon Jun  5 15:43:13 2023, max compression
```

## Comparing `taipy-config-2.3.0.dev0.tar` & `taipy-config-2.3.0.dev1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.220262 taipy-config-2.3.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.224262 taipy-config-2.3.0.dev0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.224262 taipy-config-2.3.0.dev0/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.224262 taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.228262 taipy-config-2.3.0.dev0/src/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.228262 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/_comparator_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/_config_comparator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.232262 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_toml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.232262 taipy-config-2.3.0.dev0/src/taipy/config/checker/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.232262 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/issue_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_classproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_config_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_template_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_validate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    35297 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/config/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/config/global_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/global_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/global_app/global_app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/section.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/unique_section.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/logger/_taipy_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:53:56.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.339733 taipy-config-2.3.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_comparator_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_config_comparator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.347733 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_toml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.347733 taipy-config-2.3.0.dev1/src/taipy/config/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.347733 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_auth_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/issue_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_config_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_template_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_validate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35422 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/config/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/config/global_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/global_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/global_app/global_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/unique_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/logger/_taipy_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:43:05.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/top_level.txt
```

### Comparing `taipy-config-2.3.0.dev0/LICENSE` & `taipy-config-2.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/PKG-INFO` & `taipy-config-2.3.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.3.0.dev0
+Version: 2.3.0.dev1
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.3.0.dev0/README.md` & `taipy-config-2.3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/setup.py` & `taipy-config-2.3.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/_cli/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/_cli.py` & `taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_config.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/_comparator_result.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_comparator_result.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/_config_comparator.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_config_comparator.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_base_serializer.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_base_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_json_serializer.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_json_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_toml_serializer.py` & `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_toml_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/checker/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/config/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checker.py` & `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 from typing import List
 
 from ._checkers._config_checker import _ConfigChecker
-from ._checkers._gLobal_config_checker import _GlobalConfigChecker
+from ._checkers._global_config_checker import _GlobalConfigChecker
 from .issue_collector import IssueCollector
 
 
 class _Checker:
     """Holds the various checkers to perform on the config."""
 
     _checkers: List[_ConfigChecker] = [_GlobalConfigChecker]  # type: ignore
```

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py` & `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_auth_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py` & `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/checker/issue.py` & `taipy-config-2.3.0.dev1/src/taipy/config/checker/issue.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/checker/issue_collector.py` & `taipy-config-2.3.0.dev1/src/taipy/config/checker/issue_collector.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/_classproperty.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/_classproperty.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/_config_blocker.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/_config_blocker.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import functools
 
+from ...logger._taipy_logger import _TaipyLogger
 from ..exceptions.exceptions import ConfigurationUpdateBlocked
 
 
 class _ConfigBlocker:
     """Configuration blocker singleton."""
 
+    __logger = _TaipyLogger._get_logger()
     __block_config_update = False
 
     @classmethod
     def _block(cls):
         cls.__block_config_update = True
 
     @classmethod
@@ -29,14 +31,20 @@
 
     @classmethod
     def _check(cls):
         def inner(f):
             @functools.wraps(f)
             def _check_if_is_blocking(*args, **kwargs):
                 if cls.__block_config_update:
-                    raise ConfigurationUpdateBlocked()
+                    error_message = (
+                        "The Core service should be stopped by running core.stop() before"
+                        " modifying the Configuration. For more information, please refer to:"
+                        " https://docs.taipy.io/en/latest/manuals/running_services/#running-core."
+                    )
+                    cls.__logger.error("ConfigurationUpdateBlocked: " + error_message)
+                    raise ConfigurationUpdateBlocked(error_message)
 
                 return f(*args, **kwargs)
 
             return _check_if_is_blocking
 
         return inner
```

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/_repr_enum.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/_template_handler.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/_template_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/_validate_id.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/_validate_id.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/frequency.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/frequency.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/common/scope.py` & `taipy-config-2.3.0.dev1/src/taipy/config/common/scope.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/config.py` & `taipy-config-2.3.0.dev1/src/taipy/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """Load a configuration file to replace the current python config and trigger the Config compilation.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
         cls.__logger.info(f"Loading configuration. Filename: '{filename}'")
         cls._python_config = cls._serializer._read(filename)
-        cls.__compile_configs()
+        cls._compile_configs()
         cls.__logger.info(f"Configuration '{filename}' successfully loaded.")
 
     @classmethod
     def export(cls, filename):
         """Export a configuration.
 
         The export is done in a toml file.
@@ -120,15 +120,15 @@
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
         cls.__logger.info(f"Loading configuration. Filename: '{filename}'")
         cls._file_config = cls._serializer._read(filename)
         cls.__logger.info("Overriding configuration.'")
-        cls.__compile_configs()
+        cls._compile_configs()
         cls.__logger.info(f"Configuration '{filename}' successfully loaded.")
 
     @classmethod
     def block_update(cls):
         """Block update on the configuration signgleton."""
         _ConfigBlocker._block()
 
@@ -159,15 +159,15 @@
             The global application configuration.
         """
         glob_cfg = GlobalAppConfig(root_folder, storage_folder, clean_entities_enabled, **properties)
         if cls._python_config._global_config is None:
             cls._python_config._global_config = glob_cfg
         else:
             cls._python_config._global_config._update(glob_cfg._to_dict())
-        cls.__compile_configs()
+        cls._compile_configs()
         return cls._applied_config._global_config
 
     @classmethod
     def check(cls) -> IssueCollector:
         """Check configuration.
 
         This method logs issue messages and returns an issue collector.
@@ -190,15 +190,15 @@
         else:
             if def_sections := cls._default_config._sections.get(default_section.name, None):
                 def_sections[default_section.id] = default_section
             else:
                 cls._default_config._sections[default_section.name] = {default_section.id: default_section}
         cls._serializer._section_class[default_section.name] = default_section.__class__  # type: ignore
         cls.__json_serializer._section_class[default_section.name] = default_section.__class__  # type: ignore
-        cls.__compile_configs()
+        cls._compile_configs()
 
     @classmethod
     @_ConfigBlocker._check()
     def _register(cls, section):
         if isinstance(section, UniqueSection):
             if cls._python_config._unique_sections.get(section.name, None):
                 cls._python_config._unique_sections[section.name]._update(section._to_dict())
@@ -210,25 +210,25 @@
                     sections[section.id]._update(section._to_dict())
                 else:
                     sections[section.id] = section
             else:
                 cls._python_config._sections[section.name] = {section.id: section}
         cls._serializer._section_class[section.name] = section.__class__
         cls.__json_serializer._section_class[section.name] = section.__class__
-        cls.__compile_configs()
+        cls._compile_configs()
 
     @classmethod
     def _override_env_file(cls):
         if config_filename := os.environ.get(cls._ENVIRONMENT_VARIABLE_NAME_WITH_CONFIG_PATH):
             cls.__logger.info(f"Loading configuration provided by environment variable. Filename: '{config_filename}'")
             cls._env_file_config = cls._serializer._read(config_filename)
             cls.__logger.info(f"Configuration '{config_filename}' successfully loaded.")
 
     @classmethod
-    def __compile_configs(cls):
+    def _compile_configs(cls):
         Config._override_env_file()
         cls._applied_config = _Config._default_config()
         if cls._default_config:
             cls._applied_config._update(cls._default_config)
         if cls._python_config:
             cls._applied_config._update(cls._python_config)
         if cls._file_config:
```

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/config.pyi` & `taipy-config-2.3.0.dev1/src/taipy/config/config.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,18 @@
         """"""
 
     @classmethod
     def _override_env_file(cls):
         """"""
 
     @classmethod
+    def _compile_configs(cls):
+        """"""
+
+    @classmethod
     def _to_json(cls, _config: _Config) -> str:
         """"""
 
     @classmethod
     def _from_json(cls, config_as_str: str) -> _Config:
         """"""
 
@@ -168,14 +172,17 @@
 
     def pipelines(cls) -> Dict[str, PipelineConfig]:
         """"""
 
     def scenarios(cls) -> Dict[str, ScenarioConfig]:
         """"""
 
+    def core(cls) -> Dict[str, CoreSection]:
+        """"""
+
     @staticmethod
     def configure_scenario(
         id: str,
         pipeline_configs: List[PipelineConfig],
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
         **properties,
```

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/exceptions/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/config/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/exceptions/exceptions.py` & `taipy-config-2.3.0.dev1/src/taipy/config/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/global_app/global_app_config.py` & `taipy-config-2.3.0.dev1/src/taipy/config/global_app/global_app_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/section.py` & `taipy-config-2.3.0.dev1/src/taipy/config/section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/config/unique_section.py` & `taipy-config-2.3.0.dev1/src/taipy/config/unique_section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/logger/__init__.py` & `taipy-config-2.3.0.dev1/src/taipy/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy/logger/_taipy_logger.py` & `taipy-config-2.3.0.dev1/src/taipy/logger/_taipy_logger.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev0/src/taipy_config.egg-info/PKG-INFO` & `taipy-config-2.3.0.dev1/src/taipy_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.3.0.dev0
+Version: 2.3.0.dev1
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.3.0.dev0/src/taipy_config.egg-info/SOURCES.txt` & `taipy-config-2.3.0.dev1/src/taipy_config.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 src/taipy/config/checker/__init__.py
 src/taipy/config/checker/_checker.py
 src/taipy/config/checker/issue.py
 src/taipy/config/checker/issue_collector.py
 src/taipy/config/checker/_checkers/__init__.py
 src/taipy/config/checker/_checkers/_auth_config_checker.py
 src/taipy/config/checker/_checkers/_config_checker.py
-src/taipy/config/checker/_checkers/_gLobal_config_checker.py
+src/taipy/config/checker/_checkers/_global_config_checker.py
 src/taipy/config/common/__init__.py
 src/taipy/config/common/_classproperty.py
 src/taipy/config/common/_config_blocker.py
 src/taipy/config/common/_repr_enum.py
 src/taipy/config/common/_template_handler.py
 src/taipy/config/common/_validate_id.py
 src/taipy/config/common/frequency.py
```

