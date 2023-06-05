# Comparing `tmp/animegifs-0.6.1.tar.gz` & `tmp/animegifs-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.6.1.tar", last modified: Sun Jun  4 19:12:57 2023, max compression
+gzip compressed data, was "animegifs-0.6.2.tar", last modified: Mon Jun  5 17:35:12 2023, max compression
```

## Comparing `animegifs-0.6.1.tar` & `animegifs-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.537700 animegifs-0.6.1/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     2050 2023-06-04 19:12:57.537700 animegifs-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-06-04 19:10:24.000000 animegifs-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.518699 animegifs-0.6.1/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.1/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-06-04 19:10:24.000000 animegifs-0.6.1/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.535701 animegifs-0.6.1/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.1/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     1586 2023-06-01 16:01:08.000000 animegifs-0.6.1/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     1568 2023-06-04 19:10:24.000000 animegifs-0.6.1/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.526701 animegifs-0.6.1/animegifs.egg-info/
--rw-rw-rw-   0        0        0     2050 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 19:12:57.538699 animegifs-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-04 19:10:24.000000 animegifs-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.933744 animegifs-0.6.2/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     3270 2023-06-05 17:35:12.933744 animegifs-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2463 2023-06-05 17:30:38.000000 animegifs-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.913743 animegifs-0.6.2/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.2/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3388 2023-06-05 16:14:15.000000 animegifs-0.6.2/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.931744 animegifs-0.6.2/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.2/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     2319 2023-06-05 17:31:41.000000 animegifs-0.6.2/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     2010 2023-06-05 17:23:15.000000 animegifs-0.6.2/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.922743 animegifs-0.6.2/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     3270 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:35:12.934744 animegifs-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2023-06-05 17:26:13.000000 animegifs-0.6.2/setup.py
```

### Comparing `animegifs-0.6.1/LICENSE` & `animegifs-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.1/animegifs/animegifs.py` & `animegifs-0.6.2/animegifs/animegifs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
-from animegifs.distutils import gifs, errors
 from mal import Anime
+from animegifs.distutils import gifs, errors
 
 class Animegifs:
 
     def __init__(self):
         self.category = None
 
     def get_gif(self, category: str) -> str:
@@ -20,15 +20,15 @@
                 sorry, spank, stare, tease, threat, tickle, tired, wave, yawn.
 
         Returns:
             gif: gif (url) -> str
         """
         if type(category) is int:
             raise errors.CategoryIntegral(category)
-        elif category.lower() in gifs.gifs_name_list:
+        if category.lower() in gifs.gifs_name_list:
             if category.lower() == 'random':
                 gif_list = []
                 for key, gif_url in gifs.access().items():
                     for urls in gif_url:
                         gif_list.append(urls[0])
                 gif = gif_list
             else:
@@ -53,16 +53,16 @@
         """
         for key, gif_url in gifs.access().items():
             for gif_name in gif_url:
                 if gif_name[0] == gif:
                     result = gif_name[1]
                     try:
                         mal = f"https://myanimelist.net/anime/{int(result)}/"
-                    except ValueError:
-                        raise errors.MethodNotUpdated(gif)
+                    except ValueError as exc:
+                        raise errors.MethodNotUpdated(gif) from exc
                     return mal
             else:
                 continue
 
     def get_malId(self, gif) -> int:
         """
         Return the myanimelist ID of the gif's anime.
```

### Comparing `animegifs-0.6.1/animegifs/distutils/errors.py` & `animegifs-0.6.2/animegifs/distutils/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -38,7 +38,29 @@
     Usually means is just in work in progress and will be available soon.
     """
 
     def __init__(self, gif, error="Method not yet available for this gif."):
         self.gif = gif
         self.error = error
         super().__init__(self.error)
+
+class AuthTimeout(Exception):
+    """
+    Authentication request timed out. Probably status 504 on server side. Check your connection too.
+    """
+
+    def __init__(self, exc, error="Authentication request timed out."):
+        self.exc = exc
+        self.error = error
+        super().__init__(self.error)
+
+class AuthError(Exception):
+    """
+    Authentication request returned an error. Probably status error 4xx.
+    It will be resolved soon, if it persist,
+    issue an issue on https://github.com/MarcoSa-2000/animegifs/issues.
+    """
+
+    def __init__(self, exc, error="Authentication request returned an error."):
+        self.exc = exc
+        self.error = error
+        super().__init__(self.error)
```

### Comparing `animegifs-0.6.1/animegifs/distutils/gifs.py` & `animegifs-0.6.2/animegifs/distutils/gifs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import requests
 import jwt
+from animegifs.distutils import errors
 
 global TOKEN
 TOKEN = None
 gifs_name_list = ["attack",
                   "bite", 'bloodsuck', 'blush', 'bonk', 'brofist',
                   'cry', 'cuddle',
                   'dance', 'disgust',
@@ -20,16 +21,26 @@
                   'random', 'run',
                   'sad', 'scared', 'shoot', 'shrug', 'sip', 'slap', 'smirk', 'sorry', 'spank', 'stare',
                   'tease', 'threat', 'tickle', 'tired',
                   'wave',
                   'yawn']
 
 def authentication():
-    response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1")
-    auth_key = response.json()['key']
+    try:
+        response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1", timeout=10)
+    except requests.exceptions.Timeout:
+        try:
+            response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1", timeout=25)
+        except requests.exceptions.Timeout as exc:
+            raise errors.AuthTimeout(exc)
+    if response.status_code == 200:
+        auth_key = response.json()['key']
+    else:
+        exc = response.status_code
+        raise errors.AuthError(exc)
     return auth_key
 
 def access():
     global TOKEN
     if TOKEN:
         data = jwt.decode(TOKEN, "enkidu-key", algorithms="HS512")
         data = list(data.keys())
```

### Comparing `animegifs-0.6.1/setup.py` & `animegifs-0.6.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.6.1'
+VERSION = '0.6.2'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
@@ -25,12 +25,15 @@
     install_requires=[
        'requests==2.28.2,<=2.29.0',
        'mal-api==0.5.3',
        'PyJWT>=2.4.0,<=2.7.0'
     ],
     python_requires='>=3.8',
     classifiers=[
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows"],
     keywords=['anime', 'gif', 'python', 'anime-gif', 'discord'],
 )
```

