# Comparing `tmp/libretrofuzz-2.9.2.tar.gz` & `tmp/libretrofuzz-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.2.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.3.tar", max compression
```

## Comparing `libretrofuzz-2.9.2.tar` & `libretrofuzz-2.9.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/LICENSE
--rw-r--r--   0        0        0     7557 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/README.rst
--rw-r--r--   0        0        0       22 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    49287 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      972 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/pyproject.toml
--rw-r--r--   0        0        0     8734 2023-06-05 08:44:50.953240 libretrofuzz-2.9.2/setup.py
--rw-r--r--   0        0        0     8745 2023-06-05 08:44:50.954134 libretrofuzz-2.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/LICENSE
+-rw-r--r--   0        0        0     7557 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/README.rst
+-rw-r--r--   0        0        0       22 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    49413 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      992 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/pyproject.toml
+-rw-r--r--   0        0        0     8761 2023-06-05 10:21:04.979077 libretrofuzz-2.9.3/setup.py
+-rw-r--r--   0        0        0     8786 2023-06-05 10:21:04.980087 libretrofuzz-2.9.3/PKG-INFO
```

### Comparing `libretrofuzz-2.9.2/LICENSE` & `libretrofuzz-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.2/README.rst` & `libretrofuzz-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.2/libretrofuzz/__main__.py` & `libretrofuzz-2.9.3/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,21 @@
 class StopProgram(Exception):
     def __init__(self):
         super().__init__()
 
 skip = False
 escape  = False
 enter = False
+
+@contextmanager
+def handleContinueDownload():
+  try:
+    yield
+  except ContinueDownload:
+    pass
 def checkDownload():
     '''threading.get_native_id() in this and other acesses of these variables
        confirms all accesses are in synchronous functions on one thread so
        there is no need to use any lock, async or not.
     '''
     global skip
     global escape
@@ -628,17 +635,15 @@
                tmpdir: Path,
                thumbnails_dir: Path,
                client: AsyncClient
                ):
     #not a error to pass a empty playlist
     if len(names) == 0:
         return
-    
     thumbs = Thumbs._make( await downloadgamenames(client, system) )
-    
     #before implies that the names of the playlists may be cut, so the hack and meta matching must be disabled
     if before:
         hack = False
         nometa = True
     #no-fail is equivalent to max fuzz
     if nofail:
         score = 0
@@ -773,20 +778,18 @@
             if filters:
               #nothing to download but we want to remove images that may be there in the case of --filter.
               for dirname in Thumbs._fields:
                 Path(thumbnails_dir,destination, dirname, name + '.png').unlink(missing_ok=True)
 
 async def printwait(wait : Optional[float], waiting_format: str):
     count = int(wait/0.1)
-    try:
+    with handleContinueDownload():
       for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, colour='YELLOW', leave=False):
         checkDownload()
         await asyncio.sleep(0.1)
-    except ContinueDownload as e:
-      pass
 
 async def download(client, url, destination, download_format, missing_format, waiting_format, first_wait, wait_before, max_retries):
     '''returns True if downloaded. To download, it must have waited, if first_wait is True. Exceptions may happen instead of returning False, but they
     are all caught outside the caller loop of thumbnail types that downloads, so the first_wait guard gets reset again and only waits once per game'''
     while True:
         try:
             async with client.stream('GET', url, timeout=15) as r:
@@ -801,16 +804,17 @@
                     typer.echo(missing_format + ' ' + url)
                     return False
                 with open(destination, 'w+b') as f:
                     if first_wait:
                         await printwait(wait_before, waiting_format)
                     with tqdm.wrapattr(f, 'write', total=length, dynamic_ncols=True, bar_format=download_format, colour='BLUE', leave=False) as w:
                         async for chunk in r.aiter_raw(4096):
+                          with handleContinueDownload():
                             checkDownload()
-                            w.write(chunk)
+                          w.write(chunk)
             return True
         except (RequestError,HTTPStatusError) as e:
             if max_retries <= 0:
                 error(f'Download max retries exceeded, exiting')
                 raise typer.Exit(code=1)
             max_retries -= 1
```

### Comparing `libretrofuzz-2.9.2/pyproject.toml` & `libretrofuzz-2.9.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.2"
+version = "2.9.3"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 beautifulsoup4 = "^4.10.0"
 questionary = "^1.10.0"
 typer = {extras = ["all"], version = "^0.5.0"}
 rapidfuzz = "^2.4.2"
 httpx = "^0.23.0"
-tqdm = "^4.64.0"
+tqdm = "^4.65.0"
 prompt_toolkit = "^3.0.30"
 pillow = "^9.2.0"
 regex = "^2023.6.3"
+colorama = "^0.4.6"
 
 
 [tool.poetry.scripts]
 libretro-fuzz = 'libretrofuzz.__main__:fuzzsingle'
 libretro-fuzzall = 'libretrofuzz.__main__:fuzzall'
 
 [tool.poetry.urls]
```

### Comparing `libretrofuzz-2.9.2/setup.py` & `libretrofuzz-2.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 ['libretrofuzz']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.10.0,<5.0.0',
+ 'colorama>=0.4.6,<0.5.0',
  'httpx>=0.23.0,<0.24.0',
  'pillow>=9.2.0,<10.0.0',
  'prompt_toolkit>=3.0.30,<4.0.0',
  'questionary>=1.10.0,<2.0.0',
  'rapidfuzz>=2.4.2,<3.0.0',
  'regex>=2023.6.3,<2024.0.0',
- 'tqdm>=4.64.0,<5.0.0',
+ 'tqdm>=4.65.0,<5.0.0',
  'typer[all]>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.2',
+    'version': '2.9.3',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose             Shows the failures, score and normalized local and server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-2.9.2/PKG-INFO` & `libretrofuzz-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.2
+Version: 2.9.3
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: pillow (>=9.2.0,<10.0.0)
 Requires-Dist: prompt_toolkit (>=3.0.30,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=2.4.2,<3.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.5.0,<0.6.0)
 Project-URL: Bug Tracker, https://github.com/i30817/libretrofuzz/issues
 Project-URL: Repository, https://github.com/i30817/libretrofuzz
 Project-URL: documentation, https://github.com/i30817/libretrofuzz#readme
 Project-URL: homepage, https://github.com/i30817/libretrofuzz
 Description-Content-Type: text/x-rst
```

