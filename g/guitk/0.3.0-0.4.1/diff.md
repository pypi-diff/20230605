# Comparing `tmp/guitk-0.3.0.tar.gz` & `tmp/guitk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guitk-0.3.0.tar", max compression
+gzip compressed data, was "guitk-0.4.1.tar", max compression
```

## Comparing `guitk-0.3.0.tar` & `guitk-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,40 @@
--rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.3.0/LICENSE
--rw-r--r--   0        0        0    20755 2023-04-23 23:35:05.323243 guitk-0.3.0/README.md
--rw-r--r--   0        0        0     1137 2023-04-23 23:35:20.854105 guitk-0.3.0/guitk/__init__.py
--rw-r--r--   0        0        0    18484 2023-02-17 19:39:03.000000 guitk-0.3.0/guitk/__main__.py
--rw-r--r--   0        0        0      195 2023-02-14 15:07:46.000000 guitk-0.3.0/guitk/constants.py
--rw-r--r--   0        0        0     2844 2021-03-10 13:52:24.000000 guitk-0.3.0/guitk/redirect.py
--rw-r--r--   0        0        0     2726 2023-02-17 17:18:36.000000 guitk-0.3.0/guitk/tkroot.py
--rw-r--r--   0        0        0     8651 2021-03-08 00:27:37.000000 guitk-0.3.0/guitk/tooltips.py
--rw-r--r--   0        0        0      268 2023-02-15 06:15:34.000000 guitk-0.3.0/guitk/utils.py
--rw-r--r--   0        0        0     1729 2023-04-23 23:35:05.330433 guitk-0.3.0/guitk/widgets/__init__.py
--rw-r--r--   0        0        0     1328 2023-02-16 14:26:34.000000 guitk-0.3.0/guitk/widgets/debugwindow.py
--rw-r--r--   0        0        0     2048 2023-04-23 23:35:05.331122 guitk-0.3.0/guitk/widgets/events.py
--rw-r--r--   0        0        0     1767 2023-04-23 23:35:05.331577 guitk-0.3.0/guitk/widgets/layout.py
--rw-r--r--   0        0        0     3414 2023-02-15 06:05:03.000000 guitk-0.3.0/guitk/widgets/menu.py
--rw-r--r--   0        0        0    10075 2023-04-23 20:56:32.282982 guitk-0.3.0/guitk/widgets/tk_text.py
--rw-r--r--   0        0        0    11231 2023-04-23 20:51:03.320462 guitk-0.3.0/guitk/widgets/ttk_button.py
--rw-r--r--   0        0        0     4309 2023-04-23 16:27:37.000000 guitk-0.3.0/guitk/widgets/ttk_checkbutton.py
--rw-r--r--   0        0        0     3656 2023-04-23 16:26:00.000000 guitk-0.3.0/guitk/widgets/ttk_combobox.py
--rw-r--r--   0        0        0     8950 2023-04-23 15:10:08.000000 guitk-0.3.0/guitk/widgets/ttk_entry.py
--rw-r--r--   0        0        0     6852 2023-04-23 21:03:50.313984 guitk-0.3.0/guitk/widgets/ttk_label.py
--rw-r--r--   0        0        0     5158 2023-04-23 23:35:05.332225 guitk-0.3.0/guitk/widgets/ttk_notebook.py
--rw-r--r--   0        0        0     4655 2023-04-23 16:28:49.000000 guitk-0.3.0/guitk/widgets/ttk_progressbar.py
--rw-r--r--   0        0        0     5496 2023-04-23 16:29:42.000000 guitk-0.3.0/guitk/widgets/ttk_radiobutton.py
--rw-r--r--   0        0        0     4462 2023-04-22 16:14:22.000000 guitk-0.3.0/guitk/widgets/ttk_scale.py
--rw-r--r--   0        0        0    11640 2023-04-23 16:26:50.000000 guitk-0.3.0/guitk/widgets/ttk_treeview.py
--rw-r--r--   0        0        0      290 2023-04-22 15:10:54.000000 guitk-0.3.0/guitk/widgets/types.py
--rw-r--r--   0        0        0     1842 2023-02-17 18:33:45.000000 guitk-0.3.0/guitk/widgets/utils.py
--rw-r--r--   0        0        0     3492 2023-04-23 23:35:05.332899 guitk-0.3.0/guitk/widgets/widget.py
--rw-r--r--   0        0        0    22895 2023-04-23 23:35:05.333911 guitk-0.3.0/guitk/widgets/window.py
--rw-r--r--   0        0        0      590 2023-04-23 23:35:20.854795 guitk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    21327 1970-01-01 00:00:00.000000 guitk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.4.1/LICENSE
+-rw-r--r--   0        0        0     9589 2023-06-05 13:48:02.322455 guitk-0.4.1/README.md
+-rw-r--r--   0        0        0     2820 2023-06-05 13:57:04.928578 guitk-0.4.1/guitk/__init__.py
+-rw-r--r--   0        0        0    12161 2023-06-05 13:44:42.707599 guitk-0.4.1/guitk/__main__.py
+-rw-r--r--   0        0        0     1968 2023-06-05 13:44:42.707839 guitk-0.4.1/guitk/_debug.py
+-rw-r--r--   0        0        0     2430 2023-06-05 13:44:42.708070 guitk-0.4.1/guitk/_on.py
+-rw-r--r--   0        0        0    10707 2023-06-05 13:44:42.708422 guitk-0.4.1/guitk/basewidget.py
+-rw-r--r--   0        0        0      294 2023-06-05 13:44:42.708769 guitk-0.4.1/guitk/constants.py
+-rw-r--r--   0        0        0    24190 2023-06-05 13:44:42.709103 guitk-0.4.1/guitk/containers.py
+-rw-r--r--   0        0        0     1306 2023-06-05 13:44:42.709339 guitk-0.4.1/guitk/debugwindow.py
+-rw-r--r--   0        0        0     2437 2023-06-05 13:44:42.709558 guitk-0.4.1/guitk/events.py
+-rw-r--r--   0        0        0    22563 2023-06-05 13:44:42.709859 guitk-0.4.1/guitk/frame.py
+-rw-r--r--   0        0        0     4723 2023-06-05 13:44:42.710063 guitk-0.4.1/guitk/image.py
+-rw-r--r--   0        0        0     5510 2023-06-05 13:44:42.710655 guitk-0.4.1/guitk/layout.py
+-rw-r--r--   0        0        0     3448 2023-06-05 13:44:42.710932 guitk-0.4.1/guitk/menu.py
+-rw-r--r--   0        0        0     2873 2023-06-05 13:44:42.711259 guitk-0.4.1/guitk/redirect.py
+-rw-r--r--   0        0        0     1618 2023-06-05 13:44:42.711438 guitk-0.4.1/guitk/spacer.py
+-rw-r--r--   0        0        0    11449 2023-06-05 13:44:42.711640 guitk-0.4.1/guitk/tk_text.py
+-rw-r--r--   0        0        0     2523 2023-06-05 13:44:42.712010 guitk-0.4.1/guitk/tkroot.py
+-rw-r--r--   0        0        0     8686 2023-06-05 13:44:42.712276 guitk-0.4.1/guitk/tooltips.py
+-rw-r--r--   0        0        0    13189 2023-06-05 13:44:42.712537 guitk-0.4.1/guitk/ttk_button.py
+-rw-r--r--   0        0        0     5088 2023-06-05 13:44:42.712731 guitk-0.4.1/guitk/ttk_checkbutton.py
+-rw-r--r--   0        0        0     5717 2023-06-05 13:44:42.713001 guitk-0.4.1/guitk/ttk_combobox.py
+-rw-r--r--   0        0        0    10384 2023-06-05 13:44:42.713197 guitk-0.4.1/guitk/ttk_entry.py
+-rw-r--r--   0        0        0     7596 2023-06-05 13:44:42.713434 guitk-0.4.1/guitk/ttk_label.py
+-rw-r--r--   0        0        0     8873 2023-06-05 13:44:42.713652 guitk-0.4.1/guitk/ttk_notebook.py
+-rw-r--r--   0        0        0     8883 2023-06-05 13:44:42.714581 guitk-0.4.1/guitk/ttk_panedwindow.py
+-rw-r--r--   0        0        0     4898 2023-06-05 13:44:42.714718 guitk-0.4.1/guitk/ttk_progressbar.py
+-rw-r--r--   0        0        0     6148 2023-06-05 13:44:42.714850 guitk-0.4.1/guitk/ttk_radiobutton.py
+-rw-r--r--   0        0        0     7161 2023-06-05 13:44:42.714992 guitk-0.4.1/guitk/ttk_scale.py
+-rw-r--r--   0        0        0     2943 2023-06-05 13:44:42.715116 guitk-0.4.1/guitk/ttk_separator.py
+-rw-r--r--   0        0        0     7801 2023-06-05 13:44:42.715319 guitk-0.4.1/guitk/ttk_spinbox.py
+-rw-r--r--   0        0        0    12619 2023-06-05 13:44:42.715472 guitk-0.4.1/guitk/ttk_treeview.py
+-rw-r--r--   0        0        0      771 2023-06-05 13:44:42.715589 guitk-0.4.1/guitk/types.py
+-rw-r--r--   0        0        0     2527 2023-06-05 13:44:42.715787 guitk-0.4.1/guitk/utils.py
+-rw-r--r--   0        0        0     9333 2023-06-05 13:44:42.716003 guitk-0.4.1/guitk/widget.py
+-rw-r--r--   0        0        0    18725 2023-06-05 13:44:42.716457 guitk-0.4.1/guitk/window.py
+-rw-r--r--   0        0        0      769 2023-06-05 13:57:04.928888 guitk-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    10421 1970-01-01 00:00:00.000000 guitk-0.4.1/setup.py
+-rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 guitk-0.4.1/PKG-INFO
```

### Comparing `guitk-0.3.0/LICENSE` & `guitk-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guitk-0.3.0/guitk/redirect.py` & `guitk-0.4.1/guitk/redirect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Redirect stdout/stderr """
 
+from __future__ import annotations
+
 import sys
 
 
 class _StdOutRedirectBaseClass:
-    """Base class for StdOutRedirect and StdErrRedirect """
+    """Base class for StdOutRedirect and StdErrRedirect"""
 
     def __init__(self):
         self._echo = False
         self._listeners = {}
         self._listener_count = 0
         self._redirect = False
 
@@ -68,36 +70,36 @@
         if self.stdout:
             sys.stdout = sys.__stdout__
         if self.stderr:
             sys.stderr = sys.__stderr__
 
 
 class StdOutRedirect(_StdOutRedirectBaseClass):
-    """Singleton class that handles redirect """
+    """Singleton class that handles redirect"""
 
     def __new__(cls, *args, **kwargs):
-        """ create new object or return instance of already created singleton """
+        """create new object or return instance of already created singleton"""
         if not hasattr(cls, "instance") or not cls.instance:
             cls.instance = super().__new__(cls)
 
         return cls.instance
 
     def __init__(self):
         if hasattr(self, "_init"):
             return
         super().__init__()
         self._init = True
         self.stdout = True
 
 
 class StdErrRedirect(_StdOutRedirectBaseClass):
-    """Singleton class that handles redirect """
+    """Singleton class that handles redirect"""
 
     def __new__(cls, *args, **kwargs):
-        """ create new object or return instance of already created singleton """
+        """create new object or return instance of already created singleton"""
         if not hasattr(cls, "instance") or not cls.instance:
             cls.instance = super().__new__(cls)
 
         return cls.instance
 
     def __init__(self):
         if hasattr(self, "_init"):
```

### Comparing `guitk-0.3.0/guitk/tkroot.py` & `guitk-0.4.1/guitk/tkroot.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 from __future__ import annotations
 
 import contextlib
 import tkinter as tk
 from tkinter import ttk
 from typing import TypeVar
 
-# import customtkinter
-
-# customtkinter.set_appearance_mode("System")  # Modes: system (default), light, dark
-# customtkinter.set_default_color_theme("blue")  # Themes: blue (default), dark-blue, green
-
 # create a custom type for type hinting a Window object which is defined later in this module
 Window = TypeVar("Window")
 
 __all__ = ["_TKRoot"]
 
 
 class _TKRoot:
```

### Comparing `guitk-0.3.0/guitk/tooltips.py` & `guitk-0.4.1/guitk/tooltips.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 products or services of Licensee, or any third party.
 
 8. By copying, installing or otherwise using Python, Licensee
 agrees to be bound by the terms and conditions of this License
 Agreement.
 """
 
+from __future__ import annotations
+
 import tkinter as tk
 from tkinter import ttk
 
 
 class _TooltipBase:
     """abstract base class for tooltips"""
 
@@ -225,8 +227,7 @@
             self.tipwindow,
             text=self.text,
             justify=tk.LEFT,
             relief=tk.SOLID,
             borderwidth=1,
         )
         label.pack()
-
```

### Comparing `guitk-0.3.0/guitk/widgets/events.py` & `guitk-0.4.1/guitk/events.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 """Events """
 
 from __future__ import annotations
 
 import tkinter
 from collections import namedtuple
-from typing import Hashable, TypeVar
+from typing import TYPE_CHECKING, Hashable
 
 EventCommand = namedtuple("EventCommand", ["widget", "key", "event_type", "command"])
 
-from enum import Enum, auto
+from enum import Enum
 
-Window = TypeVar("Window")
-Widget = TypeVar("Widget")
+if TYPE_CHECKING:
+    from .basewidget import BaseWidget
+    from .window import Window
 
 
 class Event:
     """Event that occurred and values for widgets in the window"""
 
-    def __init__(self, widget: object, window: Window, key, event_type):
+    def __init__(
+        self, widget: BaseWidget, window: Window, key: Hashable, event_type: EventType
+    ):
         self.id: int = id(window)
-        self.widget: Widget = widget
+        self.widget: BaseWidget = widget
         self.key: Hashable = key
         self.event_type: EventType = event_type
         self.event: tkinter.Event | None = (
             None  # placeholder for Tk event, will be set in _make_callback
         )
 
     def __str__(self):
         return f"id={self.id}, widget={self.widget}, key={self.key}, event_type={self.event_type}, event={self.event}"
 
 
 class EventType(Enum):
     """Constants for event types"""
 
-    BrowseFile = "<<BrowseFile>>"
+    Any = "*"  # special case for binding to all events
     BrowseDirectory = "<<BrowseDirectory>>"
+    BrowseFile = "<<BrowseFile>>"
     ButtonPress = "<<Button>>"
-    Checkbutton = "<<Checkbutton>>"
     CheckButton = "<<Checkbutton>>"
-    ComboboxSelected = "<<ComboboxSelected>>"
+    Checkbutton = "<<Checkbutton>>"
     ComboBoxSelected = "<<ComboboxSelected>>"
-    Radiobutton = "<<Radiobutton>>"
-    RadioButton = "<<Radiobutton>>"
-    VirtualEvent = "<<VirtualEvent>>"
+    ComboboxSelected = "<<ComboboxSelected>>"
+    DeleteWindow = "WM_DELETE_WINDOW"
+    EntryReturn = "<<EntryReturn>>"
+    ImagePress = "<<ImagePress>>"
     KeyRelease = "<KeyRelease>"
     LinkLabel = "<<LinkLabel>>"
-    ListboxSelect = "<<ListboxSelect>>"
     ListBoxSelect = "<<ListboxSelect>>"
+    ListboxSelect = "<<ListboxSelect>>"
+    MenuCommand = "<<MenuCommand>>"
+    NotebookTabChanged = "<<NotebookTabChanged>>"
     OutputWrite = "<<OutputWrite>>"
+    Quit = "WM_DELETE_WINDOW"
+    RadioButton = "<<Radiobutton>>"
+    Radiobutton = "<<Radiobutton>>"
     ScaleUpdate = "<<ScaleUpdate>>"
-    TreeviewHeading = "<<TreeviewHeading>>"
+    Setup = "<<Setup>>"
+    SpinboxDecrement = "<<SpinboxDecrement>>"
+    SpinboxIncrement = "<<SpinboxIncrement>>"
+    SpinboxUpdate = "<<SpinboxUpdate>>"
+    Teardown = "<<Teardown>>"
     TreeViewHeading = "<<TreeviewHeading>>"
-    TreeviewSelect = "<<TreeviewSelect>>"
     TreeViewSelect = "<<TreeviewSelect>>"
-    TreeviewTag = "<<TreeviewTag>>"
     TreeViewTag = "<<TreeviewTag>>"
+    TreeviewHeading = "<<TreeviewHeading>>"
+    TreeviewSelect = "<<TreeviewSelect>>"
+    TreeviewTag = "<<TreeviewTag>>"
+    VirtualEvent = "<<VirtualEvent>>"
     WM_DELETE_WINDOW = "WM_DELETE_WINDOW"
-    DeleteWindow = "WM_DELETE_WINDOW"
-    Quit = "WM_DELETE_WINDOW"
     WindowFinishedLoading = "<<WindowFinishedLoading>>"
-    NotebookTabChanged = "<<NotebookTabChanged>>"
-    MenuCommand = "<<MenuCommand>>"
```

### Comparing `guitk-0.3.0/guitk/widgets/menu.py` & `guitk-0.4.1/guitk/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Menu and Command classes"""
 
+from __future__ import annotations
+
 import tkinter as tk
 from typing import Callable, Optional
 
 from .events import Event, EventType
 
 
 def _map_key_binding_from_shortcut(shortcut):
@@ -20,15 +22,14 @@
         else:
             if len(k) == 1 and ord("A") <= ord(k) <= ord("Z"):
                 k = k.lower()
             keybinding.append(k)
     return "<" + "-".join(keybinding) + ">"
 
 
-
 class Menu:
     def __init__(
         self,
         label: str,
         underline: Optional[bool] = None,
         separator: Optional[bool] = False,
     ) -> None:
@@ -111,8 +112,7 @@
         key_binding = _map_key_binding_from_shortcut(self._shortcut)
         window.window.bind_all(
             key_binding,
             self.window._make_callback(
                 Event(self, self.window, self._key, EventType.MenuCommand)
             ),
         )
-
```

### Comparing `guitk-0.3.0/guitk/widgets/tk_text.py` & `guitk-0.4.1/guitk/tk_text.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from __future__ import annotations
 
 import tkinter as tk
 from typing import Hashable, TypeVar
 
 from guitk.redirect import StdErrRedirect, StdOutRedirect
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TooltipType
+from .types import CommandType, PadType, TooltipType
 from .utils import scrolled_widget_factory
-from .widget import Widget
 
 __all__ = ["Text", "Output"]
 
 
 _valid_standard_attributes = {
     "background",
     "borderwidth",
@@ -54,86 +54,91 @@
     "wrap",
 } | _valid_standard_attributes
 
 
 Window = TypeVar("Window")
 
 
-class Text(Widget):
-    """
-    A tk Text box
-    """
+class Text(BaseWidget):
+    """A tk Text box"""
 
     def __init__(
         self,
         text: str | None = None,
         key: Hashable | None = None,
         width: int = 40,
         height: int = 20,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = False,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         command: CommandType | None = None,
         vscrollbar: bool = False,
         hscrollbar: bool = False,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
         """
         Initialize a Text widget.
 
         Args:
             text (str | None, optional): Default text for the text box. Defaults to None.
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             width (int, optional): Width of the text box. Defaults to 40.
             height (int, optional): Height of the text box. Defaults to 20.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
             vscrollbar (bool, optional): Show vertical scrollbar. Defaults to False.
             hscrollbar (bool, optional): Show horizontal scrollbar. Defaults to False.
+            weightx (int | None, optional): Weight of the widget in the x direction. Defaults to None.
+            weighty (int | None, optional): Weight of the widget in the y direction. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to tk Text.
         """
         super().__init__(
             key=key,
             disabled=disabled,
             rowspan=rowspan,
             columnspan=columnspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
         self.widget_type = "tk.Text"
         self.key = key or "Text"
         self.width = width
         self.height = height
         self._value = text if text is not None else ""
         self.columnspan = columnspan
         self.rowspan = rowspan
         self.vscrollbar = vscrollbar
         self.hscrollbar = hscrollbar
         self.kwargs = kwargs
 
     def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
         kwargs_text = {
             k: v for k, v in self.kwargs.items() if k in _valid_tk_text_attributes
         }
         self.widget = scrolled_widget_factory(
             parent,
             tk.Text,
             vscrollbar=self.vscrollbar,
@@ -160,14 +165,15 @@
                     event_type=EventType.KeyRelease,
                     command=self._command,
                 )
             )
 
         if self._disabled:
             self.widget["state"] = "disabled"
+
         return self.widget
 
     @property
     def value(self):
         return self.widget.get("1.0", tk.END).rstrip()
 
     @value.setter
@@ -179,61 +185,66 @@
     def text(self):
         """Return the Tk text widget"""
         return self.widget
 
 
 # TODO: how to make Output read-only?
 class Output(Text):
-    """
-    Text box that redirects stderr and/or stdout to the text box.
-    """
+    """Text box that redirects stderr and/or stdout to the text box."""
 
     def __init__(
         self,
         text: str | None = None,
         key: Hashable | None = None,
         width: int = 40,
         height: int = 20,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = False,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         vscrollbar: bool = True,
         hscrollbar: bool = False,
         stdout: bool = True,
         stderr: bool = True,
         echo: bool = False,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
         """
         Initialize an Output widget.
 
         Args:
             text (str | None, optional): Default text for the text box. Defaults to None.
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             width (int, optional): Width of the text box. Defaults to 40.
             height (int, optional): Height of the text box. Defaults to 20.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
             vscrollbar (bool, optional): Show vertical scrollbar. Defaults to False.
             hscrollbar (bool, optional): Show horizontal scrollbar. Defaults to False.
             stdout (bool, optional): Redirect stdout to the text box. Defaults to True.
             stderr (bool, optional): Redirect stderr to the text box. Defaults to True.
             echo (bool, optional): Echo stdout and stderr to the console. Defaults to False.
+            weightx (int | None, optional): Weight of the widget in the x direction. Defaults to None.
+            weighty (int | None, optional): Weight of the widget in the y direction. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to tk Text.
         """
         super().__init__(
             text=text,
             key=key,
             width=width,
             height=height,
@@ -243,42 +254,56 @@
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             vscrollbar=vscrollbar,
             hscrollbar=hscrollbar,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
+            **kwargs,
         )
+
+        self.kwargs = kwargs
         self._echo = echo
+        self._stdout = stdout
+        self._stderr = stderr
+
+        # stores state for stdout and stderr redirection
         self._redirect = []
         self._redirect_id = {}
-        if stdout:
-            self._redirect.append(StdOutRedirect())
-        if stderr:
-            self._redirect.append(StdErrRedirect())
-        for r in self._redirect:
-            r.echo = self._echo
-            self._redirect_id[r] = r.register(self._write)
 
     def _create_widget(self, parent, window: "Window", row, col):
-        super()._create_widget(parent, window, row, col)
+        self.widget = super()._create_widget(parent, window, row, col)
 
         # Unbind <KeyRelease> since this isn't for user input
         self.widget.unbind("<KeyRelease>")
 
         if self.events:
             event = Event(self, window, self.key, EventType.OutputWrite)
             self.window.root.bind_all(
                 EventType.OutputWrite.value, window._make_callback(event)
             )
 
+        self._configure_redirect()
         self.enable_redirect()
 
         return self.widget
 
+    def _configure_redirect(self):
+        """Configure stdout and stderr redirection."""
+        if self._stdout:
+            self._redirect.append(StdOutRedirect())
+        if self._stderr:
+            self._redirect.append(StdErrRedirect())
+        for r in self._redirect:
+            r.echo = self._echo
+            self._redirect_id[r] = r.register(self._write)
+
     def _write(self, line):
         self.text.insert(tk.END, line)
         self.text.yview(tk.END)
         self.window.root.event_generate(EventType.OutputWrite.value)
 
     @property
     def echo(self):
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_button.py` & `guitk-0.4.1/guitk/ttk_button.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """ttk Button widgets"""
 
+from __future__ import annotations
+
 import pathlib
+import tkinter as tk
 import tkinter.ttk as ttk
 from tkinter import filedialog
-from typing import Hashable
+from typing import TYPE_CHECKING, Any, Hashable
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TooltipType
-from .widget import Widget
+from .types import CommandType, PadType, TooltipType
+from .utils import load_image
+
+if TYPE_CHECKING:
+    from .window import Window
 
 __all__ = ["Button", "BrowseFileButton", "BrowseDirectoryButton"]
 
 _valid_standard_attributes = {
     "class",
     "compound",
     "cursor",
@@ -36,89 +43,106 @@
     "defaultextension",
     "filetypes",
     "initialfile",
     "title",
 }
 
 
-class Button(Widget):
+class Button(BaseWidget):
     """Basic button"""
 
     def __init__(
         self,
         text: str,
+        image: str | None = None,
         key: Hashable | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType | None = None,
         command: CommandType | None = None,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
         """
         Initialize a Button widget.
 
         Args:
             text (str): Text for the button.
+            image (str | None, optional): Image for the button. Defaults to None.
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
+            weightx (int | None, optional): Weight in x direction. Defaults to None.
+            weighty (int | None, optional): Weight in y direction. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to ttk.Button.
         """
         super().__init__(
             key=key,
             disabled=disabled,
             rowspan=rowspan,
             columnspan=columnspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
-            **kwargs,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
 
         self.widget_type = "ttk.Button"
         self.text = text
+        self.image = image
         self.key = key or text
         self.columnspan = columnspan
         self.rowspan = rowspan
         self.tooltip = tooltip
+        self.padx = padx
+        self.pady = pady
         self.kwargs = kwargs
 
     @property
     def value(self) -> str:
         return self.widget["text"]
 
     @value.setter
     def value(self, text: str):
         self.widget["text"] = text
 
-    def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
+    def _create_widget(self, parent: Any, window: Window, row: int, col: int):
+        """Create the ttk.Button widget"""
         event = Event(self, window, self.key, EventType.ButtonPress)
 
         # build arg list for Button()
         kwargs_button = {
             k: v for k, v in self.kwargs.items() if k in _valid_ttk_button_attributes
         }
 
+        if self.image:
+            self._photoimage = load_image(self.image)
+            kwargs_button["image"] = self._photoimage
+
         self.widget = ttk.Button(
             parent,
             text=self.text,
             command=window._make_callback(event),
             **kwargs_button,
         )
         self._grid(
@@ -144,74 +168,79 @@
     @property
     def button(self):
         """Return the Tk button widget"""
         return self.widget
 
 
 class BrowseFileButton(Button):
-    """
-    Button that opens a file dialog to select a file.
-    """
+    """Button that opens a file dialog to select a file."""
 
     def __init__(
         self,
         text="Browse",
         key: Hashable | None = None,
         target_key: Hashable | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType | None = None,
         filename_only: bool = False,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
-        """
-        Initialize a BrowseFileButton widget.
+        """Initialize a BrowseFileButton widget.
 
         Args:
             text (str): Text for the button.
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             target_key (Hashable, optional): Unique key for the target widget. Defaults to None.
                 If set, the target widget's value is set to the selected filename.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             filename_only (bool, optional): If True, only the filename is returned. Defaults to False.
+            weightx (int | None, optional): Weight in x direction. Defaults to None.
+            weighty (int | None, optional): Weight in y direction. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to ttk.Button or filedialog.askopenfilename as appropriate.
         """
         super().__init__(
             text,
             key=key,
             disabled=disabled,
             columnspan=columnspan,
             rowspan=rowspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
         self.target_key = target_key
         self.widget_type = "guitk.BrowseFileButton"
         self._filename = None
         self._filename_only = filename_only
         self.kwargs = kwargs
 
     def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
         kwargs_button = {
             k: v for k, v in self.kwargs.items() if k in _valid_ttk_button_attributes
         }
         self.widget = ttk.Button(
             parent, text=self.text, command=self.browse_dialog, **kwargs_button
         )
         self._grid(
@@ -230,76 +259,85 @@
         """Open a file dialog to select a file"""
         kwargs_options = {
             k: v for k, v in self.kwargs.items() if k in _valid_askopenfile_options
         }
         self._filename = filedialog.askopenfilename(**kwargs_options)
         if self._filename_only and self._filename:
             # only want the name, not the path
-            self._filename = str(pathlib.Path(self._filename).name)
+            self._filename = pathlib.Path(self._filename).name
         if self.target_key and self._filename:
             self.window[self.target_key].value = self._filename
         event = Event(self, self.window, self.key, EventType.BrowseFile)
         self.window._handle_event(event)
 
 
 class BrowseDirectoryButton(Button):
+    """Button that opens a file dialog to select a directory."""
+
     def __init__(
         self,
         text="Browse",
         key: Hashable | None = None,
         target_key: Hashable | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType | None = None,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
         """
         Initialize a BrowseDirectoryButton widget.
 
         Args:
             text (str): Text for the button.
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             target_key (Hashable, optional): Unique key for the target widget. Defaults to None.
                 If set, the target widget's value is set to the selected directory.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
+            weightx (int | None, optional): Weight in x direction. Defaults to None.
+            weighty (int | None, optional): Weight in y direction. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to ttk.Button or filedialog.askopenfilename as appropriate.
         """
         super().__init__(
             text,
             key=key,
             disabled=disabled,
             columnspan=columnspan,
             rowspan=rowspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
         self.target_key = target_key
         self.widget_type = "guitk.BrowseDirectoryButton"
         self._dirname = None
         self.kwargs = kwargs
 
     def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
         kwargs_button = {
             k: v for k, v in self.kwargs.items() if k in _valid_ttk_button_attributes
         }
         self.widget = ttk.Button(
             parent, text=self.text, command=self.browse_dialog, **kwargs_button
         )
         self._grid(
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_checkbutton.py` & `guitk-0.4.1/guitk/ttk_checkbutton.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """ttk checkbutton widget"""
 
 from __future__ import annotations
 
 import tkinter as tk
 import tkinter.ttk as ttk
-from typing import Hashable
+from typing import TYPE_CHECKING, Hashable
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TooltipType
-from .widget import Widget
+from .types import CommandType, PadType, TooltipType
+
+if TYPE_CHECKING:
+    from .window import Window
 
 __all__ = ["Checkbutton", "CheckButton"]
 
 _valid_standard_attributes = {
     "class",
     "compound",
     "cursor",
@@ -30,47 +33,56 @@
     "command",
     "variable",
     # "offvalue",
     # "onvalue",
 } | _valid_standard_attributes
 
 
-class Checkbutton(Widget):
+class Checkbutton(BaseWidget):
     """Checkbox / checkbutton"""
 
     def __init__(
         self,
         text: str,
-        key=Hashable,
+        key: Hashable | None = None,
+        checked: bool = False,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType | None = None,
         command: CommandType | None = None,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
         """
-        Initialize a Checkbutton widget.
+        Initialize a ttk.Checkbutton widget.
 
         Args:
             text (str): Text for the checkbutton.
             key (Hashable, optional): Unique key for this widget. Defaults to None.
+            checked (bool, optional): Initial state. Defaults to False (not checked).
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
+            weightx (int | None, optional): Weight of widget in X direction. Defaults to None.
+            weighty (int | None, optional): Weight of widget in Y direction. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to ttk.Checkbutton.
 
         Notes:
             Unlike a regular ttk.Checkbutton, the onvalue and offvalue are always True and False.
         """
         super().__init__(
             key=key,
@@ -79,26 +91,28 @@
             columnspan=columnspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
         self.widget_type = "ttk.Checkbutton"
         self.text = text
         self.key = key or text
         self.columnspan = columnspan
         self.rowspan = rowspan
-        self._value = tk.BooleanVar()
+        self._value: tk.BooleanVar = tk.BooleanVar()
+        self._checked = checked
         self.kwargs = kwargs
 
-    def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
+    def _create_widget(self, parent, window: Window, row, col):
         event = Event(self, window, self.key, EventType.Checkbutton)
 
         # build arg list for Checkbutton
         kwargs_checkbutton = {
             k: v
             for k, v in self.kwargs.items()
             if k in _valid_ttk_checkbutton_attributes
@@ -107,15 +121,14 @@
         self.widget = ttk.Checkbutton(
             parent,
             text=self.text,
             anchor=self.kwargs.get("anchor"),
             command=window._make_callback(event),
             variable=self._value,
             onvalue=True,
-            offvalue=False,
             **kwargs_checkbutton,
         )
         self._grid(
             row=row, column=col, rowspan=self.rowspan, columnspan=self.columnspan
         )
 
         if self._command:
@@ -125,14 +138,17 @@
                     widget=self,
                     key=self.key,
                     event_type=EventType.Checkbutton,
                     command=self._command,
                 )
             )
 
+        if self._checked:
+            self.widget.invoke()
+
         if self._disabled:
             self.widget.state(["disabled"])
         return self.widget
 
     @property
     def checkbutton(self):
         """Return the ttk.Checkbutton widget"""
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_entry.py` & `guitk-0.4.1/guitk/ttk_entry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """ttk Entry widget"""
 
 from __future__ import annotations
 
 import tkinter as tk
 import tkinter.ttk as ttk
-from typing import Hashable, TypeVar
+from typing import TYPE_CHECKING, Hashable
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TooltipType
+from .types import CommandType, PadType, TooltipType
 from .utils import scrolled_widget_factory
-from .widget import Widget
+
+if TYPE_CHECKING:
+    from .window import Window
 
 __all__ = ["Entry", "LabelEntry"]
 
 _valid_standard_attributes = {
     "class",
     "cursor",
     "style",
@@ -30,81 +33,82 @@
     "textvariable",
     "validate",
     "validatecommand",
     "width",
 } | _valid_standard_attributes
 
 
-Window = TypeVar("Window")
-
-
-class Entry(Widget):
-    """
-    ttk.Entry text entry / input box
-    """
+class Entry(BaseWidget):
+    """ttk.Entry text entry / input box"""
 
     def __init__(
         self,
         key: Hashable | None = None,
         default: str | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = False,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         command: CommandType | None = None,
         hscrollbar: bool = False,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
-        """
-        Initialize an Entry widget.
+        """Initialize an Entry widget.
 
         Args:
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             default (str | None, optional): Default text for the entry box. Defaults to None.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
             hscrollbar (bool, optional): Show horizontal scrollbar. Defaults to False.
+            weightx (int | None, optional): Weight for horizontal resizing. Defaults to None.
+            weighty (int | None, optional): Weight for vertical resizing. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to ttk.Entry.
         """
         super().__init__(
             key=key,
             disabled=disabled,
             columnspan=columnspan,
             rowspan=rowspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
         self.widget_type = "ttk.Entry"
         default = default or ""
         self._value.set(default)
         self.key = key or "Entry"
         self.columnspan = columnspan
         self.rowspan = rowspan
         self.hscrollbar = hscrollbar
         self.kwargs = kwargs
 
-    def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
+    def _create_widget(self, parent, window: Window, row, col):
         # build arg list for ttk.Entry
         kwargs_entry = {
             k: v for k, v in self.kwargs.items() if k in _valid_ttk_entry_attributes
         }
         self.widget = scrolled_widget_factory(
             parent,
             ttk.Entry,
@@ -112,44 +116,49 @@
             textvariable=self._value,
             **kwargs_entry,
         )
         self._grid(
             row=row, column=col, rowspan=self.rowspan, columnspan=self.columnspan
         )
 
+        # bind key release event
         event = Event(self, window, self.key, EventType.KeyRelease)
         self.widget.bind("<KeyRelease>", window._make_callback(event))
 
+        # bind return key event
+        entry_return_key = Event(self, window, self.key, EventType.EntryReturn)
+        self.widget.bind("<Return>", window._make_callback(entry_return_key))
+
         if self._command:
             self.events = True
             window._bind_command(
                 EventCommand(
                     widget=self,
                     key=self.key,
                     event_type=EventType.KeyRelease,
                     command=self._command,
                 )
             )
 
         if self._disabled:
             self.widget.state(["disabled"])
+
         return self.widget
 
     @property
     def entry(self):
         """Return the Tk entry widget"""
         return self.widget
 
 
 class _ttkLabelEntry(ttk.Entry):
     """ttk.Entry with a Label"""
 
     def __init__(self, master=None, text=None, **kwargs):
-        """
-        Initialize a _ttkLabelEntry widget.
+        """Initialize a _ttkLabelEntry widget.
 
         Args:
             master (tk.Widget, optional): Parent widget. Defaults to None.
             text (str, optional): Label text. Defaults to None.
             **kwargs: Additional keyword arguments are passed to ttk.Entry.
         """
         self.frame = ttk.Frame(master)
@@ -161,60 +170,65 @@
         # Copy geometry methods of self.frame without overriding Entry
         # methods -- hack!
         text_meths = vars(ttk.Entry).keys()
         methods = vars(tk.Pack).keys() | vars(tk.Grid).keys() | vars(tk.Place).keys()
         methods = methods.difference(text_meths)
 
         for m in methods:
-            if m[0] != "_" and m != "config" and m != "configure":
+            if m[0] != "_" and m not in {"config", "configure", "focus"}:
                 setattr(self, m, getattr(self.frame, m))
 
     def __str__(self):
         return str(self.frame)
 
 
 class LabelEntry(Entry):
-    """
-    Text entry / input box with a label
-    """
+    """Text entry / input box with a label"""
+
+    # TODO: add option to put label above the entry box
 
     def __init__(
         self,
         text: str,
         key: Hashable | None = None,
         default: str | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = False,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         command: CommandType | None = None,
         hscrollbar: bool = False,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
-        """
-        Initialize an Entry widget.
+        """Initialize an Entry widget.
 
         Args:
             text (str): Label text.
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             default (str | None, optional): Default text for the entry box. Defaults to None.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
             hscrollbar (bool, optional): Show horizontal scrollbar. Defaults to False.
+            weightx (int | None, optional): Weight for horizontal resizing. Defaults to None.
+            weighty (int | None, optional): Weight for vertical resizing. Defaults to None.
+            focus (bool, optional): If True, widget will have focus. Defaults to False. Only one widget can have focus.
             **kwargs: Additional keyword arguments are passed to ttk.Entry.
         """
         super().__init__(
             key=key,
             default=default,
             disabled=disabled,
             columnspan=columnspan,
@@ -222,49 +236,55 @@
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
             hscrollbar=hscrollbar,
+            focus=focus,
+            weightx=weightx,
+            weighty=weighty,
         )
         self.widget_type = "guitk.LabelEntry"
         self.text = text
         self.kwargs = kwargs
 
     def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
         # build arg list for Entry
         kwargs_entry = {
             k: v for k, v in self.kwargs.items() if k in _valid_ttk_entry_attributes
         }
         self.widget = _ttkLabelEntry(
             parent, text=self.text, textvariable=self._value, **kwargs_entry
         )
         self._grid(
             row=row, column=col, rowspan=self.rowspan, columnspan=self.columnspan
         )
 
+        # bind key release event
         event = Event(self, window, self.key, EventType.KeyRelease)
         self.widget.bind("<KeyRelease>", window._make_callback(event))
 
+        # bind return key event
+        entry_return_key = Event(self, window, self.key, EventType.EntryReturn)
+        self.widget.bind("<Return>", window._make_callback(entry_return_key))
+
         if self._command:
             self.events = True
             window._bind_command(
                 EventCommand(
                     widget=self,
                     key=self.key,
                     event_type=EventType.KeyRelease,
                     command=self._command,
                 )
             )
 
         if self._disabled:
             self.widget.state(["disabled"])
+
         return self.widget
 
     @property
     def entry(self):
         """Return the Tk entry widget"""
         return self.widget
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_label.py` & `guitk-0.4.1/guitk/ttk_label.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """ttk.Label widget"""
 
 from __future__ import annotations
 
 import sys
 import tkinter.ttk as ttk
 from tkinter import font
-from typing import Hashable, TypeVar
+from typing import TYPE_CHECKING, Hashable
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TooltipType
-from .widget import Widget
+from .types import CommandType, PadType, TooltipType, Window
+from .utils import load_image
 
-__all__ = ["Label", "LinkLabel"]
+if TYPE_CHECKING:
+    from .window import Window
+
+__all__ = ["Label", "LinkLabel", "Linklabel"]
 
 _valid_standard_attributes = {
     "class",
     "compound",
     "cursor",
     "image",
     "style",
@@ -35,78 +39,86 @@
     "padding",
     "relief",
     "text",
     "wraplength",
 } | _valid_standard_attributes
 
 
-Window = TypeVar("Window")
-
-
-class Label(Widget):
-    """
-    ttk.Label widget
-    """
+class Label(BaseWidget):
+    """ttk.Label widget"""
 
     def __init__(
         self,
         text: str,
+        image: str | None = None,
         key: Hashable | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = False,
         sticky: str | None = None,
         tooltip: TooltipType = None,
+        weightx: int | None = None,
+        weighty: int | None = None,
         **kwargs,
     ):
         """
         Initialize a Label widget.
 
         Args:
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             text (str): Text to display in the label.
+            image: (str, optional): Path to image to display in the label. Defaults to None.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
+            weightx (int | None, optional): Weight of this widget in the horizontal direction. Defaults to None.
+            weighty (int | None, optional): Weight of this widget in the vertical direction. Defaults to None.
             **kwargs: Additional keyword arguments are passed to ttk.Entry.
         """
         super().__init__(
             key=key,
             disabled=disabled,
             rowspan=rowspan,
             columnspan=columnspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
+            weightx=weightx,
+            weighty=weighty,
         )
         self.widget_type = "ttk.Label"
         self.text = text
         self.key = key or text
         self.columnspan = columnspan
         self.rowspan = rowspan
+        self.image = image
         self.kwargs = kwargs
 
-    def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
+    def _create_widget(self, parent, window: Window, row, col):
+        """Create the ttk.Label widget"""
 
         # Arg list for ttk.Label
         kwargs_label = {
             k: v for k, v in self.kwargs.items() if k in _valid_ttk_label_attributes
         }
+
+        if self.image:
+            self._photoimage = load_image(self.image)
+            kwargs_label["image"] = self._photoimage
+
         self.widget = ttk.Label(
             parent,
             text=self.text,
             **kwargs_label,
         )
         self.widget["textvariable"] = self._value
         self._value.set(self.text)
@@ -129,39 +141,40 @@
     def __init__(
         self,
         text: str,
         key: Hashable | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType = None,
-        underline_font: bool = False,
         command: CommandType | None = None,
+        weightx: int | None = None,
+        weighty: int | None = None,
         **kwargs,
     ):
-        """
-        Initialize a LinkLabel widget.
+        """Initialize a LinkLabel widget.
 
         Args:
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             text (str): Text to display in the label.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to True.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
-            underline_font (bool, optional): If True, underline the font. Defaults to False.
             command (CommandType | None, optional): Command to execute when clicked. Defaults to None.
+            weightx (int | None, optional): Weight of this widget in the horizontal direction. Defaults to None.
+            weighty (int | None, optional): Weight of this widget in the vertical direction. Defaults to None.
             **kwargs: Additional keyword arguments are passed to ttk.Entry.
         """
         self.cursor = (
             kwargs.get("cursor") or "pointinghand"
             if sys.platform == "darwin"
             else "hand2"
         )
@@ -173,44 +186,43 @@
             columnspan=columnspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             cursor=self.cursor,
+            weightx=weightx,
+            weighty=weighty,
         )
         self.widget_type = "guitk.LinkLabel"
         self.text = text
         self.key = key or text
         self.columnspan = columnspan
         self.rowspan = rowspan
-        self.underline_font = underline_font
         self._command = command
         self.kwargs = kwargs
 
     def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
         self.widget = super()._create_widget(parent, window, row, col)
 
         event = Event(self, window, self.key, EventType.LinkLabel)
         self.widget.bind("<Button-1>", window._make_callback(event))
 
         self.widget.configure(cursor=self.cursor)
 
-        if self.underline_font:
-            f = font.Font(self.widget, self.widget.cget("font"))
-            f.configure(underline=True)
-            self.widget.configure(font=f)
-
         if self._command:
             self.events = True
             window._bind_command(
                 EventCommand(
                     widget=self,
                     key=self.key,
                     event_type=EventType.LinkLabel,
                     command=self._command,
                 )
             )
         return self.widget
+
+
+class Linklabel(LinkLabel):
+    """Non-camel case version"""
+
+    pass
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_notebook.py` & `guitk-0.4.1/guitk/ttk_combobox.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,161 +1,170 @@
-""" ttk Notebook widget """
+"""ttk Combobox widget"""
 
 from __future__ import annotations
 
 import tkinter.ttk as ttk
-from typing import Hashable, TypeVar
+from typing import TYPE_CHECKING, Hashable
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TabType, TooltipType
-from .widget import Widget
-from .window import Frame, LayoutMixin
+from .types import CommandType, PadType, TooltipType
 
-__all__ = ["Notebook", "NoteBook"]
+if TYPE_CHECKING:
+    from .window import Window
+
+__all__ = ["Combobox", "ComboBox"]
 
 _valid_standard_attributes = {
-    "width",
-    "height",
-    "padding",
-    "takefocus",
+    "class",
     "cursor",
     "style",
-    "class",
+    "takefocus",
 }
 
-_valid_ttk_notebook_attributes = _valid_standard_attributes
-
-
-Window = TypeVar("Window")
+_valid_ttk_combobox_attributes = {
+    "exportselection",
+    "height",
+    "justify",
+    "postcommand",
+    "state",
+    "textvariable",
+    "values",
+    "width",
+} | _valid_standard_attributes
 
 
-class Notebook(Widget, LayoutMixin):
-    """
-    ttk.Notebook widget
-    """
+class Combobox(BaseWidget):
+    """ttk Combobox"""
 
     def __init__(
         self,
         key: Hashable | None = None,
-        tabs: TabType | None = None,
+        default: str | None = None,
+        values: list[str] | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
-        events: bool = False,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
+        events: bool = True,
         sticky: str | None = None,
-        tooltip: TooltipType = None,
+        tooltip: TooltipType | None = None,
         command: CommandType | None = None,
+        readonly: bool = False,
+        autosize: bool = False,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
-        """
-        Initialize a Notebook widget.
-
-        Args:
-            key (Hashable, optional): Unique key for this widget. Defaults to None.
-            tabs: (TabType, optional): Tabs to add to the notebook. Defaults to None.
-            disabled (bool, optional): If True, widget is disabled. Defaults to False.
-            columnspan (int | None, optional): Number of columns to span. Defaults to None.
-            rowspan (int | None, optional): Number of rows to span. Defaults to None.
-            padx (int | None, optional): X padding. Defaults to None.
-            pady (int | None, optional): Y padding. Defaults to None.
-            events (bool, optional): Enable events for this widget. Defaults to False.
-            sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
-            tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
-            command (CommandType | None, optional): Command to execute when clicked. Defaults to None.
-            **kwargs: Additional keyword arguments are passed to ttk.Entry.
-        """
         super().__init__(
             key=key,
             disabled=disabled,
-            rowspan=rowspan,
             columnspan=columnspan,
+            rowspan=rowspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
-        self.widget_type = "ttk.Notebook"
-        self.key = key or "Notebook"
+        """
+        Initialize a ttk.Combobox widget.
+
+        Args:
+            key (Hashable, optional): Unique key for this widget. Defaults to None.
+            default (str, optional): Default value. Defaults to None.
+            values (list[str], optional): List of values for the combobox. Defaults to None.
+            disabled (bool, optional): If True, widget is disabled. Defaults to False.
+            columnspan (int | None, optional): Number of columns to span. Defaults to None.
+            rowspan (int | None, optional): Number of rows to span. Defaults to None.
+            padx (PadType | None, optional): X padding. Defaults to None.
+            pady (PadType | None, optional): Y padding. Defaults to None.
+            events (bool, optional): Enable events for this widget. Defaults to False.
+            sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
+            tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
+            command (CommandType | None, optional): Command callback. Defaults to None.
+            readonly (bool, optional): If True, widget is read-only. Defaults to False.
+                If Combobox is not readonly, user can type in a value that is not in the list of values.
+            autosize (bool, optional): If True, automatically set width to fit longest value. Defaults to False.
+            weightx (int | None, optional): Weight of widget in X direction. Defaults to None.
+            weighty (int | None, optional): Weight of widget in Y direction. Defaults to None.
+            focus (bool, optional): If True, widget has focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
+            **kwargs: Additional keyword arguments are passed to ttk.Checkbutton.
+        """
+        self.widget_type = "ttk.Combobox"
+        self.key = key or "Combobox"
         self.columnspan = columnspan
         self.rowspan = rowspan
-        self.tabs = tabs
-        self._command = command
+        self._readonly = readonly
+        self._autosize = autosize
         self.kwargs = kwargs
+        self.values = values
+        self.default = default
 
-    def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
-        # Arg list for ttk.Label
-        kwargs_notebook = {
-            k: v for k, v in self.kwargs.items() if k in _valid_ttk_notebook_attributes
+    def _create_widget(self, parent, window: Window, row, col):
+        # build arg list for Combobox
+        kwargs = {
+            k: v for k, v in self.kwargs.items() if k in _valid_ttk_combobox_attributes
         }
 
-        self.widget = ttk.Notebook(parent, **kwargs_notebook)
+        if self._autosize:
+            # automatically set width, override any width value provided
+            width = len(max(self.values, key=len))
+            kwargs["width"] = width + 1
+
+        self.widget = ttk.Combobox(
+            parent,
+            textvariable=self._value,
+            values=self.values,
+            **kwargs,
+        )
         self._grid(
             row=row, column=col, rowspan=self.rowspan, columnspan=self.columnspan
         )
 
-        event_tab_change = Event(
-            self.widget, window, self.key, EventType.NotebookTabChanged
-        )
-        self.widget.bind(
-            "<<NotebookTabChanged>>", window._make_callback(event_tab_change)
-        )
+        event_release = Event(self.widget, window, self.key, EventType.KeyRelease)
+        self.widget.bind("<KeyRelease>", window._make_callback(event_release))
 
-        if self.tabs:
-            for tab in self.tabs:
-                self.add(tab, self.tabs[tab])
+        event_selected = Event(
+            self.widget, window, self.key, EventType.ComboboxSelected
+        )
+        self.widget.bind("<<ComboboxSelected>>", window._make_callback(event_selected))
 
         if self._command:
             self.events = True
             window._bind_command(
-                # the actual widget will be a tk widget in form widget=.!toplevel.!frame.!notebook, so it won't match self.widget
-                # so set widget=None or _handle_commands won't correctly handle the command
                 EventCommand(
-                    widget=None,
+                    widget=self,
                     key=self.key,
-                    event_type=EventType.NotebookTabChanged,
+                    event_type=EventType.ComboboxSelected,
                     command=self._command,
                 )
             )
 
+        if self.default is not None:
+            self.value = self.default
+
         if self._disabled:
             self.widget.state(["disabled"])
 
-        return self.widget
+        if self._readonly:
+            self.widget.state(["readonly"])
 
-    @property
-    def current_tab(self):
-        """Return the name of the currently selected tab"""
-        return self.notebook.tab(self.notebook.select(), "text")
-
-    def add(self, text, layout, **kwargs):
-        """Add a layout to the Notebook as new tab"""
-        frame = Frame(layout=layout)
-        frame_ = frame._create_widget(self.widget, self.window, 0, 0)
-        kwargs["text"] = text
-        self.notebook.add(frame_, **kwargs)
-
-    def insert(self, pos, text, layout, **kwargs):
-        """Insert a layout to the Notebook as new tab at position pos"""
-        frame = Frame(layout=layout)
-        frame_ = frame._create_widget(self.widget, self.window, 0, 0)
-        kwargs["text"] = text
-        self.notebook.insert(pos, frame_, **kwargs)
+        return self.widget
 
     @property
-    def notebook(self):
-        """Return the ttk.Notebook widget"""
+    def combobox(self):
+        """Return the Tk combobox widget"""
         return self.widget
 
 
-class NoteBook(Notebook):
-    """
-    ttk.Notebook widget
-    """
+class ComboBox(Combobox):
+    """ttk Combobox"""
 
     pass
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_progressbar.py` & `guitk-0.4.1/guitk/ttk_progressbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """ ttk Progressbar widget """
 
 from __future__ import annotations
 
 import tkinter as tk
 import tkinter.ttk as ttk
-from typing import Hashable, TypeVar
+from typing import TYPE_CHECKING, Hashable, TypeVar
+
+from .basewidget import BaseWidget
+from .types import PadType, TooltipType
+
+if TYPE_CHECKING:
+    from .window import Window
 
-from .types import TooltipType
-from .widget import Widget
 
 __all__ = [
     "Progressbar",
     "ProgressBar",
     "PROGRESS_DETERMINATE",
     "PROGRESS_INDETERMINATE",
 ]
@@ -31,35 +35,35 @@
 
 Window = TypeVar("Window")
 
 PROGRESS_DETERMINATE = "determinate"
 PROGRESS_INDETERMINATE = "indeterminate"
 
 
-class Progressbar(Widget):
-    """
-    ttk.Progressbar
-    """
+class Progressbar(BaseWidget):
+    """ttk.Progressbar"""
 
     def __init__(
         self,
         key: Hashable | None = None,
         value: float | None = None,
         orient: str = tk.HORIZONTAL,
         length: int = 200,
         mode: str = "determinate",
         maximum: float = 100.0,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         events: bool = True,
+        weightx: int | None = None,
+        weighty: int | None = None,
         **kwargs,
     ):
         """Initialize a ttk.Progressbar widget
 
         Args:
             key (Hashable, optional): Key for the widget. Defaults to None.
             value (float, optional): Initial value. Defaults to None.
@@ -71,14 +75,16 @@
             columnspan (int, optional): Number of columns to span. Defaults to None.
             rowspan (int, optional): Number of rows to span. Defaults to None.
             padx (int, optional): Padding in x direction. Defaults to None.
             pady (int, optional): Padding in y direction. Defaults to None.
             sticky (str, optional): Sticky direction. Defaults to None.
             tooltip (TooltipType, optional): Tooltip for the widget. Defaults to None.
             events (bool, optional): Enable events for this widget. Defaults to True.
+            weightx (int, optional): Weight in x direction. Defaults to None.
+            weighty (int, optional): Weight in y direction. Defaults to None.
             **kwargs: Additional keyword arguments to pass to ttk.Progressbar.
         """
         super().__init__(
             key=key,
             disabled=disabled,
             rowspan=rowspan,
             columnspan=columnspan,
@@ -108,17 +114,14 @@
         return self.widget["value"]
 
     @value.setter
     def value(self, value):
         self._value.set(float(value))
 
     def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
         # Arg list for ttk.ProgressBar
         kwargs_progressbar = {
             k: v
             for k, v in self.kwargs.items()
             if k in _valid_ttk_progressbar_attributes
         }
         kwargs_progressbar["variable"] = self._value
@@ -145,12 +148,10 @@
         return self.widget
 
     def stop(self):
         self.widget.stop()
 
 
 class ProgressBar(Progressbar):
-    """
-    ttk.Progressbar
-    """
+    """ttk.Progressbar"""
 
     pass
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_radiobutton.py` & `guitk-0.4.1/guitk/ttk_radiobutton.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """ ttk Radiobutton widget """
 
 from __future__ import annotations
 
 import tkinter as tk
 import tkinter.ttk as ttk
-from typing import Any, Union, Hashable, TypeVar
+from typing import TYPE_CHECKING, Any, Hashable, TypeVar, Union
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TooltipType
-from .widget import Widget
+from .types import CommandType, PadType, TooltipType
+
+if TYPE_CHECKING:
+    from .window import Window
 
 __all__ = ["Radiobutton", "RadioButton"]
 
 _valid_standard_attributes = {
     "class",
     "compound",
     "cursor",
@@ -26,36 +29,40 @@
 }
 
 _valid_ttk_radiobutton_attributes = _valid_standard_attributes
 
 
 Window = TypeVar("Window")
 
+# TODO: need a better way to get radio button value
+# only way now is the key but you really only need one key for the group to get the value
+
 
-class Radiobutton(Widget):
-    """
-    ttk.Radiobutton class
-    """
+class Radiobutton(BaseWidget):
+    """ttk.Radiobutton class"""
 
     def __init__(
         self,
         text: str,
         group: Hashable,
         key: Hashable | None = None,
         value: Union[int, str, None] = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         selected: bool = False,
         command: CommandType | None = None,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs: Any,
     ):
         """Initialize a ttk.Radiobutton widget
 
         Args:
             text (str): Text to display
             group (Hashable): Group name (must be unique and will be used as key unless a separate key is specified)
@@ -67,43 +74,47 @@
             padx (int, optional): Padding in x direction. Defaults to None.
             pady (int, optional): Padding in y direction. Defaults to None.
             events (bool, optional): Whether to enable events. Defaults to True.
             sticky (str, optional): Sticky direction. Defaults to None.
             tooltip (TooltipType, optional): Tooltip text. Defaults to None.
             selected (bool, optional): Whether to select this widget. Defaults to False.
             command (CommandType, optional): Command to execute when selected. Defaults to None.
+            weightx (int, optional): Weight in x direction. Defaults to None.
+            weighty (int, optional): Weight in y direction. Defaults to None.
+            focus (bool, optional): If True, widget will have focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to ttk.Radiobutton.
         """
         super().__init__(
             key=key,
             disabled=disabled,
             rowspan=rowspan,
             columnspan=columnspan,
             padx=padx,
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
         )
         self.widget_type = "ttk.Radiobutton"
         self.text = text
         self.group = group
         self.key = key or group
         self._radiobutton_value = value if value is not None else text
         self._value = None  # will be set in _create_widget
         self.columnspan = columnspan
         self.rowspan = rowspan
         self.selected = selected
         self.kwargs = kwargs
 
     def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
         # assign control variable or create it if necessary
         if self.group not in self.window._radiobuttons:
             # determine type of control variable based on value
             var_type = type(self._radiobutton_value)
             if var_type == int:
                 self.window._radiobuttons[self.group] = tk.IntVar(
                     value=self._radiobutton_value
@@ -162,12 +173,10 @@
     @property
     def radiobutton(self):
         """Return the ttk Radiobutton widget"""
         return self.widget
 
 
 class RadioButton(Radiobutton):
-    """
-    ttk.Radiobutton class
-    """
+    """ttk.Radiobutton class"""
 
     pass
```

### Comparing `guitk-0.3.0/guitk/widgets/ttk_treeview.py` & `guitk-0.4.1/guitk/ttk_treeview.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """ ttk Treeview and Listbox widgets """
 
 
 from __future__ import annotations
 
-import tkinter as tk
 import tkinter.ttk as ttk
-from typing import Hashable, TypeVar
+from typing import TYPE_CHECKING, Hashable
 
+from .basewidget import BaseWidget
 from .events import Event, EventCommand, EventType
-from .types import CommandType, TooltipType
+from .types import CommandType, PadType, TooltipType
 from .utils import scrolled_widget_factory
-from .widget import Widget
+
+if TYPE_CHECKING:
+    from .window import Window
 
 __all__ = ["ListBox", "Listbox", "TreeView", "Treeview"]
 
 _valid_standard_attributes = {
     "class",
     "cursor",
     "displaycolumns",
@@ -26,54 +28,40 @@
     "xscrollcommand",
     "yscrollcommand",
 }
 
 _valid_ttk_treeview_attributes = _valid_standard_attributes
 
 
-Window = TypeVar("Window")
-
-
-class Treeview(Widget):
-    """
-    ttk.Treeview widget
-    """
+class Treeview(BaseWidget):
+    """ttk.Treeview widget"""
 
     def __init__(
         self,
         headings: list[str],
         key: Hashable | None = None,
         columns: list[str] | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         command: CommandType | None = None,
         hscrollbar: bool = False,
         vscrollbar: bool = False,
+        weightx: int | None = None,
+        weighty: int | None = None,
+        focus: bool = False,
         **kwargs,
     ):
-        super().__init__(
-            key=key,
-            disabled=disabled,
-            rowspan=rowspan,
-            columnspan=columnspan,
-            padx=padx,
-            pady=pady,
-            events=events,
-            sticky=sticky,
-            tooltip=tooltip,
-            command=command,
-        )
         """Initialize a ttk.Treeview widget
-        
+
         Args:
             headings (list[str]): List of column headings, required.
             key (Hashable, optional): Key to use for this widget. Defaults to None.
             columns (list[str], optional): List of column names. Defaults to None.
             disabled (bool, optional): Whether the widget is disabled. Defaults to False.
             columnspan (int, optional): Number of columns to span. Defaults to None.
             rowspan (int, optional): Number of rows to span. Defaults to None.
@@ -81,16 +69,35 @@
             pady (int, optional): Padding in y direction. Defaults to None.
             events (bool, optional): Whether to bind events. Defaults to True.
             sticky (str, optional): Sticky direction. Defaults to None.
             tooltip (TooltipType, optional): Tooltip to display. Defaults to None.
             command (CommandType, optional): Command to run when selection changes. Defaults to None.
             hscrollbar (bool, optional): Whether to display a horizontal scrollbar. Defaults to False.
             vscrollbar (bool, optional): Whether to display a vertical scrollbar. Defaults to False.
+            weightx (int, optional): Horizontal weight. Defaults to None.
+            weighty (int, optional): Vertical weight. Defaults to None.
+            focus (bool, optional): If True, widget will have focus. Defaults to False.
+                Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments to pass to ttk.Treeview.
         """
+        super().__init__(
+            key=key,
+            disabled=disabled,
+            rowspan=rowspan,
+            columnspan=columnspan,
+            padx=padx,
+            pady=pady,
+            events=events,
+            sticky=sticky,
+            tooltip=tooltip,
+            command=command,
+            weightx=weightx,
+            weighty=weighty,
+            focus=focus,
+        )
         self.key = key or "Treeview"
         self.widget_type = "ttk.Treeview"
 
         if headings and columns and len(headings) != len(columns):
             raise ValueError("headings and columns lists must be the same length")
 
         self._headings = headings
@@ -104,18 +111,15 @@
         self.events = events
         self.sticky = sticky or ""
         self.tooltip = tooltip
         self.vscrollbar = vscrollbar
         self.hscrollbar = hscrollbar
         self.kwargs = kwargs
 
-    def _create_widget(self, parent, window: "Window", row, col):
-        self.window = window
-        self._parent = parent
-
+    def _create_widget(self, parent, window: Window, row, col):
         # build arg list for Treeview()
         kwargs_treeview = {
             k: v
             for k, v in self.kwargs.items()
             if k in _valid_ttk_treeview_attributes and v is not None
         }
         if "show" not in kwargs_treeview:
@@ -204,34 +208,34 @@
     @property
     def tree(self):
         """Return the ttk Treeview widget"""
         return self.widget
 
 
 class Listbox(Treeview):
-    """
-    Listbox widget
-    """
+    """Listbox widget (which is a Treeview widget with only one column)"""
 
     def __init__(
         self,
         text: list[str] | None = None,
         key: Hashable | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
-        padx: int | None = None,
-        pady: int | None = None,
+        padx: PadType | None = None,
+        pady: PadType | None = None,
         events: bool = True,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         command: CommandType | None = None,
         hscrollbar: bool = False,
         vscrollbar: bool = False,
         width: int = 200,
+        weightx: int | None = None,
+        weighty: int | None = None,
         **kwargs,
     ):
         """Create a Listbox widget
 
         Args:
             text (list[str], optional): List of strings to display in the listbox. Defaults to None.
             key (Hashable, optional): The key used to access the widget's value. Defaults to None.
@@ -243,15 +247,21 @@
             events (bool, optional): Enable events. Defaults to True.
             sticky (str, optional): Sticky setting for the grid. Defaults to None.
             tooltip (TooltipType, optional): A tooltip to show when the mouse is over the widget. Defaults to None.
             command (CommandType, optional): A command to execute when the widget is clicked. Defaults to None.
             hscrollbar (bool, optional): Show a horizontal scrollbar. Defaults to False.
             vscrollbar (bool, optional): Show a vertical scrollbar. Defaults to False.
             width (int, optional): Width of the widget in pixels. Defaults to 200.
+            weightx (int, optional): Horizontal weight. Defaults to None.
+            weighty (int, optional): Vertical weight. Defaults to None.
             **kwargs: Additional keyword arguments to pass to the widget constructor.
+
+        Note:
+            This Listbox widget is actually implemented as a Treeview widget with only one column.
+            This is because Tk does not offer a themed ttk Listbox widget.
         """
         self.key = key or "Listbox"
         self.widget_type = "guitk.Listbox"
 
         if text and type(text) != list:
             raise ValueError("text must be a list of strings")
         self._text = text
@@ -269,18 +279,20 @@
             pady=pady,
             events=events,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
             hscrollbar=hscrollbar,
             vscrollbar=vscrollbar,
+            weightx=weightx,
+            weighty=weighty,
             **kwargs,
         )
 
-    def _create_widget(self, parent, window: "Window", row, col):
+    def _create_widget(self, parent, window: Window, row, col):
         """Create the widget"""
 
         # build arg list for Treeview()
         kwargs_treeview = {
             k: v
             for k, v in self.kwargs.items()
             if k in _valid_ttk_treeview_attributes and v is not None
@@ -319,14 +331,16 @@
                     widget=self,
                     key=self.key,
                     event_type=EventType.ListboxSelect,
                     command=self._command,
                 )
             )
 
+        return self.widget
+
     def insert(self, index, line):
         """Insert a line into Listbox"""
         self.widget.insert("", index, iid=line, values=(line))
 
     def append(self, line):
         """Append a line to end of Listbox"""
         self.widget.insert("", "end", iid=line, values=(line))
```

### Comparing `guitk-0.3.0/pyproject.toml` & `guitk-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guitk"
-version = "0.3.0"
+version = "0.4.1"
 description = "Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python."
 authors = ["Rhet Turnbull <rturnbull+git@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,11 +12,22 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.0.13"
 mkdocstrings-python = "^0.8.3"
 bump2version = "^1.0.1"
 markdownpp = "^1.5.1"
+ruff = "^0.0.265"
+mypy = "^1.3.0"
+pytest-cov = "^4.1.0"
+pillow = "^9.5.0"
+
+[tool.ruff]
+target-version = "py39"
+line-length = 125
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+python_classes = false
```

