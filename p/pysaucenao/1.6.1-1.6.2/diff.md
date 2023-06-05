# Comparing `tmp/pysaucenao-1.6.1.tar.gz` & `tmp/pysaucenao-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysaucenao-1.6.1.tar", last modified: Fri May  7 04:31:51 2021, max compression
+gzip compressed data, was "pysaucenao-1.6.2.tar", last modified: Mon Jun  5 07:21:23 2023, max compression
```

## Comparing `pysaucenao-1.6.1.tar` & `pysaucenao-1.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 04:31:51.380641 pysaucenao-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-05-07 04:31:42.000000 pysaucenao-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8533 2021-05-07 04:31:51.380641 pysaucenao-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6523 2021-05-07 04:31:42.000000 pysaucenao-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 04:31:51.380641 pysaucenao-1.6.1/pysaucenao/
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-05-07 04:31:42.000000 pysaucenao-1.6.1/pysaucenao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19018 2021-05-07 04:31:42.000000 pysaucenao-1.6.1/pysaucenao/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2021-05-07 04:31:42.000000 pysaucenao-1.6.1/pysaucenao/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7944 2021-05-07 04:31:42.000000 pysaucenao-1.6.1/pysaucenao/saucenao.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 04:31:51.380641 pysaucenao-1.6.1/pysaucenao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8533 2021-05-07 04:31:51.000000 pysaucenao-1.6.1/pysaucenao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-05-07 04:31:51.000000 pysaucenao-1.6.1/pysaucenao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-07 04:31:51.000000 pysaucenao-1.6.1/pysaucenao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-07 04:31:51.000000 pysaucenao-1.6.1/pysaucenao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-05-07 04:31:51.000000 pysaucenao-1.6.1/pysaucenao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-05-07 04:31:51.380641 pysaucenao-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2021-05-07 04:31:42.000000 pysaucenao-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:21:23.040161 pysaucenao-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 07:21:13.000000 pysaucenao-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-05 07:21:23.040161 pysaucenao-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-05 07:21:13.000000 pysaucenao-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:21:23.040161 pysaucenao-1.6.2/pysaucenao/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-05 07:21:13.000000 pysaucenao-1.6.2/pysaucenao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19680 2023-06-05 07:21:13.000000 pysaucenao-1.6.2/pysaucenao/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-05 07:21:13.000000 pysaucenao-1.6.2/pysaucenao/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-05 07:21:13.000000 pysaucenao-1.6.2/pysaucenao/saucenao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:21:23.040161 pysaucenao-1.6.2/pysaucenao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-05 07:21:22.000000 pysaucenao-1.6.2/pysaucenao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 07:21:23.000000 pysaucenao-1.6.2/pysaucenao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:21:22.000000 pysaucenao-1.6.2/pysaucenao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 07:21:22.000000 pysaucenao-1.6.2/pysaucenao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 07:21:22.000000 pysaucenao-1.6.2/pysaucenao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 07:21:23.040161 pysaucenao-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-05 07:21:13.000000 pysaucenao-1.6.2/setup.py
```

### Comparing `pysaucenao-1.6.1/LICENSE` & `pysaucenao-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysaucenao-1.6.1/PKG-INFO` & `pysaucenao-1.6.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,155 +1,134 @@
-Metadata-Version: 2.1
-Name: pysaucenao
-Version: 1.6.1
-Summary: PySauceNao is an unofficial asynchronous library for the SauceNao API. It supports lookups via URL or from the local filesystem.
-Home-page: https://github.com/FujiMakoto/pysaucenao
-Author: Makoto
-Author-email: makoto+github@taiga.sh
-License: gpl-3.0
-Download-URL: https://github.com/FujiMakoto/pysaucenao/archive/1.6.1.tar.gz
-Description: # PySauceNao
-        [![GitHub](https://img.shields.io/github/license/FujiMakoto/pysaucenao)](https://github.com/FujiMakoto/pysaucenao/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pysaucenao)](https://pypi.org/project/pysaucenao/) [![PyPI](https://img.shields.io/pypi/v/pysaucenao)](https://pypi.org/project/pysaucenao/) [![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/fujimakoto/pysaucenao/latest)](https://github.com/FujiMakoto/pysaucenao/releases)
-        
-        PySauceNao is an unofficial asynchronous library for the [SauceNao](https://saucenao.com/) API. It supports lookups via URL or from the local filesystem.
-        
-        # Installation
-        This library requires [Python 3.6](https://www.python.org) or above.
-        
-        You can install the library through pip as follows,
-        ```shell script
-        pip install pysaucenao
-        ```
-        
-        ## Usage
-        ```python
-        from pysaucenao import SauceNao
-        sauce = SauceNao(self, *, api_key: Optional[str] = None,
-                         db_mask: Optional[int] = None,
-                         db_mask_disable: Optional[int] = None,
-                         db: int = 999,
-                         results_limit: int = 6,
-                         min_similarity: float = 50.0,
-                         test_mode: int = 0,
-                         strict_mode: bool = True,
-                         loop: Optional[asyncio.AbstractEventLoop] = None)
-        
-        # results = await sauce.from_file('/path/to/image.png')
-        results = await sauce.from_url('https://i.imgur.com/QaKpV3s.png')
-        repr(results)
-        ```
-        ```
-        <SauceNaoResults(count=2, short_avail=3, long_avail=87, results=[<GenericSourc... Nico Seiga')>, <GenericSourc...e='Danbooru')>])>
-        ```
-        
-        The library attempts to provide a developer friendly container format for all results. Meaning, no matter if SauceNao returns a Pixiv source result or a more obscure source, you'll be able to easily pull the title, author URL and other useful information.
-        
-        ```python
-        from pysaucenao import SauceNao, PixivSource
-        sauce = SauceNao()
-        results = await sauce.from_url('https://i.imgur.com/oVPWy7f.png')
-        
-        len(results)  # 4
-        
-        # Find out how many API request limits you have remaining after a search query
-        results.short_remaining  # 3 (per 30 seconds limit)
-        results.long_remaining   # 86 (per day limit)
-        
-        # You can determine whether the search result is a Pixiv, Booru, Video or Other/Generic result by the type property or type checking
-        results[0].type  # pixiv
-        isinstance(results[0], PixivSource)  # True
-        
-        results[0].similarity     # 96.07
-        results[0].thumbnail      # Returns a temporary signed URL; not suitable for permanent hotlinking
-        results[0].title          # なでなでするにゃ
-        results[0].author_name    # おーじ茶＠3日目I-03b
-        results[0].author_url     # https://www.pixiv.net/member.php?id=122233
-        results[0].url            # https://www.pixiv.net/member_illust.php?mode=medium&illust_id=66106354
-        results[0].source_url     # Same as url for Pixiv results, but returns the linked original source URL for Booru entries
-        results[0].index          # Pixiv
-        ```
-        
-        Video search results provide three additional properties containing the episode number, estimated timestamp, and release year
-        ```python
-        from pysaucenao import SauceNao, VideoSource
-        sauce = SauceNao()
-        results = await sauce.from_url('https://i.imgur.com/1M8MhB0.png')
-        
-        if isinstance(results[0], VideoSource):
-            results[0].episode    # '1'
-            results[0].year       # '2017'
-            results[0].timestamp  # '00:07:53 / 00:23:40'
-        ```
-        
-        MangaSource search results, similarly, provide an additional `chapter` property.
-        
-        ### Advanced usage
-        
-        #### Additional source URL's
-        Thanks to [yuna.moe](https://github.com/BeeeQueue/arm-server), pysaucenao is no longer limited to just AniDB source URL's for anime results as of v1.3
-        
-        To utilize this new feature, you should first verify you are working with an Anime source.
-        
-        Once you have done that, you will need to preload the ID map by running the **load_ids** method.
-        
-        If you attempt to access any of the additional AnimeSource properties without first doing this, you will get an IndexError.
-        ```python
-        from pysaucenao import SauceNao, AnimeSource
-        sauce = SauceNao()
-        results = await sauce.from_url('https://i.imgur.com/poAmgY0.png')
-        
-        if isinstance(results[0], AnimeSource):
-            await results[0].load_ids()
-        ```
-        This will map the AniDB ID SauceNao returns with several other anime databases,
-        ```python
-        results[0].title        # Made in Abyss
-        results[0].anilist_id   # 97986
-        results[0].anilist_url  # https://anilist.co/anime/97986
-        results[0].mal_url      # https://myanimelist.net/anime/34599
-        results[0].kitsu_url    # https://kitsu.io/anime/13273
-        ```
-        
-        #### Priority
-        If you want to prioritize certain types of results, you can do so using the `priority` setting as of v1.2
-        
-        The most useful case for this is to prioritize anime results, preventing anime screencaps hosted on DeviantArt and other indexes some taking priority.
-        
-        To use this in your own code, just initialize SauceNao like so,
-        ```python
-        sauce = SauceNao(priority=[21, 22])
-        ```
-        As long as the anime search results are reasonably close to the next best match SauceNao returns, this will make sure the library always returns the anime result first, and ideally never a reposted screen-grab.
-        
-        If you need to prioritize other indexes, you can find a list of ID's here:
-        https://github.com/FujiMakoto/pysaucenao/blob/master/pysaucenao/containers.py#L16-L50
-        
-        ## Registering for an API key
-        If you are performing lots of API queries, you will eventually need to sign up and register for an API key (and possibly upgrade your account for very large request volumes)
-        
-        You can register for an account on [SauceNAO's website](https://saucenao.com/user.php)
-        
-        ## Error handling
-        The SauceNao class will throw an exception if any of the following occur:
-        * You have exceeded your 30-second search query limit (ShortLimitReachedException)
-        * You have exceeded your 24-hour search query limit (DailyLimitReachedException)
-        * You attempted to upload a file larger than SauceNAO allows (FileSizeLimitException)
-        * You provided an invalid API key (InvalidOrWrongApiKeyException)
-        * The image was too small for use (ImageSizeException)
-        * Either the URL or file provided was not a valid image (InvalidImageException)
-        * Too many failed requests made; try again later (TooManyFailedRequestsException)
-        * Your account does not have API access; contact SauceNao support (BannedException)
-        * Any other unknown error occurred / service may be down (UnknownStatusCodeException)
-        
-        All of these exceptions extend a base SauceNaoException class for easy catching and handling.
-        
-Keywords: saucenao,anime,artwork
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+# PySauceNao
+[![GitHub](https://img.shields.io/github/license/FujiMakoto/pysaucenao)](https://github.com/FujiMakoto/pysaucenao/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pysaucenao)](https://pypi.org/project/pysaucenao/) [![PyPI](https://img.shields.io/pypi/v/pysaucenao)](https://pypi.org/project/pysaucenao/) [![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/fujimakoto/pysaucenao/latest)](https://github.com/FujiMakoto/pysaucenao/releases)
+
+PySauceNao is an unofficial asynchronous library for the [SauceNao](https://saucenao.com/) API. It supports lookups via URL or from the local filesystem.
+
+# Installation
+This library requires [Python 3.6](https://www.python.org) or above.
+
+You can install the library through pip as follows,
+```shell script
+pip install pysaucenao
+```
+
+## Usage
+```python
+from pysaucenao import SauceNao
+sauce = SauceNao(self, *, api_key: Optional[str] = None,
+                 db_mask: Optional[int] = None,
+                 db_mask_disable: Optional[int] = None,
+                 db: int = 999,
+                 results_limit: int = 6,
+                 min_similarity: float = 50.0,
+                 test_mode: int = 0,
+                 strict_mode: bool = True,
+                 loop: Optional[asyncio.AbstractEventLoop] = None)
+
+# results = await sauce.from_file('/path/to/image.png')
+results = await sauce.from_url('https://i.imgur.com/QaKpV3s.png')
+repr(results)
+```
+```
+<SauceNaoResults(count=2, short_avail=3, long_avail=87, results=[<GenericSourc... Nico Seiga')>, <GenericSourc...e='Danbooru')>])>
+```
+
+The library attempts to provide a developer friendly container format for all results. Meaning, no matter if SauceNao returns a Pixiv source result or a more obscure source, you'll be able to easily pull the title, author URL and other useful information.
+
+```python
+from pysaucenao import SauceNao, PixivSource
+sauce = SauceNao()
+results = await sauce.from_url('https://i.imgur.com/oVPWy7f.png')
+
+len(results)  # 4
+
+# Find out how many API request limits you have remaining after a search query
+results.short_remaining  # 3 (per 30 seconds limit)
+results.long_remaining   # 86 (per day limit)
+
+# You can determine whether the search result is a Pixiv, Booru, Video or Other/Generic result by the type property or type checking
+results[0].type  # pixiv
+isinstance(results[0], PixivSource)  # True
+
+results[0].similarity     # 96.07
+results[0].thumbnail      # Returns a temporary signed URL; not suitable for permanent hotlinking
+results[0].title          # なでなでするにゃ
+results[0].author_name    # おーじ茶＠3日目I-03b
+results[0].author_url     # https://www.pixiv.net/member.php?id=122233
+results[0].url            # https://www.pixiv.net/member_illust.php?mode=medium&illust_id=66106354
+results[0].source_url     # Same as url for Pixiv results, but returns the linked original source URL for Booru entries
+results[0].index          # Pixiv
+```
+
+Video search results provide three additional properties containing the episode number, estimated timestamp, and release year
+```python
+from pysaucenao import SauceNao, VideoSource
+sauce = SauceNao()
+results = await sauce.from_url('https://i.imgur.com/1M8MhB0.png')
+
+if isinstance(results[0], VideoSource):
+    results[0].episode    # '1'
+    results[0].year       # '2017'
+    results[0].timestamp  # '00:07:53 / 00:23:40'
+```
+
+MangaSource search results, similarly, provide an additional `chapter` property.
+
+### Advanced usage
+
+#### Additional source URL's
+Thanks to [yuna.moe](https://github.com/BeeeQueue/arm-server), pysaucenao is no longer limited to just AniDB source URL's for anime results as of v1.3
+
+To utilize this new feature, you should first verify you are working with an Anime source.
+
+Once you have done that, you will need to preload the ID map by running the **load_ids** method.
+
+If you attempt to access any of the additional AnimeSource properties without first doing this, you will get an IndexError.
+```python
+from pysaucenao import SauceNao, AnimeSource
+sauce = SauceNao()
+results = await sauce.from_url('https://i.imgur.com/poAmgY0.png')
+
+if isinstance(results[0], AnimeSource):
+    await results[0].load_ids()
+```
+This will map the AniDB ID SauceNao returns with several other anime databases,
+```python
+results[0].title        # Made in Abyss
+results[0].anilist_id   # 97986
+results[0].anilist_url  # https://anilist.co/anime/97986
+results[0].mal_url      # https://myanimelist.net/anime/34599
+results[0].kitsu_url    # https://kitsu.io/anime/13273
+```
+
+#### Priority
+If you want to prioritize certain types of results, you can do so using the `priority` setting as of v1.2
+
+The most useful case for this is to prioritize anime results, preventing anime screencaps hosted on DeviantArt and other indexes some taking priority.
+
+To use this in your own code, just initialize SauceNao like so,
+```python
+sauce = SauceNao(priority=[21, 22])
+```
+As long as the anime search results are reasonably close to the next best match SauceNao returns, this will make sure the library always returns the anime result first, and ideally never a reposted screen-grab.
+
+If you need to prioritize other indexes, you can find a list of ID's here:
+https://github.com/FujiMakoto/pysaucenao/blob/master/pysaucenao/containers.py#L16-L50
+
+## Registering for an API key
+If you are performing lots of API queries, you will eventually need to sign up and register for an API key (and possibly upgrade your account for very large request volumes)
+
+You can register for an account on [SauceNAO's website](https://saucenao.com/user.php)
+
+## Error handling
+The SauceNao class will throw an exception if any of the following occur:
+* You have exceeded your 30-second search query limit (ShortLimitReachedException)
+* You have exceeded your 24-hour search query limit (DailyLimitReachedException)
+* You attempted to upload a file larger than SauceNAO allows (FileSizeLimitException)
+* You provided an invalid API key (InvalidOrWrongApiKeyException)
+* The image was too small for use (ImageSizeException)
+* Either the URL or file provided was not a valid image (InvalidImageException)
+* Too many failed requests made; try again later (TooManyFailedRequestsException)
+* Your account does not have API access; contact SauceNao support (BannedException)
+* Any other unknown error occurred / service may be down (UnknownStatusCodeException)
+
+All of these exceptions extend a base SauceNaoException class for easy catching and handling.
```

### Comparing `pysaucenao-1.6.1/pysaucenao/containers.py` & `pysaucenao-1.6.2/pysaucenao/containers.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     '35': 'Pawoo.net',
     '36': 'Madokami (Manga)',
     '37': 'MangaDex',
     '38': 'E-Hentai',
     '39': 'ArtStation',
     '40': 'FurAffinity',
     '41': 'Twitter',
-    '42': 'Furry Network'
+    '42': 'Furry Network',
+    '43': 'Fanbox'
 
 }
 
 
 class SauceNaoResults:
     """
     SauceNao results container
@@ -231,14 +232,15 @@
         self.header = header
         self.data   = data
 
         self.similarity:    typing.Optional[float] = None
         self.thumbnail:     typing.Optional[str] = None
         self.author_name:   typing.Optional[str] = None
         self.author_url:    typing.Optional[str] = None
+        self.authors:       typing.Optional[list] = None
         # self.created_at:    typing.Optional[datetime] = None
         self.title:         typing.Optional[str] = None
         self.url:           typing.Optional[str] = None
         self.urls:          typing.Optional[list] = None
         self.index:         typing.Optional[str] = None  # The name of the index pulled from. See INDEXES above
         self.index_id:      typing.Optional[int] = None
         self.index_name:    typing.Optional[str] = None
@@ -283,17 +285,26 @@
             self.title = data['material']
         elif 'source' in data:
             self.title = data['source']  # Sometimes this is a URL, sometimes it's a title. ¯\(°_o)/¯
 
         # Like above, author name can come from multiple fields
         if 'member_name' in data:
             self.author_name = data['member_name']
+            self.authors = [data['member_name']]
         elif 'creator' in data:
-            # May be multiple creators; we just grab the first in this scenario
-            self.author_name = data['creator'][0] if isinstance(data['creator'], list) else data['creator']
+            # May be multiple creators; we just grab the first in this scenario. All are stored in authors
+            if isinstance(data['creator'], list):
+                self.author_name = data['creator'][0]
+                self.authors = data['creator']
+            else:
+                self.author_name = data['creator']
+                self.authors = [data['creator']]
+        elif 'author_name' in data:
+            self.author_name = data['author_name']
+            self.authors = [data['author_name']]
 
         # Same story, different comment line
         if 'author_url' in data:
             self.author_url = data['author_url']
         elif 'pawoo_id' in data and 'ext_urls' in data:
             self.author_url = data['ext_urls'][0]
 
@@ -386,15 +397,15 @@
         Return the first source link
         """
 
         return self.url
 
     @property
     def type(self):
-        return TYPE_BOORU
+        return TYPE_GENERIC
 
     def _parse_data(self, data: dict):
         super()._parse_data(data)
 
         self.tweet_id: int = data['tweet_id']
         self.twitter_user_id: int = data['twitter_user_id']
         self.twitter_user_handle: str = data['twitter_user_handle']
@@ -543,15 +554,14 @@
 
 
 class MangaSource(GenericSource):
 
     def __init__(self, header: dict, data: dict):
 
         self.chapter:       typing.Optional[str] = None
-        self.author_name:   typing.Optional[str] = None
         super().__init__(header, data)
 
     @property
     def type(self):
         return TYPE_MANGA
 
     def _parse_data(self, data: dict):
@@ -562,14 +572,20 @@
         if 'eng_name' in data:
             self.title = data['eng_name']
         elif 'source' in data:
             self.title = data['source']
 
         if 'author' in data:
             self.author_name = data['author']
+            self.authors = [data['author']]
 
         elif 'creator' in data:
-            self.author_name = data['creator']
+            if isinstance(data['creator'], list):
+                self.author_name = data['creator'][0]
+                self.authors = data['creator']
+            else:
+                self.author_name = data['creator']
+                self.authors = [data['creator']]
 
     def __repr__(self):
         rep = reprlib.Repr()
         return f"<MangaSource(title={rep.repr(self.title)}, author={self.author_name} chapter={self.chapter}, source='{self.index}')>"
```

### Comparing `pysaucenao-1.6.1/pysaucenao/errors.py` & `pysaucenao-1.6.2/pysaucenao/errors.py`

 * *Files identical despite different names*

### Comparing `pysaucenao-1.6.1/pysaucenao/saucenao.py` & `pysaucenao-1.6.2/pysaucenao/saucenao.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import io
 from typing import *
 
+from aiohttp_proxy import ProxyConnector
+
 from pysaucenao.containers import *
 from pysaucenao.errors import *
 
 
 class SauceNao:
 
     API_URL = 'https://saucenao.com/search.php'
```

### Comparing `pysaucenao-1.6.1/setup.py` & `pysaucenao-1.6.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name='pysaucenao',  # How you named your package folder (MyLib)
         packages=['pysaucenao'],  # Chose the same as "name"
-        version='1.6.1',  # Start with a small number and increase it with every change you make
+        version='1.6.2',  # Start with a small number and increase it with every change you make
         license='gpl-3.0',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
         description='PySauceNao is an unofficial asynchronous library for the SauceNao API. It supports lookups via URL or from the local filesystem.',  # Give a short description about your library
         long_description=long_description,
         long_description_content_type='text/markdown',
         author='Makoto',  # Type in your name
         author_email='makoto+github@taiga.sh',  # Type in your E-Mail
         url='https://github.com/FujiMakoto/pysaucenao',  # Provide either the link to your github or to your website
-        download_url='https://github.com/FujiMakoto/pysaucenao/archive/1.6.1.tar.gz',
+        download_url='https://github.com/FujiMakoto/pysaucenao/archive/1.6.2.tar.gz',
         keywords=['saucenao', 'anime', 'artwork'],  # Keywords that define your package best
         install_requires=[
             'aiohttp',
             'aiohttp_proxy',
         ],
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

