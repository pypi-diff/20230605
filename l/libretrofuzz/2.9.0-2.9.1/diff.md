# Comparing `tmp/libretrofuzz-2.9.0.tar.gz` & `tmp/libretrofuzz-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.0.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.1.tar", max compression
```

## Comparing `libretrofuzz-2.9.0.tar` & `libretrofuzz-2.9.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/LICENSE
--rw-r--r--   0        0        0     7523 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/README.rst
--rw-r--r--   0        0        0       22 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    48377 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      952 2023-06-04 21:52:57.363755 libretrofuzz-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     8670 2023-06-04 21:53:06.673486 libretrofuzz-2.9.0/setup.py
--rw-r--r--   0        0        0     8667 2023-06-04 21:53:06.674465 libretrofuzz-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-05 08:07:17.800045 libretrofuzz-2.9.1/LICENSE
+-rw-r--r--   0        0        0     7523 2023-06-05 08:07:17.800045 libretrofuzz-2.9.1/README.rst
+-rw-r--r--   0        0        0       22 2023-06-05 08:07:17.800045 libretrofuzz-2.9.1/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    48649 2023-06-05 08:07:17.804045 libretrofuzz-2.9.1/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      972 2023-06-05 08:07:17.804045 libretrofuzz-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8700 2023-06-05 08:07:33.115018 libretrofuzz-2.9.1/setup.py
+-rw-r--r--   0        0        0     8711 2023-06-05 08:07:33.116015 libretrofuzz-2.9.1/PKG-INFO
```

### Comparing `libretrofuzz-2.9.0/LICENSE` & `libretrofuzz-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.0/README.rst` & `libretrofuzz-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.0/libretrofuzz/__main__.py` & `libretrofuzz-2.9.1/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from contextlib import asynccontextmanager, contextmanager
 from itertools import chain
 from struct import unpack
 import json
 import os
 import sys
 import io
-import re
+import regex
 import zlib
 import fnmatch
 import collections
 import shutil
 import unicodedata
 import asyncio
 import subprocess
@@ -45,17 +45,19 @@
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
 ADDRESS='https://thumbnails.libretro.com'
 MAX_SCORE = 200
 MAX_RETRIES = 3
 #00-1f are ascii control codes, rest is 'normal' illegal windows filename chars according to powershell + &
-forbidden = r'[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008' + \
+forbidden = regex.compile( \
+            r'[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008' + \
             r'\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015' + \
-            r'\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]'
+            r'\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]' \
+            )
 #external terminal image viewer application
 viewer = None
 
 if sys.platform == 'win32': #this is for 64 bits too
     #this order is to make 'portable' installs have priority in windows, a concept that doesn't exist in linux or macosx
     #these are the default 32 and 64 bits installer paths, since there is no way to know what the user choses, check the defaults only.
     CONFIG = Path(r'C:/RetroArch-Win64/retroarch.cfg')
@@ -149,51 +151,64 @@
             #ignore keys in buffer before we are ready
             input.read_keys()
             input.flush_keys()
             typer.echo(typer.style(f'Press escape to quit, and most other non-meta keys to skip downloads', bold=True))
             yield done
 
 #----------------non contextual str manipulation------------------------
-parenthesis_patterns = { '()': re.compile(r'\([^)(]*\)'), '[]': re.compile(r'\[[^][]*\]') }
+ppatterns = { '()': regex.compile(r'\([^)(]*\)'), '[]': regex.compile(r'\[[^][]*\]') }
 def removeparenthesis(s, open_p='(', close_p=')'):
     nb_rep = 1
     key = open_p+close_p
     try:
-      pattern = parenthesis_patterns[key]
+      pattern = ppatterns[key]
     except:
-      pattern =  re.compile(fr'\{open_p}[^{close_p}{open_p}]*\{close_p}')
-      parenthesis_patterns[key] = pattern
+      pattern =  regex.compile(fr'\{open_p}[^{close_p}{open_p}]*\{close_p}')
+      ppatterns[key] = pattern
     while (nb_rep):
-        (s, nb_rep) = re.subn(pattern, '', s)
+        (s, nb_rep) = regex.subn(pattern, '', s)
     return s
 
+spatterns = { ' - ': regex.compile(rf'.*( - .*)'), ': ': regex.compile(rf'.*(: .*)') }
+before_metadata = regex.compile(r'(^[^[({]*)')
+def nosubtitle_aux(t,subtitle_marker=' - '):
+    #last subtitle marker and everything there until the end (last because i noticed that 'subsubtitles' exist,
+    #for instance, ultima 7 - part 1|2 - subtitle
+    try:
+      pattern = spatterns[subtitle_marker]
+    except:
+      pattern = regex.compile(rf'.*({subtitle_marker}.*)')
+      spatterns[subtitle_marker] = pattern
+    subtitle = regex.search(pattern, regex.search(before_metadata, t).group(1) if no_meta else t)
+    if subtitle:
+        t = t[0:subtitle.start(1)] + ' ' + t[subtitle.end(1):]
+    return t
+
 def replacemany(our_str, to_be_replaced, replace_with):
     for nextchar in to_be_replaced:
         our_str = our_str.replace(nextchar, replace_with)
     return our_str
 
 def removefirst(name: str, suf: str):
     return name.replace(suf, '', 1)
 
 def removeprefix(name: str, pre: str):
     if name.startswith(pre):
         return name[len(pre):]
     return name
 
-
 #----------------Used to check the existence of a sixtel compatible terminal image viewer-------------------------------
 def which(executable):
     flips = shutil.which(executable)
     if not flips:
         flips = shutil.which(executable, path=os.path.dirname(__file__))
     if not flips:
         flips = shutil.which(executable, path=os.getcwd())
     return flips
 
-
 #-----------------------------------------------------------------------------------------------------------------------
 #The heart of the program, what orders titles to be 'more similar' or less to the local labels (after the normalization)
 #-----------------------------------------------------------------------------------------------------------------------
 class TitleScorer(object):
     def __init__(self):
         #rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way), so it uses internal api to prevent a possible early exit at == 100
         self._RF_ScorerPy = { 'get_scorer_flags': lambda **kwargs: {'optimal_score': MAX_SCORE, 'worst_score': 0, 'flags': (1 << 6)} }
@@ -215,37 +230,36 @@
             #3. 'current best score' includes the prefix, which this call can't include in 2.
             similarity = fuzz.token_set_ratio(s1,s2,processor=None,score_cutoff=0)
             #Combine the scorer with a common prefix heuristic to give priority to longer similar
             #names, this helps prevents false positives for shorter strings which token set ratio
             #is prone because it sets score to 100 if one string words are completely on the other.
             return min(MAX_SCORE-1,similarity + prefix)
 
-
 #-----------------------------------------------------------------------------------------------------------------------------
 # Normalization functions, part of the functions that change both local labels and remote names to be more similar to compare
 #-----------------------------------------------------------------------------------------------------------------------------
-camelcase_pattern = re.compile(r'([A-Z][^A-Z]*)')
+camelcase_pattern = regex.compile(r'(\p{Lu}\p{Ll}+)')
 #number sequences in the middle (not start or end) of a string that start with 0
-zero_lead_pattern = re.compile(r'([^\d])0+([1-9])')
+zero_lead_pattern = regex.compile(r'([^\d])0+([1-9])')
 def normalizer(t, nometa, hack):
     if nometa:
         t = removeparenthesis(t,'(',')')
     if not hack:
         t = removeparenthesis(t,'[',']')
     #change all common ascci symbol characters we aren't going to use after this (, and ')
     t = replacemany(t, '_()[]{}-.!?#"', ' ')
     #strips just because the user may have made a mistake naming the source
     #(or the replacement above introduce boundary spaces)
     t = t.strip()
     #remove any number leading 0, except at the end or the start of the string
     #where it is likely a important part of the name, not a file manager sort workaround
-    t = re.sub(zero_lead_pattern, r'\1\2', t)
+    t = regex.sub(zero_lead_pattern, r'\1\2', t)
     #CamelCaseNames for local labels are common when there are no spaces,
     #do this to normalize definite articles in normalization with spaces only (minimizes changes)
-    t = ' '.join([s.strip() for s in re.split(camelcase_pattern, t) if s])
+    t = ' '.join([s.strip() for s in regex.split(camelcase_pattern, t) if s])
     #normalize case
     t = t.lower()
     #beginning and end definite articles in several european languages (people move them)
     #make sure we're only removing the start and end forms with spaces
     t = removefirst(t, ', the')
     t = removeprefix(t, 'the ')
     t = removefirst(t, ', los')
@@ -307,28 +321,17 @@
     t = t.replace('ix',   '9')
     t = t.replace('x',   '10')
     t = t.replace('i',    '1')
     #remove diacritics (does nothing to asian languages diacritics, only for 2 to 1 character combinations)
     t = u''.join([c for c in unicodedata.normalize('NFKD', t) if not unicodedata.combining(c)])
     return t
 
-def nosubtitle_aux(t,subtitle_marker=' - '):
-    #Ignore metadata (but do not delete) and get the string before it
-    no_meta = re.search(r'(^[^[({]*)', t)
-    #last subtitle marker and everything there until the end (last because i noticed that 'subsubtitles' exist,
-    #for instance, ultima 7 - part 1|2 - subtitle
-    subtitle = re.search(rf'.*({subtitle_marker}.*)', no_meta.group(1) if no_meta else t)
-    if subtitle:
-        t = t[0:subtitle.start(1)] + ' ' + t[subtitle.end(1):]
-    return t
-
 def nosubtitle_normalizer(t, nometa, hack):
     return normalizer(nosubtitle_aux(t), nometa, hack)
 
-
 #---------------------------------------------------------------------------------
 # Initalization functions, since there are two main programs so the code is reused
 #---------------------------------------------------------------------------------
 class RzipReader(object):
     """used to abstract the libretro compressed playlist format"""
     def __init__(self, file_name):
         self.file_name = file_name
@@ -463,15 +466,14 @@
         error(f'Could not get the remote thumbnail system names, exiting: {err}')
         raise typer.Exit(code=1)
     if system and system not in SYSTEMS:
         error(f'The user provided system name {system} does not match any remote thumbnail system names')
         raise typer.Exit(code=1)
     return (playlist_dir, thumbnails_directory, sorted(PLAYLISTS), sorted(SYSTEMS))
 
-
 #####################
 # Main programs code
 #####################
 def mainfuzzsingle(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
         playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
         system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
         wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails. No-op with --no-image.'),
@@ -647,31 +649,31 @@
         #and the 'before' operation would have to find the index before the match to apply it after. A mess.
         
         nameaux = name
         
         #'before' has priority over subtitle removal
         if before:
             #Ignore metadata and get the string before it
-            no_meta = re.search(r'(^[^[({]*)', nameaux)
-            if no_meta:
-                before_index = no_meta.group(1).find(before)
+            name_without_meta = regex.search(before_metadata, nameaux)
+            if name_without_meta:
+                before_index = name_without_meta.group(1).find(before)
                 if before_index != -1:
                     nameaux = nameaux[0:before_index]
         
         #there is a second form of subtitles, which doesn't appear in the thumbnail server directly but can appear in linux game names
         #that can be more faithful to the real name. It uses the colon character, which is forbidden in windows and only applies to filenames.
         #Note that this does mean that if the servername has 'Name_ subtitle.png' and not 'Name - subtitle.png' there is less chance of a match,
         #but that is rarer on the server than the opposite.
         #not to mention that this only applies if the user signals 'no-subtitle', which presumably means they tried without it - which does match.
         if nosubtitle:
             nameaux = nosubtitle_aux(nameaux, ': ')
         
         #only the local names should have forbidden characters
-        name = re.sub(forbidden, '_', name )
-        nameaux = re.sub(forbidden, '_', nameaux )
+        name = regex.sub(forbidden, '_', name )
+        nameaux = regex.sub(forbidden, '_', nameaux )
 
         #unlike the server thumbnails, normalization wasn't done yet
         nameaux = norm(nameaux, nometa, hack)
         
         #operate on cache (to speed up by not applying normalization every iteration)
         #the normalization can make it so that the winner has the same score as the runner up(s) so to make sure we catch at least
         #two thumbnails for cases where that happens, we check both best scores if we can't find a thumb in a server directory
```

### Comparing `libretrofuzz-2.9.0/pyproject.toml` & `libretrofuzz-2.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.0"
+version = "2.9.1"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
@@ -13,14 +13,15 @@
 questionary = "^1.10.0"
 typer = {extras = ["all"], version = "^0.5.0"}
 rapidfuzz = "^2.4.2"
 httpx = "^0.23.0"
 tqdm = "^4.64.0"
 prompt_toolkit = "^3.0.30"
 pillow = "^9.2.0"
+regex = "^2023.6.3"
 
 
 [tool.poetry.scripts]
 libretro-fuzz = 'libretrofuzz.__main__:fuzzsingle'
 libretro-fuzzall = 'libretrofuzz.__main__:fuzzall'
 
 [tool.poetry.urls]
```

### Comparing `libretrofuzz-2.9.0/setup.py` & `libretrofuzz-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 install_requires = \
 ['beautifulsoup4>=4.10.0,<5.0.0',
  'httpx>=0.23.0,<0.24.0',
  'pillow>=9.2.0,<10.0.0',
  'prompt_toolkit>=3.0.30,<4.0.0',
  'questionary>=1.10.0,<2.0.0',
  'rapidfuzz>=2.4.2,<3.0.0',
+ 'regex>=2023.6.3,<2024.0.0',
  'tqdm>=4.64.0,<5.0.0',
  'typer[all]>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.0',
+    'version': '2.9.1',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails. No-op with ``--no-image``.\n                        | [1<=x<=10]\n  --delay FLOAT         | Seconds to skip thumbnails download.\n                        | [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose             Shows the failures, score and normalized local and server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-2.9.0/PKG-INFO` & `libretrofuzz-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.0
+Version: 2.9.1
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: pillow (>=9.2.0,<10.0.0)
 Requires-Dist: prompt_toolkit (>=3.0.30,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=2.4.2,<3.0.0)
+Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.5.0,<0.6.0)
 Project-URL: Bug Tracker, https://github.com/i30817/libretrofuzz/issues
 Project-URL: Repository, https://github.com/i30817/libretrofuzz
 Project-URL: documentation, https://github.com/i30817/libretrofuzz#readme
 Project-URL: homepage, https://github.com/i30817/libretrofuzz
 Description-Content-Type: text/x-rst
```

