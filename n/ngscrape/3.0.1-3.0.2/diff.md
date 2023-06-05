# Comparing `tmp/ngscrape-3.0.1.tar.gz` & `tmp/ngscrape-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-3.0.1.tar", last modified: Mon Jun  5 15:25:26 2023, max compression
+gzip compressed data, was "ngscrape-3.0.2.tar", last modified: Mon Jun  5 15:29:07 2023, max compression
```

## Comparing `ngscrape-3.0.1.tar` & `ngscrape-3.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:25:26.199057 ngscrape-3.0.1/
--rw-rw-rw-   0        0        0    35184 2023-06-04 00:16:21.000000 ngscrape-3.0.1/LICENSE
--rw-rw-rw-   0        0        0    44207 2023-06-05 15:25:26.199057 ngscrape-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-06-05 15:24:53.000000 ngscrape-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     3170 2023-06-05 15:12:52.000000 ngscrape-3.0.1/readme.md
--rw-rw-rw-   0        0        0       42 2023-06-05 15:25:26.199057 ngscrape-3.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-05 15:25:26.196608 ngscrape-3.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 15:25:26.199057 ngscrape-3.0.1/src/ngscrape/
--rw-rw-rw-   0        0        0    11018 2023-06-05 15:24:22.000000 ngscrape-3.0.1/src/ngscrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:25:26.199057 ngscrape-3.0.1/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    44207 2023-06-05 15:25:26.000000 ngscrape-3.0.1/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-05 15:25:26.000000 ngscrape-3.0.1/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:25:26.000000 ngscrape-3.0.1/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-05 15:25:26.000000 ngscrape-3.0.1/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 15:25:26.000000 ngscrape-3.0.1/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 15:29:07.736570 ngscrape-3.0.2/
+-rw-rw-rw-   0        0        0    35184 2023-06-04 00:16:21.000000 ngscrape-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0    44207 2023-06-05 15:29:07.735571 ngscrape-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-06-05 15:28:30.000000 ngscrape-3.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     3170 2023-06-05 15:12:52.000000 ngscrape-3.0.2/readme.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:29:07.736570 ngscrape-3.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 15:29:07.695015 ngscrape-3.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 15:29:07.699790 ngscrape-3.0.2/src/ngscrape/
+-rw-rw-rw-   0        0        0    11088 2023-06-05 15:28:14.000000 ngscrape-3.0.2/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:29:07.734570 ngscrape-3.0.2/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    44207 2023-06-05 15:29:07.000000 ngscrape-3.0.2/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-05 15:29:07.000000 ngscrape-3.0.2/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:29:07.000000 ngscrape-3.0.2/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-05 15:29:07.000000 ngscrape-3.0.2/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 15:29:07.000000 ngscrape-3.0.2/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-3.0.1/LICENSE` & `ngscrape-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-3.0.1/PKG-INFO` & `ngscrape-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 3.0.1
+Version: 3.0.2
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ngscrape-3.0.1/pyproject.toml` & `ngscrape-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "3.0.1"
+version = "3.0.2"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
```

### Comparing `ngscrape-3.0.1/readme.md` & `ngscrape-3.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `ngscrape-3.0.1/src/ngscrape/__init__.py` & `ngscrape-3.0.2/src/ngscrape/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,17 +189,21 @@
         except:
             if self.cache:
                 self.cachedsites[url] = _gameHTML
             _gameHTML = requests.get(url)
         if self.debug:
             print('NGScrape: Made request to ' + url + ' and got status code ' + str(_gameHTML.status_code))
         _soup = bs4.BeautifulSoup(_gameHTML.content, self.parser)
-        if self.debug:
-            print('NGScrape: Found game title "' + _soup.find('title').get_text() + '"')
-        return _soup.find('title').get_text()
+
+        try:
+            if self.debug:
+                print('NGScrape: Found game title "' + _soup.find('title').get_text() + '"')
+            return _soup.find('title').get_text()
+        except:
+            return None
 if __name__ == '__main__':
     import sys
     scraper = Scraper(debug = True)
     try:
         scraper.scrape_game(sys.argv[1])
         scraper.scrape_card(sys.argv[1])
         scraper.scrape_desc(sys.argv[1])
```

### Comparing `ngscrape-3.0.1/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-3.0.2/src/ngscrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 3.0.1
+Version: 3.0.2
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

