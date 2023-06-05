# Comparing `tmp/pyside-app-core-0.1.5.tar.gz` & `tmp/pyside-app-core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside-app-core-0.1.5.tar", last modified: Thu May 18 18:32:27 2023, max compression
+gzip compressed data, was "pyside-app-core-0.1.6.tar", last modified: Mon Jun  5 20:46:14 2023, max compression
```

## Comparing `pyside-app-core-0.1.5.tar` & `pyside-app-core-0.1.6.tar`

### file list

```diff
@@ -1,92 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.310064 pyside-app-core-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.314065 pyside-app-core-0.1.5/src/pyside_app_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.314065 pyside-app-core-0.1.5/src/pyside_app_core/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/errors/basic_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/errors/encode_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/errors/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/errors/serial_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.314065 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/generate_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/down-arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/grab-corner.svg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/reload.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/spin-down/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/spin-up/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/standard_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/style_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/log/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/qt/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/util/pixel_val.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/util/s_color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.318065 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/error_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/base_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/window_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/menu_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/multi_combo_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/object_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/settings_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/tool_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/tool_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/window_settings_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/src/pyside_app_core/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/application_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/debug_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/platform_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/serial_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/utils/float_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.322065 pyside-app-core-0.1.5/src/pyside_app_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 18:32:11.000000 pyside-app-core-0.1.5/src/pyside_app_core/types/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:32:27.314065 pyside-app-core-0.1.5/src/pyside_app_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 18:32:27.000000 pyside-app-core-0.1.5/src/pyside_app_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-18 18:32:27.000000 pyside-app-core-0.1.5/src/pyside_app_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:32:27.000000 pyside-app-core-0.1.5/src/pyside_app_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 18:32:27.000000 pyside-app-core-0.1.5/src/pyside_app_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-18 18:32:27.000000 pyside-app-core-0.1.5/src/pyside_app_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 18:32:27.000000 pyside-app-core-0.1.5/src/pyside_app_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    42086 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.049160 pyside-app-core-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.053160 pyside-app-core-0.1.6/src/pyside_app_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/basic_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/encode_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/serial_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/generate_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/down-arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/grab-corner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/reload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-down/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-up/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/standard_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/style_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/pixel_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/s_color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/error_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/window_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/window_shade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/menu_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/multi_combo_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/object_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/settings_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/window_settings_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/application_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/debug_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/platform_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/serial_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/float_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/src/pyside_app_core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/types/numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/src/pyside_app_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/utils/compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42086 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/top_level.txt
```

### Comparing `pyside-app-core-0.1.5/LICENSE` & `pyside-app-core-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/PKG-INFO` & `pyside-app-core-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -715,12 +715,17 @@
 Resource files MUST be generated at least once for stylesheets and icons to function.
 
 ```shell
 # from repo with this lib installed
 $ compile-pyside-theme <target directory>
 
 # custom QssTheme subclass where `./theme.py` has `THEME = CustomTheme()`
-$ compile-pyside-theme <target directory> --custom-theme-pypath theme.THEME
+$ compile-pyside-theme \
+    --custom-theme-pypath theme.THEME \
+    <target directory> 
 
 # if needed to resolve python modules you can include pypath updates
-$ compile-pyside-theme <target directory> --extra-python-path ./src --custom-theme-pypath src.example_app.theme.THEME
+$ compile-pyside-theme \
+    --extra-python-path ./src \
+    --custom-theme-pypath src.example_app.theme.THEME \
+    <target directory>
 ```
```

### Comparing `pyside-app-core-0.1.5/README.md` & `pyside-app-core-0.1.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -23,12 +23,17 @@
 Resource files MUST be generated at least once for stylesheets and icons to function.
 
 ```shell
 # from repo with this lib installed
 $ compile-pyside-theme <target directory>
 
 # custom QssTheme subclass where `./theme.py` has `THEME = CustomTheme()`
-$ compile-pyside-theme <target directory> --custom-theme-pypath theme.THEME
+$ compile-pyside-theme \
+    --custom-theme-pypath theme.THEME \
+    <target directory> 
 
 # if needed to resolve python modules you can include pypath updates
-$ compile-pyside-theme <target directory> --extra-python-path ./src --custom-theme-pypath src.example_app.theme.THEME
+$ compile-pyside-theme \
+    --extra-python-path ./src \
+    --custom-theme-pypath src.example_app.theme.THEME \
+    <target directory>
 ```
```

### Comparing `pyside-app-core-0.1.5/pyproject.toml` & `pyside-app-core-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyside-app-core"
-version = "0.1.5"
+version = "0.1.6"
 description = "Framework for PySide Applications"
 readme = "README.md"
 authors = [{ name = "Leo Covarrubias", email = "leo@leocov.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Development Status :: 2 - Pre-Alpha",
@@ -59,15 +59,15 @@
     "src.pyside_app_core",
 ]
 forbidden_modules = [
     "examples.simple_app",
 ]
 
 [tool.bumpver]
-current_version = "0.1.5"
+current_version = "0.1.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/constants.py` & `pyside-app-core-0.1.6/src/pyside_app_core/constants.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/errors/excepthook.py` & `pyside-app-core-0.1.6/src/pyside_app_core/errors/excepthook.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/errors/serial_errors.py` & `pyside-app-core-0.1.6/src/pyside_app_core/errors/serial_errors.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/__main__.py` & `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,55 +7,75 @@
 from pyside_app_core.generator_utils import compile_qrc_to_resources
 from pyside_app_core.qt.style import DEFAULT_THEME
 
 
 def main():
     parser = argparse.ArgumentParser("compile-pyside-theme")
 
-    parser.add_argument("--extra-python-path")
-    parser.add_argument("--custom-theme-pypath")
-    parser.add_argument("--extra-qss-paths", nargs="*")
-    parser.add_argument("--extra-rcc-pypaths", nargs="*")
+    parser.add_argument(
+        "--extra-python-path",
+        help="Provide a directory path to resolve python imports",
+    )
+    parser.add_argument(
+        "--custom-theme",
+        help='Provide a python module path for a custom theme object e.g. "my.theme.CustomTheme"',
+    )
+    parser.add_argument(
+        "--extra-qss-templates",
+        help='Provide file path to jinja template for qss e.g. "my/theme/templates/custom.qss.jinja2" (Can specify this flag multiple times)',
+        action="append",
+    )
+    parser.add_argument(
+        "--extra-qresources",
+        help='Provide a python module path for additional QResource object e.g. "my.theme.Resource" (Can specify this flag multiple times)',
+        action="append",
+    )
 
-    parser.add_argument("target_dir", metavar="target-dir")
+    parser.add_argument(
+        "target_dir",
+        help="Provide a directory path were the final resource file will be placed",
+        metavar="target-dir",
+    )
 
     args = parser.parse_args()
 
+    print("...")
+
     target_dir = Path(args.target_dir)
 
     if args.extra_python_path:
         pypath = os.path.abspath(args.extra_python_path)
         sys.path.append(pypath)
 
     theme = DEFAULT_THEME
-    if args.custom_theme_pypath:
-        mod_path, klass_name = args.custom_theme_pypath.rsplit(".", 1)
+    if args.custom_theme:
+        mod_path, klass_name = args.custom_theme.rsplit(".", 1)
 
         mod = importlib.import_module(mod_path)
 
         theme = getattr(mod, klass_name)
 
     qss_template_extra = None
-    if args.extra_qss_paths:
-        qss_template_extra = [Path(q) for q in args.extra_qss_paths]
+    if args.extra_qss_templates:
+        qss_template_extra = [Path(q) for q in args.extra_qss_templates]
 
     resources_extra = []
-    if args.extra_rcc_pypaths:
-        for rcc in args.extra_rcc_pypaths:
+    if args.extra_qresources:
+        for rcc in args.extra_qresources:
             mod_path, obj_name = rcc.rsplit(".", 1)
 
             mod = importlib.import_module(mod_path)
 
             resources_extra.append(getattr(mod, obj_name))
 
     generated_file = compile_qrc_to_resources(
         target_dir=target_dir,
         qss_theme=theme,
         qss_template_extra=qss_template_extra,
         resources_extra=resources_extra,
     )
 
-    print(f"Generated: {generated_file}")
+    print(f'Generated: "{generated_file}"')
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/generate_resources.py` & `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/generate_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/console.svg` & `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/console.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/reload.svg` & `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/reload.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/icons/save.svg` & `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/save.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/standard_resources.py` & `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/standard_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/generator_utils/templates/style.qss.jinja2` & `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/style.qss.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 /* --- standard qss style --- */
 
 /* ------------------------------------------------------------------------- */
 QWidget {
-    background: {{ theme.background_color }};
     color: {{ theme.text_color }};
     /* border: 1px solid {{ theme.widget_border_color }}; */
 }
 QWidget:!active {
-    background: {{ theme.background_color_inactive }};
     color: {{ theme.text_color_inactive }};
 }
 
 /* ------------------------------------------------------------------------- */
 QMainWindow {
     border-radius: {{ theme.win_corner_radius }};
 }
 
+QFrame {
+    border-radius: {{ theme.win_corner_radius }};
+}
+
 /* ------------------------------------------------------------------------- */
 QMenuBar {
     color: {{ theme.text_color }};
     spacing: 0;
 }
 QMenuBar::item {
     color: {{ theme.text_color }};
@@ -52,14 +54,15 @@
 QLabel {
     color: {{ theme.text_color }};
 }
 
 /* ------------------------------------------------------------------------- */
 QPlainTextEdit {
     background-color: {{ theme.input_background_color }};
+    border-radius: {{ theme.widget_corner_radius }};
 }
 QPlainTextEdit:!active {
     background-color: {{ theme.input_background_color_inactive }};
 }
 
 /* ------------------------------------------------------------------------- */
 QSizeGrip {
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/log/__init__.py` & `pyside-app-core-0.1.6/src/pyside_app_core/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/log/logger.py` & `pyside-app-core-0.1.6/src/pyside_app_core/log/logger.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/style.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/style.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     background_color = SColor(60)
     background_color_inactive = SColor(70)
 
     text_color = SColor(250)
     text_color_inactive = SColor(200)
     text_color_disabled = SColor(120)
 
-    win_corner_radius = PixelVal(12)
+    win_corner_radius = PixelVal(14)
     widget_corner_radius = PixelVal(8)
 
     win_divider_width = PixelVal(2)
     win_divider_color = SColor(85)
 
     widget_accent_main_color = SColor(80, 160, 250)
     widget_accent_neutral_color = SColor(85)
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/util/s_color.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/util/s_color.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/about_dialog.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/about_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/error_dialog.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/error_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/application.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/application.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/base_dialog.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/base_window.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_window.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from PySide6.QtCore import QPoint, QRect, QSize, Qt, Signal
-from PySide6.QtGui import QBitmap, QMouseEvent, QPainter, QPaintEvent, QResizeEvent
-from PySide6.QtWidgets import QLabel, QSizePolicy, QVBoxLayout
+from PySide6.QtGui import (
+    QBitmap,
+    QBrush,
+    QColor,
+    QMouseEvent,
+    QPainter,
+    QPainterPath,
+    QPaintEvent,
+    QPen,
+    QResizeEvent,
+)
+from PySide6.QtWidgets import QLabel, QSizePolicy, QVBoxLayout, QWidget
 
 from pyside_app_core.qt.style import QssTheme
-from pyside_app_core.qt.widgets.frameless.border import FramelessWindowBorder
+from pyside_app_core.qt.widgets.frameless.window_shade import FramelessWindowShade
 from pyside_app_core.qt.widgets.frameless.window_actions import WindowActions
 from pyside_app_core.services import application_service
 
 
 class FramelessBaseMixin:
     close_window = Signal()
 
@@ -15,30 +25,32 @@
         self,
         *args,
         **kwargs,
     ):
         super(FramelessBaseMixin, self).__init__(*args, **kwargs)
 
         self.setWindowFlags(self.windowFlags() | Qt.WindowType.FramelessWindowHint)
+        self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
         self.setMouseTracking(True)
         self.setMinimumSize(300, 128)
 
         self._theme = application_service.get_app_theme()
 
         self._top_layout = QVBoxLayout()
         self._top_layout.setContentsMargins(5, 0, 5, 5)
         self._title = QLabel("", parent=self)
+        self._title.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._title.setSizePolicy(
-            QSizePolicy.Policy.MinimumExpanding,
+            QSizePolicy.Policy.Fixed,
             QSizePolicy.Policy.MinimumExpanding,
         )
         self._title.setFixedHeight(32)
         self._top_layout.addWidget(
             self._title,
-            alignment=Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignTop,
+            alignment=Qt.AlignmentFlag.AlignTop,
         )
 
         self.setLayout(self._top_layout)
 
         self._moving = False
         self._screen_number: int = 0
         self._move_offset = QPoint(0, 0)
@@ -47,15 +59,15 @@
         self._can_maximize = True
 
         self._window_actions = WindowActions(parent=self)
         self._window_actions.close_clicked.connect(self.close)
         self._window_actions.minimize_clicked.connect(self._on_minimize)
         self._window_actions.maximize_clicked.connect(self._on_maximize)
 
-        self._window_border = FramelessWindowBorder(parent=self)
+        self._window_shade = FramelessWindowShade(parent=self)
 
     @property
     def window_bar_rect(self) -> QRect:
         return QRect(
             0, 0, self.rect().width(), self._window_actions.geometry().height()
         )
 
@@ -81,41 +93,68 @@
             return
 
         raise ValueError
 
     def paintEvent(self, event: QPaintEvent) -> None:
         super().paintEvent(event)
 
+        p = QPainter(self)
+        p.setRenderHint(QPainter.RenderHint.Antialiasing)
+
+        p.setPen(Qt.GlobalColor.transparent)
+        p.setBrush(self._theme.background_color)
+
+        p.drawRoundedRect(
+            self.rect(), self._theme.win_corner_radius, self._theme.win_corner_radius
+        )
+
+        self._draw_border(p, self.rect())
+
         # TODO: a bit crude - we want the border to be on top of everything, but no need to call
         #  every time - how to call after all subclasses have added edited widgets? unknown...
-        self._window_border.raise_()
+        self._window_shade.raise_()
         self._window_actions.raise_()
 
-        rect = self.rect()
-
-        b = self._generate_bitmap_mask(rect)
-        self.setMask(b)
+        p.end()
+        event.accept()
 
     def resizeEvent(self, event: QResizeEvent) -> None:
+        self._title.setFixedWidth(self.rect().width())
         self._window_actions.resizeEvent(event)
         super().resizeEvent(event)
 
-    def _generate_bitmap_mask(self, rect: QRect) -> QBitmap:
-        b = QBitmap(rect.size())
-        b.fill(Qt.GlobalColor.white)
-        p = QPainter(b)
-        p.setRenderHint(QPainter.RenderHint.Antialiasing)
+    def _draw_border(self, p: QPainter, rect: QRect):
+        # outline
+        p.setBrush(QBrush(Qt.GlobalColor.transparent))
+
+        draw_rect = rect.adjusted(1, 1, -1, -1)
+
+        top_corner = QPainterPath(rect.topRight())
+        top_corner.lineTo(rect.topLeft())
+        top_corner.lineTo(rect.bottomLeft())
+        p.setClipPath(top_corner)
 
-        p.setBrush(Qt.GlobalColor.black)
+        p.setPen(QPen(self._theme.background_color.lighter(220), 1))
         p.drawRoundedRect(
-            rect, self._theme.win_corner_radius, self._theme.win_corner_radius
+            draw_rect,
+            self._theme.win_corner_radius - 2,
+            self._theme.win_corner_radius - 2,
         )
-        p.end()
 
-        return b
+        bottom_corner = QPainterPath(rect.topRight())
+        bottom_corner.lineTo(rect.bottomRight())
+        bottom_corner.lineTo(rect.bottomLeft())
+        p.setClipPath(bottom_corner)
+
+        p.setPen(QPen(self._theme.background_color.lighter(130), 2))
+        p.drawRoundedRect(
+            draw_rect,
+            self._theme.win_corner_radius - 2,
+            self._theme.win_corner_radius - 2,
+        )
 
     def _on_maximize(self):
         if self.isMaximized():
             self.setWindowState(Qt.WindowState.WindowNoState)
         else:
             self.setWindowState(Qt.WindowState.WindowMaximized)
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/main_window.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class FramelessMainWindow(WindowSettingsMixin, FramelessBaseMixin, QMainWindow):
     def __init__(self):
         super(FramelessMainWindow, self).__init__(parent=None)
 
         self._about_dialog = AboutDialog()
 
         self._central = QWidget(parent=self)
+        self._central.setStyleSheet("""background-color: none;""")
         self.setCentralWidget(self._central)
 
         # must in order to show grab handle
         self.statusBar().show()
 
         self._menu_bar = MenuBarContext(
             self,
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/frameless/window_actions.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/window_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         self.setFocusPolicy(Qt.FocusPolicy.StrongFocus)
 
         self.setContentsMargins(10, 12, 0, 0)
 
         self._theme = application_service.get_app_theme()
         self._hover = Action.NONE
         self._press = Action.NONE
-        self._focus = True
 
         self._pen = QPen(Qt.GlobalColor.transparent)
 
         self._brush = QBrush(Qt.GlobalColor.transparent)
 
         _top_offset = self.contentsMargins().top() if platform_service.is_macos else 0
         self._side_offset = (
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/menu_ctx.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/menu_ctx.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/multi_combo_box.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/multi_combo_box.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/object_name_mixin.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/object_name_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,14 @@
         super(ObjectNameMixin, self).__init__(*args, **kwargs)
 
         if isinstance(self, QWidget):
             self.setAttribute(Qt.WidgetAttribute.WA_StyledBackground)
 
         obj_name = self.__class__.__name__
         if hasattr(self, "OBJECT_NAME"):
-            obj_name = self.OBJECT_NAME
+            obj_name = self.OBJECT_NAME.replace(" ", "_")
 
         self.setObjectName(obj_name)
 
     @property
     def obj_name(self):
         return self.objectName()
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/settings_mixin.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/tool_bar_ctx.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_bar_ctx.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/tool_button.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_button.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/tool_stack.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_stack.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/qt/widgets/window_settings_mixin.py` & `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/window_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/services/application_service.py` & `pyside-app-core-0.1.6/src/pyside_app_core/services/application_service.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/serial_service.py` & `pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/serial_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     SerialDisconnectedError,
     SerialReadError,
     SerialUnknownError,
     SerialWriteError,
 )
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.services.serial_service.utils.abstract_decoder import (
-    DecoderInterface,
+    CommandInterface,
+    TranscoderInterface,
 )
 
 log.set_level(lvl=logging.DEBUG)
 
 
 class CanRegister(Protocol):
     def bind_serial_service(self, serial_service: "SerialService"):
@@ -28,39 +29,34 @@
 class SerialService(ObjectNameMixin, QObject):
     ports = Signal(list)
     com_connect = Signal(QSerialPort)
     com_disconnect = Signal()
     data = Signal(object)
     error = Signal(Exception)
 
-    def __init__(self, decoder: DecoderInterface, parent: QObject):
+    def __init__(self, transcoder: TranscoderInterface, parent: QObject):
         super(SerialService, self).__init__(parent=parent)
 
-        self._decoder = decoder
+        self._transcoder = transcoder
         self._com: QSerialPort | None = None
         self._buffer = bytearray()
 
-    def _open(
+    def _new_com(
         self, port_info: QSerialPortInfo
     ) -> tuple[QSerialPort, QSerialPort.SerialPortError | None]:
         com = QSerialPort(port_info, parent=self)
         com.setBaudRate(QSerialPort.BaudRate.Baud115200)
         open_ok = com.open(QIODevice.OpenModeFlag.ReadWrite)
 
         return com, None if open_ok else com.error()
 
-    def _close(self, com: QSerialPort | None) -> None:
-        if com and com.isOpen():
-            com.flush()
-            com.close()
-
     def open_connection(self, port_info: QSerialPortInfo) -> bool:
         self.close_connection()
 
-        self._com, error = self._open(port_info)
+        self._com, error = self._new_com(port_info)
         if error:
             self._on_error(error)
             return False
 
         self._com.readyRead.connect(self._on_data)
         self._com.errorOccurred.connect(self._on_error)
 
@@ -103,28 +99,42 @@
         ports = QSerialPortInfo.availablePorts()
 
         self._debug_ports(ports)
         log.debug("sending ports...")
 
         self.ports.emit([p for p in ports if self._port_filter(p)])
 
+    def send_command(self, command: CommandInterface) -> None:
+        log.debug(f"sending cmd: {command}")
+
+        if not self._com:
+            log.debug("com port not connected")
+            return
+
+        self._com.write(command.encode())
+
     def close_connection(self) -> None:
-        if self._com:
-            self.com_disconnect.emit()
+        if not self._com:
+            return
+
+        self.com_disconnect.emit()
+
+        try:
+            self._com.errorOccurred.disconnect()
+            self._com.readyRead.disconnect()
+        except Exception as e:
+            log.exception(e)
+            pass
+
+        if self._com and self._com.isOpen():
+            self._com.flush()
+            self._com.close()
 
-            try:
-                self._com.errorOccurred.disconnect()
-                self._com.readyRead.disconnect()
-            except Exception as e:
-                log.exception(e)
-                pass
-
-            self._close(self._com)
-            self._com.deleteLater()
-            self._com = None
+        self._com.deleteLater()
+        self._com = None
 
     def deleteLater(self) -> None:
         self.close_connection()
         super().deleteLater()
 
     def _on_data(self, *args, **kwargs) -> None:
         read: bytes = self._com.readAll()
@@ -134,18 +144,18 @@
         if b"\x00" in self._buffer:
             chunks: list[bytearray]
             remainder: bytearray
             *chunks, remainder = self._buffer.split(b"\x00")
 
             for chunk in chunks:
                 try:
-                    command = self._decoder.decode_data(chunk)
+                    command = self._transcoder.decode_data(chunk)
                 except Exception as e:
                     log.exception(e)
-                    command = self._decoder.format_error(e)
+                    command = self._transcoder.format_error(e)
 
                 self.data.emit(command)
 
             self._buffer.clear()
             self._buffer.extend(remainder)
 
     def _on_error(self, error: QSerialPort.SerialPortError | None) -> None:
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/utils/conversion_utils.py` & `pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core/services/serial_service/utils/float_map.py` & `pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/float_map.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,119 @@
 import struct
 from decimal import Decimal
 from typing import Any, Iterator, Mapping, Self, TypeVar
 
+from pyside_app_core.utils import compare
 from pyside_app_core.constants import (
     DATA_STRUCT_ENDIAN,
     FLOAT_PRECISION,
     STRUCT_FLOAT_FMT,
 )
+from pyside_app_core.services.serial_service.utils.conversion_utils import (
+    int_from_bytes,
+)
 
 K = TypeVar("K", bound=int)
 
 
 class FloatMap(Mapping[K, float]):
+    _count_fmt = "H"  # unsigned short, 2 bytes
+    _key_fmt = "H"  # unsigned short, 2 bytes
+
     def __init__(self, data: Mapping[K, float]):
         self._data = data
 
+        if not data:
+            raise ValueError(f"can't create an empty {self.__class__.__name__}")
+
+        if len(data) > 65535:
+            raise ValueError("data has too many values, must fit in 2 bytes")
+
+        for k in data.keys():
+            if k > 65535:
+                raise ValueError(f'key: "{k}" does not fit in 2 bytes')
+
+            if k < 0:
+                raise ValueError(f'key: "{k}" is not a positive number')
+
     def __getitem__(self, k: K) -> float:
         return self._data[k]
 
     def __len__(self) -> int:
         return len(self._data)
 
     def __iter__(self) -> Iterator[K]:
         return iter(self._data)
 
+    def __repr__(self):
+        return self._data.__repr__()
+
+    def __str__(self):
+        return self._data.__str__()
+
+    def __eq__(self, other: Self) -> bool:
+        val_eq: List[bool] = []
+        for k, v in self.items():
+            other_v = other.get(k)
+            if other_v:
+                val_eq.append(compare.float_approx(v, other_v))
+
+        return all(
+            [
+                sorted(self.keys()) == sorted(other.keys()),
+                *val_eq,
+            ]
+        )
+
     @classmethod
     def _key_xform(cls, key: int) -> Any:
         return key
 
+    @classmethod
+    def pack_format(cls, item_count: int) -> str:
+        if item_count < 1:
+            raise ValueError("must pack at least 1 item")
+
+        accum_fmt = f"{DATA_STRUCT_ENDIAN}{cls._count_fmt}"
+
+        accum_fmt += f"{cls._key_fmt}{STRUCT_FLOAT_FMT}" * item_count
+
+        return accum_fmt
+
     def pack(self) -> bytearray:
         """
         pattern:
         count,key,value,key,value,key,value,...
-        b - count, number of pairs - max 255 params...
-        b - key in 1 byte corresponding to enum ConfigurationParam
+        H - count, number of pairs - max 2 bytes unsigned...
+        H - key in 2 bytes corresponding to enum ConfigurationParam
         f/d - value in 4 or 8 bytes corresponding to float/double value
-        example
-        struct.pack("<bbfbf", count, key, value, key, value)
+
+        example:
+        struct.pack("<HHfHf", count, key, value, key, value)
         """
         if not self._data:
             raise AttributeError("Command had no data")
 
-        accum_fmt = ""
+        count = len(self)
         flattened_data = []
 
         for key, value in self._data.items():
-            accum_fmt += f"b{STRUCT_FLOAT_FMT}"
             flattened_data.extend([key, value])
 
-        raw = struct.pack(
-            f"{DATA_STRUCT_ENDIAN}b{accum_fmt}", len(self._data), *flattened_data
-        )
+        raw = struct.pack(self.pack_format(count), count, *flattened_data)
         return bytearray(raw)
 
     @classmethod
     def unpack(cls, raw_data: bytes) -> Self:
-        raw_pair_count = raw_data[:1]
-        raw_key_val = raw_data[1:]
+        count_bytes = 2
+        raw_pair_count = raw_data[:count_bytes]
+        raw_key_val = raw_data[count_bytes:]
 
-        pair_count = utils.int_from_bytes(raw_pair_count, signed=False)
-        fmt_chars = ["b", STRUCT_FLOAT_FMT] * pair_count
+        pair_count = int_from_bytes(raw_pair_count, signed=False)
+        fmt_chars = [cls._key_fmt, STRUCT_FLOAT_FMT] * pair_count
 
         flat_pairs = struct.unpack(
             f"{DATA_STRUCT_ENDIAN}{''.join(fmt_chars)}", raw_key_val
         )
 
         data = {}
         iterable = iter(flat_pairs)
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core.egg-info/PKG-INFO` & `pyside-app-core-0.1.6/src/pyside_app_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -715,12 +715,17 @@
 Resource files MUST be generated at least once for stylesheets and icons to function.
 
 ```shell
 # from repo with this lib installed
 $ compile-pyside-theme <target directory>
 
 # custom QssTheme subclass where `./theme.py` has `THEME = CustomTheme()`
-$ compile-pyside-theme <target directory> --custom-theme-pypath theme.THEME
+$ compile-pyside-theme \
+    --custom-theme-pypath theme.THEME \
+    <target directory> 
 
 # if needed to resolve python modules you can include pypath updates
-$ compile-pyside-theme <target directory> --extra-python-path ./src --custom-theme-pypath src.example_app.theme.THEME
+$ compile-pyside-theme \
+    --extra-python-path ./src \
+    --custom-theme-pypath src.example_app.theme.THEME \
+    <target directory>
 ```
```

### Comparing `pyside-app-core-0.1.5/src/pyside_app_core.egg-info/SOURCES.txt` & `pyside-app-core-0.1.6/src/pyside_app_core.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -50,22 +50,24 @@
 src/pyside_app_core/qt/widgets/tool_button.py
 src/pyside_app_core/qt/widgets/tool_stack.py
 src/pyside_app_core/qt/widgets/window_settings_mixin.py
 src/pyside_app_core/qt/widgets/frameless/__init__.py
 src/pyside_app_core/qt/widgets/frameless/application.py
 src/pyside_app_core/qt/widgets/frameless/base_dialog.py
 src/pyside_app_core/qt/widgets/frameless/base_window.py
-src/pyside_app_core/qt/widgets/frameless/border.py
 src/pyside_app_core/qt/widgets/frameless/main_window.py
 src/pyside_app_core/qt/widgets/frameless/window_actions.py
+src/pyside_app_core/qt/widgets/frameless/window_shade.py
 src/pyside_app_core/services/__init__.py
 src/pyside_app_core/services/application_service.py
 src/pyside_app_core/services/debug_service.py
 src/pyside_app_core/services/platform_service.py
 src/pyside_app_core/services/serial_service/__init__.py
 src/pyside_app_core/services/serial_service/serial_service.py
 src/pyside_app_core/services/serial_service/utils/__init__.py
 src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
 src/pyside_app_core/services/serial_service/utils/conversion_utils.py
 src/pyside_app_core/services/serial_service/utils/float_map.py
 src/pyside_app_core/types/__init__.py
-src/pyside_app_core/types/numeric.py
+src/pyside_app_core/types/numeric.py
+src/pyside_app_core/utils/__init__.py
+src/pyside_app_core/utils/compare.py
```

