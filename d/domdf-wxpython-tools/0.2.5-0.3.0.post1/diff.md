# Comparing `tmp/domdf_wxpython_tools-0.2.5.tar.gz` & `tmp/domdf_wxpython_tools-0.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/domdf_wxpython_tools-0.2.5.tar", last modified: Thu Apr 16 19:58:01 2020, max compression
+gzip compressed data, was "domdf_wxpython_tools-0.3.0.post1.tar", last modified: Mon Jun  5 13:51:33 2023, max compression
```

## Comparing `domdf_wxpython_tools-0.2.5.tar` & `domdf_wxpython_tools-0.3.0.post1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2126 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/__pkginfo__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8267 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/chartpanel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9624 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/dialogs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1916 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/projections.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4514 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/validators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1846 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/icons.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16173 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/picker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9880 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/StylePickerPanel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15788 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/logctrl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10845 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/ColourPickerPanel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4758 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/style_picker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/timer_thread.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2218 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10641 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/imagepanel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2284 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/keyboard.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2574 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/tabbable_textctrl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6717 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/border_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4208 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23380 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/filebrowsectrl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5041 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/list_dialog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35885 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/clearable_textctrl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16749 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/editable_listbox.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-16 19:58:01.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16132 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/panel_listctrl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3672 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4334 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/font_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1410 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5074 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/css_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2519 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/WebView.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3910 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7652 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      919 2020-04-16 19:57:35.000000 domdf_wxpython_tools-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:51:33.622768 domdf_wxpython_tools-0.3.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15093 2023-06-05 13:51:33.622768 domdf_wxpython_tools-0.3.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:51:33.618768 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)    10794 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/ColourPickerPanel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10689 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/StylePickerPanel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/WebView.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/border_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8405 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/chartpanel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29466 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/clearable_textctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9569 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16958 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/editable_listbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18198 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/filebrowsectrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/icons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10580 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/imagepanel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5050 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/list_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15602 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/logctrl.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:51:33.622768 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/Default.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5106 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/css_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4617 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/font_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16337 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/panel_listctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9770 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/picker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/projections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6076 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/style_picker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/tabbable_textctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8012 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/textctrlwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/timer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4978 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:51:33.618768 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15093 2023-06-05 13:51:33.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-05 13:51:33.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 13:51:33.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 13:51:33.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-05 13:51:33.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-05 13:51:33.000000 domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5938 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-05 13:51:33.622768 domdf_wxpython_tools-0.3.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-05 13:50:55.000000 domdf_wxpython_tools-0.3.0.post1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools.egg-info/SOURCES.txt` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
-__pkginfo__.py
+pyproject.toml
 requirements.txt
+setup.cfg
 setup.py
 domdf_wxpython_tools/ColourPickerPanel.py
 domdf_wxpython_tools/StylePickerPanel.py
 domdf_wxpython_tools/WebView.py
 domdf_wxpython_tools/__init__.py
 domdf_wxpython_tools/border_config.py
 domdf_wxpython_tools/chartpanel.py
@@ -20,20 +21,23 @@
 domdf_wxpython_tools/keyboard.py
 domdf_wxpython_tools/list_dialog.py
 domdf_wxpython_tools/logctrl.py
 domdf_wxpython_tools/picker.py
 domdf_wxpython_tools/projections.py
 domdf_wxpython_tools/style_picker.py
 domdf_wxpython_tools/tabbable_textctrl.py
+domdf_wxpython_tools/textctrlwrapper.py
 domdf_wxpython_tools/timer_thread.py
 domdf_wxpython_tools/utils.py
 domdf_wxpython_tools/validators.py
 domdf_wxpython_tools.egg-info/PKG-INFO
 domdf_wxpython_tools.egg-info/SOURCES.txt
 domdf_wxpython_tools.egg-info/dependency_links.txt
+domdf_wxpython_tools.egg-info/not-zip-safe
 domdf_wxpython_tools.egg-info/requires.txt
 domdf_wxpython_tools.egg-info/top_level.txt
+domdf_wxpython_tools/panel_listctrl/Default.css
 domdf_wxpython_tools/panel_listctrl/__init__.py
 domdf_wxpython_tools/panel_listctrl/constants.py
 domdf_wxpython_tools/panel_listctrl/css_parser.py
 domdf_wxpython_tools/panel_listctrl/font_parser.py
 domdf_wxpython_tools/panel_listctrl/panel_listctrl.py
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/chartpanel.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/chartpanel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #  !/usr/bin/env python
-#   -*- coding: utf-8 -*-
+
 #
 #  chartpanel.py
 """
 A canvas for displaying a chart within a wxPython window
 """
 #
-#  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright (c) 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Method ``constrain_zoom`` based on https://stackoverflow.com/a/16709952/3092681
 #  Copyright 2013 simonb
 #  https://stackoverflow.com/users/456805/simonb
 #
 #  Method ``setup_scrollwheel_zooming`` based on https://stackoverflow.com/a/11562898/3092681
 #  Copyright 2012 Thomas A Caswell
@@ -28,259 +28,248 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
-
 # stdlib
 import types
+from typing import Optional
 
 # 3rd party
-import matplotlib
+import matplotlib  # type: ignore
+import matplotlib.projections  # type: ignore[import]
 import numpy
-import wx.html2
-from matplotlib.backends.backend_wxagg import (
-	FigureCanvasWxAgg as FigureCanvas,
-	NavigationToolbar2WxAgg as NavigationToolbar,
-	)
+import wx.html2  # type: ignore
+from matplotlib.axes import Axes  # type: ignore
+from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg as FigureCanvas  # type: ignore
+from matplotlib.backends.backend_wxagg import NavigationToolbar2WxAgg as NavigationToolbar
+from matplotlib.figure import Figure  # type: ignore
 
 # this package
 from domdf_wxpython_tools.border_config import border_config
 from domdf_wxpython_tools.projections import XPanAxes
 
+__all__ = ["ChartPanelBase"]
 
 # Constrain zoom to X axis
 matplotlib.projections.register_projection(XPanAxes)
 
 
 class ChartPanelBase(wx.Panel):
 	"""
 	Panel that contains a matplotlib plotting window, used for displaying an image.
 	The image can be right clicked to bring up a context menu allowing copying, pasting and saving of the image.
 	The image can be panned by holding the left mouse button and moving the mouse,
 	and zoomed in and out using the scrollwheel on the mouse.
+
+	:param parent: The parent window.
+	:param fig:
+	:param ax:
+	:param id: An identifier for the panel. wx.ID_ANY is taken to mean a default.
+	:param pos: The panel position. The value ``wx.DefaultPosition`` indicates a default position,
+		chosen by either the windowing system or wxWidgets, depending on platform.
+	:param size: The panel size. The value ::wxDefaultSize indicates a default size, chosen by
+		either the windowing system or wxWidgets, depending on platform.
+	:param style: The window style. See wxPanel.
+	:param name: Window name.
 	"""
-	
+
 	def __init__(
-			self, parent, fig, ax, id=wx.ID_ANY, pos=wx.DefaultPosition, size=wx.DefaultSize,
-			style=0, name=wx.PanelNameStr
+			self,
+			parent: wx.Window,
+			fig: Figure,
+			ax: Axes,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = 0,
+			name: str = wx.PanelNameStr
 			):
-		"""
-		:param parent: The parent window.
-		:type parent: wx.Window
-		:param fig:
-		:type fig:
-		:param ax:
-		:type ax:
-		:param id: An identifier for the panel. wx.ID_ANY is taken to mean a default.
-		:type id: wx.WindowID, optional
-		:param pos: The panel position. The value ::wxDefaultPosition indicates a default position,
-		:type pos: wx.Point, optional
-			chosen by either the windowing system or wxWidgets, depending on platform.
-		:param size: The panel size. The value ::wxDefaultSize indicates a default size, chosen by
-		:type size: wx.Size, optional
-			either the windowing system or wxWidgets, depending on platform.
-		:param style: The window style. See wxPanel.
-		:type style: int, optional
-		:param name: Window name.
-		:type name: str, optional
-		"""
-		
+
 		wx.Panel.__init__(self, parent, id, pos, size, style | wx.TAB_TRAVERSAL, name)
-		
+
 		self.fig = fig
 		self.ax = ax
-		
+
 		self.canvas = FigureCanvas(self, wx.ID_ANY, self.fig)
 		self._do_layout()
-		
+
 		self.toolbar = NavigationToolbar(self.canvas)
 		self.toolbar.Hide()
-		
+
 		self.Bind(wx.EVT_SIZE, self.on_size_change, self)
 		self.Bind(wx.EVT_MAXIMIZE, self.on_size_change)
-	
+
 	def setup_ylim_refresher(self, y_data, x_data):
 		"""
-		Setup the function for updating the ylim whenever the xlim changes.s
-		
+		Setup the function for updating the ylim whenever the xlim changes.
+
 		:param y_data:
-		:type y_data:
 		:param x_data:
-		:type x_data:
 		"""
-		
+
 		def update_ylim(*args):
 			# print(str(*args).startswith("MPL MouseEvent")) # Pan
-			if (str(*args).startswith("XPanAxesSubplot") and self.canvas.toolbar._active != "PAN") or (
-					str(*args).startswith("MPL MouseEvent") and self.canvas.toolbar._active != "ZOOM"):  # Zoom, Pan
+
+			# Zoom, Pan
+			if ((str(*args).startswith("XPanAxesSubplot") and self.canvas.toolbar._active != "PAN")
+				or (str(*args).startswith("MPL MouseEvent") and self.canvas.toolbar._active != "ZOOM")):
 				# print("updated xlims: ", axes.get_xlim())
 				min_x_index = (numpy.abs(x_data - self.ax.get_xlim()[0])).argmin()
 				max_x_index = (numpy.abs(x_data - self.ax.get_xlim()[1])).argmin()
 				# print(min_x_index, max_x_index)
-				
+
 				y_vals_for_range = numpy.take(y_data, [idx for idx in range(min_x_index, max_x_index)])
 				# print(max(y_vals_for_range))
 				self.ax.set_ylim(bottom=0, top=max(y_vals_for_range) * 1.1)
 				self.fig.canvas.draw()
 				# print("x-val: {}, y-val:{}
 				self.size_change()
-		
-		self.ax.callbacks.connect('xlim_changed', update_ylim)
+
+		self.ax.callbacks.connect("xlim_changed", update_ylim)
 		self.fig.canvas.callbacks.connect("button_release_event", update_ylim)
-	
-	def _do_layout(self):
+
+	def _do_layout(self) -> None:
 		# begin wxGlade: ChromatogramPanel.__do_layout
 		sizer = wx.FlexGridSizer(1, 2, 0, 0)
 		sizer.Add(self.canvas, 1, wx.EXPAND, 0)
 		self.SetSizer(sizer)
 		sizer.Fit(self)
 		self.Layout()
-	
-	def reset_view(self, *_):
+
+	def reset_view(self, *_) -> None:
 		"""
-		Reset the view of the chart
+		Reset the view of the chart.
 		"""
-		
+
 		self.canvas.toolbar.home()
 		self.canvas.draw_idle()
-	
-	def previous_view(self, *_):
+
+	def previous_view(self, *_) -> None:
 		"""
-		Go to the previous view of the chart
+		Go to the previous view of the chart.
 		"""
-		
+
 		self.canvas.toolbar.back()
-	
-	def zoom(self, enable=True):
+
+	def zoom(self, enable: bool = True) -> None:
 		"""
-		Enable the Zoom tool
+		Enable the Zoom tool.
 		"""
-		
+
 		if enable or (not enable and self.canvas.toolbar._active == "ZOOM"):
 			self.canvas.toolbar.zoom()
 		self.canvas.Refresh()
-	
-	def pan(self, enable=True):
+
+	def pan(self, enable: bool = True) -> None:
 		"""
-		Enable the Pan tool
+		Enable the Pan tool.
 		"""
-		
+
 		if enable or (not enable and self.canvas.toolbar._active == "PAN"):
 			self.canvas.toolbar.pan()
 		self.canvas.Refresh()
-	
-	def configure_borders(self, event=None):
+
+	def configure_borders(self, event: Optional[wx.Event] = None):
 		"""
-		Open the 'Configure Borders' dialog
+		Open the ``Configure Borders`` dialog.
 		"""
-		
+
 		self.border_config = border_config(self, self.fig)
 		self.border_config.Show()
-		
+
 		if event:
 			event.Skip()
-	
-	def constrain_zoom(self, key="x"):
+
+	def constrain_zoom(self, key: str = 'x') -> None:
 		"""
-		Constrain zoom to the x axis only
+		Constrain zoom to the x axis only.
 
 		:param key:
-		:type key:
-		:return:
-		:rtype:
 		"""
+
 		def press_zoom(self, event):
 			event.key = key
 			NavigationToolbar.press_zoom(self, event)
-		
-		self.fig.canvas.toolbar.press_zoom = types.MethodType(
-				press_zoom,
-				self.fig.canvas.toolbar
-				)
-	
+
+		self.fig.canvas.toolbar.press_zoom = types.MethodType(press_zoom, self.fig.canvas.toolbar)
+
 	# Other Toolbar Options
 	# Save chromatogram as image: save_figure(self, *args)
 	# set_cursor(self, cursor)
 	# Set the current cursor to one of the :class:`Cursors` enums values.
-	
+
 	# If required by the backend, this method should trigger an update in
 	# the backend event loop after the cursor is set, as this method may be
 	# called e.g. before a long-running task during which the GUI is not
 	# updated.
 	# set_history_buttons(self)
 	# Enable or disable the back/forward button.
 	# forward(self, *args)
 	# move forward in the view lim stack.
 	# print(axes.get_ylim())
 	# end of class ChromatogramPanel
-	
-	def size_change(self):
+
+	def size_change(self) -> None:
 		"""
-		Internal function that runs whenever the window is resized
+		Internal function that runs whenever the window is resized.
 		"""
-		
+
 		# self.canvas.SetMinSize(self.GetSize())
 		self.canvas.SetSize(self.GetSize())
 		self.Refresh()
 		self.canvas.draw()
 		self.canvas.Refresh()
-	
+
 		# if event.ClassName == "wxSizeEvent":
 		# 	event.Skip()
-	
-	def on_size_change(self, event):
+
+	def on_size_change(self, _) -> None:
 		"""
 		Event handler for size change events
 		"""
-		
+
 		self.size_change()
 		# event.Skip()
-	
-	def setup_scrollwheel_zooming(self, scale=1.1):
+
+	def setup_scrollwheel_zooming(self, scale: float = 1.1) -> None:
 		"""
-		Allow zooming of the chart with the scrollwheel
-		
+		Allow zooming of the chart with the scrollwheel.
+
 		:param scale:
-		:type scale:
 		"""
-		
-		def zoom_factory(ax, base_scale=1.1):
+
+		def zoom_factory(ax, base_scale: float = 1.1):
+
 			def zoom_fun(event):
 				# get the current x and y limits
 				cur_xlim = ax.get_xlim()
 				cur_ylim = ax.get_ylim()
 				cur_xrange = (cur_xlim[1] - cur_xlim[0]) * .5
 				cur_yrange = (cur_ylim[1] - cur_ylim[0]) * .5
 				xdata = event.xdata  # get event x location
 				ydata = event.ydata  # get event y location
-				if event.button == 'up':
+				if event.button == "up":
 					# deal with zoom in
 					scale_factor = 1 / base_scale
-				elif event.button == 'down':
+				elif event.button == "down":
 					# deal with zoom out
 					scale_factor = base_scale
 				else:
 					# deal with something that should never happen
 					scale_factor = 1
 					print(event.button)
 				# set new limits
-				ax.set_xlim([
-						xdata - cur_xrange * scale_factor,
-						xdata + cur_xrange * scale_factor
-						])
-				ax.set_ylim([
-						ydata - cur_yrange * scale_factor,
-						ydata + cur_yrange * scale_factor
-						])
+				ax.set_xlim([xdata - cur_xrange * scale_factor, xdata + cur_xrange * scale_factor])
+				ax.set_ylim([ydata - cur_yrange * scale_factor, ydata + cur_yrange * scale_factor])
 				self.canvas.draw()  # force re-draw
-			
+
 			fig = ax.get_figure()  # get the figure of interest
 			# attach the call back
-			fig.canvas.mpl_connect('scroll_event', zoom_fun)
-			
+			fig.canvas.mpl_connect("scroll_event", zoom_fun)
+
 			# return the function
 			return zoom_fun
-		
+
 		self.__zoom_factory = zoom_factory(self.ax, base_scale=scale)
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/dialogs.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/dialogs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  dialogs.py
 """
 Several dialog classes and helper functions for file/folder dialogs
 """
 #
 #  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
@@ -22,322 +21,327 @@
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
 # stdlib
 import os
+from typing import List, Optional, Sequence
 
 # 3rd party
-import wx
+import wx  # type: ignore
 
 # this package
 from domdf_wxpython_tools.validators import CharValidator
-from domdf_wxpython_tools.list_dialog import list_dialog
+
+__all__ = [
+		"file_dialog_wildcard",
+		"file_dialog_multiple",
+		"file_dialog",
+		"FloatEntryDialog",
+		"IntEntryDialog",
+		"Wildcards"
+		]
 
 # style enumeration
 style_uppercase = 4
 style_lowercase = 8
 style_hidden = 16
 
-
 common_filetypes = {
 		"jpeg": ("JPEG files", ["jpg", "jpeg"]),
 		"png": ("PNG files", ["png"]),
 		"bmp": ("BMP files", ["bmp"]),
 		"tiff": ("TIFF files", ["tiff", "tif"]),
 		"gif": ("GIF files", ["gif"])
 		# TODO: Add more
 		}
 
 
-def file_dialog_wildcard(parent, title, wildcard, style=wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT, **kwargs):
+def file_dialog_wildcard(
+		parent: wx.Window,
+		title: str,
+		wildcard: str,
+		style: int = wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT,
+		**kwargs,
+		) -> Optional[List[str]]:
 	"""
 	Create a wx.FileDialog with the wildcard string given, and return a list of the files selected.
-	
-	:param parent:
-	:type parent:
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
 	:param wildcard:
-	:type wildcard:
 	:param title:
-	:type title:
 	:param style:
-	:type style:
 	:param kwargs:
-	:type kwargs:
 
 	:return: List of filenames for the selected files. If wx.FD_MULTIPLE is not in the style, the list will contain only one element
 	:rtype: list of str
 	"""
-	
-	with wx.FileDialog(
-			parent, title,
-			wildcard=wildcard,
-			style=style, **kwargs
-			) as fileDialog:
-		
+
+	with wx.FileDialog(parent, title, wildcard=wildcard, style=style, **kwargs) as fileDialog:
+
 		if fileDialog.ShowModal() == wx.ID_CANCEL:
-			return  # the user changed their mind
-		
+			return None  # the user changed their mind
+
 		try:
 			pathnames = fileDialog.GetPaths()
 		except:
 			pathnames = [fileDialog.GetPath()]
-		
-		filter_extension_list = wildcard.split("|")[1::2]
-		valid_extensions = [os.path.splitext(ext)[1] for ext in ";".join(filter_extension_list).split(";")]
+
+		filter_extension_list = wildcard.split('|')[1::2]
+		valid_extensions = [os.path.splitext(ext)[1] for ext in ';'.join(filter_extension_list).split(';')]
 		selected_filter_index = fileDialog.GetFilterIndex()
-		
-		selected_filter_extensions = filter_extension_list[selected_filter_index].replace("*.", ".").split(";")
-		
+
+		selected_filter_extensions = filter_extension_list[selected_filter_index]
+		selected_filter_extensions = selected_filter_extensions.replace("*.", '.').split(';')
+
 		for index, pathname in enumerate(pathnames):
 			if selected_filter_extensions[0] != ".*":
 				if os.path.splitext(pathname)[-1].lower() not in selected_filter_extensions:
 					pathnames[index] = pathname + f"{selected_filter_extensions[0]}"
-		
+
 		return pathnames
 
 
-def file_dialog_multiple(parent, extension, title, filetypestring, style=wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT, **kwargs):
-	"""
-	Create a wx.FileDialog with for the extension and filetypestring given, and return a list of the files selected.
-	
-	:param parent:
-	:type parent:
+def file_dialog_multiple(
+		parent: wx.Window,
+		extension: str,
+		title: str,
+		filetypestring: str,
+		style=wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT,
+		**kwargs
+		) -> Optional[List[str]]:
+	r"""
+	Create a :class:`wx.FileDialog` with the extension and filetypestring given,
+	and return a list of the files selected.
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
 	:param extension:
-	:type extension:
 	:param title:
-	:type title:
 	:param filetypestring:
-	:type filetypestring:
 	:param style:
-	:type style:
-	:param kwargs:
-	:type kwargs:
-	
-	:return: List of filenames for the selected files. If wx.FD_MULTIPLE is not in the style, the list will contain only one element
-	:rtype: list of str
+	:param \*\*kwargs:
+
+	:return: List of filenames for the selected files.
+		If ``wx.FD_MULTIPLE`` is not in the style, the list will contain only one element.
 	"""
-	
+
 	with wx.FileDialog(
-			parent, title,
+			parent,
+			title,
 			wildcard=f"{filetypestring} (*.{extension.lower()})|*.{extension.lower()};*.{extension.upper()}",
-			style=style, **kwargs
-	) as fileDialog:
-		
+			style=style,
+			**kwargs
+			) as fileDialog:
+
 		if fileDialog.ShowModal() == wx.ID_CANCEL:
-			return  # the user changed their mind
-		
+			return None  # the user changed their mind
+
 		try:
 			pathnames = fileDialog.GetPaths()
 		except:
 			pathnames = [fileDialog.GetPath()]
-		
+
 		for index, pathname in enumerate(pathnames):
-			if extension != "*":
+			if extension != '*':
 				if os.path.splitext(pathname)[-1].lower() != f".{extension}":
 					pathnames[index] = pathname + f".{extension}"
 		# else:
 		# 	pathnames[index] = os.path.splitext(pathname)[0]
-		
+
 		return pathnames
 
 
-def file_dialog(*args, **kwargs):
-	"""
-	Create a wx.FileDialog with for the extension and filetypestring given, and return the filename selected.
-	
+def file_dialog(*args, **kwargs) -> Optional[str]:
+	r"""
+	Create a wx.FileDialog with for the extension and filetypestring given,
+	and return the filename selected.
+
 	:param parent:
-	:type parent:
 	:param extension:
-	:type extension:
 	:param title:
-	:type title:
 	:param filetypestring:
-	:type filetypestring:
 	:param style:
-	:type style:
-	:param kwargs:
-	:type kwargs:
-	
-	:return: The filename selected in the dialog. If wx.FD_MULTIPLE is in the style, this will be the first filename selected.
-	:rtype: str
+	:param \*\*kwargs:
+
+	:return: The filename selected in the dialog.
+		If ``wx.FD_MULTIPLE`` is in the style, this will be the first filename selected.
 	"""
-	
+
 	paths = file_dialog_multiple(*args, **kwargs)
-	
+
 	if paths is not None:
 		return paths[0]
 
+	return None
+
 
 class FloatEntryDialog(wx.TextEntryDialog):
 	"""
 	Alternative to wx.NumberEntryDialog that provides a TextCtrl which only allows numbers and decimal points to be entered.
-	
+
 	Based on http://wxpython-users.1045709.n5.nabble.com/Adding-Validation-to-wx-TextEntryDialog-td2371082.html
 	"""
-	
+
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.textctrl = self.FindWindowById(3000)
-		
+
 		self.textctrl.SetValidator(CharValidator("float-only"))
-	
+
 	def GetValue(self):
 		value = self.textctrl.GetValue()
 		if value == '':
 			return None
 		else:
 			return float(value)
 
 
 class IntEntryDialog(wx.TextEntryDialog):
 	"""
 	Alternative to wx.NumberEntryDialog that provides a TextCtrl which only allows numbers to be entered.
 
 	Based on http://wxpython-users.1045709.n5.nabble.com/Adding-Validation-to-wx-TextEntryDialog-td2371082.html
 	"""
-	
+
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.textctrl = self.FindWindowById(3000)
-		
+
 		self.textctrl.SetValidator(CharValidator("int-only"))
 
 	def GetValue(self):
 		value = self.textctrl.GetValue()
 		if value == '':
 			return None
 		else:
 			return int(value)
 
 
 class Wildcards:
 	"""
 	Class to generate glob wildcards for wx.FileDialog
 	"""
-	
+
 	def __init__(self):
 		self._wildcards = []
-	
+
 	def add_filetype(
-			self, description, extensions=None, hint_format=style_lowercase,
-			value_format=style_lowercase | style_uppercase):
+			self,
+			description: str,
+			extensions: Optional[Sequence[str]] = None,
+			hint_format: int = style_lowercase,
+			value_format: int = style_lowercase | style_uppercase
+			):
 		"""
 		Add a filetype to the wildcards
-		
+
 		:param description: Description of the filetype
-		:type description: str
 		:param extensions: A list of valid file extensions for the filetype
-		:type extensions: list of str
 		:param hint_format: How the hints should be formatted.
-		:type hint_format: int
 		:param value_format: How the values should be formatted.
-		:type value_format:	int
-		
+
 		Valid values for `hint_format` and `value_format` are `style_uppercase`,
 		`style_lowercase` and `style_hidden`, which can be combined using the `|` operator.
 		"""
-		
+
 		if extensions:
 			hint = []
 			value = []
-			
+
 			for extension in extensions:
-				
+
 				if not extension.startswith("*."):
 					extension = f"*.{extension}"
-				
+
 				# Hint
 				if not hint_format & style_hidden:
 					if hint_format & style_lowercase:
 						hint.append(extension.lower())
-						
+
 					if hint_format & style_uppercase:
 						hint.append(extension.upper())
-					
+
 				# Value
 				if value_format & style_lowercase:
 					value.append(extension.lower())
-						
+
 				if value_format & style_uppercase:
 					value.append(extension.upper())
-			
+
 			if hint_format & style_hidden:
 				self._wildcards.append(f"{description}|{';'.join(value)}")
 			else:
 				self._wildcards.append(f"{description} ({';'.join(hint)})|{';'.join(value)}")
-		
+
 		else:
 			self._wildcards.append(f"{description}")
-	
+
 	@property
-	def wildcard(self):
+	def wildcard(self) -> str:
 		"""
 		Returns a string representing the wildcards for use in wx.FileDialog or file_dialog_wildcards
-		
+
 		:rtype: str
 		"""
-		
-		return "|".join(self._wildcards)
-	
+
+		return '|'.join(self._wildcards)
+
 	def add_common_filetype(
-			self, filetype, hint_format=style_lowercase,
-			value_format=style_lowercase | style_uppercase):
+			self,
+			filetype: str,
+			hint_format: int = style_lowercase,
+			value_format: int = style_lowercase | style_uppercase,
+			):
 		"""
 		Add a common filetype.
-		
+
 		:param filetype: The name of the filetype, Possible values are in common_filetypes
-		:type filetype: str
 		:param hint_format: How the hints should be formatted.
-		:type hint_format: int
 		:param value_format: How the values should be formatted.
-		:type value_format:	int
-		
+
 		Valid values for `hint_format` and `value_format` are `style_uppercase`,
 		`style_lowercase` and `style_hidden`, which can be combined using the `|` operator.
 		"""
-		
+
 		self.add_filetype(*common_filetypes[filetype], hint_format=hint_format, value_format=value_format)
 
-	def add_image_wildcard(self, value_format=style_lowercase | style_uppercase):
+	def add_image_wildcard(self, value_format: int = style_lowercase | style_uppercase):
 		"""
 		Add a wildcard for all image filetypes.
 
 		:param value_format: How the values should be formatted.
-		:type value_format:	int
 
 		Valid values for `value_format` are `style_uppercase`,
 		`style_lowercase` and `style_hidden`, which can be combined using the `|` operator.
 		"""
-		
+
 		image_extensions = []
 		for key, item in common_filetypes.items():
 			if key in {"jpeg", "png", "bmp", "tiff", "gif"}:
 				for extension in item[1]:
 					image_extensions.append(f"*.{extension.lower()}")
 					image_extensions.append(f"*.{extension.upper()}")
-				
+
 		self.add_filetype("Image files", image_extensions, hint_format=style_hidden, value_format=value_format)
-	
-	def add_all_files_wildcard(self, hint_format=0):
+
+	def add_all_files_wildcard(self, hint_format: int = 0):
 		"""
 		Add a wildcard for 'All Files'.
 
-		:param hint_format: How the hints should be formatted. Valid values are None and `style_hidden`.
-		:type hint_format: int
+		:param hint_format: How the hints should be formatted. Valid values are :py:obj:`None` and `style_hidden`.
 		"""
-		
+
 		if hint_format & style_hidden:
 			self._wildcards.append("All files|*.*")
 		else:
 			self._wildcards.append("All files (*.*)|*.*")
-	
+
 	def __repr__(self):
 		return f"Wildcard = {self.wildcard}"
-	
+
 	def __str__(self):
 		return self.wildcard
 
 
 # legacy name
-FileDialogWildcards = Wildcards
+FileDialogWildcards = Wildcards
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/projections.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/projections.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  projections.py
 #
 #  Copyright 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Based on https://stackoverflow.com/a/16709952/3092681
 #  Copyright 2013 simonb
@@ -21,48 +20,85 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
-import matplotlib
+# stdlib
+from typing import Optional
+
+# 3rd party
+import matplotlib  # type: ignore
 from matplotlib import axes
 
+__all__ = ["XPanAxes", "XPanAxes_NoZoom", "NoZoom"]
+
 
 class XPanAxes(matplotlib.axes.Axes):
-	"""Constrain pan to x-axis"""
-	
+	"""
+	Constrain pan to x-axis.
+	"""
+
 	name = "XPanAxes"
-	
-	def drag_pan(self, button, key, x, y):
+
+	def drag_pan(self, button, key: Optional[str], x: float, y: float):
+		"""
+
+		:param button: The pressed mouse button.
+		:param key: The pressed key, if any.
+		:param x: The mouse coordinates in display coords.
+		:param y: The mouse coordinates in display coords.
+		"""
+
 		# pretend key=='x'
 		matplotlib.axes.Axes.drag_pan(self, button, 'x', x, y)
 
 
 class XPanAxes_NoZoom(matplotlib.axes.Axes):
-	"""Constrain pan to x-axis and prevent zooming"""
-	
+	"""
+	Constrain pan to x-axis and prevent zooming.
+	"""
+
 	name = "XPanAxes_NoZoom"
-	
-	def drag_pan(self, button, key, x, y):
+
+	def drag_pan(self, button, key: Optional[str], x: float, y: float):
+		"""
+
+		:param button: The pressed mouse button.
+		:param key: The pressed key, if any.
+		:param x: The mouse coordinates in display coords.
+		:param y: The mouse coordinates in display coords.
+		"""
+
 		# pretend key=='x'
 		if button != 1:
 			return
 		matplotlib.axes.Axes.drag_pan(self, button, 'x', x, y)
 
 
 class NoZoom(matplotlib.axes.Axes):
-	"""Prevent zooming in pan mode"""
-	
+	"""
+	Prevent zooming in pan mode.
+	"""
+
 	name = "NoZoom"
-	
-	def drag_pan(self, button, key, x, y):
+
+	def drag_pan(self, button, key: Optional[str], x: float, y: float):
+		"""
+
+		:param button: The pressed mouse button.
+		:param key: The pressed key, if any.
+		:param x: The mouse coordinates in display coords.
+		:param y: The mouse coordinates in display coords.
+		"""
+
 		# pretend key=='x'
 		if button != 1:
 			return
 		matplotlib.axes.Axes.drag_pan(self, button, key, x, y)
 
+
 #
 # matplotlib.projections.register_projection(NoZoom)
 # matplotlib.projections.register_projection(XPanAxes_NoZoom)
 # matplotlib.projections.register_projection(XPanAxes)
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/validators.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  validators.py
 """
 Various validator classes
 """
 #
-#  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright (c) 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -19,154 +18,187 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
+#  Based on the wxPython Demo.
+#  Licenced under the wxWindows Library Licence, Version 3.1
+#
+#  CharValidator based on
+#  http://wxpython-users.1045709.n5.nabble.com/best-way-to-restrict-input-to-integers-td2370605.html
+#
 
 # stdlib
 import string
 
 # 3rd party
-import wx
+import wx  # type: ignore
+
+__all__ = ["ValidatorBase", "CharValidator", "FloatValidator"]
 
 
 class ValidatorBase(wx.Validator):
 	"""
-	Based on the wxPython Demo
-	Licenced under the wxWindows Library Licence, Version 3.1
+	Base class for Validators.
 	"""
-	
+
 	def Clone(self):
 		"""
-		Standard cloner.
-
-		Note that every validator must implement the Clone() method.
+		Clones the :class:`wx.Validator`.
 		"""
+
 		return self.__class__()
-	
-	def TransferToWindow(self):
-		""" Transfer data from validator to window.
 
-			The default implementation returns False, indicating that an error
-			occurred.  We simply return True, as we don't do any data transfer.
+	def TransferToWindow(self) -> bool:
 		"""
+		Transfer data from validator to window.
+
+		The default implementation returns :py:obj:`False`, indicating that an error
+		occurred. We simply return :py:obj:`True`, as we don't do any data transfer.
+		"""
+
 		return True  # Prevent wxDialog from complaining.
-	
-	def TransferFromWindow(self):
-		""" Transfer data from window to validator.
 
-			The default implementation returns False, indicating that an error
-			occurred.  We simply return True, as we don't do any data transfer.
+	def TransferFromWindow(self) -> bool:
+		"""
+		Transfer data from window to validator.
+
+		The default implementation returns :py:obj:`False`, indicating that an error
+		occurred.  We simply return :py:obj:`True`, as we don't do any data transfer.
 		"""
+
 		return True  # Prevent wxDialog from complaining.
-	
-	def set_warning(self):
+
+	def set_warning(self) -> bool:
+		"""
+		Set the control's background colour to pink.
+		"""
+
 		self.GetWindow().SetBackgroundColour("pink")
 		self.GetWindow().SetFocus()
 		self.GetWindow().Refresh()
 		return False
-	
-	def reset_ctrl(self):
-		self.GetWindow().SetBackgroundColour(
-				wx.SystemSettings.GetColour(wx.SYS_COLOUR_WINDOW))
+
+	def reset_ctrl(self) -> bool:
+		"""
+		Resets the control's background colour.
+		"""
+
+		self.GetWindow().SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_WINDOW))
 		self.GetWindow().Refresh()
 		return True
 
 
 class CharValidator(ValidatorBase):
 	"""
 	A Validator that only allows the type of characters selected to be entered.
-	
+
 	The possible flags are:
-		int-only - only the numbers 0123456789 can be entered
-		float-only - only numbers and decimal points can be entered
-	
-	Based on http://wxpython-users.1045709.n5.nabble.com/best-way-to-restrict-input-to-integers-td2370605.html
+
+	* int-only - only the numbers ``0123456789`` can be entered.
+	* float-only - only numbers and decimal points can be entered.
 	"""
-	
+
 	def __init__(self, flag):
 		wx.Validator.__init__(self)
 		self.flag = flag
 		self.Bind(wx.EVT_CHAR, self.OnChar)
-		
+
 		# Special allowed keys, including del, Ctrl+C, Ctrl+X and Ctrl+V
 		self.special_keys = {
 				wx.WXK_BACK,
 				wx.WXK_TAB,
 				wx.WXK_RETURN,
 				wx.WXK_SHIFT,
 				wx.WXK_CONTROL,
 				wx.WXK_ALT,
 				wx.WXK_CONTROL_C,
 				wx.WXK_CONTROL_V,
 				wx.WXK_CONTROL_X,
 				wx.WXK_DELETE,
 				}
-		
+
 	def Clone(self):
 		"""
-		Standard cloner.
-
-		Note that every validator must implement the Clone() method.
+		Clones the :class:`~.CharValidator`.
 		"""
+
 		return self.__class__(self.flag)
-	
-	def Validate(self, win):
+
+	def Validate(self, win) -> bool:
+		"""
+		Validate the control.
+
+		:param win:
+		"""
+
 		return True
-	
-	def OnChar(self, event):
+
+	def OnChar(self, event) -> None:
+		"""
+		Event handler for text being entered in the control.
+
+		:param event: The wxPython event.
+		"""
+
 		keycode = int(event.GetKeyCode())
 		if keycode < 256:
 			key = chr(keycode)
-			
+
 			if keycode in self.special_keys:
 				event.Skip()
 			if self.flag == "int-only":
 				if key not in "0123456789":
 					return
 			elif self.flag == "float-only":
-				if key == "." and "." in event.GetEventObject().GetValue():
+				if key == '.' and '.' in event.GetEventObject().GetValue():
 					return
 				if key not in "0123456789.":
 					return
-			elif self.flag == 'no-alpha' and key in string.ascii_letters:
+			elif self.flag == "no-alpha" and key in string.ascii_letters:
 				return
-			elif self.flag == 'no-digit' and key in string.digits:
+			elif self.flag == "no-digit" and key in string.digits:
 				return
-		
+
 		event.Skip()
 
 
 class FloatValidator(CharValidator):
 	"""
 	A Validator that only allows numbers and decimal points to be entered.
 	If a decimal point has already been entered, a second one cannot be entered.
 	The argument `flag` is used to limit the number of decimal places that can be entered.
 	"""
-	def OnChar(self, event):
-		
+
+	def OnChar(self, event) -> None:
+		"""
+		Event handler for text being entered in the control.
+
+		:param event: The wxPython event.
+		"""
+
 		keycode = int(event.GetKeyCode())
 		if keycode < 256:
 			key = chr(keycode)
 			if keycode in self.special_keys:
 				event.Skip()
-			
+
 			current_value = event.GetEventObject().GetValue()
-			
+
 			if key not in "0123456789.":
 				return
-			
-			if "." in current_value:
-				if key == ".":
-					if "." not in event.GetEventObject().GetStringSelection():
+
+			if '.' in current_value:
+				if key == '.':
+					if '.' not in event.GetEventObject().GetStringSelection():
 						return
-				
+
 				# Current decimal places
-				current_dp = len(current_value.split(".")[1])
-				
+				current_dp = len(current_value.split('.')[1])
+
 				if current_dp == self.flag:
 					# Already at maximum decimal places
 					return
-		
+
 		event.Skip()
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/icons.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/icons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  icons.py
 #
-#  Copyright 2019 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  GetStockBitmap and GetStockToolbarBitmap from
 #  		https://sourceforge.net/p/wxglade/mailman/message/6475744/
 #       Copyright (C) 2005 Antoine Pitrou
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
@@ -21,38 +20,42 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
-import wx
+# 3rd party
+import wx  # type: ignore
+
+__all__ = ["get_toolbar_icon", "get_button_icon", "GetStockBitmap", "GetStockToolbarBitmap"]
 
 
 def get_toolbar_icon(icon_name, size=24):
+
 	return wx.Bitmap(wx.ArtProvider.GetBitmap(f"wx{icon_name}", "wxART_TOOLBAR_C", wx.Size(size, size)))
 
 
 def get_button_icon(icon_name, size=24):
 	return wx.Bitmap(wx.ArtProvider.GetBitmap(f"wx{icon_name}", "wxART_BUTTON_C", wx.Size(size, size)))
 
+
 # The following code (C) 2005 Antoine Pitrou
 # https://sourceforge.net/p/wxglade/mailman/message/6475744/
 _art_provider = None
 
 
 def GetStockBitmap(art_id, art_client=None):
 	"""
 	Get a stock bitmap from its wx.ART_xxx ID
 	"""
 	global _art_provider
 	if _art_provider is None:
 		_art_provider = wx.ArtProvider()
-	return _art_provider.GetBitmap(id=art_id,
-								   client=art_client or wx.ART_OTHER)
+	return _art_provider.GetBitmap(id=art_id, client=art_client or wx.ART_OTHER)
 
 
 def GetStockToolbarBitmap(art_id):
 	return GetStockBitmap(art_id, wx.ART_TOOLBAR)
 
 
 TB = GetStockToolbarBitmap
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/StylePickerPanel.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/ColourPickerPanel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
+
 #
-#  StylePickerPanel.py
+#  ColourPickerPanel.py
+"""
+Based on StylePickerPanel, a Panel for selecting a list of colours, and their order
+"""
 #
-#  Copyright 2019 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -21,154 +24,175 @@
 #  MA 02110-1301, USA.
 #
 #
 # generated by wxGlade 0.9.3 on Tue Apr  9 18:07:58 2019
 #
 
 # stdlib
-import sys
+from typing import List, Optional
 
 # 3rd party
-import wx
-from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg as FigureCanvas
-from matplotlib.figure import Figure
+import matplotlib  # type: ignore
+import wx  # type: ignore
+from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg as FigureCanvas  # type: ignore
+from matplotlib.figure import Figure  # type: ignore
+
+# this package
+from domdf_wxpython_tools.StylePickerPanel import StylePickerPanel
+
+__all__ = ["ColourPickerPanel"]
 
 # begin wxGlade: dependencies
 # end wxGlade
 
 # begin wxGlade: extracode
 # end wxGlade
 
+default_colours = [
+		"#1f77b4",
+		"#ff7f0e",
+		"#2ca02c",
+		"#d62728",
+		"#9467bd",
+		"#8c564b",
+		"#e377c2",
+		"#7f7f7f",
+		"#bcbd22",
+		"#17becf",
+		]
+
+default_picker_choices = [
+		"#000000",
+		"#ff0000",
+		"#ffa500",
+		"#00ff00",
+		"#0000ff",
+		"#551a8b",
+		"#008080",
+		]
+
+
+class ColourPickerPanel(StylePickerPanel):
+	"""
+	Based on StylePickerPanel, a Panel for selecting a list of colours, and their order.
+
+	:param parent: The parent window.
+	:param id: An identifier for the panel. wx.ID_ANY is taken to mean a default.
+	:param pos: The panel position. The value ``wx.DefaultPosition`` indicates a default position, chosen by either the windowing system or wxWidgets, depending on platform.
+	:param size: The panel size. The value ``wx.DefaultSize`` indicates a default size, chosen by either the windowing system or wxWidgets, depending on platform.
+	:param style: The window style. See wxPanel.
+	:param name: The window name.
+	:param label: Label for the panel
+	:param picker_choices: A list of hex value choices to populate the 'picker' side of the panel with
+	:param selection_choices: A list of hex value choices to populate the 'selection' side of the panel with
+	"""
 
-default_styles = ["o", "v", "^", "<", ">", "s", "h", "X", "D", "d"]
-
-
-class StylePickerPanel(wx.Panel):
 	def __init__(
-			self, parent, id=wx.ID_ANY, pos=wx.DefaultPosition, size=wx.DefaultSize,
-			style=wx.TAB_TRAVERSAL, name=wx.PanelNameStr, label="Choose Styles: ",
-			selection_choices=None,
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = wx.TAB_TRAVERSAL,
+			name: str = wx.PanelNameStr,
+			label: str = "Choose Colours: ",
+			picker_choices: Optional[List[str]] = None,
+			selection_choices: Optional[List[str]] = None,
 			):
+
+		args = (parent, id, pos, size)
+		kwds = {"style": style, "name": name}
+
+		if picker_choices is None:
+			picker_choices = default_picker_choices
+
 		if selection_choices is None:
-			selection_choices = default_styles[:]
+			selection_choices = default_colours[:]
+
 		self.label = label
+		self.picker_choices = picker_choices
 		self.selection_choices = selection_choices
 
-		args = (parent, id, pos, size)
-		kwds = {"style": style, "name": name}
-		
-		# begin wxGlade: StylePickerPanel.__init__
+		# begin wxGlade: ColourPickerPanel.__init__
 		kwds["style"] = kwds.get("style", 0) | wx.TAB_TRAVERSAL
 		wx.Panel.__init__(self, *args, **kwds)
 		self.main_panel = wx.Panel(self, wx.ID_ANY)
 		self.move_panel = wx.Panel(self.main_panel, wx.ID_ANY)
 		self.picker_list_box = wx.ListBox(self.main_panel, wx.ID_ANY, choices=[])
-		
+
 		self.picker_figure = Figure()
-		
+
 		self.picker_canvas = FigureCanvas(self.main_panel, wx.ID_ANY, self.picker_figure)
-		self.add_btn = wx.Button(self.main_panel, wx.ID_ANY, u"Add 🡲")
-		self.remove_btn = wx.Button(self.main_panel, wx.ID_ANY, u"🡰 Remove")
+		self.add_btn = wx.Button(self.main_panel, wx.ID_ANY, "Add 🡲")
+		self.remove_btn = wx.Button(self.main_panel, wx.ID_ANY, "🡰 Remove")
 		self.selection_list_box = wx.ListBox(self.main_panel, wx.ID_ANY, choices=[])
-		self.up_btn = wx.Button(self.main_panel, wx.ID_ANY, u"🡱 Up")
-		self.down_btn = wx.Button(self.main_panel, wx.ID_ANY, u"🡳 Down")
-		
+		self.up_btn = wx.Button(self.main_panel, wx.ID_ANY, "🡱 Up")
+		self.down_btn = wx.Button(self.main_panel, wx.ID_ANY, "🡳 Down")
+
 		self.selection_figure = Figure()
-		
+
 		self.selection_canvas = FigureCanvas(self.main_panel, wx.ID_ANY, self.selection_figure)
 
 		self.__set_properties()
 		self.__do_layout()
-
+		# end wxGlade
 		self.Bind(wx.EVT_LISTBOX, self.update_picker_preview, self.picker_list_box)
 		self.Bind(wx.EVT_LISTBOX_DCLICK, self.add, self.picker_list_box)
 		self.Bind(wx.EVT_BUTTON, self.add, self.add_btn)
 		self.Bind(wx.EVT_BUTTON, self.remove, self.remove_btn)
 		self.Bind(wx.EVT_LISTBOX, self.update_selection_preview, self.selection_list_box)
 		self.Bind(wx.EVT_BUTTON, self.move_up, self.up_btn)
 		self.Bind(wx.EVT_BUTTON, self.move_down, self.down_btn)
-		# end wxGlade
-	
+
 		self.Bind(wx.EVT_LISTBOX_DCLICK, self.remove, self.selection_list_box)
-		
-		self.markers = {
-				"point": ".",
-				"pixel": ",",
-				"circle": "o",
-				"triangle_down": "v",
-				"triangle_up": "^",
-				"triangle_left": "<",
-				"triangle_right": ">",
-				"tri_down": "1",
-				"tri_up": "2",
-				"tri_left": "3",
-				"tri_right": "4",
-				"octagon": "8",
-				"square": "s",
-				"pentagon": "p",
-				"plus (filled)": "P",
-				"star": "*",
-				"hexagon1": "h",
-				"hexagon2": "H",
-				"plus": "+",
-				"x": "x",
-				"x (filled)": "X",
-				"diamond": "D",
-				"thin_diamond": "d",
-				"caretleft": 4,  # (CARETLEFT),
-				"caretright": 5,  # (CARETRIGHT),
-				"caretup": 6,  # (CARETUP),
-				"caretdown": 7,  # (CARETDOWN),
-				}
-		
-		for marker in self.selection_choices:
-			for key in self.markers.keys():
-				if marker == self.markers[key]:
-					self.selection_list_box.Append(key)
+
+		self.remove_btn.SetLabel("Remove")
+
+		self.selection_list_box.Clear()
+		self.selection_list_box.AppendItems(self.selection_choices)
 		if not self.selection_list_box.IsEmpty():
 			self.selection_list_box.SetSelection(0)
-		
-		for marker in list(filter(lambda x: x not in self.selection_choices, [self.markers[y] for y in self.markers])):
-			for key in self.markers.keys():
-				if marker == self.markers[key]:
-					self.picker_list_box.Append(key)
-		self.picker_list_box.SetSelection(0)
-		
+
+		self.picker_list_box.Clear()
+		self.picker_list_box.AppendItems(self.picker_choices)
+		if not self.picker_list_box.IsEmpty():
+			self.picker_list_box.SetSelection(0)
+
 		self.picker_axes = self.picker_figure.add_subplot(111)
 		self.selection_axes = self.selection_figure.add_subplot(111)
 		self.update_picker_preview()
 		self.update_selection_preview()
 
 	def __set_properties(self):
-		# begin wxGlade: StylePickerPanel.__set_properties
+		# begin wxGlade: ColourPickerPanel.__set_properties
 		self.move_panel.SetMinSize((170, -1))
 		self.picker_list_box.SetMinSize((170, 256))
 		self.picker_canvas.SetMinSize((64, 64))
 		self.selection_list_box.SetMinSize((170, 256))
 		self.up_btn.SetMinSize((80, -1))
 		self.down_btn.SetMinSize((80, -1))
 		self.selection_canvas.SetMinSize((64, 64))
 		self.main_panel.SetMinSize((450, -1))
 		# end wxGlade
 
 	def __do_layout(self):
-		# begin wxGlade: StylePickerPanel.__do_layout
+		# begin wxGlade: ColourPickerPanel.__do_layout
 		parent_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		main_sizer = wx.BoxSizer(wx.VERTICAL)
 		list_grid_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		sizer_4 = wx.BoxSizer(wx.VERTICAL)
 		selection_preview_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		move_grid = wx.GridSizer(1, 2, 0, 5)
 		sizer_3 = wx.BoxSizer(wx.VERTICAL)
 		sizer_2 = wx.BoxSizer(wx.VERTICAL)
 		picker_preview_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		grid_sizer = wx.GridSizer(1, 3, 10, 10)
 		borders_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Choose Styles: ")
 		borders_label.SetMinSize((128, 20))
-		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ""))
+		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ''))
 		grid_sizer.Add(borders_label, 0, wx.BOTTOM, 7)
 		grid_sizer.Add(self.move_panel, 1, wx.ALIGN_CENTER | wx.EXPAND, 0)
 		main_sizer.Add(grid_sizer, 0, 0, 0)
 		sizer_2.Add(self.picker_list_box, 5, wx.EXPAND, 0)
 		sizer_2.Add((0, 0), 0, 0, 0)
 		preview_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Preview: ")
 		picker_preview_sizer.Add(preview_label, 0, 0, 0)
@@ -193,90 +217,102 @@
 		self.main_panel.SetSizer(main_sizer)
 		parent_sizer.Add(self.main_panel, 0, wx.ALL, 10)
 		self.SetSizer(parent_sizer)
 		parent_sizer.Fit(self)
 		self.Layout()
 		# end wxGlade
 		borders_label.SetLabel(self.label)
-	
-	def move_up(self, event):  # wxGlade: StylePickerPanel.<event_handler>
-		self.move(-1)
-		event.Skip()
-	
-	def move_down(self, event):  # wxGlade: StylePickerPanel.<event_handler>
-		self.move(1)
-		event.Skip()
-	
-	def move(self, direction=1):
-		selection = self.selection_list_box.GetSelection()
-		selection_string = self.selection_list_box.GetString(selection)
-		if self.selection_list_box.GetCount() == selection + direction or selection + direction < 0:
-			return
-		
-		self.selection_list_box.Delete(selection)
-		self.selection_list_box.InsertItems([selection_string], selection + direction)
-		self.selection_list_box.SetSelection(selection + direction)
-	
-	def add(self, event):  # wxGlade: StylePickerPanel.<event_handler>
+
+	def add(self, event):  # wxGlade: ColourPickerPanel.<event_handler>
+		"""
+		Event handler for adding the colour currently selected in the 'picker' to the 'selection'
+		"""
+
 		selection = self.picker_list_box.GetSelection()
 		if selection == -1:
 			return
-		
+
 		selection_string = self.picker_list_box.GetString(selection)
 		if selection_string == '':
 			return
-		
+
 		self.selection_list_box.Append(selection_string)
-		self.picker_list_box.Delete(selection)
-		
+
 		self.update_picker_preview()
+
+		self.selection_list_box.SetSelection(self.selection_list_box.GetCount() - 1)
+		self.update_selection_preview()
 		event.Skip()
-	
-	def remove(self, event):  # wxGlade: StylePickerPanel.<event_handler>
+
+	def remove(self, event):  # wxGlade: ColourPickerPanel.<event_handler>
+		"""
+		Event handler for removing the colour currently selected in the 'selection'
+		"""
+
 		selection = self.selection_list_box.GetSelection()
 		if selection == -1:
 			return
-		
+
 		selection_string = self.selection_list_box.GetString(selection)
 		if selection_string == '':
 			return
-		
-		self.picker_list_box.Append(selection_string)
+
 		self.selection_list_box.Delete(self.selection_list_box.GetSelection())
-		
+
 		self.update_selection_preview()
 		event.Skip()
-	
-	def update_picker_preview(self, *_):  # wxGlade: StylePickerPanel.<event_handler>
-		self.update_preview(self.picker_list_box, self.picker_axes)
-		self.picker_canvas.draw_idle()
-	
-	def update_selection_preview(self, *_):  # wxGlade: StylePickerPanel.<event_handler>
-		self.update_preview(self.selection_list_box, self.selection_axes)
-		self.selection_canvas.draw_idle()
-	
-	def update_preview(self, list_obj, axes):
+
+	def update_preview(self, list_obj: wx.ListBox, axes: matplotlib.axes.Axes):
+		"""
+		Update the preview from the given list.
+
+		:param list_obj: The list to update the preview for.
+		:param axes: The preview axes to update.
+		"""
+
 		axes.clear()
-		axes.axis('off')
+		axes.axis("off")
 		selection_string = list_obj.GetStringSelection()
 		if selection_string == '':
 			return
-		
-		axes.scatter(1, 1, s=200, color="red", marker=self.markers[selection_string])
-	
-	do_layout = __do_layout
-	set_properties = __set_properties
-	
-	def get_selection(self):
-		return [
-				self.markers[
-					self.selection_list_box.GetString(item)
-					] for item in range(self.selection_list_box.GetCount())
-				]
-	
-	def _do_layout(self):
-		return self.__do_layout()
-	
-	def _set_properties(self):
-		return self.__set_properties()
 
-# end of class StylePickerPanel
+		axes.scatter(1, 1, s=400, color=selection_string, marker='s')
+
+	def pick(self, *args):
+		"""
+		Open a :py:class:`wx.ColourDialog` to edit the colour currently selected in the picker.
+		"""
+
+		selection = self.selection_list_box.GetSelection()
+		if selection == -1:
+			return
+
+		selection_string = self.selection_list_box.GetString(selection)
+		if selection_string == '':
+			return
+
+		colour = wx.ColourData()
+		colour.SetColour(selection_string)
+
+		dlg = wx.ColourDialog(self, data=colour)
+
+		res = dlg.ShowModal()
+		if res == wx.ID_OK:
+			self.selection_list_box.Delete(selection)
+			self.selection_list_box.InsertItems(
+				[dlg.GetColourData().GetColour().GetAsString(wx.C2S_HTML_SYNTAX)],
+				selection)  # yapf: disable
+			self.selection_list_box.SetSelection(selection)
+			self.update_selection_preview()
+			dlg.Destroy()
+
+	def GetSelection(self) -> List[str]:
+		"""
+		Returns a list of the currently selected colours
+		"""
+
+		return [self.selection_list_box.GetString(item) for item in range(self.selection_list_box.GetCount())]
+
+	get_selection = GetSelection
+
+
+# end of class ColourPickerPanel
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/logctrl.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/logctrl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python
-#   -*- coding: utf-8 -*-
 #
 #  logctrl.py
 """
 Log Control, supporting text copying and zoom.
 """
 #
-#  Copyright (c) 2019 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright (c) 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #  Based on PyCrust by Patrick K. O'Brien <pobrien@orbtech.com>
 #   and https://wiki.wxpython.org/StyledTextCtrl%20Log%20Window%20Demo
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -23,154 +22,158 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 #
 
-
 # stdlib
 import keyword
 import os
+import time
+from typing import List, Optional
 
 # 3rd party
-import wx
+import wx  # type: ignore
 from wx import stc
 
 # this package
-from domdf_wxpython_tools.utils import generate_faces
 from domdf_wxpython_tools.keyboard import gen_keymap
+from domdf_wxpython_tools.utils import generate_faces
 
+__all__ = ["LogCtrl"]
 
 # IDs
 ID_WRAP = wx.NewIdRef()
 ID_SHOW_LINENUMBERS = wx.NewIdRef()
 ID_ZOOM_IN = wx.NewIdRef()
 ID_ZOOM_OUT = wx.NewIdRef()
 ID_ZOOM_DEFAULT = wx.NewIdRef()
 ID_ZOOM_SET = wx.NewIdRef()
 
-
 # Key bindings:
 # Home              Go to the beginning of the line.
 # Shift+Home        Select to the beginning of the command or line.
 # Shift+End         Select to the end of the line.
 # End               Go to the end of the line.
 # Ctrl+C            Copy selected text
 # Ctrl+]            Increase font size.
 # Ctrl+[            Decrease font size.
 # Ctrl+=            Default font size.
 # Ctrl+F            Search
 # TODO: F3                Search next
-#
+
 
 class LogCtrl(stc.StyledTextCtrl):
 	"""
 	Log Window based on StyledTextCtrl.
+
+	:param parent: The parent window.
+	:param id: An identifier for the Log window. wx.ID_ANY is taken to mean a default.
+	:param pos: The Log window position. The value ``wx.DefaultPosition`` indicates a default position, chosen by either the windowing system or wxWidgets, depending on platform.
+	:param size: The Log window size. The value ::wxDefaultSize indicates a default size, chosen by either the windowing system or wxWidgets, depending on platform.
+	:param style: The window style. See wxPanel.
+	:param name: Window name.
 	"""
-	
+
+	findDlg: Optional[wx.FindReplaceDialog]
+
 	def __init__(
-			self, parent, id=wx.ID_ANY, pos=wx.DefaultPosition, size=wx.DefaultSize,
-			style=wx.CLIP_CHILDREN | wx.SUNKEN_BORDER, name="Log"
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = wx.CLIP_CHILDREN | wx.SUNKEN_BORDER,
+			name: str = "Log"
 			):
-		"""
-		:param parent: The parent window.
-		:type parent: wx.Window
-		:param id: An identifier for the Log window. wx.ID_ANY is taken to mean a default.
-		:type id: wx.WindowID, optional
-		:param pos: The Log window position. The value ::wxDefaultPosition indicates a default position, chosen by either the windowing system or wxWidgets, depending on platform.
-		:type pos: wx.Point, optional
-		:param size: The Log window size. The value ::wxDefaultSize indicates a default size, chosen by either the windowing system or wxWidgets, depending on platform.
-		:type size: wx.Size, optional
-		:param style: The window style. See wxPanel.
-		:type style: int, optional
-		:param name: Window name.
-		:type name: str, optional
-		"""
-		
+
 		stc.StyledTextCtrl.__init__(self, parent, id, pos, size, style, name)
-		
+
 		self._FACES = generate_faces()
 		self._keyMap = gen_keymap()
 		self._config()
 		self.default_zoom = self.GetZoom()
-		self._styles = [None] * 32
+		self._styles: List[Optional[str]] = [None] * 32
 		self._free = 1
-		
+
 		# dispatcher.connect(receiver=self._fontsizer, signal='FontIncrease')
 		# dispatcher.connect(receiver=self._fontsizer, signal='FontDecrease')
 		# dispatcher.connect(receiver=self._fontsizer, signal='FontDefault')
-		
+
 		self.findDlg = None
 		self.findData = wx.FindReplaceData()
 		self.findData.SetFlags(wx.FR_DOWN)
-		
+
 		self.Bind(wx.EVT_CONTEXT_MENU, self.OnContextMenu)
 		self.Bind(wx.EVT_FIND_CLOSE, self.OnFindClose)
 		self.Bind(wx.EVT_KEY_DOWN, self.onKeyPress)
 		self.Bind(wx.EVT_MENU, lambda event: self.Copy(), id=wx.ID_COPY)
 		self.Bind(wx.EVT_MENU, lambda event: self.SelectAll(), id=wx.ID_SELECTALL)
 		self.Bind(wx.EVT_MENU, self.OnFindText, id=wx.ID_FIND)
-		#self.Bind(wx.EVT_MENU, self.OnWrap, id=ID_WRAP)
+		# self.Bind(wx.EVT_MENU, self.OnWrap, id=ID_WRAP)
 		self.Bind(wx.EVT_MENU, self.ToggleWrap, id=ID_WRAP)
-		#self.Bind(wx.EVT_MENU, self.OnShowLineNumbers, id=ID_SHOW_LINENUMBERS)
+		# self.Bind(wx.EVT_MENU, self.OnShowLineNumbers, id=ID_SHOW_LINENUMBERS)
 		self.Bind(wx.EVT_MENU, self.ToggleLineNumbers, id=ID_SHOW_LINENUMBERS)
 		self.Bind(wx.EVT_MENU, self.OnZoomIn, id=ID_ZOOM_IN)
 		self.Bind(wx.EVT_MENU, self.OnZoomOut, id=ID_ZOOM_OUT)
 		self.Bind(wx.EVT_MENU, self.OnZoomDefault, id=ID_ZOOM_DEFAULT)
 		# TODO: Default Zoom and Set Zoom
-		
+
 		# Display the introductory banner information.
 		self.AppendText('''Click "▶ Run Comparison" to start
-		
+
 Right click for options
 ''')
 		# TODO: Make this not specific to GSMatch
-		
+
 		wx.CallAfter(self.ScrollToLine, 0)
-	
+
 	def _config(self):
 		self.wrap()
 		self.setDisplayLineNumbers(False)
-		
+
 		self.SetLexer(stc.STC_LEX_PYTHON)
 		self.SetKeyWords(0, ' '.join(keyword.kwlist))
-		
+
 		self.setStyles(self._FACES)
 		self.SetViewWhiteSpace(False)
 		self.SetWrapMode(True)
 		try:
 			self.SetEndAtLastLine(False)
 		except AttributeError:
 			pass
-		
+
 		self.SetMargins(5, 5)
-	
+
 	def onKeyPress(self, event):
-		"""Event Handler for key being pressed"""
+		"""
+		Event Handler for key being pressed.
+		"""
+
 		keycode = event.GetKeyCode()
 		keyname = self._keyMap.get(keycode, None)
-		modifiers = ""
+		modifiers = ''
 		for mod, ch in (
-				(event.ControlDown(), 'Ctrl+'),
-				(event.AltDown(), 'Alt+'),
-				(event.ShiftDown(), 'Shift+'),
-				(event.MetaDown(), 'Meta+')
-				):
+			(event.ControlDown(), "Ctrl+"),
+			(event.AltDown(), "Alt+"),
+			(event.ShiftDown(), "Shift+"),
+			(event.MetaDown(), "Meta+"),
+			):
 			if mod:
 				modifiers += ch
-		
+
 		if keyname is None:
 			if 27 < keycode < 256:
 				keyname = chr(keycode)
 			else:
 				keyname = "(%s)unknown" % keycode
-		
+
 		combination = modifiers + keyname
-		
+
 		commands = {
 				"Ctrl+A": self.SelectAll,
 				"Ctrl+C": self.Copy,
 				"Ctrl+F": self.OnFindText,
 				"UP": self.LineUp,
 				"DOWN": self.LineDown,
 				"RIGHT": self.CharRight,
@@ -188,391 +191,379 @@
 				"Shift+LEFT": self.CharLeftExtend,
 				"Shift+RIGHT": self.CharRightExtend,
 				"Shift+UP": self.LineUpExtend,
 				"Shift+DOWN": self.LineDownExtend,
 				"Ctrl+Shift+LEFT": self.WordLeftExtend,
 				"Ctrl+Shift+RIGHT": self.WordRightExtend,
 				"Ctrl+]": self.ZoomIn,
-				"Ctrl+[": self.ZoomOut,
-				# "ESCAPE": here we should remove focus from the widget,
+				"Ctrl+[": self.ZoomOut,  # "ESCAPE": here we should remove focus from the widget,
 				"Ctrl+W": self.ToggleWrap,
 				"Ctrl+L": self.ToggleLineNumbers,
 				}
-		
+
 		if combination in commands:
 			commands[combination]()
 		elif combination == "Ctrl+=":
 			self.SetZoom(self.default_zoom)
-		
+
 		print(combination)
-	
+
 	def fixLineEndings(self, text):
 		"""
 		Return text with line endings replaced by OS-specific endings.
 
 		:param text:
-		:type text:
-
-		:return:
-		:rtype:
 		"""
-		
+
 		lines = text.split('\r\n')
-		for l in range(len(lines)):
-			chunks = lines[l].split('\r')
-			for c in range(len(chunks)):
-				chunks[c] = os.linesep.join(chunks[c].split('\n'))
-			lines[l] = os.linesep.join(chunks)
+		for idx, line in enumerate(lines):
+			chunks = line.split('\r')
+			for idx, chunk in enumerate(chunks):
+				chunks[idx] = os.linesep.join(chunk.split('\n'))
+			lines[idx] = os.linesep.join(chunks)
 		text = os.linesep.join(lines)
 		return text
-	
+
 	def setStyles(self, faces):
 		"""
 		Configure font size, typeface and color for lexer.
-		
+
 		:param faces:
-		:type faces:
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		# Default style
-		self.StyleSetSpec(
-				stc.STC_STYLE_DEFAULT,
-				"face:{mono},size:{size:d},back:{backcol}".format(**faces)
-				)
-		
+		self.StyleSetSpec(stc.STC_STYLE_DEFAULT, "face:{mono},size:{size:d},back:{backcol}".format(**faces))
+
 		self.StyleClearAll()
 		self.SetSelForeground(True, wx.SystemSettings.GetColour(wx.SYS_COLOUR_HIGHLIGHTTEXT))
 		self.SetSelBackground(True, wx.SystemSettings.GetColour(wx.SYS_COLOUR_HIGHLIGHT))
-		
+
 		styles = [  # Built in styles
 			(stc.STC_STYLE_LINENUMBER, f"back:#C0C0C0,face:{faces}(mono)s,size:{faces}(lnsize)d"),
 			(stc.STC_STYLE_CONTROLCHAR, f"face:{faces}(mono)s"),
 			(stc.STC_STYLE_BRACELIGHT, "fore:#0000FF,back:#FFFF88"),
 			(stc.STC_STYLE_BRACEBAD, "fore:#FF0000,back:#FFFF88"),
 			# Python styles
 			(stc.STC_P_DEFAULT, f"face:{faces}(mono)s"),
 			(stc.STC_P_COMMENTLINE, f"fore:#007F00,face:{faces}(mono)s"),
-			(stc.STC_P_NUMBER, ""),
+			(stc.STC_P_NUMBER, ''),
 			(stc.STC_P_STRING, f"fore:#7F007F,face:{faces}(mono)s"),
 			(stc.STC_P_CHARACTER, f"fore:#7F007F,face:{faces}(mono)s"),
 			# (stc.STC_P_WORD, "fore:#00007F,bold"),
 			(stc.STC_P_TRIPLE, "fore:#7F0000"),
 			(stc.STC_P_TRIPLEDOUBLE, "fore:#000033,back:#FFFFE8"),
 			# (stc.STC_P_CLASSNAME, "fore:#0000FF,bold"),
 			# (stc.STC_P_DEFNAME, "fore:#007F7F,bold"),
-			(stc.STC_P_OPERATOR, ""),
-			(stc.STC_P_IDENTIFIER, ""),
+			(stc.STC_P_OPERATOR, ''),
+			(stc.STC_P_IDENTIFIER, ''),
 			(stc.STC_P_COMMENTBLOCK, "fore:#7F7F7F"),
 			(stc.STC_P_STRINGEOL, f"fore:#000000,face:{faces}(mono)s,back:#E0C0E0,eolfilled"),
 			]
-		
+
 		for style in styles:
 			self.StyleSetSpec(*style)
-	
-	def getStyle(self, c='black'):
+
+	def getStyle(self, c: str = "black"):
 		"""
-		Returns a style for a given colour if one exists.  If no style
-		exists for the colour, make a new style.
+		Returns a style for a given colour if one exists.
+
+		If no style exists for the colour, make a new style.
 
-		If we run out of styles, (only 32 allowed here) we go to the top
-		of the list and reuse previous styles.
+		If we run out of styles, (only 32 allowed here) we go to the top of the list and reuse previous styles.
 
+		:param c:
 		"""
+
 		free = self._free
 		if c and isinstance(c, str):
 			c = c.lower()
 		else:
-			c = 'black'
-		
+			c = "black"
+
 		try:
 			style = self._styles.index(c)
 			return style
-		
+
 		except ValueError:
 			style = free
 			self._styles[style] = c
 			self.StyleSetForeground(style, wx.NamedColour(c))
-			
+
 			free += 1
 			if free > 31:
 				free = 0
 			self._free = free
 			return style
 
-	def OnZoomIn(self, *args):
-		"""Event Handler for zooming in"""
+	def OnZoomIn(self, *_):
+		"""
+		Event Handler for zooming in
+		"""
+
 		self.ZoomIn()
-	
-	def OnZoomOut(self, *args):
-		"""Event Handler for zooming out"""
+
+	def OnZoomOut(self, *_):
+		"""
+		Event Handler for zooming out
+		"""
+
 		self.ZoomOut()
-	
-	def OnZoomDefault(self, *args):
-		"""Event Handler for resetting the zoom"""
+
+	def OnZoomDefault(self, *_):
+		"""
+		Event Handler for resetting the zoom
+		"""
+
 		self.SetZoom(self.default_zoom)
 
 	def setDisplayLineNumbers(self, state):
 		self.lineNumbers = state
 		if state:
 			self.SetMarginType(1, stc.STC_MARGIN_NUMBER)
 			self.SetMarginWidth(1, 40)
 		else:
 			# Leave a small margin so the feature hidden lines marker can be seen
 			self.SetMarginType(1, 0)
 			self.SetMarginWidth(1, 10)
-	
+
 	# def OnShowLineNumbers(self, event):
 	# 	print("sln")
 	# 	if hasattr(self, 'lineNumbers'):
 	# 		self.lineNumbers = event.IsChecked()
 	# 		self.setDisplayLineNumbers(self.lineNumbers)
-	
-	def ToggleLineNumbers(self, *args):
+
+	def ToggleLineNumbers(self, *_):
 		self.setDisplayLineNumbers(not self.lineNumbers)
 
-	def CanCopy(self):
+	def CanCopy(self) -> bool:
 		"""
-		Returns True if text is selected and can be copied, False otherwise.
-		
+		Returns :py:obj:`True` if text is selected and can be copied, :py:obj:`False` otherwise.
+
 		:rtype: bool
 		"""
 		return self.GetSelectionStart() != self.GetSelectionEnd()
 
 	def Copy(self):
 		"""
 		Copy the selection and place it on the clipboard.
 		"""
-		
+
 		if self.CanCopy():
 			command = self.GetSelectedText()
 			data = wx.TextDataObject(command)
 			self._clip(data)
 
-	def _clip(self, data):
+	@staticmethod
+	def _clip(data):
 		"""
 		Internal function for copying to clipboard
 		"""
-		
+
 		if wx.TheClipboard.Open():
 			wx.TheClipboard.UsePrimarySelection(False)
 			wx.TheClipboard.SetData(data)
 			wx.TheClipboard.Flush()
 			wx.TheClipboard.Close()
 
-	def wrap(self, wrap=True):
+	def wrap(self, wrap: bool = True):
 		"""
 		Set whether text is word wrapped.
-		
+
 		:param wrap: Whether the text should be word wrapped
-		:type wrap: bool
 		"""
-		
+
 		try:
 			self.SetWrapMode(wrap)
 		except AttributeError:
-			return 'Wrapping is not available in this version.'
+			return "Wrapping is not available in this version."
+
 	#
 	# def OnWrap(self, event):
 	# 	self.SetWrapMode(event.IsChecked())
-	
-	def ToggleWrap(self, *args):
+
+	def ToggleWrap(self, *_) -> None:
 		"""
-		Toggle word wrap
+		Toggle word wrap.
 		"""
-		
+
 		self.SetWrapMode(not self.GetWrapMode())
-	
+
 	def GetContextMenu(self):
 		"""
 		Create and return a context menu for the log.
 		This is used instead of the scintilla default menu
 		in order to correctly respect our immutable buffer.
 		"""
-		
+
 		menu = wx.Menu()
 		menu.Append(wx.ID_COPY, "&Copy")
 		menu.Append(wx.ID_SELECTALL, "Select &All \tCtrl+A")
 		menu.AppendSeparator()
-		menu.Append(
-				wx.ID_FIND, '&Find \tCtrl+F',
-				'Search for text in the log'
-				)
-		menu.Append(
-				ID_WRAP, '&Wrap Lines\tCtrl+W',
-				'Wrap lines at right edge', wx.ITEM_CHECK
-				)
-		menu.Append(
-				ID_SHOW_LINENUMBERS, '&Show Line Numbers\tCtrl+L',
-				'Show Line Numbers', wx.ITEM_CHECK
-				)
+		menu.Append(wx.ID_FIND, "&Find \tCtrl+F", "Search for text in the log")
+		menu.Append(ID_WRAP, "&Wrap Lines\tCtrl+W", "Wrap lines at right edge", wx.ITEM_CHECK)
+		menu.Append(ID_SHOW_LINENUMBERS, "&Show Line Numbers\tCtrl+L", "Show Line Numbers", wx.ITEM_CHECK)
 		menu.AppendSeparator()
-		menu.Append(ID_ZOOM_IN, 'Zoom &In\tCtrl+]', 'Zoom In')
-		menu.Append(ID_ZOOM_OUT, 'Zoom &Out\tCtrl+[', 'Zoom Out')
-		menu.Append(ID_ZOOM_DEFAULT, '&Reset Zoom\tCtrl+=', 'Zoom Out')
-		menu.Append(ID_ZOOM_SET, 'Set &Zoom', 'Zoom Out')
-		
+		menu.Append(ID_ZOOM_IN, "Zoom &In\tCtrl+]", "Zoom In")
+		menu.Append(ID_ZOOM_OUT, "Zoom &Out\tCtrl+[", "Zoom Out")
+		menu.Append(ID_ZOOM_DEFAULT, "&Reset Zoom\tCtrl+=", "Zoom Out")
+		menu.Append(ID_ZOOM_SET, "Set &Zoom", "Zoom Out")
+
 		menu.Check(ID_WRAP, self.GetWrapMode())
 		menu.Check(ID_SHOW_LINENUMBERS, self.lineNumbers)
-		
+
 		return menu
-	
-	def OnContextMenu(self, event):
-		"""Event Handler for showing the context menu"""
+
+	def OnContextMenu(self, _):
+		"""
+		vent Handler for showing the context menu
+		"""
+
 		menu = self.GetContextMenu()
 		self.PopupMenu(menu)
 
-
 	# Find Dialog Methods
+
 	def GetLastPosition(self):
 		return self.GetLength()
-	
+
 	def GetRange(self, start, end):
 		return self.GetTextRange(start, end)
-	
+
 	def GetSelection(self):
 		return self.GetAnchor(), self.GetCurrentPos()
-	
+
 	def ShowPosition(self, pos):
 		line = self.LineFromPosition(pos)
 		# self.EnsureVisible(line)
 		self.GotoLine(line)
-	
+
 	def DoFindNext(self, findData, findDlg=None):
 		backward = not (findData.GetFlags() & wx.FR_DOWN)
 		matchcase = (findData.GetFlags() & wx.FR_MATCHCASE) != 0
 		end = self.GetLength()
 		# Changed to reflect the fact that StyledTextControl is in UTF-8 encoding
-		textstring = self.GetTextRange(0, end).encode('utf-8')
-		findstring = findData.GetFindString().encode('utf-8')
+		textstring = self.GetTextRange(0, end).encode("utf-8")
+		findstring = findData.GetFindString().encode("utf-8")
 		if not matchcase:
 			textstring = textstring.lower()
 			findstring = findstring.lower()
 		if backward:
 			start = self.GetSelection()[0]
 			loc = textstring.rfind(findstring, 0, start)
 		else:
 			start = self.GetSelection()[1]
 			loc = textstring.find(findstring, start)
-		
+
 		# if it wasn't found then restart at begining
 		if loc == -1 and start != 0:
 			if backward:
 				start = end
 				loc = textstring.rfind(findstring, 0, start)
 			else:
 				start = 0
 				loc = textstring.find(findstring, start)
-		
+
 		# was it still not found?
 		if loc == -1:
-			dlg = wx.MessageDialog(self, 'Unable to find the search text.',
-								   'Not found!',
-								   wx.OK | wx.ICON_INFORMATION)
+			dlg = wx.MessageDialog(
+					self,
+					"Unable to find the search text.",
+					"Not found!",
+					wx.OK | wx.ICON_INFORMATION,
+					)
 			dlg.ShowModal()
 			dlg.Destroy()
 		if findDlg:
 			if loc == -1:
 				wx.CallAfter(findDlg.SetFocus)
 				return
 			else:
 				findDlg.Close()
-		
+
 		# show and select the found text
 		self.ShowPosition(loc)
 		self.SetSelection(loc, loc + len(findstring))
-	
-	def OnFindText(self, *args):
+
+	def OnFindText(self, *_):
 		if self.findDlg is not None:
 			return
-		
-		self.findDlg = wx.FindReplaceDialog(self, self.findData,
-											"Find", wx.FR_NOWHOLEWORD)
+
+		self.findDlg = wx.FindReplaceDialog(self, self.findData, "Find", wx.FR_NOWHOLEWORD)
 		self.findDlg.Show()
-	
-	def OnFindClose(self, event):
-		self.findDlg.Destroy()
-		self.findDlg = None
 
+	def OnFindClose(self, _):
+		if self.findDlg is not None:
+			self.findDlg.Destroy()
+			self.findDlg = None
 
 	# Save Methods
+
 	def bufferHasChanged(self):
 		# the log buffers can always be saved
 		return True
-	
+
 	def bufferSave(self):
-		import time
+
 		appname = wx.GetApp().GetAppName()
 		default = appname + '-' + time.strftime("%Y%m%d-%H%M.py")
 		filename = wx.FileSelector(
-				"Save File As", "Saving",
+				"Save File As",
+				"Saving",
 				default_filename=default,
 				default_extension="py",
 				wildcard="*.py",
 				flags=wx.SAVE | wx.OVERWRITE_PROMPT
 				)
-		
+
 		if not filename:
 			return
-		
+
 		text = self.GetText()
-		
+
 		try:
-			f = open(filename, "w")
+			f = open(filename, 'w')
 			f.write(text)
 			f.close()
 		except:  # TODO: Find error type
-			d = wx.MessageDialog(
-					self, u'Error saving session', u'Error',
-					wx.OK | wx.ICON_ERROR
-					)
-			
+			d = wx.MessageDialog(self, "Error saving session", "Error", wx.OK | wx.ICON_ERROR)
+
 			d.ShowModal()
 			d.Destroy()
-		
+
 	def write(self, text):
 		"""
 		Display text in the log.
 
 		Replace line endings with OS-specific endings.
-		
+
 		:param text:
-		:type text:
 		"""
-		
+
 		text = self.fixLineEndings(text)
 		self.AddText(text)
 		self.EnsureCaretVisible()
 
 	def Append(self, text, c=None):
 		"""
 		Add the text to the end of the control using colour c which
 		should be suitable for feeding directly to wx.NamedColour.
 
 		:param text: ... Should be a unicode string or contain only ascii data.
-		:type text:
 		:param c:
-		:type c:
 		"""
-		
+
 		style = self.getStyle(c)
-		lenText = len(text.encode('utf8'))
+		lenText = len(text.encode("utf8"))
 		end = self.GetLength()
 		self.AppendText(text)
 		self.StartStyling(end, 31)
 		self.SetStyling(lenText, style)
 		self.EnsureCaretVisible()
-	
+
 	def AppendStderr(self, text):
 		"""
 		Add the stderr text to the end of the control using colour "red"
 
 		:param text: ... Should be a unicode string or contain only ascii data.
-		:type text:
 		"""
-		
-		self.Append(text, "red")
-
-
 
+		self.Append(text, "red")
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/ColourPickerPanel.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/StylePickerPanel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
-#  ColourPickerPanel.py
-"""
-Based on StylePickerPanel, a Panel for selecting a list of colours, and their order
-"""
+#  StylePickerPanel.py
 #
-#  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright 2019 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -19,177 +15,178 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
-#
 # generated by wxGlade 0.9.3 on Tue Apr  9 18:07:58 2019
 #
 
+# stdlib
+from typing import List, Optional
 
 # 3rd party
-import wx
-from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg as FigureCanvas
-from matplotlib.figure import Figure
-from domdf_wxpython_tools.StylePickerPanel import StylePickerPanel
+import wx  # type: ignore
+from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg as FigureCanvas  # type: ignore
+from matplotlib.figure import Figure  # type: ignore
+
+__all__ = ["StylePickerPanel"]
 
 # begin wxGlade: dependencies
 # end wxGlade
 
 # begin wxGlade: extracode
 # end wxGlade
 
+default_styles = ['o', 'v', '^', '<', '>', 's', 'h', 'X', 'D', 'd']
 
-default_colours = [
-		'#1f77b4',
-		'#ff7f0e',
-		'#2ca02c',
-		'#d62728',
-		'#9467bd',
-		'#8c564b',
-		'#e377c2',
-		'#7f7f7f',
-		'#bcbd22',
-		'#17becf'
-		]
-
-default_picker_choices = [
-		'#000000',
-		'#ff0000',
-		'#ffa500',
-		'#00ff00',
-		'#0000ff',
-		'#551a8b',
-		'#008080'
-		]
 
-
-class ColourPickerPanel(StylePickerPanel):
+class StylePickerPanel(wx.Panel):
 	"""
-	Based on StylePickerPanel, a Panel for selecting a list of colours, and their order
+	Based on StylePickerPanel, a Panel for selecting a list of colours, and their order.
+
+	:param parent: The parent window.
+	:param id: An identifier for the panel. wx.ID_ANY is taken to mean a default.
+	:param pos: The panel position. The value ``wx.DefaultPosition`` indicates a default position, chosen by either the windowing system or wxWidgets, depending on platform.
+	:param size: The panel size. The value ``wx.DefaultSize`` indicates a default size, chosen by either the windowing system or wxWidgets, depending on platform.
+	:param style: The window style. See wxPanel.
+	:param name: The window name.
+	:param label: Label for the panel
+	:param selection_choices: A list of hex value choices to populate the 'selection' side of the panel with
 	"""
-	
+
 	def __init__(
-			self, parent, id=wx.ID_ANY, pos=wx.DefaultPosition, size=wx.DefaultSize,
-			style=wx.TAB_TRAVERSAL, name=wx.PanelNameStr, label="Choose Colours: ",
-			picker_choices=None, selection_choices=None,
+			self,
+			parent: wx.Window,
+			id=wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			pos=wx.DefaultPosition,
+			size=wx.DefaultSize,
+			style=wx.TAB_TRAVERSAL,
+			name=wx.PanelNameStr,
+			label="Choose Styles: ",
+			selection_choices: Optional[List[str]] = None,
 			):
-		"""
-		:param parent: The parent window.
-		:type parent: wx.Window
-		:param id: An identifier for the panel. wx.ID_ANY is taken to mean a default.
-		:type id: wx.WindowID, optional
-		:param pos: The panel position. The value ::wxDefaultPosition indicates a default position, chosen by either the windowing system or wxWidgets, depending on platform.
-		:type pos: wx.Point, optional
-		:param size: The panel size. The value ::wxDefaultSize indicates a default size, chosen by either the windowing system or wxWidgets, depending on platform.
-		:type size: wx.Size, optional
-		:param style: The window style. See wxPanel.
-		:type style: int, optional
-		:param name: Window name.
-		:type name: str, optional
-		:param label: Label for the panel
-		:type label: str, optional
-		:param picker_choices: A list of hex value choices to populate the 'picker' size of the panel with
-		:type picker_choices: list of str
-		:param selection_choices: A list of hex value choices to populate the 'selection' size of the panel with
-		:type selection_choices: list of str
-		"""
-		
-		args = (parent, id, pos, size)
-		kwds = {"style": style, "name": name}
-		
-		if picker_choices is None:
-			picker_choices = default_picker_choices
-
 		if selection_choices is None:
-			selection_choices = default_colours[:]
-
+			selection_choices = default_styles[:]
 		self.label = label
-		self.picker_choices = picker_choices
 		self.selection_choices = selection_choices
-		
-		# begin wxGlade: ColourPickerPanel.__init__
+
+		args = (parent, id, pos, size)
+		kwds = {"style": style, "name": name}
+
+		# begin wxGlade: StylePickerPanel.__init__
 		kwds["style"] = kwds.get("style", 0) | wx.TAB_TRAVERSAL
 		wx.Panel.__init__(self, *args, **kwds)
 		self.main_panel = wx.Panel(self, wx.ID_ANY)
 		self.move_panel = wx.Panel(self.main_panel, wx.ID_ANY)
 		self.picker_list_box = wx.ListBox(self.main_panel, wx.ID_ANY, choices=[])
-		
+
 		self.picker_figure = Figure()
-		
+
 		self.picker_canvas = FigureCanvas(self.main_panel, wx.ID_ANY, self.picker_figure)
-		self.add_btn = wx.Button(self.main_panel, wx.ID_ANY, u"Add 🡲")
-		self.remove_btn = wx.Button(self.main_panel, wx.ID_ANY, u"🡰 Remove")
+		self.add_btn = wx.Button(self.main_panel, wx.ID_ANY, "Add 🡲")
+		self.remove_btn = wx.Button(self.main_panel, wx.ID_ANY, "🡰 Remove")
 		self.selection_list_box = wx.ListBox(self.main_panel, wx.ID_ANY, choices=[])
-		self.up_btn = wx.Button(self.main_panel, wx.ID_ANY, u"🡱 Up")
-		self.down_btn = wx.Button(self.main_panel, wx.ID_ANY, u"🡳 Down")
-		
+		self.up_btn = wx.Button(self.main_panel, wx.ID_ANY, "🡱 Up")
+		self.down_btn = wx.Button(self.main_panel, wx.ID_ANY, "🡳 Down")
+
 		self.selection_figure = Figure()
-		
+
 		self.selection_canvas = FigureCanvas(self.main_panel, wx.ID_ANY, self.selection_figure)
 
 		self.__set_properties()
 		self.__do_layout()
-		# end wxGlade
+
 		self.Bind(wx.EVT_LISTBOX, self.update_picker_preview, self.picker_list_box)
 		self.Bind(wx.EVT_LISTBOX_DCLICK, self.add, self.picker_list_box)
 		self.Bind(wx.EVT_BUTTON, self.add, self.add_btn)
 		self.Bind(wx.EVT_BUTTON, self.remove, self.remove_btn)
 		self.Bind(wx.EVT_LISTBOX, self.update_selection_preview, self.selection_list_box)
 		self.Bind(wx.EVT_BUTTON, self.move_up, self.up_btn)
 		self.Bind(wx.EVT_BUTTON, self.move_down, self.down_btn)
-		
+		# end wxGlade
+
 		self.Bind(wx.EVT_LISTBOX_DCLICK, self.remove, self.selection_list_box)
-		
-		self.remove_btn.SetLabel("Remove")
-		
-		self.selection_list_box.Clear()
-		self.selection_list_box.AppendItems(self.selection_choices)
+
+		self.markers = {
+				"point": '.',
+				"pixel": ',',
+				"circle": 'o',
+				"triangle_down": 'v',
+				"triangle_up": '^',
+				"triangle_left": '<',
+				"triangle_right": '>',
+				"tri_down": '1',
+				"tri_up": '2',
+				"tri_left": '3',
+				"tri_right": '4',
+				"octagon": '8',
+				"square": 's',
+				"pentagon": 'p',
+				"plus (filled)": 'P',
+				"star": '*',
+				"hexagon1": 'h',
+				"hexagon2": 'H',
+				"plus": '+',
+				'x': 'x',
+				"x (filled)": 'X',
+				"diamond": 'D',
+				"thin_diamond": 'd',
+				"caretleft": 4,
+				"caretright": 5,
+				"caretup": 6,
+				"caretdown": 7,
+				}
+
+		for marker in self.selection_choices:
+			for key in self.markers.keys():
+				if marker == self.markers[key]:
+					self.selection_list_box.Append(key)
 		if not self.selection_list_box.IsEmpty():
 			self.selection_list_box.SetSelection(0)
-		
-		self.picker_list_box.Clear()
-		self.picker_list_box.AppendItems(self.picker_choices)
-		if not self.picker_list_box.IsEmpty():
-			self.picker_list_box.SetSelection(0)
-		
+
+		for mark in filter(lambda x: x not in self.selection_choices, [self.markers[y] for y in self.markers]):
+			for key in self.markers.keys():
+				if mark == self.markers[key]:
+					self.picker_list_box.Append(key)
+		self.picker_list_box.SetSelection(0)
+
 		self.picker_axes = self.picker_figure.add_subplot(111)
 		self.selection_axes = self.selection_figure.add_subplot(111)
 		self.update_picker_preview()
 		self.update_selection_preview()
 
 	def __set_properties(self):
-		# begin wxGlade: ColourPickerPanel.__set_properties
+		# begin wxGlade: StylePickerPanel.__set_properties
 		self.move_panel.SetMinSize((170, -1))
 		self.picker_list_box.SetMinSize((170, 256))
 		self.picker_canvas.SetMinSize((64, 64))
 		self.selection_list_box.SetMinSize((170, 256))
 		self.up_btn.SetMinSize((80, -1))
 		self.down_btn.SetMinSize((80, -1))
 		self.selection_canvas.SetMinSize((64, 64))
 		self.main_panel.SetMinSize((450, -1))
 		# end wxGlade
 
 	def __do_layout(self):
-		# begin wxGlade: ColourPickerPanel.__do_layout
+		# begin wxGlade: StylePickerPanel.__do_layout
 		parent_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		main_sizer = wx.BoxSizer(wx.VERTICAL)
 		list_grid_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		sizer_4 = wx.BoxSizer(wx.VERTICAL)
 		selection_preview_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		move_grid = wx.GridSizer(1, 2, 0, 5)
 		sizer_3 = wx.BoxSizer(wx.VERTICAL)
 		sizer_2 = wx.BoxSizer(wx.VERTICAL)
 		picker_preview_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		grid_sizer = wx.GridSizer(1, 3, 10, 10)
 		borders_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Choose Styles: ")
 		borders_label.SetMinSize((128, 20))
-		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ""))
+		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ''))
 		grid_sizer.Add(borders_label, 0, wx.BOTTOM, 7)
 		grid_sizer.Add(self.move_panel, 1, wx.ALIGN_CENTER | wx.EXPAND, 0)
 		main_sizer.Add(grid_sizer, 0, 0, 0)
 		sizer_2.Add(self.picker_list_box, 5, wx.EXPAND, 0)
 		sizer_2.Add((0, 0), 0, 0, 0)
 		preview_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Preview: ")
 		picker_preview_sizer.Add(preview_label, 0, 0, 0)
@@ -214,108 +211,90 @@
 		self.main_panel.SetSizer(main_sizer)
 		parent_sizer.Add(self.main_panel, 0, wx.ALL, 10)
 		self.SetSizer(parent_sizer)
 		parent_sizer.Fit(self)
 		self.Layout()
 		# end wxGlade
 		borders_label.SetLabel(self.label)
-	
-	def add(self, event):  # wxGlade: ColourPickerPanel.<event_handler>
-		"""
-		Event handler for adding the colour currently selected in the 'picker' to the 'selection'
-		"""
-		
+
+	def move_up(self, event):  # wxGlade: StylePickerPanel.<event_handler>
+		self.move(-1)
+		event.Skip()
+
+	def move_down(self, event):  # wxGlade: StylePickerPanel.<event_handler>
+		self.move(1)
+		event.Skip()
+
+	def move(self, direction=1):
+		selection = self.selection_list_box.GetSelection()
+		selection_string = self.selection_list_box.GetString(selection)
+		if self.selection_list_box.GetCount() == selection + direction or selection + direction < 0:
+			return
+
+		self.selection_list_box.Delete(selection)
+		self.selection_list_box.InsertItems([selection_string], selection + direction)
+		self.selection_list_box.SetSelection(selection + direction)
+
+	def add(self, event):  # wxGlade: StylePickerPanel.<event_handler>
 		selection = self.picker_list_box.GetSelection()
 		if selection == -1:
 			return
-		
+
 		selection_string = self.picker_list_box.GetString(selection)
 		if selection_string == '':
 			return
-		
+
 		self.selection_list_box.Append(selection_string)
-		
+		self.picker_list_box.Delete(selection)
+
 		self.update_picker_preview()
-		
-		self.selection_list_box.SetSelection(self.selection_list_box.GetCount() - 1)
-		self.update_selection_preview()
 		event.Skip()
 
-	def remove(self, event):  # wxGlade: ColourPickerPanel.<event_handler>
-		"""
-		Event handler for removing the colour currently selected in the 'selection'
-		"""
-		
+	def remove(self, event):  # wxGlade: StylePickerPanel.<event_handler>
 		selection = self.selection_list_box.GetSelection()
 		if selection == -1:
 			return
-		
+
 		selection_string = self.selection_list_box.GetString(selection)
 		if selection_string == '':
 			return
-		
+
+		self.picker_list_box.Append(selection_string)
 		self.selection_list_box.Delete(self.selection_list_box.GetSelection())
-		
+
 		self.update_selection_preview()
 		event.Skip()
 
+	def update_picker_preview(self, *_):  # wxGlade: StylePickerPanel.<event_handler>
+		self.update_preview(self.picker_list_box, self.picker_axes)
+		self.picker_canvas.draw_idle()
+
+	def update_selection_preview(self, *_):  # wxGlade: StylePickerPanel.<event_handler>
+		self.update_preview(self.selection_list_box, self.selection_axes)
+		self.selection_canvas.draw_idle()
+
 	def update_preview(self, list_obj, axes):
-		"""
-		Update the preview from the given list
-		
-		:param list_obj: The list to update the preview for
-		:type list_obj: wx.ListBox
-		:param axes: The preview axes to update
-		:type axes: matplotlib.axes.Axes
-		"""
-		
 		axes.clear()
-		axes.axis('off')
+		axes.axis("off")
 		selection_string = list_obj.GetStringSelection()
 		if selection_string == '':
 			return
-		
-		axes.scatter(1, 1, s=400, color=selection_string, marker="s")
-	
-	def pick(self, *args):
-		"""
-		Open a wx.ColourDialog to edit the colour currently selected in the picker
-		"""
-		
-		selection = self.selection_list_box.GetSelection()
-		if selection == -1:
-			return
 
-		selection_string = self.selection_list_box.GetString(selection)
-		if selection_string == '':
-			return
-
-		colour = wx.ColourData()
-		colour.SetColour(selection_string)
+		axes.scatter(1, 1, s=200, color="red", marker=self.markers[selection_string])
 
-		dlg = wx.ColourDialog(self, data=colour)
+	do_layout = __do_layout
+	set_properties = __set_properties
 
-		res = dlg.ShowModal()
-		if res == wx.ID_OK:
-			self.selection_list_box.Delete(selection)
-			self.selection_list_box.InsertItems(
-					[dlg.GetColourData().GetColour().GetAsString(wx.C2S_HTML_SYNTAX)],
-					selection
-					)
-			self.selection_list_box.SetSelection(selection)
-			self.update_selection_preview()
-			dlg.Destroy()
-	
-	def GetSelection(self):
-		"""
-		Returns a list of the currently selected colours
-		
-		:rtype: list of str
-		"""
+	def get_selection(self):
 		return [
-				self.selection_list_box.GetString(item) for item in
-				range(self.selection_list_box.GetCount())
+				self.markers[self.selection_list_box.GetString(item)]
+				for item in range(self.selection_list_box.GetCount())
 				]
-	
-	get_selection = GetSelection
-	
-# end of class ColourPickerPanel
+
+	def _do_layout(self):
+		return self.__do_layout()
+
+	def _set_properties(self):
+		return self.__set_properties()
+
+
+# end of class StylePickerPanel
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/style_picker.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/style_picker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  style_picker.py
+"""
+Dialogs for choosing Matplotlib colours and styles.
+"""
 #
-#  Copyright 2019 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright (c) 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -16,133 +18,192 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
-#
 # generated by wxGlade 0.9.3 on Tue Apr  9 18:07:58 2019
 #
 
 # stdlib
-import sys
+from typing import List, Optional
 
 # 3rd party
-import wx
+import wx  # type: ignore
 
 # this package
-from domdf_wxpython_tools.StylePickerPanel import StylePickerPanel, default_styles
-from domdf_wxpython_tools.ColourPickerPanel import ColourPickerPanel, default_colours
+from domdf_wxpython_tools.ColourPickerPanel import ColourPickerPanel
+from domdf_wxpython_tools.StylePickerPanel import StylePickerPanel
 
+__all__ = ["StylePicker", "ColourPicker"]
 
 # begin wxGlade: dependencies
 # end wxGlade
 
 # begin wxGlade: extracode
 # end wxGlade
 
 
-class style_picker(wx.Dialog):
+class StylePicker(wx.Dialog):
+	r"""
+	Dialog for choosing Matplotlib marker styles.
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
+	:param title: The dialog title.
+	:param label: The dialog label.
+	:param selection_choices:
+	:param \*args: Additional arguments passed to :class:`wx.Dialog`.
+	:param \*\*kwds:  Additional keyword arguments passed to :class:`wx.Dialog`.
+	"""
+
 	def __init__(
-			self, parent, title="Choose Styles", label="Choose Styles: ",
-			selection_choices=None, *args, **kwds
+			self,
+			parent: wx.Window,
+			title: str = "Choose Styles",
+			label: str = "Choose Styles: ",
+			selection_choices: Optional[List] = None,
+			*args,
+			**kwds,
 			):
-		
+
 		self.title = title
-		
-		args = (parent,) + args
-		# begin wxGlade: style_picker.__init__
+
+		args = (parent, ) + args
+		# begin wxGlade: StylePicker.__init__
 		kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_DIALOG_STYLE
 		wx.Dialog.__init__(self, *args, **kwds)
 		self.StylePickerPanel = StylePickerPanel(self, label=label, selection_choices=selection_choices)
 		self.button_panel = wx.Panel(self, wx.ID_ANY)
 		self.cancel_btn = wx.Button(self.button_panel, wx.ID_ANY, "Cancel")
 		self.apply_btn = wx.Button(self.button_panel, wx.ID_ANY, "Apply")
 
 		self.__set_properties()
 		self.__do_layout()
 
 		self.Bind(wx.EVT_BUTTON, self.cancel, self.cancel_btn)
 		self.Bind(wx.EVT_BUTTON, self.apply, self.apply_btn)
 		# end wxGlade
-	
+
 	def __set_properties(self):
-		# begin wxGlade: style_picker.__set_properties
+		# begin wxGlade: StylePicker.__set_properties
 		self.SetTitle("Choose Styles")
 		# end wxGlade
 		self.SetTitle(self.title)
-	
+
 	def __do_layout(self):
-		# begin wxGlade: style_picker.__do_layout
+		# begin wxGlade: StylePicker.__do_layout
 		parent_sizer = wx.FlexGridSizer(2, 1, 0, 0)
 		button_grid = wx.GridSizer(1, 2, 0, 5)
 		parent_sizer.Add(self.StylePickerPanel, 1, wx.EXPAND, 0)
 		button_grid.Add(self.cancel_btn, 0, wx.ALIGN_CENTER, 0)
 		button_grid.Add(self.apply_btn, 0, wx.ALIGN_CENTER, 0)
 		self.button_panel.SetSizer(button_grid)
 		parent_sizer.Add(self.button_panel, 1, wx.ALIGN_BOTTOM | wx.ALIGN_RIGHT | wx.ALL, 5)
 		self.SetSizer(parent_sizer)
 		parent_sizer.Fit(self)
 		self.Layout()
 		# end wxGlade
 
-	def cancel(self, _):  # wxGlade: style_picker.<event_handler>
+	def cancel(self, _):  # wxGlade: StylePicker.<event_handler>
+		"""
+		Called when the user presses the :guilabel:`Cancel` button.
+		"""
+
 		self.Destroy()
-	
-	def apply(self, event):  # wxGlade: style_picker.<event_handler>
+
+	def apply(self, event) -> None:  # wxGlade: StylePicker.<event_handler>
+		"""
+		Called when the user presses the :guilabel:`Apply` button.
+
+		:param event: The wxPython event.
+		"""
+
 		self.style_list = self.StylePickerPanel.get_selection()
 		event.Skip()
 		self.EndModal(wx.ID_OK)
 
-# end of class style_picker
+
+# end of class StylePicker
+
+style_picker = StylePicker
 
 
-class colour_picker(style_picker):
+class ColourPicker(style_picker):
+	r"""
+	Dialog for choosing Matplotlib colours.
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
+	:param title: The dialog title.
+	:param label: The dialog label.
+	:param selection_choices:
+	:param \*args: Additional arguments passed to :class:`wx.Dialog`.
+	:param \*\*kwds:  Additional keyword arguments passed to :class:`wx.Dialog`.
+	"""
+
 	def __init__(
-			self, parent, title="Choose Colours", label="Choose Colours: ",
-			picker_choices=None, selection_choices=None, *args, **kwds
+			self,
+			parent: wx.Window,
+			title: str = "Choose Colours",
+			label: str = "Choose Colours: ",
+			picker_choices: Optional[List] = None,
+			selection_choices: Optional[List] = None,
+			*args,
+			**kwds
 			):
-		
+
 		self.title = title
 		self.picker_choices = picker_choices
 
-		args = (parent,) + args
+		args = (parent, ) + args
 
 		kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_DIALOG_STYLE
 		wx.Dialog.__init__(self, *args, **kwds)
-		self.StylePickerPanel = ColourPickerPanel(self, label=label, picker_choices=picker_choices, selection_choices=selection_choices)
+		self.StylePickerPanel = ColourPickerPanel(
+				self,
+				label=label,
+				picker_choices=picker_choices,
+				selection_choices=selection_choices,
+				)
 		self.button_panel = wx.Panel(self, wx.ID_ANY)
 		self.cancel_btn = wx.Button(self.button_panel, wx.ID_ANY, "Cancel")
 		self.apply_btn = wx.Button(self.button_panel, wx.ID_ANY, "Apply")
 
 		self.__set_properties()
 		self.__do_layout()
 
 		self.Bind(wx.EVT_BUTTON, self.cancel, self.cancel_btn)
 		self.Bind(wx.EVT_BUTTON, self.apply, self.apply_btn)
 
-	
-	def apply(self, event):
+	def apply(self, event) -> None:
+		"""
+		Called when the user presses the :guilabel:`Apply` button.
+
+		:param event: The wxPython event.
+		"""
+
 		self.colour_list = self.StylePickerPanel.get_selection()
 		event.Skip()
 		self.EndModal(wx.ID_OK)
-	
+
 	def __set_properties(self):
 		# begin wxGlade: style_picker.__set_properties
 		self.SetTitle("Choose Styles")
 		# end wxGlade
 		self.SetTitle(self.title)
-	
+
 	def __do_layout(self):
 		# begin wxGlade: style_picker.__do_layout
 		parent_sizer = wx.FlexGridSizer(2, 1, 0, 0)
 		button_grid = wx.GridSizer(1, 2, 0, 5)
 		parent_sizer.Add(self.StylePickerPanel, 1, wx.EXPAND, 0)
 		button_grid.Add(self.cancel_btn, 0, wx.ALIGN_CENTER, 0)
 		button_grid.Add(self.apply_btn, 0, wx.ALIGN_CENTER, 0)
 		self.button_panel.SetSizer(button_grid)
 		parent_sizer.Add(self.button_panel, 1, wx.ALIGN_BOTTOM | wx.ALIGN_RIGHT | wx.ALL, 5)
 		self.SetSizer(parent_sizer)
 		parent_sizer.Fit(self)
 		self.Layout()
 		# end wxGlade
+
+
+colour_picker = ColourPicker
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/timer_thread.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/timer_thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #  !/usr/bin/env python
-#   -*- coding: utf-8 -*-
 #
 #  timer_thread.py
 """
 Background thread that sends an event after the specified interval.
-Useful for timeouts or updating timers, clocks etc.
-
 
-Includes code from https://gist.github.com/samarthbhargav/5a515a399f7113137331
+Useful for timeouts or updating timers, clocks etc.
 """
 #
 #  Copyright (c) 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
@@ -23,59 +20,66 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
+#  Includes code from https://gist.github.com/samarthbhargav/5a515a399f7113137331
+#
 
+# stdlib
 import time
+from threading import Event, Thread
 
-from threading import Thread, Event
+# 3rd party
+import wx  # type: ignore
 
+# this package
 from domdf_wxpython_tools.events import SimpleEvent
 
-timer_event = SimpleEvent("Timer")
+__all__ = ["Timer", "timer_event"]
+
+timer_event = SimpleEvent(name="Timer")
+"""
+An instance of :class:`domdf_python_tools.events.SimpleEvent` called **Timer**.
+
+This event is triggered when the timer has expired.
+"""
 
 
 class Timer(Thread):
 	"""
-	Background Timer Class
+	Background Timer Class.
+
+	:param parent: Class to send event updates to.
+	:param interval: Interval to trigger events at, in seconds.
 	"""
-	
-	def __init__(self, parent, interval=1.0):
-		"""
-		Init Timer Thread Class
 
-		:param parent: Class to send event updates to
-		:param interval: Interval to trigger events at, in seconds. Default 1.0
-		:type interval: float
-		"""
-		
+	def __init__(self, parent: wx.Window, interval: float = 1.0):
 		self._stopevent = Event()
 		Thread.__init__(self, name="TimerThread")
 		self._parent = parent
 		self._interval = interval
-	
-	def run(self):
+
+	def run(self) -> None:
 		"""
-		Run Timer Thread
+		Run the timer thread.
 		"""
-		
+
 		wait_time = 0 + self._interval
 		while not self._stopevent.isSet():
 			time.sleep(0.1)
 			wait_time -= 0.1
 			if wait_time < 0.0:
 				timer_event.trigger()
 				wait_time = 0 + self._interval
-	
-	def join(self, timeout=None):
+
+	def join(self, timeout=None) -> None:
 		"""
-		Stop the thread and wait for it to end
+		Stop the thread and wait for it to end.
 
 		:param timeout:
-		:type:
 		"""
-		
+
 		self._stopevent.set()
-		Thread.join(self, timeout)
+		Thread.join(self, timeout)
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/imagepanel.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/imagepanel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #  !/usr/bin/env python
-#   -*- coding: utf-8 -*-
 #
 #  imagepanel.py
 """
 Based on ChartPanelBase, a canvas for displaying an image within a wxPython window
 using PIL and matplotlib, with a right click menu with some basic options
-"""
+"""  # noqa: D400
 #
 #  Copyright 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -21,25 +20,33 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
+# stdlib
+from typing import Union
+
 # 3rd party
-import matplotlib
-import wx
-from matplotlib.figure import Figure
+import matplotlib  # type: ignore
+import matplotlib.projections  # type: ignore
+import PIL  # type: ignore
+import wx  # type: ignore
+from domdf_python_tools.typing import PathLike
+from matplotlib.figure import Figure  # type: ignore
 from PIL import Image
 
 # this package
 from domdf_wxpython_tools.chartpanel import ChartPanelBase
-from domdf_wxpython_tools.dialogs import file_dialog_wildcard, Wildcards
+from domdf_wxpython_tools.dialogs import Wildcards, file_dialog_wildcard
 from domdf_wxpython_tools.projections import NoZoom
 
+__all__ = ["EvtImgPanelChanged", "ImagePanel"]
+
 # Prevent zooming of axis with mouse click
 matplotlib.projections.register_projection(NoZoom)
 
 # Wildcard for Open and Save dialogs
 images_wildcard = Wildcards()
 images_wildcard.add_image_wildcard()
 images_wildcard.add_common_filetype("jpeg")
@@ -60,295 +67,290 @@
 # Events
 ImgPanelChangedEvent = wx.NewEventType()
 EVT_IMAGE_PANEL_CHANGED = wx.PyEventBinder(ImgPanelChangedEvent, 0)
 
 
 class EvtImgPanelChanged(wx.PyCommandEvent):
 	"""
-	Custom Event for an image in the ImagePanel being changed
+	Custom Event for an image in the ImagePanel being changed.
+
+	:param windowID:
+	:param obj:
 	"""
+
 	eventType = ImgPanelChangedEvent
 
-	def __init__(self, windowID, obj):
-		"""
-		
-		:param windowID:
-		:type windowID: int
-		:param obj:
-		:type obj:
-		"""
-		
+	def __init__(self, windowID: int, obj):
+
 		wx.PyCommandEvent.__init__(self, self.eventType, windowID)
 		self.SetEventObject(obj)
 
 
 class ImagePanel(ChartPanelBase):
 	"""
 	Panel that contains a matplotlib plotting window, used for displaying an image.
 	The image can be right clicked to bring up a context menu allowing copying, pasting and saving of the image.
 	The image can be panned by holding the left mouse button and moving the mouse,
 	and zoomed in and out using the scrollwheel on the mouse.
+
+	:param parent: The parent window.
+	:param image:
+	:param id: An identifier for the panel. wx.ID_ANY is taken to mean a default.
+	:param pos: The panel position. The value ``wx.DefaultPosition`` indicates a default position,
+		chosen by either the windowing system or wxWidgets, depending on platform.
+	:param size: The panel size. The value ::wxDefaultSize indicates a default size, chosen by
+		either the windowing system or wxWidgets, depending on platform.
+	:param style: The window style. See wxPanel.
+	:param name: Window name.
 	"""
-	
+
 	default_image = ("RGB", (640, 480), (240, 240, 240))
-	
+
 	def __init__(
-			self, parent, image=None, id=wx.ID_ANY, pos=wx.DefaultPosition,
-			size=wx.DefaultSize, style=0, name=wx.PanelNameStr):
-		"""
-		:param parent: The parent window.
-		:type parent: wx.Window
-		:param image:
-		:type image:
-		:param id: An identifier for the panel. wx.ID_ANY is taken to mean a default.
-		:type id: wx.WindowID, optional
-		:param pos: The panel position. The value ::wxDefaultPosition indicates a default position,
-		:type pos: wx.Point, optional
-			chosen by either the windowing system or wxWidgets, depending on platform.
-		:param size: The panel size. The value ::wxDefaultSize indicates a default size, chosen by
-		:type size: wx.Size, optional
-			either the windowing system or wxWidgets, depending on platform.
-		:param style: The window style. See wxPanel.
-		:type style: int, optional
-		:param name: Window name.
-		:type name: str, optional
-		"""
-		
+			self,
+			parent: wx.Window,
+			image=None,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = 0,
+			name: str = wx.PanelNameStr
+			):
+
 		fig = Figure()
 		ax = fig.add_subplot(111, frameon=False, projection="NoZoom")  # 1x1 grid, first subplot
-		
+
 		ChartPanelBase.__init__(self, parent, fig, ax, id, pos, size, style, name)
-		
+
 		if isinstance(image, Image.Image):
 			# PIL Image object, load directly
 			self._image = image
 		elif image is None:
 			self._image = Image.new(*self.default_image)
 		else:
 			# Filename, load from file
 			# self._image = mpimg.imread(image)
 			self._image = Image.open(image)
-			
+
 		self.editable = True
-		
+
 		self._setup_context_menu()
-		
+
 		self._load_image()
 		wx.CallAfter(self.reset_view)
-	
+
 	def _setup_context_menu(self):
 		self.context_menu = wx.Menu()
-		
+
 		self.context_menu.Append(ID_ImagePanel_Reset_View, "Reset View")
 		self.Bind(wx.EVT_MENU, self.reset_view, id=ID_ImagePanel_Reset_View)
-		
+
 		self.context_menu.AppendSeparator()
-		
+
 		self.context_menu.Append(ID_ImagePanel_Copy_Image, "Copy Image")
 		self.Bind(wx.EVT_MENU, self.copy, id=ID_ImagePanel_Copy_Image)
 		self.context_menu.Append(ID_ImagePanel_Paste_Image, "Paste Image")
 		self.Bind(wx.EVT_MENU, self.paste, id=ID_ImagePanel_Paste_Image)
-		
+
 		self.context_menu.Append(ID_ImagePanel_Save_Image, "Save Image")
 		self.Bind(wx.EVT_MENU, self.on_save, id=ID_ImagePanel_Save_Image)
-		
+
 		self.context_menu.AppendSeparator()
-		
+
 		self.context_menu.Append(ID_ImagePanel_Load_Image, "Load Image")
 		self.Bind(wx.EVT_MENU, self.on_load, id=ID_ImagePanel_Load_Image)
-		
+
 		self.context_menu.Append(ID_ImagePanel_Delete_Image, "Delete Image")
 		self.Bind(wx.EVT_MENU, self.clear, id=ID_ImagePanel_Delete_Image)
-	
-	def load_image(self, new_image=None, suppress_event=False):
+
+	def load_image(self, new_image: Union[Image.Image, None, PathLike] = None, suppress_event: bool = False):
 		"""
-		Load the 'new_image' into the contol
-		
-		:param new_image: The image to load, or a string pointing to the image on a filesystem
-		:type new_image: :class:`PIL.Image.Image` or str or pathlib.Path, optional
-		:param suppress_event: Whether the event that the image has changed should be suppressed, default False
-		:type suppress_event: bool, optional
-		
-		TODO: Do we even need to be triggering an event here, since "load_image"
-		 is only ever going to be called by the programmer
+		Load the 'new_image' into the control.
+
+		:param new_image: The image to load, or a string pointing to the image
+			on a filesystem.
+		:param suppress_event: Whether the event that the image has changed should
+			be suppressed.
+
+		.. TODO::
+
+			Do we even need to be triggering an event here, since "load_image"
+			is only ever going to be called by the programmer
 		"""
-		
+
 		self.ax.clear()
 		self._image = None
 		self._image = None
-		
+
 		if isinstance(new_image, Image.Image):
 			# PIL Image object, load directly
 			self._image = new_image
 		elif new_image is None:
 			self._image = Image.new(*self.default_image)
 		else:
 			# Filename, load from file
 			# self._image = mpimg.imread(image)
 			self._image = Image.open(str(new_image))
-		
+
 		self._load_image()
 		self.pan(True)
-		
+
 		if not suppress_event:
 			wx.PostEvent(self.GetEventHandler(), EvtImgPanelChanged(self.GetId(), self))
-	
+
 	def _load_image(self):
 		"""
 		Internal function for the actual loading of the image
 		"""
-		
+
 		self.ax.clear()
-		self.ax.imshow(self._image, aspect='equal')
-		
+		self.ax.imshow(self._image, aspect="equal")
+
 		self.ax.axes.get_xaxis().set_visible(False)
 		self.ax.axes.get_yaxis().set_visible(False)
 		# self.fig.tight_layout()
 		self.fig.subplots_adjust(left=0, bottom=0, top=1, right=1)
-		
+
 		self.canvas.draw()
-		
+
 		self.pan(True)
 		self.ax.autoscale(tight=True)
 		self.setup_scrollwheel_zooming()
-		self.canvas.mpl_connect('button_press_event', self.on_context_menu)
-		
+		self.canvas.mpl_connect("button_press_event", self.on_context_menu)
+
 	def on_context_menu(self, event):
 		"""
 		Event Handler for bringing up right click context menu
 		"""
-		
+
 		if event.button == matplotlib.backend_bases.MouseButton.RIGHT:
 			event.guiEvent.GetEventObject().ReleaseMouse()
-			print('in context_menu callback: clicked at (%g, %g)' % (event.x, event.y))
+			print(f'in context_menu callback: clicked at ({event.x:g}, {event.y:g})')
 			self.PopupMenu(self.context_menu)
 			# UIActionSimulator().MouseClick(wx.MOUSE_BTN_RIGHT)
-	
-	def copy(self, event=None):
+
+	def copy(self, _=None):
 		"""
-		Copy the image to the clipboard
+		Copy the image to the clipboard.
 		"""
-		
+
 		width, height = self._image.size
 		bmp = wx.Bitmap.FromBuffer(width, height, self._image.tobytes())
-		
+
 		# Create BitmapDataObject
 		bmp_data = wx.BitmapDataObject(bmp)
-		
+
 		# Write image from clipboard
 		if wx.TheClipboard.Open():
 			wx.TheClipboard.SetData(bmp_data)
 			wx.TheClipboard.Flush()
 		wx.TheClipboard.Close()
-	
+
 	def paste(self, event=None):
 		"""
-		Paste the image from the clipboard into the control
+		Paste the image from the clipboard into the control.
 		"""
-		
+
 		# Create empty BitmapDataObject
 		bmp_data = wx.BitmapDataObject()
-		
+
 		# Read image from clipboard
 		wx.TheClipboard.Open()
 		if wx.TheClipboard.GetData(bmp_data):
 			wx.TheClipboard.Close()
-			
+
 			# https://stackoverflow.com/a/46606553/3092681
 			# Get bitmap and convert to PIL Image
 			bmp = bmp_data.GetBitmap()
 			size = tuple(bmp.GetSize())
 			buf = size[0] * size[1] * 3 * b"\x00"
 			bmp.CopyToBuffer(buf)
 			self._image = Image.frombuffer("RGB", size, buf, "raw", "RGB", 0, 1)
 			self._load_image()
 			self.pan(True)
 			if event:
 				event.Skip()
-			
+
 			wx.PostEvent(self.GetEventHandler(), EvtImgPanelChanged(self.GetId(), self))
-		
+
 		else:
 			# No image on clipboard
 			wx.TheClipboard.Close()
-	
+
 	def on_save(self, event=None):
 		"""
 		Save the image to the location selected in the dialog
 		"""
 
 		save_location = file_dialog_wildcard(
-				self, "Save Image",
-				images_wildcard.wildcard,
-				style=wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT
+				self, "Save Image", images_wildcard.wildcard, style=wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT
 				)
-		
+
 		if not save_location:
 			return
-		
+
 		self._image.save(save_location[0])
-	
+
 	def on_load(self, event=None):
 		"""
 		Load the image into the dialog from the file selected in the dialog
 		"""
-		
+
 		new_image = file_dialog_wildcard(
-				self, "Choose an Image",
-				images_wildcard.wildcard,
-				style=wx.FD_OPEN | wx.FD_FILE_MUST_EXIST
+				self, "Choose an Image", images_wildcard.wildcard, style=wx.FD_OPEN | wx.FD_FILE_MUST_EXIST
 				)
-		
+
 		if not new_image:
 			return
-		
+
 		self._image = Image.open(new_image[0])
 		self._load_image()
 		self.pan(True)
 		if event:
 			event.Skip()
-		
+
 		wx.PostEvent(self.GetEventHandler(), EvtImgPanelChanged(self.GetId(), self))
-	
+
 	def clear(self, event=None):
 		"""
 		Clear the image from the control
 		"""
-		
+
 		self.ax.clear()
 		self._image = None
 		self._image = None
 		if event:
 			event.Skip()
-		
+
 		wx.PostEvent(self.GetEventHandler(), EvtImgPanelChanged(self.GetId(), self))
-		
+
 	def reset_view(self, *_):
 		"""
-		Reset the view of the image
+		Reset the view of the image.
 		"""
-		
+
 		self._load_image()
 		# self.fig.tight_layout()
 		self.fig.subplots_adjust(left=0, bottom=0, top=1, right=1)
 		self.canvas.SetSize(self.GetSize())
 		self.Refresh()
 		self.canvas.draw()
 		self.canvas.Refresh()
 		self.pan(True)
 		# wx.CallAfter(self.pan)
-	
+
 	@property
-	def image(self):
+	def image(self) -> PIL.Image.Image:
 		"""
 		Returns the image being displayed in the control
-		
+
 		:rtype: PIL.Image.Image
 		"""
 		return self._image
+
 	#
 	# @image.setter
 	# def image(self, new_image):
 	#
 	# 	if isinstance(new_image, Image.Image):
 	# 		# PIL Image object, load directly
 	# 		self._image = new_image
@@ -358,8 +360,7 @@
 	# 		# Filename, load from file
 	# 		# self._image = mpimg.imread(image)
 	# 		self._image = Image.open(new_image)
 	#
 	# 	self.load_image()
 	# 	#self.reset_view()
 	# 	wx.CallAfter(self.reset_view)
-
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/keyboard.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/keyboard.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
+
 #
 #  keyboard.py
 #
 #  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
@@ -17,46 +17,132 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
-import wx
+# 3rd party
+import wx  # type: ignore
+
+__all__ = ["gen_keymap"]
 
 
 def gen_keymap():
-	
+
 	keys = (
-			"BACK", "TAB", "RETURN", "ESCAPE", "SPACE", "DELETE", "START",
-			"LBUTTON", "RBUTTON", "CANCEL", "MBUTTON", "CLEAR", "PAUSE",
-			"CAPITAL", "END", "HOME", "LEFT", "UP", "RIGHT",
-			"DOWN", "SELECT", "PRINT", "EXECUTE", "SNAPSHOT", "INSERT", "HELP",
-			"NUMPAD0", "NUMPAD1", "NUMPAD2", "NUMPAD3", "NUMPAD4", "NUMPAD5",
-			"NUMPAD6", "NUMPAD7", "NUMPAD8", "NUMPAD9", "MULTIPLY", "ADD",
-			"SEPARATOR", "SUBTRACT", "DECIMAL", "DIVIDE", "F1", "F2", "F3", "F4",
-			"F5", "F6", "F7", "F8", "F9", "F10", "F11", "F12", "F13", "F14",
-			"F15", "F16", "F17", "F18", "F19", "F20", "F21", "F22", "F23", "F24",
-			"NUMLOCK", "SCROLL", "PAGEUP", "PAGEDOWN", "NUMPAD_SPACE",
-			"NUMPAD_TAB", "NUMPAD_ENTER", "NUMPAD_F1", "NUMPAD_F2", "NUMPAD_F3",
-			"NUMPAD_F4", "NUMPAD_HOME", "NUMPAD_LEFT", "NUMPAD_UP",
-			"NUMPAD_RIGHT", "NUMPAD_DOWN", "NUMPAD_PAGEUP",
-			"NUMPAD_PAGEDOWN", "NUMPAD_END", "NUMPAD_BEGIN",
-			"NUMPAD_INSERT", "NUMPAD_DELETE", "NUMPAD_EQUAL", "NUMPAD_MULTIPLY",
-			"NUMPAD_ADD", "NUMPAD_SEPARATOR", "NUMPAD_SUBTRACT", "NUMPAD_DECIMAL",
-			"NUMPAD_DIVIDE"
+			"BACK",
+			"TAB",
+			"RETURN",
+			"ESCAPE",
+			"SPACE",
+			"DELETE",
+			"START",
+			"LBUTTON",
+			"RBUTTON",
+			"CANCEL",
+			"MBUTTON",
+			"CLEAR",
+			"PAUSE",
+			"CAPITAL",
+			"END",
+			"HOME",
+			"LEFT",
+			"UP",
+			"RIGHT",
+			"DOWN",
+			"SELECT",
+			"PRINT",
+			"EXECUTE",
+			"SNAPSHOT",
+			"INSERT",
+			"HELP",
+			"NUMPAD0",
+			"NUMPAD1",
+			"NUMPAD2",
+			"NUMPAD3",
+			"NUMPAD4",
+			"NUMPAD5",
+			"NUMPAD6",
+			"NUMPAD7",
+			"NUMPAD8",
+			"NUMPAD9",
+			"MULTIPLY",
+			"ADD",
+			"SEPARATOR",
+			"SUBTRACT",
+			"DECIMAL",
+			"DIVIDE",
+			"F1",
+			"F2",
+			"F3",
+			"F4",
+			"F5",
+			"F6",
+			"F7",
+			"F8",
+			"F9",
+			"F10",
+			"F11",
+			"F12",
+			"F13",
+			"F14",
+			"F15",
+			"F16",
+			"F17",
+			"F18",
+			"F19",
+			"F20",
+			"F21",
+			"F22",
+			"F23",
+			"F24",
+			"NUMLOCK",
+			"SCROLL",
+			"PAGEUP",
+			"PAGEDOWN",
+			"NUMPAD_SPACE",
+			"NUMPAD_TAB",
+			"NUMPAD_ENTER",
+			"NUMPAD_F1",
+			"NUMPAD_F2",
+			"NUMPAD_F3",
+			"NUMPAD_F4",
+			"NUMPAD_HOME",
+			"NUMPAD_LEFT",
+			"NUMPAD_UP",
+			"NUMPAD_RIGHT",
+			"NUMPAD_DOWN",
+			"NUMPAD_PAGEUP",
+			"NUMPAD_PAGEDOWN",
+			"NUMPAD_END",
+			"NUMPAD_BEGIN",
+			"NUMPAD_INSERT",
+			"NUMPAD_DELETE",
+			"NUMPAD_EQUAL",
+			"NUMPAD_MULTIPLY",
+			"NUMPAD_ADD",
+			"NUMPAD_SEPARATOR",
+			"NUMPAD_SUBTRACT",
+			"NUMPAD_DECIMAL",
+			"NUMPAD_DIVIDE",
 			)
-	
+
 	keyMap = {}
-	
+
 	for i in keys:
 		keyMap[getattr(wx, "WXK_" + i)] = i
 	for i in ("SHIFT", "ALT", "CONTROL", "MENU"):
 		keyMap[getattr(wx, "WXK_" + i)] = ''
-	
+
 	return keyMap
 
 
 NAVKEYS = {
-		wx.WXK_END, wx.WXK_PAGEUP, wx.WXK_PAGEDOWN,
-		wx.WXK_LEFT, wx.WXK_RIGHT, wx.WXK_UP, wx.WXK_DOWN,
+		wx.WXK_END,
+		wx.WXK_PAGEUP,
+		wx.WXK_PAGEDOWN,
+		wx.WXK_LEFT,
+		wx.WXK_RIGHT,
+		wx.WXK_UP,
+		wx.WXK_DOWN,
 		}
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/tabbable_textctrl.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/tabbable_textctrl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #  !/usr/bin/env python
-#   -*- coding: utf-8 -*-
 #
-#  imagepanel.py
+#  tabbable_textctrl.py
 """
 Multiline wx.TextCtrl that allows tabbing to the next or previous control.
 """
 #
-#  Copyright 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #  With help from http://wxpython-users.1045709.n5.nabble.com/Text-control-and-TAB-td2306159.html
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
@@ -21,57 +20,69 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
-import wx
+# stdlib
+from typing import AnyStr
+
+# 3rd party
+import wx  # type: ignore
+
+__all__ = ["TabbableTextCtrl"]
 
 
 class TabbableTextCtrl(wx.TextCtrl):
 	"""
-	Multiline wx.TextCtrl that allows tabbing to the next or previous control.
+	Multiline :class:`wx.TextCtrl` that allows tabbing to the next or previous control.
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
+	:param id: Control identifier. A value of ``-1`` denotes a default value.
+	:param value: Default text value.
+	:param pos: Text control position.
+	:param size: Text control size.
+	:param style: Window style. See :class:`wx.TextCtrl`.
+	:param validator: Window validator.
+	:default validator: :py:obj:`wx.DefaultValidator`
+	:param name: Window name.
 	"""
-	
+
 	def __init__(
-			self, parent, id=wx.ID_ANY, value='',
-			pos=wx.DefaultPosition, size=wx.DefaultSize, style=0,
-			validator=wx.DefaultValidator, name=wx.TextCtrlNameStr):
-		"""
-		:param parent: Parent window. Should not be None.
-		:type parent: wx.Window
-		:param id: Control identifier. A value of -1 denotes a default value.
-		:type id: wx.WindowID
-		:param value: Default text value.
-		:type value: str
-		:param pos: Text control position.
-		:type pos: wx.Point
-		:param size:  Text control size.
-		:type size: wx.Size
-		:param style: Window style. See wx.TextCtrl.
-		:type style: int
-		:param validator: Window validator.
-		:type validator: wx.Validator
-		:param name: Window name.
-		:type name: str
-		"""
-		
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			value: str = '',
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = 0,
+			validator: wx.Validator = wx.DefaultValidator,
+			name: AnyStr = wx.TextCtrlNameStr
+			):
 		wx.TextCtrl.__init__(
-				self, parent, id, value=value, pos=pos, size=size,
+				self,
+				parent,
+				id,
+				value=value,
+				pos=pos,
+				size=size,
 				style=style | wx.TE_MULTILINE | wx.TE_PROCESS_ENTER,
-				validator=validator, name=name)
-		
+				validator=validator,
+				name=name
+				)
+
 		self.Bind(wx.EVT_CHAR, self.on_char)
-	
+
 	@staticmethod
-	def on_char(event):
+	def on_char(event) -> None:
 		"""
-		Event handler for key being pressed, to allow for navigating between controls with TAB
+		Event handler for key being pressed, to allow for navigating between controls with :kbd:`TAB`.
 		"""
+
 		if event.GetKeyCode() == wx.WXK_TAB:
 			flags = wx.NavigationKeyEvent.IsForward
 			if event.ShiftDown():
 				flags = wx.NavigationKeyEvent.IsBackward
 			# if event.ControlDown():
 			# 	flags = wx.NavigationKeyEvent.WinChange
 			event.GetEventObject().GetParent().Navigate(flags)
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/border_config.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/border_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #  !/usr/bin/env python
-#   -*- coding: utf-8 -*-
 #
 #  border_config.py
 """
-Dialog for configuring borders for charts
+Dialog for configuring borders for charts.
 """
 #
 #  Copyright (c) 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This file was originally part of GunShotMatch
 #  Copyright (c) 2019 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
@@ -24,27 +23,37 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
 # 3rd party
-import wx
+import wx  # type: ignore
+
+__all__ = ["border_config"]
 
 # begin wxGlade: dependencies
 # end wxGlade
 
 # begin wxGlade: extracode
 # end wxGlade
 
 
 class border_config(wx.Dialog):
-	def __init__(self, parent, chromatogram_figure, *args, **kwds):
+	r"""
+
+	:param parent:
+	:param chromatogram_figure:
+	:param \*args:
+	:param \*\*kwds:
+	"""
+
+	def __init__(self, parent: wx.Window, chromatogram_figure, *args, **kwds):
 		self.chromatogram_figure = chromatogram_figure
-		args = (parent,) + args
+		args = (parent, ) + args
 		# begin wxGlade: border_config.__init__
 		kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_DIALOG_STYLE
 		wx.Dialog.__init__(self, *args, **kwds)
 		self.main_panel = wx.Panel(self, wx.ID_ANY)
 		self.top_border_value = wx.SpinCtrlDouble(self.main_panel, wx.ID_ANY, "0.9", min=0.0, max=2.0)
 		self.top_border_value.SetDigits(3)
 		self.bottom_border_value = wx.SpinCtrlDouble(self.main_panel, wx.ID_ANY, "0.125", min=0.0, max=2.0)
@@ -71,35 +80,35 @@
 		self.Bind(wx.EVT_SPINCTRLDOUBLE, self.update_borders, self.right_border_value)
 		self.Bind(wx.EVT_TEXT, self.update_borders, self.right_border_value)
 		self.Bind(wx.EVT_TEXT_ENTER, self.update_borders, self.right_border_value)
 		self.Bind(wx.EVT_BUTTON, self.apply_tight_layout, self.tight_layout_button)
 		self.Bind(wx.EVT_BUTTON, self.close_dialog, self.close_btn)
 		# end wxGlade
 
-	def __set_properties(self):
+	def __set_properties(self) -> None:
 		# begin wxGlade: border_config.__set_properties
 		self.SetTitle("Configure Borders")
 		self.top_border_value.SetMinSize((120, -1))
 		self.top_border_value.SetIncrement(0.005)
 		self.bottom_border_value.SetMinSize((120, -1))
 		self.bottom_border_value.SetIncrement(0.005)
 		self.left_border_value.SetMinSize((120, -1))
 		self.left_border_value.SetIncrement(0.005)
 		self.right_border_value.SetMinSize((120, -1))
 		self.right_border_value.SetIncrement(0.005)
 		self.tight_layout_button.SetMinSize((120, -1))
 		# end wxGlade
 
-	def __do_layout(self):
+	def __do_layout(self) -> None:
 		# begin wxGlade: border_config.__do_layout
 		parent_sizer = wx.BoxSizer(wx.VERTICAL)
 		main_sizer = wx.BoxSizer(wx.VERTICAL)
 		spinner_grid = wx.FlexGridSizer(4, 2, 4, 7)
 		borders_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Configure Borders")
-		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ""))
+		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ''))
 		main_sizer.Add(borders_label, 0, wx.BOTTOM, 7)
 		top_border_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Top: ")
 		spinner_grid.Add(top_border_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
 		spinner_grid.Add(self.top_border_value, 0, wx.ALIGN_CENTER_VERTICAL, 0)
 		bottom_border_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Bottom: ")
 		spinner_grid.Add(bottom_border_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
 		spinner_grid.Add(self.bottom_border_value, 0, wx.ALIGN_CENTER_VERTICAL, 0)
@@ -116,31 +125,32 @@
 		main_sizer.Add(self.close_btn, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT, 5)
 		self.main_panel.SetSizer(main_sizer)
 		parent_sizer.Add(self.main_panel, 1, wx.ALL | wx.EXPAND, 10)
 		self.SetSizer(parent_sizer)
 		parent_sizer.Fit(self)
 		self.Layout()
 		# end wxGlade
-	
-	def update_borders(self, event):  # wxGlade: border_config.<event_handler>
+
+	def update_borders(self, _) -> None:  # wxGlade: border_config.<event_handler>
 		self.chromatogram_figure.subplots_adjust(
-			self.left_border_value.GetValue(),
-			self.bottom_border_value.GetValue(),
-			self.right_border_value.GetValue(),
-			self.top_border_value.GetValue()
-		)
+				self.left_border_value.GetValue(),
+				self.bottom_border_value.GetValue(),
+				self.right_border_value.GetValue(),
+				self.top_border_value.GetValue()
+				)
 		self.chromatogram_figure.canvas.draw_idle()
-	
-	def apply_tight_layout(self, event):  # wxGlade: border_config.<event_handler>
+
+	def apply_tight_layout(self, _) -> None:  # wxGlade: border_config.<event_handler>
 		self.chromatogram_figure.tight_layout()
 		self.chromatogram_figure.canvas.draw_idle()
-		
+
 		# set SpinCtrls to new values
 		self.right_border_value.SetValue(self.chromatogram_figure.subplotpars.right)
 		self.left_border_value.SetValue(self.chromatogram_figure.subplotpars.left)
 		self.bottom_border_value.SetValue(self.chromatogram_figure.subplotpars.bottom)
 		self.top_border_value.SetValue(self.chromatogram_figure.subplotpars.top)
-	
-	def close_dialog(self, event):  # wxGlade: border_config.<event_handler>
+
+	def close_dialog(self, _) -> None:  # wxGlade: border_config.<event_handler>
 		self.Destroy()
 
+
 # end of class border_config
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/__init__.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
+
 #
 #  __init__.py
+"""
+Tools and widgets for wxPython.
+
+isort:skip_file
+"""
 #
 #  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
@@ -23,25 +28,35 @@
 #
 
 from domdf_wxpython_tools.border_config import border_config as BorderConfigDialog
 from domdf_wxpython_tools.chartpanel import ChartPanelBase
 from domdf_wxpython_tools.clearable_textctrl import ClearableTextCtrl
 from . import ColourPickerPanel  # TODO: ColourPickerPanel
 from domdf_wxpython_tools.dialogs import (
-	file_dialog_wildcard, file_dialog_multiple, file_dialog, FloatEntryDialog, IntEntryDialog, Wildcards,
-	)
+		file_dialog_wildcard,
+		file_dialog_multiple,
+		file_dialog,
+		FloatEntryDialog,
+		IntEntryDialog,
+		Wildcards,
+		)
 from domdf_wxpython_tools.editable_listbox import EditableListBox, CleverListCtrl, EditableNumericalListBox
 from domdf_wxpython_tools.events import PayloadEvent, SimpleEvent
 from domdf_wxpython_tools.filebrowsectrl import FileBrowseCtrl, FileBrowseCtrlWithHistory, DirBrowseCtrl
 from domdf_wxpython_tools.icons import get_button_icon, get_toolbar_icon, GetStockBitmap, GetStockToolbarBitmap
 from domdf_wxpython_tools.imagepanel import (
-	ID_ImagePanel_Copy_Image, ID_ImagePanel_Delete_Image, ID_ImagePanel_Load_Image,
-	ID_ImagePanel_Paste_Image, ID_ImagePanel_Reset_View, ID_ImagePanel_Save_Image,
-	EVT_IMAGE_PANEL_CHANGED, ImagePanel,
-	)
+		ID_ImagePanel_Copy_Image,
+		ID_ImagePanel_Delete_Image,
+		ID_ImagePanel_Load_Image,
+		ID_ImagePanel_Paste_Image,
+		ID_ImagePanel_Reset_View,
+		ID_ImagePanel_Save_Image,
+		EVT_IMAGE_PANEL_CHANGED,
+		ImagePanel,
+		)
 from domdf_wxpython_tools.keyboard import gen_keymap, NAVKEYS
 from . import list_dialog  # TODO: list_dialog
 from domdf_wxpython_tools.logctrl import LogCtrl
 from . import panel_listctrl
 from . import picker  # TODO: picker
 from domdf_wxpython_tools.projections import XPanAxes, XPanAxes_NoZoom, NoZoom
 from domdf_wxpython_tools.style_picker import style_picker as StylePickerDialog
@@ -49,15 +64,14 @@
 from . import StylePickerPanel  # TODO: StylePickerPanel
 from domdf_wxpython_tools.tabbable_textctrl import TabbableTextCtrl
 from domdf_wxpython_tools.timer_thread import Timer
 from domdf_wxpython_tools.utils import toggle, coming_soon, collapse_label, generate_faces
 from domdf_wxpython_tools.validators import ValidatorBase, FloatValidator, CharValidator
 # TODO: WebView
 
-
 __all__ = [
 		"BorderConfigDialog",
 		"ChartPanelBase",
 		"ClearableTextCtrl",
 		"ColourPickerPanel",
 		"file_dialog_wildcard",
 		"file_dialog_multiple",
@@ -110,17 +124,16 @@
 		"EditableListBox",
 		"CleverListCtrl",
 		"EditableNumericalListBox",
 		"StylePickerDialog",
 		"ColourPickerDialog",
 		"__author__",
 		"__version__",
-		"__copyright__"
-]
+		"__copyright__",
+		]
 
 __author__ = "Dominic Davis-Foster"
 __copyright__ = "Copyright 2019-2020 Dominic Davis-Foster"
 
 __license__ = "LGPL"
 __version__ = "0.2.5"
 __email__ = "dominic@davis-foster.co.uk"
-
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/list_dialog.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/list_dialog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1 +1,153 @@
-#!/usr/bin/env python# -*- coding: utf-8 -*-##  list_dialog.py##  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>##  This program is free software; you can redistribute it and/or modify#  it under the terms of the GNU Lesser General Public License as published by#  the Free Software Foundation; either version 3 of the License, or#  (at your option) any later version.##  This program is distributed in the hope that it will be useful,#  but WITHOUT ANY WARRANTY; without even the implied warranty of#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#  GNU Lesser General Public License for more details.##  You should have received a copy of the GNU Lesser General Public License#  along with this program; if not, write to the Free Software#  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,#  MA 02110-1301, USA.### generated by wxGlade 0.9.3 on Wed Jun 12 18:14:39 2019#import wx# begin wxGlade: dependencies# end wxGlade# begin wxGlade: extracode# end wxGladeclass list_dialog(wx.Dialog):	"""	A dialog containing a wx.ListBox	"""		def __init__(			self, parent, id=wx.ID_ANY,			title='Choose', label="Choose: ", choices=None,			pos=wx.DefaultPosition, size=wx.DefaultSize,			style=wx.DEFAULT_DIALOG_STYLE, name=wx.DialogNameStr			):				"""		:param parent: The parent window. Can be None, a frame or another dialog box		:type parent: wx.Window		:param id: An identifier for the dialog. wx.ID_ANY is taken to mean a default.		:type id: wx.WindowID, optional		:param title: The title of the dialog		:type title: str, optional		:param label: The label for the wx.ListBox		:type label: str, optional		:param choices: A list of choices for the wx.ListBox		:type choices: list of str		:param pos: The dialog position. The value ::wxDefaultPosition indicates a default position, chosen by either the windowing system or wxWidgets, depending on platform.		:type pos: wx.Point, optional		:param size: The dialog size. The value ::wxDefaultSize indicates a default size, chosen by either the windowing system or wxWidgets, depending on platform.		:type size: wx.Size, optional		:param style: The window style. See wxPanel.		:type style: int, optional		:param name: Window name.		:type name: str, optional		"""				if choices is None:			choices = [					"egg and bacon",					"egg sausage and bacon",					"egg and spam",					"egg bacon and spam",					"egg bacon sausage and spam",					"spam bacon sausage and spam",					"spam egg spam spam bacon and spam",					"spam sausage spam spam bacon spam tomato and spam",					"spam spam spam egg and spam",					"spam spam spam spam spam spam baked beans spam spam spam",					]					self.title = title		self.label = label		self.choices = choices				args = (parent, id)		kwds = dict(pos=pos, size=size, style=style, name=name)				# begin wxGlade: list_dialog.__init__		kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_DIALOG_STYLE		wx.Dialog.__init__(self, *args, **kwds)		self.SetSize((512, -1))		self.main_panel = wx.Panel(self, wx.ID_ANY)		self.list_box = wx.ListBox(self.main_panel, wx.ID_ANY, choices=[])		self.cancel_btn = wx.Button(self.main_panel, wx.ID_CANCEL, "")		self.select_btn = wx.Button(self.main_panel, wx.ID_ANY, "Select")				self.__set_properties()		self.__do_layout()				self.Bind(wx.EVT_LISTBOX_DCLICK, self.do_select, self.list_box)		self.Bind(wx.EVT_BUTTON, self.do_select, self.select_btn)		# end wxGlade		self.list_box.Clear()		self.list_box.AppendItems(choices)		def __set_properties(self):		# begin wxGlade: list_dialog.__set_properties		self.SetTitle("Choose")		self.SetSize((512, -1))		# end wxGlade		self.SetTitle(self.title)		def __do_layout(self):		# begin wxGlade: list_dialog.__do_layout		parent_sizer = wx.BoxSizer(wx.VERTICAL)		main_sizer = wx.BoxSizer(wx.VERTICAL)		btn_sizer = wx.GridSizer(1, 2, 0, 7)		borders_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Choose: ")		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ""))		main_sizer.Add(borders_label, 0, wx.BOTTOM, 7)		main_sizer.Add(self.list_box, 1, wx.EXPAND, 0)		static_line_10 = wx.StaticLine(self.main_panel, wx.ID_ANY)		main_sizer.Add(static_line_10, 0, wx.BOTTOM | wx.EXPAND | wx.TOP, 5)		btn_sizer.Add(self.cancel_btn, 0, wx.ALIGN_CENTER, 0)		btn_sizer.Add(self.select_btn, 0, wx.ALIGN_CENTER, 0)		main_sizer.Add(btn_sizer, 0, wx.ALIGN_BOTTOM | wx.ALIGN_RIGHT, 0)		self.main_panel.SetSizer(main_sizer)		parent_sizer.Add(self.main_panel, 1, wx.ALL | wx.EXPAND, 10)		self.SetSizer(parent_sizer)		self.Layout()		# end wxGlade		borders_label.SetLabel(self.label)		def do_select(self, event):  # wxGlade: list_dialog.<event_handler>		"""Event Handler for item in list being selected"""		self.EndModal(wx.ID_OK)		def do_cancel(self, event):  # wxGlade: list_dialog.<event_handler>		"""Event Handler for dialog being cancelled"""		self.Destroy()# end of class list_dialog
+#!/usr/bin/env python
+#
+#  list_dialog.py
+#
+#  Copyright 2019-2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#
+#  This program is free software; you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published by
+#  the Free Software Foundation; either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License
+#  along with this program; if not, write to the Free Software
+#  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
+#  MA 02110-1301, USA.
+#
+#
+# generated by wxGlade 0.9.3 on Wed Jun 12 18:14:39 2019
+#
+
+# stdlib
+from typing import List, Optional
+
+# 3rd party
+import wx  # type: ignore
+
+__all__ = ["list_dialog"]
+
+# begin wxGlade: dependencies
+
+# end wxGlade
+
+# begin wxGlade: extracode
+# end wxGlade
+
+
+class list_dialog(wx.Dialog):
+	"""
+	A dialog containing a :class:`wx.ListBox`.
+
+	:param parent: The parent window. Can be None, a frame or another dialog box
+	:param id: An identifier for the dialog. :py:obj:`wx.ID_ANY` is taken to mean a default.
+	:param title: The title of the dialog
+	:param label: The label for the :class:`wx.ListBox`.
+	:param choices: A list of choices for the wx.ListBox
+	:param pos: The dialog position. The value :py:obj:`wx.DefaultPosition` indicates a default position,
+		chosen by either the windowing system or wxWidgets, depending on platform.
+	:param size: The dialog size. The value ::wxDefaultSize indicates a default size,
+		chosen by either the windowing system or wxWidgets, depending on platform.
+	:param style: The window style. See wxPanel.
+	:param name: Window name.
+	"""
+
+	def __init__(
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			title: str = "Choose",
+			label: str = "Choose: ",
+			choices: Optional[List[str]] = None,
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = wx.DEFAULT_DIALOG_STYLE,
+			name: str = wx.DialogNameStr
+			):
+		if choices is None:
+			choices = [
+					"egg and bacon",
+					"egg sausage and bacon",
+					"egg and spam",
+					"egg bacon and spam",
+					"egg bacon sausage and spam",
+					"spam bacon sausage and spam",
+					"spam egg spam spam bacon and spam",
+					"spam sausage spam spam bacon spam tomato and spam",
+					"spam spam spam egg and spam",
+					"spam spam spam spam spam spam baked beans spam spam spam",
+					]
+
+		self.title = title
+		self.label = label
+		self.choices = choices
+
+		args = (parent, id)
+		kwds = dict(pos=pos, size=size, style=style, name=name)
+
+		# begin wxGlade: list_dialog.__init__
+		kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_DIALOG_STYLE
+		wx.Dialog.__init__(self, *args, **kwds)
+		self.SetSize((512, -1))
+		self.main_panel = wx.Panel(self, wx.ID_ANY)
+		self.list_box = wx.ListBox(self.main_panel, wx.ID_ANY, choices=[])
+		self.cancel_btn = wx.Button(self.main_panel, wx.ID_CANCEL, '')
+		self.select_btn = wx.Button(self.main_panel, wx.ID_ANY, "Select")
+
+		self.__set_properties()
+		self.__do_layout()
+
+		self.Bind(wx.EVT_LISTBOX_DCLICK, self.do_select, self.list_box)
+		self.Bind(wx.EVT_BUTTON, self.do_select, self.select_btn)
+		# end wxGlade
+		self.list_box.Clear()
+		self.list_box.AppendItems(choices)
+
+	def __set_properties(self) -> None:
+		# begin wxGlade: list_dialog.__set_properties
+		self.SetTitle("Choose")
+		self.SetSize((512, -1))
+		# end wxGlade
+		self.SetTitle(self.title)
+
+	def __do_layout(self) -> None:
+		# begin wxGlade: list_dialog.__do_layout
+		parent_sizer = wx.BoxSizer(wx.VERTICAL)
+		main_sizer = wx.BoxSizer(wx.VERTICAL)
+		btn_sizer = wx.GridSizer(1, 2, 0, 7)
+		borders_label = wx.StaticText(self.main_panel, wx.ID_ANY, "Choose: ")
+		borders_label.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ''))
+		main_sizer.Add(borders_label, 0, wx.BOTTOM, 7)
+		main_sizer.Add(self.list_box, 1, wx.EXPAND, 0)
+		static_line_10 = wx.StaticLine(self.main_panel, wx.ID_ANY)
+		main_sizer.Add(static_line_10, 0, wx.BOTTOM | wx.EXPAND | wx.TOP, 5)
+		btn_sizer.Add(self.cancel_btn, 0, wx.ALIGN_CENTER, 0)
+		btn_sizer.Add(self.select_btn, 0, wx.ALIGN_CENTER, 0)
+		main_sizer.Add(btn_sizer, 0, wx.ALIGN_BOTTOM | wx.ALIGN_RIGHT, 0)
+		self.main_panel.SetSizer(main_sizer)
+		parent_sizer.Add(self.main_panel, 1, wx.ALL | wx.EXPAND, 10)
+		self.SetSizer(parent_sizer)
+		self.Layout()
+		# end wxGlade
+		borders_label.SetLabel(self.label)
+
+	def do_select(self, _) -> None:  # wxGlade: list_dialog.<event_handler>
+		"""
+		Event Handler for item in list being selected
+		"""
+
+		self.EndModal(wx.ID_OK)
+
+	def do_cancel(self, _) -> None:  # wxGlade: list_dialog.<event_handler>
+		"""
+		Event Handler for dialog being cancelled
+		"""
+
+		self.Destroy()
+
+
+# end of class list_dialog
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/clearable_textctrl.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/clearable_textctrl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
-#   -*- coding: utf-8 -*-
 #
 #  ClearableTextCtrl.py
 """
 A TextCtrl with a button to clear its contents
 """
 #
 #  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
-#  Adapted from src/generic/srchctlg.cpp (part of wxWidgets, https://github.com/wxWidgets/wxWidgets)
+#  Adapted from src/generic/srchctlg.cpp
+#  Part of wxWidgets, https://github.com/wxWidgets/wxWidgets
 #  Copyright (c) 2006 Vince Harron.
 #  Licenced under the wxWindows licence
 #
-#
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -25,82 +24,92 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
+# stdlib
+from typing import List, Tuple
+
 # 3rd party
-import wx
-from wx.lib.embeddedimage import PyEmbeddedImage
+import wx  # type: ignore
+
+# this package
+from domdf_wxpython_tools.textctrlwrapper import TextCtrlWrapper
+
+__all__ = ["CTCWidget", "ClearButton", "ClearableTextCtrl", "clear_btn"]
 
 # the margin between the text control and the clear button
 MARGIN = 3
 
 # arguments to wxColour::ChangeLightness() for making the search/clear
 # bitmaps foreground colour, respectively
 CANCEL_BITMAP_LIGHTNESS = 16  # a bit more lighter
 
-
 ClearableTextCtrlNameStr = "ClearableTextCtrl"
 
 
 class CTCWidget(wx.TextCtrl):
 	"""
-	CTCWidget: text control used by ClearableTextCtrl
+	Text control used by :class:`~.ClearableTextCtrl`.
+
+	:param parent: The parent window.
+	:param value: The initial value of the text control
+	:param style: The style of the text control
+	:param validator:
 	"""
-	
-	def __init__(self, parent, value, style, validator):
-		"""
-		:param parent: The parent window.
-		:type parent: ClearableTextCtrl
-		:param value: The initial value of the text control
-		:type value: str
-		:param style: The style of the text control
-		:type style: int
-		"""
-		
+
+	def __init__(self, parent: "ClearableTextCtrl", value: str, style: int, validator):
 		wx.TextCtrl.__init__(self, parent, value=value, style=style, validator=validator)
 		self.parent = parent
-		
+
 		# Ensure that our best size is recomputed using our overridden DoGetBestSize()
 		self.InvalidateBestSize()
-		
+
 		self.Bind(wx.EVT_TEXT, self.OnText, id=wx.ID_ANY)
 		self.Bind(wx.EVT_TEXT_ENTER, self.OnTextEnter, id=wx.ID_ANY)
 		self.Bind(wx.EVT_TEXT_MAXLEN, self.OnText, id=wx.ID_ANY)
-		
-	def GetMainWindowOfCompositeControl(self):
+
+	def GetMainWindowOfCompositeControl(self) -> "ClearableTextCtrl":
+		"""
+		Returns the parent object.
+		"""
+
 		return self.parent
-	
-	def OnText(self, event):
+
+	def OnText(self, event) -> None:
 		"""
-		Event handler for text being entered in the control
+		Event handler for text being entered in the control.
+
+		:param event: The wxPython event.
 		"""
-		
+
 		event = wx.CommandEvent(event)
 		event.SetEventObject(self.parent)
 		event.SetId(self.parent.GetId())
-		
+
 		self.parent.GetEventHandler().ProcessEvent(event)
-	
-	def OnTextEnter(self, event):
+
+	def OnTextEnter(self, _) -> None:
 		"""
-		Event handler for the enter/return key being pressed
+		Event handler for the :kbd:`enter` / :kbd:`return ⏎` key being pressed
+
+		:param event: The wxPython event.
 		"""
-		
+
 		if not self.IsEmpty():
 			event = wx.CommandEvent(wx.EVT_SEARCHCTRL_SEARCH_BTN, self.parent.GetId)
 			event.SetEventObject(self.parent)
 			event.SetString(self.parent.GetValue())
-			
+
 			self.parent.ProcessWindowEvent(event)
-	
+
 	"""
-	
+
 #ifdef __WXMSW__
 	# We increase the text control height to be the same as for the controls
 	# with border as this is what we actually need here because even though
 	# this control itself is borderless, it's inside wxClearableTextCtrl which does
 	# have the border and so should have the same height as the normal text
 	# entries with border.
 	#
@@ -128,479 +137,393 @@
 
 		self.SetWindowStyleFlag(flags)
 
 		return size
 	}
 #endif # __WXMSW__"""
 
-#b"                       ",
 
-clear_btn = [
-	b"25 19 2 1",
-	b"   c None",
-	b"+  c #000000",
-	b"                         ",
-	b"                         ",
-	b"                         ",
-	b"                         ",
-	b"                         ",
-	b"                         ",
-	b"         +++++++++++++   ",
-	b"        ++           +   ",
-	b"       ++    +   +   +   ",
-	b"      ++      + +    +   ",
-	b"     ++        +     +   ",
-	b"      ++      + +    +   ",
-	b"       ++    +   +   +   ",
-	b"        ++           +   ",
-	b"         +++++++++++++   ",
-	b"                         ",
-	b"                         ",
-	b"                         ",
-	b"                         ",
-	b"                         ",
+#: XPM button icon for clearing the text control.
+clear_btn: List[bytes] = [
+		b"25 19 2 1",
+		b"   c None",
+		b"+  c #000000",
+		b"                         ",
+		b"                         ",
+		b"                         ",
+		b"                         ",
+		b"                         ",
+		b"                         ",
+		b"         +++++++++++++   ",
+		b"        ++           +   ",
+		b"       ++    +   +   +   ",
+		b"      ++      + +    +   ",
+		b"     ++        +     +   ",
+		b"      ++      + +    +   ",
+		b"       ++    +   +   +   ",
+		b"        ++           +   ",
+		b"         +++++++++++++   ",
+		b"                         ",
+		b"                         ",
+		b"                         ",
+		b"                         ",
+		b"                         ",
 		]
 
 
 class ClearButton(wx.Control):
 	"""
-	Clear button for the ClearableTextCtrl
+	Clear button for the :class:`~.ClearableTextCtrl`.
+
+	:param parent: The parent window.
+	:param eventType:
+	:param bmp:
 	"""
-	def __init__(self, parent, eventType, bmp):
-		"""
-		:param parent: The parent window.
-		:type parent: ClearableTextCtrl
-		:param eventType:
-		:type eventType:wx.PyEventBinder
-		:param bmp:
-		:type bmp: wx.Bitmap
-		"""
-		
+
+	def __init__(self, parent: "ClearableTextCtrl", eventType: wx.PyEventBinder, bmp: wx.Bitmap):
+
 		wx.Control.__init__(self, parent, id=wx.ID_ANY, style=wx.NO_BORDER)
 		self.parent = parent
 		self.m_eventType = eventType.typeId
 		self.m_bmp = bmp
-		
+
 		self.SetBackgroundStyle(wx.BG_STYLE_PAINT)
-		
+
 		self.Bind(wx.EVT_LEFT_UP, self.OnLeftUp)
 		self.Bind(wx.EVT_PAINT, self.OnPaint)
-		
-	def SetBitmapLabel(self, label):
+
+	def SetBitmapLabel(self, label: wx.Bitmap) -> None:
 		"""
-		Set bitmap for the button
-		
-		:param label: Bitmap to set for the button
-		:type label: wx.Bitmap
+		Set bitmap for the button.
+
+		:param label: Bitmap to set for the button.
 		"""
-		
+
 		self.m_bmp = label
 		self.InvalidateBestSize()
-	
+
 	# The buttons in ClearableTextCtrl shouldn't accept focus from keyboard because
 	# this would interfere with the usual TAB processing: the user expects
 	# that pressing TAB in the search control should switch focus to the next
 	# control and not give it to the button inside the same control.
-	def AcceptsFocusFromKeyboard(self):
+	def AcceptsFocusFromKeyboard(self) -> bool:
+		"""
+		Always returns :py:obj:`False`.
+		"""
+
 		return False
-	
-	def GetMainWindowOfCompositeControl(self):
+
+	def GetMainWindowOfCompositeControl(self) -> "ClearableTextCtrl":
+		"""
+		Returns the parent object.
+		"""
+
 		return self.parent
-	
-	def GetBestSize(self):
+
+	def GetBestSize(self) -> wx.Size:
+		"""
+		Returns the best size for the control.
+		"""
+
 		return wx.Size(self.m_bmp.GetWidth(), self.m_bmp.GetHeight())
-	
-	def OnLeftUp(self, event):
+
+	def OnLeftUp(self, _) -> None:
 		"""
-		Event Handler for left mouse button being released
+		Event Handler for left mouse button being released.
 		"""
-		
+
 		event = wx.CommandEvent(self.m_eventType, self.parent.GetId())
 		event.SetEventObject(self.parent)
-		
+
 		if self.m_eventType == wx.EVT_SEARCHCTRL_SEARCH_BTN.typeId:
 			# it's convenient to have the string to search for directly in the
 			# event instead of having to retrieve it from the control in the
 			# event handler code later, so provide it here
 			event.SetString(self.parent.GetValue())
-		
+
 		self.GetEventHandler().ProcessEvent(event)
-		
+
 		self.parent.SetFocus()
-		
-	def OnPaint(self, event):
+
+	def OnPaint(self, _) -> None:
 		"""
-		Event Handler for widget being painted
+		Event Handler for widget being painted.
 		"""
-		
+
 		dc = wx.PaintDC(self)
-		
+
 		# Clear the background in case of a user bitmap with alpha channel
 		dc.GetBrush().SetColour(self.parent.GetBackgroundColour())
-		#dc.SetBrush(self.parent.GetBackgroundColour())
+		# dc.SetBrush(self.parent.GetBackgroundColour())
 		dc.Clear()
-		
+
 		# Draw the bitmap
 		dc.DrawBitmap(self.m_bmp, 0, 0, True)
-		
 
-class ClearableTextCtrl(wx.Panel):
+
+class ClearableTextCtrl(TextCtrlWrapper, wx.Panel):
 	"""
-	TextCtrl with button to clear its contents
+	TextCtrl with a button to clear its contents.
+
+	:param parent: The parent window.
+	:param id: An identifier for the control. :py:obj:`wx.ID_ANY` is taken to mean a default.
+	:param value: Default text value.
+	:param pos: The control position. The value :py:obj:`wx.DefaultPosition` indicates a default position,
+		chosen by either the windowing system or wxWidgets, depending on platform.
+	:param size: The control size. The value wx.DefaultSize indicates a default size,
+		chosen by either the windowing system or wxWidgets, depending on platform.
+	:param style: The window style. See :class:`wx.TextCtrl`.
+	:param validator: Window validator.
+	:param name: Window name.
 	"""
-	
+
 	def __init__(
-			self, parent, id=wx.ID_ANY, value="", pos=wx.DefaultPosition,
-			size=wx.DefaultSize, style=0, validator=wx.DefaultValidator,
-			name=ClearableTextCtrlNameStr
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			value: str = '',
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = 0,
+			validator: wx.Validator = wx.DefaultValidator,
+			name: str = ClearableTextCtrlNameStr
 			):
-		"""
-		:param parent: The parent window.
-		:type parent: wx.Window
-		:param id: An identifier for the control. wx.ID_ANY is taken to mean a default.
-		:type id: wx.WindowID, optional
-		:param value: Default text value
-		:type value: str
-		:param pos: The control position. The value wx.DefaultPosition indicates a default position, chosen by either the windowing system or wxWidgets, depending on platform.
-		:type pos: wx.Point, optional
-		:param size: The control size. The value wx.DefaultSize indicates a default size, chosen by either the windowing system or wxWidgets, depending on platform.
-		:type size: wx.Size, optional
-		:param style: The window style. See wx.TextCtrl.
-		:type style: int, optional
-		:param validator: Window validator
-		:type validator: wx.Validator, optional
-		:param name: Window name.
-		:type name: str, optional
-		"""
-		
+
 		wx.Panel.__init__(self, parent, id, pos, size, style | wx.BORDER_SUNKEN, name)
-		
+
 		textctrl_style = style | wx.TAB_TRAVERSAL | wx.BORDER_NONE | wx.TE_RICH2
-		
+
 		if wx.Platform == "__WXGTK__":
-			print(122)
 			# wx.BORDER_NONE doesn't work unless its a multiline textctrl
 			textctrl_style |= wx.TE_MULTILINE | wx.TE_DONTWRAP
-		
-		self.m_text = CTCWidget(self, value, textctrl_style, validator=validator)
+
+		self.textctrl = self.m_text = CTCWidget(self, value, textctrl_style, validator=validator)
 		self.m_clearBitmap = self.default_clear_bitmap
 		self.m_clearButton = ClearButton(self, wx.EVT_SEARCHCTRL_CANCEL_BTN, self.m_clearBitmap)
 		self.m_clearButton.SetSize((16, 16))
 		self.LayoutControls()
-		
+
 		self.SetBackgroundColour(self.m_text.GetBackgroundColour())
 		# self.m_text.SetBackgroundColour(wx.Colour())
-		
+
 		self.SetInitialSize(size)
 		self.SetMinSize((-1, 29))
 		self.Move(pos)
 
 		self.Bind(wx.EVT_SEARCHCTRL_CANCEL_BTN, self.OnClearButton, id=wx.ID_ANY)
 		self.Bind(wx.EVT_SIZE, self.OnSize)
-		
+
 	# def Destroy(self):
 	# 	self.m_text.Destroy()
 	# 	self.m_clearButton.Destroy()
 	# 	wx.Control.Destroy(self)
-	
+
 	@property
-	def default_clear_bitmap(self):
+	def default_clear_bitmap(self) -> wx.Bitmap:
 		"""
-		Returns the default clear button bitmap for the control
-
-		:rtype: wx.Bitmap
+		Returns the default clear button bitmap for the control.
 		"""
-		
-		#return Clear_Button_16.GetBitmap()
+
+		# return Clear_Button_16.GetBitmap()
 		return wx.Bitmap(clear_btn)
-	
-	def SetFont(self, font):
+
+	def SetFont(self, font: wx.Font) -> bool:
 		"""
-		Sets the font for the control
-		
-		:param font: Font to associate with this control, pass wx.NullFont to reset to the default font.
-		:type font: wx.Font
-		
-		:return: True if the operation completes successfully, False otherwise
-		:rtype: bool
+		Sets the font for the control.
+
+		:param font: Font to associate with this control.
+			Pass ``wx.NullFont`` to reset to the default font.
+
+		:return: :py:obj:`True` if the operation completes successfully,
+			:py:obj:`False` otherwise.
 		"""
-		
+
 		if not self.m_text.SetFont(font):
 			return False
-	
+
 		# TODO: Recreate the bitmaps as their size may have changed.
 
 		return True
-	
-	def SetBackgroundColour(self, colour):
+
+	def SetBackgroundColour(self, colour: wx.Colour) -> bool:
 		"""
 		Sets the background colour of the control
-		
-		:param colour: The colour to be used as the background colour; pass wx.NullColour to reset to the default colour.
-		:type colour: wx.Colour
-		
+
+		:param colour: The colour to be used as the background colour; pass :py:obj:`wx.NullColour`.
+			to reset to the default colour.
+
 		.. note::
-		
-			You may want to use wx.SystemSettings.GetColour to retrieve a
+
+			You may want to use ``wx.SystemSettings.GetColour`` to retrieve a
 			suitable colour to use rather than setting an hard-coded one.
-		
-		:return: True if the operation completes successfully, False otherwise
-		:rtype: bool
-		"""
-		
-		if not all([
-				self.m_text.SetBackgroundColour(colour),
-				wx.Window.SetBackgroundColour(self, colour)
-				]):
+
+		:return: :py:obj:`True` if the operation completes successfully,
+			:py:obj:`False` otherwise.
+		"""
+
+		if not all([self.m_text.SetBackgroundColour(colour), wx.Window.SetBackgroundColour(self, colour)]):
 			return False
-	
+
 		# TODO: When the background changes, re-render the bitmaps so that the correct
 		#  colour shows in their "transparent" area.
 
 		return True
-	
-	def AppendText(self, text):
-		"""
-		Appends the text to the end of the text control.
-
-		.. note::
-			
-			After the text is appended, the insertion point will be at the end of the text control.
-			If this behaviour is not desired, the programmer should use GetInsertionPoint and SetInsertionPoint.
 
-		:param text: Text to write to the text control.
-		:type text:	str
-		"""
-
-		self.m_text.AppendText(text)
-	
-	def AutoComplete(self, completer):
+	def AutoComplete(self, completer: wx.TextCompleter) -> bool:
 		"""
 		Enable auto-completion using the provided completer object.
 
-		The specified completer object will be used to retrieve the list of possible completions for the already entered text and will be deleted by wx.TextEntry itself when it’s not needed any longer.
-		
-		:param completer: The object to be used for generating completions if not None. If it is None, auto-completion is disabled. The wx.TextEntry object takes ownership of this pointer and will delete it in any case (i.e. even if this method return False).
-		:type completer: wx.TextCompleter
-		
-		:return: True if the auto-completion was enabled or False if the operation failed, typically because auto-completion is not supported by the current platform.
-		:rtype: bool
+		The specified completer object will be used to retrieve the list of possible
+		completions for the already entered text and will be deleted by :class:`wx.TextEntry`
+		itself when it's not needed any longer.
+
+		:param completer: The object to be used for generating completions if not :py:obj:`None`.
+			If it is :py:obj:`None`, auto-completion is disabled. The :class:`wx.TextEntry` object
+			takes ownership of this pointer and will delete it in any case
+			(i.e. even if this method return :py:obj:`False`).
+
+		:return: :py:obj:`True` if the auto-completion was enabled or :py:obj:`False`
+			if the operation failed, typically because auto-completion is not supported by the current platform.
 		"""
 
 		return self.m_text.AutoComplete(completer)
-		
-	def AutoCompleteDirectories(self):
+
+	def AutoCompleteDirectories(self) -> bool:
 		"""
 		Call this function to enable auto-completion of the text using the file system directories.
 
-		Unlike AutoCompleteFileNames which completes both file names and directories, this function only completes the directory names.
-		
-		Notice that currently this function is only implemented in wxMSW port and does nothing under the other platforms.
-		
-		:return: True if the auto-completion was enabled or False if the operation failed, typically because auto-completion is not supported by the current platform.
-		:rtype: bool
+		Unlike :meth:`~.ClearableTextCtrl.AutoCompleteFileNames`, which completes both file names and directories,
+		this function only completes the directory names.
+
+		.. note:: This function is only implemented in wxMSW port and does nothing under the other platforms.
+
+		:return: :py:obj:`True` if the auto-completion was enabled or :py:obj:`False` if the
+			operation failed, typically because auto-completion is not supported by the current platform.
 		"""
-	
+
 		return self.m_text.AutoCompleteDirectories()
-		
-	def AutoCompleteFileNames(self):
+
+	def AutoCompleteFileNames(self) -> bool:
 		"""
-		Call this function to enable auto-completion of the text typed in a single-line text control using all valid file system paths.
+		Call this function to enable auto-completion of the text typed in a single-line text control
+		using all valid file system paths.
 
-		Notice that currently this function is only implemented in wxMSW port and does nothing under the other platforms.
-		
-		:return: True if the auto-completion was enabled or False if the operation failed, typically because auto-completion is not supported by the current platform.
-		:rtype: bool
+		.. note:: This function is only implemented in wxMSW port and does nothing under the other platforms.
+
+		:return: :py:obj:`True` if the auto-completion was enabled or :py:obj:`False`
+			if the operation failed, typically because auto-completion is not supported by the current platform.
 		"""
-	
+
 		return self.m_text.AutoCompleteFileNames()
-	
-	def CanCopy(self):
-		"""
-		:return: True if the selection can be copied to the clipboard.
-		:rtype:	bool
-		"""
-		
-		return self.m_text.CanCopy()
-	
-	def CanCut(self):
-		"""
-		:return: True if the selection can be cut to the clipboard.
-		:rtype:	bool
-		"""
-		
-		return self.m_text.CanCut()
-	
-	def CanPaste(self):
-		"""
-		:return: True if the contents of the clipboard can be pasted into the text control.
-		:rtype:	bool
-		
-		On some platforms (Motif, GTK) this is an approximation and returns True if the control is editable, False otherwise.
-		"""
-		
-		return self.m_text.CanPaste()
-	
-	def CanRedo(self):
-		"""
-		:return: True if there is a redo facility available and the last operation can be redone.
-		:rtype: bool
-		"""
-		
-		return self.m_text.CanRedo()
-	
-	def CanUndo(self):
-		"""
-		:return: True if there is an undo facility available and the last operation can be undone.
-		:rtype: bool
-		"""
-		
-		return self.m_text.CanUndo()
-	
-	def ChangeValue(self, value):
+
+	def ChangeValue(self, value: str):
 		"""
 		Sets the new text control value.
 
-		It also marks the control as not-modified which means that IsModified() would return False immediately after the call to ChangeValue .
-		
+		It also marks the control as not-modified which means that :meth:`~.ClearableTextCtrl.IsModified`
+		would return :py:obj:`False` immediately after the call to :meth:`~.ClearableTextCtrl.ChangeValue`.
+
 		The insertion point is set to the start of the control (i.e. position 0) by this function.
-		
-		This functions does not generate the wxEVT_TEXT event but otherwise is identical to SetValue .
-		
-		See User Generated Events vs Programmatically Generated Events for more information.
-		
-		:param value: The new value to set. It may contain newline characters if the text control is multi-line
-		:type value: str
+
+		This functions does not generate the :py:obj:`wx.wxEVT_TEXT` event but otherwise is identical to
+		:meth:`~.ClearableTextCtrl.SetValue`.
+
+		:param value: The new value to set. It may contain newline characters if the text control is multiline.
 		"""
-		
+
 		self.m_text.ChangeValue(value)
-	
-	def Clear(self):
-		"""
-		Clears the text in the control.
 
-		Note that this function will generate a wxEVT_TEXT event, i.e. its effect is identical to calling SetValue (“”).
+	def DiscardEdits(self) -> None:
 		"""
-		
-		self.m_text.Clear()
-	
-	def Copy(self):
-		"""Copies the selected text to the clipboard."""
-		
-		self.m_text.Copy()
-	
-	def Cut(self):
-		"""Copies the selected text to the clipboard and removes it from the control."""
-		
-		self.m_text.Cut()
-	
-	def DiscardEdits(self):
-		"""Resets the internal modified flag as if the current changes had been saved."""
-		
+		Resets the internal modified flag as if the current changes had been saved.
+		"""
+
 		self.m_text.DiscardEdits()
-	
-	def EmulateKeyPress(self, event):
+
+	def EmulateKeyPress(self, event: wx.KeyEvent) -> bool:
 		"""
-		This function inserts into the control the character which would have been inserted if the given key event had occurred in the text control.
+		Inserts into the control the character which would have been inserted if the given
+		key event had occurred in the text control.
 
-		The event object should be the same as the one passed to EVT_KEY_DOWN handler previously by wxWidgets. Please note that this function doesn’t currently work correctly for all keys under any platform but MSW.
+		The event object should be the same as the one passed to :py:obj:`wx.EVT_KEY_DOWN` handler
+		previously by wxWidgets.
+
+		.. note:: This function doesn't currently work correctly for all keys under any platform but MSW.
 
 		:param event:
-		:type event: wx.KeyEvent
-		
-		:return: True if the event resulted in a change to the control, False otherwise.
-		:rtype: bool
+
+		:return: :py:obj:`True` if the event resulted in a change to the control, :py:obj:`False` otherwise.
 		"""
-		
+
 		return self.m_text.EmulateKeyPress(event)
-	
-	def GetBestClientSize(self):
-		"""
 
-		:return:
-		:rtype:	wx.Size
+	def GetBestClientSize(self) -> wx.Size:
 		"""
-		
+		Returns the best size for the control.
+		"""
+
 		size = self.m_text.GetBestSize()
-		
+
 		if self.IsClearButtonVisible():
 			size.x += self.m_clearButton.GetBestSize().x + self.FromDIP(MARGIN)
-		
+
 		# horizontalBorder = FromDIP(1) + (size.y - size.y * 14 / 21 ) / 2
 		horizontalBorder = (size.y - size.y * 14 / 21) / 2
 		size.x += 2 * horizontalBorder
-		
+
 		return size
-	
-	def GetCompositeWindowParts(self):
-		"""
 
-		:return:
-		:rtype:	wxWindowList
+	def GetCompositeWindowParts(self) -> List[wx.Window]:
 		"""
-		
+		Returns a list of :class:`wx.Window` objects that make up this control.
+		"""
+
 		return [self.m_text, self.m_clearButton]
-	
-	def GetDefaultStyle(self):
+
+	def GetDefaultStyle(self) -> wx.TextAttr:
 		"""
-		:return: The style currently used for the new text.
-		:rtype: wx.TextAttr
+		Returns the style currently used for new text.
 		"""
-		
+
 		return self.m_text.GetDefaultStyle()
-	
-	def GetInsertionPoint(self):
+
+	def GetInsertionPoint(self) -> int:
 		"""
 		Returns the insertion point, or cursor, position.
 
-		This is defined as the zero based index of the character position to the right of the insertion point. For example, if the insertion point is at the end of the single-line text control, it is equal to GetLastPosition .
-
-		:return:
-		:rtype:	int
+		This is defined as the zero based index of the character position
+		to the right of the insertion point.
+		For example, if the insertion point is at the end of the single-line text control,
+		it is equal to :meth:`~.ClearableTextCtrl.GetLastPosition`.
 		"""
-		
+
 		return self.m_text.GetInsertionPoint()
-	
-	def GetLastPosition(self):
-		"""
-		Returns the zero based index of the last position in the text control, which is equal to the number of characters in the control.
 
-		:return:
-		:rtype: wx.TextPos
-		"""
-		return self.m_text.GetLastPosition()
-	
-	def GetLineLength(self, lineNo):
+	def GetLineLength(self, lineNo: int) -> int:
 		"""
 		Gets the length of the specified line, not including any trailing newline character(s).
-		
+
 		:param lineNo: Line number (starting from zero).
-		:type lineNo: int
 
 		:return: The length of the line, or -1 if lineNo was invalid.
-		:rtype:	int
 		"""
-		
+
 		return self.m_text.GetLineLength(lineNo)
-	
-	def GetLineText(self, lineNo):
+
+	def GetLineText(self, lineNo: int) -> str:
 		"""
 		Returns the contents of a given line in the text control, not including any trailing newline character(s).
-		
-		:param lineNo: Line number (starting from zero).
-		:type lineNo: int
 
-		:return: The contents of the line.
-		:rtype:	str
+		:param lineNo: Line number (starting from zero).
 		"""
-		
+
 		return self.m_text.GetLineText(lineNo)
-	
+
 	# GetMargins
-	
+
 	# @staticmethod
 	# def GetMultiplier():
 	# 	"""
 	# 	Icons are rendered at 3-8 times larger than necessary and downscaled for antialiasing
 	#
 	# 	:return:
 	# 	:rtype: int
@@ -608,319 +531,217 @@
 	#
 	# 	depth = wx.DisplayDepth()
 	#
 	# 	if depth >= 24:
 	# 		return 8
 	# 	else:
 	# 		return 6
-	
-	def GetNumberOfLines(self):
+
+	def GetNumberOfLines(self) -> int:
 		"""
 		Returns the number of lines in the text control buffer.
-		
-		:return:
-		:rtype:	int
-		"""
-		
-		return 1
-	
-	def GetRange(self, from_, to_):
 		"""
-		Returns the string containing the text starting in the positions from and up to to in the control.
 
-		The positions must have been returned by another wx.TextCtrl method. Please note that the positions in a multiline wx.TextCtrl do not correspond to the indices in the string returned by GetValue because of the different new line representations ( CR or CR LF) and so this method should be used to obtain the correct results instead of extracting parts of the entire value. It may also be more efficient, especially if the control contains a lot of data.
+		return 1
 
-		:param from_:
-		:type from_: int
-		:param to_:
-		:type to_: int
+	def GetRange(self, from_: int, to_: int) -> str:
+		r"""
+		Returns the string containing the text starting in the positions from and up to to in the control.
 
-		:return:
-		:rtype: str
-		"""
-		
-		return self.m_text.GetRange(from_, to_)
-	
-	def GetSelection(self):
-		"""
-		Gets the current selection span.
+		The positions must have been returned by another :class:`wx.TextCtrl` method.
 
-		If the returned values are equal, there was no selection. Please note that the indices returned may be used with the other wx.TextCtrl methods but don’t necessarily represent the correct indices into the string returned by GetValue for multiline controls under Windows (at least,) you should use GetStringSelection to get the selected text.
+		.. note::
 
-		:return:
-		:rtype: tuple
-		"""
+			The positions in a multiline :class:`wx.TextCtrl` do not correspond to the indices in the string
+			returned by GetValue because of the different new line representations ( ``CR`` or ``CR LF`` )
+			and so this method should be used to obtain the correct results instead of extracting parts
+			of the entire value. It may also be more efficient, especially if the control contains a lot of data.
 
-		return self.m_text.GetSelection()
-	
-	def GetStringSelection(self):
+		:param from\_:
+		:param to\_:
 		"""
-		Gets the text currently selected in the control.
 
-		If there is no selection, the returned string is empty.
+		return self.m_text.GetRange(from_, to_)
 
-		:return:
-		:rtype: str
-		"""
-		
-		return self.m_text.GetStringSelection()
-	
-	def GetStyle(self, position, style):
+	def GetStyle(self, position: int, style: wx.TextAttr) -> bool:
 		"""
 		Returns the style at this position in the text control.
-		
+
 		Not all platforms support this function.
-		
+
 		:param position:
-		:type position: int
 		:param style:
-		:type style: wx.TextAttr
 
-		:return: True on success, False if an error occurred (this may also mean that the styles are not supported under this platform).
-		:rtype: bool
+		:return: :py:obj:`True` on success, :py:obj:`False` if an error occurred (this may also mean that the styles are not supported under this platform).
 		"""
-		
+
 		return self.m_text.GetStyle(position, style)
-	
-	def GetValue(self):
-		"""
-		Gets the contents of the control.
-		
-		Notice that for a multiline text control, the lines will be separated by (Unix-style) \n characters, even under Windows where they are separated by a \r\n sequence in the native control.
-		
-		:return:
-		:rtype:	str
-		"""
-		
-		return self.m_text.GetValue()
-	
-	def HitTestPos(self, pt):
+
+	def HitTestPos(self, pt) -> None:
 		"""
 		Finds the position of the character at the specified point.
 
-		If the return code is not TE_HT_UNKNOWN the position of the character closest to this position is returned, otherwise the output parameter is not modified.
-		
-		Please note that this function is currently only implemented in Univ, wxMSW and wxGTK ports and always returns TE_HT_UNKNOWN in the other ports.
+		If the return code is not :py:obj:`wx.TE_HT_UNKNOWN` the position of the character
+		closest to this position is returned, otherwise the output parameter is not modified.
+
+		.. note::
+
+			This function is currently only implemented in Univ, wxMSW and
+			wxGTK ports and always returns :py:obj:`wx.TE_HT_UNKNOWN` in the other ports.
 
 		:param pt:
-		:type pt:
 
-		:return:
 		:rtype:	wxTextCtrlHitTestResult
 		"""
-		
+
 		return self.m_text.HitTestPos(pt)
-	
-	def HitTest(self, pt):
+
+	def HitTest(self, pt) -> wx.TextCtrlHitTestResult:
 		"""
 		Finds the row and column of the character at the specified point.
 
-		If the return code is not TE_HT_UNKNOWN the row and column of the character closest to this position are returned, otherwise the output parameters are not modified.
-		
-		Please note that this function is currently only implemented in Univ, wxMSW and wxGTK ports and always returns TE_HT_UNKNOWN in the other ports.
+		If the return code is not :py:obj:`wx.TE_HT_UNKNOWN` the row and column
+		of the character closest to this position are returned, otherwise the
+		output parameters are not modified.
 
-		NB: pt is in device coords (not adjusted for the client area origin nor scrolling)
+		.. note::
 
-		:param pt:
-		:type pt:
+			This function is currently only implemented in Univ, wxMSW and
+			wxGTK ports and always returns :py:obj:`wx.TE_HT_UNKNOWN` in the other ports.
 
-		:return:
-		:rtype:	wxTextCtrlHitTestResult
+		NB: pt is in device coords (not adjusted for the client area origin nor scrolling).
+
+		:param pt:
 		"""
-		
+
 		return self.m_text.HitTest(pt)
-	
-	def IsClearButtonVisible(self):
-		"""Returns the clear button’s visibility state"""
+
+	def IsClearButtonVisible(self) -> bool:
+		"""
+		Returns the clear button's visibility state.
+		"""
+
 		return self.m_clearButton and self.m_clearButton.IsShown()
-	
-	def IsEditable(self):
+
+	def IsModified(self) -> bool:
 		"""
-		Returns True if the controls contents may be edited by user (note that it always can be changed by the program).
-		
-		In other words, this functions returns True if the control hasn't been put in read-only mode by a previous call to SetEditable .
-		
-		:return:
-		:rtype:	bool
-		"""
-		
-		return self.m_text.IsEditable()
-	
-	def IsEmpty(self):
-		"""
-		Returns True if the control is currently empty.
-
-		This is the same as GetValue.empty() but can be much more efficient for the multiline controls containing big amounts of text.
-		
-		:return:
-		:rtype:	bool
-		"""
-		
-		return self.m_text.IsEmpty()
-	
-	def IsModified(self):
-		"""
-		Returns True if the text has been modified by user.
-		
-		Note that calling SetValue doesn’t make the control modified.
-		
-		:return:
-		:rtype:	bool
+		Returns whether the text has been modified by user.
+
+		.. note:: Calling :meth:`~.ClearableTextCtrl.SetValue` doesn't make the control modified.
 		"""
-		
+
 		return self.m_text.IsModified()
-	
-	def IsMultiLine(self):
+
+	def IsMultiLine(self) -> bool:
 		"""
-		Returns True if this is a multi line edit control and False otherwise.
-		
-		:return:
-		:rtype:	bool
+		Returns whether this is a multi line control.
 		"""
-		
+
 		return self.m_text.IsMultiLine()
-	
-	def IsSingleLine(self):
+
+	def IsSingleLine(self) -> bool:
 		"""
-		Returns True if this is a single line edit control and False otherwise.
-		
-		:return:
-		:rtype:	bool
+		Returns whether this is a single line control.
 		"""
-		
+
 		return self.m_text.IsSingleLine()
-		
-	def LayoutControls(self):
+
+	def LayoutControls(self) -> None:
+		"""
+		Lays out the child controls.
+		"""
+
 		if not self.m_text:
 			return
-		
+
 		total_size = self.GetClientSize()
 		overall_width = total_size.x
 		overall_height = total_size.y
-		
 
-		
 		text_size = self.m_text.GetBestSize()
 		clear_size = self.m_clearButton.GetBestSize()
 		clear_margin = MARGIN
-		
+
 		# make room for the clear button
 		horizontalBorder = 1 + (text_size.y - text_size.y * 14 / 21) / 2
-		
+
 		x = 0
 		textWidth = overall_width
-		
-		
+
 		textWidth -= horizontalBorder
-		
-		textWidth -= + clear_size.x + clear_margin + 1
+
+		textWidth -= +clear_size.x + clear_margin + 1
 		if textWidth < 0:
 			textWidth = 0
-		
+
 		# position the subcontrols inside the client area
-		
+
 		if wx.Platform == "__WXMSW__":
 			# The text control is too high up on Windows; normally a text control looks OK because
 			# of the white border that's part of the theme border. We can also remove a pixel from
 			# the height to fit the text control in, because the padding in EDIT_HEIGHT_FROM_CHAR_HEIGHT
 			# is already generous.
 			textY = 1
 		else:
 			textY = 0
-		
+
 		self.m_text.SetSize(x, textY, textWidth, overall_height - textY - 10)
-		
+
 		text_pos = self.m_text.GetPosition()
 		self.m_text.SetPosition((text_pos.x + 3, text_pos.y + 5))
 
 		x += textWidth
-		
+
 		x += clear_margin
-		self.m_clearButton.SetSize(
-				x,
-				(overall_height - clear_size.y) / 2,
-				clear_size.x, clear_size.y
-				)
-	
+		self.m_clearButton.SetSize(x, (overall_height - clear_size.y) / 2, clear_size.x, clear_size.y)
+
 		clear_pos = self.m_clearButton.GetPosition()
 		self.m_clearButton.SetPosition((clear_pos.x, clear_pos.y))
-	
-	def MarkDirty(self):
-		"""Mark text as modified (dirty)."""
+
+	def MarkDirty(self) -> None:
+		"""
+		Mark the control as modified (dirty).
+		"""
 
 		self.m_text.MarkDirty()
-	
-	def OnClearButton(self, event):
+
+	def OnClearButton(self, event: wx.CommandEvent) -> None:
 		"""
 		Event handler for clear button being pressed
-		
+
 		:param event:
-		:type event: wx.CommandEvent
 		"""
-		
+
 		self.m_text.Clear()
 		event.Skip()
-	
-	def OnSize(self, event):
+
+	def OnSize(self, event: wx.SizeEvent) -> None:
 		"""
-		Event handler for the size of the control being changed
-		
+		Event handler for the size of the control being changed.
+
 		:param event:
-		:type event: wx.SizeEvent
 		"""
-		
+
 		# pass
 		self.LayoutControls()
-	
-	def Paste(self):
-		self.m_text.Paste()
-		
-	def PositionToXY(self, pos):
+
+	def PositionToXY(self, pos: int) -> Tuple[int, int]:
 		"""
 		Converts given position to a zero-based column, line number pair.
 
 		:param pos: Position
-		:type pos: int
-
-		:return:
-		:rtype: tuple
 		"""
-		
+
 		return self.m_text.PositionToXY(pos)
-	
-	def Redo(self):
-		"""
-		If there is a redo facility and the last operation can be redone, redoes the last operation.
-		
-		Does nothing if there is no redo facility.
-		"""
-		
-		self.m_text.Redo()
-	
-	def Remove(self, from_, to_):
-		"""
-		Removes the text starting at the first given position up to (but not including) the character at the last position.
-
-		This function puts the current insertion point position at to as a side effect.
-		
-		:param from_: The first position
-		:type from_:	int
-		:param to_: The last position
-		:type to_:	int
-		"""
-		
-		self.m_text.Remove(from_, to_)
-	
-	# def RenderClearBitmap(self, x, y):
+
+	# def RenderClearBitmap(self, x: int, y: int):
 	# 	"""
 	#
 	# 	:param x:
-	# 	:type x:	int
 	# 	:param y:
-	# 	:type y: 	int
 	# 	:param renderDrop:
 	# 	:type renderDrop:	bool
 	# 	"""
 	#
 	# 	bg = self.GetBackgroundColour()
 	# 	fg = self.GetForegroundColour().ChangeLightness(CANCEL_BITMAP_LIGHTNESS)
 	#
@@ -994,255 +815,173 @@
 	# 	# end drawing code
 	# 	# ===============================================================================
 	#
 	# 	#if multiplier != 1:
 	# 	self.RescaleBitmap(bitmap, wx.Size(x, y))
 	#
 	# 	return bitmap
-	
-	def Replace(self, from_, to_, value):
-		"""
-		Replaces the text starting at the first position up to (but not including) the character at the last position with the given text.
 
-		This function puts the current insertion point position at to as a side effect.
-		
-		:param from_: The first position
-		:type from_:	int
-		:param to_: The last position
-		:type to_:	int
-		:param value: The value to replace the existing text with.
-		:type value: str
-		"""
-		
-		self.m_text.Replace(from_, to_, value)
-	
-	@staticmethod
-	def RescaleBitmap(bmp, sizeNeeded):
-		"""
-
-		:param bmp:
-		:type bmp: wx.Bitmap
-		:param sizeNeeded:
-		:type sizeNeeded: wx.Size
-		"""
-		
-		if not sizeNeeded.IsFullySpecified():
-			raise ValueError("New size must be given")
-		
-		img = bmp.ConvertToImage()
-		img.Rescale(sizeNeeded.x, sizeNeeded.y)
-		bmp = wx.Bitmap(img)
-	
+	# @staticmethod
+	# def RescaleBitmap(bmp: wx.Bitmap, sizeNeeded: wx.Size):
+	# 	"""
+	#
+	# 	:param bmp:
+	# 	:param sizeNeeded:
+	# 	"""
+	#
+	# 	if not sizeNeeded.IsFullySpecified():
+	# 		raise ValueError("New size must be given")
+	#
+	# 	img = bmp.ConvertToImage()
+	# 	img.Rescale(sizeNeeded.x, sizeNeeded.y)
+	# 	bmp = wx.Bitmap(img)
+
 	#
 	# if wx.Platform in {"__WXMSW__", "__WXOSX__"}:
 	# 	newBmp.UseAlpha(bmp.HasAlpha())
 	#
 	# dc(newBmp)
 	# scX = sizeNeeded.GetWidth() / bmp.GetWidth()
 	# scY = sizeNeeded.GetHeight() / bmp.GetHeight()
 	# dc.SetUserScale(scX, scY)
 	# dc.DrawBitmap(bmp, 0, 0)
 	#
 	# bmp = newBmp
-	
-	def SelectAll(self):
-		"""Selects all text in the control."""
-		
-		self.m_text.SelectAll()
-		
-	def SelectNone(self):
-		"""Deselects selected text in the control."""
-		
-		self.m_text.SelectNone()
-	
-	def SetClearBitmap(self, bitmap):
+
+	def SetClearBitmap(self, bitmap: wx.Bitmap):
 		"""
-		
+		Sets the bitmap for the clear button.
+
 		:param bitmap:
-		:type bitmap:	 wxBitmap
 		"""
-		
+
 		if bitmap.IsOk:
 			self.m_clearBitmap = bitmap
 			if self.m_clearButton:
 				self.m_clearButton.SetBitmapLabel(self.m_clearBitmap)
-	
-	def SetDefaultStyle(self, style):
+
+	def SetDefaultStyle(self, style: wx.TextAttr) -> bool:
 		"""
 		Changes the default style to use for the new text which is going to be added to the control.
-		
-		This applies both to the text added programmatically using WriteText or AppendText and to the text entered by the user interactively.
-		
-		If either of the font, foreground, or background colour is not set in style, the values of the previous default style are used for them. If the previous default style didn’t set them neither, the global font or colours of the text control itself are used as fall back.
-		
-		However if the style parameter is the default wx.TextAttr, then the default style is just reset (instead of being combined with the new style which wouldn’t change it at all).
-		
+
+		This applies both to the text added programmatically using :meth:`~.ClearableTextCtrl.WriteText` or
+		:meth:`~.ClearableTextCtrl.AppendText` and to the text entered by the user interactively.
+
+		If either of the font, foreground, or background colour is not set in style,
+		the values of the previous default style are used for them.
+		If the previous default style didn't set them either then the global font or colours
+		of the text control itself are used as fall back.
+
+		However, if the style parameter is the default :class:`wx.TextAttr`,
+		then the default style is just reset (instead of being combined with
+		the new style which wouldn't change it at all).
+
 		:param style: The style for the new text
-		:type style: wx.TextAttr
 
-		:return: True on success, False if an error occurred (this may also mean that the styles are not supported under this platform).
-		:rtype: bool
+		:return: :py:obj:`True` on success, :py:obj:`False` if an error occurred
+			(this may also mean that the styles are not supported under this platform).
 		"""
-		
+
 		return self.m_text.SetDefaultStyle(style)
-	
-	def SetEditable(self, editable):
+
+	def SetEditable(self, editable: bool):
 		"""
-		Makes the text item editable or read-only, overriding the wx.TE_READONLY flag.
-		
-		:param editable: If True, the control is editable. If False, the control is read-only.
-		:type editable:	bool
+		Makes the text item editable or read-only, overriding the :py:obj:`wx.TE_READONLY` flag.
+
+		:param editable: If :py:obj:`True`, the control should be editable.
+			If :py:obj:`False`, the control should be read-only.
 		"""
-		
+
 		self.m_text.SetEditable(editable)
-	
-	def SetInsertionPoint(self, pos):
+
+	def SetInsertionPoint(self, pos: int):
 		"""
 		Sets the insertion point at the given position.
-		
-		:param pos: Position to set, in the range from 0 to GetLastPosition inclusive.
-		:type pos: int
+
+		:param pos: Position to set, in the range from 0 to :meth:`~.ClearableTextCtrl.GetLastPosition` inclusive.
 		"""
-		
+
 		self.m_text.SetInsertionPoint(pos)
-	
+
 	def SetInsertionPointEnd(self):
 		"""
 		Sets the insertion point at the end of the text control.
 
-		This is equivalent to calling wx.TextCtrl.SetInsertionPoint with wx.TextCtrl.GetLastPosition argument.
+		This is equivalent to calling :meth:`~.ClearableTextCtrl.SetInsertionPoint`
+		with :meth:`~.ClearableTextCtrl.GetLastPosition` as the argument.
 		"""
-		
+
 		self.m_text.SetInsertionPointEnd()
-	
+
 	# SetMargins
-	
-	def SetMaxLength(self, len):
+
+	def SetMaxLength(self, length: int):
 		"""
 		This function sets the maximum number of characters the user can enter into the control.
-		
-		In other words, it allows limiting the text value length to len not counting the terminating NUL character.
-		
-		If len is 0, the previously set max length limit, if any, is discarded and the user may enter as much text as the underlying native text control widget supports (typically at least 32Kb). If the user tries to enter more characters into the text control when it already is filled up to the maximal length, a wxEVT_TEXT_MAXLEN event is sent to notify the program about it (giving it the possibility to show an explanatory message, for example) and the extra input is discarded.
-		
+
+		In other words, it allows limiting the text value length to len not counting the terminating ``NUL`` character.
+
+		If len is 0, the previously set max length limit, if any, is discarded,
+		and the user may enter as much text as the underlying native text control widget supports
+		(typically at least 32Kb).
+
+		If the user tries to enter more characters into the text control when it is already
+		filled up to the maximal length, a :py:obj:`wx.wxEVT_TEXT_MAXLEN` event is sent to
+		notify the program about it (giving it the possibility to show an explanatory message, for example)
+		and the extra input is discarded.
+
 		Note that in wxGTK this function may only be used with single line text controls.
 
-		:param len:
-		:type len:	long
+		:param length:
 		"""
-		
-		self.m_text.SetMaxLength(len)
-	
-	def SetModified(self, modified):
+
+		self.m_text.SetMaxLength(length)
+
+	def SetModified(self, modified: bool):
 		"""
 		Marks the control as being modified by the user or not.
 
 		:param modified:
-		:type modified: bool
 		"""
-		
+
 		self.m_text.SetModified(modified)
-	
-	def SetSelection(self, from_, to_):
-		"""
-		Selects the text starting at the first position up to (but not including) the character at the last position.
-	
-		If both parameters are equal to -1 all text in the control is selected.
-		
-		Notice that the insertion point will be moved to from by this function.
-
-		:param from_: The first position
-		:type from_: int
-		:param to_: The last position
-		:type to_: int
-		"""
-		
-		self.m_text.SetSelection(from_, to_)
-	
-	def SetStyle(self, start, end, style):
+
+	def SetStyle(self, start: int, end: int, style: wx.TextAttr) -> bool:
 		"""
 		Changes the style of the given range.
 
 		If any attribute within style is not set, the corresponding attribute from GetDefaultStyle is used.
 
 		:param start: The start of the range to change.
-		:type start: int
 		:param end: The end of the range to change.
-		:type end: int
 		:param style: The new style for the range.
-		:type style: wx.TextAttr
 
-		:return: True on success, False if an error occurred (this may also mean that the styles are not supported under this platform).
-		:rtype: bool
+		:return: :py:obj:`True` on success, :py:obj:`False` if an error occurred
+			(this may also mean the styles are not supported under this platform).
 		"""
-		
+
 		return self.m_text.SetStyle(start, end, style)
-	
-	def SetValue(self, value):
-		"""
-		Sets the new text control value.
 
-		It also marks the control as not-modified which means that IsModified() would return False immediately after the call to SetValue .
-		
-		The insertion point is set to the start of the control (i.e. position 0) by this function unless the control value doesn’t change at all, in which case the insertion point is left at its original position.
-		
-		Note that, unlike most other functions changing the controls values, this function generates a wxEVT_TEXT event. To avoid this you can use ChangeValue instead.
-
-		:param value: The new value to set. It may contain newline characters if the text control is multi-line.
-		:type value: str
-		"""
-	
-		self.m_text.SetValue(value)
-	
-	def ShowPosition(self, pos):
+	def ShowPosition(self, pos: int):
 		"""
 		Makes the line containing the given position visible.
-		
+
 		:param pos: The position that should be visible.
-		:type pos: int
 		"""
-		
+
 		self.m_text.ShowPosition(pos)
-	
-	def ShouldInheritColours(self):
-			"""
-			
-			:rtype: bool
-			
-			:return:
-			:rtype:
-			"""
-		
-			return True
-	
-	def Undo(self):
-		"""
-		If there is an undo facility and the last operation can be undone, undoes the last operation.
-		
-		Does nothing if there is no undo facility.
-		"""
-		
-		self.m_text.Undo()
-	
-	def WriteText(self, text):
-		"""
-		Writes the text into the text control at the current insertion position.
-		
-		:param text: Text to write to the text control
-		:type text: str
-		"""
-		
-		self.m_text.WriteText(text)
-	
-	def XYToPosition(self, x, y):
+
+	def ShouldInheritColours(self) -> bool:
 		"""
-		Converts the given zero based column and line number to a position.
+		"""
+
+		return True
+
+	def XYToPosition(self, x: int, y: int) -> int:
+		"""
+		Converts the given zero-based column and line number to a position.
 
 		:param x: The column number
-		:type x: int
 		:param y: The line number
-		:type y: int
-
-		:rtype: int
 		"""
-		
+
 		return self.m_text.XYToPosition(x, y)
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/editable_listbox.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/editable_listbox.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #  !/usr/bin/env python
-#   -*- coding: utf-8 -*-
 #
 #  editable_listbox.py
 """
 A Python implementation of wx.EditableListBox, a ListBox with editable items.
 
 Available in two flavours:
-	> Vanilla, that accepts any string value; and
-	> Numerical, that only accepts numerical values.
-	  Those could be str, int, float or decimal.Decimal, but decimal.Decimal
-	  is used internally and is the type that will be returned.
+
+* Vanilla, that accepts any string value; and
+* Numerical, that only accepts numerical values.
+	Those could be str, int, float or decimal.Decimal, but decimal.Decimal
+	is used internally and is the type that will be returned.
+
 """
 #
 #  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Based on src/generic/editlbox.cpp from wxWidgets
 #  Copyright (c) Vaclav Slavik
 #  Licenced under the wxWindows licence
@@ -32,615 +33,616 @@
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
 # stdlib
 from decimal import Decimal
+from typing import List, Sequence, Union
 
 # 3rd party
-import wx
-import wx.adv
+import wx  # type: ignore
+import wx.adv  # type: ignore
 from mathematical.utils import rounders
 
-# This package
+# this package
 from domdf_wxpython_tools.validators import FloatValidator
 
+__all__ = ["CleverListCtrl", "EditableListBox", "EditableNumericalListBox"]
 
 # IDs
 ID_ELB_DELETE = wx.NewIdRef()
 ID_ELB_EDIT = wx.NewIdRef()
 ID_ELB_NEW = wx.NewIdRef()
 ID_ELB_UP = wx.NewIdRef()
 ID_ELB_DOWN = wx.NewIdRef()
 ID_ELB_LISTCTRL = wx.NewIdRef()
 
-
 # XPM for Buttons
 
 edit_btn_xpm = [
-	b"16 16 3 1",
-	b"   c None",
-	b".  c #000000",
-	b"+  c #00007F",
-	b"                ",
-	b"                ",
-	b"      .. ..     ",
-	b"        .       ",
-	b"        .       ",
-	b"  ++++  .  ++++ ",
-	b"     ++ . ++  ++",
-	b"  +++++ . ++++++",
-	b" ++  ++ . ++    ",
-	b" ++  ++ . ++  ++",
-	b"  +++++ .  ++++ ",
-	b"        .       ",
-	b"        .       ",
-	b"      .. ..     ",
-	b"                ",
-	b"                "
+		b"16 16 3 1",
+		b"   c None",
+		b".  c #000000",
+		b"+  c #00007F",
+		b"                ",
+		b"                ",
+		b"      .. ..     ",
+		b"        .       ",
+		b"        .       ",
+		b"  ++++  .  ++++ ",
+		b"     ++ . ++  ++",
+		b"  +++++ . ++++++",
+		b" ++  ++ . ++    ",
+		b" ++  ++ . ++  ++",
+		b"  +++++ .  ++++ ",
+		b"        .       ",
+		b"        .       ",
+		b"      .. ..     ",
+		b"                ",
+		b"                "
 		]
 
 numerical_edit_btn_xpm = [
-	b"16 16 3 1",
-	b"   c None",
-	b".  c #000000",
-	b"+  c #00007F",
-	b"                ",
-	b"                ",
-	b"      .. ..     ",
-	b"        .       ",
-	b"   ++   .  ++++ ",
-	b"  +++   . ++  ++",
-	b" ++++   . ++  ++",
-	b"   ++   . ++  ++",
-	b"   ++   . ++  ++",
-	b"   ++   . ++  ++",
-	b" ++++++ .  ++++ ",
-	b"        .       ",
-	b"        .       ",
-	b"      .. ..     ",
-	b"                ",
-	b"                "
+		b"16 16 3 1",
+		b"   c None",
+		b".  c #000000",
+		b"+  c #00007F",
+		b"                ",
+		b"                ",
+		b"      .. ..     ",
+		b"        .       ",
+		b"   ++   .  ++++ ",
+		b"  +++   . ++  ++",
+		b" ++++   . ++  ++",
+		b"   ++   . ++  ++",
+		b"   ++   . ++  ++",
+		b"   ++   . ++  ++",
+		b" ++++++ .  ++++ ",
+		b"        .       ",
+		b"        .       ",
+		b"      .. ..     ",
+		b"                ",
+		b"                "
 		]
 
 new_btn_xpm = [
-	b"16 16 5 1",
-	b"   c None",
-	b".  c #7F7F7F",
-	b"+  c #FFFFFF",
-	b"@  c #FFFF00",
-	b"#  c #000000",
-	b"                ",
-	b"                ",
-	b" .  .+ .@       ",
-	b"  . .@.@# # #   ",
-	b"  @.@+....   #  ",
-	b" ... @@         ",
-	b"  @ . @.     #  ",
-	b" .# .@          ",
-	b"    .        #  ",
-	b"  #             ",
-	b"             #  ",
-	b"  #             ",
-	b"             #  ",
-	b"  # # # # # #   ",
-	b"                ",
-	b"                "
+		b"16 16 5 1",
+		b"   c None",
+		b".  c #7F7F7F",
+		b"+  c #FFFFFF",
+		b"@  c #FFFF00",
+		b"#  c #000000",
+		b"                ",
+		b"                ",
+		b" .  .+ .@       ",
+		b"  . .@.@# # #   ",
+		b"  @.@+....   #  ",
+		b" ... @@         ",
+		b"  @ . @.     #  ",
+		b" .# .@          ",
+		b"    .        #  ",
+		b"  #             ",
+		b"             #  ",
+		b"  #             ",
+		b"             #  ",
+		b"  # # # # # #   ",
+		b"                ",
+		b"                "
 		]
 
 delete_btn_xpm = [
-	b"16 16 3 1",
-	b"   c None",
-	b".  c #7F0000",
-	b"+  c #FFFFFF",
-	b"                ",
-	b"                ",
-	b"                ",
-	b" ..+        ..+ ",
-	b" ....+     ..+  ",
-	b"  ....+   ..+   ",
-	b"    ...+ .+     ",
-	b"     .....+     ",
-	b"      ...+      ",
-	b"     .....+     ",
-	b"    ...+ ..+    ",
-	b"   ...+   ..+   ",
-	b"  ...+     .+   ",
-	b"  ...+      .+  ",
-	b"   .         .  ",
-	b"                "
+		b"16 16 3 1",
+		b"   c None",
+		b".  c #7F0000",
+		b"+  c #FFFFFF",
+		b"                ",
+		b"                ",
+		b"                ",
+		b" ..+        ..+ ",
+		b" ....+     ..+  ",
+		b"  ....+   ..+   ",
+		b"    ...+ .+     ",
+		b"     .....+     ",
+		b"      ...+      ",
+		b"     .....+     ",
+		b"    ...+ ..+    ",
+		b"   ...+   ..+   ",
+		b"  ...+     .+   ",
+		b"  ...+      .+  ",
+		b"   .         .  ",
+		b"                "
 		]
 
 down_btn_xpm = [
-	b"16 16 2 1",
-	b"   c None",
-	b".  c #000000",
-	b"                ",
-	b"                ",
-	b"         ...    ",
-	b"        ...     ",
-	b"       ...      ",
-	b"       ...      ",
-	b"       ...      ",
-	b"       ...      ",
-	b"   ...........  ",
-	b"    .........   ",
-	b"     .......    ",
-	b"      .....     ",
-	b"       ...      ",
-	b"        .       ",
-	b"                ",
-	b"                "
+		b"16 16 2 1",
+		b"   c None",
+		b".  c #000000",
+		b"                ",
+		b"                ",
+		b"         ...    ",
+		b"        ...     ",
+		b"       ...      ",
+		b"       ...      ",
+		b"       ...      ",
+		b"       ...      ",
+		b"   ...........  ",
+		b"    .........   ",
+		b"     .......    ",
+		b"      .....     ",
+		b"       ...      ",
+		b"        .       ",
+		b"                ",
+		b"                "
 		]
 
 up_btn_xpm = [
-	b"16 16 2 1",
-	b"   c None",
-	b".  c #000000",
-	b"                ",
-	b"        .       ",
-	b"       ...      ",
-	b"      .....     ",
-	b"     .......    ",
-	b"    .........   ",
-	b"   ...........  ",
-	b"       ...      ",
-	b"       ...      ",
-	b"       ...      ",
-	b"       ...      ",
-	b"      ...       ",
-	b"     ...        ",
-	b"                ",
-	b"                ",
-	b"                "
+		b"16 16 2 1",
+		b"   c None",
+		b".  c #000000",
+		b"                ",
+		b"        .       ",
+		b"       ...      ",
+		b"      .....     ",
+		b"     .......    ",
+		b"    .........   ",
+		b"   ...........  ",
+		b"       ...      ",
+		b"       ...      ",
+		b"       ...      ",
+		b"       ...      ",
+		b"      ...       ",
+		b"     ...        ",
+		b"                ",
+		b"                ",
+		b"                "
 		]
 
 
 class CleverListCtrl(wx.ListCtrl):
 	"""
 	list control with auto-resizable column:
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
+	:param id:
+	:param pos:
+	:param size:
+	:param style:
+	:param validator:
+	:param name:
 	"""
+
 	def __init__(
-			self, parent, id=wx.ID_ANY, pos=wx.DefaultPosition,
-			size=wx.DefaultSize, style=wx.LC_ICON,
-			validator=wx.DefaultValidator, name=wx.ListCtrlNameStr
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = wx.LC_ICON,
+			validator: wx.Validator = wx.DefaultValidator,
+			name: str = wx.ListCtrlNameStr
 			):
-		"""
-		:param parent:
-		:type parent: wx.Window
-		:param id:
-		:type id: wx.WindowID
-		:param pos:
-		:type pos: wx.Point
-		:param size:
-		:type size: wx.Size
-		:param style:
-		:type style: int
-		:param validator:
-		:type validator: wx.Validator
-		:param name:
-		:type name: str
-		"""
-		
+
 		wx.ListCtrl.__init__(self, parent, id, pos, size, style, validator, name)
-		
+
 		self.CreateColumns()
-		
+
 		self.Bind(wx.EVT_SIZE, self.OnSize)
-	
+
 	def CreateColumns(self):
 		self.InsertColumn(0, "item")
 		self.SizeColumns()
-	
+
 	def SizeColumns(self):
 		w = self.GetSize().x
-		
+
 		if wx.Platform == "__WXMSW__":
 			w -= wx.SystemSettings.GetMetric(wx.SYS_VSCROLL_X, self) + 6
 		else:
 			w -= 2 * wx.SystemSettings.GetMetric(wx.SYS_VSCROLL_X, self)
-		
+
 		if w < 0:
 			w = 0
 		self.SetColumnWidth(0, w)
-	
+
 	# private
-	def OnSize(self, event):
+	def OnSize(self, event) -> None:
+		"""
+
+		:param event: The wxPython event.
+		"""
+
 		self.SizeColumns()
 		event.Skip()
 
 
 class EditableListBox(wx.Panel):
-	def __init__(self, parent, id=wx.ID_ANY, label="",
-			pos=wx.DefaultPosition, size=wx.DefaultSize,
-			style=wx.adv.EL_DEFAULT_STYLE, name=wx.adv.EditableListBoxNameStr
+	"""
+	This class provides a composite control that lets the user easily enter
+	and edit a list of strings.
+
+	Styles supported:
+
+	* :py:obj:`wx.adv.EL_ALLOW_NEW` - Allow user to create new items.
+	* :py:obj:`wx.adv.EL_ALLOW_EDIT` - Allow user to edit text in the control.
+	* :py:obj:`wx.adv.EL_ALLOW_DELETE` - Allow user to delete text from the control.
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
+	:param id:
+	:param label:
+	:param pos:
+	:param size:
+	:param style:
+	:param name:
+	"""  # noqa: D400
+
+	def __init__(
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			label: str = '',
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = wx.adv.EL_DEFAULT_STYLE,
+			name: str = wx.adv.EditableListBoxNameStr
 			):
-		"""
-		This class provides a composite control that lets the user easily enter
-		and edit a list of strings.
 
-		Styles supported:
-			> wx.adv.EL_ALLOW_NEW - Allow user to create new items.
-			> wx.adv.EL_ALLOW_EDIT - Allow user to edit text in the control.
-			> wx.adv.EL_ALLOW_DELETE - Allow user to delete text from the control.
-
-		:param parent:
-		:type parent: wx.Window
-		:param id:
-		:type id: wx.WindowID
-		:param label:
-		:type label: wx.String
-		:param pos:
-		:type pos: wx.Point
-		:param size:
-		:type size:  wx.Size
-		:param style:
-		:type style: int
-		:param name:
-		:type name: str
-		"""
-		
 		wx.Panel.__init__(self, parent, id, pos, size, style, name)
-		
+
 		self.m_style = style
-		
+
 		sizer = wx.BoxSizer(wx.VERTICAL)
-		
+
 		subp = wx.Panel(self, style=wx.SUNKEN_BORDER | wx.TAB_TRAVERSAL)
 		subsizer = wx.BoxSizer(wx.HORIZONTAL)
-		
-		subsizer.Add(wx.StaticText(subp, wx.ID_ANY, label),
-					 1, wx.CENTER | wx.LEFT, 5)
+
+		subsizer.Add(wx.StaticText(subp, wx.ID_ANY, label), 1, wx.CENTER | wx.LEFT, 5)
 		# TODO: if width too small put label on row above buttons
 		# Min width to see all buttons = (152, 250)
-		
+
 		if self.m_style & wx.adv.EL_ALLOW_EDIT:
-			self.m_bEdit = wx.BitmapButton(subp, ID_ELB_EDIT, wx.Bitmap(
-				edit_btn_xpm))  # wx.ArtProvider.GetBitmap(wx.ART_EDIT, wx.ART_BUTTON))
+			self.m_bEdit = wx.BitmapButton(subp, ID_ELB_EDIT, wx.Bitmap(edit_btn_xpm))
 			self.m_bEdit.SetToolTip("Edit item")
 			subsizer.Add(self.m_bEdit, 0, wx.CENTER)
-		
+
 		if self.m_style & wx.adv.EL_ALLOW_NEW:
-			self.m_bNew = wx.BitmapButton(subp, ID_ELB_NEW,
-										  wx.ArtProvider.GetBitmap(wx.ART_NEW, wx.ART_BUTTON))
+			self.m_bNew = wx.BitmapButton(subp, ID_ELB_NEW, wx.ArtProvider.GetBitmap(wx.ART_NEW, wx.ART_BUTTON))
 			self.m_bNew.SetToolTip("New item")
 			subsizer.Add(self.m_bNew, 0, wx.CENTER)
-		
+
 		if self.m_style & wx.adv.EL_ALLOW_DELETE:
 			self.m_bDel = wx.BitmapButton(subp, ID_ELB_DELETE, wx.Bitmap(delete_btn_xpm))
 			self.m_bDel.SetToolTip("Delete item")
 			subsizer.Add(self.m_bDel, 0, wx.CENTER)
-		
+
 		if not (self.m_style & wx.adv.EL_NO_REORDER):
-			self.m_bUp = wx.BitmapButton(subp, ID_ELB_UP,
-										 wx.ArtProvider.GetBitmap(wx.ART_GO_UP, wx.ART_BUTTON))
+			self.m_bUp = wx.BitmapButton(subp, ID_ELB_UP, wx.ArtProvider.GetBitmap(wx.ART_GO_UP, wx.ART_BUTTON))
 			self.m_bUp.SetToolTip("Move up")
 			subsizer.Add(self.m_bUp, 0, wx.CENTER)
-			
-			self.m_bDown = wx.BitmapButton(subp, ID_ELB_DOWN,
-										   wx.ArtProvider.GetBitmap(wx.ART_GO_DOWN, wx.ART_BUTTON))
+
+			self.m_bDown = wx.BitmapButton(
+					subp, ID_ELB_DOWN, wx.ArtProvider.GetBitmap(wx.ART_GO_DOWN, wx.ART_BUTTON)
+					)
 			self.m_bDown.SetToolTip("Move down")
 			subsizer.Add(self.m_bDown, 0, wx.CENTER)
-		
+
 		subp.SetSizer(subsizer)
 		subsizer.Fit(subp)
-		
+
 		sizer.Add(subp, 0, wx.EXPAND)
-		
+
 		st = wx.LC_REPORT | wx.LC_NO_HEADER | wx.LC_SINGLE_SEL | wx.SUNKEN_BORDER
-		
+
 		if style & wx.adv.EL_ALLOW_EDIT:
 			st |= wx.LC_EDIT_LABELS
-		
+
 		self.m_listCtrl = CleverListCtrl(self, ID_ELB_LISTCTRL, wx.DefaultPosition, wx.DefaultSize, st)
-		
+
 		self.SetStrings([])
-		
+
 		sizer.Add(self.m_listCtrl, 1, wx.EXPAND)
-		
+
 		self.SetSizer(sizer)
 		self.Layout()
-		
+
 		self.Bind(wx.EVT_LIST_ITEM_SELECTED, self.OnItemSelected, id=ID_ELB_LISTCTRL)
 		self.Bind(wx.EVT_LIST_BEGIN_LABEL_EDIT, self.OnBeginLabelEdit, id=ID_ELB_LISTCTRL)
 		self.Bind(wx.EVT_LIST_END_LABEL_EDIT, self.OnEndLabelEdit, id=ID_ELB_LISTCTRL)
 		self.Bind(wx.EVT_BUTTON, self.OnNewItem, id=ID_ELB_NEW)
 		self.Bind(wx.EVT_BUTTON, self.OnUpItem, id=ID_ELB_UP)
 		self.Bind(wx.EVT_BUTTON, self.OnDownItem, id=ID_ELB_DOWN)
 		self.Bind(wx.EVT_BUTTON, self.OnEditItem, id=ID_ELB_EDIT)
 		self.Bind(wx.EVT_BUTTON, self.OnDelItem, id=ID_ELB_DELETE)
 		self.Bind(wx.EVT_LIST_ITEM_ACTIVATED, self.OnItemActivated, self.m_listCtrl)
-	
+
 	def OnItemActivated(self, evt):
 		self.curRow = evt.GetIndex()
 		print(123)
 		self.m_listCtrl.EditLabel(self.curRow)
 		evt.Skip()
-	
-	def SetStrings(self, strings):
+
+	def SetStrings(self, strings: List[str]):
 		"""
 		Replaces current contents with given strings.
-		
-		:param strings: list of strings
-		:type strings: list of str
+
+		:param strings: list of strings.
 		"""
-		
+
 		self.m_listCtrl.DeleteAllItems()
-		for i in range(len(strings)):
-			self.m_listCtrl.InsertItem(i, str(strings[i]))
-		
+		for idx, string in enumerate(strings):
+			self.m_listCtrl.InsertItem(idx, str(string))
+
 		self.m_listCtrl.InsertItem(len(strings), '')
 		self.m_listCtrl.SetItemState(0, wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED)
-	
-	def GetStrings(self):
+
+	def GetStrings(self) -> List[str]:
 		"""
 		Returns a list of the current contents of the control.
-		
+
 		:return: list of strings
 		:rtype: list of str
 		"""
-		
+
 		strings = []
-		
+
 		for i in range(self.m_listCtrl.GetItemCount()):
 			val = self.m_listCtrl.GetItemText(i)
 			if val:
 				strings.append(val)
-	
+
 		return strings
-	
+
 	def OnItemSelected(self, event):
 		self.m_selection = event.GetIndex()
 		if not (self.m_style & wx.adv.EL_NO_REORDER):
 			self.m_bUp.Enable(self.m_selection != 0 and self.m_selection < self.m_listCtrl.GetItemCount() - 1)
 			self.m_bDown.Enable(self.m_selection < self.m_listCtrl.GetItemCount() - 2)
-			
+
 		if self.m_style & wx.adv.EL_ALLOW_EDIT:
 			self.m_bEdit.Enable(self.m_selection < self.m_listCtrl.GetItemCount())
 			if self.m_style & wx.adv.EL_ALLOW_DELETE:
 				self.m_bDel.Enable(self.m_selection < self.m_listCtrl.GetItemCount() - 1)
-	
-	def OnNewItem(self, event):
+
+	def OnNewItem(self, event) -> None:
+		"""
+
+		:param event: The wxPython event.
+		"""
+
 		self.m_listCtrl.SetItemState(
-				self.m_listCtrl.GetItemCount() - 1,
-				wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED
+				self.m_listCtrl.GetItemCount() - 1, wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED
 				)
-		
+
 		self.m_listCtrl.EditLabel(self.m_selection)
-	
-	def OnBeginLabelEdit(self, event):
+
+	def OnBeginLabelEdit(self, event) -> None:
+		"""
+
+		:param event: The wxPython event.
+		"""
+
 		event.Skip()
-		
+
 		# To ensure it happens after editing starts
 		wx.CallAfter(self.SetupEditControl)
-	
+
 	def SetupEditControl(self):
 		edit_control = self.m_listCtrl.GetEditControl()
-		
+
 		# Bind Events
 		edit_control.Bind(wx.EVT_TEXT, self.on_value_changed)
 		edit_control.Bind(wx.EVT_TEXT_ENTER, self.on_value_changed)
-		
+
 		return edit_control
-	
+
 	def on_value_changed(self, event):  # wxGlade: CalibreMeasurementPanel.<event_handler>
 		event.Skip()
-	
-	def OnEndLabelEdit(self, event):
+
+	def OnEndLabelEdit(self, event) -> None:
+		"""
+
+		:param event: The wxPython event.
+		"""
 		# return
-		if event.GetIndex() == self.m_listCtrl.GetItemCount()-1 and event.GetText():
+		if event.GetIndex() == self.m_listCtrl.GetItemCount() - 1 and event.GetText():
 			# The user edited last (empty) line, i.e. added new entry. We have to
 			# add new empty line here so that adding one more line is still
 			# possible:
 			self.m_listCtrl.InsertItem(self.m_listCtrl.GetItemCount(), '')
-			
+
 			# Simulate a wxEVT_LIST_ITEM_SELECTED event for the new item,
 			# so that the buttons are enabled/disabled properly
 			selectionEvent = wx.ListEvent(wx.wxEVT_LIST_ITEM_SELECTED, self.m_listCtrl.GetId())
 			selectionEvent.SetIndex(event.GetIndex())
 			self.m_listCtrl.GetEventHandler().ProcessEvent(selectionEvent)
-	
-	def OnDelItem(self, event):
-		
+
+	def OnDelItem(self, _) -> None:
 		self.m_listCtrl.DeleteItem(self.m_selection)
 		self.m_listCtrl.SetItemState(self.m_selection, wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED)
-	
-	def OnEditItem(self, event):
-		
+
+	def OnEditItem(self, _) -> None:
 		self.m_listCtrl.EditLabel(self.m_selection)
-	
-	def SwapItems(self, i1, i2):
+
+	def SwapItems(self, i1: int, i2: int):
 		"""
-		
+
 		:param i1:
-		:type i1: int
 		:param i2:
-		:type i2: int
 		"""
-		
+
 		# swap the text
 		t1 = self.m_listCtrl.GetItemText(i1)
 		t2 = self.m_listCtrl.GetItemText(i2)
 		self.m_listCtrl.SetItemText(i1, t2)
 		self.m_listCtrl.SetItemText(i2, t1)
 
 		# swap the item data
 		d1 = self.m_listCtrl.GetItemData(i1)
 		d2 = self.m_listCtrl.GetItemData(i2)
 		self.m_listCtrl.SetItemData(i1, d2)
 		self.m_listCtrl.SetItemData(i2, d1)
-	
-	def OnUpItem(self, event):
-		
+
+	def OnUpItem(self, _) -> None:
 		self.SwapItems(self.m_selection - 1, self.m_selection)
-		self.m_listCtrl.SetItemState(
-				self.m_selection - 1,
-				wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED)
-	
-	def OnDownItem(self, event):
-		
+		self.m_listCtrl.SetItemState(self.m_selection - 1, wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED)
+
+	def OnDownItem(self, _) -> None:
 		self.SwapItems(self.m_selection + 1, self.m_selection)
-		self.m_listCtrl.SetItemState(
-				self.m_selection + 1,
-				wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED)
-	
-	def GetListCtrl(self):
+		self.m_listCtrl.SetItemState(self.m_selection + 1, wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED)
+
+	def GetListCtrl(self) -> wx.ListCtrl:
 		"""
 		Returns a reference to the actual list control portion of the custom control.
-		
+
 		:return:
 		:rtype: wx.ListCtrl
 		"""
-		
+
 		return self.m_listCtrl
-	
+
 	def GetDelButton(self):
 		"""
 		Retrieves a reference to the BitmapButton that is used as the 'delete' button in the control.
 		"""
-		
+
 		return self.m_bDel
-	
+
 	def GetNewButton(self):
 		"""
 		Retrieves a reference to the BitmapButton that is used as the 'new' button in the control.
 		"""
-		
+
 		return self.m_bNew
-	
+
 	def GetUpButton(self):
 		"""
 		Retrieves a reference to the BitmapButton that is used as the 'up' button in the control.
 		"""
-		
+
 		return self.m_bUp
-	
+
 	def GetDownButton(self):
 		"""
 		Retrieves a reference to the BitmapButton that is used as the 'down' button in the control.
 		"""
-		
+
 		return self.m_bDown
-	
+
 	def GetEditButton(self):
 		"""
 		Retrieves a reference to the BitmapButton that is used as the 'edit' button in the control.
 		"""
-		
+
 		return self.m_bEdit
-			
-			
+
+
 class EditableNumericalListBox(EditableListBox):
-	def __init__(self, parent, id=wx.ID_ANY, label="", decimal_places=-1,
-			pos=wx.DefaultPosition, size=wx.DefaultSize,
-			style=wx.adv.EL_DEFAULT_STYLE, name=wx.adv.EditableListBoxNameStr
+	"""
+
+	:param parent: Parent window. Should not be :py:obj:`None`.
+	:param id:
+	:param label:
+	:param pos:
+	:param size:
+	:param style:
+	:param name:
+	"""
+
+	def __init__(
+			self,
+			parent: wx.Window,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			label: str = '',
+			decimal_places=-1,
+			pos: wx.Point = wx.DefaultPosition,
+			size: wx.Size = wx.DefaultSize,
+			style: int = wx.adv.EL_DEFAULT_STYLE,
+			name: str = wx.adv.EditableListBoxNameStr
 			):
-		"""
-		
-		:param parent:
-		:type parent: wx.Window
-		:param id:
-		:type id: wx.WindowID
-		:param label:
-		:type label: wx.String
-		:param pos:
-		:type pos: wx.Point
-		:param size:
-		:type size:  wx.Size
-		:param style:
-		:type style: int
-		:param name:
-		:type name: str
-		"""
-		
+
 		EditableListBox.__init__(self, parent, id, label, pos, size, style, name)
-		
+
 		self.SetDecimalPlaces(decimal_places)
-		
+
 		# Change bitmap for Edit button
 		self.m_bEdit.SetBitmap(wx.Bitmap(numerical_edit_btn_xpm))
 		self.m_bEdit.SetBitmapDisabled(wx.NullBitmap)
-	
+
 	def SetDecimalPlaces(self, _decimal_places):
 		self._decimal_places = _decimal_places
-		
+
 		if self._decimal_places == 0:
-			self._rounders_string = "0"
+			self._rounders_string = '0'
 		elif self._decimal_places == -1:
 			self._rounders_string = ''
 		else:
 			self._rounders_string = f"0.{'0' * self._decimal_places}"
-	
+
 	def GetDecimalPlaces(self):
 		return self._decimal_places
-	
+
 	@property
 	def decimal_places(self):
 		return self._decimal_places
-	
+
 	@decimal_places.setter
 	def decimal_places(self, decimal_places):
 		self.SetDecimalPlaces(decimal_places)
-	
+
 	def SetStrings(self, strings):
 		self.SetValues(strings)
-	
-	def SetValues(self, values):
+
+	def SetValues(self, values: Sequence[Union[float, Decimal]]) -> None:
 		"""
 		Replaces current contents with given values.
-		
+
 		:param values: list of values
-		:type values: list of int or list of float or list of decimal.Decimal
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		self.m_listCtrl.DeleteAllItems()
-		for i in range(len(values)):
-			self.m_listCtrl.InsertItem(i, str(values[i]))
-		
+		for idx, value in enumerate(values):
+			self.m_listCtrl.InsertItem(idx, str(value))
+
 		self.m_listCtrl.InsertItem(len(values), '')
 		self.m_listCtrl.SetItemState(0, wx.LIST_STATE_SELECTED, wx.LIST_STATE_SELECTED)
-	
+
 	def GetStrings(self):
 		return self.GetValues()
-	
+
 	def GetValues(self):
 		"""
 		Returns a list of the current contents of the control.
-		
+
 		:return:
 		:rtype:
 		"""
-		
+
 		values = []
-		
+
 		for i in range(self.m_listCtrl.GetItemCount()):
 			val = self.m_listCtrl.GetItemText(i)
 			if val:
 				if self.decimal_places == -1:
 					# Don't format
 					values.append(Decimal(val))
 				else:
 					values.append(rounders(val, self._rounders_string))
-		
+
 		return values
-	
+
 	def SetupEditControl(self):
 		edit_control = self.m_listCtrl.GetEditControl()
 		print(edit_control)
 		edit_control.SetValidator(FloatValidator(5))
-		
+
 		# Bind Events
 		edit_control.Bind(wx.EVT_TEXT, self.on_value_changed)
 		edit_control.Bind(wx.EVT_TEXT_ENTER, self.on_value_changed)
-	
+
 	def on_value_changed(self, event):  # wxGlade: CalibreMeasurementPanel.<event_handler>
 		value = event.GetEventObject().GetValue()
-		
-		if value == ".":
+
+		if value == '.':
 			event.GetEventObject().ChangeValue("0.")
 			wx.CallAfter(event.GetEventObject().SetInsertionPointEnd)
-			
+
 		event.Skip()
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/panel_listctrl.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/panel_listctrl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  panel_listctrl.py
 """
 A custom Panel that acts as a ListCtrl for other wx.Panel objects.
 
 An example ListItem exists that provides two StaticText fields and
 can be used as the basis for custom list items
@@ -26,341 +25,327 @@
 #  MA 02110-1301, USA.
 #
 # generated by wxGlade 0.9.2 on Thu Jan 16 16:34:51 2020
 #
 
 # stdlib
 import pathlib
+from typing import Dict, List, Union
 
 # 3rd party
-import wx
+import wx  # type: ignore
+from typing_extensions import Literal
 
 # this package
 from domdf_wxpython_tools.panel_listctrl.css_parser import parse_css, parse_css_file
 from domdf_wxpython_tools.panel_listctrl.font_parser import parse_font
 
+__all__ = ["PanelListCtrl", "PanelListItem"]
 
 # begin wxGlade: dependencies
 # end wxGlade
 
 # begin wxGlade: extracode
 # end wxGlade
 
 
 class PanelListCtrl(wx.ScrolledWindow):
+
 	def __init__(
-			self, parent, id=wx.ID_ANY, pos=wx.DefaultPosition, size=wx.DefaultSize,
-			style=wx.TAB_TRAVERSAL, name=wx.PanelNameStr, left_padding=32):
-			
+			self,
+			parent: wx.Window,
+			id=wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			pos=wx.DefaultPosition,
+			size=wx.DefaultSize,
+			style=wx.TAB_TRAVERSAL,
+			name=wx.PanelNameStr,
+			left_padding=32
+			):
+
 		wx.ScrolledWindow.__init__(self, parent, id, pos=pos, size=size, style=style | wx.TAB_TRAVERSAL, name=name)
 
-		self._items = []
+		self._items: List[PanelListItem] = []
 		self.parent = parent
 		self.left_padding = left_padding
 
 		self.SetScrollRate(10, 10)
-		
+
 		self.sizer_1 = wx.BoxSizer(wx.VERTICAL)
 		self.SetSizer(self.sizer_1)
 		self.sizer_1.Fit(self)
-		
+
 		self.Layout()
-		
+
 		self.Bind(wx.EVT_LIST_ITEM_SELECTED, self._on_selection_changed)
 		self.Bind(wx.EVT_LIST_KEY_DOWN, self._on_key_down)
-		
+
 		self.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_LISTBOX))
-		
+
 	def _on_selection_changed(self, event):
 		"""
-		Handler for EVT_LIST_ITEM_SELECTED, triggered by clicking on an Item
+		Handler for EVT_LIST_ITEM_SELECTED, triggered by clicking on an Item.
 		"""
-		
+
 		for item in self._items:
 			if item == event.GetEventObject():
 				item.SelectItem()
 			else:
 				item.DeselectItem()
-		
+
 		event.Skip()
 
-	def _on_key_down(self, event):
+	def _on_key_down(self, event) -> None:
 		"""
-		Handler for EVT_LIST_KEY_DOWN, triggered by pressing key on keyboard when an item is focused
+		Handler for EVT_LIST_KEY_DOWN, triggered by pressing key on keyboard when an item is focused.
 		"""
-		
+
 		key_code = event.GetKeyCode()
 		index = self.GetItemPosition(event.GetEventObject())
 
 		self.DeselectAll()
-		
+
 		if key_code == wx.WXK_UP:
 			index = index - 1
 		elif key_code == wx.WXK_DOWN:
 			index = index + 1
-		
+
 		if key_code == wx.WXK_PAGEUP:
 			index = index - 5
 		elif key_code == wx.WXK_PAGEDOWN:
 			index = index + 5
-		
+
 		if index >= self.GetItemCount():
-			index = self.GetItemCount()-1
+			index = self.GetItemCount() - 1
 		elif index < 0:
 			index = 0
-		
+
 		self.Select(index)
-		
+
 		event.Skip()
 		# TODO: Keyboard autocompletion?
 
-	def SetSelection(self, idx):
+	def SetSelection(self, idx: int):
 		"""
-		Set the current selection to the item at the given index
-		
-		:param idx: index of the item to select
-		:type idx: int
+		Set the current selection to the item at the given index.
+
+		:param idx: index of the item to select.
 		"""
-		
+
 		item_to_select = self.GetItem(idx)
-		
+
 		for item in self._items:
 			if item == item_to_select:
 				item.SelectItem()
 			else:
 				item.DeselectItem()
-	
+
 	def DeselectAll(self):
 		"""
-		Deselect all items
+		Deselect all items.
 		"""
-		
+
 		for i in range(self.GetItemCount()):
 			self.Select(i, False)
-	
-	def AcceptsFocus(self):
+
+	def AcceptsFocus(self):  # noqa: D400
 		return True
-	
+
 	def AcceptsFocusFromKeyboard(self):
 		return False
-	
-	def Append(self, panel_list_item):
+
+	def Append(self, panel_list_item: "PanelListItem"):
 		"""
 		Append a 'PanelListItem' object, or an instance of a custom subclass, to the control.
 		"""
-		
+
 		self.sizer_1.Add(panel_list_item, 0, wx.EXPAND, wx.TOP, 0)
 		self._items.append(panel_list_item)
 		self.sizer_1.Fit(self)
 		self.Layout()
 
-	def AppendNewItem(self, text_dict, style_data):
+	def AppendNewItem(self, text_dict: Dict, style_data) -> "PanelListItem":
 		"""
 		Append a new 'PanelListItem' object to the control, passing the 'text_dict' and 'style_data'
 		parameters to the new object.
-		
+
 		:param text_dict:
-		:type text_dict:
 		:param style_data:
-		:type style_data:
-		
+
 		:return: The new PanelListItem object that was added to the control
-		:rtype:
 		"""
-		
+
 		item = PanelListItem(self, text_dict, style_data, left_padding=self.left_padding)
 		self.Append(item)
 		return item
-		
+
 	def Clear(self):
 		"""
 		Removes all items from the control
 		"""
-		
+
 		for item in self._items:
 			self.sizer_1.Hide(item)
 			self.sizer_1.Remove(0)
-			
+
 			item.Destroy()
 			self.Layout()
-		
+
 		self._items = []
-		
+
 		event = wx.ListEvent(wx.wxEVT_LIST_DELETE_ALL_ITEMS)
 		event.SetEventObject(self)
 		wx.PostEvent(self, event)
-		
+
 		return True
-	
-	def DeleteItem(self, item):
+
+	def DeleteItem(self, item) -> bool:
 		"""
 		Deletes the specified item from the control.
-		
+
 		:param item:
-		:type item:
-		
-		:return: True if the item was removed, False otherwise (usually because the item wasn't in the control)
-		:rtype: bool
+
+		:return: :py:obj:`True` if the item was removed, :py:obj:`False` otherwise
+			(usually because the item wasn't in the control)
 		"""
-		
+
 		for index, widget in enumerate(self._items):
 			if widget == item:
 				self.sizer_1.Hide(self._items.pop(index))
 				self.sizer_1.Remove(index)
-				
+
 				item.Destroy()
-				
+
 				self.Layout()
-				
+
 				event = wx.ListEvent(wx.wxEVT_LIST_DELETE_ITEM)
 				event.SetEventObject(self)
 				wx.PostEvent(self, event)
-				
+
 				return True
-		
+
 		return False
 
 	def Focus(self, idx):
-		""" Set Focus to the the given item. """
+		"""
+		Set Focus to the the given item.
+
+		:param idx:
+		"""
+
 		for index, item in enumerate(self._items):
 			if index == idx:
 				item.SelectItem()
 			else:
 				item.DeselectItem()
 
 	def GetColumnCount(self):
 		"""
 		Returns the number of columns.
 		"""
-		
+
 		return 1
 
 #
-# 	def GetCountPerPage(self):
+# 	def GetCountPerPage(self) -> int:
 # 		"""
 # 		GetCountPerPage() -> int
 #
 # 		Gets the number of items that can fit vertically in the visible area
 # 		of the list control (list or report view) or the total number of items
 # 		in the list control (icon or small icon view).
 # 		"""
 # 		return 0
 #
-	
-	def GetFirstSelected(self, *args):
+
+	def GetFirstSelected(self, *_) -> int:
 		"""
 		Returns the first selected item, or -1 when none is selected.
-		
-		:param args:
-		:type args:
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		for item in self._items:
 			if item.IsSelected():
 				return item
-		
+
 		return -1
 
 	def GetFocusedItem(self):
 		"""
 		Gets the currently focused item or -1 if none is focused.
-		
+
 		:return:
 		:rtype:
 		"""
-		
+
 		for item in self._items:
 			if item.IsSelected():
 				return item
-		
+
 		return -1
 
-	def GetItem(self, itemIdx, *args):
+	def GetItem(self, itemIdx, *_):
 		"""
-		GetItem(itemIdx, col=0) -> ListItem
+		Returns information about the item. See :meth:`~.SetItem` for more information.
 
-		Gets information about the item. See SetItem() for more information.
-		
 		:param itemIdx:
-		:type itemIdx:
-		:param args:
-		:type args:
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		return self._items[itemIdx]
-		
-	def GetItemBackgroundColour(self, item):
-		"""
-		GetItemBackgroundColour(item) -> Colour
 
+	def GetItemBackgroundColour(self, item) -> wx.Colour:
+		"""
 		Returns the colour for this item.
 		"""
-		
+
 		return item.GetBackgroundColour()
 
-	def GetItemCount(self):
+	def GetItemCount(self) -> int:
 		"""
 		Returns the number of items in the list control.
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		return len(self._items)
 
-	def GetItemPosition(self, item):
+	def GetItemPosition(self, item) -> int:
 		"""
-		GetItemPosition(item) -> Point
-
-		Returns the position of the item, or -1 if it is not found
+		Returns the position of the item, or ``-1`` if it is not found.
 		"""
+
 		if item in self._items:
 			return self._items.index(item)
-		
+
 		return -1
 
 	def GetNextSelected(self, item):
 		"""
 		Returns subsequent selected items, or -1 when no more are selected.
-		
+
 		:param item:
-		:type item:
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		index_of_item = self.GetItemPosition(item)
-		
+
 		for index, item in enumerate(self._items):
 			if index <= index_of_item:
 				continue
 			if item.IsSelected():
 				return item
-		
+
 		return -1
 
-	def GetSelectedItemCount(self):
+	def GetSelectedItemCount(self) -> int:
 		"""
-		GetSelectedItemCount() -> int
-
 		Returns the number of selected items in the list control.
 		"""
+
 		selected_item_count = 0
-		
+
 		for item in self._items:
 			if item.IsSelected():
 				selected_item_count += 1
-		
+
 		return selected_item_count
 #
 # 	def HitTest(self, point):
 # 		"""
 # 		HitTest(point) -> (long, flags)
 #
 # 		Determines which item (if any) is at the specified point, giving
@@ -375,327 +360,345 @@
 # 		InsertItem(index, imageIndex) -> long
 # 		InsertItem(index, label, imageIndex) -> long
 #
 # 		Inserts an item, returning the index of the new item if successful, -1
 # 		otherwise.
 # 		"""
 # 		return 0
-		# TODO: Trigger EVT_LIST_INSERT_ITEM
+# TODO: Trigger EVT_LIST_INSERT_ITEM
 #
+
 	def IsEmpty(self):
 		"""
 		Returns true if the control doesn't currently contain any items.
-		
+
 		:return:
 		:rtype:
 		"""
-		
+
 		return bool(self._items)
 
 	def IsSelected(self, idx):
 		"""
-		Returns ``True`` if the item is selected.
-		
+		Returns ``:py:obj:`True``` if the item is selected.
+
 		:param idx:
-		:type idx:
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		return self._items[idx].IsSelected()
 
 	def RefreshItem(self, item):
 		"""
 		Redraws the given item.
-		
+
 		:param item:
-		:type item:
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		item.Layout()
 		item.Refresh()
 
 	def RefreshItems(self, itemFrom, itemTo):
 		"""
 		Redraws the items between itemFrom and itemTo.
-		
+
 		:param itemFrom:
-		:type itemFrom:
 		:param itemTo:
-		:type itemTo:
-		
-		:return:
-		:rtype:
 		"""
-		
-		for index in range(itemFrom, itemTo+1):
+
+		for index in range(itemFrom, itemTo + 1):
 			self.RefreshItem(self._items[index])
 #
-# 	def ScrollList(self, dx, dy):
+# 	def ScrollList(self, dx, dy) -> bool:
 # 		"""
 # 		ScrollList(dx, dy) -> bool
 #
 # 		Scrolls the list control.
 # 		"""
 # 		return False
 
-	def Select(self, idx, on=1):
+	def Select(self, idx, on: int = 1):
 		"""
 		Selects/deselects an item.
-		
+
 		:param idx:
-		:type idx:
 		:param on:
-		:type on:
-		
-		:return:
-		:rtype:
 		"""
-		
+
 		self._items[idx].SelectItem(on)
 
-# 	def SortItems(self, fnSortCallBack):
+# 	def SortItems(self, fnSortCallBack) -> bool:
 # 		"""
 # 		SortItems(fnSortCallBack) -> bool
 #
 # 		Call this function to sort the items in the list control.
 # 		"""
 # 		return False
-#
+
 	@property
-	def ColumnCount(self):
+	def ColumnCount(self) -> int:
 		"""
 		Returns the number of columns.
-		
+
 		:rtype: int
 		"""
 		return 1
 
 #
 # 	CountPerPage = property(lambda self: object(), lambda self, v: None, lambda self: None)  # default
 # 	"""GetCountPerPage() -> int
 #
 # Gets the number of items that can fit vertically in the visible area
 # of the list control (list or report view) or the total number of items
 # in the list control (icon or small icon view)."""
 #
 #
+
 	@property
 	def FocusedItem(self):
 		"""
 		Gets the currently focused item or -1 if none is focused.
-		
+
 		:return:
 		:rtype:
 		"""
-		
+
 		return self.GetFocusedItem()
 
-	
 	@property
-	def ItemCount(self):
+	def ItemCount(self) -> int:
 		"""
 		Returns the number of items in the list control.
-		
+
 		:rtype: int
 		"""
 		return len(self._items)
 
+
 # end of class RecentProjectsPanel
 
 
 class PanelListItem(wx.Panel):
+	"""
+
+	:param parent: The PanelListCtrl the item is to go into
+	:param text_dict:
+	:param style_data:
+	:param id: An identifier for the panel. ID_ANY is taken to mean a default.
+	:param style: The window style. See wx.Panel.
+	:param name: Window name
+	:param left_padding: the spacing to the left of the text in the control
+	"""
+
 	def __init__(
-			self, parent, text_dict, style_data, id=wx.ID_ANY,
-			style=0, name=wx.PanelNameStr, left_padding=32
+			self,
+			parent: PanelListCtrl,
+			text_dict: Dict,
+			style_data,
+			id: int = wx.ID_ANY,  # noqa: A002  # pylint: disable=redefined-builtin
+			style: int = 0,
+			name: str = wx.PanelNameStr,
+			left_padding: int = 32,
 			):
-		"""
-		
-		:param parent: The PanelListCtrl the item is to go into
-		:type parent: PanelListCtrl
-		:param text_dict:
-		:type text_dict:
-		:param style_data:
-		:type style_data:
-		:param id: An identifier for the panel. ID_ANY is taken to mean a default.
-		:type id: wx.WindowID
-		:param style: The window style. See wx.Panel.
-		:type style: int
-		:param name: Window name
-		:type name: str
-		:param left_padding: the spacing to the left of the text in the control
-		:type left_padding: int
-		"""
-		
+
 		self.parent = parent
-		
+
 		if not isinstance(text_dict, dict):
 			raise TypeError("'text_dict' must be a dict containing 'css class:text' pairs")
-		
+
 		if isinstance(style_data, pathlib.Path):
 			# Filename provided
 			style_data = parse_css_file(style_data)
 		if isinstance(style_data, str):
 			# Filename or css provided
 			try:
 				# CSS
 				style_data = parse_css(style_data)
 			except ValueError:
 				# Filename
 				style_data = parse_css_file(style_data)
-		
+
 		elif not isinstance(style_data, dict):
-			raise TypeError("""'style_data' must be either:
+			raise TypeError(
+					"""'style_data' must be either:
 	> A string or pathlib.Path object pointing to a css file, or
 	> A dictionary containing the style data, or
-	> A string containing css properties.""")
-		
+	> A string containing css properties."""
+					)
+
 		self.style_data = style_data
-		
+
 		wx.Panel.__init__(self, parent, id, style=style | wx.TAB_TRAVERSAL | wx.WANTS_CHARS, name=name)
-		
+
 		self.selected = False
-		
+
 		# Bind events
 		self.Bind(wx.EVT_LEFT_UP, self.OnClick)
 		self.Bind(wx.EVT_LEFT_DCLICK, self.OnDoubleClick)
 		self.Bind(wx.EVT_MIDDLE_UP, self.OnMiddleClick)
 		self.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
 
 		# for wxMSW
 		self.Bind(wx.EVT_COMMAND_RIGHT_CLICK, self.OnRightClick)
-		
+
 		# for wxGTK
 		self.Bind(wx.EVT_RIGHT_UP, self.OnRightClick)
-		
+
 		# Background colour settings for panel
 		if "li" in self.style_data and "background-color" in self.style_data["li"]:
 			self._default_background = self.style_data["li"]["background-color"]
 		else:
 			self._default_background = wx.SystemSettings.GetColour(wx.SYS_COLOUR_LISTBOX)
-		
+
 		if "li::selection" in self.style_data and "background-color" in self.style_data["li::selection"]:
 			self._selected_background = self.style_data["li::selection"]["background-color"]
 		else:
 			self._selected_background = wx.SystemSettings.GetColour(wx.SYS_COLOUR_MENUHILIGHT)
-		
+
 		self._items = {}
-		self._text_properties = {}
-		
+		self._text_properties: Dict = {}
+
 		self.outer_sizer = wx.BoxSizer(wx.HORIZONTAL)
 		main_grid = wx.FlexGridSizer(len(text_dict), 2, 0, left_padding)
-		
+
 		for index, (css_class, text) in enumerate(text_dict.items()):
 			widget = wx.StaticText(self, wx.ID_ANY, text, style=wx.ST_ELLIPSIZE_MIDDLE)
 			self._items[css_class] = widget
-			
+
 			if index == 0:
 				main_grid.Add((0, 0), 0, 0, 0)
 				main_grid.Add(widget, 0, wx.TOP, 6)
 			else:
 				main_grid.Add((0, 0), 0, 0, 0)
 				main_grid.Add(widget, 0, wx.TOP, 0 if wx.Platform == "__WXGTK__" else 2)
-			
+
 			widget.Bind(wx.EVT_LEFT_UP, self.OnClick)
 			widget.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
 			widget.Bind(wx.EVT_LEFT_DCLICK, self.OnDoubleClick)
 			widget.Bind(wx.EVT_MIDDLE_UP, self.OnMiddleClick)
 			# for wxMSW
 			widget.Bind(wx.EVT_COMMAND_RIGHT_CLICK, self.OnRightClick)
-			
+
 			# for wxGTK
 			widget.Bind(wx.EVT_RIGHT_UP, self.OnRightClick)
-		
+
 		self.outer_sizer.Add(main_grid, 0, wx.BOTTOM, 4)
-		
+
 		self.SetSizer(self.outer_sizer)
 		self.outer_sizer.Fit(self)
 		self.Layout()
-		
+
 		self.Refresh()
-	
-	def SelectItem(self, select=True):
+
+	def SelectItem(self, select: bool = True):
+		"""
+		Select (or deselect) the given item.
+
+		:param select: If :py:obj:`False` the item is deselected.
+		"""
+
 		self.selected = select
 		if select:
 			self.SetFocus()
 		self.Refresh()
-	
-	def DeselectItem(self):
+
+	def DeselectItem(self):  # noqa: D102
 		self.selected = False
 		self.Refresh()
 		event = wx.ListEvent(wx.wxEVT_LIST_ITEM_DESELECTED)
 		event.SetEventObject(self)
 		wx.PostEvent(self, event)
-	
-	def OnRightClick(self, event):
+
+	def OnRightClick(self, _) -> None:  # noqa: D102
 		event = wx.ListEvent(wx.wxEVT_LIST_ITEM_RIGHT_CLICK)
 		event.SetEventObject(self)
 		wx.PostEvent(self, event)
-	
-	def OnMiddleClick(self, event):
+
+	def OnMiddleClick(self, _) -> None:  # noqa: D102
 		event = wx.ListEvent(wx.wxEVT_LIST_ITEM_RIGHT_CLICK)
 		event.SetEventObject(self)
 		wx.PostEvent(self, event)
-	
-	def OnClick(self, event):
+
+	def OnClick(self, _) -> None:  # noqa: D102
 		event = wx.ListEvent(wx.wxEVT_LIST_ITEM_SELECTED)
 		event.SetEventObject(self)
 		wx.PostEvent(self, event)
-		
-	def OnDoubleClick(self, event):
+
+	def OnDoubleClick(self, _) -> None:  # noqa: D102
 		event = wx.ListEvent(wx.wxEVT_LIST_ITEM_ACTIVATED)
 		event.SetEventObject(self)
 		wx.PostEvent(self, event)
 
-	def OnKeyDown(self, event):
+	def OnKeyDown(self, event) -> None:
+		"""
+
+		:param event: The wxPython event.
+		"""
+
 		key_event = event
 		event = wx.ListEvent(wx.wxEVT_LIST_KEY_DOWN)
 		event.SetEventObject(self)
 		event.SetKeyCode(key_event.GetKeyCode())
 		wx.PostEvent(self, event)
-	
-	def IsSelected(self):
+
+	def IsSelected(self) -> bool:
+		"""
+		Returns whether the :class:`~.PanelListItem` is selected.
+		"""
+
 		return self.selected
-	
+
 	def _refresh_background_colour(self):
 		if self.selected:
 			wx.Panel.SetBackgroundColour(self, self._selected_background)
 		else:
 			wx.Panel.SetBackgroundColour(self, self._default_background)
-	
+
 	def _refresh_text(self):
 		for classname, widget in self._items.items():
 			if self.selected:
 				class_style_data = self.style_data[f"li p.{classname}::selection"]
 			else:
 				class_style_data = self.style_data[f"li p.{classname}"]
-				
+
 			colour, font_data = parse_font(class_style_data)
-			
+
 			widget.SetForegroundColour(colour)
 			widget.SetFont(wx.Font(**font_data))
-	
-	def SetBackgroundColour(self, colour):
+
+	def SetBackgroundColour(self, colour) -> None:
+		"""
+		Set the background colour for the item.
+
+		:param colour:
+		"""
+
 		self._default_background = colour
-	
-	def SetSelectedBackgroundColour(self, colour):
+
+	def SetSelectedBackgroundColour(self, colour) -> None:
+		"""
+		Set the background colour for the item when it is selected.
+
+		:param colour:
+		"""
+
 		self._selected_background = colour
-	
+
 	def GetBackgroundColour(self):
 		return self._default_background
-	
+
 	def GetCurrentBackgroundColour(self):
+		"""
+		Returns the current background colour of the :class`wx.Panel` class.
+		"""
+
 		return wx.Panel.GetBackgroundColour(self)
-	
+
 	def Refresh(self, **kwargs):
 		self._refresh_background_colour()
 		self._refresh_text()
 		wx.Panel.Refresh(self)
-	
+
 	def GetContents(self):
 		return self._items.values()
 
-# end of class RecentProjectItem
+
+# end of class RecentProjectItem
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/constants.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  constants.py
 """
-Constants for panel_listctrl
+Constants for :mod:`~.panel_listctrl`.
 """
 #
 #  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
@@ -21,35 +20,41 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 
 # 3rd party
 import webcolors
-import wx
+import wx  # type: ignore
 
 # Default text settings
 text_defaults = {
 		"color": webcolors.name_to_hex("black"),
 		"font-size": "11pt",
 		"font-family": "default",
 		"font-style": "normal",
 		"font-weight": "normal",
 		"text-decoration": "none",
-		"font-face-name": ''
+		"font-face-name": '',
 		}
 
 if wx.Platform == "__WXMSW__":
 	text_defaults["font-size"] = "9pt"
 elif wx.Platform == "__WXGTK__":
 	text_defaults["font-size"] = "11pt"
-	import lsb_release
-	
-	if "Ubuntu" in lsb_release.get_distro_information().values():
-		text_defaults["font-face-name"] = "Ubuntu"
+
+	try:
+		# 3rd party
+		import lsb_release  # type: ignore
+
+		if "Ubuntu" in lsb_release.get_distro_information().values():
+			text_defaults["font-face-name"] = "Ubuntu"
+
+	except ImportError:
+		pass
 
 # System colours
 sys_colour_lookup = {
 		"SYS_COLOUR_SCROLLBAR": wx.SYS_COLOUR_SCROLLBAR,
 		"SYS_COLOUR_DESKTOP": wx.SYS_COLOUR_DESKTOP,
 		"SYS_COLOUR_BACKGROUND": wx.SYS_COLOUR_DESKTOP,
 		"SYS_COLOUR_ACTIVECAPTION": wx.SYS_COLOUR_ACTIVECAPTION,
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/font_parser.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/font_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  font_parser.py
 #
 #  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Function 'freezeargs' Copyright 2018 Cedar
 #  https://stackoverflow.com/users/5810747/cedar
@@ -27,87 +26,92 @@
 #
 # generated by wxGlade 0.9.2 on Thu Jan 16 16:34:51 2020
 #
 
 # stdlib
 import re
 from functools import lru_cache, wraps
+from typing import Callable, Dict, Tuple, cast
 
 # 3rd party
-from frozendict import frozendict
+from cawdrey import frozendict
 
+__all__ = ["freezeargs", "parse_font"]
 
-def freezeargs(func):
-	"""
-	Make mutable dictionary immutable for lru_cache
 
-	From stackoverflow.com/a/53394430
+def freezeargs(func: Callable) -> Callable:
+	"""
+	Makes a mutable dictionary immutable, so it can be used as an argument for :func:`slru_cache`.
 	"""
-	
+
+	# From stackoverflow.com/a/53394430
+
 	@wraps(func)
 	def wrapped(*args, **kwargs):
-		args = tuple(
-				[frozendict(arg) if isinstance(arg, dict) else arg for arg in args])
+		args = tuple([frozendict(arg) if isinstance(arg, dict) else arg for arg in args])
 		kwargs = {k: frozendict(v) if isinstance(v, dict) else v for k, v in kwargs.items()}
 		return func(*args, **kwargs)
-	
+
 	return wrapped
 
 
 @freezeargs
 @lru_cache(5)
-def parse_font(style_dict):
+def parse_font(style_dict: Dict) -> Tuple[str, Dict]:
 	"""
-	Parse the font from the style_dict
-	
+	Parse the font from the ``style_dict``.
+
 	:param style_dict: Dictionary containing styling information for the font
-	:type style_dict: dict
-	
+
 	:return: Tuple containing the colour of the font, and the font properties
-	:rtype: (str, dict)
-	
+
 	The font properties dictionary returned will contain the following keys:
-	
-		family (wx.FontFamily) – The font family: a generic portable way of referring to fonts without specifying a facename. This parameter must be one of the wx.FontFamily enumeration values. If the faceName argument is provided, then it overrides the font family.
-		
-		style (wx.FontStyle) – One of wx.FONTSTYLE_NORMAL, wx.FONTSTYLE_SLANT and wx.FONTSTYLE_ITALIC.
-		
-		weight (wx.FontWeight) – Font weight, sometimes also referred to as font boldness. One of the wx.FontWeight enumeration values.
-		
-		underline (wx.bool) – The value can be True or False. At present this has an effect on Windows and Motif 2.x only.
-		
-		faceName (wx.string) – An optional string specifying the face name to be used. If it is an empty string, a default face name will be chosen based on the family.
-		
-		encoding (wx.FontEncoding) – An encoding which may be one of the enumeration values of wx.FontEncoding. If the specified encoding isn’t available, no font is created (see also Font Encodings).
-	
+
+	* family (:class:`wx.FontFamily`) – The font family: a generic portable way of referring to fonts without specifying a facename. This parameter must be one of the wx.FontFamily enumeration values. If the faceName argument is provided, then it overrides the font family.
+
+	* style (:class:`wx.FontStyle`) – One of :py:obj:`wx.FONTSTYLE_NORMAL`, :py:obj:`wx.FONTSTYLE_SLANT` and :py:obj:`wx.FONTSTYLE_ITALIC`.
+
+	* weight (:class:`wx.FontWeight`) – Font weight, sometimes also referred to as font boldness. One of the wx.FontWeight enumeration values.
+
+	* underline (:class:`wx.bool`) – The value can be :py:obj:`True` or :py:obj:`False`. At present this has an effect on Windows and Motif 2.x only.
+
+	* faceName (:class:`str) –` An optional string specifying the face name to be used. If it is an empty string, a default face name will be chosen based on the family.
+
+	* encoding (:class:`wx.FontEncoding`) – An encoding which may be one of the enumeration values of wx.FontEncoding. If the specified encoding isn't available, no font is created (see also Font Encodings).
+
 	and one of:
-	
-		pointSize (int) – Size in points. See SetPointSize for more info. Notice that, for historical reasons, the value 70 here is interpreted at DEFAULT and results in creation of the font with the default size and not of a font with the size of 70pt. If you really need the latter, please use SetPointSize(70). Note that this constructor and the matching Create() method overload are the only places in wx.Font API handling DEFAULT specially: neither SetPointSize nor the constructor taking wx.FontInfo handle this value in this way.
-		
-		pixelSize (wx.Size) – Size in pixels. See SetPixelSize for more info.
+
+	* pointSize (:class:`int`) – Size in points. See SetPointSize for more info. Notice that, for historical reasons, the value 70 here is interpreted at DEFAULT and results in creation of the font with the default size and not of a font with the size of 70pt. If you really need the latter, please use SetPointSize(70). Note that this constructor and the matching Create() method overload are the only places in wx.Font API handling DEFAULT specially: neither SetPointSize nor the constructor taking wx.FontInfo handle this value in this way.
+
+	* pixelSize (:class:`wx.Size`) – Size in pixels. See SetPixelSize for more info.
 
 	depending on the font size specified in 'style_dict'
 	"""
-	
+
 	colour = style_dict["color"]
-	
+
 	font_data = {
 			"family": style_dict["font-family"],
 			"style": style_dict["font-style"],
 			"weight": style_dict["font-weight"],
-			"faceName": style_dict["font-face-name"]
+			"faceName": style_dict["font-face-name"],
 			}
-	
+
 	if style_dict["text-decoration"].lower() == "underline":
 		font_data["underline"] = True
-	
+
 	# if style_dict["font-size"] is None:
 	# 	font_data["pointSize"] = None
 	# else:
-	font_size_value, pt_or_px = filter(None, re.split("(\d+|\D+)", style_dict["font-size"]))
+
+	font_size_value: str
+	pt_or_px: str
+	font_size_value, pt_or_px = filter(None, re.split(r"(\d+|\D+)", style_dict["font-size"]))
+
+	pt_or_px = cast(str, pt_or_px)
 
 	if pt_or_px.lower() == "pt":
 		font_data["pointSize"] = int(font_size_value)
 	elif pt_or_px.lower() == "px":
 		font_data["pixelSize"] = int(font_size_value)
 
 	return colour, font_data
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/__init__.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  __init__.py
 """
 A custom Panel that acts as a ListCtrl for other wx.Panel objects.
 
 An example ListItem exists that provides two StaticText fields and
 can be used as the basis for custom list items
 """
 #
+#  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -28,12 +28,12 @@
 # generated by wxGlade 0.9.2 on Thu Jan 16 16:34:51 2020
 #
 
 # stdlib
 from pathlib import Path
 
 # this package
-from domdf_wxpython_tools.panel_listctrl.panel_listctrl import PanelListCtrl, PanelListItem
 from domdf_wxpython_tools.panel_listctrl.css_parser import parse_css, parse_css_file
 from domdf_wxpython_tools.panel_listctrl.font_parser import parse_font
+from domdf_wxpython_tools.panel_listctrl.panel_listctrl import PanelListCtrl, PanelListItem
 
 default_css = Path(__file__).parent / "Default.css"
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/panel_listctrl/css_parser.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/panel_listctrl/css_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 #  css_parser.py
 #
 #  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
@@ -19,172 +18,172 @@
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 # generated by wxGlade 0.9.2 on Thu Jan 16 16:34:51 2020
 #
 
+# stdlib
+from typing import Dict
+
 # 3rd party
-import tinycss
+import tinycss  # type: ignore
 import webcolors
-import wx
+import wx  # type: ignore
+from domdf_python_tools.typing import PathLike
 
 # this package
-from domdf_wxpython_tools.panel_listctrl.constants import text_defaults, sys_colour_lookup
+from domdf_wxpython_tools.panel_listctrl.constants import sys_colour_lookup, text_defaults
 
+__all__ = ["parse_css_file", "parse_css"]
 
 # Setup tinycss
 parser = tinycss.make_parser("page3")
 
 
-def parse_css_file(filename):
+def parse_css_file(filename: PathLike) -> Dict:
 	"""
-	Parse the stylesheet in the given file
-	
-	:param filename: The filename of the stylesheet to parse
-	:type filename: str or pathlib.Path
-	
-	:return: Parsed CSS stylesheet
-	:rtype: dict
+	Parse the stylesheet in the given file.
+
+	:param filename: The filename of the stylesheet to parse.
+
+	:return: Parsed CSS stylesheet.
 	"""
-	
+
 	stylesheet = parser.parse_stylesheet_file(css_file=str(filename))
-	
+
 	return _parse_css(stylesheet)
 
 
-def parse_css(css_data):
+def parse_css(css_data: str) -> Dict:
 	"""
 	Parse the stylesheet from the given string
 
 	:param css_data: A string representing a CSS stylesheel
-	:type css_data: str
 
 	:return: Parsed CSS stylesheet
-	:rtype: dict
 	"""
-	
+
 	stylesheet = parser.parse_stylesheet(css_unicode=css_data)
-	
+
 	return _parse_css(stylesheet)
 
 
-def _parse_css(stylesheet):
+def _parse_css(stylesheet: tinycss.css21.Stylesheet) -> Dict:
 	"""
-	Internal function for actual parsing of css
-	
-	:param stylesheet: A tinycss parsed stylesheel
-	:type stylesheet: :class:`tinycss.css21.Stylesheet`
-	:return: Parsed CSS stylesheet
-	:rtype: dict
+	Internal function for actual parsing of css.
+
+	:param stylesheet: A tinycss parsed stylesheet.
+
+	:return: Parsed CSS stylesheet.
 	"""
-	
+
 	if stylesheet.errors:
 		raise ValueError(stylesheet.errors[0])
-	
-	styles = {}
-	
+
+	styles = {}  # type: ignore
+
 	# Remove declarations for other platforms and make
-	
+
 	for rule in stylesheet.rules:
 		styles[rule.selector.as_css()] = {}
-		
+
 		for declaration in rule.declarations:
 			name = declaration.name
 			value = declaration.value.as_css()
-			
+
 			if "color" in name:
 				value.lstrip("wx.")
-				
+
 				if value.startswith("SYS_COLOUR"):
 					# wx.SystemColour
 					if value in sys_colour_lookup:
 						value = wx.SystemSettings.GetColour(sys_colour_lookup[value])
 					else:
-						raise ValueError(f"""wx.SystemColour 'value' not recognised.
-See https://wxpython.org/Phoenix/docs/html/wx.SystemColour.enumeration.html for the list of valid values""")
-				
-				elif value.startswith("#"):
+						raise ValueError(
+								f"""wx.SystemColour 'value' not recognised.
+See https://wxpython.org/Phoenix/docs/html/wx.SystemColour.enumeration.html for the list of valid values"""
+								)
+
+				elif value.startswith('#'):
 					# Hex value, pass to wx.Colour directly
 					pass
-				
+
 				elif value.startswith("rgb("):
 					# RGB value, convert to hex
-					rgb_triplet = (int(x) for x in value.lstrip("rgb(").rstrip(")").split(","))
-					value = webcolors.rgb_to_hex(rgb_triplet)
-				
+					rgb_triplet = tuple(int(x) for x in value.lstrip("rgb(").rstrip(')').split(','))
+					value = webcolors.rgb_to_hex(rgb_triplet)  # type: ignore
+
 				else:
 					# Named colour, convert to hex
 					value = webcolors.name_to_hex(value)
-			
+
 			if name == "font-family":
 				if value == "decorative":
 					value = wx.FONTFAMILY_DECORATIVE
-				
+
 				elif value == "roman":
 					value = wx.FONTFAMILY_ROMAN
-				
+
 				elif value == "script":
 					value = wx.FONTFAMILY_SCRIPT
-				
+
 				elif value == "swiss":
 					value = wx.FONTFAMILY_SWISS
-				
+
 				elif value == "modern":
 					value = wx.FONTFAMILY_MODERN
-				
+
 				else:
 					value = wx.FONTFAMILY_DEFAULT
-			
+
 			elif name == "font-style":
 				if value == "slant":
 					value = wx.FONTSTYLE_SLANT
 				elif value == "italic":
 					value = wx.FONTSTYLE_ITALIC
 				else:
 					value = wx.FONTSTYLE_NORMAL
-			
+
 			elif name == "font-weight":
 				if value == "light":
 					value = wx.FONTWEIGHT_LIGHT
 				elif value == "bolt":
 					value = wx.FONTWEIGHT_BOLD
 				else:
 					value = wx.FONTWEIGHT_NORMAL
-			
+
 			styles[rule.selector.as_css()][name] = value
-	
+
 	# if li p is not styled, use the default values
 	if "li p" not in styles:
 		styles["li p"] = text_defaults.copy()
-	
+
 	# If li p is missing any parameters, add them from the default values
 	styles["li p"] = {**text_defaults, **styles["li p"]}
-	
+
 	# if li p::selection is not styled, use the values from p
 	if "li p::selection" not in styles:
 		styles["li p::selection"] = styles["li p"].copy()
-	
+
 	# If li p is missing any parameters, add them from p
 	styles["li p::selection"] = {**styles["li p"], **styles["li p::selection"]}
-	
+
 	# For each li p class, add undefined values from p
 	for style in styles:
-		if style.split(".")[0] == "li p":
+		if style.split('.')[0] == "li p":
 			if style == "li p":
 				continue
 			if "::selection" in style:
 				continue
 			styles[style] = {**styles["li p"], **styles[style]}
-	
+
 	# For each p::selection class, add undefined values from p::selection
 	for style in styles:
-		if style.split(".")[0] == "li p":
+		if style.split('.')[0] == "li p":
 			if style == "li p::selection":
 				continue
 			if "::selection" not in style:
 				continue
 			styles[style] = {**styles["li p::selection"], **styles[style]}
-	
-	return styles
-
 
+	return styles
```

### Comparing `domdf_wxpython_tools-0.2.5/domdf_wxpython_tools/events.py` & `domdf_wxpython_tools-0.3.0.post1/domdf_wxpython_tools/events.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #  !/usr/bin/env python
-#   -*- coding: utf-8 -*-
+
 #
 #  events.py
 """
 Reusable code for simple events
 
 Usage:
 
@@ -45,120 +45,121 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #
 
+# stdlib
 from collections import OrderedDict
 
-import wx
+# 3rd party
+import wx  # type: ignore
+
+__all__ = ["PayloadEvent", "SimpleEvent"]
 
 
 class PayloadEvent(wx.PyCommandEvent):
-	"""Event containing a message payload"""
-	
+	"""
+	Event containing a message payload.
+	"""
+
 	def __init__(self, etype, eid, value):
-		"""Creates the event object"""
+		"""
+		Creates the event object.
+		"""
+
 		wx.PyCommandEvent.__init__(self, etype, eid)
 		self.value = value
-	
+
 	def GetValue(self):
 		"""Returns the value from the event.
 		@return: the value of this event
 
 		"""
 		return self.value
 
 
-class SimpleEvent(object):
+class SimpleEvent:
 	"""
-	SimpleEvent(receiver, name, event, binder)
+
+	:param receiver:
+	:param name:
 	"""
-	
+
 	_fields = ("receiver", "name", "event", "binder")
-	
-	def __init__(self, receiver=None, name="Event"):
-		"""
 
-		:param receiver:
-		:param name:
-		"""
-		
+	def __init__(self, receiver=None, name="Event"):
 		self.receiver = receiver
 		self.name = name
 		self.event = wx.NewEventType()
 		self.binder = wx.PyEventBinder(self.event, 1)
 		self.value = None
 		self.bindings = {}
-	
+
 	def __repr__(self):
 		"""
-		Return a nicely formatted representation string
+		Return a nicely formatted representation string.
 		"""
-		
+
 		return f'SimpleEvent(name={self.name})'
-	
+
+	@property
 	def __dict__(self):
 		"""
-		Return a new OrderedDict which maps field names to their values
-
-		:return:
-		:rtype: OrderedDict
+		Return a new OrderedDict which maps field names to their values.
 		"""
-		
-		return OrderedDict(zip(self._fields, self))
-	
+
+		return OrderedDict(zip(self._fields, self))  # type: ignore
+
 	def set_receiver(self, receiver):
 		"""
-		Set the class that is to receive the event trigger
+		Set the class that is to receive the event trigger.
 
 		:param receiver:
 		"""
-		
+
 		self.receiver = receiver
-	
+
 	def Bind(self, handler, receiver=None, **kwargs):
 		"""
-		Bind the event to the handler
+		Bind the event to the handler.
 
-		:param handler: handler to bind the event to
-		:param kwargs: keyword arguments to pass through to receiver's Bind method
+		:param handler: handler to bind the event to.
+		:param kwargs: keyword arguments to pass through to receiver's Bind method.
 		"""
 		if receiver is None:
 			receiver = self.receiver
-		
+
 		receiver.Bind(self.binder, handler, **kwargs)
 		self.bindings[receiver] = handler
-	
+
 	# self.receiver.Bind(self.binder, handler, **kwargs)
-	
+
 	def Unbind(self, receiver=None, **kwargs):
 		"""
 		Unbind the event from the handler
 
 		:param kwargs: keyword arguments to pass through to receiver's Unbind method
 		"""
-		
+
 		if receiver:
 			receiver.Unbind(self.binder, handler=self.bindings[receiver], **kwargs)
 		else:
 			for receiver, handler in self.bindings.items():
 				receiver.Unbind(self.binder, handler=handler, **kwargs)
-	
+
 	# self.receiver.Unbind(self.binder, **kwargs)
-	
+
 	def trigger(self, value=None):
 		"""
 		Trigger the event
 		"""
-		
+
 		if value is not None:
 			self.value = value
-		
+
 		for receiver in self.bindings:
 			wx.PostEvent(receiver, PayloadEvent(self.event, -1, self.value))
-		
+
 		# wx.PostEvent(self.receiver, PayloadEvent(self.event, -1, self.value))
 		self.value = None
-
-
```

### Comparing `domdf_wxpython_tools-0.2.5/LICENSE` & `domdf_wxpython_tools-0.3.0.post1/LICENSE`

 * *Files identical despite different names*

