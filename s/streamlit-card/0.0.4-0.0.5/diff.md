# Comparing `tmp/streamlit-card-0.0.4.tar.gz` & `tmp/streamlit-card-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-card-0.0.4.tar", last modified: Tue Nov 22 12:00:38 2022, max compression
+gzip compressed data, was "streamlit-card-0.0.5.tar", last modified: Mon Jun  5 13:10:15 2023, max compression
```

## Comparing `streamlit-card-0.0.4.tar` & `streamlit-card-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 12:00:38.936958 streamlit-card-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2022-11-22 11:59:31.000000 streamlit-card-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2022-11-22 11:59:31.000000 streamlit-card-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      891 2022-11-22 12:00:38.936958 streamlit-card-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      460 2022-11-22 11:59:31.000000 streamlit-card-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 12:00:38.936958 streamlit-card-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      889 2022-11-22 11:59:31.000000 streamlit-card-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 12:00:38.928958 streamlit-card-0.0.4/streamlit_card/
--rw-r--r--   0 runner    (1001) docker     (122)     1187 2022-11-22 11:59:31.000000 streamlit-card-0.0.4/streamlit_card/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 12:00:38.928958 streamlit-card-0.0.4/streamlit_card/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 12:00:38.932958 streamlit-card-0.0.4/streamlit_card/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (122)      586 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)   197459 2022-11-22 12:00:02.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   646432 2022-11-22 12:00:02.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      406 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/precache-manifest.49f3f4093ba9c781031e7c22b0736831.js
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 12:00:38.928958 streamlit-card-0.0.4/streamlit_card/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 12:00:38.936958 streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)   497991 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (122)  2065691 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (122)     2297 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (122)     5540 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js
--rw-r--r--   0 runner    (1001) docker     (122)     7997 2022-11-22 12:00:24.000000 streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 12:00:38.928958 streamlit-card-0.0.4/streamlit_card.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      891 2022-11-22 12:00:38.000000 streamlit-card-0.0.4/streamlit_card.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      965 2022-11-22 12:00:38.000000 streamlit-card-0.0.4/streamlit_card.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 12:00:38.000000 streamlit-card-0.0.4/streamlit_card.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-22 12:00:38.000000 streamlit-card-0.0.4/streamlit_card.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-22 12:00:38.000000 streamlit-card-0.0.4/streamlit_card.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:10:15.220914 streamlit-card-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-05 13:09:05.000000 streamlit-card-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 13:09:05.000000 streamlit-card-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-05 13:10:15.220914 streamlit-card-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 13:09:05.000000 streamlit-card-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:10:15.220914 streamlit-card-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-05 13:09:05.000000 streamlit-card-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:10:15.212913 streamlit-card-0.0.5/streamlit_card/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-05 13:09:05.000000 streamlit-card-0.0.5/streamlit_card/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:10:15.212913 streamlit-card-0.0.5/streamlit_card/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:10:15.216913 streamlit-card-0.0.5/streamlit_card/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-06-05 13:09:35.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   646432 2023-06-05 13:09:35.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/precache-manifest.49f3f4093ba9c781031e7c22b0736831.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:10:15.212913 streamlit-card-0.0.5/streamlit_card/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:10:15.220914 streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   497991 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2065691 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-05 13:09:56.000000 streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:10:15.216913 streamlit-card-0.0.5/streamlit_card.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-05 13:10:15.000000 streamlit-card-0.0.5/streamlit_card.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-05 13:10:15.000000 streamlit-card-0.0.5/streamlit_card.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:10:15.000000 streamlit-card-0.0.5/streamlit_card.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 13:10:15.000000 streamlit-card-0.0.5/streamlit_card.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 13:10:15.000000 streamlit-card-0.0.5/streamlit_card.egg-info/top_level.txt
```

### Comparing `streamlit-card-0.0.4/LICENSE` & `streamlit-card-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/setup.py` & `streamlit-card-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 
 setuptools.setup(
     name="streamlit-card",
-    version="0.0.4",
+    version="0.0.5",
     author="gamcoh",
     author_email="cohengamliel8@gmail.com",
     description="A streamlit component, to make UI cards",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/gamcoh/st-card",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-card-0.0.4/streamlit_card/__init__.py` & `streamlit-card-0.0.5/streamlit_card/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional
+from typing import Optional, Callable, Any
 
 import streamlit.components.v1 as components
 
 _RELEASE = True
 COMPONENT_NAME = "streamlit_card"
 
 if _RELEASE:  # use the build instead of development if release is true
@@ -18,21 +18,28 @@
 
 
 def card(
     title: str,
     text: str,
     image: Optional[str] = None,
     url: Optional[str] = None,
+    on_click: Callable[[Any], Any] = None,
     key: Optional[str] = None,
 ) -> bool:
     """Creates a UI card like component.
 
     Args:
         title (str): The title of the card.
         text (str): The text of the card.
         image (str, optional): An optional background image. Defaults to None.
         url (str, optional): An optional url to open when the card is clicked. Defaults to None.
+        on_click (Callable, optional): An optional function callback that
+                                   will fire when clicked.
+                                   Can only work if the url is None.
         key (str, optional): An optional key for the component. Defaults to None.
     """
-    return _streamlit_card(
+    clicked = _streamlit_card(
         title=title, text=text, image=image, url=url, key=key, default=False
     )
+    if clicked:
+        on_click()
+    return clicked
```

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/asset-manifest.json` & `streamlit-card-0.0.5/streamlit_card/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/bootstrap.min.css` & `streamlit-card-0.0.5/streamlit_card/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/bootstrap.min.css.map` & `streamlit-card-0.0.5/streamlit_card/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/index.html` & `streamlit-card-0.0.5/streamlit_card/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/service-worker.js` & `streamlit-card-0.0.5/streamlit_card/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js` & `streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js.map` & `streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/2.921ed9e7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js` & `streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js.map` & `streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/main.d3689c9d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js` & `streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map` & `streamlit-card-0.0.5/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.4/streamlit_card.egg-info/SOURCES.txt` & `streamlit-card-0.0.5/streamlit_card.egg-info/SOURCES.txt`

 * *Files identical despite different names*

