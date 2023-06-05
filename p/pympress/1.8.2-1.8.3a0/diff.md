# Comparing `tmp/pympress-1.8.2.tar.gz` & `tmp/pympress-1.8.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympress-1.8.2.tar", last modified: Tue Apr  4 12:27:15 2023, max compression
+gzip compressed data, was "pympress-1.8.3a0.tar", last modified: Mon Jun  5 13:28:15 2023, max compression
```

## Comparing `pympress-1.8.2.tar` & `pympress-1.8.3a0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.455036 pympress-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-04 12:26:55.000000 pympress-1.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-04-04 12:27:15.455036 pympress-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23333 2023-04-04 12:26:55.000000 pympress-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.443036 pympress-1.8.2/pympress/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22802 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/deck.py
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48780 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/document.py
--rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/editable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    29137 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/media_overlays/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/gif_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/gst_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/media_overlays/vlc_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/scribble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/applications/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/applications/io.github.pympress.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/css/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/defaults.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/cs/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/de/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/es/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/fr/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/hi/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/it/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/ja/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/pl/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/zh_HANT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress/share/locale/zh_HANT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.439036 pympress-1.8.2/pympress/share/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.451036 pympress-1.8.2/pympress/share/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-04 12:27:14.000000 pympress-1.8.2/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.451036 pympress-1.8.2/pympress/share/pixmaps/
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/eraser.png
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_fill_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_fill_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/marker_fill_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pointer_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pointer_green.png
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pointer_red.png
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-22.png
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-24.png
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-48.png
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress-64.png
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/pixmaps/pympress.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.455036 pympress-1.8.2/pympress/share/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/autoplay.glade
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/content.glade
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/deck.glade
--rw-r--r--   0 runner    (1001) docker     (123)    23168 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/highlight.glade
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/layout_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/media_overlay.glade
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/menu_bar.xml
--rw-r--r--   0 runner    (1001) docker     (123)    77009 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/presenter.glade
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/shortcuts.glade
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/share/xml/time_report_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/surfacecache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/talk_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    76248 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-04-04 12:26:55.000000 pympress-1.8.2/pympress/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:27:15.447036 pympress-1.8.2/pympress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 12:27:15.000000 pympress-1.8.2/pympress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-04 12:26:55.000000 pympress-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-04 12:27:15.455036 pympress-1.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-04-04 12:26:55.000000 pympress-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.351712 pympress-1.8.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-05 13:28:02.000000 pympress-1.8.3a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-06-05 13:28:15.351712 pympress-1.8.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-06-05 13:28:02.000000 pympress-1.8.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/deck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48780 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/editable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29137 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/media_overlays/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/gif_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/gst_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/vlc_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/pointer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36275 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/scribble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/applications/io.github.pympress.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/css/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/defaults.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/cs/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/de/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/es/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/fr/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/hi/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/it/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/ja/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/pl/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/zh_HANT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/zh_HANT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.351712 pympress-1.8.3a0/pympress/share/pixmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/eraser.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pointer_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pointer_green.png
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pointer_red.png
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-22.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-24.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-64.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.351712 pympress-1.8.3a0/pympress/share/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/autoplay.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/content.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/deck.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    23169 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/highlight.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/layout_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/media_overlay.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/menu_bar.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    77009 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/presenter.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/shortcuts.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/time_report_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/surfacecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/talk_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76144 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-05 13:28:15.355712 pympress-1.8.3a0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-06-05 13:28:02.000000 pympress-1.8.3a0/setup.py
```

### Comparing `pympress-1.8.2/LICENSE.txt` & `pympress-1.8.3a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/PKG-INFO` & `pympress-1.8.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympress
-Version: 1.8.2
+Version: 1.8.3a0
 Summary: A simple and powerful dual-screen PDF reader designed for presentations
 Home-page: https://github.com/Cimbali/pympress/
 Download-URL: https://github.com/Cimbali/pympress/releases/latest
 Author: Cimbali, Thomas Jost, Christof Rath, Epithumia
 Author-email: me@cimba.li
 License: GPL-2.0-or-later
 Project-URL: Issues, https://github.com/Cimbali/pympress/issues/
@@ -265,14 +265,15 @@
 Ferdinand Fichtner,
 Frederik. blome,
 FriedrichFröbel,
 He. yifan. xs,
 Jaroslav Svoboda,
 Jeertmans,
 Kristýna,
+lazycat,
 Leonvincenterd,
 LogCreative,
 Lorenzo. pacchiardi,
 Luis Sibaja,
 Marcin Dohnalik,
 marquitul,
 Morfit,
```

### Comparing `pympress-1.8.2/README.md` & `pympress-1.8.3a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -346,14 +346,15 @@
 Ferdinand Fichtner,
 Frederik. blome,
 FriedrichFröbel,
 He. yifan. xs,
 Jaroslav Svoboda,
 Jeertmans,
 Kristýna,
+lazycat,
 Leonvincenterd,
 LogCreative,
 Lorenzo. pacchiardi,
 Luis Sibaja,
 Marcin Dohnalik,
 marquitul,
 Morfit,
```

### Comparing `pympress-1.8.2/pympress/__init__.py` & `pympress-1.8.3a0/pympress/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """ A simple and powerful dual-screen PDF reader designed for presentations.
 """
 
 #
 # DON'T IMPORT ANYTHING HERE (OR YOU WILL BREAK setup.py)
 #
 
-__version__ = '1.8.2'
+__version__ = '1.8.3a'
 __author__ = """2009, 2010 Thomas Jost <thomas.jost@gmail.com>
 2015-2023 Cimbali <me@cimba.li>
 2016 Christoph Rath <christof.rath@iaik.tugraz.at>
 2016 Epithumia <endless@airelle.info>
 """
 
 __all__ = ['app', 'builder', 'config', 'document', 'editable_label', 'extras', 'media_overlays', 'pointer', 'scribble',
```

### Comparing `pympress-1.8.2/pympress/__main__.py` & `pympress-1.8.3a0/pympress/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 -------------------------------------------------------
 """
 
 import logging
 import os
 import sys
 import locale
-import gettext
 
 from pympress import util
 
 
 # Setup logging, and catch all uncaught exceptions in the log file.
 # Load pympress.util early (OS and path-specific things) to load and setup gettext translation asap.
 logger = logging.getLogger(__name__)
@@ -56,15 +55,15 @@
 
 try:
     loaded_locale = locale.setlocale(locale.LC_ALL, '')
 except locale.Error as err:
     logger.exception('Failed loading locale: {}'.format(err))
     print('Failed loading locale: {}'.format(err), file=sys.stderr)
 
-gettext.install('pympress', util.get_locale_dir())
+util.get_translation('pympress').install()
 
 
 try:
     # python <3.6 does not have this
     ModuleNotFoundError
 except NameError:
     ModuleNotFoundError = ImportError  # noqa: A001 -- not shadowing ModuleNotFoundError if it doesn’t exist
```

### Comparing `pympress-1.8.2/pympress/app.py` & `pympress-1.8.3a0/pympress/app.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/builder.py` & `pympress-1.8.3a0/pympress/builder.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/config.py` & `pympress-1.8.3a0/pympress/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,16 @@
 
         Args:
             search_legacy_locations (`bool`): whether to look in previously used locations
 
         Returns:
             :class:`~pathlib.Path`: The path to the config file to use
         """
-        portable_config = util.get_portable_config()
-        if portable_config.exists():
-            return portable_config
+        if Config.using_portable_config():
+            return util.get_portable_config()
 
         user_config = util.get_user_config()
 
         # migrate old configuration files from previously-used erroneous locations
         if search_legacy_locations and (util.IS_POSIX or util.IS_MAC_OS) and not user_config.exists():
             for legacy_location in ['~/.pympress', '~/.config/pympress']:
                 legacy_location = pathlib.Path(legacy_location).expanduser()
@@ -102,14 +101,16 @@
         No need to populate the new config file, this will be done on pympress exit.
 
         Args:
             gaction (:class:`~Gio.Action`): the action triggering the call
             param (:class:`~GLib.Variant`): the parameter as a variant, or None
         """
         portable_config = util.get_portable_config()
+        if portable_config is None:
+            return
         if Config.using_portable_config():
             portable_config.unlink()
         else:
             with open(portable_config, 'w'):
                 pass
         gaction.set_state(GLib.Variant.new_boolean(Config.using_portable_config()))
 
@@ -117,15 +118,16 @@
     @staticmethod
     def using_portable_config():
         """ Checks which configuration file location is in use.
 
         Returns:
             `bool`: `True` iff we are using the portable (i.e. in install dir) location
         """
-        return util.get_portable_config().exists()
+        portable_config = util.get_portable_config()
+        return portable_config is not None and portable_config.exists()
 
 
     def __init__(config):
         # Remove : from delimiters so we can use it in preferences
         super(Config, config).__init__(delimiters=('=',))
 
         # populate values first from the default config file, then from the proper one
@@ -166,20 +168,21 @@
         Args:
             builder (:class:`pympress.builder.Builder`): a builder to setup the actions
         """
         p_full = self.getboolean('presenter', 'start_fullscreen')
         c_full = self.getboolean('content', 'start_fullscreen')
         blank = self.getboolean('content', 'start_blanked')
         portable = self.using_portable_config()
+        can_port = util.get_portable_config() is not None
 
         builder.setup_actions({
             'start-content-fullscreen':   dict(activate=self.toggle_start, state=c_full),
             'start-presenter-fullscreen': dict(activate=self.toggle_start, state=p_full),
             'start-blanked':              dict(activate=self.toggle_start, state=blank),
-            'portable-config':            dict(activate=self.toggle_portable_config, state=portable),
+            'portable-config':            dict(activate=self.toggle_portable_config, state=portable, enabled=can_port),
         })
 
 
     def upgrade(self):
         """ Update obsolete config options when pympress updates.
         """
         if self.get('presenter', 'pointer') == 'pointer_none':
```

### Comparing `pympress-1.8.2/pympress/deck.py` & `pympress-1.8.3a0/pympress/deck.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/dialog.py` & `pympress-1.8.3a0/pympress/dialog.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/document.py` & `pympress-1.8.3a0/pympress/document.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/editable_label.py` & `pympress-1.8.3a0/pympress/editable_label.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/extras.py` & `pympress-1.8.3a0/pympress/extras.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/media_overlays/__init__.py` & `pympress-1.8.3a0/pympress/media_overlays/__init__.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/media_overlays/base.py` & `pympress-1.8.3a0/pympress/media_overlays/base.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/media_overlays/gif_backend.py` & `pympress-1.8.3a0/pympress/media_overlays/gif_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/media_overlays/gst_backend.py` & `pympress-1.8.3a0/pympress/media_overlays/gst_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/media_overlays/vlc_backend.py` & `pympress-1.8.3a0/pympress/media_overlays/vlc_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/pointer.py` & `pympress-1.8.3a0/pympress/pointer.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/scribble.py` & `pympress-1.8.3a0/pympress/scribble.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     Args:
         config (:class:`~pympress.config.Config`): A config object containing preferences
         builder (:class:`~pympress.builder.Builder`): A builder from which to load widgets
         notes_mode (`bool`): The current notes mode, i.e. whether we display the notes on second slide
     """
     #: Whether we are displaying the interface to scribble on screen and the overlays containing said scribbles
     scribbling_mode = False
-    #: `list` of scribbles to be drawn, as tuples of color :class:`~Gdk.RGBA`, width `int`, and a `list` of points.
+    #: `list` of scribbles to be drawn, as tuples of color :class:`~Gdk.RGBA`, width `int`, a `list` of points,
+    #: and a `list` of pressure values.
     scribble_list = []
     #: `list` of undone scribbles to possibly redo
     scribble_redo_list = []
     #: Whether the current mouse movements are drawing strokes or should be ignored
     scribble_drawing = False
     #: :class:`~Gdk.RGBA` current color of the scribbling tool
     scribble_color = Gdk.RGBA()
@@ -185,15 +186,15 @@
 
         self.marker_surfaces = list(zip(icons, masks))
         self.eraser_surface = cairo.ImageSurface.create_from_png(str(util.get_icon_path('eraser.png')))
 
         # Load color and active pen preferences. Pen 0 is the eraser.
         self.color_width = [(Gdk.RGBA(0, 0, 0, 0), 150)] + list(zip(
             [self.parse_color(config.get('highlight', 'color_{}'.format(pen))) for pen in range(1, 10)],
-            [config.getint('highlight', 'width_{}'.format(pen)) for pen in range(1, 10)],
+            [config.getfloat('highlight', 'width_{}'.format(pen)) for pen in range(1, 10)],
         ))
 
         self.scribble_preset_buttons = [
             self.get_object('pen_preset_{}'.format(pen) if pen else 'eraser') for pen in range(10)
         ]
 
         self.tools_orientation = self.config.get('layout', 'highlight_tools')
@@ -290,40 +291,41 @@
             `list`: control points of a bezier curves to draw
         """
         curves = []
 
         if len(points) <= 2:
             return curves
 
-        c1 = points[1]
-        for c2, pt in zip(points[2:-1:2], points[3:-1:2]):
-            half_c2pt = (pt[0] - c2[0]) / 2, (pt[1] - c2[1]) / 2
-
-            curves.append((*c1, c2[0] + half_c2pt[0], c2[1] + half_c2pt[1], *pt))
-            c1 = (pt[0] + half_c2pt[0], pt[1] + half_c2pt[1])
-
-        if len(points) % 2 == 0:
-            curves.append((*c1, *points[-2], *points[-1]))
+        for (ax, ay), (bx, by), (cx, cy), (dx, dy) in zip(
+                [points[0], *points[:-2]], points[:-1], points[1:], [*points[2:], points[-1]]
+        ):
+            curves.append((bx, by,
+                           bx + (cx - ax) / 4, by + (cy - ay) / 4,
+                           cx + (bx - dx) / 4, cy + (by - dy) / 4,
+                           cx, cy))
 
         return curves
 
 
     def track_scribble(self, widget, event):
         """ Draw the scribble following the mouse's moves.
 
         Args:
             widget (:class:`~Gtk.Widget`):  the widget which has received the event.
             event (:class:`~Gdk.Event`):  the GTK event.
 
         Returns:
             `bool`: whether the event was consumed
         """
-        pos = self.get_slide_point(widget, event)
+        pos = self.get_slide_point(widget, event) + ()
+
         if self.scribble_drawing:
-            self.scribble_list[-1][-1].append(pos)
+            self.scribble_list[-1][-2].append(pos)
+            pressure = event.get_axis(Gdk.AxisUse.PRESSURE)
+            self.scribble_list[-1][-1].append(1. if pressure is None else pressure)
             self.scribble_redo_list.clear()
 
             self.adjust_buttons()
 
         self.mouse_pos = pos
         self.redraw_current_slide()
         return self.scribble_drawing
@@ -370,21 +372,22 @@
         Returns:
             `bool`: whether the event was consumed
         """
         if not self.scribbling_mode:
             return False
 
         if event.get_event_type() == Gdk.EventType.BUTTON_PRESS:
-            if any(mod & event.get_state() == mod for mod in self.toggle_erase_modifiers) and self.active_preset \
-                    and self.toggle_erase_source is None:
+            eraser_button = event.get_source_device().get_source() == Gdk.InputSource.ERASER
+            eraser_modifier = any(mod & event.get_state() == mod for mod in self.toggle_erase_modifiers)
+            if (eraser_button or eraser_modifier) and self.active_preset and self.toggle_erase_source is None:
                 self.previous_preset = self.active_preset
                 self.toggle_erase_source = 'modifier'
                 self.load_preset(target=0)
 
-            self.scribble_list.append((self.scribble_color, self.scribble_width, []))
+            self.scribble_list.append((self.scribble_color, self.scribble_width, [], []))
             self.scribble_drawing = True
 
             return self.track_scribble(widget, event)
         elif event.get_event_type() == Gdk.EventType.BUTTON_RELEASE:
             self.scribble_drawing = False
             self.prerender()
 
@@ -442,58 +445,64 @@
             return
 
         scale = self.c_da.get_window().get_scale_factor()
         ww, wh = self.scribble_cache.get_width() / scale, self.scribble_cache.get_height() / scale
         pen_scale_factor = max(ww / 900, wh / 900)  # or sqrt of product
 
         cairo_context = cairo.Context(self.scribble_cache)
-        cairo_context.set_line_cap(cairo.LINE_CAP_ROUND)
 
         draw = slice(self.next_render, -1 if self.scribble_drawing else None)
 
-        for color, width, points in self.scribble_list[draw]:
-            self.render_scribble(cairo_context, color, width * pen_scale_factor, [(x * ww, y * wh) for x, y in points])
+        # Draw every stroke on a separate surface, then merge them all into the scribble cache
+        for color, width, points, pressure in self.scribble_list[draw]:
+            cairo_context.push_group()
+
+            cairo_context.set_line_cap(cairo.LINE_CAP_ROUND)
+            self.render_scribble(cairo_context, color, width * pen_scale_factor, [(x * ww, y * wh) for x, y in points],
+                                 pressure)
+
+            cairo_context.pop_group_to_source()
+            cairo_context.paint()
 
         del cairo_context
 
-        self.next_render = len(self.scribble_list) + (draw.stop if draw.stop else 0)
+        self.next_render = draw.indices(len(self.scribble_list))[1]
 
 
-    def render_scribble(self, cairo_context, color, width, points):
+    def render_scribble(self, cairo_context, color, width, points, pressures):
         """ Draw a single scribble, i.e. a bezier curve, on the cairo context
 
         Args:
             cairo_context (:class:`~cairo.Context`): The canvas on which to render the drawings
             color (:class:`~Gdk.RGBA`): The color of the scribble
             width (`float`): The width of the curve
             points (`list`): The control points of the curve, scaled to the surface.
-
-        Returns:
-            :class:`~cairo.Path`: A copy of the path that was drawn
+            pressures (`list`): The relative line width at each point as `float` values in 0..1
         """
         if not points:
             return
 
         # alpha == 0 -> Eraser mode
-        cairo_context.set_operator(cairo.OPERATOR_OVER if color.alpha else cairo.OPERATOR_CLEAR)
+        cairo_context.set_operator(cairo.OPERATOR_SOURCE if color.alpha else cairo.OPERATOR_CLEAR)
         cairo_context.set_source_rgba(*color)
-        cairo_context.set_line_width(width)
-
-        cairo_context.move_to(*points[0])
-
-        for curve in self.points_to_curves(points):
-            cairo_context.curve_to(*curve)
-
-        path = cairo_context.copy_path()
 
+        curves = self.points_to_curves(points)
+        curve_widths = [(a + b) / 2 for a, b in zip(pressures[:-1], pressures[1:])]
+        for curve, relwidth in zip(curves, curve_widths):
+            cairo_context.move_to(*curve[:2])
+            cairo_context.set_line_width(width * relwidth)
+            cairo_context.curve_to(*curve[2:])
+            cairo_context.stroke()
+
+        # Draw from last uneven-indexed point to last point
+        cairo_context.move_to(*points[-2 if len(points) % 2 and len(points) > 1 else -1])
+        cairo_context.set_line_width(width * curve_widths[-1] if curve_widths else pressures[-1])
         cairo_context.line_to(*points[-1])
         cairo_context.stroke()
 
-        return path
-
 
     def draw_scribble(self, widget, cairo_context):
         """ Perform the drawings by user.
 
         Args:
             widget (:class:`~Gtk.DrawingArea`): The widget where to draw the scribbles.
             cairo_context (:class:`~cairo.Context`): The canvas on which to render the drawings
@@ -511,16 +520,17 @@
         cairo_context.restore()
 
         cairo_context.push_group()
 
         pen_scale_factor = max(ww / 900, wh / 900)  # or sqrt of product
         if self.scribble_drawing:
             cairo_context.set_line_cap(cairo.LINE_CAP_ROUND)
-            color, width, points = self.scribble_list[-1]
-            self.render_scribble(cairo_context, color, width * pen_scale_factor, [(x * ww, y * wh) for x, y in points])
+            color, width, points, pressure = self.scribble_list[-1]
+            self.render_scribble(cairo_context, color, width * pen_scale_factor, [(x * ww, y * wh) for x, y in points],
+                                 pressure)
 
         cairo_context.pop_group_to_source()
         cairo_context.paint()
 
 
         if widget.get_name() == 'scribble_p_da' and self.mouse_pos is not None:
             cairo_context.set_source_rgba(0, 0, 0, 1)
@@ -550,15 +560,15 @@
         """ Callback for the width chooser slider, to set scribbling width.
 
         Args:
             widget (:class:`~Gtk.Scale`): The slider control used to select the scribble width
             event (:class:`~Gdk.Event`):  the GTK event triggering this update.
             value (`int`): the width of the scribbles to be drawn
         """
-        self.scribble_width = max(5, min(90, int(value)))
+        self.scribble_width = max(1, min(100, 10 ** value if value < 1 else 10 + (value - 1) * 90))
         self.update_active_color_width()
 
 
     def update_active_color_width(self):
         """ Update modifications to the active scribble color and width, on the pen button and config object
         """
         if not self.active_preset:
@@ -731,14 +741,17 @@
 
         self.scribble_off_render.remove(self.scribble_overlay)
         self.load_layout('highlight')
 
         self.p_central.queue_draw()
         self.scribble_overlay.queue_draw()
 
+        # Get frequent events for smooth drawing
+        self.p_central.get_window().set_event_compression(False)
+
         self.scribbling_mode = True
         self.get_application().lookup_action('highlight').change_state(GLib.Variant.new_boolean(self.scribbling_mode))
         self.pen_action.set_enabled(self.scribbling_mode)
 
         self.p_central.queue_draw()
         extras.Cursor.set_cursor(self.scribble_p_da, 'invisible')
         return True
@@ -754,14 +767,15 @@
             return False
 
         self.scribbling_mode = False
 
         extras.Cursor.set_cursor(self.scribble_p_da, 'default')
         self.load_layout(None)
         self.scribble_off_render.add(self.scribble_overlay)
+        self.p_central.get_window().set_event_compression(True)
 
         self.get_application().lookup_action('highlight').change_state(GLib.Variant.new_boolean(self.scribbling_mode))
         self.pen_action.set_enabled(self.scribbling_mode)
 
         self.p_central.queue_draw()
         extras.Cursor.set_cursor(self.p_central)
         self.mouse_pos = None
@@ -788,15 +802,16 @@
 
         self.config.set('highlight', 'active_pen', target)
         self.pen_action.change_state(GLib.Variant.new_string(target))
         self.scribble_color, self.scribble_width = self.color_width[self.active_preset]
 
         # Presenter-side setup
         self.scribble_color_selector.set_rgba(self.scribble_color)
-        self.scribble_width_selector.set_value(self.scribble_width)
+        self.scribble_width_selector.set_value(math.log10(self.scribble_width) if self.scribble_width < 10
+                                               else 1 + (self.scribble_width - 10) / 90)
         self.scribble_color_selector.set_sensitive(target != 'eraser')
         self.scribble_width_selector.set_sensitive(target != 'eraser')
 
         # Re-draw the eraser
         self.scribble_p_da.queue_draw()
         self.c_da.queue_draw()
 
@@ -826,15 +841,15 @@
 
         Args:
             widget (:class:`~Gtk.Widget`):  the widget to update
             cairo_context (:class:`~cairo.Context`):  the Cairo context (or `None` if called directly)
         """
         button_number = int(widget.get_name().split('_')[-1])
         color, width = self.color_width[button_number]
-        icon, mask = self.marker_surfaces[int((width - 1) / 30)]
+        icon, mask = self.marker_surfaces[int(width >= 2) + int(width >= 40)]
 
         ww, wh = widget.get_allocated_width(), widget.get_allocated_height()
         scale = wh / icon.get_height()
 
         dw, dh = self.scribble_p_da.get_allocated_width(), self.scribble_p_da.get_allocated_height()
         pen_scale_factor = max(dw / 900, dh / 900)  # or sqrt of product
         width *= pen_scale_factor
```

### Comparing `pympress-1.8.2/pympress/share/css/default.css` & `pympress-1.8.3a0/pympress/share/css/default.css`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/defaults.conf` & `pympress-1.8.3a0/pympress/share/defaults.conf`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/locale/cs/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/cs/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/de/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/de/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/es/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/es/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/fr/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/fr/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/hi/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/hi/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hi\n"
 "Language-Team: hi <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/it/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/it/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/ja/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/ja/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/pl/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/pl/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.2/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo` & `pympress-1.8.3a0/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-04 12:27+0000\n"
+"POT-Creation-Date: 2023-06-05 13:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language: zh_HANT\n"
-"Language-Team: zh_HANT <LL@li.org>\n"
+"Language: zh_TW\n"
+"Language-Team: zh_TW <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "(paused)"
```

### Comparing `pympress-1.8.2/pympress/share/pixmaps/eraser.png` & `pympress-1.8.3a0/pympress/share/pixmaps/eraser.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/marker_1.png` & `pympress-1.8.3a0/pympress/share/pixmaps/marker_1.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/marker_2.png` & `pympress-1.8.3a0/pympress/share/pixmaps/marker_2.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/marker_3.png` & `pympress-1.8.3a0/pympress/share/pixmaps/marker_3.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/marker_fill_1.png` & `pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_1.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/marker_fill_2.png` & `pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_2.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/marker_fill_3.png` & `pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_3.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pointer_blue.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pointer_blue.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pointer_green.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pointer_green.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pointer_red.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pointer_red.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pympress-16.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pympress-16.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pympress-22.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pympress-22.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pympress-24.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pympress-24.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pympress-32.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pympress-32.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pympress-48.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pympress-48.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pympress-64.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pympress-64.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/pixmaps/pympress.png` & `pympress-1.8.3a0/pympress/share/pixmaps/pympress.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/autoplay.glade` & `pympress-1.8.3a0/pympress/share/xml/autoplay.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/content.glade` & `pympress-1.8.3a0/pympress/share/xml/content.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/deck.glade` & `pympress-1.8.3a0/pympress/share/xml/deck.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/highlight.glade` & `pympress-1.8.3a0/pympress/share/xml/highlight.glade`

 * *Files 0% similar despite different names*

#### Comparing `pympress-1.8.2/pympress/share/xml/highlight.glade` & `pympress-1.8.3a0/pympress/share/xml/highlight.glade`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Generated with glade 3.38.2 -->
+<!-- Generated with glade 3.40.0 -->
 <interface>
   <requires lib="gtk+" version="3.4"/>
   <object class="GtkAdjustment" id="scribble_width_adjust">
-    <property name="lower">2</property>
-    <property name="upper">90</property>
-    <property name="value">8</property>
-    <property name="step-increment">1</property>
+    <property name="lower">0</property>
+    <property name="upper">2</property>
+    <property name="value">.9</property>
+    <property name="step-increment">.1</property>
     <property name="page-increment">1</property>
   </object>
   <object class="GtkOffscreenWindow" id="scribble_off_render">
     <property name="can-focus">False</property>
     <child>
       <object class="GtkBox" id="scribble_overlay">
         <property name="visible">True</property>
```

### Comparing `pympress-1.8.2/pympress/share/xml/layout_dialog.glade` & `pympress-1.8.3a0/pympress/share/xml/layout_dialog.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/media_overlay.glade` & `pympress-1.8.3a0/pympress/share/xml/media_overlay.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/menu_bar.xml` & `pympress-1.8.3a0/pympress/share/xml/menu_bar.xml`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/presenter.glade` & `pympress-1.8.3a0/pympress/share/xml/presenter.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/shortcuts.glade` & `pympress-1.8.3a0/pympress/share/xml/shortcuts.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/share/xml/time_report_dialog.glade` & `pympress-1.8.3a0/pympress/share/xml/time_report_dialog.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/surfacecache.py` & `pympress-1.8.3a0/pympress/surfacecache.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/talk_time.py` & `pympress-1.8.3a0/pympress/talk_time.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/pympress/ui.py` & `pympress-1.8.3a0/pympress/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -743,15 +743,14 @@
         pympress = util.get_pympress_meta()
         about.set_program_name('pympress')
         about.set_version(pympress['version'])
         about.set_copyright(_('Contributors:') + '\n' + pympress['contributors'])
         about.set_comments(_('pympress is a little PDF reader written in Python ' +
                              'using Poppler for PDF rendering and GTK for the GUI.\n') +
                            _('Some preferences are saved in ') + str(self.config.path_to_config()) + '\n' +
-                           _('Resources are loaded from ') + str(util.get_locale_dir().parent) + '\n' +
                            _('The log is written to ') + str(util.get_log_path()) + '\n\n' +
                            _('Media support uses {}.').format(self.medias.backend_version) + '\n' +
                            _('Python version {}').format(sys.version))
         about.set_website('https://github.com/Cimbali/pympress')
         try:
             about.set_logo(GdkPixbuf.Pixbuf.new_from_file(util.get_icon_path('pympress.png')))
         except Exception:
```

### Comparing `pympress-1.8.2/pympress/util.py` & `pympress-1.8.3a0/pympress/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 import contextlib
 import subprocess
 import importlib
+import gettext
 import os
 import sys
 import pathlib
 
 if sys.version_info >= (3, 9):
     # Using parts introduced in 3.9
     import importlib.resources as importlib_resources
@@ -109,30 +110,56 @@
 
 
 def close_opened_resources():
     """ Close all importlib context managers for resources that we needed over the program lifetime. """
     _opened_resources.close()
 
 
-def get_locale_dir():
-    """ Returns the path to the locale directory.
+def get_translation(domain):
+    """ Returns a gettext translation object.
+
+    This re-implements gettext’s translation() and find() to allow using a python 3.9 Traversable as localedir
 
     Returns:
-        :class:`~pathlib.Path`: The path to the locale directory
+        :class:`~gettext.NullTranslations`: A gettext translation object with the strings for the domain loaded
     """
-    return __get_resource_path('share', 'locale')
+    localedir = importlib_resources.files('pympress').joinpath('share', 'locale')
+
+    for envar in ('LANGUAGE', 'LC_ALL', 'LC_MESSAGES', 'LANG'):
+        enval = os.environ.get(envar)
+        if enval:
+            break
+    else:
+        return gettext.NullTranslations()
+
+    # now normalize and expand the languages
+    for lang in enval.split(':'):
+        for nelang in gettext._expand_lang(lang):
+            file = localedir.joinpath(nelang, 'LC_MESSAGES', domain + '.mo')
+            if file.is_file():
+                break
+    else:
+        return gettext.NullTranslations()
+
+    with file.open() as fp:
+        return gettext.GNUTranslations(fp)
 
 
 def get_portable_config():
     """ Returns the path to the configuration file for a portable install (i.e. in the install root).
 
+    May return None if the install root is not a real directory (e.g. in a zip file).
+
     Returns:
-        :class:`~pathlib.Path`: The path to the portable configuration file.
+        :class:`~pathlib.Path` or `None`: The path to the portable configuration file.
     """
-    return __get_resource_path('pympress.conf')
+    try:
+        return __get_resource_path('pympress.conf')
+    except FileNotFoundError:
+        return None
 
 
 def get_default_config():
     """ Returns the path to the configuration file containing the defaults.
 
     Returns:
         :class:`~pathlib.Path`: The path to the portable configuration file.
```

### Comparing `pympress-1.8.2/pympress.egg-info/PKG-INFO` & `pympress-1.8.3a0/pympress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympress
-Version: 1.8.2
+Version: 1.8.3a0
 Summary: A simple and powerful dual-screen PDF reader designed for presentations
 Home-page: https://github.com/Cimbali/pympress/
 Download-URL: https://github.com/Cimbali/pympress/releases/latest
 Author: Cimbali, Thomas Jost, Christof Rath, Epithumia
 Author-email: me@cimba.li
 License: GPL-2.0-or-later
 Project-URL: Issues, https://github.com/Cimbali/pympress/issues/
@@ -265,14 +265,15 @@
 Ferdinand Fichtner,
 Frederik. blome,
 FriedrichFröbel,
 He. yifan. xs,
 Jaroslav Svoboda,
 Jeertmans,
 Kristýna,
+lazycat,
 Leonvincenterd,
 LogCreative,
 Lorenzo. pacchiardi,
 Luis Sibaja,
 Marcin Dohnalik,
 marquitul,
 Morfit,
```

### Comparing `pympress-1.8.2/pympress.egg-info/SOURCES.txt` & `pympress-1.8.3a0/pympress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/setup.cfg` & `pympress-1.8.3a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pympress-1.8.2/setup.py` & `pympress-1.8.3a0/setup.py`

 * *Files identical despite different names*

