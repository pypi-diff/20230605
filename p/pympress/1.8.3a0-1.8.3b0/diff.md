# Comparing `tmp/pympress-1.8.3a0.tar.gz` & `tmp/pympress-1.8.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympress-1.8.3a0.tar", last modified: Mon Jun  5 13:28:15 2023, max compression
+gzip compressed data, was "pympress-1.8.3b0.tar", last modified: Mon Jun  5 20:31:10 2023, max compression
```

## Comparing `pympress-1.8.3a0.tar` & `pympress-1.8.3b0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.351712 pympress-1.8.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-05 13:28:02.000000 pympress-1.8.3a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-06-05 13:28:15.351712 pympress-1.8.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-06-05 13:28:02.000000 pympress-1.8.3a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/deck.py
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48780 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/document.py
--rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/editable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    29137 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/media_overlays/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/gif_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/gst_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/media_overlays/vlc_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/pointer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36275 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/scribble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/applications/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/applications/io.github.pympress.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/css/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/defaults.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/cs/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/de/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/es/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/fr/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/hi/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/it/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/ja/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/pl/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/zh_HANT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/zh_HANT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.343711 pympress-1.8.3a0/pympress/share/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress/share/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-05 13:28:14.000000 pympress-1.8.3a0/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.351712 pympress-1.8.3a0/pympress/share/pixmaps/
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/eraser.png
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pointer_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pointer_green.png
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pointer_red.png
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-22.png
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-24.png
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-48.png
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress-64.png
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/pixmaps/pympress.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.351712 pympress-1.8.3a0/pympress/share/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/autoplay.glade
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/content.glade
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/deck.glade
--rw-r--r--   0 runner    (1001) docker     (123)    23169 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/highlight.glade
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/layout_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/media_overlay.glade
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/menu_bar.xml
--rw-r--r--   0 runner    (1001) docker     (123)    77009 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/presenter.glade
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/shortcuts.glade
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/share/xml/time_report_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/surfacecache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/talk_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    76144 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pympress/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:28:15.347711 pympress-1.8.3a0/pympress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 13:28:15.000000 pympress-1.8.3a0/pympress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 13:28:02.000000 pympress-1.8.3a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-05 13:28:15.355712 pympress-1.8.3a0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-06-05 13:28:02.000000 pympress-1.8.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.448364 pympress-1.8.3b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-05 20:30:58.000000 pympress-1.8.3b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-06-05 20:31:10.448364 pympress-1.8.3b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-06-05 20:30:58.000000 pympress-1.8.3b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.440364 pympress-1.8.3b0/pympress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/deck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48780 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/editable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29137 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/media_overlays/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/media_overlays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/media_overlays/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/media_overlays/gif_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/media_overlays/gst_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/media_overlays/vlc_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/pointer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36441 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/scribble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/applications/io.github.pympress.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/css/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/defaults.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/cs/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/de/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/es/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/fr/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/hi/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/it/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/ja/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/pl/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/zh_HANT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/zh_HANT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.436363 pympress-1.8.3b0/pympress/share/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.444364 pympress-1.8.3b0/pympress/share/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-05 20:31:09.000000 pympress-1.8.3b0/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.448364 pympress-1.8.3b0/pympress/share/pixmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/eraser.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/marker_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/marker_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/marker_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/marker_fill_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/marker_fill_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/marker_fill_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pointer_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pointer_green.png
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pointer_red.png
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pympress-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pympress-22.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pympress-24.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pympress-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pympress-48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pympress-64.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/pixmaps/pympress.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.448364 pympress-1.8.3b0/pympress/share/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/autoplay.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/content.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/deck.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    23169 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/highlight.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/layout_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/media_overlay.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/menu_bar.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    77009 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/presenter.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/shortcuts.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/share/xml/time_report_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/surfacecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/talk_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76144 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pympress/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:31:10.440364 pympress-1.8.3b0/pympress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-06-05 20:31:10.000000 pympress-1.8.3b0/pympress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-05 20:31:10.000000 pympress-1.8.3b0/pympress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:31:10.000000 pympress-1.8.3b0/pympress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 20:31:10.000000 pympress-1.8.3b0/pympress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-05 20:31:10.000000 pympress-1.8.3b0/pympress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 20:31:10.000000 pympress-1.8.3b0/pympress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 20:30:58.000000 pympress-1.8.3b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-05 20:31:10.452364 pympress-1.8.3b0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-06-05 20:30:58.000000 pympress-1.8.3b0/setup.py
```

### Comparing `pympress-1.8.3a0/LICENSE.txt` & `pympress-1.8.3b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/PKG-INFO` & `pympress-1.8.3b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympress
-Version: 1.8.3a0
+Version: 1.8.3b0
 Summary: A simple and powerful dual-screen PDF reader designed for presentations
 Home-page: https://github.com/Cimbali/pympress/
 Download-URL: https://github.com/Cimbali/pympress/releases/latest
 Author: Cimbali, Thomas Jost, Christof Rath, Epithumia
 Author-email: me@cimba.li
 License: GPL-2.0-or-later
 Project-URL: Issues, https://github.com/Cimbali/pympress/issues/
```

### Comparing `pympress-1.8.3a0/README.md` & `pympress-1.8.3b0/README.md`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/__init__.py` & `pympress-1.8.3b0/pympress/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """ A simple and powerful dual-screen PDF reader designed for presentations.
 """
 
 #
 # DON'T IMPORT ANYTHING HERE (OR YOU WILL BREAK setup.py)
 #
 
-__version__ = '1.8.3a'
+__version__ = '1.8.3b'
 __author__ = """2009, 2010 Thomas Jost <thomas.jost@gmail.com>
 2015-2023 Cimbali <me@cimba.li>
 2016 Christoph Rath <christof.rath@iaik.tugraz.at>
 2016 Epithumia <endless@airelle.info>
 """
 
 __all__ = ['app', 'builder', 'config', 'document', 'editable_label', 'extras', 'media_overlays', 'pointer', 'scribble',
```

### Comparing `pympress-1.8.3a0/pympress/__main__.py` & `pympress-1.8.3b0/pympress/__main__.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/app.py` & `pympress-1.8.3b0/pympress/app.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/builder.py` & `pympress-1.8.3b0/pympress/builder.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/config.py` & `pympress-1.8.3b0/pympress/config.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/deck.py` & `pympress-1.8.3b0/pympress/deck.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/dialog.py` & `pympress-1.8.3b0/pympress/dialog.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/document.py` & `pympress-1.8.3b0/pympress/document.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/editable_label.py` & `pympress-1.8.3b0/pympress/editable_label.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/extras.py` & `pympress-1.8.3b0/pympress/extras.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/media_overlays/__init__.py` & `pympress-1.8.3b0/pympress/media_overlays/__init__.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/media_overlays/base.py` & `pympress-1.8.3b0/pympress/media_overlays/base.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/media_overlays/gif_backend.py` & `pympress-1.8.3b0/pympress/media_overlays/gif_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/media_overlays/gst_backend.py` & `pympress-1.8.3b0/pympress/media_overlays/gst_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/media_overlays/vlc_backend.py` & `pympress-1.8.3b0/pympress/media_overlays/vlc_backend.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/pointer.py` & `pympress-1.8.3b0/pympress/pointer.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/scribble.py` & `pympress-1.8.3b0/pympress/scribble.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         icons = [cairo.ImageSurface.create_from_png(util.get_icon_path('marker_{}.png'.format(n))) for n in ms]
         masks = [cairo.ImageSurface.create_from_png(util.get_icon_path('marker_fill_{}.png'.format(n))) for n in ms]
 
         self.marker_surfaces = list(zip(icons, masks))
         self.eraser_surface = cairo.ImageSurface.create_from_png(str(util.get_icon_path('eraser.png')))
 
         # Load color and active pen preferences. Pen 0 is the eraser.
-        self.color_width = [(Gdk.RGBA(0, 0, 0, 0), 150)] + list(zip(
+        self.color_width = [(Gdk.RGBA(0, 0, 0, 0), config.getfloat('highlight', 'width_eraser'))] + list(zip(
             [self.parse_color(config.get('highlight', 'color_{}'.format(pen))) for pen in range(1, 10)],
             [config.getfloat('highlight', 'width_{}'.format(pen)) for pen in range(1, 10)],
         ))
 
         self.scribble_preset_buttons = [
             self.get_object('pen_preset_{}'.format(pen) if pen else 'eraser') for pen in range(10)
         ]
@@ -448,25 +448,18 @@
         ww, wh = self.scribble_cache.get_width() / scale, self.scribble_cache.get_height() / scale
         pen_scale_factor = max(ww / 900, wh / 900)  # or sqrt of product
 
         cairo_context = cairo.Context(self.scribble_cache)
 
         draw = slice(self.next_render, -1 if self.scribble_drawing else None)
 
-        # Draw every stroke on a separate surface, then merge them all into the scribble cache
         for color, width, points, pressure in self.scribble_list[draw]:
-            cairo_context.push_group()
-
             cairo_context.set_line_cap(cairo.LINE_CAP_ROUND)
             self.render_scribble(cairo_context, color, width * pen_scale_factor, [(x * ww, y * wh) for x, y in points],
                                  pressure)
-
-            cairo_context.pop_group_to_source()
-            cairo_context.paint()
-
         del cairo_context
 
         self.next_render = draw.indices(len(self.scribble_list))[1]
 
 
     def render_scribble(self, cairo_context, color, width, points, pressures):
         """ Draw a single scribble, i.e. a bezier curve, on the cairo context
@@ -477,54 +470,63 @@
             width (`float`): The width of the curve
             points (`list`): The control points of the curve, scaled to the surface.
             pressures (`list`): The relative line width at each point as `float` values in 0..1
         """
         if not points:
             return
 
+        # Draw every stroke on a separate surface, then merge them all into the scribble cache
+        # Erasers do not have their own group as they are meant to interfere with strokes below
+        if color.alpha:
+            cairo_context.push_group()
+
         # alpha == 0 -> Eraser mode
         cairo_context.set_operator(cairo.OPERATOR_SOURCE if color.alpha else cairo.OPERATOR_CLEAR)
         cairo_context.set_source_rgba(*color)
 
         curves = self.points_to_curves(points)
         curve_widths = [(a + b) / 2 for a, b in zip(pressures[:-1], pressures[1:])]
         for curve, relwidth in zip(curves, curve_widths):
             cairo_context.move_to(*curve[:2])
             cairo_context.set_line_width(width * relwidth)
             cairo_context.curve_to(*curve[2:])
             cairo_context.stroke()
 
         # Draw from last uneven-indexed point to last point
         cairo_context.move_to(*points[-2 if len(points) % 2 and len(points) > 1 else -1])
-        cairo_context.set_line_width(width * curve_widths[-1] if curve_widths else pressures[-1])
+        cairo_context.set_line_width(width * (curve_widths[-1] if curve_widths else pressures[-1]))
         cairo_context.line_to(*points[-1])
         cairo_context.stroke()
 
+        if color.alpha:
+            cairo_context.pop_group_to_source()
+            cairo_context.paint()
+
 
     def draw_scribble(self, widget, cairo_context):
         """ Perform the drawings by user.
 
         Args:
             widget (:class:`~Gtk.DrawingArea`): The widget where to draw the scribbles.
             cairo_context (:class:`~cairo.Context`): The canvas on which to render the drawings
         """
         scale = widget.get_window().get_scale_factor()
         ww, wh = widget.get_allocated_width(), widget.get_allocated_height()
         cw, ch = self.scribble_cache.get_width(), self.scribble_cache.get_height()
 
+        cairo_context.push_group()
+
         cairo_context.save()
 
         cairo_context.scale(ww * scale / cw, wh * scale / ch)
         cairo_context.set_source_surface(self.scribble_cache)
         cairo_context.paint()
 
         cairo_context.restore()
 
-        cairo_context.push_group()
-
         pen_scale_factor = max(ww / 900, wh / 900)  # or sqrt of product
         if self.scribble_drawing:
             cairo_context.set_line_cap(cairo.LINE_CAP_ROUND)
             color, width, points, pressure = self.scribble_list[-1]
             self.render_scribble(cairo_context, color, width * pen_scale_factor, [(x * ww, y * wh) for x, y in points],
                                  pressure)
 
@@ -567,22 +569,21 @@
         self.scribble_width = max(1, min(100, 10 ** value if value < 1 else 10 + (value - 1) * 90))
         self.update_active_color_width()
 
 
     def update_active_color_width(self):
         """ Update modifications to the active scribble color and width, on the pen button and config object
         """
-        if not self.active_preset:
-            return
-
         self.color_width[self.active_preset] = self.scribble_color, self.scribble_width
-        self.scribble_preset_buttons[self.active_preset].queue_draw()
+        if self.active_preset:
+            self.scribble_preset_buttons[self.active_preset].queue_draw()
 
-        pen = self.active_preset
-        self.config.set('highlight', 'color_{}'.format(pen), self.scribble_color.to_string())
+        pen = self.active_preset if self.active_preset else 'eraser'
+        if self.active_preset:
+            self.config.set('highlight', 'color_{}'.format(pen), self.scribble_color.to_string())
         self.config.set('highlight', 'width_{}'.format(pen), str(self.scribble_width))
 
 
     def adjust_buttons(self):
         """ Properly enable and disable buttons based on scribblings lists.
         """
         self.scribble_undo.set_sensitive(bool(self.scribble_list))
@@ -805,15 +806,14 @@
         self.scribble_color, self.scribble_width = self.color_width[self.active_preset]
 
         # Presenter-side setup
         self.scribble_color_selector.set_rgba(self.scribble_color)
         self.scribble_width_selector.set_value(math.log10(self.scribble_width) if self.scribble_width < 10
                                                else 1 + (self.scribble_width - 10) / 90)
         self.scribble_color_selector.set_sensitive(target != 'eraser')
-        self.scribble_width_selector.set_sensitive(target != 'eraser')
 
         # Re-draw the eraser
         self.scribble_p_da.queue_draw()
         self.c_da.queue_draw()
 
         return True
```

### Comparing `pympress-1.8.3a0/pympress/share/css/default.css` & `pympress-1.8.3b0/pympress/share/css/default.css`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/defaults.conf` & `pympress-1.8.3b0/pympress/share/defaults.conf`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 horizontal = right
 vertical = bottom
 
 [cache]
 maxpages = 200
 
 [highlight]
+width_eraser = 90
 color_1 = rgba(255,255,0,0.5)
 width_1 = 90
 color_2 = rgba(128,255,0,0.5)
 width_2 = 90
 color_3 = rgba(255,0,128,0.5)
 width_3 = 90
 color_4 = rgba(48,48,255,0.5)
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/cs/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/cs/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/de/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/de/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/es/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/es/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/fr/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/fr/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/hi/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/hi/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hi\n"
 "Language-Team: hi <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/it/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/it/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/ja/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/ja/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/pl/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/pl/LC_MESSAGES/pympress.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/zh_CN/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/zh_HANT/LC_MESSAGES/pympress.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_HANT\n"
 "Language-Team: zh_HANT <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo` & `pympress-1.8.3b0/pympress/share/locale/zh_TW/LC_MESSAGES/pympress.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  pympress\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-05 13:28+0000\n"
+"POT-Creation-Date: 2023-06-05 20:31+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_TW\n"
 "Language-Team: zh_TW <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/eraser.png` & `pympress-1.8.3b0/pympress/share/pixmaps/eraser.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/marker_1.png` & `pympress-1.8.3b0/pympress/share/pixmaps/marker_1.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/marker_2.png` & `pympress-1.8.3b0/pympress/share/pixmaps/marker_2.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/marker_3.png` & `pympress-1.8.3b0/pympress/share/pixmaps/marker_3.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_1.png` & `pympress-1.8.3b0/pympress/share/pixmaps/marker_fill_1.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_2.png` & `pympress-1.8.3b0/pympress/share/pixmaps/marker_fill_2.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/marker_fill_3.png` & `pympress-1.8.3b0/pympress/share/pixmaps/marker_fill_3.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pointer_blue.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pointer_blue.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pointer_green.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pointer_green.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pointer_red.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pointer_red.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pympress-16.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pympress-16.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pympress-22.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pympress-22.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pympress-24.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pympress-24.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pympress-32.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pympress-32.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pympress-48.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pympress-48.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pympress-64.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pympress-64.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/pixmaps/pympress.png` & `pympress-1.8.3b0/pympress/share/pixmaps/pympress.png`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/autoplay.glade` & `pympress-1.8.3b0/pympress/share/xml/autoplay.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/content.glade` & `pympress-1.8.3b0/pympress/share/xml/content.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/deck.glade` & `pympress-1.8.3b0/pympress/share/xml/deck.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/highlight.glade` & `pympress-1.8.3b0/pympress/share/xml/highlight.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/layout_dialog.glade` & `pympress-1.8.3b0/pympress/share/xml/layout_dialog.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/media_overlay.glade` & `pympress-1.8.3b0/pympress/share/xml/media_overlay.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/menu_bar.xml` & `pympress-1.8.3b0/pympress/share/xml/menu_bar.xml`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/presenter.glade` & `pympress-1.8.3b0/pympress/share/xml/presenter.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/shortcuts.glade` & `pympress-1.8.3b0/pympress/share/xml/shortcuts.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/share/xml/time_report_dialog.glade` & `pympress-1.8.3b0/pympress/share/xml/time_report_dialog.glade`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/surfacecache.py` & `pympress-1.8.3b0/pympress/surfacecache.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/talk_time.py` & `pympress-1.8.3b0/pympress/talk_time.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/ui.py` & `pympress-1.8.3b0/pympress/ui.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress/util.py` & `pympress-1.8.3b0/pympress/util.py`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/pympress.egg-info/PKG-INFO` & `pympress-1.8.3b0/pympress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympress
-Version: 1.8.3a0
+Version: 1.8.3b0
 Summary: A simple and powerful dual-screen PDF reader designed for presentations
 Home-page: https://github.com/Cimbali/pympress/
 Download-URL: https://github.com/Cimbali/pympress/releases/latest
 Author: Cimbali, Thomas Jost, Christof Rath, Epithumia
 Author-email: me@cimba.li
 License: GPL-2.0-or-later
 Project-URL: Issues, https://github.com/Cimbali/pympress/issues/
```

### Comparing `pympress-1.8.3a0/pympress.egg-info/SOURCES.txt` & `pympress-1.8.3b0/pympress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/setup.cfg` & `pympress-1.8.3b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pympress-1.8.3a0/setup.py` & `pympress-1.8.3b0/setup.py`

 * *Files identical despite different names*

