# Comparing `tmp/bqt-0.2.0.tar.gz` & `tmp/bqt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bqt-0.2.0.tar", last modified: Fri Jun 19 19:22:36 2020, max compression
+gzip compressed data, was "bqt-1.0.0.tar", last modified: Mon Jun  5 15:15:34 2023, max compression
```

## Comparing `bqt-0.2.0.tar` & `bqt-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,46 @@
-drwxrwxrwx   0        0        0        0 2020-06-19 19:22:36.000000 bqt-0.2.0/
--rw-rw-rw-   0        0        0       38 2020-06-19 19:22:10.000000 bqt-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      590 2020-06-19 19:22:36.000000 bqt-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      261 2020-06-19 19:22:10.000000 bqt-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt/
--rw-rw-rw-   0        0        0     3430 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt/blender_applications/
--rw-rw-rw-   0        0        0      535 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/blender_applications/__init__.py
--rw-rw-rw-   0        0        0     4829 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/blender_applications/blender_application.py
--rw-rw-rw-   0        0        0     2311 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/blender_applications/darwin_blender_application.py
--rw-rw-rw-   0        0        0     1171 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/blender_applications/win32_blender_application.py
--rw-rw-rw-   0        0        0      471 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/blender_icon_16.png
--rw-rw-rw-   0        0        0     5967 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/blender_stylesheet.qss
-drwxrwxrwx   0        0        0        0 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt/dist/
--rw-rw-rw-   0        0        0      133 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/dist/bqt_startup.py
--rw-rw-rw-   0        0        0     1180 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/hello_world.py
-drwxrwxrwx   0        0        0        0 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt/images/
--rw-rw-rw-   0        0        0      835 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QCheckBox_checked.png
--rw-rw-rw-   0        0        0      656 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QCheckBox_unchecked.png
--rw-rw-rw-   0        0        0      836 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QCheckbox_checked_hover.png
--rw-rw-rw-   0        0        0      663 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QCheckbox_unchecked_hover.png
--rw-rw-rw-   0        0        0      702 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QComboBox_down_arrow.png
--rw-rw-rw-   0        0        0     5238 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QRadioButton_checked.png
--rw-rw-rw-   0        0        0     5435 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QRadioButton_checked_hover.png
--rw-rw-rw-   0        0        0     4224 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QRadioButton_unchecked.png
--rw-rw-rw-   0        0        0     4526 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QRadioButton_unchecked_hover.png
--rw-rw-rw-   0        0        0     2777 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QSpinBox_down_arrow.png
--rw-rw-rw-   0        0        0      708 2020-06-19 19:22:10.000000 bqt-0.2.0/bqt/images/QSpinBox_up_arrow.png
-drwxrwxrwx   0        0        0        0 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt.egg-info/
--rw-rw-rw-   0        0        0      590 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2020-06-19 19:22:36.000000 bqt-0.2.0/bqt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-19 19:22:36.000000 bqt-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3742 2020-06-19 19:22:10.000000 bqt-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.875142 bqt-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-05 15:15:25.000000 bqt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-05 15:15:25.000000 bqt-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-05 15:15:34.875142 bqt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-05 15:15:25.000000 bqt-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.867142 bqt-1.0.0/bqt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.867142 bqt-1.0.0/bqt/blender_applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/darwin_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/win32_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.871142 bqt-1.0.0/bqt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckBox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckBox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckbox_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckbox_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QComboBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QSpinBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QSpinBox_up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/blender_icon_16.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.871142 bqt-1.0.0/bqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/ui/quit_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.867142 bqt-1.0.0/bqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.875142 bqt-1.0.0/bqt_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/anim_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/pyside_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:15:34.875142 bqt-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-05 15:15:25.000000 bqt-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bqt-0.2.0/bqt/blender_applications/blender_application.py` & `bqt-1.0.0/bqt/blender_applications/blender_application.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,53 +2,63 @@
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """
 
 from abc import abstractmethod, abstractstaticmethod, ABCMeta
 from pathlib import Path
-
+import os
 from PySide2.QtWidgets import QApplication, QWidget
+from PySide2.QtWidgets import QMainWindow
 from PySide2.QtGui import QCloseEvent, QIcon, QImage, QPixmap, QWindow
 from PySide2.QtCore import QEvent, QObject, QRect, QSettings
+from bqt.ui.quit_dialogue import BlenderClosingDialog
+import bpy
+
+
+STYLESHEET_PATH = Path(__file__).parents[1] / "blender_stylesheet.qss"
+ORGANISATION = "Tech-Artists.org"
+APP = "Blender Qt"
+WINDOW_TITLE = "Blender Qt"
+WINDOW_GROUP_NAME = "MainWindow"
+GEOMETRY = "Geometry"
+MAXIMIZED = "IsMaximized"
+FULL_SCREEN = "IsFullScreen"
 
 
 class BlenderApplication(QApplication):
     """
     Base Implementation for QT Blender Window Container
     """
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         __metaclass__ = ABCMeta
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
-        self._stylesheet_filepath = Path(__file__).parent / ".." / "blender_stylesheet.qss"
-        self._settings_key_geometry = "Geometry"
-        self._settings_key_maximized = "IsMaximized"
-        self._settings_key_full_screen = "IsFullScreen"
-        self._settings_key_window_group_name = "MainWindow"
-
-        # QApplication
-        if self._stylesheet_filepath.exists():
-            self.setStyleSheet(self._stylesheet_filepath.read_text())
+        if STYLESHEET_PATH.exists():
+            self.setStyleSheet(STYLESHEET_PATH.read_text())
 
         QApplication.setWindowIcon(self._get_application_icon())
 
         # Blender Window
         self._hwnd = self._get_application_hwnd()
-        self._blender_window = QWindow.fromWinId(self._hwnd)
-        self.blender_widget = QWidget.createWindowContainer(self._blender_window)
-        self.blender_widget.setWindowTitle("Blender")
-
-        # Variables
-        self.should_close = False
-
-        # Runtime
-        self._set_window_geometry()
-        self.focusObjectChanged.connect(self._on_focus_object_changed)
+        failed_to_get_handle = self._hwnd is None
+
+        if os.getenv("BQT_DISABLE_WRAP") == "1" or failed_to_get_handle:
+            self._blender_window = QWindow()
+            self.blender_widget = QWidget.createWindowContainer(self._blender_window)
+        else:
+            self.blender_widget = QMainWindow()
+            self.blender_widget.setWindowTitle(WINDOW_TITLE)
+            self._blender_window = QWindow.fromWinId(self._hwnd)  # also sets flag to Qt.ForeignWindow
+            self.window_container = QMainWindow.createWindowContainer(self._blender_window)
+            self.blender_widget.setCentralWidget(self.window_container)
+            self._set_window_geometry()
+            self.blender_widget.show()
+            self.focusObjectChanged.connect(self._on_focus_object_changed)
 
     @abstractstaticmethod
     def _get_application_hwnd() -> int:
         """
         This finds the blender application window and collects the
         handler window ID
 
@@ -62,15 +72,15 @@
         """
         This finds the running blender process, extracts the blender icon from the blender.exe file on disk and saves it to the user's temp folder.
         It then creates a QIcon with that data and returns it.
 
         Returns QIcon: Application Icon
         """
 
-        icon_filepath = Path(__file__).parent / ".." / "blender_icon_16.png"
+        icon_filepath = Path(__file__).parents[1] / "images" / "blender_icon_16.png"
         icon = QIcon()
 
         if icon_filepath.exists():
             image = QImage(str(icon_filepath))
             if not image.isNull():
                 icon = QIcon(QPixmap().fromImage(image))
 
@@ -81,61 +91,91 @@
         """
         Args:
             focus_object: Object to track focus event
         """
 
         pass
 
+    def _unwrapped_window_geometry(self) -> QRect:
+        """
+        Get the window geometry from the Blender window before it was wrapped in a QWidgetContainer
+        Run this before wrapping the window in a QWidgetContainer
+        Returns QRect(x, y, width, height)
+        """
+        window = bpy.context.window_manager.windows[0]
+        height, widht = window.height, window.width
+        x = window.x
+        y = window.y  # blender y relative from bottom of screen to bottom of Blender window
+        # convert y to be relative from the top
+        current_screen_rect = self.primaryScreen().availableGeometry()
+        y = current_screen_rect.height() - y - height
+        y += 56  # title bar offset
+        return QRect(x, y, widht, height)
+
+
     def _set_window_geometry(self):
         """
         Loads stored window geometry preferences and applies them to the QWindow.
         .setGeometry() sets the size of the window minus the window frame.
         For this reason it should be set on self.blender_widget.
         """
+        settings = QSettings(ORGANISATION, APP)
+        settings.beginGroup(WINDOW_GROUP_NAME)
+        fullscreen = settings.value(FULL_SCREEN, defaultValue=False, type=bool)
+        maximized = settings.value(MAXIMIZED, defaultValue=False, type=bool)
+        saved_geometry = settings.value(GEOMETRY)
+        settings.endGroup()
 
-        settings = QSettings('Tech-Artists.org', 'Blender Qt Wrapper')
-        settings.beginGroup(self._settings_key_window_group_name)
-
-        if settings.value(self._settings_key_full_screen, 'false').lower() == 'true':
+        if fullscreen:
             self.blender_widget.showFullScreen()
             return
 
-        if settings.value(self._settings_key_maximized, 'false').lower() == 'true':
+        if maximized:
             self.blender_widget.showMaximized()
             return
 
-        self.blender_widget.setGeometry(settings.value(self._settings_key_geometry, QRect(0, 0, 640, 480)))
-        self.blender_widget.show()
 
-        settings.endGroup()
-        return
+        unwrapped_geometry = self._unwrapped_window_geometry()  # maintain unwrapped window size & pos
+        geometry = saved_geometry or unwrapped_geometry  # if no saved geometry, use previous blender window size
+        self.blender_widget.setGeometry(geometry)  # setGeometry is relative to its parent
+
 
     def notify(self, receiver: QObject, event: QEvent) -> bool:
         """
         Args:
-            receiver: Object to recieve event
+            receiver: Object to receive event
             event: Event
 
         Returns: bool
         """
 
         if isinstance(event, QCloseEvent) and receiver in (self.blender_widget, self._blender_window):
+            # catch the close event when clicking close on the qt window,
+            # ignore the event, and ask user if they want to close blender if unsaved changes.
             event.ignore()
-            self.store_window_geometry()
-            self.should_close = True
+
+            self.store_window_geometry()  # save qt window geometry, to restore on next launch
+
+            if os.getenv("BQT_DISABLE_CLOSE_DIALOGUE") == "1":
+                # this triggers the default blender close event, showing the save dialog if needed
+                bpy.ops.wm.quit_blender({"window": bpy.context.window_manager.windows[0]}, "INVOKE_DEFAULT")
+            else:
+                closing_dialog = BlenderClosingDialog(self.blender_widget)
+                closing_dialog.execute()
+
             return False
 
         return super().notify(receiver, event)
 
     def store_window_geometry(self):
         """
         Stores the current window geometry for the QWindow
         The .geometry() method on QWindow includes the size of the application minus the window frame.
         For that reason the _blender_widget should be used.
         """
 
-        settings = QSettings('Tech-Artists.org', 'Blender Qt Wrapper')
-        settings.beginGroup(self._settings_key_window_group_name)
-        settings.setValue(self._settings_key_geometry, self.blender_widget.geometry())
-        settings.setValue(self._settings_key_maximized, self.blender_widget.isMaximized())
-        settings.setValue(self._settings_key_full_screen, self.blender_widget.isFullScreen())
+        settings = QSettings(ORGANISATION, APP)
+        settings.beginGroup(WINDOW_GROUP_NAME)
+        settings.setValue(GEOMETRY, self.blender_widget.geometry())
+        settings.setValue(MAXIMIZED, self.blender_widget.isMaximized())
+        settings.setValue(FULL_SCREEN, self.blender_widget.isFullScreen())
         settings.endGroup()
```

### Comparing `bqt-0.2.0/bqt/blender_applications/darwin_blender_application.py` & `bqt-1.0.0/bqt/blender_applications/darwin_blender_application.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from .blender_application import BlenderApplication
 
 
 class DarwinBlenderApplication(BlenderApplication):
     """
     Darwin (MACOS) Implementation of BlenderApplication
     """
-    def __init__(self):
+
+    def __init__(self, *args, **kwargs):
         # OSX Specific - Needs to initialize first
         self._ns_window = self.__get_application_window() or None
 
-        super().__init__()
-
+        super().__init__(*args, **kwargs)
 
     def _get_application_hwnd(self) -> int:
         """
         This finds the blender application window and collects the
         handler window ID
 
         Returns int: Handler Window ID
@@ -40,44 +40,43 @@
 
         # Check to ensure ns_window is set
         if self._ns_window is None:
             self._ns_window = self.__get_application_window()
 
         return objc.pyobjc_id(self._ns_window.contentView())
 
-
     @staticmethod
     def _get_application_icon() -> QIcon:
         """
         This finds the running blender process, extracts the blender icon from the blender.exe file on disk and saves it to the user's temp folder.
         It then creates a QIcon with that data and returns it.
 
         Returns QIcon: Application Icon
         """
 
         blender_path = bpy.app.binary_path
         contents_path = Path(blender_path).resolve().parent.parent
         icon_path = contents_path / "Resources" / "blender icon.icns"
         return QIcon(str(icon_path))
 
-
     @staticmethod
     def _get_application_window() -> AppKit.NSApp.mainWindow:
         """
         Specific to OSX; Main application window
 
         Returns: Main NSWindow of the application
         """
 
         ns_window = AppKit.NSApp.mainWindow()
         ns_window.setSharingType_(AppKit.NSWindowSharingReadWrite)
         return ns_window
 
-
     def _on_focus_object_changed(self, focus_object: QObject):
         """
         Args:
             focus_object: Object to track focus event
         """
 
         if focus_object is self.blender_widget:
             self._ns_window.makeKey()
+            with bpy.context.temp_override(window=bpy.context.window_manager.windows[0]):
+                bpy.ops.bqt.return_focus("INVOKE_DEFAULT")
```

### Comparing `bqt-0.2.0/bqt/images/QCheckBox_checked.png` & `bqt-1.0.0/bqt/images/QCheckBox_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QCheckBox_unchecked.png` & `bqt-1.0.0/bqt/images/QCheckBox_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QCheckbox_checked_hover.png` & `bqt-1.0.0/bqt/images/QCheckbox_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QCheckbox_unchecked_hover.png` & `bqt-1.0.0/bqt/images/QCheckbox_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QComboBox_down_arrow.png` & `bqt-1.0.0/bqt/images/QComboBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QRadioButton_checked.png` & `bqt-1.0.0/bqt/images/QRadioButton_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QRadioButton_checked_hover.png` & `bqt-1.0.0/bqt/images/QRadioButton_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QRadioButton_unchecked.png` & `bqt-1.0.0/bqt/images/QRadioButton_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QRadioButton_unchecked_hover.png` & `bqt-1.0.0/bqt/images/QRadioButton_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QSpinBox_down_arrow.png` & `bqt-1.0.0/bqt/images/QSpinBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt/images/QSpinBox_up_arrow.png` & `bqt-1.0.0/bqt/images/QSpinBox_up_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-0.2.0/bqt.egg-info/SOURCES.txt` & `bqt-1.0.0/bqt.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 bqt/__init__.py
-bqt/blender_icon_16.png
 bqt/blender_stylesheet.qss
-bqt/hello_world.py
+bqt/focus.py
+bqt/utils.py
 bqt.egg-info/PKG-INFO
 bqt.egg-info/SOURCES.txt
 bqt.egg-info/dependency_links.txt
 bqt.egg-info/requires.txt
 bqt.egg-info/top_level.txt
 bqt/blender_applications/__init__.py
 bqt/blender_applications/blender_application.py
 bqt/blender_applications/darwin_blender_application.py
 bqt/blender_applications/win32_blender_application.py
-bqt/dist/bqt_startup.py
 bqt/images/QCheckBox_checked.png
 bqt/images/QCheckBox_unchecked.png
 bqt/images/QCheckbox_checked_hover.png
 bqt/images/QCheckbox_unchecked_hover.png
 bqt/images/QComboBox_down_arrow.png
 bqt/images/QRadioButton_checked.png
 bqt/images/QRadioButton_checked_hover.png
 bqt/images/QRadioButton_unchecked.png
 bqt/images/QRadioButton_unchecked_hover.png
 bqt/images/QSpinBox_down_arrow.png
-bqt/images/QSpinBox_up_arrow.png
+bqt/images/QSpinBox_up_arrow.png
+bqt/images/blender_icon_16.png
+bqt/ui/__init__.py
+bqt/ui/quit_dialogue.py
+bqt_demo/__init__.py
+bqt_demo/anim_bar.py
+bqt_demo/demo.py
+bqt_demo/hello_world.py
+bqt_demo/pyside_widgets.py
+bqt_demo/timer.py
```

