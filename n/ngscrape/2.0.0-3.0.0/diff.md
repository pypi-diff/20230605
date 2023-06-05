# Comparing `tmp/ngscrape-2.0.0.tar.gz` & `tmp/ngscrape-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-2.0.0.tar", last modified: Sun Jun  4 00:43:46 2023, max compression
+gzip compressed data, was "ngscrape-3.0.0.tar", last modified: Mon Jun  5 15:17:03 2023, max compression
```

## Comparing `ngscrape-2.0.0.tar` & `ngscrape-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.646937 ngscrape-2.0.0/
--rw-rw-rw-   0        0        0    35184 2023-06-04 00:16:21.000000 ngscrape-2.0.0/LICENSE
--rw-rw-rw-   0        0        0    44073 2023-06-04 00:43:46.645936 ngscrape-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-06-04 00:32:50.000000 ngscrape-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     3036 2023-06-04 00:32:26.000000 ngscrape-2.0.0/readme.md
--rw-rw-rw-   0        0        0       42 2023-06-04 00:43:46.646937 ngscrape-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.600712 ngscrape-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.607714 ngscrape-2.0.0/src/ngscrape/
--rw-rw-rw-   0        0        0    11246 2023-06-04 00:32:25.000000 ngscrape-2.0.0/src/ngscrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.644936 ngscrape-2.0.0/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    44073 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:03.942740 ngscrape-3.0.0/
+-rw-rw-rw-   0        0        0    35184 2023-06-04 00:16:21.000000 ngscrape-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0    44207 2023-06-05 15:17:03.942740 ngscrape-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-06-05 15:16:24.000000 ngscrape-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     3170 2023-06-05 15:12:52.000000 ngscrape-3.0.0/readme.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:17:03.943738 ngscrape-3.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:03.906117 ngscrape-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:03.909117 ngscrape-3.0.0/src/ngscrape/
+-rw-rw-rw-   0        0        0    11021 2023-06-05 15:13:30.000000 ngscrape-3.0.0/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:03.940738 ngscrape-3.0.0/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    44207 2023-06-05 15:17:03.000000 ngscrape-3.0.0/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-05 15:17:03.000000 ngscrape-3.0.0/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:17:03.000000 ngscrape-3.0.0/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-05 15:17:03.000000 ngscrape-3.0.0/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 15:17:03.000000 ngscrape-3.0.0/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-2.0.0/LICENSE` & `ngscrape-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-2.0.0/PKG-INFO` & `ngscrape-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 2.0.0
+Version: 3.0.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,47 +680,47 @@
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
-    - Parameters:
-        - debug (bool) = False: Enable/Disable debug mode
-        - cache (bool) = False: Enable/Disable caching
+        - Parameters:
+            - debug (bool) = False: Enable/Disable debug mode
+            - cache (bool) = False: Enable/Disable caching
+            - parser (str) = 'lxml': Parser used by BS4
 - `scrape_game(url: str, download: str, filename: str) -> None`
-    - Scrape a flash game by url.
-    - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-        - download (str): The directory to download the file to.
-        - filename (str): The name of the downloaded file.
-    - Example parameters:
-        - `url = 'https://www.newgrounds.com/portal/view/59593'`
-        - `download = 'testdir'`
-        - `filename = 'game.swf'`
-    - Example output with debug mode:
-        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-        - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
-        - NGScrape: Downloaded swf file to testdir/game.swf
+    - Scrape a flash game by url. Returns the URL for the swf.
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
 - `scrape_desc(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
-    - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-    - Example parameters:
-        - `url = 'https://www.newgrounds.com/portal/view/59593'`
-    - Example output with debug mode:
-        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-        - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
-- `scrape_card(self, url: str, download: str, filename: str) -> str`
-    - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
-    - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-        - download (str): The directory to download the file to.
-        - filename (str): The name of the downloaded file. The file extention will be automatically determined.
-    - Example parameters:
-        - `url = 'https://www.newgrounds.com/portal/view/59593'`
-        - `download = 'testdir'`
-        - `filename = 'card'`
-    - Example output with debug mode:
-        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-        - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
-        - NGScrape: Downloaded `png` file to `testdir/card.png`
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
+- `scrape_card(self, url: str) -> str`
+    - Scrape a flash game's card by url. Returns the URL of the card file.
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
+- `scrape_title(self, url: str) -> str`
+    - Scrape a flash game's title with url. Returns title of the flash game.
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found game title "Alien Homonid"
```

### Comparing `ngscrape-2.0.0/pyproject.toml` & `ngscrape-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "2.0.0"
+version = "3.0.0"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
```

### Comparing `ngscrape-2.0.0/src/ngscrape/__init__.py` & `ngscrape-3.0.0/src/ngscrape/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,91 +11,88 @@
     NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
     Please star is this was useful!
 
     Functions:
     - `__init__(debug: bool = False) -> None`
         - Start a new NGScrape Instance.
-        - Parameters:
-            - debug (bool) = False: Enable/Disable debug mode
-            - cache (bool) = False: Enable/Disable caching
+            - Parameters:
+                - debug (bool) = False: Enable/Disable debug mode
+                - cache (bool) = False: Enable/Disable caching
+                - parser (str) = 'lxml': Parser used by BS4
     - `scrape_game(url: str, download: str, filename: str) -> None`
-        - Scrape a flash game by url.
-        - Parameters:
-            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-            - download (str): The directory to download the file to.
-            - filename (str): The name of the downloaded file.
-        - Example parameters:
-            - `url = 'https://www.newgrounds.com/portal/view/59593'`
-            - `download = 'testdir'`
-            - `filename = 'game.swf'`
-        - Example output with debug mode:
-            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-            - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
-            - NGScrape: Downloaded swf file to testdir/game.swf
+        - Scrape a flash game by url. Returns the URL for the swf.
+            - Parameters:
+                - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+            - Example parameters:
+                - `url = 'https://www.newgrounds.com/portal/view/59593'`
+            - Example output with debug mode:
+                - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+                - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
     - `scrape_desc(self, url: str) -> str`
         - Scrape a flash game's description by url. Returns the description of the game.
-        - Parameters:
-            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-        - Example parameters:
-            - `url = 'https://www.newgrounds.com/portal/view/59593'`
-        - Example output with debug mode:
-            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-            - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
-    - `scrape_card(self, url: str, download: str, filename: str) -> str`
-        - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
-        - Parameters:
-            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-            - download (str): The directory to download the file to.
-            - filename (str): The name of the downloaded file. The file extention will be automatically determined.
-        - Example parameters:
-            - `url = 'https://www.newgrounds.com/portal/view/59593'`
-            - `download = 'testdir'`
-            - `filename = 'card'`
-        - Example output with debug mode:
-            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-            - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
-            - NGScrape: Downloaded `png` file to `testdir/card.png`
+            - Parameters:
+                - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+            - Example parameters:
+                - `url = 'https://www.newgrounds.com/portal/view/59593'`
+            - Example output with debug mode:
+                - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+                - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
+    - `scrape_card(self, url: str) -> str`
+        - Scrape a flash game's card by url. Returns the URL of the card file.
+            - Parameters:
+                - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+            - Example parameters:
+                - `url = 'https://www.newgrounds.com/portal/view/59593'`
+            - Example output with debug mode:
+                - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+                - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
+    - `scrape_title(self, url: str) -> str`
+        - Scrape a flash game's title with url. Returns title of the flash game.
+            - Parameters:
+                - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+            - Example parameters:
+                - `url = 'https://www.newgrounds.com/portal/view/59593'`
+            - Example output with debug mode:
+                - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+                - NGScrape: Found game title "Alien Homonid"
     '''
-    def __init__(self, debug: bool = False, cache: bool = False) -> None:
+    def __init__(self, debug: bool = False, cache: bool = False, parser: str = 'lxml') -> None:
         '''
         Start a new NGScrape Instance.
         - Parameters:
             - debug (bool) = False: Enable/Disable debug mode
             - cache (bool) = False: Enable/Disable caching
+            - parser (str) = 'lxml': Parser used by BS4
         '''
         self.debug = debug
         self.cache = cache
+        self.parser = parser
         self.cachedsites = {}
         return
     
-    def scrape_game(self, url: str, download: str, filename: str) -> None:
+    def scrape_game(self, url: str) -> str:
         '''
-        Scrape a flash game by url.
+        Scrape a flash game by url. Returns the URL for the swf.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-            - download (str): The directory to download the file to.
-            - filename (str): The name of the downloaded file.
         - Example parameters:
             - `url = 'https://www.newgrounds.com/portal/view/59593'`
-            - `download = 'testdir'`
-            - `filename = 'game.swf'`
         - Example output with debug mode:
             - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
             - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
-            - NGScrape: Downloaded swf file to testdir/game.swf
         '''
         try:
             self.cachedsites[url]
             _gameHTML = self.cachedsites[url]
         except:
             if self.cache:
                 self.cachedsites[url] = _gameHTML
             _gameHTML = requests.get(url)
-        _soup = bs4.BeautifulSoup(_gameHTML.content, 'html.parser')
+        _soup = bs4.BeautifulSoup(_gameHTML.content, self.parser)
         if self.debug:
             print('NGScrape: Made request to ' + url + ' and got status code ' + str(_gameHTML.status_code))
         '''
         NOTE: Newgrounds site format has the flash game url inside <script> tags, with the varible 'embed_controller'.
         Example:
         var embed_controller = new embedController([{"url":"https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499","is_published":true, ... );
                             0                          1  2                                     [3]
@@ -103,71 +100,49 @@
         _scripts = _soup.find_all('script')
         for i in _scripts:
             if 'var embed_controller = new embedController([{"url":"' in i.get_text():
                 _gameLink: str = i.get_text().split('"')[3]
                 if self.debug:
                     print('NGScrape: Found flash game link ' + _gameLink)
                 break
-        try:
-            os.mkdir(download)
-        except:
-            pass
-        open(download + '/' + filename, 'wb').write(requests.get(_gameLink.replace('\\', ''), allow_redirects = True).content)
-        if self.debug:
-            print('NGScrape: Downloaded swf file to ' + download + '/' + filename)
+        return _gameLink.replace('\\', '')
             
-    def scrape_card(self, url: str, download: str, filename: str) -> str:
+    def scrape_card(self, url: str) -> str:
         '''
-        Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
+        Scrape a flash game's card by url. Returns the URL of the card file.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-            - download (str): The directory to download the file to.
-            - filename (str): The name of the downloaded file. The file extention will be automatically determined.
         - Example parameters:
             - `url = 'https://www.newgrounds.com/portal/view/59593'`
-            - `download = 'testdir'`
-            - `filename = 'card'`
         - Example output with debug mode:
             - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
             - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
-            - NGScrape: Downloaded `png` file to `testdir/card.png`
         '''
         try:
-            os.mkdir(download)
-        except:
-            pass
-        try:
             self.cachedsites[url]
             _gameHTML = self.cachedsites[url]
         except:
             if self.cache:
                 self.cachedsites[url] = _gameHTML
             _gameHTML = requests.get(url)
         if self.debug:
             print('NGScrape: Made request to ' + url + ' and got status code ' + str(_gameHTML.status_code))
-        _soup = bs4.BeautifulSoup(_gameHTML.content, 'html.parser')
+        _soup = bs4.BeautifulSoup(_gameHTML.content, self.parser)
         
         _metadata = _soup.find_all('meta')
         for i in _metadata:
             try:
                 if i['property'] == 'og:image':
                     _gameLink = i['content']
                     if self.debug:
                         print('NGScrape: Found card link ' + _gameLink)
                     break
             except:
                 pass # This is because some tags don't have the property attribute
-        _commonImageFileTypes = ['.png', '.jpg', '.jfif', '.webp', '.jpeg', '.jpe', '.jif', '.jfi', '.bmp']
-        for i in _commonImageFileTypes:
-            if i in _gameLink:
-                _imageFiletype = i
-        open(download + '/' + filename + _imageFiletype, 'wb').write(requests.get(_gameLink, allow_redirects = True).content)
-        if self.debug:
-            print('NGScrape: Downloaded swf file to ' + download + '/' + filename + _imageFiletype)
-        return filename + _imageFiletype
+        return _gameLink
     def scrape_desc(self, url: str) -> str:
         '''
         Scrape a flash game's description by url. Returns the description of the game.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - Example parameters:
             - `url = 'https://www.newgrounds.com/portal/view/59593'`
@@ -181,31 +156,54 @@
             _gameHTML = self.cachedsites[url]
         except:
             if self.cache:
                 self.cachedsites[url] = _gameHTML
             _gameHTML = requests.get(url)
         if self.debug:
             print('NGScrape: Made request to ' + url + ' and got status code ' + str(_gameHTML.status_code))
-        _soup = bs4.BeautifulSoup(_gameHTML.content, 'html.parser')
+        _soup = bs4.BeautifulSoup(_gameHTML.content, self.parser)
         
         _metadata = _soup.find_all('meta')
         for i in _metadata:
             try:
                 if i['property'] == 'og:description':
                     _desc = i['content']
                     if self.debug:
                         print('Found game description "' + _desc + '"')
                     return _desc
             except:
                 pass # This is because some tags don't have the property attribute
-        
+    def scrape_title(self, url: str) -> str:
+        '''
+        Scrape a flash game's title with url. Returns title of the flash game.
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found game title "Alien Homonid"
+        '''
+        try:
+            self.cachedsites[url]
+            _gameHTML = self.cachedsites[url]
+        except:
+            if self.cache:
+                self.cachedsites[url] = _gameHTML
+            _gameHTML = requests.get(url)
+        if self.debug:
+            print('NGScrape: Made request to ' + url + ' and got status code ' + str(_gameHTML.status_code))
+        _soup = bs4.BeautifulSoup(_gameHTML.content, self.parser)
+        if self.debug:
+            print('NGScrape: Found game title "' + _soup.find_next('title').get_text() + '"')
+        return _soup.find_next('title').get_text()
 if __name__ == '__main__':
     import sys
     scraper = Scraper(debug = True)
     try:
-        scraper.scrape_game(sys.argv[1], sys.argv[2], sys.argv[3])
-        scraper.scrape_card(sys.argv[1], sys.argv[2], sys.argv[3].replace('.swf', ''))
+        scraper.scrape_game(sys.argv[1])
+        scraper.scrape_card(sys.argv[1])
         scraper.scrape_desc(sys.argv[1])
     except:
-        print('ngscrape [newgrounds url, should be formatted like this: https://www.newgrounds.com/portal/view/xxxxx] [directory to save to] [file to save to]')
+        print('ngscrape https://www.newgrounds.com/portal/view/xxxxx')
         exit(1)
     exit(0)
```

### Comparing `ngscrape-2.0.0/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-3.0.0/src/ngscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 2.0.0
+Version: 3.0.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,47 +680,47 @@
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
-    - Parameters:
-        - debug (bool) = False: Enable/Disable debug mode
-        - cache (bool) = False: Enable/Disable caching
+        - Parameters:
+            - debug (bool) = False: Enable/Disable debug mode
+            - cache (bool) = False: Enable/Disable caching
+            - parser (str) = 'lxml': Parser used by BS4
 - `scrape_game(url: str, download: str, filename: str) -> None`
-    - Scrape a flash game by url.
-    - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-        - download (str): The directory to download the file to.
-        - filename (str): The name of the downloaded file.
-    - Example parameters:
-        - `url = 'https://www.newgrounds.com/portal/view/59593'`
-        - `download = 'testdir'`
-        - `filename = 'game.swf'`
-    - Example output with debug mode:
-        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-        - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
-        - NGScrape: Downloaded swf file to testdir/game.swf
+    - Scrape a flash game by url. Returns the URL for the swf.
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
 - `scrape_desc(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
-    - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-    - Example parameters:
-        - `url = 'https://www.newgrounds.com/portal/view/59593'`
-    - Example output with debug mode:
-        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-        - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
-- `scrape_card(self, url: str, download: str, filename: str) -> str`
-    - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
-    - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
-        - download (str): The directory to download the file to.
-        - filename (str): The name of the downloaded file. The file extention will be automatically determined.
-    - Example parameters:
-        - `url = 'https://www.newgrounds.com/portal/view/59593'`
-        - `download = 'testdir'`
-        - `filename = 'card'`
-    - Example output with debug mode:
-        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
-        - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
-        - NGScrape: Downloaded `png` file to `testdir/card.png`
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
+- `scrape_card(self, url: str) -> str`
+    - Scrape a flash game's card by url. Returns the URL of the card file.
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
+- `scrape_title(self, url: str) -> str`
+    - Scrape a flash game's title with url. Returns title of the flash game.
+        - Parameters:
+            - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - Example parameters:
+            - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - Example output with debug mode:
+            - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+            - NGScrape: Found game title "Alien Homonid"
```

