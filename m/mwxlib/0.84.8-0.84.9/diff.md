# Comparing `tmp/mwxlib-0.84.8-py3-none-any.whl.zip` & `tmp/mwxlib-0.84.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 162132 bytes, number of entries: 22
+Zip file size: 162167 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-03 17:04 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43499 b- defN 23-Jun-03 17:04 mwx/controls.py
--rw-rw-rw-  2.0 fat    73816 b- defN 23-Jun-04 13:38 mwx/framework.py
--rw-rw-rw-  2.0 fat    68561 b- defN 23-Jun-04 13:38 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73816 b- defN 23-Jun-05 06:58 mwx/framework.py
+-rw-rw-rw-  2.0 fat    68716 b- defN 23-Jun-05 06:02 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-Jun-03 17:04 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-Jun-03 17:04 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27598 b- defN 23-Jun-03 17:04 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   138759 b- defN 23-Jun-03 17:04 mwx/nutshell.py
--rw-rw-rw-  2.0 fat    37431 b- defN 23-Jun-03 17:04 mwx/utilus.py
+-rw-rw-rw-  2.0 fat   138759 b- defN 23-Jun-05 06:58 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat    37431 b- defN 23-Jun-05 06:58 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-Jun-03 17:04 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-Jun-03 17:04 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-Jun-03 17:04 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-Jun-03 17:04 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Jun-03 17:04 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/RECORD
-22 files, 614451 bytes uncompressed, 159630 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/RECORD
+22 files, 614606 bytes uncompressed, 159665 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.84.8.dist-info/LICENSE
+Filename: mwxlib-0.84.9.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.84.8.dist-info/METADATA
+Filename: mwxlib-0.84.9.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.84.8.dist-info/WHEEL
+Filename: mwxlib-0.84.9.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.84.8.dist-info/top_level.txt
+Filename: mwxlib-0.84.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.84.8.dist-info/RECORD
+Filename: mwxlib-0.84.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.84.8"
+__version__ = "0.84.9"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
```

## mwx/graphman.py

```diff
@@ -347,19 +347,18 @@
                     self.thread.active = 0
                     self.thread.Stop()
                 del self.Arts
             v.Skip()
         self.Bind(wx.EVT_WINDOW_DESTROY, destroy)
         
         def on_show(v):
-            if self.category: # -> notebook
-                if v.IsShown():
-                    self.handler('page_shown', self)
-                else:
-                    self.handler('page_hidden', self)
+            if v.IsShown():
+                self.handler('page_shown', self)
+            elif self and isinstance(self.Parent, aui.AuiNotebook):
+                self.handler('page_hidden', self) # -> notebook
             v.Skip()
         self.Bind(wx.EVT_SHOW, on_show)
         
         try:
             self.Init()
             if session:
                 self.load_session(session)
@@ -847,37 +846,38 @@
         ## Set the graph and output window sizes to half & half.
         if name == "output" or name is self.output:
             w, h = self.graph.GetClientSize()
             pane.best_size = (w//2, h) # ドッキング時に再計算される
         
         ## Force Layer windows to show.
         if interactive:
-            ## [M-menu] Reload plugin (ret: None if succeeded).
-            if wx.GetKeyState(wx.WXK_ALT):
+            ## [M-S-menu] Reload plugin
+            if wx.GetKeyState(wx.WXK_ALT) and wx.GetKeyState(wx.WXK_SHIFT):
                 self.reload_plug(name)
                 pane = self.get_pane(name)
                 show = True
             
             ## [S-menu] Reset floating position of a stray window.
             if wx.GetKeyState(wx.WXK_SHIFT):
                 pane.floating_pos = wx.GetMousePosition()
                 pane.Float()
                 show = True
         
-        plug = self.get_plug(name) # -> None if pane.window is Graph
+        plug = self.get_plug(name) # -> None if pane.window is a Graph
         win = pane.window # -> Window (plug / notebook / Graph)
         if show:
             if isinstance(win, aui.AuiNotebook):
                 j = win.GetPageIndex(plug)
                 if j != win.Selection:
                     win.Selection = j # the focus is moved => [page_shown]
                 else:
                     plug.handler('page_shown', plug)
             elif not pane.IsShown():
-                win.handler('page_shown', win)
+                if not plug or win.Parent is not self: # otherwise Layer.on_show
+                    win.handler('page_shown', win)
         else:
             if isinstance(win, aui.AuiNotebook):
                 for plug in win.all_pages: # => [page_closed] to all pages
                     plug.handler('page_closed', plug)
             elif pane.IsShown():
                 win.handler('page_closed', win)
         
@@ -1266,14 +1266,15 @@
     def reload_plug(self, name):
         plug = self.get_plug(name)
         if not plug:
             return
         if plug.reloadable:
             session = {}
             try:
+                print("Reloading {}...".format(plug))
                 plug.save_session(session)
             except Exception:
                 traceback.print_exc()
                 print("- Failed to save session: {}".format(plug))
             return self.load_plug(plug.__module__, force=1, session=session)
         return False
```

## Comparing `mwxlib-0.84.8.dist-info/LICENSE` & `mwxlib-0.84.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.84.8.dist-info/METADATA` & `mwxlib-0.84.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.84.8
+Version: 0.84.9
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.84.8.dist-info/RECORD` & `mwxlib-0.84.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=pD1IjgkwdvD-ebntnAH-6Jo7KY5hDq30Ne6rTE_i9fE,43499
-mwx/framework.py,sha256=FREzT3tMg6wXLvVmJhRMEuc8KHLH655JT0Zoxtc5a3E,73816
-mwx/graphman.py,sha256=rDOYa3IZVp48hD0bio7fCwIG0-dNWjdZHm1cvfINszY,68561
+mwx/framework.py,sha256=axKlqwJG6pi5x6q0-dUtegNtDzBDWqow9QGasGt3vXM,73816
+mwx/graphman.py,sha256=iF1cSVYdQHiu1Wylt1cBGIzbQtZQLSetRN3qw_g6-jA,68716
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=vVlBulRQDyYonI9EKfqp-3SpNbGyIJQ6ldkw6bZlalo,27598
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
 mwx/nutshell.py,sha256=ajJBsC9o_21DuYuw5mwRGpB4GgwWT2rOjlf-DS-ntLI,138759
 mwx/utilus.py,sha256=ADA8I7qg339TJOvbrWWD91jqICWfc5C-ENFE-a7YBvU,37431
 mwx/wxmon.py,sha256=hEXto7dD5JunPf-iv2hhcwTIILLkNPlcl6wRt20_Wqc,11343
 mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=UG361QTUheO_hlSIRgkprrGUYh0IzHB8ZqOoJeeMzUs,7424
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.84.8.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.84.8.dist-info/METADATA,sha256=xZ7328VNHvIs8oA83rx-zd5jDLlh6jTIQfGO6kg3NkI,1893
-mwxlib-0.84.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.84.8.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.84.8.dist-info/RECORD,,
+mwxlib-0.84.9.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.84.9.dist-info/METADATA,sha256=Nt7X4C4jS8_safBBRGm2ZcZzk3WEo5B9-czJj-3UIfU,1893
+mwxlib-0.84.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.84.9.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.84.9.dist-info/RECORD,,
```

