# Comparing `tmp/muxtools-0.0.3.tar.gz` & `tmp/muxtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muxtools-0.0.3.tar", last modified: Sun Jun  4 11:22:49 2023, max compression
+gzip compressed data, was "muxtools-0.0.5.tar", last modified: Mon Jun  5 18:42:28 2023, max compression
```

## Comparing `muxtools-0.0.3.tar` & `muxtools-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.110119 muxtools-0.0.3/
--rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1115 2023-06-04 11:22:49.110119 muxtools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-27 13:25:07.000000 muxtools-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.077110 muxtools-0.0.3/muxtools/
--rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.095115 muxtools-0.0.3/muxtools/audio/
--rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.3/muxtools/audio/__init__.py
--rw-rw-rw-   0        0        0    11068 2023-06-03 01:30:34.000000 muxtools-0.0.3/muxtools/audio/audioutils.py
--rw-rw-rw-   0        0        0    14858 2023-06-04 10:23:26.000000 muxtools-0.0.3/muxtools/audio/encoders.py
--rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.3/muxtools/audio/extractors.py
--rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.3/muxtools/audio/memecoders.py
--rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.3/muxtools/audio/tools.py
--rw-rw-rw-   0        0        0     7680 2023-06-01 16:53:16.000000 muxtools-0.0.3/muxtools/cli.py
--rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.3/muxtools/functions.py
--rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/main.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.096115 muxtools-0.0.3/muxtools/misc/
--rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.3/muxtools/misc/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/misc/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.099116 muxtools-0.0.3/muxtools/muxing/
--rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/muxing/__init__.py
--rw-rw-rw-   0        0        0     4386 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/muxing/mux.py
--rw-rw-rw-   0        0        0     4403 2023-06-03 01:13:02.000000 muxtools-0.0.3/muxtools/muxing/muxfiles.py
--rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/muxing/tmdb.py
--rw-rw-rw-   0        0        0     6836 2023-06-04 10:19:37.000000 muxtools-0.0.3/muxtools/muxing/tracks.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.102116 muxtools-0.0.3/muxtools/subtitle/
--rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/subtitle/__init__.py
--rw-rw-rw-   0        0        0     1621 2023-06-04 10:32:35.000000 muxtools-0.0.3/muxtools/subtitle/font.py
--rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/subtitle/styles.py
--rw-rw-rw-   0        0        0    19594 2023-06-04 10:24:58.000000 muxtools-0.0.3/muxtools/subtitle/sub.py
--rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/subtitle/subutils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.109120 muxtools-0.0.3/muxtools/utils/
--rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/convert.py
--rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.3/muxtools/utils/download.py
--rw-rw-rw-   0        0        0     1449 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/env.py
--rw-rw-rw-   0        0        0     5357 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/files.py
--rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/format.py
--rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/glob.py
--rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/utils/log.py
--rw-rw-rw-   0        0        0     8153 2023-06-04 11:20:52.000000 muxtools-0.0.3/muxtools/utils/parsing.py
--rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.3/muxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.091114 muxtools-0.0.3/muxtools.egg-info/
--rw-rw-rw-   0        0        0     1115 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1335 2023-06-04 11:22:12.000000 muxtools-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 11:22:49.110119 muxtools-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.639931 muxtools-0.0.5/
+-rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1115 2023-06-05 18:42:28.638931 muxtools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-27 13:25:07.000000 muxtools-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.604832 muxtools-0.0.5/muxtools/
+-rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.623841 muxtools-0.0.5/muxtools/audio/
+-rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.5/muxtools/audio/__init__.py
+-rw-rw-rw-   0        0        0    11068 2023-06-03 01:30:34.000000 muxtools-0.0.5/muxtools/audio/audioutils.py
+-rw-rw-rw-   0        0        0    14858 2023-06-04 10:23:26.000000 muxtools-0.0.5/muxtools/audio/encoders.py
+-rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.5/muxtools/audio/extractors.py
+-rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.5/muxtools/audio/memecoders.py
+-rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.5/muxtools/audio/tools.py
+-rw-rw-rw-   0        0        0     7680 2023-06-01 16:53:16.000000 muxtools-0.0.5/muxtools/cli.py
+-rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.5/muxtools/functions.py
+-rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.624841 muxtools-0.0.5/muxtools/misc/
+-rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.5/muxtools/misc/__init__.py
+-rw-rw-rw-   0        0        0     7596 2023-06-04 11:54:07.000000 muxtools-0.0.5/muxtools/misc/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.628841 muxtools-0.0.5/muxtools/muxing/
+-rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/muxing/__init__.py
+-rw-rw-rw-   0        0        0     4718 2023-06-04 21:27:11.000000 muxtools-0.0.5/muxtools/muxing/mux.py
+-rw-rw-rw-   0        0        0     4403 2023-06-03 01:13:02.000000 muxtools-0.0.5/muxtools/muxing/muxfiles.py
+-rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/muxing/tmdb.py
+-rw-rw-rw-   0        0        0     6836 2023-06-04 10:19:37.000000 muxtools-0.0.5/muxtools/muxing/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.631842 muxtools-0.0.5/muxtools/subtitle/
+-rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/subtitle/__init__.py
+-rw-rw-rw-   0        0        0     1621 2023-06-04 10:32:35.000000 muxtools-0.0.5/muxtools/subtitle/font.py
+-rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.5/muxtools/subtitle/styles.py
+-rw-rw-rw-   0        0        0    20827 2023-06-04 13:49:24.000000 muxtools-0.0.5/muxtools/subtitle/sub.py
+-rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.5/muxtools/subtitle/subutils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.637931 muxtools-0.0.5/muxtools/utils/
+-rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/convert.py
+-rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.5/muxtools/utils/download.py
+-rw-rw-rw-   0        0        0     1468 2023-06-04 13:18:33.000000 muxtools-0.0.5/muxtools/utils/env.py
+-rw-rw-rw-   0        0        0     5357 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/files.py
+-rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/format.py
+-rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/glob.py
+-rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.5/muxtools/utils/log.py
+-rw-rw-rw-   0        0        0     8153 2023-06-04 11:20:52.000000 muxtools-0.0.5/muxtools/utils/parsing.py
+-rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.5/muxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.619063 muxtools-0.0.5/muxtools.egg-info/
+-rw-rw-rw-   0        0        0     1115 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1335 2023-06-05 18:41:01.000000 muxtools-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 18:42:28.639931 muxtools-0.0.5/setup.cfg
```

### Comparing `muxtools-0.0.3/LICENSE` & `muxtools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/PKG-INFO` & `muxtools-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.3
+Version: 0.0.5
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.3/muxtools/__init__.py` & `muxtools-0.0.5/muxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/audio/audioutils.py` & `muxtools-0.0.5/muxtools/audio/audioutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/audio/encoders.py` & `muxtools-0.0.5/muxtools/audio/encoders.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/audio/extractors.py` & `muxtools-0.0.5/muxtools/audio/extractors.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/audio/memecoders.py` & `muxtools-0.0.5/muxtools/audio/memecoders.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/audio/tools.py` & `muxtools-0.0.5/muxtools/audio/tools.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/cli.py` & `muxtools-0.0.5/muxtools/cli.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/functions.py` & `muxtools-0.0.5/muxtools/functions.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/main.py` & `muxtools-0.0.5/muxtools/main.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/misc/chapters.py` & `muxtools-0.0.5/muxtools/misc/chapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 from ..utils.log import error, info
 from ..utils.glob import GlobSearch
 from ..utils.download import get_executable
 from ..utils.types import Chapter, PathLike
 from ..utils.parsing import parse_ogm, parse_xml
-from ..utils.files import clean_temp_files, ensure_path_exists
+from ..utils.files import clean_temp_files, ensure_path_exists, ensure_path
 from ..utils.env import get_temp_workdir, get_workdir, run_commandline
 from ..utils.convert import format_timedelta, frame_to_timedelta, timedelta_to_frame
 
 __all__ = ["Chapters"]
 
 
 class Chapters:
@@ -153,21 +153,23 @@
         """
         info("Chapters:")
         for time, name in self.chapters:
             print(f"{name}: {format_timedelta(time)} | {timedelta_to_frame(time, self.fps)}")
         print("", end="\n")
         return self
 
-    def to_file(self, out: PathLike = get_workdir()) -> str:
+    def to_file(self, out: PathLike | None = None) -> str:
         """
         Outputs the chapters to an OGM file
 
         :param out:     Can be either a directory or a full file path
         """
-        out = out.resolve() if isinstance(out, Path) else Path(out).resolve()
+        if not out:
+            out = get_workdir()
+        out = ensure_path(out, self)
         if out.is_dir():
             out_file = os.path.join(out, "chapters.txt")
         else:
             out_file = out
         with open(out_file, "w", encoding="UTF-8") as f:
             f.writelines(
                 [
```

### Comparing `muxtools-0.0.3/muxtools/muxing/mux.py` & `muxtools-0.0.5/muxtools/muxing/mux.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 from ..utils.files import ensure_path, ensure_path_exists, get_crc32
 from ..utils.env import get_setup_attr, get_workdir, run_commandline
 
 __all__ = ["mux"]
 
 
 def mux(*tracks, tmdb: TmdbConfig | None = None, outfile: PathLike | None = None, quiet: bool = True) -> PathLike:
+    """
+    Runs the mux.
+
+    :param *tracks:     Any amount of track objects and a Chapters object
+    :param tmdb:        A TMDB Config used for additional tagging if you so desire.
+    :param outfile:     If you want to overwrite the output file path
+    :param quiet:       Whether or not to print the mkvmerge output
+    """
+
     tracks = list(tracks)
     show_name = get_setup_attr("show_name", "Example")
     out_name = get_setup_attr("out_name", R"$show$ - $ep$ (premux)")
     out_dir = ensure_path(get_setup_attr("out_dir", "premux"), "Mux")
     mkv_title_naming = get_setup_attr("mkv_title_naming", R"$show$ - $ep$")
     args: list[str] = [get_executable("mkvmerge")]
     episode = get_setup_attr("episode", "01")
```

### Comparing `muxtools-0.0.3/muxtools/muxing/muxfiles.py` & `muxtools-0.0.5/muxtools/muxing/muxfiles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/muxing/tmdb.py` & `muxtools-0.0.5/muxtools/muxing/tmdb.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/muxing/tracks.py` & `muxtools-0.0.5/muxtools/muxing/tracks.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/subtitle/font.py` & `muxtools-0.0.5/muxtools/subtitle/font.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/subtitle/styles.py` & `muxtools-0.0.5/muxtools/subtitle/styles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/subtitle/sub.py` & `muxtools-0.0.5/muxtools/subtitle/sub.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from pathlib import Path
 from typing import Self
 import shutil
 import json
 import re
 import os
 
-
 from .subutils import dummy_video, has_arch_resampler
 from ..utils.glob import GlobSearch
 from ..utils.download import get_executable
 from ..utils.types import PathLike, TrackType
 from ..utils.log import debug, error, info, warn
 from ..utils.convert import frame_to_timedelta, timedelta_to_frame
 from ..utils.env import get_temp_workdir, get_workdir, run_commandline
-from ..utils.files import ensure_path_exists, get_absolute_track, make_output, clean_temp_files
+from ..utils.files import ensure_path_exists, get_absolute_track, make_output, clean_temp_files, uniquify_path
 from ..muxing.muxfiles import MuxingFile
 
+__all__ = ["FontFile", "SubFile", "DEFAULT_DIALOGUE_STYLES"]
+
+
 DEFAULT_DIALOGUE_STYLES = ["default", "main", "alt", "overlap", "flashback", "top", "italics"]
 
 
 @dataclass
 class FontFile(MuxingFile):
     pass
 
@@ -438,14 +440,48 @@
                 raise error("Failed to resample perspective of subtitles!", self)
 
         self.file.unlink(True)
         self.file = shutil.copy(output, self.file)
         clean_temp_files()
         return self
 
+    def separate_signs(self, styles: list[str] = DEFAULT_DIALOGUE_STYLES) -> Self:
+        """
+        Basically deletes lines that have any of the passed styles.
+
+        :param styles:      List of style names to get rid of
+        """
+        doc = self._read_doc()
+        events = []
+        for line in doc.events:
+            skip = False
+            for style in styles:
+                if str(line.style).strip().casefold() == style.strip().casefold():
+                    skip = True
+                    break
+
+            if skip:
+                continue
+            events.append(line)
+        doc.events = events
+        self.__update_doc(doc)
+        return self.clean_styles()
+
+    def copy(self) -> "SubFile":
+        """
+        Creates a new copy of the current SubFile object, including its file.
+        So you can run anything on the new one without impacting the other one.
+        """
+        doc = self._read_doc()
+        new_path = uniquify_path(self.file)
+        with open(new_path, "w", encoding=self.encoding) as writer:
+            doc.dump_file(writer)
+
+        return SubFile(new_path, self.container_delay, self.source)
+
     @staticmethod
     def from_mkv(file: PathLike, track: int = 0, preserve_delay: bool = False, quiet: bool = True) -> "SubFile":
         """
         Extract subtitle from mkv.
 
         :param file:            Input mkv file
         :param track:           Relative track number
```

### Comparing `muxtools-0.0.3/muxtools/subtitle/subutils.py` & `muxtools-0.0.5/muxtools/subtitle/subutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/convert.py` & `muxtools-0.0.5/muxtools/utils/convert.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/download.py` & `muxtools-0.0.5/muxtools/utils/download.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/env.py` & `muxtools-0.0.5/muxtools/utils/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import json
 import subprocess
 from pathlib import Path
 
 from ..main import Setup
 
-__all__ = ["save_setup", "get_setup_attr", "get_workdir", "get_temp_workdir", "is_debug", "download_allowed"]
+__all__ = ["save_setup", "get_setup_attr", "get_workdir", "get_temp_workdir", "is_debug", "download_allowed", "run_commandline"]
 
 
 def save_setup(setup: Setup):
     os.environ["vof_setup"] = setup._toJson()
 
 
 def get_setup_attr(attr: str, default: any = None) -> any:
```

### Comparing `muxtools-0.0.3/muxtools/utils/files.py` & `muxtools-0.0.5/muxtools/utils/files.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/format.py` & `muxtools-0.0.5/muxtools/utils/format.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/glob.py` & `muxtools-0.0.5/muxtools/utils/glob.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/log.py` & `muxtools-0.0.5/muxtools/utils/log.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/parsing.py` & `muxtools-0.0.5/muxtools/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools/utils/types.py` & `muxtools-0.0.5/muxtools/utils/types.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/muxtools.egg-info/PKG-INFO` & `muxtools-0.0.5/muxtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.3
+Version: 0.0.5
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.3/muxtools.egg-info/SOURCES.txt` & `muxtools-0.0.5/muxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.3/pyproject.toml` & `muxtools-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "muxtools"
-version = "0.0.3"
+version = "0.0.5"
 description = "A library for various muxing and automation tools for anything and everything fansubbing related"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "requests>=2.31.0",
     "fontcollector>=2.1.0",
```

