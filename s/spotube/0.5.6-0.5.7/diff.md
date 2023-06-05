# Comparing `tmp/spotube-0.5.6.tar.gz` & `tmp/spotube-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotube-0.5.6.tar", max compression
+gzip compressed data, was "spotube-0.5.7.tar", max compression
```

## Comparing `spotube-0.5.6.tar` & `spotube-0.5.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3184 2023-06-03 14:20:17.592777 spotube-0.5.6/LICENSE
--rw-r--r--   0        0        0     6182 2023-06-03 14:20:17.592777 spotube-0.5.6/README.md
--rw-r--r--   0        0        0      742 2023-06-03 14:24:49.067513 spotube-0.5.6/pyproject.toml
--rw-r--r--   0        0        0       40 2023-06-03 14:20:17.592777 spotube-0.5.6/spotube/__init__.py
--rw-r--r--   0        0        0     3638 2023-06-03 14:20:17.592777 spotube-0.5.6/spotube/downloader_class.py
--rw-r--r--   0        0        0    15914 2023-06-03 14:20:17.592777 spotube-0.5.6/spotube/downloader_utils.py
--rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 spotube-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     3184 2023-06-05 18:12:47.828129 spotube-0.5.7/LICENSE
+-rw-r--r--   0        0        0     6182 2023-06-05 18:12:47.828129 spotube-0.5.7/README.md
+-rw-r--r--   0        0        0      742 2023-06-05 18:18:04.419427 spotube-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-06-05 18:12:47.828129 spotube-0.5.7/spotube/__init__.py
+-rw-r--r--   0        0        0     3638 2023-06-05 18:12:47.828129 spotube-0.5.7/spotube/downloader_class.py
+-rw-r--r--   0        0        0    16042 2023-06-05 18:12:47.828129 spotube-0.5.7/spotube/downloader_utils.py
+-rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 spotube-0.5.7/PKG-INFO
```

### Comparing `spotube-0.5.6/LICENSE` & `spotube-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spotube-0.5.6/README.md` & `spotube-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `spotube-0.5.6/pyproject.toml` & `spotube-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotube"
-version = "0.5.6"
+version = "0.5.7"
 description = "A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs."
 authors = ["GiorgosNik <giorgosnl17@gmail.com>"]
 license = "Free for non-commercial use"
 readme = "README.md"
 repository = 'https://github.com/GiorgosNik/spotube-package'
 packages = [{include = "spotube"}]
```

### Comparing `spotube-0.5.6/spotube/downloader_class.py` & `spotube-0.5.7/spotube/downloader_class.py`

 * *Files identical despite different names*

### Comparing `spotube-0.5.6/spotube/downloader_utils.py` & `spotube-0.5.7/spotube/downloader_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,14 +500,16 @@
         members = archive.getmembers()
         extraction_bar = tqdm(
             total=len(members), desc="Extracting files", position=1, leave=False
         )
         for member in members:
             if member.isreg() and member.name.split(".")[0] == member.name:
                 member.name = os.path.basename(member.name)
+                if os.getcwd() not in  os.path.realpath(member.name):
+                    raise RuntimeError("Invalid tarball")
                 archive.extract(member.name, ".")
             extraction_bar.update(n=1)
     os.remove(filename)
 
 
 class DownloadProgressBar(tqdm):
     def update_to(self, b=1, bsize=1, tsize=None):
```

### Comparing `spotube-0.5.6/PKG-INFO` & `spotube-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotube
-Version: 0.5.6
+Version: 0.5.7
 Summary: A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs.
 Home-page: https://github.com/GiorgosNik/spotube-package
 License: Free for non-commercial use
 Author: GiorgosNik
 Author-email: giorgosnl17@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

