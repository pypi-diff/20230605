# Comparing `tmp/libretrofuzz-2.9.1.tar.gz` & `tmp/libretrofuzz-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.1.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.2.tar", max compression
```

## Comparing `libretrofuzz-2.9.1.tar` & `libretrofuzz-2.9.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-05 08:07:17.800045 libretrofuzz-2.9.1/LICENSE
--rw-r--r--   0        0        0     7523 2023-06-05 08:07:17.800045 libretrofuzz-2.9.1/README.rst
--rw-r--r--   0        0        0       22 2023-06-05 08:07:17.800045 libretrofuzz-2.9.1/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    48649 2023-06-05 08:07:17.804045 libretrofuzz-2.9.1/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      972 2023-06-05 08:07:17.804045 libretrofuzz-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     8700 2023-06-05 08:07:33.115018 libretrofuzz-2.9.1/setup.py
--rw-r--r--   0        0        0     8711 2023-06-05 08:07:33.116015 libretrofuzz-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/LICENSE
+-rw-r--r--   0        0        0     7557 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/README.rst
+-rw-r--r--   0        0        0       22 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    49287 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      972 2023-06-05 08:44:41.480125 libretrofuzz-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8734 2023-06-05 08:44:50.953240 libretrofuzz-2.9.2/setup.py
+-rw-r--r--   0        0        0     8745 2023-06-05 08:44:50.954134 libretrofuzz-2.9.2/PKG-INFO
```

### Comparing `libretrofuzz-2.9.1/LICENSE` & `libretrofuzz-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.1/README.rst` & `libretrofuzz-2.9.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,18 @@
   
                         MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``
   
   --playlist <NAME libretro-fuzz only>
                         Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
-  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails. No-op with ``--no-image``.
-                        | [1<=x<=10]
-  --delay FLOAT         | Seconds to skip thumbnails download.
-                        | [1<=x<=10]
+  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
+                        | [1<=x<=30]
+  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
+                        | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
   --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--score 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
```

### Comparing `libretrofuzz-2.9.1/libretrofuzz/__main__.py` & `libretrofuzz-2.9.2/libretrofuzz/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 ###########################################
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
 ADDRESS='https://thumbnails.libretro.com'
 MAX_SCORE = 200
 MAX_RETRIES = 3
+MAX_WAIT_SECS = 30
 #00-1f are ascii control codes, rest is 'normal' illegal windows filename chars according to powershell + &
 forbidden = regex.compile( \
             r'[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008' + \
             r'\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015' + \
             r'\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]' \
             )
 #external terminal image viewer application
@@ -87,36 +88,45 @@
     Note, parts of server might still be available
     so this only stops a playlist in libretro-fuzzall'''
     def __init__(self):
         super().__init__()
 class StopDownload(Exception):
     def __init__(self):
         super().__init__()
+class ContinueDownload(Exception):
+    def __init__(self):
+        super().__init__()
 class StopProgram(Exception):
     def __init__(self):
         super().__init__()
 
 skip = False
 escape  = False
+enter = False
 def checkDownload():
     '''threading.get_native_id() in this and other acesses of these variables
        confirms all accesses are in synchronous functions on one thread so
        there is no need to use any lock, async or not.
     '''
     global skip
     global escape
+    global enter
     if escape:
         raise StopProgram()
     if skip:
         raise StopDownload()
+    if enter:
+        raise ContinueDownload()
 def checkEscape():
     '''only called when it doesn't matter if a escape will happen, usually at the start of a iteration or the preparation phase'''
     #so we can reset skip here, since it wont matter either way and will help remove false skip positives from the key event loop
     global skip
     skip = False
+    global enter
+    enter = False
     global escape
     if escape:
         raise StopProgram()
 @asynccontextmanager
 async def lock_keys() -> None:
     '''blocks key echoing for this console and recognizes most keys
        including many combinations, user kill still works, alt+tab...
@@ -134,28 +144,32 @@
        So then you should reset skip on the 'checkescape' function at the start of every iteration
     '''
     done = asyncio.Event()
     input = create_input()
     def keys_ready():
         global skip
         global escape
+        global enter
         #ctrl-c needs flush, so this chain
         for key_press in chain(input.read_keys(), input.flush_keys()):
             if key_press.key == 'escape' or key_press.key == 'c-c': #esc or control-c
                 escape = True
                 done.set()
+            elif key_press.key == 'c-m': #linefeed or the final result of enter on both unix and windows
+                enter = True
+                done.set()
             else:
                 skip = True
 
     with input.raw_mode():
         with input.attach(keys_ready):
             #ignore keys in buffer before we are ready
             input.read_keys()
             input.flush_keys()
-            typer.echo(typer.style(f'Press escape to quit, and most other non-meta keys to skip downloads', bold=True))
+            typer.echo(typer.style(f'Press escape to quit, enter to continue and most other non-meta keys to skip downloads', bold=True))
             yield done
 
 #----------------non contextual str manipulation------------------------
 ppatterns = { '()': regex.compile(r'\([^)(]*\)'), '[]': regex.compile(r'\[[^][]*\]') }
 def removeparenthesis(s, open_p='(', close_p=')'):
     nb_rep = 1
     key = open_p+close_p
@@ -174,15 +188,16 @@
     #last subtitle marker and everything there until the end (last because i noticed that 'subsubtitles' exist,
     #for instance, ultima 7 - part 1|2 - subtitle
     try:
       pattern = spatterns[subtitle_marker]
     except:
       pattern = regex.compile(rf'.*({subtitle_marker}.*)')
       spatterns[subtitle_marker] = pattern
-    subtitle = regex.search(pattern, regex.search(before_metadata, t).group(1) if no_meta else t)
+    name_without_meta = regex.search(before_metadata, t)
+    subtitle = regex.search(pattern, name_without_meta.group(1) if name_without_meta else t)
     if subtitle:
         t = t[0:subtitle.start(1)] + ' ' + t[subtitle.end(1):]
     return t
 
 def replacemany(our_str, to_be_replaced, replace_with):
     for nextchar in to_be_replaced:
         our_str = our_str.replace(nextchar, replace_with)
@@ -472,16 +487,16 @@
 
 #####################
 # Main programs code
 #####################
 def mainfuzzsingle(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
         playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
         system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
-        wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails. No-op with --no-image.'),
-        wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download.'),
+        wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
+        wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
         filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
         score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with --no-fail.'),
         nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
         nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
@@ -528,16 +543,16 @@
             raise typer.Exit(code=1)
         except StopProgram as e:
             error(f'Cancelled by user, exiting')
             raise typer.Exit()
     asyncio.run(runit(), debug=False)
 
 def mainfuzzall(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
-        wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails. No-op with --no-image.'),
-        wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download.'),
+        wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
+        wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
         filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
         score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with --no-fail.'),
         nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
         nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
@@ -758,17 +773,20 @@
             if filters:
               #nothing to download but we want to remove images that may be there in the case of --filter.
               for dirname in Thumbs._fields:
                 Path(thumbnails_dir,destination, dirname, name + '.png').unlink(missing_ok=True)
 
 async def printwait(wait : Optional[float], waiting_format: str):
     count = int(wait/0.1)
-    for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, colour='YELLOW', leave=False):
+    try:
+      for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, colour='YELLOW', leave=False):
         checkDownload()
         await asyncio.sleep(0.1)
+    except ContinueDownload as e:
+      pass
 
 async def download(client, url, destination, download_format, missing_format, waiting_format, first_wait, wait_before, max_retries):
     '''returns True if downloaded. To download, it must have waited, if first_wait is True. Exceptions may happen instead of returning False, but they
     are all caught outside the caller loop of thumbnail types that downloads, so the first_wait guard gets reset again and only waits once per game'''
     while True:
         try:
             async with client.stream('GET', url, timeout=15) as r:
```

### Comparing `libretrofuzz-2.9.1/pyproject.toml` & `libretrofuzz-2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.1"
+version = "2.9.2"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.9.1/setup.py` & `libretrofuzz-2.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.1',
+    'version': '2.9.2',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails. No-op with ``--no-image``.\n                        | [1<=x<=10]\n  --delay FLOAT         | Seconds to skip thumbnails download.\n                        | [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose             Shows the failures, score and normalized local and server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose             Shows the failures, score and normalized local and server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-2.9.1/PKG-INFO` & `libretrofuzz-2.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.1
+Version: 2.9.2
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -78,18 +78,18 @@
   
                         MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``
   
   --playlist <NAME libretro-fuzz only>
                         Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
-  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails. No-op with ``--no-image``.
-                        | [1<=x<=10]
-  --delay FLOAT         | Seconds to skip thumbnails download.
-                        | [1<=x<=10]
+  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
+                        | [1<=x<=30]
+  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
+                        | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
   --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--score 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
```

