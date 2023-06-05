# Comparing `tmp/taipy-gui-2.3.0.dev1.tar.gz` & `tmp/taipy-gui-2.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-gui-2.3.0.dev1.tar", last modified: Tue May 30 12:32:01 2023, max compression
+gzip compressed data, was "taipy-gui-2.3.0.dev2.tar", last modified: Mon Jun  5 16:02:15 2023, max compression
```

## Comparing `taipy-gui-2.3.0.dev1.tar` & `taipy-gui-2.3.0.dev2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.631815 taipy-gui-2.3.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-30 12:32:01.631815 taipy-gui-2.3.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:32:01.631815 taipy-gui-2.3.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.579815 taipy-gui-2.3.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.579815 taipy-gui-2.3.0.dev1/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.587815 taipy-gui-2.3.0.dev1/src/taipy/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/_gui_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/_gui_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.587815 taipy-gui-2.3.0.dev1/src/taipy/gui/data/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/array_dict_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/content_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/data_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.591815 taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/lttb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/minmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/scatter_decimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/numpy_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/pandas_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.591815 taipy-gui-2.3.0.dev1/src/taipy/gui/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/extension/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    91614 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/gui_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.591815 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.591815 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_html/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_html/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_html/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.595815 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/blocproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/postproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40046 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.603815 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_locals_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_map_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_runtime_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_variable_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/chart_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/clientvarname.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/expr_var_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/filename.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/filter_locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/get_imported_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/get_module_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/getdatecolstrname.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/is_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/isnotebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/table_col_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/utils/varnamefromcontent.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 12:27:44.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.619815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-30 12:31:11.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/227.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-05-30 12:31:11.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/499.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-05-30 12:31:11.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/660.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-30 12:31:11.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.619815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.619815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/base/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/base/fontfaces.css
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/base/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.619815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/blocks/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.623815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/button.css
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/date.css
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/expandable.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/image.css
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/input.css
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/navbar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/number.css
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/selector.css
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/slider.css
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.627815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/card.css
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/container.css
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/header.css
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/stylekit.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.627815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.627815 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/elements.css
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/shapes.css
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/typography.css
--rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-05-30 12:29:06.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-deps.dll.js
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-30 12:29:06.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-dom.js
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)  1084540 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-30 12:31:11.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy.status.json
--rw-r--r--   0 runner    (1001) docker     (123)    55957 2023-05-30 12:31:53.000000 taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:01.631815 taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-30 12:32:01.000000 taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-30 12:32:01.000000 taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:32:01.000000 taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:31:54.000000 taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-30 12:32:01.000000 taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 12:32:01.000000 taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.241002 taipy-gui-2.3.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.241002 taipy-gui-2.3.0.dev2/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.245002 taipy-gui-2.3.0.dev2/src/taipy/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/_gui_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/_gui_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.245002 taipy-gui-2.3.0.dev2/src/taipy/gui/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/array_dict_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/content_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/data_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.245002 taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/lttb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/scatter_decimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/numpy_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/pandas_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.245002 taipy-gui-2.3.0.dev2/src/taipy/gui/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/extension/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91660 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/gui_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.245002 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.245002 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_html/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_html/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.249002 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/blocproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23256 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.253002 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_locals_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_map_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_runtime_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_variable_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/chart_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/clientvarname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/expr_var_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/filter_locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/get_imported_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/get_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/getdatecolstrname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/is_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/isnotebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/table_col_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/utils/varnamefromcontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 15:57:19.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.265002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-05 16:01:18.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/227.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-06-05 16:01:18.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/499.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-06-05 16:01:18.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/660.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-05 16:01:18.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.265002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.265002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/base/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/base/fontfaces.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/base/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.265002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/blocks/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/button.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/date.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/expandable.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/image.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/number.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/selector.css
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/card.css
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/container.css
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/stylekit.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/elements.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/shapes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/typography.css
+-rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-06-05 15:58:52.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-deps.dll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-05 15:58:52.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-dom.js
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)  1084737 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-05 16:01:18.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy.status.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56105 2023-06-05 16:02:07.000000 taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:02:15.269002 taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-05 16:02:15.000000 taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-05 16:02:15.000000 taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:02:15.000000 taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:02:08.000000 taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-05 16:02:15.000000 taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:02:15.000000 taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/top_level.txt
```

### Comparing `taipy-gui-2.3.0.dev1/LICENSE` & `taipy-gui-2.3.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/PKG-INFO` & `taipy-gui-2.3.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.3.0.dev1/README.md` & `taipy-gui-2.3.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/setup.py` & `taipy-gui-2.3.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/_default_config.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/_default_config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/_gui_cli.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/_gui_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/_gui_section.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/_gui_section.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/_page.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/_page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/config.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/array_dict_data_accessor.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/array_dict_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/content_accessor.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/content_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/data_accessor.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/data_format.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/data_format.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/data_scope.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/data_scope.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/lttb.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/lttb.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/minmax.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/minmax.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/rdp.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/rdp.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/decimator/scatter_decimator.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/decimator/scatter_decimator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/numpy_data_accessor.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/numpy_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/pandas_data_accessor.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/pandas_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/data/utils.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/data/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/extension/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/extension/library.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/extension/library.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/gui.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1145,15 +1145,15 @@
                         attributes.get("columns", {}),
                         self._accessors._get_col_types(data_hash, _TaipyData(data, data_hash)),
                         attributes.get("date_format"),
                         attributes.get("number_format"),
                     )
                     _enhance_columns(attributes, hashes, col_dict, "table(cols)")
 
-                    return json.dumps(col_dict)
+                    return json.dumps(col_dict, cls=_TaipyJsonEncoder)
             except Exception as e:  # pragma: no cover
                 _warn(f"Exception while rebuilding table columns {e}.")
         return Gui.__DO_NOT_UPDATE_VALUE
 
     def _chart_conf(
         self, rebuild: bool, rebuild_val: t.Optional[bool], attr_json: str, hash_json: str, **kwargs
     ) -> t.Union[str, _DoNotUpdate]:
@@ -1165,15 +1165,15 @@
                     data_hash = hashes.get("data", "")
                     config = _build_chart_config(
                         self,
                         attributes,
                         self._accessors._get_col_types(data_hash, _TaipyData(kwargs.get(data_hash), data_hash)),
                     )
 
-                    return json.dumps(config)
+                    return json.dumps(config, cls=_TaipyJsonEncoder)
             except Exception as e:  # pragma: no cover
                 _warn(f"Exception while rebuilding chart config {e}.")
         return Gui.__DO_NOT_UPDATE_VALUE
 
     # Proxy methods for Adapter
 
     def _add_adapter_for_type(self, type_name: str, adapter: t.Callable) -> None:
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/gui_actions.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/gui_actions.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/icon.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/icon.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/page.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/partial.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/partial.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_html/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_html/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_html/factory.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_html/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_html/parser.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_html/parser.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/blocproc.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/blocproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/control.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/control.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/factory.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/postproc.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/postproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/_markdown/preproc.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/_markdown/preproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/builder.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,29 +211,57 @@
         """
         TODO
         Defines a React attribute as a stringified json dict.
         The original property can be a dict or a string formed as <key 1>:<value 1>;<key 2>:<value 2>.
 
         Arguments:
             name (str): The property name.
-            default value (dict): iused if no value is specified
+            default value (dict): used if no value is specified.
         """
         dict_attr = self.__attributes.get(name)
         if dict_attr is None:
             dict_attr = default_value
         if dict_attr is not None:
             if isinstance(dict_attr, str):
                 vals = [x.strip().split(":") for x in dict_attr.split(";")]
                 dict_attr = {val[0].strip(): val[1].strip() for val in vals if len(val) > 1}
             if isinstance(dict_attr, (dict, _MapDict)):
                 self.__set_json_attribute(_to_camel_case(name), dict_attr)
             else:
                 _warn(f"{self.__element_name}: {name} should be a dict: '{str(dict_attr)}'.")
         return self
 
+    def set_dynamic_dict_attribute(self, name: str, default_value: t.Optional[t.Dict[str, t.Any]] = None):
+        """
+        TODO
+        Defines a React attribute as a stringified json dict.
+        The original property can be a dict or a string formed as <key 1>:<value 1>;<key 2>:<value 2>.
+
+        Arguments:
+            name (str): The property name.
+            default value (dict): used if no value is specified.
+        """
+        dict_attr = self.__attributes.get(name)
+        if dict_attr is None:
+            dict_attr = default_value
+        if dict_attr is not None:
+            if isinstance(dict_attr, str):
+                vals = [x.strip().split(":") for x in dict_attr.split(";")]
+                dict_attr = {val[0].strip(): val[1].strip() for val in vals if len(val) > 1}
+            if isinstance(dict_attr, (dict, _MapDict)):
+                self.__set_json_attribute(_to_camel_case("default_" + name), dict_attr)
+            else:
+                _warn(f"{self.__element_name}: {name} should be a dict: '{str(dict_attr)}'.")
+        if dict_hash := self.__hashes.get(name):
+            dict_hash = self.__get_typed_hash_name(dict_hash, PropertyType.dynamic_dict)
+            prop_name = _to_camel_case(name)
+            self.__update_vars.append(f"{prop_name}={dict_hash}")
+            self.__set_react_attribute(prop_name, dict_hash)
+        return self
+
     def __set_json_attribute(self, name, value):
         return self.set_attribute(name, json.dumps(value, cls=_TaipyJsonEncoder))
 
     def __set_list_of_(self, name: str):
         lof = self.__get_list_of_(name)
         if not isinstance(lof, (list, tuple)):
             if lof is not None:
@@ -283,21 +311,20 @@
     def __set_dynamic_string_attribute(
         self,
         name: str,
         default_value: t.Optional[str] = None,
         with_update: t.Optional[bool] = False,
         dynamic_property_name: t.Optional[str] = None,
     ):
-        hash_name = self.__hashes.get(name)
         str_val = self.__attributes.get(name, default_value)
         if str_val is not None:
             self.set_attribute(
                 _to_camel_case(f"default_{name}" if dynamic_property_name is None else name), str(str_val)
             )
-        if hash_name:
+        if hash_name := self.__hashes.get(name):
             prop_name = _to_camel_case(name if dynamic_property_name is None else dynamic_property_name)
             if with_update:
                 self.__update_vars.append(f"{prop_name}={hash_name}")
             self.__set_react_attribute(prop_name, hash_name)
         return self
 
     def __set_function_attribute(
@@ -849,14 +876,16 @@
                 self.__set_react_attribute(
                     _to_camel_case(attr[0]), _get_broadcast_var_name(_get_tuple_val(attr, 2, None))
                 )
             elif var_type == PropertyType.string_or_number:
                 self.__set_string_or_number_attribute(attr[0], _get_tuple_val(attr, 2, None))
             elif var_type == PropertyType.dict:
                 self.set_dict_attribute(attr[0], _get_tuple_val(attr, 2, None))
+            elif var_type == PropertyType.dynamic_dict:
+                self.set_dynamic_dict_attribute(attr[0], _get_tuple_val(attr, 2, None))
             elif var_type == PropertyType.dynamic_list:
                 self.__set_dynamic_string_list(attr[0], _get_tuple_val(attr, 2, None))
             elif var_type == PropertyType.boolean_or_list:
                 if _is_boolean(self.__attributes.get(attr[0])):
                     self.__set_dynamic_bool_attribute(attr[0], _get_tuple_val(attr, 2, False), True, update_main=False)
                 else:
                     self.__set_dynamic_string_list(attr[0], _get_tuple_val(attr, 2, None))
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/factory.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         .set_value_and_default(with_default=False, var_type=PropertyType.data)
         .set_attributes(
             [
                 ("id",),
                 ("title",),
                 ("width", PropertyType.string_or_number),
                 ("height", PropertyType.string_or_number),
-                ("layout", PropertyType.dict),
+                ("layout", PropertyType.dynamic_dict),
                 ("plot_config", PropertyType.dict),
                 ("on_range_change", PropertyType.function),
                 ("active", PropertyType.dynamic_boolean, True),
                 ("render", PropertyType.dynamic_boolean, True),
                 ("hover_text", PropertyType.dynamic_string),
                 ("on_change", PropertyType.function),
                 ("template", PropertyType.dict),
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/json.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/json.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/renderers/utils.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/renderers/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/server.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,27 +143,33 @@
         taipy_bp = Blueprint("Taipy", __name__, static_folder=static_folder, template_folder=template_folder)
         # Serve static react build
 
         @taipy_bp.route("/", defaults={"path": ""})
         @taipy_bp.route("/<path:path>")
         def my_index(path):
             if path == "" or path == "index.html" or "." not in path:
-                return render_template(
-                    "index.html",
-                    title=title,
-                    favicon=favicon,
-                    root_margin=root_margin,
-                    watermark=watermark,
-                    config=client_config,
-                    scripts=scripts,
-                    styles=styles,
-                    version=version,
-                    css_vars=css_vars,
-                    base_url=base_url,
-                )
+                try:
+                    return render_template(
+                        "index.html",
+                        title=title,
+                        favicon=favicon,
+                        root_margin=root_margin,
+                        watermark=watermark,
+                        config=client_config,
+                        scripts=scripts,
+                        styles=styles,
+                        version=version,
+                        css_vars=css_vars,
+                        base_url=base_url,
+                    )
+                except Exception:  # pragma: no cover
+                    raise RuntimeError(
+                        "Something is wrong with the taipy-gui front-end installation. Check that the js bundle has been properly built (is Node.js installed?)."
+                    )
+
             if path == "taipy.status.json":
                 return self._direct_render_json(self._gui._serve_status(pathlib.Path(template_folder) / path))
             if str(os.path.normpath(file_path := ((base_path := static_folder + os.path.sep) + path))).startswith(
                 base_path
             ) and os.path.isfile(file_path):
                 return send_from_directory(base_path, path)
             # use the path mapping to detect and find resources
@@ -193,18 +199,14 @@
                 )
                 and os.path.isfile(file_path)
                 and not self.__is_ignored(file_path)
             ):
                 return send_from_directory(base_path, path)
             return ("", 404)
 
-        @taipy_bp.errorhandler(404)
-        def page_not_found(e):
-            return f"{e.message}, {e.description}"
-
         return taipy_bp
 
     # Update to render as JSX
     def _render(self, html_fragment, style, head, context):
         template_str = _Server.__RE_OPENING_CURLY.sub(_Server.__OPENING_CURLY, html_fragment)
         template_str = _Server.__RE_CLOSING_CURLY.sub(_Server.__CLOSING_CURLY, template_str)
         template_str = template_str.replace('"{!', "{")
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/state.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/state.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/types.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .utils import (
     _TaipyBase,
     _TaipyBool,
     _TaipyContent,
     _TaipyContentImage,
     _TaipyData,
     _TaipyDate,
+    _TaipyDict,
     _TaipyLov,
     _TaipyLovValue,
     _TaipyNumber,
 )
 
 
 class _WsType(Enum):
@@ -66,14 +67,18 @@
     content = _TaipyContent
     data = _TaipyData
     date = _TaipyDate
     dict = "dict"
     """
     The property holds a dictionary.
     """
+    dynamic_dict = _TaipyDict
+    """
+    The property holds a dynamic dictionary.
+    """
     dynamic_number = _TaipyNumber
     """
     The property holds a dynamic number.
     """
     dynamic_boolean = _TaipyBool
     """
     The property holds a dynamic Boolean value.
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/__init__.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,12 +37,13 @@
 from .types import (
     _TaipyBase,
     _TaipyBool,
     _TaipyContent,
     _TaipyContentImage,
     _TaipyData,
     _TaipyDate,
+    _TaipyDict,
     _TaipyLov,
     _TaipyLovValue,
     _TaipyNumber,
 )
 from .varnamefromcontent import _varname_from_content
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_adapter.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_attributes.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_attributes.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_bindings.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_bindings.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_evaluator.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_evaluator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_locals_context.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_locals_context.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_map_dict.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_map_dict.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_runtime_manager.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_runtime_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/_variable_directory.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/_variable_directory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/boolean.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/chart_config_builder.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/chart_config_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/clientvarname.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/clientvarname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/datatype.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/date.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/date.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/expr_var_name.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/expr_var_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/filename.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/filename.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/filter_locals.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/filter_locals.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/get_imported_var.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/get_imported_var.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/get_module_name.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/get_module_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/getdatecolstrname.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/getdatecolstrname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/html.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/html.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/is_debugging.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/is_debugging.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/isnotebook.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/isnotebook.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/proxy.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/singleton.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/table_col_builder.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/table_col_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/types.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
+import json
 import typing as t
 from abc import ABC
 from datetime import datetime
 
 from .._warnings import _warn
-from . import _date_to_ISO, _ISO_to_date, _variable_decode
+from . import _date_to_ISO, _ISO_to_date, _MapDict, _variable_decode
 
 
 class _TaipyBase(ABC):
     __HOLDER_PREFIXES: t.Optional[t.List[str]] = None
     _HOLDER_PREFIX = "_Tp"
 
     def __init__(self, data: t.Any, hash_name: str) -> None:
@@ -133,7 +134,17 @@
         return _TaipyBase._HOLDER_PREFIX + "C"
 
 
 class _TaipyContentImage(_TaipyBase):
     @staticmethod
     def get_hash():
         return _TaipyBase._HOLDER_PREFIX + "Ci"
+
+
+class _TaipyDict(_TaipyBase):
+    def get(self):
+        val = super().get()
+        return json.dumps(val._dict if isinstance(val, _MapDict) else val)
+
+    @staticmethod
+    def get_hash():
+        return _TaipyBase._HOLDER_PREFIX + "Di"
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/utils/varnamefromcontent.py` & `taipy-gui-2.3.0.dev2/src/taipy/gui/utils/varnamefromcontent.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/227.taipy-gui.js` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/227.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/499.taipy-gui.js` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/499.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/660.taipy-gui.js` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/660.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/favicon.ico` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/favicon.png` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/favicon.png`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/index.html` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/index.html`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/base/base.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/base/base.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/base/fontfaces.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/base/fontfaces.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/base/typography.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/base/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/blocks/layout.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/blocks/layout.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/button.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/button.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/chart.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/chart.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/date.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/date.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/expandable.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/expandable.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/image.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/image.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/input.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/input.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/navbar.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/navbar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/number.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/number.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/selector.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/selector.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/slider.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/slider.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/table.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/table.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/controls/toggle.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/controls/toggle.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/card.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/card.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/container.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/container.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/header.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/header.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/elements/sidebar.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/elements/sidebar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/stylekit.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/stylekit.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/colors.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/misc.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/spacing.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/utilities/typography.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/utilities/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/colors.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/elements.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/elements.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/misc.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/shapes.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/shapes.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/spacing.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/stylekit/variables/typography.css` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/stylekit/variables/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-deps-manifest.json` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-deps-manifest.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-deps.dll.js` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-deps.dll.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui-dom.js` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui-dom.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui.d.ts` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui.d.ts`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui.js` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -17429,17 +17429,21 @@
                             }
                         },
                         MuiInputLabel: {
                             styleOverrides: {
                                 outlined: {
                                     zIndex: "0",
                                     transition: "all 200ms cubic-bezier(0, 0, 0.2, 1) 0ms",
-                                    "&:not(.MuiInputLabel-shrink)": {
+                                    "&:not(.MuiInputLabel-shrink):not(.static-label)": {
                                         top: "50%",
                                         transform: "translate(14px, -50%) scale(1)"
+                                    },
+                                    "&.static-label": {
+                                        position: "relative",
+                                        transform: "none"
                                     }
                                 }
                             }
                         },
                         MuiInputBase: {
                             styleOverrides: {
                                 root: {
@@ -21042,15 +21046,15 @@
                     height: a,
                     updateVarName: o,
                     updateVars: s,
                     id: l,
                     data: c = {},
                     onRangeChange: u,
                     propagate: d = !0
-                } = e, p = qd(), [h, f] = (0, n.useState)([]), m = (0, n.useRef)(null), [g, v] = (0, n.useState)("__default__"), b = (0, pt.Z)(), y = Yd(), x = null === c, w = Gd(e.libClassName, e.dynamicClassName, e.className), k = zd(e.active, e.defaultActive, !0), S = zd(e.render, e.defaultRender, !0), C = zd(e.hoverText, e.defaultHoverText, void 0);
+                } = e, p = qd(), [h, f] = (0, n.useState)([]), m = (0, n.useRef)(null), [g, v] = (0, n.useState)("__default__"), b = (0, pt.Z)(), y = Yd(), x = null === c, w = Gd(e.libClassName, e.dynamicClassName, e.className), k = zd(e.active, e.defaultActive, !0), S = zd(e.render, e.defaultRender, !0), C = zd(e.hoverText, e.defaultHoverText, void 0), T = $d(e.layout, e.defaultLayout || "", {});
                 (0, n.useEffect)((() => {
                     f((t => (Object.keys(e).forEach((n => {
                         const r = Dp.exec(n);
                         if (r && 2 == r.length) {
                             const i = parseInt(r[1], 10);
                             let a = e[n];
                             if (void 0 !== a) {
@@ -21060,151 +21064,146 @@
                                     a = []
                                 }
                                 Array.isArray(a) || (a = []), (i >= t.length || a.length !== t[i].length || a.some(((e, n) => t[i][n] != e))) && ((t = t.concat())[i] = a)
                             }
                         }
                     })), t)))
                 }), [e]);
-                const T = $d(e.config, e.defaultConfig, Ip);
+                const P = $d(e.config, e.defaultConfig, Ip);
                 (0, n.useEffect)((() => {
                     if (x || !c[g]) {
-                        const e = Object.values(T.columns).map((e => e.dfid)),
-                            t = e.join("-") + (T.decimators ? `--${T.decimators.join("")}` : "");
-                        v(t), !x && c[t] || p(Ps(o, l, y, e, t, Np(T.decimators, m.current, T.modes, T.columns, T.traces)))
-                    }
-                }), [x, p, T.columns, T.traces, T.modes, T.decimators, o, l, y]), Wd(p, l, y, s);
-                const P = (0, n.useMemo)((() => {
-                        let t, n = {};
-                        if (e.layout) try {
-                            n = JSON.parse(e.layout)
-                        } catch (e) {
-                            console.info(`Error while parsing Chart.layout\n${e.message||e}`)
-                        }
+                        const e = Object.values(P.columns).map((e => e.dfid)),
+                            t = e.join("-") + (P.decimators ? `--${P.decimators.join("")}` : "");
+                        v(t), !x && c[t] || p(Ps(o, l, y, e, t, Np(P.decimators, m.current, P.modes, P.columns, P.traces)))
+                    }
+                }), [x, p, P.columns, P.traces, P.modes, P.decimators, o, l, y]), Wd(p, l, y, s);
+                const E = (0, n.useMemo)((() => {
+                        let t;
                         try {
                             const n = e.template && JSON.parse(e.template),
                                 r = "dark" === b.palette.mode ? e.template_Dark_ ? JSON.parse(e.template_Dark_) : Fp : e.template_Light_ && JSON.parse(e.template_Light_);
                             t = n ? r ? Object.assign(Object.assign({}, n), r) : n : r || void 0
                         } catch (e) {
                             console.info(`Error while parsing Chart.template\n${e.message||e}`)
                         }
-                        return t && (n.template = t), Object.assign(Object.assign({}, n), {
-                            title: r || n.title,
+                        return t && (T.template = t), Object.assign(Object.assign({}, T), {
+                            title: r || T.title,
                             xaxis: Object.assign({
-                                title: T.traces.length && T.traces[0].length && T.traces[0][0] ? Mp(T.columns[T.traces[0][0]].dfid) : void 0
-                            }, n.xaxis),
+                                title: P.traces.length && P.traces[0].length && P.traces[0][0] ? Mp(P.columns[P.traces[0][0]].dfid) : void 0
+                            }, T.xaxis),
                             yaxis: Object.assign({
-                                title: 1 == T.traces.length && T.traces[0].length > 1 && T.columns[T.traces[0][1]] ? Mp(T.columns[T.traces[0][1]].dfid) : void 0
-                            }, n.yaxis),
+                                title: 1 == P.traces.length && P.traces[0].length > 1 && P.columns[P.traces[0][1]] ? Mp(P.columns[P.traces[0][1]].dfid) : void 0
+                            }, T.yaxis),
                             clickmode: "event+select"
                         })
-                    }), [b.palette.mode, r, T.columns, T.traces, e.layout, e.template, e.template_Dark_, e.template_Light_]),
-                    E = (0, n.useMemo)((() => void 0 === a ? Object.assign(Object.assign({}, Op), {
+                    }), [b.palette.mode, r, P.columns, P.traces, T, e.template, e.template_Dark_, e.template_Light_]),
+                    O = (0, n.useMemo)((() => void 0 === a ? Object.assign(Object.assign({}, Op), {
                         width: i
                     }) : Object.assign(Object.assign({}, Op), {
                         width: i,
                         height: a
                     })), [i, a]),
-                    O = (0, n.useMemo)((() => Object.assign(Object.assign({}, E), {
+                    Z = (0, n.useMemo)((() => Object.assign(Object.assign({}, O), {
                         minHeight: "7em"
-                    })), [E]),
-                    Z = (0, n.useMemo)((() => {
+                    })), [O]),
+                    M = (0, n.useMemo)((() => {
                         const e = c && c[g];
-                        return e ? T.traces.map(((t, n) => {
-                            const r = Object.assign(Object.assign({}, Dd(T.options, n, {})), {
-                                type: T.types[n],
-                                mode: T.modes[n],
-                                name: Dd(T.names, n) || (T.columns[t[1]] ? Mp(T.columns[t[1]].dfid) : void 0)
+                        return e ? P.traces.map(((t, n) => {
+                            const r = Object.assign(Object.assign({}, Dd(P.options, n, {})), {
+                                type: P.types[n],
+                                mode: P.modes[n],
+                                name: Dd(P.names, n) || (P.columns[t[1]] ? Mp(P.columns[t[1]].dfid) : void 0)
                             });
-                            r.marker = Dd(T.markers, n, r.marker || {}), _p.forEach((t => {
+                            r.marker = Dd(P.markers, n, r.marker || {}), _p.forEach((t => {
                                 const n = r.marker[t];
                                 if (void 0 !== n && "string" == typeof n) {
                                     const i = Ap(e, n);
                                     i.length && (r.marker[t] = i)
                                 }
                             }));
                             const i = Rp(e, t, 0) || [],
                                 a = Rp(e, t, 1) || [],
-                                o = Dd(T.addIndex, n, !0) && !a.length,
+                                o = Dd(P.addIndex, n, !0) && !a.length,
                                 s = o ? Array.from(Array(i.length).keys()) : i,
                                 l = o ? i : a,
-                                c = T.axisNames.length > n ? T.axisNames[n] : [];
+                                c = P.axisNames.length > n ? P.axisNames[n] : [];
                             s.length && (c.length > 0 ? r[c[0]] = s : r.x = s), l.length && (c.length > 1 ? r[c[1]] = l : r.y = l);
                             const u = Rp(e, t, 2, !0);
                             u && (c.length > 2 ? r[c[2]] = u : r.z = u);
                             for (let n = 3; n < c.length; n++) r[c[n]] = Rp(e, t, n, !0);
-                            r.text = Rp(e, T.texts, n, !0), r.xaxis = T.xaxis[n], r.yaxis = T.yaxis[n], r.hovertext = Rp(e, T.labels, n, !0);
+                            r.text = Rp(e, P.texts, n, !0), r.xaxis = P.xaxis[n], r.yaxis = P.yaxis[n], r.hovertext = Rp(e, P.labels, n, !0);
                             const d = Dd(h, n, []);
-                            (null == d ? void 0 : d.length) && (r.selectedpoints = d), r.orientation = Dd(T.orientations, n), r.line = Dd(T.lines, n), r.textposition = Dd(T.textAnchors, n);
-                            const p = Dd(T.selectedMarkers, n);
+                            (null == d ? void 0 : d.length) && (r.selectedpoints = d), r.orientation = Dd(P.orientations, n), r.line = Dd(P.lines, n), r.textposition = Dd(P.textAnchors, n);
+                            const p = Dd(P.selectedMarkers, n);
                             return p && (r.selected = {
                                 marker: p
                             }), r
                         })) : []
-                    }), [c, T, h, g]),
-                    M = (0, n.useMemo)((() => {
+                    }), [c, P, h, g]),
+                    R = (0, n.useMemo)((() => {
                         let t = {};
                         if (e.plotConfig) {
                             try {
                                 t = JSON.parse(e.plotConfig)
                             } catch (e) {
                                 console.info(`Error while parsing Chart.plot_config\n${e.message||e}`)
                             }("object" != typeof t || null === t || Array.isArray(t)) && (console.info("Error Chart.plot_config is not a dictionnary"), t = {})
                         }
                         return k ? t : Object.assign(Object.assign({}, t), {
                             staticPlot: !0
                         })
                     }), [k, e.plotConfig]),
-                    R = (0, n.useCallback)((e => {
+                    A = (0, n.useCallback)((e => {
                         if (Object.keys(e).some((e => e.startsWith("xaxis."))) && (u && p(Ts(l, y, Object.assign({
                                 action: u
-                            }, e))), T.decimators && !T.types.includes("scatter3d"))) {
-                            const t = Object.values(T.columns).map((e => e.dfid)),
+                            }, e))), P.decimators && !P.types.includes("scatter3d"))) {
+                            const t = Object.values(P.columns).map((e => e.dfid)),
                                 n = Object.entries(e).map((([e, t]) => `${e}=${t}`)).join("-"),
-                                r = t.join("-") + (T.decimators ? `--${T.decimators.join("")}` : "") + "--" + n;
-                            v(r), p(Ps(o, l, y, t, r, Np(T.decimators, m.current, T.modes, T.columns, T.traces, e)))
+                                r = t.join("-") + (P.decimators ? `--${P.decimators.join("")}` : "") + "--" + n;
+                            v(r), p(Ps(o, l, y, t, r, Np(P.decimators, m.current, P.modes, P.columns, P.traces, e)))
                         }
-                    }), [p, u, l, T.modes, T.columns, T.traces, T.types, T.decimators, o, y]),
-                    A = (0, n.useCallback)((() => {}), []),
-                    j = (0, n.useCallback)((e => c[g].tp_index ? c[g].tp_index[e] : e), [c, g]),
-                    N = (0, n.useCallback)((t => {
+                    }), [p, u, l, P.modes, P.columns, P.traces, P.types, P.decimators, o, y]),
+                    j = (0, n.useCallback)((() => {}), []),
+                    N = (0, n.useCallback)((e => c[g].tp_index ? c[g].tp_index[e] : e), [c, g]),
+                    D = (0, n.useCallback)((t => {
                         if (s) {
-                            const n = ((null == t ? void 0 : t.points) || []).reduce(((e, t) => (e[t.curveNumber] = e[t.curveNumber] || [], e[t.curveNumber].push(j(t.pointIndex)), e)), []);
+                            const n = ((null == t ? void 0 : t.points) || []).reduce(((e, t) => (e[t.curveNumber] = e[t.curveNumber] || [], e[t.curveNumber].push(N(t.pointIndex)), e)), []);
                             if (n.length) n.forEach(((t, n) => {
                                 const r = _d(s, `selected${n}`);
                                 r && t && t.length && p(Ss(r, t, y, e.onChange, d))
                             }));
-                            else if (1 === T.traces.length) {
+                            else if (1 === P.traces.length) {
                                 const t = _d(s, "selected0");
                                 t && p(Ss(t, [], y, e.onChange, d))
                             }
                         }
-                    }), [j, p, s, d, e.onChange, T.traces.length, y]);
+                    }), [N, p, s, d, e.onChange, P.traces.length, y]);
                 return S ? (0, t.jsx)(Pp, Object.assign({
                     id: l,
                     "data-testid": e.testId,
                     className: w,
                     ref: m
                 }, {
                     children: (0, t.jsx)(qr, Object.assign({
                         title: C || ""
                     }, {
                         children: (0, t.jsx)(n.Suspense, Object.assign({
                             fallback: (0, t.jsx)(yp, {
-                                sx: O
+                                sx: Z
                             }, "skeleton")
                         }, {
                             children: (0, t.jsx)(Ep, {
-                                data: Z,
-                                layout: P,
-                                style: E,
-                                onRelayout: R,
-                                onAfterPlot: A,
-                                onSelected: N,
-                                onDeselect: N,
-                                config: M
+                                data: M,
+                                layout: E,
+                                style: O,
+                                onRelayout: A,
+                                onAfterPlot: j,
+                                onSelected: D,
+                                onDeselect: D,
+                                config: R
                             })
                         }))
                     }))
                 }), "div") : null
             };
             const Fp = {
                 data: {
@@ -37380,17 +37379,20 @@
                         }), [o, d, w, h, g, e.onChange, k]),
                         N = (0, n.useCallback)((e => b(e.target.value)), []),
                         D = u && (c ? y : y.length > 0 ? y[0] : "");
                     return (0, t.jsxs)(zg, Object.assign({
                         sx: M,
                         className: C
                     }, {
-                        children: [e.label ? (0, t.jsx)(Ig, {
+                        children: [e.label ? (0, t.jsx)(Ig, Object.assign({
+                            disableAnimation: !0,
+                            className: u ? void 0 : "static-label"
+                        }, {
                             children: e.label
-                        }) : null, (0, t.jsx)(qr, Object.assign({
+                        })) : null, (0, t.jsx)(qr, Object.assign({
                             title: P || ""
                         }, {
                             children: u ? (0, t.jsx)(eb, Object.assign({
                                 id: r,
                                 multiple: c,
                                 value: D,
                                 onChange: A,
@@ -47814,15 +47816,20 @@
                                         r.forEach(((e, n) => t[n].payload.value = e)), e(bs(n))
                                     })).catch(console.warn)
                                 } else "MS" === n.type && Array.isArray(n.payload) ? n.payload.forEach((e => t(e))) : e(bs(n))
                             };
                             return t
                         })(t)), e.connect())
                     })(e.socket, r)
-                }), [e.socket]), (0, t.jsx)(jd.Provider, Object.assign({
+                }), [e.socket]), (0, n.useEffect)((() => {
+                    const e = [l];
+                    document.body.classList.forEach((t => {
+                        t.startsWith("taipy-") || e.push(t)
+                    })), document.body.className = e.join(" ")
+                }), [l]), (0, t.jsx)(jd.Provider, Object.assign({
                     value: {
                         state: e,
                         dispatch: r
                     }
                 }, {
                     children: (0, t.jsx)(bd, {
                         children: (0, t.jsx)(mN, Object.assign({
@@ -47835,16 +47842,15 @@
                                     dateAdapter: RR
                                 }, {
                                     children: (0, t.jsx)(Nd.Provider, Object.assign({
                                         value: QD
                                     }, {
                                         children: (0, t.jsxs)(GS, {
                                             children: [(0, t.jsxs)(Pp, Object.assign({
-                                                style: KD,
-                                                className: l
+                                                style: KD
                                             }, {
                                                 children: [(0, t.jsx)(lN, {}), (0, t.jsx)(Md, Object.assign({
                                                     FallbackComponent: ik
                                                 }, {
                                                     children: (0, t.jsx)(UD, Object.assign({}, e.menu))
                                                 })), (0, t.jsx)(Pp, Object.assign({
                                                     component: "main",
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy/gui/webapp/viselements.json` & `taipy-gui-2.3.0.dev2/src/taipy/gui/webapp/viselements.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967695815573131%*

 * *Differences: {"'blocks'": "{0: {1: {'properties': {1: {'doc': 'A list of CSS class names, separated by white "*

 * *             'spaces, that will be associated with the generated HTML Element.<br/>These class '*

 * *             "names are added to the default <code>taipy-part</code>.'}}}}, 3: {1: {'properties': "*

 * *             "{1: {'doc': 'The name of a function that is triggered when this pane is closed (if "*

 * *             'the user clicks outside of it or presses the Esc key).<br/>All parameters of that '*

 * *             'functi […]*

```diff
@@ -12,15 +12,15 @@
                         "default_value": "True",
                         "doc": "If True, this part is visible on the page.<br/>If False, the part is hidden and its content is not displayed.",
                         "name": "render",
                         "type": "dynamic(bool)"
                     },
                     {
                         "default_property": true,
-                        "doc": "List of CSS class names that will be associated with the generated HTML Element.<br/>This class names will be added to the default <code>taipy-part</code>.",
+                        "doc": "A list of CSS class names, separated by white spaces, that will be associated with the generated HTML Element.<br/>These class names are added to the default <code>taipy-part</code>.",
                         "name": "class_name",
                         "type": "dynamic(str)"
                     },
                     {
                         "doc": "The page to show as the content of the block (page name if defined or an URL in an <i>iframe</i>).<br/>This should not be defined if <i>partial</i> is set.",
                         "name": "page",
                         "type": "dynamic(str)"
@@ -95,15 +95,15 @@
                         "default_property": true,
                         "default_value": "False",
                         "doc": "If True, this pane is visible on the page.<br/>If False, the pane is hidden.",
                         "name": "open",
                         "type": "dynamic(bool)"
                     },
                     {
-                        "doc": "The name of a function that is be triggered when this pane is closed (if the user clicks outside of it or presses the Esc key).<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (optional[str]): the identifier of the button.</li>\n<li>action (optional[str]): the name of the action that provoked the change.</li>\n</ul><br/>If this property is not set, no function is called when this pane is closed.",
+                        "doc": "The name of a function that is triggered when this pane is closed (if the user clicks outside of it or presses the Esc key).<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (optional[str]): the identifier of the button.</li>\n<li>action (optional[str]): the name of the action that provoked the change.</li>\n</ul><br/>If this property is not set, no function is called when this pane is closed.",
                         "name": "on_close",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -154,15 +154,15 @@
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "default_value": "\"\"",
                         "doc": "The value displayed as text by this control.",
                         "name": "value",
-                        "type": "dynamic(Any)"
+                        "type": "dynamic(any)"
                     },
                     {
                         "default_value": "False",
                         "doc": "If set to True, the component renders as an HTML &lt;span&gt; element without any default style.",
                         "name": "raw",
                         "type": "bool"
                     },
@@ -225,15 +225,15 @@
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "default_value": "None",
                         "doc": "The value represented by this control.",
                         "name": "value",
-                        "type": "dynamic(Any)"
+                        "type": "dynamic(any)"
                     },
                     {
                         "default_value": "False",
                         "doc": "If True, the text is obscured: all input characters are displayed as an asterisk ('*').",
                         "name": "password",
                         "type": "bool"
                     },
@@ -267,15 +267,15 @@
                     "propagate"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The numerical value represented by this control.",
                         "name": "value",
-                        "type": "dynamic(Any)"
+                        "type": "dynamic(any)"
                     },
                     {
                         "default_value": "None",
                         "doc": "The label associated with the input.",
                         "name": "label",
                         "type": "str"
                     }
@@ -290,65 +290,65 @@
                     "propagate"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The value that is set for this slider.<br/>It would be a <i>lov</i> label if it is used.",
                         "name": "value",
-                        "type": "dynamic(int | float | str)"
+                        "type": "dynamic(int|float|str)"
                     },
                     {
                         "default_value": "0",
                         "doc": "The minimum value.<br/>This is ignored when <i>lov</i> is defined.",
                         "name": "min",
-                        "type": "int | float"
+                        "type": "int|float"
                     },
                     {
                         "default_value": "100",
                         "doc": "The maximum value.<br/>This is ignored when <i>lov</i> is defined.",
                         "name": "max",
-                        "type": "int | float"
+                        "type": "int|float"
                     },
                     {
                         "default_value": "\"bottom\"",
                         "doc": "When the <i>lov</i> property is used, this property indicates the location of the label.<br/>Possible values are:\n<ul>\n<li>\"bottom\"</li>\n<li>\"top\"</li>\n<li>\"left\"</li>\n<li>\"right\"</li>\n<li>\"none\" (no label is displayed)</li>\n</ul>",
                         "name": "text_anchor",
                         "type": "str"
                     },
                     {
                         "doc": "The labels for specific points of the slider.<br/>If set to True, this slider uses the labels of the <i>lov</i> if there are any.<br/>If set to a dictionary, the slider uses the dictionary keys as a <i>lov</i> key or index, and the associated value as the label.",
                         "name": "labels",
                         "type": "bool|dict"
                     },
                     {
                         "default_value": "True",
-                        "doc": "If set to False, the control emits an on_change notification only when the mouse button is released, otherwise notifications are emitted during the cursor movements. \nIf <i>lov</i> is defined, the default value is False.",
+                        "doc": "If set to False, the control emits an on_change notification only when the mouse button is released, otherwise notifications are emitted during the cursor movements.<br/>If <i>lov</i> is defined, the default value is False.",
                         "name": "continuous",
                         "type": "bool"
                     },
                     {
                         "default_value": "<i>App config</i>",
-                        "doc": "Minimum time between triggering two <i>on_change</i> calls.\nThe default value is defined at the application configuration level by the <strong>change_delay</strong> configuration option. if None or 0, there's no delay.",
+                        "doc": "Minimum time between triggering two <i>on_change</i> calls.<br/>The default value is defined at the application configuration level by the <strong>change_delay</strong> configuration option. if None or 0, there's no delay.",
                         "name": "change_delay",
                         "type": "int"
                     },
                     {
                         "default_value": "\"300px\"",
                         "doc": "The width, in CSS units, of this element.",
                         "name": "width",
                         "type": "str"
                     },
                     {
-                        "doc": "The height, in CSS units, of this element.\nIt defaults to the <i>width</i> value when using the vertical orientation.",
+                        "doc": "The height, in CSS units, of this element.<br/>It defaults to the <i>width</i> value when using the vertical orientation.",
                         "name": "height",
                         "type": "str"
                     },
                     {
                         "default_value": "\"horizontal\"",
-                        "doc": "The orientation of this slider.\nValid values are \"horizontal\" or \"vertical\".",
+                        "doc": "The orientation of this slider.<br/>Valid values are \"horizontal\" or \"vertical\".",
                         "name": "orientation",
                         "type": "str"
                     }
                 ]
             }
         ],
         [
@@ -383,26 +383,26 @@
                 "inherits": [
                     "on_change",
                     "propagate"
                 ],
                 "properties": [
                     {
                         "default_property": true,
-                        "doc": "The date that this control represents and can modify.\nIt is typically bound to a <code>datetime</code> object.",
+                        "doc": "The date that this control represents and can modify.<br/>It is typically bound to a <code>datetime</code> object.",
                         "name": "date",
                         "type": "dynamic(datetime)"
                     },
                     {
                         "default_value": "False",
                         "doc": "Whether or not to show the time part of the date.",
                         "name": "with_time",
                         "type": "bool"
                     },
                     {
-                        "doc": "The format to apply to the value.\nSee below.",
+                        "doc": "The format to apply to the value. See below.",
                         "name": "format",
                         "type": "str"
                     },
                     {
                         "default_value": "True",
                         "doc": "Shows the date as a formatted string if not editable.",
                         "name": "editable",
@@ -420,15 +420,15 @@
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The data object bound to this chart control.<br/>See the section on the <a href=\"#the-data-property\"><i>data</i> property</a> below for details.",
                         "name": "data",
                         "required": true,
-                        "type": "dynamic(Any)"
+                        "type": "dynamic(any)"
                     },
                     {
                         "default_value": "scatter",
                         "doc": "Chart type.<br/>See the Plotly <a href=\"https://plotly.com/javascript/reference/\">chart type</a> documentation for details.",
                         "name": "type",
                         "type": "indexed(str)"
                     },
@@ -526,15 +526,15 @@
                     {
                         "default_value": "True",
                         "doc": "If True, this chart is visible on the page.",
                         "name": "render",
                         "type": "dynamic(bool)"
                     },
                     {
-                        "doc": "Callback function called when the visible part of the x axis changes.<br/>The function receives four parameters:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (optional[str]): the identifier of the chart control.</li>\n<li>action (optional[str]): the name of the action that provoked the change.</li>\n<li>payload (dict[str, Any]): the full details on this callback's invocation, as emitted by <a href=\"https://plotly.com/javascript/plotlyjs-events/#update-data\">Plotly</a>.</li>\n</ul>",
+                        "doc": "The callback function that is invoked when the visible part of the x axis changes.<br/>The function receives four parameters:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (optional[str]): the identifier of the chart control.</li>\n<li>action (optional[str]): the name of the action that provoked the change.</li>\n<li>payload (dict[str, any]): the full details on this callback's invocation, as emitted by <a href=\"https://plotly.com/javascript/plotlyjs-events/#update-data\">Plotly</a>.</li>\n</ul>",
                         "name": "on_range_change",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -550,30 +550,30 @@
                                 "dict"
                             ]
                         ],
                         "type": "Callback"
                     },
                     {
                         "default_value": "_All columns_",
-                        "doc": "List of column names\n<ul>\n<li>str: ;-separated list of column names</li>\n<li>List[str]: list of names</li>\n<li>dict: {\"col_name\": {format: \"format\", index: 1}} if index is specified, it represents the display order of the columns.\nIf not, the list order defines the index</li>\n</ul>",
+                        "doc": "The list of column names\n<ul>\n<li>str: ;-separated list of column names</li>\n<li>list[str]: list of names</li>\n<li>dict: {\"column_name\": {format: \"format\", index: 1}} if index is specified, it represents the display order of the columns.\nIf not, the list order defines the index</li>\n</ul>",
                         "name": "columns",
-                        "type": "str|List[str]|dict[str, dict[str, str]]"
+                        "type": "str|list[str]|dict[str, dict[str, str]]"
                     },
                     {
                         "doc": "The label for the indicated trace.<br/>This is used when the mouse hovers over a trace.",
                         "name": "label",
                         "type": "indexed(str)"
                     },
                     {
                         "doc": "The name of the indicated trace.",
                         "name": "name",
                         "type": "indexed(str)"
                     },
                     {
-                        "doc": "List of the selected point indices.",
+                        "doc": "The list of the selected point indices  .",
                         "name": "selected",
                         "type": "indexed(dynamic(list[int]|str))"
                     },
                     {
                         "doc": "The color of the indicated trace (or a column name for scattered).",
                         "name": "color",
                         "type": "indexed(str)"
@@ -582,40 +582,40 @@
                         "doc": "The color of the selected points for the indicated trace.",
                         "name": "selected_color",
                         "type": "indexed(str)"
                     },
                     {
                         "doc": "The type of markers used for the indicated trace.<br/>See <a href=\"https://plotly.com/javascript/reference/scatter/#scatter-marker\">marker</a> for details.<br/>Color, opacity, size and symbol can be column name.",
                         "name": "marker",
-                        "type": "indexed(dict[str, Any])"
+                        "type": "indexed(dict[str, any])"
                     },
                     {
                         "doc": "The configuration of the line used for the indicated trace.<br/>See <a href=\"https://plotly.com/javascript/reference/scatter/#scatter-line\">line</a> for details.<br/>If the value is a string, it must be a dash type or pattern (see <a href=\"https://plotly.com/python/reference/scatter/#scatter-line-dash\">dash style of lines</a> for details).",
                         "name": "line",
-                        "type": "indexed(str|dict[str, Any])"
+                        "type": "indexed(str|dict[str, any])"
                     },
                     {
                         "doc": "The type of markers used for selected points in the indicated trace.<br/>See <a href=\"https://plotly.com/javascript/reference/scatter/#scatter-selected-marker\">selected marker for details.",
                         "name": "selected_marker",
-                        "type": "indexed(dict[str, Any])"
+                        "type": "indexed(dict[str, any])"
                     },
                     {
                         "doc": "The <i>plotly.js</i> compatible <a href=\"https://plotly.com/javascript/reference/layout/\">layout object</a>.",
                         "name": "layout",
-                        "type": "dict[str, Any]"
+                        "type": "dynamic(dict[str, any])"
                     },
                     {
                         "doc": "The <i>plotly.js</i> compatible <a href=\"https://plotly.com/javascript/configuration-options/\"> configuration options object</a>.",
                         "name": "plot_config",
-                        "type": "dict[str, Any]"
+                        "type": "dict[str, any]"
                     },
                     {
                         "doc": "The <i>plotly.js</i> compatible <a href=\"https://plotly.com/javascript/reference/\">data object where dynamic data will be overridden.</a>.",
                         "name": "options",
-                        "type": "indexed(dict[str, Any])"
+                        "type": "indexed(dict[str, any])"
                     },
                     {
                         "doc": "The orientation of the indicated trace.",
                         "name": "orientation",
                         "type": "indexed(str)"
                     },
                     {
@@ -681,15 +681,15 @@
                     "shared"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The content of the file.<br/>If a buffer is provided (string, array of bytes...), and in order to prevent the bandwidth to be consumed too much, the way the data is transferred depends on the the <i>data_url_max_size</i> parameter of the application configuration (which is set to 50kB by default):\n<ul>\n<li>If the size of the buffer is smaller than this setting, then the raw content is generated as a data URL, encoded using base64 (i.e. <code>\"data:&lt;mimetype&gt;;base64,&lt;data&gt;\"</code>).</li>\n<li>If the size of the buffer is greater than this setting, then it is transferred through a temporary file.</li>\n</ul>",
                         "name": "content",
-                        "type": "dynamic(url | path | file | ReadableBuffer)"
+                        "type": "dynamic(url|path|file|ReadableBuffer)"
                     },
                     {
                         "doc": "The label of the button.",
                         "name": "label",
                         "type": "dynamic(str)"
                     },
                     {
@@ -804,15 +804,15 @@
                     "shared"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The image source.<br/>If a buffer is provided (string, array of bytes...), and in order to prevent the bandwidth to be consumed too much, the way the image data is transferred depends on the the <i>data_url_max_size</i> parameter of the application configuration (which is set to 50kB by default):\n<ul>\n<li>If the size of the buffer is smaller than this setting, then the raw content is generated as a\n  data URL, encoded using base64 (i.e. <code>\"data:&lt;mimetype&gt;;base64,&lt;data&gt;\"</code>).</li>\n<li>If the size of the buffer is greater than this setting, then it is transferred through a temporary\n  file.</li>\n</ul>",
                         "name": "content",
-                        "type": "dynamic(url | path | file | ReadableBuffer)"
+                        "type": "dynamic(url|path|file|ReadableBuffer)"
                     },
                     {
                         "doc": "The label for this image.",
                         "name": "label",
                         "type": "dynamic(str)"
                     },
                     {
@@ -859,15 +859,15 @@
                     "shared"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The label to be displayed.<br/>This can be formatted if it is a numerical value.",
                         "name": "display",
-                        "type": "dynamic(Any)"
+                        "type": "dynamic(any)"
                     },
                     {
                         "default_value": "<i>min</i>",
                         "doc": "The location of the label on the [<i>min</i>, <i>max</i>] range.",
                         "name": "value",
                         "type": "dynamic(int,float)"
                     },
@@ -916,15 +916,15 @@
                     "active"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The list of menu option values.",
                         "name": "lov",
-                        "type": "dynamic(str|List[str|Icon|Any])"
+                        "type": "dynamic(str|list[str|Icon|any])"
                     },
                     {
                         "default_value": "`\"lambda x: str(x)\"`",
                         "doc": "The function that transforms an element of <i>lov</i> into a <i>tuple(id:str, label:str|Icon)</i>.",
                         "name": "adapter",
                         "type": "Function"
                     },
@@ -948,15 +948,15 @@
                     {
                         "default_value": "\"85vw\"",
                         "doc": "The width, in CSS units, of the menu when unfolded, on a mobile device.",
                         "name": "width[mobile]",
                         "type": "str"
                     },
                     {
-                        "doc": "The name of the function that will be triggered when a menu option is selected.<br/><br/>All the parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (str): the identifier of the button.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>args: List where the first element contains the id of the selected option.</li>\n</ul>\n</li>\n</ul>",
+                        "doc": "The name of the function that is triggered when a menu option is selected.<br/><br/>All the parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (str): the identifier of the button.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>args: List where the first element contains the id of the selected option.</li>\n</ul>\n</li>\n</ul>",
                         "name": "on_action",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -984,15 +984,15 @@
                     "active",
                     "shared"
                 ],
                 "properties": [
                     {
                         "doc": "The list of pages. The keys should be page id and start with \"/\", the values are labels. See the <a href=\"../../binding/#list-of-values\">section on List of Values</a> for details.",
                         "name": "lov",
-                        "type": "dict[str, Any]"
+                        "type": "dict[str, any]"
                     }
                 ]
             }
         ],
         [
             "selector",
             {
@@ -1044,21 +1044,21 @@
             {
                 "inherits": [
                     "shared"
                 ],
                 "properties": [
                     {
                         "default_property": true,
-                        "doc": "The different statuses to represent. See below.",
+                        "doc": "The different status items to represent. See below.",
                         "name": "value",
-                        "type": "dict|list[dict]|tuple|list[tuple]"
+                        "type": "tuple|dict|list[dict]|list[tuple]"
                     },
                     {
                         "default_value": "False",
-                        "doc": "If True, the user cannot hide the child statuses.",
+                        "doc": "If True, the user cannot remove the status items from the list.",
                         "name": "without_close",
                         "type": "bool"
                     }
                 ]
             }
         ],
         [
@@ -1070,103 +1070,103 @@
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The data to be represented in this table.",
                         "name": "data",
                         "required": true,
-                        "type": "Any"
+                        "type": "any"
                     },
                     {
                         "default_value": "100",
-                        "doc": "For paginated table, the number of rows displayed.",
+                        "doc": "For a paginated table, the number of visible rows.",
                         "name": "page_size",
                         "type": "int"
                     },
                     {
                         "default_value": "False",
-                        "doc": "For paginated table, adds an option to show all rows.",
+                        "doc": "For a paginated table, adds an option to show all the rows.",
                         "name": "allow_all_rows",
                         "type": "bool"
                     },
                     {
                         "default_value": "False",
-                        "doc": "For paginated table, show all rows.",
+                        "doc": "For a paginated table, show all the rows.",
                         "name": "show_all",
                         "type": "bool"
                     },
                     {
                         "default_value": "False",
-                        "doc": "data will be loaded on demand.",
+                        "doc": "If True, the data will be loaded on demand.",
                         "name": "auto_loading",
                         "type": "bool"
                     },
                     {
                         "doc": "The width, in CSS units, of the indicated column.",
-                        "name": "width[<i>col_name</i>]",
+                        "name": "width[<i>column_name</i>]",
                         "type": "str"
                     },
                     {
-                        "doc": "The list of the indices of the rows to show as selected.",
+                        "doc": "The list of the indices of the rows to be displayed as selected.",
                         "name": "selected",
                         "type": "list[int]|str"
                     },
                     {
                         "default_value": "[50, 100, 500]",
-                        "doc": "The list of available page sizes that users can choose.",
+                        "doc": "The list of available page sizes that users can choose from.",
                         "name": "page_size_options",
-                        "type": "List[int]|str"
+                        "type": "list[int]|str"
                     },
                     {
                         "default_value": "<i>shows all columns when empty</i>",
-                        "doc": "The list of the column names to display.\n<ul>\n<li>str: Semicolon (';')-separated list of column names.</li>\n<li>List[str]: list of column names</li>\n<li>dict: a dictionary with entries matching: {\"col name\": {format: \"format\", index: 1}}.<br/>\nif <i>index</i> is specified, it represents the display order of the columns.\nIf <i>index</i> is not specified, the list order defines the index.<br/>\nIf <i>format</i> is specified, it is used for numbers or dates.</li>\n</ul>",
+                        "doc": "The list of the column names to display.\n<ul>\n<li>str: Semicolon (';')-separated list of column names.</li>\n<li>list[str]: The list of column names.</li>\n<li>dict: A dictionary with entries matching: {\"col name\": {format: \"format\", index: 1}}.<br/>\nif <i>index</i> is specified, it represents the display order of the columns.\nIf <i>index</i> is not specified, the list order defines the index.<br/>\nIf <i>format</i> is specified, it is used for numbers or dates.</li>\n</ul>",
                         "name": "columns",
-                        "type": "str|List[str]|Dict[str, Dict[str, str|int]]"
+                        "type": "str|list[str]|dict[str, dict[str, str|int]]"
                     },
                     {
                         "default_value": "\"MM/dd/yyyy\"",
-                        "doc": "The date format that is used for all date columns when format is not specifically defined.",
+                        "doc": "The date format used for all date columns when the format is not specifically defined.",
                         "name": "date_format",
                         "type": "str"
                     },
                     {
-                        "doc": "The number format that is used for all number columns when format is not specifically defined.",
+                        "doc": "The number format used for all number columns when the format is not specifically defined.",
                         "name": "number_format",
                         "type": "str"
                     },
                     {
                         "default_value": "False",
                         "doc": "Indicates, if True, that the given column can be aggregated.<br/>See <a href=\"#aggregation\">below</a> for details.",
-                        "name": "group_by[<i>col_name</i>]",
+                        "name": "group_by[<i>column_name</i>]",
                         "type": "bool"
                     },
                     {
                         "default_value": "\"first\"",
                         "doc": "The name of the aggregation function to use.<br/>This is used only if <i>group_by[column_name]</i> is set to True.<br/>See <a href=\"#aggregation\">below</a> for details.",
-                        "name": "apply[<i>col_name</i>]",
+                        "name": "apply[<i>column_name</i>]",
                         "type": "str"
                     },
                     {
-                        "doc": "Allows the styling of table lines.<br/>See <a href=\"#styling\">below</a> for details.",
+                        "doc": "Allows the styling of table lines.<br/>See <a href=\"#dynamic-styling\">below</a> for details.",
                         "name": "style",
                         "type": "str"
                     },
                     {
-                        "doc": "Allows the styling of table cells.<br/>See <a href=\"#styling\">below</a> for details.",
-                        "name": "style[<i>col_name</i>]",
+                        "doc": "Allows the styling of table cells.<br/>See <a href=\"#dynamic-styling\">below</a> for details.",
+                        "name": "style[<i>column_name</i>]",
                         "type": "str"
                     },
                     {
                         "doc": "The name of the function that must return a tooltip text for a cell.<br/>See <a href=\"#cell%20tooltip\">below</a> for details.",
                         "name": "tooltip",
                         "type": "str"
                     },
                     {
                         "doc": "The name of the function that must return a tooltip text for a cell.<br/>See <a href=\"#cell%20tooltip\">below</a> for details.",
-                        "name": "tooltip[<i>col_name</i>]",
+                        "name": "tooltip[<i>column_name</i>]",
                         "type": "str"
                     },
                     {
                         "default_value": "\"100%\"",
                         "doc": "The width, in CSS units, of this table control.",
                         "name": "width",
                         "type": "str"
@@ -1182,43 +1182,43 @@
                         "doc": "Indicates, if True, that all columns can be filtered.",
                         "name": "filter",
                         "type": "bool"
                     },
                     {
                         "default_value": "False",
                         "doc": "Indicates, if True, that the indicated column can be filtered.",
-                        "name": "filter[<i>col_name</i>]",
+                        "name": "filter[<i>column_name</i>]",
                         "type": "bool"
                     },
                     {
                         "default_value": "\"\"",
                         "doc": "The replacement text for NaN (not-a-number) values.",
                         "name": "nan_value",
                         "type": "str"
                     },
                     {
                         "default_value": "\"\"",
                         "doc": "The replacement text for NaN (not-a-number) values for the indicated column.",
-                        "name": "nan_value[<i>col_name</i>]",
+                        "name": "nan_value[<i>column_name</i>]",
                         "type": "str"
                     },
                     {
                         "default_value": "True",
                         "doc": "Indicates, if True, that all columns can be edited.",
                         "name": "editable",
                         "type": "dynamic(bool)"
                     },
                     {
                         "default_value": "editable",
                         "doc": "Indicates, if False, that the indicated column cannot be edited when editable is True.",
-                        "name": "editable[<i>col_name</i>]",
+                        "name": "editable[<i>column_name</i>]",
                         "type": "bool"
                     },
                     {
-                        "doc": "The name of a function that is to be triggered when a cell edition is validated.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li>\n<li>col (str): the column name.</li>\n<li>value (Any): the new cell value cast to the type of the column.</li>\n<li>user_value (str): the new cell value as entered by the user.</li>\n</ul>\n</li>\n</ul><br/>If this property is not set, the user cannot edit cells.",
+                        "doc": "The name of a function that is triggered when a cell edition is validated.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li>\n<li>col (str): the column name.</li>\n<li>value (any): the new cell value cast to the type of the column.</li>\n<li>user_value (str): the new cell value, as it was provided by the user.</li>\n</ul>\n</li>\n</ul><br/>If this property is not set, the user cannot edit cells.",
                         "name": "on_edit",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -1233,15 +1233,15 @@
                                 "payload",
                                 "dict"
                             ]
                         ],
                         "type": "Callback"
                     },
                     {
-                        "doc": "The name of a function that is to be triggered when a row is deleted.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li>\n</ul>\n</li>\n</ul><br/>If this property is not set, the user cannot delete rows.",
+                        "doc": "The name of a function that is triggered when a row is deleted.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li>\n</ul>\n</li>\n</ul><br/>If this property is not set, the user cannot delete rows.",
                         "name": "on_delete",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -1256,15 +1256,15 @@
                                 "payload",
                                 "dict"
                             ]
                         ],
                         "type": "str"
                     },
                     {
-                        "doc": "The name of a function that is to be triggered when the user requests a row to be added.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>This dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li>\n</ul>\n</li>\n</ul><br/>If this property is not set, the user cannot add rows.",
+                        "doc": "The name of a function that is triggered when the user requests a row to be added.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>This dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li>\n</ul>\n</li>\n</ul><br/>If this property is not set, the user cannot add rows.",
                         "name": "on_add",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -1279,15 +1279,15 @@
                                 "payload",
                                 "dict"
                             ]
                         ],
                         "type": "str"
                     },
                     {
-                        "doc": "The name of a function that is to be triggered when the user selects a row.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>This dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li></ul></li></ul>.",
+                        "doc": "The name of a function that is triggered when the user selects a row.<br/>All parameters of that function are optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the name of the tabular data variable.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>This dictionary has the following keys:\n<ul>\n<li>index (int): the row index.</li></ul></li></ul>.",
                         "name": "on_action",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -1303,21 +1303,21 @@
                                 "dict"
                             ]
                         ],
                         "type": "str"
                     },
                     {
                         "default_value": "\"small\"",
-                        "doc": "The size of the rows, valid values are \"small\" and \"medium\".",
+                        "doc": "The size of the rows.<br/>Valid values are \"small\" and \"medium\".",
                         "name": "size",
                         "type": "str"
                     },
                     {
                         "default_value": "False",
-                        "doc": "Allows dynamic columns refresh if set to True.",
+                        "doc": "If set to True, this allows to dynamically refresh the  columns.",
                         "name": "rebuild",
                         "type": "dynamic(bool)"
                     }
                 ]
             }
         ],
         [
@@ -1333,15 +1333,15 @@
                         "default_property": true,
                         "default_value": "False",
                         "doc": "If True, the dialog is visible. If False, it is hidden.",
                         "name": "open",
                         "type": "bool"
                     },
                     {
-                        "doc": "Name of a function that is triggered when a button is pressed.<br/>The parameters of that function are all optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (str): the identifier of the dialog.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>This dictionary has the following keys:\n<ul>\n<li>args: a list where the first element contains the index of the selected label.</li>\n</ul>\n</li>\n</ul>",
+                        "doc": "Name of a function triggered when a button is pressed.<br/>The parameters of that function are all optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (str): the identifier of the dialog.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>This dictionary has the following keys:\n<ul>\n<li>args: a list where the first element contains the index of the selected label.</li>\n</ul>\n</li>\n</ul>",
                         "name": "on_action",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -1438,20 +1438,20 @@
                     "on_change"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "Bound to the selection value.",
                         "name": "value",
-                        "type": "dynamic(Any)"
+                        "type": "dynamic(any)"
                     },
                     {
                         "doc": "The list of values. See the <a href=\"../../binding/#list-of-values\">section on List of Values</a> for details.",
                         "name": "lov",
-                        "type": "dict[str, Any]"
+                        "type": "dict[str, any]"
                     },
                     {
                         "default_value": "`lambda x: str(x)`",
                         "doc": "The function that transforms an element of <i>lov</i> into a <i>tuple(id:str, label:str|Icon)</i>.",
                         "name": "adapter",
                         "type": "Function"
                     },
@@ -1471,15 +1471,15 @@
             }
         ],
         [
             "on_change",
             {
                 "properties": [
                     {
-                        "doc": "The name of a function that is triggered when the value is updated.<br/>The parameters of that function are all optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the variable name.</li>\n<li>value (Any): the new value.</li>\n</ul>",
+                        "doc": "The name of a function that is triggered when the value is updated.<br/>The parameters of that function are all optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>var_name (str): the variable name.</li>\n<li>value (any): the new value.</li>\n</ul>",
                         "name": "on_change",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -1537,15 +1537,15 @@
                     {
                         "default_value": "<i>App config</i>",
                         "doc": "Minimum time between triggering two calls to the <i>on_change</i> callback.<br/>The default value is defined at the application configuration level by the <strong>change_delay</strong> configuration option. if None, the delay is set to 300 ms.",
                         "name": "change_delay",
                         "type": "int"
                     },
                     {
-                        "doc": "Name of a function that is triggered when a specific key is pressed.<br/>The parameters of that function are all optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (str): the identifier of the input.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>args (List):\n<ul><li>key name</li><li>variable name</li><li>current value</li></ul>\n</li>\n</ul>\n</li>\n</ul>",
+                        "doc": "Name of a function that is triggered when a specific key is pressed.<br/>The parameters of that function are all optional:\n<ul>\n<li>state (<code>State^</code>): the state instance.</li>\n<li>id (str): the identifier of the input.</li>\n<li>action (str): the name of the action that provoked the change.</li>\n<li>payload (dict): the details on this callback's invocation.<br/>\nThis dictionary has the following keys:\n<ul>\n<li>args (list):\n<ul><li>key name</li><li>variable name</li><li>current value</li></ul>\n</li>\n</ul>\n</li>\n</ul>",
                         "name": "on_action",
                         "signature": [
                             [
                                 "state",
                                 "State"
                             ],
                             [
@@ -1580,23 +1580,23 @@
                         "doc": "The identifier that will be assigned to the rendered HTML component.",
                         "name": "id",
                         "type": "str"
                     },
                     {
                         "doc": "Bound to a dictionary that contains additional properties for this element.",
                         "name": "properties",
-                        "type": "dict[str, Any]"
+                        "type": "dict[str, any]"
                     },
                     {
-                        "doc": "List of CSS class names that will be associated with the generated HTML Element.<br/>This class names will be added to the default <code>taipy-&lt;element_type&gt;</code>.",
+                        "doc": "The list of CSS class names that will be associated with the generated HTML Element.<br/>These class names will be added to the default <code>taipy-&lt;element_type&gt;</code>.",
                         "name": "class_name",
                         "type": "dynamic(str)"
                     },
                     {
-                        "doc": "Information that is displayed when the user hovers over this element.",
+                        "doc": "The information that is displayed when the user hovers over this element.",
                         "name": "hover_text",
                         "type": "dynamic(str)"
                     }
                 ]
             }
         ]
     ]
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/PKG-INFO` & `taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/SOURCES.txt` & `taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev1/src/taipy_gui.egg-info/requires.txt` & `taipy-gui-2.3.0.dev2/src/taipy_gui.egg-info/requires.txt`

 * *Files identical despite different names*

