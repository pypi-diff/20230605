# Comparing `tmp/QPUIQ-0.2.1.tar.gz` & `tmp/QPUIQ-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.2.1.tar", last modified: Tue May 23 17:06:28 2023, max compression
+gzip compressed data, was "QPUIQ-0.2.2.tar", last modified: Mon Jun  5 21:22:26 2023, max compression
```

## Comparing `QPUIQ-0.2.1.tar` & `QPUIQ-0.2.2.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.244078 QPUIQ-0.2.1/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.2.1/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     6125 2023-05-23 17:06:28.243929 QPUIQ-0.2.1/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.227040 QPUIQ-0.2.1/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.232369 QPUIQ-0.2.1/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)     1245 2023-05-22 07:48:34.000000 QPUIQ-0.2.1/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.2.1/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     5095 2023-05-21 20:51:56.000000 QPUIQ-0.2.1/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      575 2023-05-14 18:07:46.000000 QPUIQ-0.2.1/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2708 2023-05-12 01:01:59.000000 QPUIQ-0.2.1/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      764 2023-05-14 14:59:50.000000 QPUIQ-0.2.1/PUI/PySide6/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     2343 2023-05-14 16:38:10.000000 QPUIQ-0.2.1/PUI/PySide6/combobox.py
--rw-r--r--   0 Bug        (504) staff       (20)      722 2023-05-14 18:07:33.000000 QPUIQ-0.2.1/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      941 2023-05-10 09:26:37.000000 QPUIQ-0.2.1/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      667 2023-05-20 18:18:18.000000 QPUIQ-0.2.1/PUI/PySide6/mdi.py
--rw-r--r--   0 Bug        (504) staff       (20)     2818 2023-05-22 05:29:49.000000 QPUIQ-0.2.1/PUI/PySide6/menu.py
--rw-r--r--   0 Bug        (504) staff       (20)      493 2023-05-04 13:36:49.000000 QPUIQ-0.2.1/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      784 2023-05-14 14:54:11.000000 QPUIQ-0.2.1/PUI/PySide6/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     3453 2023-05-22 11:07:05.000000 QPUIQ-0.2.1/PUI/PySide6/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1363 2023-05-22 10:28:02.000000 QPUIQ-0.2.1/PUI/PySide6/splitter.py
--rw-r--r--   0 Bug        (504) staff       (20)     1544 2023-05-14 18:06:04.000000 QPUIQ-0.2.1/PUI/PySide6/text.py
--rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-05-20 03:18:54.000000 QPUIQ-0.2.1/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     2251 2023-05-22 07:59:01.000000 QPUIQ-0.2.1/PUI/PySide6/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      488 2023-05-23 17:05:44.000000 QPUIQ-0.2.1/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      432 2023-05-15 20:31:59.000000 QPUIQ-0.2.1/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     3541 2023-05-23 12:21:44.000000 QPUIQ-0.2.1/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.235509 QPUIQ-0.2.1/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      658 2023-05-23 17:06:02.000000 QPUIQ-0.2.1/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      236 2023-05-22 11:27:04.000000 QPUIQ-0.2.1/PUI/flet/appbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      610 2023-05-20 06:55:30.000000 QPUIQ-0.2.1/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      612 2023-05-22 11:17:29.000000 QPUIQ-0.2.1/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      482 2023-05-14 18:08:03.000000 QPUIQ-0.2.1/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      645 2023-05-18 18:20:23.000000 QPUIQ-0.2.1/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1203 2023-05-23 15:24:05.000000 QPUIQ-0.2.1/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      499 2023-05-23 15:26:28.000000 QPUIQ-0.2.1/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)     1559 2023-05-23 15:23:00.000000 QPUIQ-0.2.1/PUI/flet/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      799 2023-05-18 17:43:47.000000 QPUIQ-0.2.1/PUI/flet/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.2.1/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      729 2023-05-23 15:25:40.000000 QPUIQ-0.2.1/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     4613 2023-05-20 17:17:52.000000 QPUIQ-0.2.1/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)    13532 2023-05-20 07:10:33.000000 QPUIQ-0.2.1/PUI/state.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.239605 QPUIQ-0.2.1/PUI/textual/
--rw-r--r--   0 Bug        (504) staff       (20)      967 2023-05-20 08:22:45.000000 QPUIQ-0.2.1/PUI/textual/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1963 2023-05-20 06:54:39.000000 QPUIQ-0.2.1/PUI/textual/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1177 2023-05-17 14:39:47.000000 QPUIQ-0.2.1/PUI/textual/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      421 2023-05-15 19:40:06.000000 QPUIQ-0.2.1/PUI/textual/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      531 2023-05-15 21:53:10.000000 QPUIQ-0.2.1/PUI/textual/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     1288 2023-05-16 07:25:36.000000 QPUIQ-0.2.1/PUI/textual/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     2681 2023-05-23 07:47:17.000000 QPUIQ-0.2.1/PUI/textual/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      484 2023-05-15 19:42:35.000000 QPUIQ-0.2.1/PUI/textual/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      634 2023-05-15 21:50:12.000000 QPUIQ-0.2.1/PUI/textual/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     1349 2023-05-23 07:46:17.000000 QPUIQ-0.2.1/PUI/textual/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      371 2023-05-16 08:39:00.000000 QPUIQ-0.2.1/PUI/textual/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      725 2023-05-17 14:33:03.000000 QPUIQ-0.2.1/PUI/textual/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      381 2023-05-20 17:16:55.000000 QPUIQ-0.2.1/PUI/textual/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-05-20 17:15:22.000000 QPUIQ-0.2.1/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.243078 QPUIQ-0.2.1/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      461 2023-05-20 08:22:54.000000 QPUIQ-0.2.1/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      614 2023-05-20 06:55:48.000000 QPUIQ-0.2.1/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      564 2023-05-10 11:04:22.000000 QPUIQ-0.2.1/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-05-14 18:07:17.000000 QPUIQ-0.2.1/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1283 2023-05-12 18:42:45.000000 QPUIQ-0.2.1/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      522 2023-05-14 18:06:49.000000 QPUIQ-0.2.1/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     2197 2023-05-12 09:01:37.000000 QPUIQ-0.2.1/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.2.1/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      565 2023-05-12 15:00:48.000000 QPUIQ-0.2.1/PUI/tkinter/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.2.1/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1524 2023-05-12 08:31:21.000000 QPUIQ-0.2.1/PUI/tkinter/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      505 2023-05-07 08:48:56.000000 QPUIQ-0.2.1/PUI/utils.py
--rw-r--r--   0 Bug        (504) staff       (20)     2860 2023-05-20 17:17:35.000000 QPUIQ-0.2.1/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.243728 QPUIQ-0.2.1/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     6125 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1463 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     5865 2023-05-18 06:35:30.000000 QPUIQ-0.2.1/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-05-23 17:06:28.244119 QPUIQ-0.2.1/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.2.1/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.325611 QPUIQ-0.2.2/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-05 21:22:26.325450 QPUIQ-0.2.2/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.314389 QPUIQ-0.2.2/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.318175 QPUIQ-0.2.2/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)     1245 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      498 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5469 2023-06-05 21:20:44.000000 QPUIQ-0.2.2/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      563 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2696 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      752 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2331 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/combobox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      710 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      905 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      805 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/mdi.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2782 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/menu.py
+-rw-r--r--   0 Bug        (504) staff       (20)      481 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      772 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3806 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1351 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/splitter.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1532 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1287 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2239 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-06-05 21:22:25.000000 QPUIQ-0.2.2/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3607 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.319873 QPUIQ-0.2.2/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      658 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      610 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      487 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      650 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1205 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      592 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      775 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      736 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      751 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5588 2023-06-05 21:20:44.000000 QPUIQ-0.2.2/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)    13532 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/state.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.322667 QPUIQ-0.2.2/PUI/textual/
+-rw-r--r--   0 Bug        (504) staff       (20)      955 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1963 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2952 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      437 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      519 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1300 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1501 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      502 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      622 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1612 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      388 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      742 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      381 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.324680 QPUIQ-0.2.2/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      461 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      602 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      564 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      450 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1271 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      510 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2161 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      456 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      553 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      854 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1512 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/utils.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2860 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.325242 QPUIQ-0.2.2/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1444 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     5869 2023-06-05 21:20:44.000000 QPUIQ-0.2.2/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-06-05 21:22:26.325654 QPUIQ-0.2.2/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/setup.py
```

### Comparing `QPUIQ-0.2.1/LICENSE.txt` & `QPUIQ-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PKG-INFO` & `QPUIQ-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.1
+Version: 0.2.2
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -92,15 +92,15 @@
 
 ## Layout & Styling
 ```python
 # example/pyside6_feedparser.py
 
 ...
 with VBox():
-    Label(title).qt(StyleSheet="font-weight:bold") # QT-specific
+    Label(title).qt(StyleSheet={"font-weight":"bold"}) # QT-specific
 
     with HBox():
         with Scroll():
             with VBox():
                 for i,e in enumerate(entries):
                     Label(e.title).click(self.entry_selected, i)
                 Spacer()
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/__init__.py` & `QPUIQ-0.2.2/PUI/PySide6/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PUI/PySide6/base.py` & `QPUIQ-0.2.2/PUI/PySide6/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 from .. import *
 
 from PySide6 import QtCore, QtWidgets, QtGui
 
 class QtViewSignal(QtCore.QObject):
     redraw = QtCore.Signal()
 
-def _apply_params(ui, params):
-    HorizontalPolicy = params.get("HorizontalPolicy")
+def _apply_params(ui, node):
+    styles = {}
+    if node.style_fontsize:
+        styles["font"] = f"{node.style_fontsize}pt"
+    if node.style_color:
+        styles["color"] = f"#{node.style_color:06X}"
+    if node.style_bgcolor:
+        styles["background-color"] = f"#{node.style_bgcolor:06X}"
+
+    HorizontalPolicy = node.qt_params.get("HorizontalPolicy")
     if not HorizontalPolicy is None:
         ui.sizePolicy().setHorizontalPolicy(HorizontalPolicy)
 
-    VerticalPolicy = params.get("VerticalPolicy")
+    VerticalPolicy = node.qt_params.get("VerticalPolicy")
     if not VerticalPolicy is None:
         ui.sizePolicy().setVerticalPolicy(VerticalPolicy)
 
-    SizeConstraint = params.get("SizeConstraint")
+    SizeConstraint = node.qt_params.get("SizeConstraint")
     if not SizeConstraint is None:
         ui.setSizeConstraint(SizeConstraint)
 
-    StyleSheet = params.get("StyleSheet")
-    if not StyleSheet is None:
-        ui.setStyleSheet(StyleSheet)
+    StyleSheet = node.qt_params.get("StyleSheet", {})
+    for k,v in StyleSheet.items():
+        styles[k] = v
+
+    if hasattr(ui, "setStyleSheet"):
+        ui.setStyleSheet("".join([f"{k}:{v};" for k,v in styles.items()]))
 
 class QPUIView(PUIView):
     def __init__(self):
         super().__init__()
         self.qt_params = {}
         self.signal = QtViewSignal()
         self.signal.redraw.connect(self.update)
@@ -44,15 +55,15 @@
         self.signal.redraw.emit()
 
     def update(self, prev=None):
         if self.retired_by:
             return
         self.dirty = False
         super().update(prev)
-        _apply_params(self.ui, self.qt_params)
+        _apply_params(self.ui, self)
         self.updating = False
         if self.dirty:
             self.update(prev)
 
     def qt(self, **kwargs):
         for k,v in kwargs.items():
             self.qt_params[k] = v
@@ -69,15 +80,15 @@
         if direct:
             self.ui.deleteLater()
         self.ui = None
         super().destroy(direct)
 
     def update(self, prev=None):
         super().update(prev)
-        _apply_params(self.ui, self.qt_params)
+        _apply_params(self.ui, self)
 
     def qt(self, **kwargs):
         for k,v in kwargs.items():
             self.qt_params[k] = v
         return self
 
 class QtBaseLayout(PUINode):
@@ -89,15 +100,15 @@
         if direct:
             self.ui.deleteLater()
         self.ui = None
         super().destroy(direct)
 
     def update(self, prev=None):
         super().update(prev)
-        _apply_params(self.ui, self.qt_params)
+        _apply_params(self.ui, self)
 
     def addChild(self, idx, child):
         from .layout import QtSpacerItem
         if isinstance(child, QtBaseLayout):
             params = {}
             if not child.layout_weight is None:
                 params["stretch"] = child.layout_weight
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/button.py` & `QPUIQ-0.2.2/PUI/PySide6/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class QtButton(QtBaseWidget):
     def __init__(self, text):
         super().__init__()
         self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.setText(self.text)
             try:
                 self.ui.clicked.disconnect()
             except:
                 pass
             prev.callback = None
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/canvas.py` & `QPUIQ-0.2.2/PUI/PySide6/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         super().__init__()
         self.ui = None
         self.painter = painter
         self.args = args
         self.bgColor = bgColor
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.puinode = self
         else:
             self.ui = PUIQtCanvas(self, self.layout_width or 0, self.layout_height or 0)
         self.ui.update()
         super().update(prev)
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/checkbox.py` & `QPUIQ-0.2.2/PUI/PySide6/checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class QtCheckbox(QtBaseWidget):
     def __init__(self, text, model):
         super().__init__()
         self.text = text
         self.model = model
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             try:
                 self.ui.stateChanged.disconnect()
             except:
                 pass
         else:
             self.ui = QtWidgets.QCheckBox()
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/combobox.py` & `QPUIQ-0.2.2/PUI/PySide6/combobox.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         if text_changed:
             self.text_changed = text_changed
         return self
 
     def update(self, prev):
         index = self.index_model.value
         text = self.text_model.value
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             if prev.last_index != index:
                 self.ui.currentIndexChanged.disconnect()
                 self.ui.setCurrentIndex(index)
                 self.ui.currentIndexChanged.connect(self.on_currentIndexChanged)
             self.last_index = index
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/label.py` & `QPUIQ-0.2.2/PUI/PySide6/label.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class QtLabel(QtBaseWidget):
     def __init__(self, text):
         super().__init__()
         self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.setText(self.text)
         else:
             self.ui = ClickableQLabel(self.text)
             self.ui.setTextFormat(QtCore.Qt.TextFormat.PlainText)
             self.ui.clicked.connect(self._clicked)
         if self.onClicked:
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/layout.py` & `QPUIQ-0.2.2/PUI/PySide6/layout.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from .. import *
 from .base import *
 
 class QtHBox(QtBaseLayout):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QHBoxLayout()
         super().update(prev)
 
 class QtVBox(QtBaseLayout):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QVBoxLayout()
         super().update(prev)
 
 class QtSpacerItem(PUINode):
     terminal = True
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QSpacerItem(0, 0, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         super().update(prev)
 
     def destroy(self, direct):
         # self.ui.deleteLater() # QSpacerItem doesn't have .deleteLater()
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/mdi.py` & `QPUIQ-0.2.2/PUI/PySide6/mdi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from .. import *
 from .base import *
 
 class QtMdiArea(QtBaseWidget):
     terminal = False
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QMdiArea()
 
         super().update(prev)
 
     def addChild(self, idx, child):
         self.ui.addSubWindow(child.outer)
 
     def removeChild(self, idx, child):
         self.ui.removeSubWindow(child.outer)
 
+    def addSubWindow(self, child):
+        self.ui.addSubWindow(child.outer)
+
+    def removeSubWindow(self, child):
+        self.ui.removeSubWindow(child.outer)
+
 class QtMdiSubWindow(QtBaseFrame):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QMdiSubWindow()
 
         super().update(prev)
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/menu.py` & `QPUIQ-0.2.2/PUI/PySide6/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .. import *
 from .base import *
 
 class QtMenuBar(PUINode):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.actions = prev.actions
         else:
             self.ui = QtWidgets.QMenuBar()
             self.actions = []
 
         super().update(prev)
@@ -29,15 +29,15 @@
 
 class QtMenu(PUINode):
     def __init__(self, text):
         super().__init__()
         self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.setTitle(self.text)
             self.actions = prev.actions
         else:
             self.ui = QtWidgets.QMenu(self.text)
             self.actions = []
 
@@ -61,15 +61,15 @@
 class QtAction(PUINode):
     def __init__(self, text):
         super().__init__()
         self.text = text
         self.onTriggered = None
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.setText(self.text)
             self.ui.triggered.disconnect()
         else:
             self.ui = QtGui.QAction(self.text)
         self.ui.triggered.connect(self._triggered)
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/radiobutton.py` & `QPUIQ-0.2.2/PUI/PySide6/radiobutton.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, text, value, model):
         super().__init__()
         self.text = text
         self.value = value
         self.model = model
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             try:
                 self.ui.clicked.disconnect()
             except:
                 pass
         else:
             self.ui = QtWidgets.QRadioButton()
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/scroll.py` & `QPUIQ-0.2.2/PUI/PySide6/scroll.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         if direct:
             if self.widget:
                 self.widget.deleteLater()
                 self.widget = None
         super().destroy(direct)
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.widget = prev.widget
         else:
             self.ui = QtWidgets.QScrollArea()
             self.ui.setWidgetResizable(True)
             self.widget = None
             if self.vertical is None:
@@ -42,17 +42,21 @@
     def addChild(self, idx, child):
         if idx != 0:
             return
         if isinstance(child, QtBaseLayout):
             self.widget = QtWidgets.QWidget()
             self.ui.setWidget(self.widget)
             self.widget.setLayout(child.outer)
+            if not hasattr(self.widget, "origResizeEvent"):
+                self.widget.origResizeEvent = self.widget.resizeEvent
             self.widget.resizeEvent = self.onUiResized
         elif isinstance(child, QtBaseWidget):
             self.ui.setWidget(child.outer)
+            if not hasattr(child.outer, "origResizeEvent"):
+                child.outer.origResizeEvent = child.outer.resizeEvent
             child.outer.resizeEvent = self.onUiResized
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if idx != 0:
             return
@@ -67,16 +71,18 @@
             self.removeChild(idx, child.children[0])
 
     def onUiResized(self, event):
         node = self.get_node()
         if node.destroyed:
             return
         if node.widget:
+            node.widget.origResizeEvent(event)
             node.widget.resizeEvent = self.onUiResized
         else:
+            node.children[0].outer.origResizeEvent(event)
             node.children[0].outer.resizeEvent = self.onUiResized
         if node.horizontal is False:
             if isinstance(node.children[0], QtBaseLayout):
                 node.outer.setMinimumWidth(node.children[0].outer.sizeHint().width())
             elif isinstance(node.children[0], QtBaseWidget):
                 node.outer.setMinimumWidth(node.children[0].outer.sizeHint().width())
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/splitter.py` & `QPUIQ-0.2.2/PUI/PySide6/splitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if direct:
             for frame in self.frame:
                 if frame:
                     frame.deleteLater()
         super().destroy(direct)
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.frame = prev.frame
         else:
             self.ui = QtWidgets.QSplitter()
             self.frame = []
         self.ui.setOrientation(QtCore.Qt.Orientation.Vertical if self.vertical else QtCore.Qt.Orientation.Horizontal)
         super().update(prev)
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/text.py` & `QPUIQ-0.2.2/PUI/PySide6/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     textformat = QtCore.Qt.TextFormat.PlainText
     def __init__(self, text, sizeHint=(120,320)):
         super().__init__()
         self.text = text
         self.sizeHint = sizeHint
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.setText(self.text)
             self.ui.setSizeHint(self.sizeHint)
         else:
             self.ui = QText(self.text, self.sizeHint)
             self.ui.setTextFormat(self.textformat)
             self.ui.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/textfield.py` & `QPUIQ-0.2.2/PUI/PySide6/textfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def __init__(self, model):
         super().__init__()
         self.model = model
         self.editing = False
 
     def update(self, prev):
         value = self.model.value
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.editing = prev.editing
             self.ui = prev.ui
             self.ui.focusOutEvent = self.focusOutEvent
             if prev.last_value != value:
                 self.ui.textChanged.disconnect()
                 if not self.editing:
                     self.ui.setText(str(value))
```

### Comparing `QPUIQ-0.2.1/PUI/PySide6/window.py` & `QPUIQ-0.2.2/PUI/PySide6/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.curr_size = None
         self.maximize = maximize
         self.curr_maximize = None
         self.fullscreen = fullscreen
         self.curr_fullscreen = None
 
     def update(self, prev=None):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.frame = prev.frame
             self.curr_size = prev.curr_size
             self.curr_maximize = prev.curr_maximize
             self.curr_fullscreen = prev.curr_fullscreen
         else:
             from PySide6 import QtWidgets
```

### Comparing `QPUIQ-0.2.1/PUI/dom.py` & `QPUIQ-0.2.2/PUI/dom.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,9 +106,14 @@
     nl = len(newDOM)
     while len(oldDOM) > nl:
         old = oldDOM.pop(nl)
         oldMap.pop(nl)
         node.removeChild(nl, old)
         tbd.append(old)
 
+    for c in newDOM:
+        c.postUpdate()
+
+    node.postSync()
+
     for old in tbd:
         recur_delete(node, old, True)
```

### Comparing `QPUIQ-0.2.1/PUI/flet/__init__.py` & `QPUIQ-0.2.2/PUI/flet/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PUI/flet/application.py` & `QPUIQ-0.2.2/PUI/flet/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PUI/flet/base.py` & `QPUIQ-0.2.2/PUI/flet/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,23 +3,31 @@
 
 def _apply_params(ui, params):
     for k,v in params.items():
         setattr(ui, k, v)
 class FBase(PUINode):
     def __init__(self, *args):
         super().__init__(*args)
+        self.child_weight = None
+        if self.fparent:
+            self.layout_weight = self.fparent.child_weight
+
         self.flet_params = {}
 
     def flet(self, **kwargs):
         for k,v in kwargs.items():
             self.flet_params[k] = v
         return self
 
     def update(self, prev):
         _apply_params(self.ui, self.flet_params)
         super().update(prev)
 
-def find_flet_outer(node):
-    if isinstance(node, FBase):
-        return node.outer
-    else:
-        return find_flet_outer(node.children[0])
+    @property
+    def fparent(self):
+        parent = self.parent
+        while True:
+            if isinstance(parent, FBase):
+                return parent
+            if parent.parent == parent:
+                return None
+            parent = parent.parent
```

### Comparing `QPUIQ-0.2.1/PUI/flet/label.py` & `QPUIQ-0.2.2/PUI/flet/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 class FLabel(FBase):
     def __init__(self, text, **kwargs):
         super().__init__(**kwargs)
         self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = ft.Text(spans=[], expand=self.layout_weight)
+            self.ui = ft.Text(spans=[])
+        self.ui.expand = self.layout_weight
         if self.onClicked:
             self.ui.spans = [
                 ft.TextSpan(self.text, on_click=self._clicked)
             ]
         else:
             self.ui.spans = [
                 ft.TextSpan(self.text)
```

### Comparing `QPUIQ-0.2.1/PUI/flet/layout.py` & `QPUIQ-0.2.2/PUI/flet/layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .. import *
 from .base import *
 
 class FRow(FBase):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = ft.Row(expand=self.layout_weight)
+            self.ui = ft.Row()
+        self.ui.expand = self.layout_weight
         super().update(prev)
 
     def addChild(self, idx, child):
         self.ui.controls.insert(idx, child.outer)
         try:
             self.ui.update()
         except:
@@ -18,18 +19,19 @@
 
     def removeChild(self, idx, child):
         self.ui.controls.pop(idx)
         self.ui.update()
 
 class FColumn(FBase):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = ft.Column(expand=self.layout_weight)
+            self.ui = ft.Column()
+        self.ui.expand = self.layout_weight
         super().update(prev)
 
     def addChild(self, idx, child):
         self.ui.controls.insert(idx, child.outer)
         try:
             self.ui.update()
         except:
@@ -37,12 +39,12 @@
 
     def removeChild(self, idx, child):
         self.ui.controls.pop(idx)
         self.ui.update()
 
 class FSpacer(FBase):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = ft.Container()
         super().update(prev)
```

### Comparing `QPUIQ-0.2.1/PUI/flet/scroll.py` & `QPUIQ-0.2.2/PUI/flet/scroll.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,41 @@
 
 class FScroll(FBase):
     def __init__(self, vertical=None, horizontal=False):
         self.vertical = vertical
         self.horizontal = horizontal
         self.widget = None
         super().__init__()
+        self.layout_weight = 1
 
     def update(self, prev):
         if prev and hasattr(prev, "hframe"):
             self.vframe = prev.vframe
             self.hframe = prev.hframe
-            self.vframe.update()
         else:
             self.vframe = ft.Column() # outer
             self.hframe = ft.Row() # inner
             self.vframe.controls.append(self.hframe)
-            if self.vertical is None:
-                self.vframe.scroll = ft.ScrollMode.AUTO
-            elif self.vertical:
-                self.vframe.scroll = ft.ScrollMode.ADAPTIVE
-            else:
-                self.vframe.scroll = None
-            if self.horizontal is None:
-                self.hframe.scroll = ft.ScrollMode.AUTO
-            elif self.horizontal:
-                self.hframe.scroll = ft.ScrollMode.ADAPTIVE
-            else:
-                self.hframe.scroll = None
+        self.vframe.expand = self.layout_weight
+        if self.vertical is None:
+            self.vframe.scroll = ft.ScrollMode.AUTO
+        elif self.vertical:
+            self.vframe.scroll = ft.ScrollMode.ADAPTIVE
+        else:
+            self.vframe.scroll = None
+        if self.horizontal is None:
+            self.hframe.scroll = ft.ScrollMode.AUTO
+        elif self.horizontal:
+            self.hframe.scroll = ft.ScrollMode.ADAPTIVE
+        else:
+            self.hframe.scroll = None
+        try:
+            self.vframe.update()
+        except:
+            pass
 
     def addChild(self, idx, child):
         if idx != 0:
             return
         self.hframe.controls.insert(idx, child.outer)
         try:
             self.hframe.update()
```

### Comparing `QPUIQ-0.2.1/PUI/flet/text.py` & `QPUIQ-0.2.2/PUI/flet/text.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 class FText(FBase):
     def __init__(self, text, **kwargs):
         super().__init__(**kwargs)
         self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.value = self.text
             self.ui.update()
         else:
             self.ui = ft.Text(self.text, expand=self.layout_weight)
 
 class FHtml(FBase):
     supported = False
     def __init__(self, text, **kwargs):
         super().__init__(**kwargs)
         self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.value = self.text
             self.ui.update()
         else:
             self.ui = ft.Text(self.text, expand=self.layout_weight)
```

### Comparing `QPUIQ-0.2.1/PUI/flet/textfield.py` & `QPUIQ-0.2.2/PUI/flet/textfield.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def __init__(self, model, label="", **kwargs):
         super().__init__(**kwargs)
         self.model = model
         self.label = label
 
     def update(self, prev):
         value = self.model.value
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             if prev.last_value != value:
                 self.ui.value = str(value)
                 self.ui.update()
             self.last_value = value
         else:
             self.last_value = value
```

### Comparing `QPUIQ-0.2.1/PUI/flet/window.py` & `QPUIQ-0.2.2/PUI/flet/window.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from .. import *
 from .base import *
 
-class FWindow(PUINode):
+class FWindow(FBase):
     def __init__(self, title=None, size=None, maximize=None, fullscreen=None):
         super().__init__()
         self.title = title
         self.size = size
         self.curr_size = None
         self.maximize = maximize
         self.curr_maximize = None
         self.fullscreen = fullscreen
         self.curr_fullscreen = None
+        self.child_weight = 1
 
     def update(self, prev=None):
-        self.parent.ui.title = self.title
+        self.inner.title = self.title
         super().update(prev)
 
     def addChild(self, idx, child):
         if idx != 0:
             return
-        self.parent.ui.add(child.ui)
+        self.inner.add(child.outer)
 
     def removeChild(self, idx, child):
         if idx != 0:
             return
-        self.parent.ui.remove(child.ui)
+        self.inner.remove(child.outer)
```

### Comparing `QPUIQ-0.2.1/PUI/node.py` & `QPUIQ-0.2.2/PUI/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,20 +19,26 @@
 
         if not hasattr(self, "name"):
             self.name = None
 
         self.destroyed = False
         self.retired_by = None
         self._debug = 0
+        self._tag = ""
 
         self.layout_weight = None
         self.layout_width = None
         self.layout_height = None
         self.layout_padding = None
         self.layout_margin = None
+        self.style_color = None
+        self.style_bgcolor = None
+        self.style_fontsize = None
+        self.style_fontweight = None
+        self.style_fontfamily = None
 
         self.onClicked = None
 
         self.ui = None
         self.args = args
         try:
             self.root = find_puiview()
@@ -40,26 +46,32 @@
         except PuiViewNotFoundError:
             self.root = self
             self.parent = self
 
         if isinstance(self, PUIView):
             self.root = self
 
-        # key has to be relative to PUIView, so that it can be identical when a sub-PUIView is updated individually
-        self.key = "|".join([x.name or type(x).__name__ for x in self.root.frames]+[self.name or type(self).__name__]+[str(id(x)) for x in self.args])
+        self.genKey()
 
         self.children = []
 
         if self.parent is self:
             self.path = tuple()
         else:
             self.path = self.parent.path + tuple([len(self.parent.children)])
             self.parent.children.append(self)
+
         # print(type(self).__name__, self.path, "parent=", self.parent.path)
 
+    def genKey(self):
+        # key has to be relative to PUIView, so that it can be identical when a sub-PUIView is updated individually
+        self.key = "|".join([x.name or type(x).__name__ for x in self.root.frames]+[self.name or type(self).__name__]+[str(id(x)) for x in self.args])
+        if self._tag:
+            self.key += f"@{self._tag}"
+
     def __enter__(self):
         # print("enter", type(self).__name__, id(self))
         self.root.frames.append(self)
         return self
 
     def __exit__(self, ex_type, value, traceback):
         # print("exit", type(self).__name__, id(self))
@@ -84,28 +96,39 @@
     def comment(self):
         return None
 
     def update(self, prev):
         if prev:
             prev.retired_by = self
 
+    def postUpdate(self):
+        pass
+
+    def postSync(self):
+        pass
+
     def destroy(self, direct):
         self.root = None
         self.parent = None
 
     def addChild(self, idx, child):
         pass
 
     def removeChild(self, idx, child):
         pass
 
     def debug(self, level=1):
         self._debug = level
         return self
 
+    def tag(self, name):
+        self._tag = name
+        self.genKey()
+        return self
+
     def get_node(self):
         node = self
         while node.retired_by:
             node = node.retired_by
         return node
 
     def __repr__(self):
@@ -149,14 +172,28 @@
         if not padding is None:
             self.layout_padding = trbl(padding)
         if not margin is None:
             self.layout_margin = trbl(margin)
 
         return self
 
+    def style(self, color=None, bgColor=None, fontSize=None, fontWeight=None, fontFamily=None):
+        if not color is None:
+            self.style_color = color
+        if not bgColor is None:
+            self.style_bgcolor = bgColor
+        if not fontSize is None:
+            self.style_fontsize = fontSize
+        if not fontWeight is None:
+            self.style_fontweight = fontWeight
+        if not fontFamily is None:
+            self.style_fontfamily = fontFamily
+
+        return self
+
     def click(self, callback, *cb_args, **cb_kwargs):
         self.onClicked = callback
         self.click_args = cb_args
         self.click_kwargs = cb_kwargs
         return self
 
     def _clicked(self, *args, **kwargs):
```

### Comparing `QPUIQ-0.2.1/PUI/state.py` & `QPUIQ-0.2.2/PUI/state.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PUI/textual/__init__.py` & `QPUIQ-0.2.2/PUI/textual/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class DummyWidget(TBase):
     supported = False
     def __init__(self, *args, **kwrgas):
         super().__init__()
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = widgets.Label("Not Implemented")
 
 
 Application = TApplication
 Window = TWindow
```

### Comparing `QPUIQ-0.2.1/PUI/textual/application.py` & `QPUIQ-0.2.2/PUI/textual/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PUI/textual/checkbox.py` & `QPUIQ-0.2.2/PUI/textual/checkbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class TCheckbox(TBase):
     def __init__(self, text, model):
         super().__init__()
         self.text = text
         self.model = model
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.ui.value = self.model.value
         else:
             self.ui = widgets.Checkbox(self.text, self.model.value)
 
         self.ui.puinode = self
         super().update(prev)
```

### Comparing `QPUIQ-0.2.1/PUI/textual/label.py` & `QPUIQ-0.2.2/PUI/textual/label.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from .. import *
 from .base import *
 
 class TLabel(TBase):
     def __init__(self, text, **kwargs):
         super().__init__(**kwargs)
+        self.widget = None
         self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.widget = prev.widget
         else:
             self.ui = containers.Container()
             self.ui.set_styles("width: auto; height: auto;")
-            self.widget = None
         if self.onClicked:
             if self.widget is None or not isinstance(self.widget, widgets.Button):
                 if self.widget:
                     self.widget.remove()
                 self.widget = widgets.Button(self.text)
                 self.widget.set_styles("height: 1; border-top: none; border-bottom: none; min-width: 0;")
                 self.widget.puinode = self
@@ -28,7 +28,8 @@
             if self.widget is None or not isinstance(self.widget, widgets.Label):
                 if self.widget:
                     self.widget.remove()
                 self.widget = widgets.Label(self.text, markup=False)
                 self.ui.mount(self.widget)
             else:
                 self.widget.update(self.text)
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.1/PUI/textual/textfield.py` & `QPUIQ-0.2.2/PUI/textual/textfield.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 class TInput(TBase):
     content_width = None
     def __init__(self, model):
         super().__init__()
         self.model = model
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             model_value = self.model.value
             if self.ui_text != model_value:
                 self.ui_text = model_value
                 self.ui.value = model_value
         else:
             self.ui_text = self.model.value
             self.ui = widgets.Input(self.ui_text)
 
         self.ui.puinode = self
+        super().update(prev)
 
 
     def _changed(self, value):
         self.ui_text = value
         self.model.value = value
 
     def _submitted(self, value):
```

### Comparing `QPUIQ-0.2.1/PUI/timeline.py` & `QPUIQ-0.2.2/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PUI/tkinter/application.py` & `QPUIQ-0.2.2/PUI/tkinter/application.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     def redraw(self):
         if self.ui:
             self.ui.after(0, functools.partial(self.update, redraw=True))
         else:
             self.update(redraw=True)
 
     def update(self, prev=None):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = tk.Tk()
             self.ui.withdraw()
 
         super().update(prev)
```

### Comparing `QPUIQ-0.2.1/PUI/tkinter/base.py` & `QPUIQ-0.2.2/PUI/tkinter/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/PUI/tkinter/canvas.py` & `QPUIQ-0.2.2/PUI/tkinter/canvas.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         super().__init__()
         self.painter = painter
         self.args = args
         self.size = size
         self.bgColor = bgColor
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = tk.Canvas(self.parent.ui, **self.kwargs)
         self.ui.delete("all")
 
         if self.bgColor:
             self.ui.config(bg=f"#{self.bgColor:06X}")
```

### Comparing `QPUIQ-0.2.1/PUI/tkinter/layout.py` & `QPUIQ-0.2.2/PUI/tkinter/layout.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .. import *
 from .base import *
 
 class TkHBox(TkBaseWidget):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = tk.Frame(self.tkparent.inner)
             self.ui.grid_rowconfigure(0, weight=1)
 
     def addChild(self, idx, child):
         if isinstance(child, TkBaseWidget):
@@ -24,15 +24,15 @@
         if isinstance(child, TkBaseWidget):
             child.ui.grid_forget()
         elif child.children:
             self.removeChild(idx, child.children[0])
 
 class TkVBox(TkBaseWidget):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = tk.Frame(self.tkparent.inner)
             self.ui.config(bg="white")
             self.ui.grid_columnconfigure(0, weight=1)
 
     def addChild(self, idx, child):
@@ -54,11 +54,11 @@
 
 class TkSpacer(TkBaseWidget):
     def __init__(self, *args):
         super().__init__(*args)
         self.layout_weight = 1
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = tk.Frame(self.tkparent.inner)
```

### Comparing `QPUIQ-0.2.1/PUI/tkinter/scroll.py` & `QPUIQ-0.2.2/PUI/tkinter/scroll.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .. import *
 from .base import *
 from tkinter.scrolledtext import ScrolledText
 
 class TkScroll(TkBaseWidget):
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = ScrolledText(self.tkparent.ui, state='disable')
             self.ui.grid(row=0, column=0, sticky='nsew')
             self.ui.config(cursor="arrow")
 
     def addChild(self, idx, child):
```

### Comparing `QPUIQ-0.2.1/PUI/tkinter/textfield.py` & `QPUIQ-0.2.2/PUI/tkinter/textfield.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class TkEntry(TkBaseWidget):
     def __init__(self, model, **kwargs):
         super().__init__(**kwargs)
         self.model = model
 
     def update(self, prev):
         value = self.model.value
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.variable = prev.variable
             self.ui = prev.ui
             if prev.last_value != value:
                 self.variable.set(value)
             self.last_value = value
         else:
             self.variable = tk.StringVar(self.parent.ui, str(value))
```

### Comparing `QPUIQ-0.2.1/PUI/tkinter/window.py` & `QPUIQ-0.2.2/PUI/tkinter/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.curr_size = None
         self.maximize = maximize
         self.curr_maximize = None
         self.fullscreen = fullscreen
         self.curr_fullscreen = None
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
+        if prev and prev.ui:
             self.ui = prev.ui
             self.curr_size = prev.curr_size
             self.curr_maximize = prev.curr_maximize
             self.curr_fullscreen = prev.curr_fullscreen
         else:
             self.ui = tk.Toplevel(self.parent.ui)
```

### Comparing `QPUIQ-0.2.1/PUI/view.py` & `QPUIQ-0.2.2/PUI/view.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.1/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.2.2/QPUIQ.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.1
+Version: 0.2.2
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -92,15 +92,15 @@
 
 ## Layout & Styling
 ```python
 # example/pyside6_feedparser.py
 
 ...
 with VBox():
-    Label(title).qt(StyleSheet="font-weight:bold") # QT-specific
+    Label(title).qt(StyleSheet={"font-weight":"bold"}) # QT-specific
 
     with HBox():
         with Scroll():
             with VBox():
                 for i,e in enumerate(entries):
                     Label(e.title).click(self.entry_selected, i)
                 Spacer()
```

### Comparing `QPUIQ-0.2.1/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.2.2/QPUIQ.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 PUI/PySide6/radiobutton.py
 PUI/PySide6/scroll.py
 PUI/PySide6/splitter.py
 PUI/PySide6/text.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
 PUI/flet/__init__.py
-PUI/flet/appbar.py
 PUI/flet/application.py
 PUI/flet/base.py
 PUI/flet/button.py
 PUI/flet/label.py
 PUI/flet/layout.py
 PUI/flet/progressbar.py
 PUI/flet/scroll.py
```

### Comparing `QPUIQ-0.2.1/README.md` & `QPUIQ-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ## Layout & Styling
 ```python
 # example/pyside6_feedparser.py
 
 ...
 with VBox():
-    Label(title).qt(StyleSheet="font-weight:bold") # QT-specific
+    Label(title).qt(StyleSheet={"font-weight":"bold"}) # QT-specific
 
     with HBox():
         with Scroll():
             with VBox():
                 for i,e in enumerate(entries):
                     Label(e.title).click(self.entry_selected, i)
                 Spacer()
```

### Comparing `QPUIQ-0.2.1/setup.py` & `QPUIQ-0.2.2/setup.py`

 * *Files identical despite different names*

