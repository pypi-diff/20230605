# Comparing `tmp/tksheet-6.2.0.tar.gz` & `tmp/tksheet-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.2.0.tar", last modified: Mon May 29 11:30:32 2023, max compression
+gzip compressed data, was "tksheet-6.2.1.tar", last modified: Mon Jun  5 17:39:49 2023, max compression
```

## Comparing `tksheet-6.2.0.tar` & `tksheet-6.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 11:30:32.240130 tksheet-6.2.0/
--rw-rw-rw-   0        0        0     1101 2023-05-28 17:19:38.000000 tksheet-6.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-05-29 11:30:32.240130 tksheet-6.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-28 17:19:38.000000 tksheet-6.2.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-29 11:30:32.240130 tksheet-6.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-28 17:20:16.000000 tksheet-6.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:30:32.240130 tksheet-6.2.0/tksheet/
--rw-rw-rw-   0        0        0     1901 2023-05-28 17:19:38.000000 tksheet-6.2.0/tksheet/__init__.py
--rw-rw-rw-   0        0        0   164380 2023-05-29 09:52:00.000000 tksheet-6.2.0/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   111722 2023-05-28 17:19:38.000000 tksheet-6.2.0/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8844 2023-05-29 11:00:01.000000 tksheet-6.2.0/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   333219 2023-05-29 09:49:54.000000 tksheet-6.2.0/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12695 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   108646 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5746 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:30:32.240130 tksheet-6.2.0/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 17:39:49.065009 tksheet-6.2.1/
+-rw-rw-rw-   0        0        0     1101 2023-06-05 17:22:27.000000 tksheet-6.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-06-05 17:39:49.066009 tksheet-6.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-06-05 17:22:27.000000 tksheet-6.2.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-05 17:39:49.069520 tksheet-6.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-06-05 17:26:19.000000 tksheet-6.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:39:49.060003 tksheet-6.2.1/tksheet/
+-rw-rw-rw-   0        0        0     1901 2023-06-05 17:22:27.000000 tksheet-6.2.1/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   164453 2023-06-05 17:33:41.000000 tksheet-6.2.1/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   111843 2023-06-05 17:28:15.000000 tksheet-6.2.1/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8880 2023-06-05 17:28:19.000000 tksheet-6.2.1/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   333260 2023-06-05 17:29:44.000000 tksheet-6.2.1/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12733 2023-06-05 17:28:30.000000 tksheet-6.2.1/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   108771 2023-06-05 17:28:35.000000 tksheet-6.2.1/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5784 2023-06-05 17:28:39.000000 tksheet-6.2.1/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    60025 2023-06-05 17:28:46.000000 tksheet-6.2.1/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:39:49.065009 tksheet-6.2.1/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.2.0/LICENSE.txt` & `tksheet-6.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.0/PKG-INFO` & `tksheet-6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.2.0
+Version: 6.2.1
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.2.0.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.1.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.2.0/README.md` & `tksheet-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.0/setup.py` & `tksheet-6.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.2.0',
+  version = '6.2.1',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.2.0.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.2.1.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.2.0/tksheet/__init__.py` & `tksheet-6.2.1/tksheet/__init__.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.0/tksheet/_tksheet.py` & `tksheet-6.2.1/tksheet/_tksheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import tkinter as tk
 from collections import deque
 from itertools import accumulate, chain, islice
 from tkinter import ttk
 import bisect
 from typing import Union, Callable, List, Set, Tuple
 
@@ -2734,16 +2736,16 @@
             old_total = self.MT.total_data_cols()
         if isinstance(columns, int):
             if columns < 1:
                 raise ValueError(f"columns arg must be greater than 0, not {columns}")
             total_rows = self.MT.total_data_rows()
             start = old_total if idx == "end" else idx
             data = [
-                self.MT.get_empty_row_seq(rn, end=start + columns, start=start, c_ops=idx == "end")
-                for rn in range(total_rows)
+                [self.MT.get_value_for_empty_cell(datarn, datacn, c_ops=idx == "end") for datarn in range(total_rows)]
+                for datacn in range(start, start + columns)
             ]
             numcols = columns
         else:
             data = columns
             numcols = len(columns)
         if self.MT.all_columns_displayed:
             if mod_column_positions:
```

### Comparing `tksheet-6.2.0/tksheet/_tksheet_column_headers.py` & `tksheet-6.2.1/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pickle
 import tkinter as tk
 import zlib
 from collections import defaultdict
 from itertools import accumulate, chain, cycle, islice
 from math import ceil, floor
 
@@ -1890,14 +1892,15 @@
                 self.set_col_width_run_binding(c, width=new_width, only_set_if_too_small=False)
                 kwargs = self.get_cell_kwargs(datacn, key="dropdown")
                 if kwargs:
                     self.itemconfig(kwargs["canvas_id"], width=new_width)
                     kwargs["window"].update_idletasks()
                     kwargs["window"]._reselect()
                 self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False, redraw_table=True)
+                self.coords(self.text_editor_id, self.MT.col_positions[c] + 1, 0)
 
     # displayed indexes
     def text_editor_newline_binding(self, r=0, c=0, event=None, check_lines=True):
         if self.height_resizing_enabled:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             curr_height = self.text_editor.winfo_height()
             if (
```

### Comparing `tksheet-6.2.0/tksheet/_tksheet_formatters.py` & `tksheet-6.2.1/tksheet/_tksheet_formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, Union, Dict
 
 from ._tksheet_vars import (
     falsy,
     nonelike,
     truthy,
 )
```

### Comparing `tksheet-6.2.0/tksheet/_tksheet_main_table.py` & `tksheet-6.2.1/tksheet/_tksheet_main_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import bisect
 import csv as csv
 import io
 import pickle
 import tkinter as tk
 import zlib
 from collections import defaultdict, deque
@@ -4108,27 +4110,31 @@
         self.parentframe.emit_event("<<SheetModified>>")
 
     def del_cols_rc(self, event=None, c=None):
         seld_cols = sorted(self.get_selected_cols())
         curr = self.currently_selected()
         if not seld_cols or not curr:
             return
-        if self.CH.popup_menu_loc is None or self.CH.popup_menu_loc < seld_cols[0] or self.CH.popup_menu_loc > seld_cols[-1]:
+        if (
+            self.CH.popup_menu_loc is None
+            or self.CH.popup_menu_loc < seld_cols[0]
+            or self.CH.popup_menu_loc > seld_cols[-1]
+        ):
             c = seld_cols[0]
         else:
             c = self.CH.popup_menu_loc
         seld_cols = get_seq_without_gaps_at_index(seld_cols, c)
         self.deselect("all", redraw=False)
         self.create_selected(
-                        0,
-                        seld_cols[0],
-                        len(self.row_positions) - 1,
-                        seld_cols[-1] + 1,
-                        "columns",
-                    )
+            0,
+            seld_cols[0],
+            len(self.row_positions) - 1,
+            seld_cols[-1] + 1,
+            "columns",
+        )
         self.set_currently_selected(0, seld_cols[0], type_="column")
         seldmax = seld_cols[-1] if self.all_columns_displayed else self.displayed_columns[seld_cols[-1]]
         if self.extra_begin_del_cols_rc_func is not None:
             try:
                 self.extra_begin_del_cols_rc_func(DeleteRowColumnEvent("begin_delete_columns", seld_cols))
             except Exception:
                 return
@@ -4196,27 +4202,31 @@
         self.parentframe.emit_event("<<SheetModified>>")
 
     def del_rows_rc(self, event=None, r=None):
         seld_rows = sorted(self.get_selected_rows())
         curr = self.currently_selected()
         if not seld_rows or not curr:
             return
-        if self.RI.popup_menu_loc is None or self.RI.popup_menu_loc < seld_rows[0] or self.RI.popup_menu_loc > seld_rows[-1]:
+        if (
+            self.RI.popup_menu_loc is None
+            or self.RI.popup_menu_loc < seld_rows[0]
+            or self.RI.popup_menu_loc > seld_rows[-1]
+        ):
             r = seld_rows[0]
         else:
             r = self.RI.popup_menu_loc
         seld_rows = get_seq_without_gaps_at_index(seld_rows, r)
         self.deselect("all", redraw=False)
         self.create_selected(
-                        seld_rows[0],
-                        0,
-                        seld_rows[-1] + 1,
-                        len(self.col_positions) - 1,
-                        "rows",
-                    )
+            seld_rows[0],
+            0,
+            seld_rows[-1] + 1,
+            len(self.col_positions) - 1,
+            "rows",
+        )
         self.set_currently_selected(seld_rows[0], 0, type_="row")
         seldmax = seld_rows[-1] if self.all_rows_displayed else self.displayed_rows[seld_rows[-1]]
         if self.extra_begin_del_rows_rc_func is not None:
             try:
                 self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
             except Exception:
                 return
@@ -4782,15 +4792,20 @@
                 else:
                     self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill=fill, outline=outline, tag=tag, smooth=True)
             self.disp_checkbox[t] = True
 
-    def main_table_redraw_grid_and_text(self, redraw_header=False, redraw_row_index=False, redraw_table=True,):
+    def main_table_redraw_grid_and_text(
+        self,
+        redraw_header=False,
+        redraw_row_index=False,
+        redraw_table=True,
+    ):
         try:
             can_width = self.winfo_width()
             can_height = self.winfo_height()
         except Exception:
             return False
         row_pos_exists = self.row_positions != [0] and self.row_positions
         col_pos_exists = self.col_positions != [0] and self.col_positions
```

### Comparing `tksheet-6.2.0/tksheet/_tksheet_other_classes.py` & `tksheet-6.2.1/tksheet/_tksheet_other_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import bisect
 import tkinter as tk
 from collections import namedtuple
 from itertools import islice
 
 from ._tksheet_vars import (
     ctrl_key,
```

### Comparing `tksheet-6.2.0/tksheet/_tksheet_row_index.py` & `tksheet-6.2.1/tksheet/_tksheet_row_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pickle
 import tkinter as tk
 import zlib
 from collections import defaultdict
 from itertools import accumulate, chain, cycle, islice
 from math import ceil, floor
 
@@ -1828,14 +1830,15 @@
                 space_bot = self.MT.get_space_bot(r)
                 if new_height > space_bot:
                     new_height = space_bot
                 if new_height != curr_height:
                     self.set_row_height(datarn, new_height)
                     self.MT.refresh()
                     self.text_editor.config(height=new_height)
+                    self.coords(self.text_editor_id, 0, self.MT.row_positions[r] + 1)
                     kwargs = self.get_cell_kwargs(datarn, key="dropdown")
                     if kwargs:
                         text_editor_h = self.text_editor.winfo_height()
                         win_h, anchor = self.get_dropdown_height_anchor(datarn, text_editor_h)
                         if anchor == "nw":
                             self.coords(
                                 kwargs["canvas_id"],
```

### Comparing `tksheet-6.2.0/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.2.1/tksheet/_tksheet_top_left_rectangle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import tkinter as tk
 
 from ._tksheet_vars import (
     rc_binding,
 )
```

### Comparing `tksheet-6.2.0/tksheet/_tksheet_vars.py` & `tksheet-6.2.1/tksheet/_tksheet_vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 # for mac bindings
 from platform import system as get_os
 
 USER_OS = f"{get_os()}".lower()
 ctrl_key = "Command" if USER_OS == "darwin" else "Control"
 rc_binding = "<2>" if USER_OS == "darwin" else "<3>"
 symbols_set = set("""!#\$%&'()*+,-./:;"@[]^_`{|}~>?= """)
```

### Comparing `tksheet-6.2.0/tksheet.egg-info/PKG-INFO` & `tksheet-6.2.1/tksheet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.2.0
+Version: 6.2.1
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.2.0.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.1.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

