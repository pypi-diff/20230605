# Comparing `tmp/tldraw-0.1.0.tar.gz` & `tmp/tldraw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldraw-0.1.0.tar", max compression
+gzip compressed data, was "tldraw-0.1.1.tar", max compression
```

## Comparing `tldraw-0.1.0.tar` & `tldraw-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-04-24 08:16:11.663668 tldraw-0.1.0/LICENSE
--rw-r--r--   0        0        0      879 2023-06-02 20:48:23.730846 tldraw-0.1.0/README.md
--rw-r--r--   0        0        0      571 2023-06-02 20:43:23.128962 tldraw-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-02 20:40:28.237924 tldraw-0.1.0/tldraw/__init__.py
--rw-r--r--   0        0        0      320 2023-05-15 18:18:52.187379 tldraw-0.1.0/tldraw/comp.tsx
--rw-r--r--   0        0        0      245 2023-05-20 16:51:27.378161 tldraw-0.1.0/tldraw/tldraw.py
--rw-r--r--   0        0        0     2006 2023-06-02 20:48:24.934888 tldraw-0.1.0/tldraw/tldraw_matplotlib.py
--rw-r--r--   0        0        0     1183 2023-06-02 14:17:44.885169 tldraw-0.1.0/tldraw/tldraw_matplotlib_component.tsx
--rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 tldraw-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-24 08:16:11.663668 tldraw-0.1.1/LICENSE
+-rw-r--r--   0        0        0      928 2023-06-05 10:26:27.640799 tldraw-0.1.1/README.md
+-rw-r--r--   0        0        0      571 2023-06-05 10:27:18.744845 tldraw-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-02 20:40:28.237924 tldraw-0.1.1/tldraw/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-15 18:18:52.187379 tldraw-0.1.1/tldraw/comp.tsx
+-rw-r--r--   0        0        0      245 2023-05-20 16:51:27.378161 tldraw-0.1.1/tldraw/tldraw.py
+-rw-r--r--   0        0        0     2226 2023-06-03 16:39:39.741537 tldraw-0.1.1/tldraw/tldraw_matplotlib.py
+-rw-r--r--   0        0        0     1183 2023-06-02 14:17:44.885169 tldraw-0.1.1/tldraw/tldraw_matplotlib_component.tsx
+-rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 tldraw-0.1.1/PKG-INFO
```

### Comparing `tldraw-0.1.0/LICENSE` & `tldraw-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tldraw-0.1.0/README.md` & `tldraw-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 jupyterlab   (or alternative VS Code Jupyter Lab)
 ```
 
 
 
 # Changelog
 
+## 0.1.1
+
+* add update_plot in TldrawMatplotlib
+
 ## 0.1.0
 
 * Added TldrawMatplotlib
 
 ## 0.0.3
 
 * refactor readme
```

### Comparing `tldraw-0.1.0/pyproject.toml` & `tldraw-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tldraw"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tldraw fo Jupyter"
 authors = ["kolibril13 <44469195+kolibril13@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.14"
```

### Comparing `tldraw-0.1.0/tldraw/tldraw_matplotlib.py` & `tldraw-0.1.1/tldraw/tldraw_matplotlib.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from traitlets import Unicode, Int
 import io
 import base64
 from pathlib import Path
 
 
 class TldrawMatplotlib(ipyreact.ReactWidget):
+
+    def update_plot(self,fig):
+        self.base64img = TldrawMatplotlib.figure_to_base64(fig)
+
+
     @staticmethod
     def figure_to_base64(my_figure):
         buf = io.BytesIO()
         my_figure.savefig(buf, format="png")
 
         buf.seek(0)
         base64_img_string_only = base64.b64encode(buf.getvalue()).decode()
@@ -34,14 +39,15 @@
         # extract image width and height from the IHDR chunk
         image_width = int.from_bytes(ihdr_chunk[8:12], byteorder="big")
         image_height = int.from_bytes(ihdr_chunk[12:16], byteorder="big")
 
         return image_width, image_height
 
     def __init__(self, my_figure=None, **kwargs):
+        # print("Info: All drawings are deleted when the notebook is reloaded, saving the overlay is not supported yet.")
         if my_figure is None:
             "Plase provide a figure"
 
         base64_img_string = TldrawMatplotlib.figure_to_base64(my_figure)
         image_width, image_height = TldrawMatplotlib.base64_to_image_dimensions(
             base64_img_string
         )
```

### Comparing `tldraw-0.1.0/tldraw/tldraw_matplotlib_component.tsx` & `tldraw-0.1.1/tldraw/tldraw_matplotlib_component.tsx`

 * *Files identical despite different names*

### Comparing `tldraw-0.1.0/PKG-INFO` & `tldraw-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldraw
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tldraw fo Jupyter
 License: MIT
 Author: kolibril13
 Author-email: 44469195+kolibril13@users.noreply.github.com
 Requires-Python: >=3.8,<3.14
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,18 @@
 jupyterlab   (or alternative VS Code Jupyter Lab)
 ```
 
 
 
 # Changelog
 
+## 0.1.1
+
+* add update_plot in TldrawMatplotlib
+
 ## 0.1.0
 
 * Added TldrawMatplotlib
 
 ## 0.0.3
 
 * refactor readme
```

