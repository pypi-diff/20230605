# Comparing `tmp/mkdocs-thumbnails-0.0.7.tar.gz` & `tmp/mkdocs-thumbnails-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-thumbnails-0.0.7.tar", last modified: Wed May 26 16:29:51 2021, max compression
+gzip compressed data, was "mkdocs-thumbnails-0.0.9.tar", last modified: Tue Jun  1 21:12:59 2021, max compression
```

## Comparing `mkdocs-thumbnails-0.0.7.tar` & `mkdocs-thumbnails-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-05-26 16:29:51.409603 mkdocs-thumbnails-0.0.7/
--rw-rw-rw-   0        0        0     1057 2021-04-19 16:13:15.000000 mkdocs-thumbnails-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2855 2021-05-26 16:29:51.410603 mkdocs-thumbnails-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2155 2021-04-20 19:41:53.000000 mkdocs-thumbnails-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2021-04-19 16:15:53.000000 mkdocs-thumbnails-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      913 2021-05-26 16:29:51.419603 mkdocs-thumbnails-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      125 2021-04-19 16:26:19.000000 mkdocs-thumbnails-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-26 16:29:51.347602 mkdocs-thumbnails-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2021-05-26 16:29:51.405603 mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/
--rw-rw-rw-   0        0        0     2855 2021-05-26 16:29:51.000000 mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2021-05-26 16:29:51.000000 mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-26 16:29:51.000000 mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2021-05-26 16:29:51.000000 mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2021-05-26 16:29:51.000000 mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-05-26 16:29:51.000000 mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-05-26 16:29:51.408603 mkdocs-thumbnails-0.0.7/src/thumbnails/
--rw-rw-rw-   0        0        0        0 2021-04-17 17:08:28.000000 mkdocs-thumbnails-0.0.7/src/thumbnails/__init__.py
--rw-rw-rw-   0        0        0     3657 2021-05-26 16:24:48.000000 mkdocs-thumbnails-0.0.7/src/thumbnails/plugin.py
--rw-rw-rw-   0        0        0     1380 2021-04-28 13:55:18.000000 mkdocs-thumbnails-0.0.7/src/thumbnails/thumbnail.py
+drwxrwxrwx   0        0        0        0 2021-06-01 21:12:59.048097 mkdocs-thumbnails-0.0.9/
+-rw-rw-rw-   0        0        0     1057 2021-04-19 16:13:15.000000 mkdocs-thumbnails-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2872 2021-06-01 21:12:59.048097 mkdocs-thumbnails-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2021-05-26 17:00:02.000000 mkdocs-thumbnails-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-04-19 16:15:53.000000 mkdocs-thumbnails-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      930 2021-06-01 21:12:59.057096 mkdocs-thumbnails-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      125 2021-04-19 16:26:19.000000 mkdocs-thumbnails-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-01 21:12:58.988098 mkdocs-thumbnails-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-06-01 21:12:59.043097 mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/
+-rw-rw-rw-   0        0        0     2872 2021-06-01 21:12:58.000000 mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2021-06-01 21:12:58.000000 mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-01 21:12:58.000000 mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2021-06-01 21:12:58.000000 mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2021-06-01 21:12:58.000000 mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2021-06-01 21:12:58.000000 mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-06-01 21:12:59.047096 mkdocs-thumbnails-0.0.9/src/thumbnails/
+-rw-rw-rw-   0        0        0        0 2021-04-17 17:08:28.000000 mkdocs-thumbnails-0.0.9/src/thumbnails/__init__.py
+-rw-rw-rw-   0        0        0     3904 2021-06-01 20:08:51.000000 mkdocs-thumbnails-0.0.9/src/thumbnails/plugin.py
+-rw-rw-rw-   0        0        0     2274 2021-06-01 20:36:08.000000 mkdocs-thumbnails-0.0.9/src/thumbnails/thumbnail.py
```

### Comparing `mkdocs-thumbnails-0.0.7/LICENSE` & `mkdocs-thumbnails-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-thumbnails-0.0.7/PKG-INFO` & `mkdocs-thumbnails-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-thumbnails
-Version: 0.0.7
+Version: 0.0.9
 Summary: An MkDocs plugin.  Generates thumbnails of PDF files and YouTube links.
 Home-page: https://github.com/normanlorrain/mkdocs-thumbnails
 Author: Norman Lorrain
 Author-email: normanlorrain@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/normanlorrain/mkdocs-thumbnails/issues
 Platform: UNKNOWN
@@ -58,15 +58,15 @@
 
 ```
 
 The markdown conversion generates:
 ```html
 <a href="foo.pdf" class="pdf" >My PDF file</a>
 <br>
-<a href="https://youtu.be/dQw4w9WgXcQ">A YouTube video link</a>
+<a href="https://youtu.be/dQw4w9WgXcQ" class="youtube" >A YouTube video link</a>
 <br>
 ```
 
 ...which is converted by the plugin:
 ```html
 <a href="foo.pdf"><img src="foo.pdf-thumb.png" class="pdf" >My PDF file</a>
 <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-thumbnails Version: 0.0.7 Summary: An MkDocs
+Metadata-Version: 2.1 Name: mkdocs-thumbnails Version: 0.0.9 Summary: An MkDocs
 plugin. Generates thumbnails of PDF files and YouTube links. Home-page: https:/
 /github.com/normanlorrain/mkdocs-thumbnails Author: Norman Lorrain Author-
 email: normanlorrain@gmail.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/normanlorrain/mkdocs-thumbnails/issues Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `mkdocs-thumbnails-0.0.7/README.md` & `mkdocs-thumbnails-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 ```
 
 The markdown conversion generates:
 ```html
 <a href="foo.pdf" class="pdf" >My PDF file</a>
 <br>
-<a href="https://youtu.be/dQw4w9WgXcQ">A YouTube video link</a>
+<a href="https://youtu.be/dQw4w9WgXcQ" class="youtube" >A YouTube video link</a>
 <br>
 ```
 
 ...which is converted by the plugin:
 ```html
 <a href="foo.pdf"><img src="foo.pdf-thumb.png" class="pdf" >My PDF file</a>
 <br>
```

### Comparing `mkdocs-thumbnails-0.0.7/setup.cfg` & `mkdocs-thumbnails-0.0.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6b64 6f63 732d 7468 756d 626e   = mkdocs-thumbn
 00000020: 6169 6c73 0d0a 7665 7273 696f 6e20 3d20  ails..version = 
-00000030: 302e 302e 370d 0a61 7574 686f 7220 3d20  0.0.7..author = 
+00000030: 302e 302e 390d 0a61 7574 686f 7220 3d20  0.0.9..author = 
 00000040: 4e6f 726d 616e 204c 6f72 7261 696e 0d0a  Norman Lorrain..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 206e  author_email = n
 00000060: 6f72 6d61 6e6c 6f72 7261 696e 4067 6d61  ormanlorrain@gma
 00000070: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000080: 696f 6e20 3d20 416e 204d 6b44 6f63 7320  ion = An MkDocs 
 00000090: 706c 7567 696e 2e20 2047 656e 6572 6174  plugin.  Generat
 000000a0: 6573 2074 6875 6d62 6e61 696c 7320 6f66  es thumbnails of
@@ -40,19 +40,20 @@
 00000270: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
 00000280: 7320 3d20 3e3d 332e 360d 0a69 6e73 7461  s = >=3.6..insta
 00000290: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
 000002a0: 0970 796d 7570 6466 203e 3d31 2e31 380d  .pymupdf >=1.18.
 000002b0: 0a09 6d6b 646f 6373 203e 3d31 2e30 0d0a  ..mkdocs >=1.0..
 000002c0: 0950 696c 6c6f 7720 3e3d 382e 300d 0a09  .Pillow >=8.0...
 000002d0: 6265 6175 7469 6675 6c73 6f75 7034 0d0a  beautifulsoup4..
-000002e0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002f0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000300: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000310: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000320: 0d0a 6d6b 646f 6373 2e70 6c75 6769 6e73  ..mkdocs.plugins
-00000330: 203d 200d 0a09 7468 756d 626e 6169 6c73   = ...thumbnails
-00000340: 203d 2074 6875 6d62 6e61 696c 732e 706c   = thumbnails.pl
-00000350: 7567 696e 3a54 6875 6d62 6e61 696c 4d61  ugin:ThumbnailMa
-00000360: 6b65 720d 0a0d 0a5b 6567 675f 696e 666f  ker....[egg_info
-00000370: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000380: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000390: 0a                                       .
+000002e0: 0972 6571 7565 7374 732d 6361 6368 650d  .requests-cache.
+000002f0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000300: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000310: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
+00000320: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+00000330: 5d0d 0a6d 6b64 6f63 732e 706c 7567 696e  ]..mkdocs.plugin
+00000340: 7320 3d20 0d0a 0974 6875 6d62 6e61 696c  s = ...thumbnail
+00000350: 7320 3d20 7468 756d 626e 6169 6c73 2e70  s = thumbnails.p
+00000360: 6c75 6769 6e3a 5468 756d 626e 6169 6c4d  lugin:ThumbnailM
+00000370: 616b 6572 0d0a 0d0a 5b65 6767 5f69 6e66  aker....[egg_inf
+00000380: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000390: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000003a0: 0d0a                                     ..
```

### Comparing `mkdocs-thumbnails-0.0.7/src/mkdocs_thumbnails.egg-info/PKG-INFO` & `mkdocs-thumbnails-0.0.9/src/mkdocs_thumbnails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-thumbnails
-Version: 0.0.7
+Version: 0.0.9
 Summary: An MkDocs plugin.  Generates thumbnails of PDF files and YouTube links.
 Home-page: https://github.com/normanlorrain/mkdocs-thumbnails
 Author: Norman Lorrain
 Author-email: normanlorrain@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/normanlorrain/mkdocs-thumbnails/issues
 Platform: UNKNOWN
@@ -58,15 +58,15 @@
 
 ```
 
 The markdown conversion generates:
 ```html
 <a href="foo.pdf" class="pdf" >My PDF file</a>
 <br>
-<a href="https://youtu.be/dQw4w9WgXcQ">A YouTube video link</a>
+<a href="https://youtu.be/dQw4w9WgXcQ" class="youtube" >A YouTube video link</a>
 <br>
 ```
 
 ...which is converted by the plugin:
 ```html
 <a href="foo.pdf"><img src="foo.pdf-thumb.png" class="pdf" >My PDF file</a>
 <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-thumbnails Version: 0.0.7 Summary: An MkDocs
+Metadata-Version: 2.1 Name: mkdocs-thumbnails Version: 0.0.9 Summary: An MkDocs
 plugin. Generates thumbnails of PDF files and YouTube links. Home-page: https:/
 /github.com/normanlorrain/mkdocs-thumbnails Author: Norman Lorrain Author-
 email: normanlorrain@gmail.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/normanlorrain/mkdocs-thumbnails/issues Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `mkdocs-thumbnails-0.0.7/src/thumbnails/plugin.py` & `mkdocs-thumbnails-0.0.9/src/thumbnails/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,22 +71,24 @@
         # YouTube links
         # See https://webapps.stackexchange.com/questions/54443/format-for-id-of-youtube-video
         #
         links = soup.find_all("a", class_="youtube")
         self.yt_count+=len(links)
         for link in links:
             href = link.get('href')
-            id = re.search( r'.*youtu.be\/([0-9A-Za-z_-]+).*', href).group(1)
             try:
-                thumbnail.createYouTubeThumb(id, tgtDir/Path(id+"-thumb.png"))
-            except urllib.error.HTTPError as e:
-                log.warn(f'Bad Youtube link: {href} in {pageFile.abs_src_path} ')
-                continue
-
-            
+                if 'playlist' in href:
+                    id = re.search( r'.*playlist\?list=([0-9A-Za-z_-]+).*', href).group(1)
+                    thumbnail.createYouTubePlaylistThumb(href,tgtDir/Path(id+"-thumb.png"))
+                else:
+                    id = re.search( r'.*youtu.be\/([0-9A-Za-z_-]+).*', href).group(1)
+                    thumbnail.createYouTubeThumb(id, tgtDir/Path(id+"-thumb.png"))
+            except thumbnail.HTTPError as e:
+                    log.warn(f'Bad Youtube link: {href} in {pageFile.abs_src_path} ')
+                    continue
             img = soup.new_tag('img')
             img['src'] = f"{id}-thumb.png"
             img['style'] = self.config["style"]
             img['class'] = "youtube"
             del link['class']
             link.contents.insert(0,img)
```

### Comparing `mkdocs-thumbnails-0.0.7/src/thumbnails/thumbnail.py` & `mkdocs-thumbnails-0.0.9/src/thumbnails/thumbnail.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import glob
 import shutil
 import tempfile
 from pathlib import Path
 import os
-from urllib.request import pathname2url
+import requests_cache
 import sys
 import json
 import fitz
 from PIL import Image
 from jinja2 import Environment, FileSystemLoader, select_autoescape
-import urllib.request
+from requests.exceptions import *
+_session = requests_cache.CachedSession()
 
 
 def createPdfThumb(inputPDFfile,outputThumbFile):        
     # Extract image
     doc = fitz.open(inputPDFfile)  # open document
     pix = doc.get_page_pixmap(0, alpha=False)  # render page to an image
 
@@ -26,22 +27,43 @@
     if not outputThumbFile.parent.exists():
         outputThumbFile.parent.mkdir(parents=True, exist_ok = True)
 
     # Save image to file
     im.save(str(outputThumbFile))
 
 def createYouTubeThumb(id, outputThumbFile):
-    # Get image from YouTube
-    url = f'https://img.youtube.com/vi/{id}/default.jpg'
-    thumbdata = urllib.request.urlopen(url)
+    # Create directory paths if necessary
+    if not outputThumbFile.parent.exists():
+        outputThumbFile.parent.mkdir(parents=True, exist_ok = True)
 
+    # Save image 
+    with open(outputThumbFile,'wb') as outfile:
+         # Get image from YouTube
+        url = f'https://img.youtube.com/vi/{id}/default.jpg'
+        response = _session.get(url)
+        response.raise_for_status()
+        imageBytes = response.content
+        outfile.write(imageBytes)
+        
+    
+# Playlists are a little harder; need to get the thumbnail via the oembed api
+def createYouTubePlaylistThumb(playlistUrl, outputThumbFile):
     # Create directory paths if necessary
     if not outputThumbFile.parent.exists():
         outputThumbFile.parent.mkdir(parents=True, exist_ok = True)
 
     # Save image 
     with open(outputThumbFile,'wb') as outfile:
-        outfile.write(thumbdata.read())
+        # Get URL of thumbnail from playlist url 
+        response = _session.get(f'https://youtube.com/oembed?url={playlistUrl}&format=json')
+        response.raise_for_status()
+        playlistData = response.json()
+        
+        # Get thumbnail 
+        response = _session.get(playlistData['thumbnail_url'])
+        response.raise_for_status()
+
+        outfile.write(response.content)
```

