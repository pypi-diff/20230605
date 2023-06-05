# Comparing `tmp/xklb-1.29.8.tar.gz` & `tmp/xklb-1.30.2.tar.gz`

## Comparing `xklb-1.29.8.tar` & `xklb-1.30.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.8/.gitattributes
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 xklb-1.29.8/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.8/Windows.md
--rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.8/pdm.lock
--rw-r--r--   0        0        0    19065 2020-02-02 00:00:00.000000 xklb-1.29.8/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.8/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/__init__.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/books.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/consts.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/dl_config.py
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/dl_extract.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/gui.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/hn_extract.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/lb.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/playback.py
--rw-r--r--   0        0        0    33325 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/player.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/praw_extract.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/search.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/subtitle.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tabs_extract.py
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tube_backend.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tube_extract.py
--rw-r--r--   0        0        0    61617 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/usage.py
--rw-r--r--   0        0        0    33490 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/history.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.8/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.8/LICENSE
--rw-r--r--   0        0        0    83918 2020-02-02 00:00:00.000000 xklb-1.29.8/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.8/pyproject.toml
--rw-r--r--   0        0        0    87514 2020-02-02 00:00:00.000000 xklb-1.29.8/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.2/.gitattributes
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 xklb-1.30.2/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.2/Windows.md
+-rw-r--r--   0        0        0   489912 2020-02-02 00:00:00.000000 xklb-1.30.2/pdm.lock
+-rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 xklb-1.30.2/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.2/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/__init__.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/books.py
+-rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/consts.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/dl_config.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/lb.py
+-rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/play_actions.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/playback.py
+-rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/player.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/search.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    22742 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tube_extract.py
+-rw-r--r--   0        0        0    77169 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/usage.py
+-rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.2/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.2/LICENSE
+-rw-r--r--   0        0        0    99455 2020-02-02 00:00:00.000000 xklb-1.30.2/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.2/pyproject.toml
+-rw-r--r--   0        0        0   103051 2020-02-02 00:00:00.000000 xklb-1.30.2/PKG-INFO
```

### Comparing `xklb-1.29.8/Windows.md` & `xklb-1.30.2/Windows.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 local media subcommands:
   fsadd [extract, xr]                Create a local media database; Add folders
   listen [lt]                        Listen to local media
   watch [wt]                         Watch local media
 ```
 
-Optional: xklb[full] deps: `choco install exiftool rust`
+Optional: xklb[deluxe] deps: `choco install exiftool rust`
 
 <details>
   <summary><h3>Alternative environment: msys2</h3></summary>
-  
+
 `cygwin`, `WSL`, or `WSL2` is not recommended.
 
 1. Install [msys2](https://www.msys2.org/) and ConEmu
 
     ```powershell
     choco install msys2 conemu
     ```
@@ -46,15 +46,15 @@
 
 3. Install build tools, mpv, fish, and python
 
     ```bash
     pacman -S mingw-w64-x86_64-mpv mingw-w64-x86_64-youtube-dl make automake python-pip python-wheel fish
     ```
 
-    Optional: xklb[full] deps:
+    Optional: xklb[deluxe] deps:
 
     ```bash
     choco install exiftool
     pacman -S mingw-w64-x86_64-rust
     ```
 
 4. **Configure ConEmu to use fish shell** in msys2
@@ -62,10 +62,10 @@
     https://superuser.com/questions/1024301/conemu-how-to-call-msys2-as-tab
 
 5. Set the [MSYSTEM](https://www.msys2.org/docs/environments/) environment variable and close and restart your shell
 
     ```fish
     set -Ux MSYSTEM MINGW64
     ```
-  
+
 </details>
```

### Comparing `xklb-1.29.8/pdm.lock` & `xklb-1.30.2/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -494,15 +494,15 @@
 summary = "Python port of markdown-it. Markdown parsing, done right!"
 dependencies = [
     "mdurl~=0.1",
 ]
 
 [[package]]
 name = "markupsafe"
-version = "2.1.2"
+version = "2.1.3"
 requires_python = ">=3.7"
 summary = "Safely add untrusted strings to HTML/XML markup."
 
 [[package]]
 name = "matplotlib-inline"
 version = "0.1.6"
 requires_python = ">=3.5"
@@ -557,15 +557,15 @@
 name = "olefile"
 version = "0.46"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Python package to parse, read and write Microsoft OLE2 files (Structured Storage or Compound Document, Microsoft Office)"
 
 [[package]]
 name = "orjson"
-version = "3.8.14"
+version = "3.9.0"
 requires_python = ">=3.7"
 summary = "Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy"
 
 [[package]]
 name = "packaging"
 version = "23.1"
 requires_python = ">=3.7"
@@ -852,15 +852,15 @@
 [[package]]
 name = "rebulk"
 version = "3.2.0"
 summary = "Rebulk - Define simple search patterns in bulk to perform advanced matching on any string."
 
 [[package]]
 name = "regex"
-version = "2023.5.5"
+version = "2023.6.3"
 requires_python = ">=3.6"
 summary = "Alternative regular expression module, to replace re."
 
 [[package]]
 name = "requests"
 version = "2.24.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
@@ -870,15 +870,15 @@
     "chardet<4,>=3.0.2",
     "idna<3,>=2.5",
     "urllib3!=1.25.0,!=1.25.1,<1.26,>=1.21.1",
 ]
 
 [[package]]
 name = "rich"
-version = "13.3.5"
+version = "13.4.1"
 requires_python = ">=3.7.0"
 summary = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 dependencies = [
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
@@ -1144,15 +1144,15 @@
 summary = "Typer, build great CLIs. Easy to code. Based on Python type hints."
 dependencies = [
     "click<9.0.0,>=7.1.1",
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.6.2"
+version = "4.6.3"
 requires_python = ">=3.7"
 summary = "Backported and Experimental Type Hints for Python 3.7+"
 
 [[package]]
 name = "tzdata"
 version = "2023.3"
 requires_python = ">=2"
@@ -1257,15 +1257,15 @@
     "mutagen",
     "pycryptodomex",
     "websockets",
 ]
 
 [[package]]
 name = "zeroconf"
-version = "0.63.0"
+version = "0.64.1"
 requires_python = ">=3.7,<4.0"
 summary = "A pure python implementation of multicast DNS service discovery"
 dependencies = [
     "async-timeout>=3.0.0; python_version < \"3.11\"",
     "ifaddr>=0.1.7",
 ]
 
@@ -2133,65 +2133,65 @@
     {url = "https://files.pythonhosted.org/packages/9a/a1/1352b0e5a3c71a79fa9265726e2217f69df9fd4de0bcb5725cc61f62a5df/Markdown-3.4.3-py3-none-any.whl", hash = "sha256:065fd4df22da73a625f14890dd77eb8040edcbd68794bcd35943be14490608b2"},
     {url = "https://files.pythonhosted.org/packages/9d/80/cc67bfb7deb973d5ae662ee6454d2dafaa8f7c106feafd0d1572666ebde5/Markdown-3.4.3.tar.gz", hash = "sha256:8bf101198e004dc93e84a12a7395e31aac6a9c9942848ae1d99b9d72cf9b3520"},
 ]
 "markdown-it-py 2.2.0" = [
     {url = "https://files.pythonhosted.org/packages/bf/25/2d88e8feee8e055d015343f9b86e370a1ccbec546f2865c98397aaef24af/markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
     {url = "https://files.pythonhosted.org/packages/e4/c0/59bd6d0571986f72899288a95d9d6178d0eebd70b6650f1bb3f0da90f8f7/markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
 ]
-"markupsafe 2.1.2" = [
-    {url = "https://files.pythonhosted.org/packages/02/2c/18d55e5df6a9ea33709d6c33e08cb2e07d39e20ad05d8c6fbf9c9bcafd54/MarkupSafe-2.1.2-cp310-cp310-win_amd64.whl", hash = "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156"},
-    {url = "https://files.pythonhosted.org/packages/04/cf/9464c3c41b7cdb8df660cda75676697e7fb49ce1be7691a1162fc88da078/MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc"},
-    {url = "https://files.pythonhosted.org/packages/06/3b/d026c21cd1dbee89f41127e93113dcf5fa85c6660d108847760b59b3a66d/MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4"},
-    {url = "https://files.pythonhosted.org/packages/0a/88/78cb3d95afebd183d8b04442685ab4c70cfc1138b850ba20e2a07aff2f53/MarkupSafe-2.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd"},
-    {url = "https://files.pythonhosted.org/packages/0d/15/82b108c697bec4c26c00aed6975b778cf0eac6cbb77598862b10550b7fcc/MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03"},
-    {url = "https://files.pythonhosted.org/packages/19/00/3b8eb0093c885576a1ce7f2263e7b8c01e55b9977433f8246f57cd81b0be/MarkupSafe-2.1.2-cp311-cp311-win32.whl", hash = "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625"},
-    {url = "https://files.pythonhosted.org/packages/1f/20/76f6337f1e7238a626ab34405ddd634636011b2ff947dcbd8995f16a7776/MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0"},
-    {url = "https://files.pythonhosted.org/packages/22/88/9c0cae2f5ada778182f2842b377dd273d6be689953345c10b165478831eb/MarkupSafe-2.1.2-cp39-cp39-win32.whl", hash = "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7"},
-    {url = "https://files.pythonhosted.org/packages/29/d2/243e6b860d97c18d848fc2bee2f39d102755a2b04a5ce4d018d839711b46/MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba"},
-    {url = "https://files.pythonhosted.org/packages/30/3e/0a69a24adb38df83e2f6989c38d68627a5f27181c82ecaa1fd03d1236dca/MarkupSafe-2.1.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601"},
-    {url = "https://files.pythonhosted.org/packages/34/19/64b0abc021b22766e86efee32b0e2af684c4b731ce8ac1d519c791800c13/MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036"},
-    {url = "https://files.pythonhosted.org/packages/37/b2/6f4d5cac75ba6fe9f17671304fe339ea45a73c5609b5f5e652aa79c915c8/MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7"},
-    {url = "https://files.pythonhosted.org/packages/39/8d/5c5ce72deb8567ab48a18fbd99dc0af3dd651b6691b8570947e54a28e0f3/MarkupSafe-2.1.2-cp37-cp37m-win_amd64.whl", hash = "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666"},
-    {url = "https://files.pythonhosted.org/packages/3d/66/2f636ba803fd6eb4cee7b3106ae02538d1e84a7fb7f4f8775c6528a87d31/MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323"},
-    {url = "https://files.pythonhosted.org/packages/41/54/6e88795c64ab5dcda31b06406c062c2740d1a64db18219d4e21fc90928c1/MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c"},
-    {url = "https://files.pythonhosted.org/packages/46/0c/10ee33673c5e36fa3809cf136971f81d951ca38516188ee11a965d9b2fe9/MarkupSafe-2.1.2-cp39-cp39-win_amd64.whl", hash = "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed"},
-    {url = "https://files.pythonhosted.org/packages/48/cc/d027612e17b56088cfccd2c8e083518995fcb25a7b4f17fc146362a0499d/MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"},
-    {url = "https://files.pythonhosted.org/packages/4b/34/dc837e5ad9e14634aac4342eb8b12a9be20a4f74f50cc0d765f7aa2fc1e3/MarkupSafe-2.1.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094"},
-    {url = "https://files.pythonhosted.org/packages/50/41/1442b693a40eb76d835ca2016e86a01479f17d7fd8288f9830f6790e366a/MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3"},
-    {url = "https://files.pythonhosted.org/packages/52/36/b35c577c884ea352fc0c1eaed9ca4946ffc22cc9c3527a70408bfa9e9496/MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f"},
-    {url = "https://files.pythonhosted.org/packages/56/0d/c9818629672a3368b773fa94597d79da77bdacc3186f097bb85023f785f6/MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460"},
-    {url = "https://files.pythonhosted.org/packages/5a/94/d056bf5dbadf7f4b193ee2a132b3d49ffa1602371e3847518b2982045425/MarkupSafe-2.1.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6"},
-    {url = "https://files.pythonhosted.org/packages/5e/f6/8eb8a5692c1986b6e863877b0b8a83628aff14e5fbfaf11d9522b532bd9d/MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1"},
-    {url = "https://files.pythonhosted.org/packages/66/21/dadb671aade8eb67ef96e0d8f90b1bd5e8cfb6ad9d8c7fa2c870ec0c257b/MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619"},
-    {url = "https://files.pythonhosted.org/packages/76/b5/05ce70a3e31ecebcd3628cd180dc4761293aa496db85170fdc085ed2d79a/MarkupSafe-2.1.2-cp38-cp38-win32.whl", hash = "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2"},
-    {url = "https://files.pythonhosted.org/packages/77/26/af46880038c6eac3832e751298f1965f3a550f38d1e9ddaabd674860076b/MarkupSafe-2.1.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd"},
-    {url = "https://files.pythonhosted.org/packages/78/e6/91c9a20a943ea231c59024e181c4c5480097daf132428f2272670974637f/MarkupSafe-2.1.2-cp310-cp310-win32.whl", hash = "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603"},
-    {url = "https://files.pythonhosted.org/packages/79/e2/b818bf277fa6b01244943498cb2127372c01dde5eff7682837cc72740618/MarkupSafe-2.1.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d"},
-    {url = "https://files.pythonhosted.org/packages/7b/0f/0e99c2f342933c43af69849a6ba63f2eef54e14c6d0e10a26470fb6b40a9/MarkupSafe-2.1.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a"},
-    {url = "https://files.pythonhosted.org/packages/7c/e6/454df09f18e0ea34d189b447a9e1a9f66c2aa332b77fd5577ebc7ca14d42/MarkupSafe-2.1.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2"},
-    {url = "https://files.pythonhosted.org/packages/80/64/ccb65aadd71e7685caa69a885885a673e8748525a243fb26acea37201b44/MarkupSafe-2.1.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54"},
-    {url = "https://files.pythonhosted.org/packages/82/70/b3978786c7b576c25d84b009d2a20a11b5300d252fc3ce984e37b932e97c/MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65"},
-    {url = "https://files.pythonhosted.org/packages/82/e3/4efcd74f10a7999783955aec36386f71082e6d7dafcc06b77b9df72b325a/MarkupSafe-2.1.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f"},
-    {url = "https://files.pythonhosted.org/packages/87/a1/d0f05a09c6c1aef89d1eea0ab0ff1ea897d4117d27f1571034a7e3ff515b/MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a"},
-    {url = "https://files.pythonhosted.org/packages/93/ca/1c3ae0c6a5712d4ba98610cada03781ea0448436b17d1dcd4759115b15a1/MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1"},
-    {url = "https://files.pythonhosted.org/packages/93/fa/d72f68f84f8537ee8aa3e0764d1eb11e5e025a5ca90c16e94a40f894c2fc/MarkupSafe-2.1.2-cp38-cp38-win_amd64.whl", hash = "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147"},
-    {url = "https://files.pythonhosted.org/packages/95/7e/68018b70268fb4a2a605e2be44ab7b4dd7ce7808adae6c5ef32e34f4b55a/MarkupSafe-2.1.2.tar.gz", hash = "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d"},
-    {url = "https://files.pythonhosted.org/packages/95/88/8c8cce021ac1b1eedde349c6a41f6c256da60babf95e572071361ff3f66b/MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a"},
-    {url = "https://files.pythonhosted.org/packages/96/92/a873b4a7fa20c2e30bffe883bb560330f3b6ce03aaf278f75f96d161935b/MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff"},
-    {url = "https://files.pythonhosted.org/packages/9d/80/8320f182d06a9b289b1a9f266f593feb91d3781c7e104bbe09e0c4c11439/MarkupSafe-2.1.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419"},
-    {url = "https://files.pythonhosted.org/packages/be/18/988e1913a40cc8eb725b1e073eacc130f7803a061577bdc0b9343eb3c696/MarkupSafe-2.1.2-cp37-cp37m-win32.whl", hash = "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859"},
-    {url = "https://files.pythonhosted.org/packages/c3/e5/42842a44bfd9ba2955c562b1139334a2f64cedb687e8969777fd07de42a9/MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2"},
-    {url = "https://files.pythonhosted.org/packages/c7/0e/22d0c8e6ee84414e251bd1bc555b2705af6b3fb99f0ba1ead2a0f51d423b/MarkupSafe-2.1.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa"},
-    {url = "https://files.pythonhosted.org/packages/cf/c1/d7596976a868fe3487212a382cc121358a53dc8e8d85ff2ee2c3d3b40f04/MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1"},
-    {url = "https://files.pythonhosted.org/packages/d1/10/ff89b23d4a24051c4e4f689b79ee06f230d7e9431445e24f5dd9d9a89730/MarkupSafe-2.1.2-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed"},
-    {url = "https://files.pythonhosted.org/packages/e3/a9/e366665c7eae59c9c9d34b747cd5a3994847719a2304e0c8dec8b604dd98/MarkupSafe-2.1.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013"},
-    {url = "https://files.pythonhosted.org/packages/e6/ff/d2378ca3cb3ac4a37af767b820b0f0bf3f5e9193a6acce0eefc379425c1c/MarkupSafe-2.1.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a"},
-    {url = "https://files.pythonhosted.org/packages/e9/c6/2da36728c1310f141395176556500aeedfdea8c2b02a3b72ba61b69280e8/MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513"},
-    {url = "https://files.pythonhosted.org/packages/ea/60/2400ba59cf2465fa136487ee7299f52121a9d04b2cf8539ad43ad10e70e8/MarkupSafe-2.1.2-cp311-cp311-win_amd64.whl", hash = "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3"},
-    {url = "https://files.pythonhosted.org/packages/f9/aa/ebcd114deab08f892b1d70badda4436dbad1747f9e5b72cffb3de4c7129d/MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65"},
+"markupsafe 2.1.3" = [
+    {url = "https://files.pythonhosted.org/packages/03/06/e72e88f81f8c91d4f488d21712d2d403fd644e3172eaadc302094377bc22/MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4"},
+    {url = "https://files.pythonhosted.org/packages/03/65/3473d2cb84bb2cda08be95b97fc4f53e6bcd701a2d50ba7b7c905e1e9273/MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636"},
+    {url = "https://files.pythonhosted.org/packages/10/b3/c2b0a61cc0e1d50dd8a1b663ba4866c667cb58fb35f12475001705001680/MarkupSafe-2.1.3-cp38-cp38-win32.whl", hash = "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5"},
+    {url = "https://files.pythonhosted.org/packages/12/b3/d9ed2c0971e1435b8a62354b18d3060b66c8cb1d368399ec0b9baa7c0ee5/MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
+    {url = "https://files.pythonhosted.org/packages/20/1d/713d443799d935f4d26a4f1510c9e61b1d288592fb869845e5cc92a1e055/MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
+    {url = "https://files.pythonhosted.org/packages/22/81/b5659e2b6ae1516495a22f87370419c1d79c8d853315e6cbe5172fc01a06/MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea"},
+    {url = "https://files.pythonhosted.org/packages/32/d4/ce98c4ca713d91c4a17c1a184785cc00b9e9c25699d618956c2b9999500a/MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9"},
+    {url = "https://files.pythonhosted.org/packages/3c/c8/74d13c999cbb49e3460bf769025659a37ef4a8e884de629720ab4e42dcdb/MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7"},
+    {url = "https://files.pythonhosted.org/packages/43/70/f24470f33b2035b035ef0c0ffebf57006beb2272cf3df068fc5154e04ead/MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc"},
+    {url = "https://files.pythonhosted.org/packages/43/ad/7246ae594aac948b17408c0ff0f9ff0bc470bdbe9c672a754310db64b237/MarkupSafe-2.1.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c"},
+    {url = "https://files.pythonhosted.org/packages/44/53/93405d37bb04a10c43b1bdd6f548097478d494d7eadb4b364e3e1337f0cc/MarkupSafe-2.1.3-cp311-cp311-win32.whl", hash = "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb"},
+    {url = "https://files.pythonhosted.org/packages/47/26/932140621773bfd4df3223fbdd9e78de3477f424f0d2987c313b1cb655ff/MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779"},
+    {url = "https://files.pythonhosted.org/packages/4d/e4/77bb622d6a37aeb51ee55857100986528b7f47d6dbddc35f9b404622ed50/MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc"},
+    {url = "https://files.pythonhosted.org/packages/4f/13/cf36eff21600fb21d5bd8c4c1b6ff0b7cc0ff37b955017210cfc6f367972/MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b"},
+    {url = "https://files.pythonhosted.org/packages/62/9b/4908a57acf39d8811836bc6776b309c2e07d63791485589acf0b6d7bc0c6/MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b"},
+    {url = "https://files.pythonhosted.org/packages/68/8d/c33c43c499c19f4b51181e196c9a497010908fc22c5de33551e298aa6a21/MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58"},
+    {url = "https://files.pythonhosted.org/packages/6a/86/654dc431513cd4417dfcead8102f22bece2d6abf2f584f0e1cc1524f7b94/MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198"},
+    {url = "https://files.pythonhosted.org/packages/6d/7c/59a3248f411813f8ccba92a55feaac4bf360d29e2ff05ee7d8e1ef2d7dbf/MarkupSafe-2.1.3.tar.gz", hash = "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad"},
+    {url = "https://files.pythonhosted.org/packages/71/61/f5673d7aac2cf7f203859008bb3fc2b25187aa330067c5e9955e5c5ebbab/MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6"},
+    {url = "https://files.pythonhosted.org/packages/74/a3/54fc60ee2da3ab6d68b1b2daf4897297c597840212ee126e68a4eb89fcd7/MarkupSafe-2.1.3-cp38-cp38-win_amd64.whl", hash = "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc"},
+    {url = "https://files.pythonhosted.org/packages/7d/48/6ba4db436924698ca22109325969e00be459d417830dafec3c1001878b57/MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e"},
+    {url = "https://files.pythonhosted.org/packages/84/a8/c4aebb8a14a1d39d5135eb8233a0b95831cdc42c4088358449c3ed657044/MarkupSafe-2.1.3-cp310-cp310-win_amd64.whl", hash = "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559"},
+    {url = "https://files.pythonhosted.org/packages/8b/bb/72ca339b012054a84753accabe3258e0baf6e34bd0ab6e3670b9a65f679d/MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8"},
+    {url = "https://files.pythonhosted.org/packages/8d/66/4a46c7f1402e0377a8b220fd4b53cc4f1b2337ab0d97f06e23acd1f579d1/MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee"},
+    {url = "https://files.pythonhosted.org/packages/96/e4/4db3b1abc5a1fe7295aa0683eafd13832084509c3b8236f3faf8dd4eff75/MarkupSafe-2.1.3-cp310-cp310-win32.whl", hash = "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431"},
+    {url = "https://files.pythonhosted.org/packages/9b/c1/9f44da5ca74f95116c644892152ca6514ecdc34c8297a3f40d886147863d/MarkupSafe-2.1.3-cp37-cp37m-win_amd64.whl", hash = "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24"},
+    {url = "https://files.pythonhosted.org/packages/a2/b2/624042cb58cc6b3529a6c3a7b7d230766e3ecb768cba118ba7befd18ed6f/MarkupSafe-2.1.3-cp39-cp39-win_amd64.whl", hash = "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba"},
+    {url = "https://files.pythonhosted.org/packages/a2/f7/9175ad1b8152092f7c3b78c513c1bdfe9287e0564447d1c2d3d1a2471540/MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee"},
+    {url = "https://files.pythonhosted.org/packages/a6/56/f1d4ee39e898a9e63470cbb7fae1c58cce6874f25f54220b89213a47f273/MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f"},
+    {url = "https://files.pythonhosted.org/packages/a8/12/fd9ef3e09a7312d60467c71037283553ff2acfcd950159cd4c3ca9558af4/MarkupSafe-2.1.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2"},
+    {url = "https://files.pythonhosted.org/packages/ab/20/f59423543a8422cb8c69a579ebd0ef2c9dafa70cc8142b7372b5b4073caa/MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e"},
+    {url = "https://files.pythonhosted.org/packages/b2/0d/cbaade3ee8efbd5ce2fb72b48cc51479ebf3d4ce2c54dcb6557d3ea6a950/MarkupSafe-2.1.3-cp37-cp37m-win32.whl", hash = "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0"},
+    {url = "https://files.pythonhosted.org/packages/b2/27/07e5aa9f93314dc65ad2ad9b899656dee79b70a9425ee199dd5a4c4cf2cd/MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3"},
+    {url = "https://files.pythonhosted.org/packages/bb/82/f88ccb3ca6204a4536cf7af5abdad7c3657adac06ab33699aa67279e0744/MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac"},
+    {url = "https://files.pythonhosted.org/packages/be/bb/08b85bc194034efbf572e70c3951549c8eca0ada25363afc154386b5390a/MarkupSafe-2.1.3-cp311-cp311-win_amd64.whl", hash = "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686"},
+    {url = "https://files.pythonhosted.org/packages/bf/b7/c5ba9b7ad9ad21fc4a60df226615cf43ead185d328b77b0327d603d00cc5/MarkupSafe-2.1.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00"},
+    {url = "https://files.pythonhosted.org/packages/c0/c7/171f5ac6b065e1425e8fabf4a4dfbeca76fd8070072c6a41bd5c07d90d8b/MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575"},
+    {url = "https://files.pythonhosted.org/packages/c9/80/f08e782943ee7ae6e9438851396d00a869f5b50ea8c6e1f40385f3e95771/MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d"},
+    {url = "https://files.pythonhosted.org/packages/d2/a1/4ae49dd1520c7b891ea4963258aab08fb2554c564781ecb2a9c4afdf9cb1/MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48"},
+    {url = "https://files.pythonhosted.org/packages/d5/c1/1177f712d4ab91eb67f79d763a7b5f9c5851ee3077d6b4eee15e23b6b93e/MarkupSafe-2.1.3-cp39-cp39-win32.whl", hash = "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"},
+    {url = "https://files.pythonhosted.org/packages/de/63/cb7e71984e9159ec5f45b5e81e896c8bdd0e45fe3fc6ce02ab497f0d790e/MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e"},
+    {url = "https://files.pythonhosted.org/packages/de/e2/32c14301bb023986dff527a49325b6259cab4ebb4633f69de54af312fc45/MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be"},
+    {url = "https://files.pythonhosted.org/packages/e5/dd/49576e803c0d974671e44fa78049217fcc68af3662a24f831525ed30e6c7/MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707"},
+    {url = "https://files.pythonhosted.org/packages/e6/5c/8ab8f67bbbbf90fe88f887f4fa68123435c5415531442e8aefef1e118d5c/MarkupSafe-2.1.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e"},
+    {url = "https://files.pythonhosted.org/packages/f4/a0/103f94793c3bf829a18d2415117334ece115aeca56f2df1c47fa02c6dbd6/MarkupSafe-2.1.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9"},
+    {url = "https://files.pythonhosted.org/packages/f7/9c/86cbd8e0e1d81f0ba420f20539dd459c50537c7751e28102dbfee2b6f28c/MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57"},
+    {url = "https://files.pythonhosted.org/packages/f8/33/e9e83b214b5f8d9a60b26e60051734e7657a416e5bce7d7f1c34e26badad/MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0"},
+    {url = "https://files.pythonhosted.org/packages/fa/bb/12fb5964c4a766eb98155dd31ec070adc8a69a395564ffc1e7b34d91335a/MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155"},
+    {url = "https://files.pythonhosted.org/packages/fe/09/c31503cb8150cf688c1534a7135cc39bb9092f8e0e6369ec73494d16ee0e/MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c"},
+    {url = "https://files.pythonhosted.org/packages/fe/21/2eff1de472ca6c99ec3993eab11308787b9879af9ca8bbceb4868cf4f2ca/MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2"},
 ]
 "matplotlib-inline 0.1.6" = [
     {url = "https://files.pythonhosted.org/packages/d9/50/3af8c0362f26108e54d58c7f38784a3bdae6b9a450bab48ee8482d737f44/matplotlib-inline-0.1.6.tar.gz", hash = "sha256:f887e5f10ba98e8d2b150ddcf4702c1e5f8b3a20005eb0f74bfdbd360ee6f304"},
     {url = "https://files.pythonhosted.org/packages/f2/51/c34d7a1d528efaae3d8ddb18ef45a41f284eacf9e514523b191b7d0872cc/matplotlib_inline-0.1.6-py3-none-any.whl", hash = "sha256:f1f41aab5328aa5aaea9b16d083b128102f8712542f819fe7e6a420ff581b311"},
 ]
 "mdurl 0.1.2" = [
     {url = "https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
@@ -2344,61 +2344,61 @@
     {url = "https://files.pythonhosted.org/packages/f0/e8/1ea9adebdccaadfc208c7517e09f5145ed5a73069779ff436393085d47a2/numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
     {url = "https://files.pythonhosted.org/packages/f3/23/7cc851bae09cf4db90d42a701dfe525780883ada86bece45e3da7a07e76b/numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
     {url = "https://files.pythonhosted.org/packages/fa/7d/8dfb40eecbb6bc83ca00ef979f5cdeca5909a250cb8b642dcf1fbd34c078/numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
 ]
 "olefile 0.46" = [
     {url = "https://files.pythonhosted.org/packages/34/81/e1ac43c6b45b4c5f8d9352396a14144bba52c8fec72a80f425f6a4d653ad/olefile-0.46.zip", hash = "sha256:133b031eaf8fd2c9399b78b8bc5b8fcbe4c31e85295749bb17a87cba8f3c3964"},
 ]
-"orjson 3.8.14" = [
-    {url = "https://files.pythonhosted.org/packages/03/bb/28d2ced376eebb93869eda6dbd7205597eb757220e39746bc088096b75f4/orjson-3.8.14-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:19415aaf30525a5baff0d72a089fcdd68f19a3674998263c885c3908228c1086"},
-    {url = "https://files.pythonhosted.org/packages/09/c6/4ba2bfc85dea2126a15b48933aa4e5dfaeaeac558808a83555c0c1af7831/orjson-3.8.14-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:e53bc5beb612df8ddddb065f079d3fd30b5b4e73053518524423549d61177f3f"},
-    {url = "https://files.pythonhosted.org/packages/10/32/c29c34bc0661277ea5493cfbe56a88746d5112c93db8990d25526f30b5e0/orjson-3.8.14-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:739f9f633e1544f2a477fa3bef380f488c8dca6e2521c8dc36424b12554ee31e"},
-    {url = "https://files.pythonhosted.org/packages/16/53/a961ea06b24422226df1e27158a5110b82cc8fa403a774a10323ce959e6d/orjson-3.8.14-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:04c70dc8ca79b0072a16d82f94b9d9dd6598a43dd753ab20039e9f7d2b14f017"},
-    {url = "https://files.pythonhosted.org/packages/1a/b7/983036df5ac56bbaaa91f34dbd2d0940998fbd259643cdd1c68b8db5714a/orjson-3.8.14-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:5fb66f0ac23e861b817c858515ac1f74d1cd9e72e3f82a5b2c9bae9f92286adc"},
-    {url = "https://files.pythonhosted.org/packages/1d/e5/2e39fe3ac903c0007984ac3a410b948e2c548853c6143510e06f4a8f56a8/orjson-3.8.14-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:27967be4c16bd09f4aeff8896d9be9cbd00fd72f5815d5980e4776f821e2f77c"},
-    {url = "https://files.pythonhosted.org/packages/21/17/3c75f22a4d8f120b13b23c46702a636e33bf6faefaca4833dd675d4df7c7/orjson-3.8.14-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:087c0dc93379e8ba2d59e9f586fab8de8c137d164fccf8afd5523a2137570917"},
-    {url = "https://files.pythonhosted.org/packages/25/44/1577b80174487557f04adf61c065c54bc90d77d29c0df0b440f0f289eb34/orjson-3.8.14-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7cb35dd3ba062c1d984d57e6477768ed7b62ed9260f31362b2d69106f9c60ebd"},
-    {url = "https://files.pythonhosted.org/packages/2a/60/f889bc75c6a8fc39f96499a71f8e69d7aa2fdc97193a45e707273c4d560f/orjson-3.8.14-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ebca14ae80814219ea3327e3dfa7ff618621ff335e45781fac26f5cd0b48f2b4"},
-    {url = "https://files.pythonhosted.org/packages/2d/cb/d54d87ae58c3a09038458f5ad5efe93b3ab2f3d956ac47156469181777ef/orjson-3.8.14-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:38ca39bae7fbc050332a374062d4cdec28095540fa8bb245eada467897a3a0bb"},
-    {url = "https://files.pythonhosted.org/packages/2f/3a/1e89459e59fbc81ca3d5ff3465c8c7c55670552c2e08b7e437b6f2a016a2/orjson-3.8.14-cp310-none-win_amd64.whl", hash = "sha256:0bf00c42333412a9338297bf888d7428c99e281e20322070bde8c2314775508b"},
-    {url = "https://files.pythonhosted.org/packages/31/b4/9a11ba173208354fe2f393e8b2ea8e7dcd41ec3e8d044eb4ba7a1e9e3b61/orjson-3.8.14-cp37-cp37m-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:de1ee13d6b6727ee1db38722695250984bae81b8fc9d05f1176c74d14b1322d9"},
-    {url = "https://files.pythonhosted.org/packages/38/f5/85fd06d179e9c2cf6d9b46fd19e0d22463167c8623ce2100edf7dd5c3e36/orjson-3.8.14-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:67a7e883b6f782b106683979ccc43d89b98c28a1f4a33fe3a22e253577499bb1"},
-    {url = "https://files.pythonhosted.org/packages/3a/bb/425f0d9d0373fe82bc839009e4fa6e560e6dd9b2bbb67bfa02fb3c44caff/orjson-3.8.14-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:33bc310da4ad2ffe8f7f1c9e89692146d9ec5aec2d1c9ef6b67f8dc5e2d63241"},
-    {url = "https://files.pythonhosted.org/packages/43/de/5cdf2a1a218468190685f9a9490f566cd9f6b1101d03ceeddeb7f5cde3e7/orjson-3.8.14-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9df820e6c8c84c52ec39ea2cc9c79f7999c839c7d1481a056908dce3b90ce9f9"},
-    {url = "https://files.pythonhosted.org/packages/4d/1c/e94425b29eaf3a34b58311d79ed2f2cc11caa7c838a60f59f9ecc5266625/orjson-3.8.14-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:aedba48264fe87e5060c0e9c2b28909f1e60626e46dc2f77e0c8c16939e2e1f7"},
-    {url = "https://files.pythonhosted.org/packages/4f/33/677d6ecec94e3ae639e0c5558dac64ea8b7fc08e48b986564773e6ea1245/orjson-3.8.14-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:062829b5e20cd8648bf4c11c3a5ee7cf196fa138e573407b5312c849b0cf354d"},
-    {url = "https://files.pythonhosted.org/packages/4f/54/7761dccc1a177f2259d291022c17d364340a061f5cb6d4133baa613b9efd/orjson-3.8.14-cp38-cp38-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:9f5cf61b6db68f213c805c55bf0aab9b4cb75a4e9c7f5bfbd4deb3a0aef0ec53"},
-    {url = "https://files.pythonhosted.org/packages/52/55/9f2277b6dbdba514889433ef892ad6735b15e774c69dcb6afde444439734/orjson-3.8.14-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:01640ab79111dd97515cba9fab7c66cb3b0967b0892cc74756a801ff681a01b6"},
-    {url = "https://files.pythonhosted.org/packages/5d/5e/4d5b1ea3bfde7595afa7ca57a16835e3cabe04cc3d624062048562b59e8e/orjson-3.8.14-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3ee09bfbf1d54c127d3061f6721a1a11d2ce502b50597c3d0d2e1bd2d235b764"},
-    {url = "https://files.pythonhosted.org/packages/6c/9b/7a7c65b44da3e405463bba712aac1ae5de77eca1b78ecd9a11c5c9b8ce43/orjson-3.8.14-cp38-none-win_amd64.whl", hash = "sha256:d03f29b0369bb1ab55c8a67103eb3a9675daaf92f04388568034fe16be48fa5d"},
-    {url = "https://files.pythonhosted.org/packages/6c/a4/a616e36bec0ca0e55a26b72b1e735a64d6c0d5203eabdcde4cd3498e802b/orjson-3.8.14-cp311-cp311-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:d66966fd94719beb84e8ed84833bc59c3c005d3d2d0c42f11d7552d3267c6de7"},
-    {url = "https://files.pythonhosted.org/packages/6e/ca/c50071a746ef136b4c120f4ec60d19d146b55c73301ba85058b161c40c87/orjson-3.8.14-cp37-none-win_amd64.whl", hash = "sha256:87ba7882e146e24a7d8b4a7971c20212c2af75ead8096fc3d55330babb1015fb"},
-    {url = "https://files.pythonhosted.org/packages/74/69/38b4676e007ae513499ab6fbe7260d7bfd2ea668b06d4d6c64e39293455f/orjson-3.8.14-cp311-none-win_amd64.whl", hash = "sha256:20b7ffc7736000ea205f9143df322b03961f287b4057606291c62c842ff3c5b5"},
-    {url = "https://files.pythonhosted.org/packages/8f/38/3d5630a9fa808d15f8c76de2a6318c45f3ad12c5dc3680572c6b3bd53e61/orjson-3.8.14-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:bf6825e160e4eb0ef65ce37d8c221edcab96ff2ffba65e5da2437a60a12b3ad1"},
-    {url = "https://files.pythonhosted.org/packages/90/20/73b99827beea76722b8b2a20b7b0b4003d267912b4f94f6933529d583e89/orjson-3.8.14-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:7e2f75b7d9285e35c3d4dff9811185535ff2ea637f06b2b242cb84385f8ffe63"},
-    {url = "https://files.pythonhosted.org/packages/94/7d/87bbb5e4d6368c6a7463ec60683cef924e6f60c1c167a8bada89d5e77137/orjson-3.8.14-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:92374bc35b6da344a927d5a850f7db80a91c7b837de2f0ea90fc870314b1ff44"},
-    {url = "https://files.pythonhosted.org/packages/9e/56/b2327648cc9e2e30f681c0121787cdbb1768c8c643666ebab1f268e2026c/orjson-3.8.14-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ee0299b2dda9afce351a5e8c148ea7a886de213f955aa0288fb874fb44829c36"},
-    {url = "https://files.pythonhosted.org/packages/a0/2c/c8e38867801fb20ee4ffdc509550fad92e90e2c8c77d1d52e001e0d681e3/orjson-3.8.14-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6112194c11e611596eed72f46efb0e6b4812682eff3c7b48473d1146c3fa0efb"},
-    {url = "https://files.pythonhosted.org/packages/b2/ac/39719ba71753cc4a6ab67927809cdb7214aa83f10fabc91b957112ef1ed8/orjson-3.8.14-cp39-none-win_amd64.whl", hash = "sha256:9725226478d1dafe46d26f758eadecc6cf98dcbb985445e14a9c74aaed6ccfea"},
-    {url = "https://files.pythonhosted.org/packages/b5/96/f7dc7a640288b53e33ba772349066a6bbc8663e60a1d6bb64573709e93ae/orjson-3.8.14-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:97ebb7fab5f1ae212a6501f17cb7750a6838ffc2f1cebbaa5dec1a90038ca3c6"},
-    {url = "https://files.pythonhosted.org/packages/bb/ed/4edbbb4af8d72ea678a030514f670ce53b289de8c46bd6cf2b72e8e0cce0/orjson-3.8.14-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7d3d8faded5a514b80b56d0429eb38b429d7a810f8749d25dc10a0cc15b8a3c8"},
-    {url = "https://files.pythonhosted.org/packages/be/d1/bdc112671bd3c6373b8283889ba4d2bf34a7a029e33f58cf02b3d59abe30/orjson-3.8.14-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:0bc6b7abf27f1dc192dadad249df9b513912506dd420ce50fd18864a33789b71"},
-    {url = "https://files.pythonhosted.org/packages/c7/88/5c908d9ec55cad47d4a199535aac3f8aa2755fd85867f60ac1cc2c0c4bb5/orjson-3.8.14-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:31a2a29be559e92dcc5c278787b4166da6f0d45675b59a11c4867f5d1455ebf4"},
-    {url = "https://files.pythonhosted.org/packages/c8/a1/c7ded18ed1952bed15439f2331752b5ef0d33f1d9a0f9fdeee7549a84c8d/orjson-3.8.14.tar.gz", hash = "sha256:5ea93fd3ef7be7386f2516d728c877156de1559cda09453fc7dd7b696d0439b3"},
-    {url = "https://files.pythonhosted.org/packages/cd/1c/d6672a73e6359a4a767414246bad8216d44636809c9eea27e9a6938b3a7b/orjson-3.8.14-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8b206cca6836a4c6683bcaa523ab467627b5f03902e5e1082dc59cd010e6925f"},
-    {url = "https://files.pythonhosted.org/packages/cf/db/cdfed7a5efde531bdb7166db364ff4cf1f0b0c7e6edab0f9aecbbb855f08/orjson-3.8.14-cp39-cp39-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:716a3994e039203f0a59056efa28185d4cac51b922cc5bf27ab9182cfa20e12e"},
-    {url = "https://files.pythonhosted.org/packages/d1/d1/0ba3844cd12cbb01113a67a01ab3a77a9f59d7acaa346e517f2be6399def/orjson-3.8.14-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ca90db8f551b8960da95b0d4cad6c0489df52ea03585b6979595be7b31a3f946"},
-    {url = "https://files.pythonhosted.org/packages/d4/ad/d92c12caec047cb62ad56f169c29dcee6cbbec5de1abc863e71963cd14f6/orjson-3.8.14-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:09a3bf3154f40299b8bc95e9fb8da47436a59a2106fc22cae15f76d649e062da"},
-    {url = "https://files.pythonhosted.org/packages/d4/e5/5d8061ad5fc4907151e5c00db98d65f0590c9389672fefb93429b343dbe9/orjson-3.8.14-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:017de5ba22e58dfa6f41914f5edb8cd052d23f171000684c26b2d2ab219db31e"},
-    {url = "https://files.pythonhosted.org/packages/d9/47/4c30dca1f9b4b0d10c91381368554d8c7b89fc74889c8152f48ddcc84665/orjson-3.8.14-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:64b4fca0531030040e611c6037aaf05359e296877ab0a8e744c26ef9c32738b9"},
-    {url = "https://files.pythonhosted.org/packages/e3/ca/36ebce082fe66dd5f9555cc7ca2760ef593baaedd514aaf5eef0b7740303/orjson-3.8.14-cp310-cp310-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:7a7b0fead2d0115ef927fa46ad005d7a3988a77187500bf895af67b365c10d1f"},
-    {url = "https://files.pythonhosted.org/packages/e4/57/8331bd4ea3675ba72d96962346f0d9aabab7d2b11f00378adb42953ef004/orjson-3.8.14-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8a896a12b38fe201a72593810abc1f4f1597e65b8c869d5fc83bbcf75d93398f"},
-    {url = "https://files.pythonhosted.org/packages/ea/f7/ca03a52cdda6d4702b554e446980f0278911abb2a0ebf7ec245bdf7ecc12/orjson-3.8.14-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f80e62afe49e6bfc706e041faa351d7520b5f86572b8e31455802251ea989613"},
-    {url = "https://files.pythonhosted.org/packages/f4/18/a84b513905e1ed78529084967ca0b937f6ec45df200f908c4393aefddd79/orjson-3.8.14-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f4ac01a3db4e6a98a8ad1bb1a3e8bfc777928939e87c04e93e0d5006df574a4b"},
-    {url = "https://files.pythonhosted.org/packages/f9/fa/35ba54c9ff8ba0c0759d8a496095f9fdf0ff7c18182c330784f6b3025754/orjson-3.8.14-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9393a63cb0424515ec5e434078b3198de6ec9e057f1d33bad268683935f0a5d5"},
+"orjson 3.9.0" = [
+    {url = "https://files.pythonhosted.org/packages/00/a3/f645f6bdf235e217114250f8354705d6307ad2b083f4e3ae7c22b763f0be/orjson-3.9.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:bd89d63707ac616462832bfc5d16fa0c12483f86add2432ce55c8710c9531c03"},
+    {url = "https://files.pythonhosted.org/packages/02/6c/c29d9f8d0bd85d105d9b8508008831cd5ec4895a48e1283134f8ed8699de/orjson-3.9.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:748c1e8df0b0880c63d323e167ad17ab4db2e1178a40902c2fcb68cbe402d7c8"},
+    {url = "https://files.pythonhosted.org/packages/06/52/2e60bda73f04f66859c6b0ab2468275d0cf4519804d85d4daecc5935c142/orjson-3.9.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e44ebe2129d43c5a48f3affa3fa59c6484ed16faf5b00486add1061a95384ab0"},
+    {url = "https://files.pythonhosted.org/packages/0c/75/e41f01986e5ee56362c93ac5c92149f8fb6b6c8123c5aa5afe8a8b96746e/orjson-3.9.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:88626d898c408450c57664899831cf072787898af4847fa4466607ad2a83f454"},
+    {url = "https://files.pythonhosted.org/packages/10/1f/2915887049c72a195a7991ec8e5cf0344fcd6a940a2e50abee860752b7bf/orjson-3.9.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:9ee5f1ba82146a50d61fb58d310a37c0f406eda898172f9c98673b5d6f9461c3"},
+    {url = "https://files.pythonhosted.org/packages/15/a3/7520991c2e46ad7d9c2a9076aac4c3ca2bbe6820fc166b184f49ccbcea81/orjson-3.9.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:09522937479bd39d5bb32d11a5ecdf6926fda43ac2cbde21cc1a9508b4e4ea29"},
+    {url = "https://files.pythonhosted.org/packages/1b/4a/bb3412d18379e708311166699a4eccee9f6c1eadc756c7227246939da8a3/orjson-3.9.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:c68af71b1110820c914f9df75842895b5528ff524d3286fde57097b2b5ed8f22"},
+    {url = "https://files.pythonhosted.org/packages/2a/38/f0026e0413e3de18cbd03ad5120ed9651ed5675b5d8b3e8732a14aae765b/orjson-3.9.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f6ab80b60195f166a9d666b2eaf6d2c74202b6da2a1fb4b4d66b9cc0ce5c9957"},
+    {url = "https://files.pythonhosted.org/packages/2a/9f/e6e15918c7ef6fc38e3c009aa704937dfb31ba3916a7783eaf365b7a257f/orjson-3.9.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:2af7dff1c7ddb0c83eb5773acf6566b153f8cd32e4ba782ae9ccd6d0f324efd3"},
+    {url = "https://files.pythonhosted.org/packages/2e/ee/2b2ca51b317e975ef8fbc67b7909269c97591bc921bb5946174905b71d16/orjson-3.9.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1e3bde77c1e0061eb34bae6fea44818b2198e043ee10a16ad7b160921fee26ea"},
+    {url = "https://files.pythonhosted.org/packages/3a/d5/835fa231ae3e6811b9333522d4dbd09d02927d1e1c387820b1890c673b6e/orjson-3.9.0-cp38-cp38-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:d4c2d31178e3027affd98eead033f1c406890df83a0ca2016604cc21f722a1d1"},
+    {url = "https://files.pythonhosted.org/packages/3e/b0/75635bd68fcf9dc3139e7c0f9d84dec8e0db1fcaa9d06a289c4e657edac7/orjson-3.9.0-cp38-none-win_amd64.whl", hash = "sha256:3a208d0bca609de3152eb8320d5093ad9c52979332f626c13500d1645c66bf8d"},
+    {url = "https://files.pythonhosted.org/packages/40/51/9d5dcc6c72996d6cc9192cc31aac2326d5ca388bbf6342963e7489a2897b/orjson-3.9.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:04e61db09ff155846b69d07cf5aa21001f2010ea669ec3169c1fbad9c9e40cd5"},
+    {url = "https://files.pythonhosted.org/packages/44/1e/cc7c47dcf5ce59a4b9b1fd873d3813a4bf8e3f18fbda3c402e70e07fdd87/orjson-3.9.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:45df5bf6531ffda518331cc93cdcd4c84f4a4a0507d72af8fb698c7131a440a0"},
+    {url = "https://files.pythonhosted.org/packages/45/46/baedf92b3d24ae05325441e8d04c835ebf96e154d270530c48e7cd4ca4a2/orjson-3.9.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:8a1fcddcabe121e393f3c4a31ed6d3535214d42a4ece0f9dde2e250006d6a58d"},
+    {url = "https://files.pythonhosted.org/packages/46/ed/5b360740dae0de25303789d2447a4a5827a162314a376ace7112b22d83b5/orjson-3.9.0-cp37-none-win_amd64.whl", hash = "sha256:5afd22847b07b63f2b8fcfddd5b7a6f47c5aaa25e19b97a3d6d39508b8fd465a"},
+    {url = "https://files.pythonhosted.org/packages/49/a1/de519d9901d92ef086d8ddfc80d63a2ee51871887af5397ed4896cf06202/orjson-3.9.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:2536a7f30fd4d77532769ea9285cd20c69bd2b40acf980de94bbc79b1c6fad5a"},
+    {url = "https://files.pythonhosted.org/packages/56/f4/571b77ad51b91641aabef03e135792daa741939855d6e1ed4e830786f26d/orjson-3.9.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c50654e4870805e4b1a587c2c3c5ef2f36f3e67fc463a738339ff40d65f7db1"},
+    {url = "https://files.pythonhosted.org/packages/5c/ca/4d7a76381df4119c9ccfdaae1ab62004ed909f24519673118c3ad651a857/orjson-3.9.0-cp39-cp39-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:a901c432828c191332d75f358142736c433d4a192f7794123e1d30d68193de86"},
+    {url = "https://files.pythonhosted.org/packages/61/ac/1923bf83c0e36a9ac35d4c7347f715ce87b807c8692403b66047c7ac11e1/orjson-3.9.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:0e7fe5d603ee9177ff2e45858b4fc47fea2da0688f23d9773654889d56dfbc82"},
+    {url = "https://files.pythonhosted.org/packages/69/63/a0a20c4d858e23be5d7cb544d28bd513771d71bab04f20b293a06eb9ecb1/orjson-3.9.0-cp37-cp37m-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:f6476e2487c0b7387187de15e5b8f6635c29b75934f2e689ca8cad6550439f3d"},
+    {url = "https://files.pythonhosted.org/packages/6f/1b/7aa9c75c7f6647c0c4b41c8a77d84d409fead13a23dc63f407ef964222fa/orjson-3.9.0-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:d414fd0678e949779104f5b307f0f9fac861728e19d3cdde66759af77f892da0"},
+    {url = "https://files.pythonhosted.org/packages/73/59/cb014160188df36c74aac8c1fcab3b4a59a0f0d070c69f65423cf1ddfca6/orjson-3.9.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c7b241c3229084035b38cac9b5c96b43644da829da41d9d5be0fefb96fb116e1"},
+    {url = "https://files.pythonhosted.org/packages/73/dc/377f4ab9875b25f79e3c46d025922045c66e2057592f473a0675091a6f6a/orjson-3.9.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:721d47dffedb7795ffea8a06f2de7d192de7b58e085cf357a99abf0eb931f2c3"},
+    {url = "https://files.pythonhosted.org/packages/87/15/f643ee5e696ab43a690c4745310553d2c3e8180c8cac59bab4e50dccd22a/orjson-3.9.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2fbf34667a8be48ec89d5ef479a00d4e7b3acda62d722c97377702da0c30ffd"},
+    {url = "https://files.pythonhosted.org/packages/8b/8a/59611e84d2d76f5eb23ffaa9c7c8aaa728174b5e1cb86c6a29b8418ec349/orjson-3.9.0-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:949698bdddb1daff986d73e6bbe6cd68833cd80c4adc6b69fafbd46634d4672c"},
+    {url = "https://files.pythonhosted.org/packages/8e/87/61885b10fa30cb2ed4ddf0f9149cdd295d8cf409cf78370b55a200e4db2b/orjson-3.9.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebe372e9f4e4f0335b7b4ebfab991b3734371e3d5b7f989ca3baa5da25185f4a"},
+    {url = "https://files.pythonhosted.org/packages/95/1c/be392b9e88f568a67fe546008a1d46cb955798c5bb02f11f9d0485dfa8ed/orjson-3.9.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7a3693fde44b2eeb80074ecbe8c504b25baf71e66c080af2a574193a5ba81960"},
+    {url = "https://files.pythonhosted.org/packages/a9/d0/c3341cc7d1818dc80df738e3879275a8236da26cd17823ba4a66d12d577b/orjson-3.9.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:edd77183c154cbedaa6dac32fee9cb770b04e2a7f367a5864f444578554cc946"},
+    {url = "https://files.pythonhosted.org/packages/ad/c3/bdc121a246921d0699c695eb73cf56417ab487767c4f761f9425dd1bf59c/orjson-3.9.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:108c58d2c7648c991f82f9b2217c50981ad7cf6aaee3efbfaa9d807e49cd69b8"},
+    {url = "https://files.pythonhosted.org/packages/b1/e6/6389d8ea0a3d9981f13c61be638715c8f616d1231574131081d35195b9fe/orjson-3.9.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d4fcf598bd5a99a94caa7ec92ce657939f12491e4753ea7e4d6c03faf5f7912e"},
+    {url = "https://files.pythonhosted.org/packages/b2/95/707184b9b991a58bc8f290aed0c3942f642e85c089f0228168af41e54cf3/orjson-3.9.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:271b6f1018757fc6bca40ae72e6cdb6cf84584dde2d1e5eaac30e387a13d9e72"},
+    {url = "https://files.pythonhosted.org/packages/c3/cb/683a60de5c1820412979aeca04e43cdb6c01a282edf1583bf84054d22458/orjson-3.9.0-cp311-none-win_amd64.whl", hash = "sha256:44fa74b497e608a8cdca1ee37fe3533a30f17163c7e2872ab1b854900cf0dfcf"},
+    {url = "https://files.pythonhosted.org/packages/c9/35/31348485dd1e303c5f87c2e2d3be6ae4bdfdb51c2677227190543b5a3f0b/orjson-3.9.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:9de2129d40674007cb24164939e075b5b39fee768bf20801e08c0e3283bfb18e"},
+    {url = "https://files.pythonhosted.org/packages/c9/d9/0382e682322a996476ece62f92cc90cb067da3266a6a9ed71da9b49cc442/orjson-3.9.0-cp39-none-win_amd64.whl", hash = "sha256:3235c31d0fe674f6e3433e9ddfed212aa840c83a9b6ef5ae128950e2c808c303"},
+    {url = "https://files.pythonhosted.org/packages/ce/19/ae05dd3d72f8036ad4f7ab6ff5e41d4dd44e81fb62aa6a04d6c1f53d051f/orjson-3.9.0-cp310-cp310-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:128b1cd0f00a37ba64a12cceeba4e8070655d4400edd55a737513ee663c1ed5a"},
+    {url = "https://files.pythonhosted.org/packages/d5/64/9e81da69bb5dfc0a30d7ce2682f1a0aa4637a82fde9fd56e2e188f040898/orjson-3.9.0-cp311-cp311-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:47d7e4a3effc0e9314bd5b06e7431f2490a5e64dcdcbbc4d60e713786fec327d"},
+    {url = "https://files.pythonhosted.org/packages/d7/c8/a604ad0c7f0ffb5897328e0ca4a81697c2ffe1fac3f72bbaee59b12629cb/orjson-3.9.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:09ee828572fadcd58bf356d2c1bad99a95c7c9c1f182b407abbc7dec1810f542"},
+    {url = "https://files.pythonhosted.org/packages/df/8c/1184f03df5233823f88a1d3c5c1878f985a9958d06512d875fc9f8f5340b/orjson-3.9.0-cp310-none-win_amd64.whl", hash = "sha256:46c9733330b75c116438f555c0b971a2388b5f502e2dd4ec3bf6bacb96f82741"},
+    {url = "https://files.pythonhosted.org/packages/e3/96/fa927d1c19866b11dcfaf56d4de9d29b4ec4c14786b4a8c816cb58bb7e95/orjson-3.9.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:21f6a6fdfbc13cd715c61e9fa9daeff732df6401ab7d6a2ebad0042313a40bd1"},
+    {url = "https://files.pythonhosted.org/packages/e5/e4/b48906b617a14e8e9b4d99d5b5f470002674ba434bc10770f17511255f1f/orjson-3.9.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c41d1ef6ec308e9e3701764b3de889ed8c1c126eceaea881dd1027bffbed89fe"},
+    {url = "https://files.pythonhosted.org/packages/e8/7a/fffa0e31dde392a9116718e371e9deb27ac35b6f089644a1fd9ffdb6b3fe/orjson-3.9.0-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:3f1193417b5a93deb41bcb8db27b61179b9b3e299b337b578c31f19159664da3"},
+    {url = "https://files.pythonhosted.org/packages/ea/d0/59c5a2e35724d2af65f42b05030783d356035f91ca81c3bf2dee454070fa/orjson-3.9.0-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:c4949fc1304b702197c0840882e84b86d8d5ca33c3d945cc60727bc1786c2b20"},
+    {url = "https://files.pythonhosted.org/packages/ec/2b/a2530675913d060f7ee760efcb88dd94b4d2b4bb1dedf3b09c401a0b82f9/orjson-3.9.0-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:86da00836029b2a071229c8aecab998a2f316c1bc7de10ae020d7311de3a6d0d"},
+    {url = "https://files.pythonhosted.org/packages/ee/45/47bcbad2c90b2846428bcd3a0a4623e37bb74ae3583bb96929b2e625d095/orjson-3.9.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:08cb43569198c1f5c89ecafcbfc62414f6115d894ff908d8cf8e5e24801364e6"},
+    {url = "https://files.pythonhosted.org/packages/ef/00/f3beb032641547b01c5850a4ff02bf6dbc318207c10b116d405f071321a0/orjson-3.9.0.tar.gz", hash = "sha256:f6dd27c71cd6e146795f876449a8eae74f67ae1e4e244dfc1203489103eb2d94"},
 ]
 "packaging 23.1" = [
     {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pandas 2.0.2" = [
     {url = "https://files.pythonhosted.org/packages/07/66/a1c77bc7af5358f4404e47a28a0f16d624fffa20ed35ba189d03872023b8/pandas-2.0.2-cp38-cp38-win32.whl", hash = "sha256:6d6d10c2142d11d40d6e6c0a190b1f89f525bcf85564707e31b0a39e3b398e08"},
@@ -2800,111 +2800,111 @@
     {url = "https://files.pythonhosted.org/packages/0c/2f/894bc187ce40367f2e878ced196e1b5a9bc66cb553a062ed955d4f7dcbab/rarfile-4.0.tar.gz", hash = "sha256:67548769229c5bda0827c1663dce3f54644f9dbfba4ae86d4da2b2afd3e602a1"},
     {url = "https://files.pythonhosted.org/packages/95/f4/c92fab227c7457e3b76a4096ccb655ded9deac869849cb03afbe55dfdc1e/rarfile-4.0-py3-none-any.whl", hash = "sha256:1094869119012f95c31a6f22cc3a9edbdca61861b805241116adbe2d737b68f8"},
 ]
 "rebulk 3.2.0" = [
     {url = "https://files.pythonhosted.org/packages/84/4d/df073d593f7e7e4a5a7e19148b2e9b4ae63b4ddcbb863f1e7bb2b6f19c62/rebulk-3.2.0-py3-none-any.whl", hash = "sha256:6bc31ae4b37200623c5827d2f539f9ec3e52b50431322dad8154642a39b0a53e"},
     {url = "https://files.pythonhosted.org/packages/f2/06/24c69f8d707c9eefc1108a64e079da56b5f351e3f59ed76e8f04b9f3e296/rebulk-3.2.0.tar.gz", hash = "sha256:0d30bf80fca00fa9c697185ac475daac9bde5f646ce3338c9ff5d5dc1ebdfebc"},
 ]
-"regex 2023.5.5" = [
-    {url = "https://files.pythonhosted.org/packages/01/36/aedf96310757fa5a421749be911ed750077171930f439a233bfd8f87e43c/regex-2023.5.5-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:fee0016cc35a8a91e8cc9312ab26a6fe638d484131a7afa79e1ce6165328a135"},
-    {url = "https://files.pythonhosted.org/packages/02/b7/af3253bc0173045f9df1f8492705823ddf85150f71a52a51fd622796ae66/regex-2023.5.5-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a56c18f21ac98209da9c54ae3ebb3b6f6e772038681d6cb43b8d53da3b09ee81"},
-    {url = "https://files.pythonhosted.org/packages/09/26/925431262010b6e3efe962fa30a8cede87dd4c3f27d2c84c1ae3e54af5db/regex-2023.5.5-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:18196c16a584619c7c1d843497c069955d7629ad4a3fdee240eb347f4a2c9dbe"},
-    {url = "https://files.pythonhosted.org/packages/0b/15/b0857fc4ccfc3f0262bfc580f0c3338ce11ab050879201fc16ee716890fe/regex-2023.5.5-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:59e4b729eae1a0919f9e4c0fc635fbcc9db59c74ad98d684f4877be3d2607dd6"},
-    {url = "https://files.pythonhosted.org/packages/0d/3c/a61379572196a04a866c0013c500576b001832533bc12f80ec13c6872c22/regex-2023.5.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:256f7f4c6ba145f62f7a441a003c94b8b1af78cee2cccacfc1e835f93bc09426"},
-    {url = "https://files.pythonhosted.org/packages/16/9a/2ddd037546c1f6446b26bd9037f4b551c2f38e250038388626e5da88e7f1/regex-2023.5.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:53e22e4460f0245b468ee645156a4f84d0fc35a12d9ba79bd7d79bdcd2f9629d"},
-    {url = "https://files.pythonhosted.org/packages/18/ba/538b878727ab58a55cad175ab5aececb979c21b8b1e1830094f35ac66882/regex-2023.5.5-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ced02e3bd55e16e89c08bbc8128cff0884d96e7f7a5633d3dc366b6d95fcd1d6"},
-    {url = "https://files.pythonhosted.org/packages/1f/5a/ebddb94a8912c0cd08e9a501efb7fb9698fd011c49352a49516249f33643/regex-2023.5.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:8f08276466fedb9e36e5193a96cb944928301152879ec20c2d723d1031cd4ddd"},
-    {url = "https://files.pythonhosted.org/packages/23/35/af9d7cd565526173cac5ec76549429f18476d64335c8fa8338f5f080cc13/regex-2023.5.5-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:8f5e06df94fff8c4c85f98c6487f6636848e1dc85ce17ab7d1931df4a081f657"},
-    {url = "https://files.pythonhosted.org/packages/27/30/69a2eb2a74c5098f3ff69e52c44f739f11fc19ecea84ce69ed6073bda9d2/regex-2023.5.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:cf123225945aa58b3057d0fba67e8061c62d14cc8a4202630f8057df70189051"},
-    {url = "https://files.pythonhosted.org/packages/2a/b2/ff7e8650aad92b2486c27ba1bb87c473a7b000304a2e7cb9892f597aeca8/regex-2023.5.5-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0a69cf0c00c4d4a929c6c7717fd918414cab0d6132a49a6d8fc3ded1988ed2ea"},
-    {url = "https://files.pythonhosted.org/packages/2a/b6/5d44a38161062c48b8db4742bb7076315b08d267bbdfe77b1f8bee02f85a/regex-2023.5.5-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:f83fe9e10f9d0b6cf580564d4d23845b9d692e4c91bd8be57733958e4c602956"},
-    {url = "https://files.pythonhosted.org/packages/2b/06/ee0731f71dd2825393e56da78af9114eee083686105cc635daab2ab1b7d6/regex-2023.5.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:1189fbbb21e2c117fda5303653b61905aeeeea23de4a94d400b0487eb16d2d60"},
-    {url = "https://files.pythonhosted.org/packages/2d/db/d6e9577d4935e8bd6519fc502a3d032f4dabf6175b04f68a3e2e1dad244f/regex-2023.5.5-cp38-cp38-win32.whl", hash = "sha256:7923470d6056a9590247ff729c05e8e0f06bbd4efa6569c916943cb2d9b68b91"},
-    {url = "https://files.pythonhosted.org/packages/33/a8/12bdc84d78e2748cc7c2d990317930fe05e421937f42a05e9621a2d90a89/regex-2023.5.5-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:e645c757183ee0e13f0bbe56508598e2d9cd42b8abc6c0599d53b0d0b8dd1479"},
-    {url = "https://files.pythonhosted.org/packages/35/d7/33315abe1555850bfdf9cae6175344858b6614fb9a0bca58c8102dd42a42/regex-2023.5.5-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a623564d810e7a953ff1357f7799c14bc9beeab699aacc8b7ab7822da1e952b8"},
-    {url = "https://files.pythonhosted.org/packages/37/10/3e47ec258cd5319202cc11b2956bd52b1e8613240b276662d96aa4ba2f71/regex-2023.5.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:f764e4dfafa288e2eba21231f455d209f4709436baeebb05bdecfb5d8ddc3d35"},
-    {url = "https://files.pythonhosted.org/packages/3b/0f/d3bd4ad92c1c530c344414b1438d826da72825d41b64db397e903aa7c260/regex-2023.5.5-cp39-cp39-win32.whl", hash = "sha256:732176f5427e72fa2325b05c58ad0b45af341c459910d766f814b0584ac1f9ac"},
-    {url = "https://files.pythonhosted.org/packages/41/fb/2eee67ebd59417a0a329ae5ae88b6a1bded20e66693c1851adf9cfcb065a/regex-2023.5.5-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:18f05d14f14a812fe9723f13afafefe6b74ca042d99f8884e62dbd34dcccf3e2"},
-    {url = "https://files.pythonhosted.org/packages/44/1c/bbe0e8507361ce6f70902dbf6c23839ab548364c95dfaefe3c7fdf60cc49/regex-2023.5.5-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:db09e6c18977a33fea26fe67b7a842f706c67cf8bda1450974d0ae0dd63570df"},
-    {url = "https://files.pythonhosted.org/packages/44/a2/b3eae40cab9864fc784a4c1709cafa95db47d875a2297b70daf1afd7fbe6/regex-2023.5.5-cp36-cp36m-win32.whl", hash = "sha256:821a88b878b6589c5068f4cc2cfeb2c64e343a196bc9d7ac68ea8c2a776acd46"},
-    {url = "https://files.pythonhosted.org/packages/45/27/03118528e248b3a6df85d8bbc87bea77d5324488ae27f387aafaa7cc24e6/regex-2023.5.5-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:6b8d0c153f07a953636b9cdb3011b733cadd4178123ef728ccc4d5969e67f3c2"},
-    {url = "https://files.pythonhosted.org/packages/4e/fa/dd1b555c71aa7d6e834165c882cefdafd9865eee990985aba01990a7280c/regex-2023.5.5-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:fb2b495dd94b02de8215625948132cc2ea360ae84fe6634cd19b6567709c8ae2"},
-    {url = "https://files.pythonhosted.org/packages/51/56/cc303c524837c15aa305ea00cc898b57add23f7db9753f8856a351dda54f/regex-2023.5.5-cp310-cp310-win32.whl", hash = "sha256:40005cbd383438aecf715a7b47fe1e3dcbc889a36461ed416bdec07e0ef1db66"},
-    {url = "https://files.pythonhosted.org/packages/53/95/27d4887cf0cd2c6e94920bcc5877280cb943888686db85049df18a66e4dd/regex-2023.5.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:a4c5da39bca4f7979eefcbb36efea04471cd68db2d38fcbb4ee2c6d440699833"},
-    {url = "https://files.pythonhosted.org/packages/54/8d/3e346fc5c6e63383c6e6a62a31e7b9cdf5d9539e127aa6f6a7f6b2e4d47e/regex-2023.5.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f2910502f718828cecc8beff004917dcf577fc5f8f5dd40ffb1ea7612124547b"},
-    {url = "https://files.pythonhosted.org/packages/57/5e/6dff6880b5ab4aa6e9e6f658b34de97ad4cba6488a8ad7328acb3b689daa/regex-2023.5.5-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:2e9c4f778514a560a9c9aa8e5538bee759b55f6c1dcd35613ad72523fd9175b8"},
-    {url = "https://files.pythonhosted.org/packages/5b/aa/c63c8b23cca132c1688078ccc56c0654cd3cbc6a639d0ac9fa8e48d8b7de/regex-2023.5.5-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:6893544e06bae009916a5658ce7207e26ed17385149f35a3125f5259951f1bbe"},
-    {url = "https://files.pythonhosted.org/packages/5e/15/4ac85a6ce5c46223e312de2a38137f7ff1e6c5b4b233054cd7e72466345b/regex-2023.5.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9fda3e50abad8d0f48df621cf75adc73c63f7243cbe0e3b2171392b445401550"},
-    {url = "https://files.pythonhosted.org/packages/5f/32/9a6c6af6f6013a7bfe12469a910f577ac27d6c6767adef69ebf798f07a7f/regex-2023.5.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a99757ad7fe5c8a2bb44829fc57ced11253e10f462233c1255fe03888e06bc19"},
-    {url = "https://files.pythonhosted.org/packages/61/78/d3e53ac70db4eeea69d51093c1c1667a58a72cb603fa094e721b35eaaf67/regex-2023.5.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:33d430a23b661629661f1fe8395be2004006bc792bb9fc7c53911d661b69dd7e"},
-    {url = "https://files.pythonhosted.org/packages/61/f8/4f94b89fbacfd301ab1b96fc54d3d942260202701f25a4c549b2c5406dbe/regex-2023.5.5-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:144b5b017646b5a9392a5554a1e5db0000ae637be4971c9747566775fc96e1b2"},
-    {url = "https://files.pythonhosted.org/packages/67/e9/3d300456309174e7c431fd3575bb8e6c5d057d03f647cda787038c3cfb51/regex-2023.5.5-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:445d6f4fc3bd9fc2bf0416164454f90acab8858cd5a041403d7a11e3356980e8"},
-    {url = "https://files.pythonhosted.org/packages/6a/36/9ac9b08bc8bbe006041cc2155347b4a29593d448941d036ea8b8023a6add/regex-2023.5.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:02f4541550459c08fdd6f97aa4e24c6f1932eec780d58a2faa2068253df7d6ff"},
-    {url = "https://files.pythonhosted.org/packages/6a/36/d5e3666b761525204dadfd8ad684c231e56c5936cbfd8359bd7ff1ba4383/regex-2023.5.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:811040d7f3dd9c55eb0d8b00b5dcb7fd9ae1761c454f444fd9f37fe5ec57143a"},
-    {url = "https://files.pythonhosted.org/packages/77/5d/98efc9cf46d60f3704cf00f8b3bd81319493639fd4367efb5d02fd29ffc1/regex-2023.5.5.tar.gz", hash = "sha256:7d76a8a1fc9da08296462a18f16620ba73bcbf5909e42383b253ef34d9d5141e"},
-    {url = "https://files.pythonhosted.org/packages/78/86/530a560a506ef8c461fb055c1fed355aed79caa6f7de04ae83f7b7be0bda/regex-2023.5.5-cp36-cp36m-musllinux_1_1_ppc64le.whl", hash = "sha256:e2205a81f815b5bb17e46e74cc946c575b484e5f0acfcb805fb252d67e22938d"},
-    {url = "https://files.pythonhosted.org/packages/78/db/a9fb9a194d340cb507aabae958280b8f8c24bd3038361b209fb7ded9b989/regex-2023.5.5-cp311-cp311-win_amd64.whl", hash = "sha256:586a011f77f8a2da4b888774174cd266e69e917a67ba072c7fc0e91878178a80"},
-    {url = "https://files.pythonhosted.org/packages/79/87/da8099926c2d627839159126ed5a58980b18408b9304110435b7ec06bfc6/regex-2023.5.5-cp36-cp36m-win_amd64.whl", hash = "sha256:7918a1b83dd70dc04ab5ed24c78ae833ae8ea228cef84e08597c408286edc926"},
-    {url = "https://files.pythonhosted.org/packages/7c/81/b064cc2c67ca2182137641f9d3fd47fe470f1a84674d9b9f91fd39bf0e6f/regex-2023.5.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:aad5524c2aedaf9aa14ef1bc9327f8abd915699dea457d339bebbe2f0d218f86"},
-    {url = "https://files.pythonhosted.org/packages/7f/2a/5d4c1315e17eb54e8524952b80a03308735a5e6d3288ba04b19845b56f92/regex-2023.5.5-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:b6365703e8cf1644b82104cdd05270d1a9f043119a168d66c55684b1b557d008"},
-    {url = "https://files.pythonhosted.org/packages/80/07/518121c35e002a73f8fb75fcac23f9c6a5a1784c149e9bcb98d3ec6bca78/regex-2023.5.5-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5ac2b7d341dc1bd102be849d6dd33b09701223a851105b2754339e390be0627a"},
-    {url = "https://files.pythonhosted.org/packages/80/f6/2edf65ed793b9d5ba39083776b83481c41555a2ad57bf6b6934c4d7dd9a8/regex-2023.5.5-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:21e90a288e6ba4bf44c25c6a946cb9b0f00b73044d74308b5e0afd190338297c"},
-    {url = "https://files.pythonhosted.org/packages/83/ba/da371627cb5df2216f2022a51eea6728b5048319cd1c41c967134a0df3f3/regex-2023.5.5-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:1ecf3dcff71f0c0fe3e555201cbe749fa66aae8d18f80d2cc4de8e66df37390a"},
-    {url = "https://files.pythonhosted.org/packages/83/ff/7164610b30e447e3bb86171f95cf3172a013e475472c8b7a22314bdb54cc/regex-2023.5.5-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:921473a93bcea4d00295799ab929522fc650e85c6b9f27ae1e6bb32a790ea7d3"},
-    {url = "https://files.pythonhosted.org/packages/8a/0c/65a0809640bcbb2e55c8c1c87ee300ab90481130676c26a4581985a6705e/regex-2023.5.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bd966475e963122ee0a7118ec9024388c602d12ac72860f6eea119a3928be053"},
-    {url = "https://files.pythonhosted.org/packages/8d/d5/4d56a7655dcec858d697f0fa9b7eb1ff30ec4ed5a445fe60a432955cc30b/regex-2023.5.5-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:844671c9c1150fcdac46d43198364034b961bd520f2c4fdaabfc7c7d7138a2dd"},
-    {url = "https://files.pythonhosted.org/packages/90/23/ff74c6c56fe82e1fa398b8a7f73e81848b05cbefe5af99f22f0f4b25e57c/regex-2023.5.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:50fd2d9b36938d4dcecbd684777dd12a407add4f9f934f235c66372e630772b0"},
-    {url = "https://files.pythonhosted.org/packages/91/48/d2a23b461b7136df911ab50412a3e480ecf4c8b5caf8c6185244da6af7af/regex-2023.5.5-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:de2f780c3242ea114dd01f84848655356af4dd561501896c751d7b885ea6d3a1"},
-    {url = "https://files.pythonhosted.org/packages/93/70/027e3599cb021b1462dcb4b4c5b8233dbfd8e4779eaf7738871b27c630cc/regex-2023.5.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:290fd35219486dfbc00b0de72f455ecdd63e59b528991a6aec9fdfc0ce85672e"},
-    {url = "https://files.pythonhosted.org/packages/9b/05/7fe34981c97401ab999f2bdc39b45578308748b1db69b27cb3cc1f034a8f/regex-2023.5.5-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:bd7b68fd2e79d59d86dcbc1ccd6e2ca09c505343445daaa4e07f43c8a9cc34da"},
-    {url = "https://files.pythonhosted.org/packages/a0/90/34880cf20e335921095ba9ca8a5dce273c10ee70b970a7cd71f4d5eb1a8e/regex-2023.5.5-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a8906669b03c63266b6a7693d1f487b02647beb12adea20f8840c1a087e2dfb5"},
-    {url = "https://files.pythonhosted.org/packages/a0/dd/ce702f781c4fdd4dca86bda1f842f64e68c75840eba7beb5556f91c8b70d/regex-2023.5.5-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:72aa4746993a28c841e05889f3f1b1e5d14df8d3daa157d6001a34c98102b393"},
-    {url = "https://files.pythonhosted.org/packages/a2/23/c9a511f32618ab757e6775c0e5c63a01fd17056c1158e72ea7845d796133/regex-2023.5.5-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:338994d3d4ca4cf12f09822e025731a5bdd3a37aaa571fa52659e85ca793fb67"},
-    {url = "https://files.pythonhosted.org/packages/a8/e1/581b12525a47073e38517aeb4621b4e189ac949158c3bf3f2a9c87fd4910/regex-2023.5.5-cp310-cp310-win_amd64.whl", hash = "sha256:59597cd6315d3439ed4b074febe84a439c33928dd34396941b4d377692eca810"},
-    {url = "https://files.pythonhosted.org/packages/a9/bb/f37e451ab9870090f50eba06b118e3ed000d53940ebd97decfbf89ff4ade/regex-2023.5.5-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:4a5059bd585e9e9504ef9c07e4bc15b0a621ba20504388875d66b8b30a5c4d18"},
-    {url = "https://files.pythonhosted.org/packages/aa/1a/aaf87f92c6d911256e7ddd78a80db2b089d7a15d30d82d26853c3ef5bedb/regex-2023.5.5-cp39-cp39-win_amd64.whl", hash = "sha256:1307aa4daa1cbb23823d8238e1f61292fd07e4e5d8d38a6efff00b67a7cdb764"},
-    {url = "https://files.pythonhosted.org/packages/aa/9a/4eebbfedf7f0a3ae14307a9f7fb65bfe853b32b0f209e31bc21a548d3016/regex-2023.5.5-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:3d45864693351c15531f7e76f545ec35000d50848daa833cead96edae1665559"},
-    {url = "https://files.pythonhosted.org/packages/ab/cb/8518e23ada66106aaeddf551c7a5539854bf6782b13d453ac5ae7f244c59/regex-2023.5.5-cp37-cp37m-win_amd64.whl", hash = "sha256:9b320677521aabf666cdd6e99baee4fb5ac3996349c3b7f8e7c4eee1c00dfe3a"},
-    {url = "https://files.pythonhosted.org/packages/ac/63/a6301bcb744b45756796fd35080d6dc0e2453cfdca28bee63fff20c239a4/regex-2023.5.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:48c9ec56579d4ba1c88f42302194b8ae2350265cb60c64b7b9a88dcb7fbde309"},
-    {url = "https://files.pythonhosted.org/packages/ae/4b/9926dd761af4aa8e703ccef72ce7d3a5599e36153f871a270aeb68dab8ba/regex-2023.5.5-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c2ce65bdeaf0a386bb3b533a28de3994e8e13b464ac15e1e67e4603dd88787fa"},
-    {url = "https://files.pythonhosted.org/packages/b8/bc/dc3b8c54628635802192f4b1fe4934f279da24692655ee203463e5326482/regex-2023.5.5-cp36-cp36m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b8b942d8b3ce765dbc3b1dad0a944712a89b5de290ce8f72681e22b3c55f3cc8"},
-    {url = "https://files.pythonhosted.org/packages/be/42/ffde1f44c3fa2ecbe285ee2f5949b491b0ac2a18dc13327f34e249e2a9a3/regex-2023.5.5-cp36-cp36m-musllinux_1_1_s390x.whl", hash = "sha256:385992d5ecf1a93cb85adff2f73e0402dd9ac29b71b7006d342cc920816e6f32"},
-    {url = "https://files.pythonhosted.org/packages/c0/e6/38875874e79498c998f9a19476fb2bd152840a4c7f34517eb0ee8d6f1fb0/regex-2023.5.5-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:690a17db524ee6ac4a27efc5406530dd90e7a7a69d8360235323d0e5dafb8f5b"},
-    {url = "https://files.pythonhosted.org/packages/c3/26/a561242ece9b3a84d60e1fc5d07f7ba1f64729bad37687094d5d83553de8/regex-2023.5.5-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:941b3f1b2392f0bcd6abf1bc7a322787d6db4e7457be6d1ffd3a693426a755f2"},
-    {url = "https://files.pythonhosted.org/packages/c5/3a/3dc14c9b1c0a32f3ddf45d993233395d115a89923c2190c33920e316be3b/regex-2023.5.5-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:72a28979cc667e5f82ef433db009184e7ac277844eea0f7f4d254b789517941d"},
-    {url = "https://files.pythonhosted.org/packages/c6/86/f0bb334088b102e2bb3528b502d3c0c0a7301cbc2c8d2e0304ec4b1964d7/regex-2023.5.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:84397d3f750d153ebd7f958efaa92b45fea170200e2df5e0e1fd4d85b7e3f58a"},
-    {url = "https://files.pythonhosted.org/packages/c7/17/5b76862f602277d33b2beeeba202657f6f1c1ed35c59466f4061bb0a97bd/regex-2023.5.5-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:10250a093741ec7bf74bcd2039e697f519b028518f605ff2aa7ac1e9c9f97423"},
-    {url = "https://files.pythonhosted.org/packages/c9/e4/d82c1a857a5346a37c4a72af6d995f6aeea1f17d6163a39d68c6362d6143/regex-2023.5.5-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:6164d4e2a82f9ebd7752a06bd6c504791bedc6418c0196cd0a23afb7f3e12b2d"},
-    {url = "https://files.pythonhosted.org/packages/d0/02/b3a2c110ed3d51c0138e12fa555920c3c81693ec9b5fb8dd229c6482355c/regex-2023.5.5-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:4b870b6f632fc74941cadc2a0f3064ed8409e6f8ee226cdfd2a85ae50473aa94"},
-    {url = "https://files.pythonhosted.org/packages/dc/15/be319fd51cb9980ec1abf855e1b358e1b20e3655f3cec8cf5d58f8f924e5/regex-2023.5.5-cp311-cp311-win32.whl", hash = "sha256:c8c143a65ce3ca42e54d8e6fcaf465b6b672ed1c6c90022794a802fb93105d22"},
-    {url = "https://files.pythonhosted.org/packages/de/01/71793c90f543c97848d09a9993ac6039a95190d92d69dce5bfb50b309462/regex-2023.5.5-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:ba73a14e9c8f9ac409863543cde3290dba39098fc261f717dc337ea72d3ebad2"},
-    {url = "https://files.pythonhosted.org/packages/de/d4/e44c3b5e5934ae90c67036e8d80ebc0ced7a8702e2dd1afd31b0c564f3fc/regex-2023.5.5-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:890a09cb0a62198bff92eda98b2b507305dd3abf974778bae3287f98b48907d3"},
-    {url = "https://files.pythonhosted.org/packages/e0/7c/941e5c89bbbcd6ba460444c6ec029d54e7147741078f1c8300a8cbf8abb9/regex-2023.5.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d1cbe6b5be3b9b698d8cc4ee4dee7e017ad655e83361cd0ea8e653d65e469468"},
-    {url = "https://files.pythonhosted.org/packages/e1/d2/76a59a6483c32f5aa658fa8e56ec9dbe6e6025aba0270ce337e7fe5d965e/regex-2023.5.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:afb1c70ec1e594a547f38ad6bf5e3d60304ce7539e677c1429eebab115bce56e"},
-    {url = "https://files.pythonhosted.org/packages/e2/ff/80f795d39a4f7afc4c0912f57fdf7d3ae39d964d949bb0e6ea9e2eafb077/regex-2023.5.5-cp37-cp37m-win32.whl", hash = "sha256:10374c84ee58c44575b667310d5bbfa89fb2e64e52349720a0182c0017512f6c"},
-    {url = "https://files.pythonhosted.org/packages/e3/38/d7873187b26f1bedcb2db83b458156c348878844c0c293a74fc5e219b7e9/regex-2023.5.5-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9c3efee9bb53cbe7b285760c81f28ac80dc15fa48b5fe7e58b52752e642553f1"},
-    {url = "https://files.pythonhosted.org/packages/e4/0a/cc8a552c9ef9f65e07398a077872d7a9b611e663f4d7af4cbd63676d84c9/regex-2023.5.5-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5a0f874ee8c0bc820e649c900243c6d1e6dc435b81da1492046716f14f1a2a96"},
-    {url = "https://files.pythonhosted.org/packages/eb/0d/ef48969f8626d3cbc8a82b8e9d46abe6294ca51f4bdcf2bb3a50cded4089/regex-2023.5.5-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:171c52e320fe29260da550d81c6b99f6f8402450dc7777ef5ced2e848f3b6f8f"},
-    {url = "https://files.pythonhosted.org/packages/eb/d5/d992d17a298f3d4ec93f63437e2cca60924f924e4404ad5affd6d5e3892c/regex-2023.5.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:0bbd5dcb19603ab8d2781fac60114fb89aee8494f4505ae7ad141a3314abb1f9"},
-    {url = "https://files.pythonhosted.org/packages/f0/3c/99f8edd0feb2e97117d6e797a99455529d9ff725e45b9b902b0b2c1d02d2/regex-2023.5.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:d19e57f888b00cd04fc38f5e18d0efbd91ccba2d45039453ab2236e6eec48d4d"},
-    {url = "https://files.pythonhosted.org/packages/f6/e6/5ebc73b4f1c9712369b30cc8f808cea1172bd5bcc1b025ddc9a7cf95a2d0/regex-2023.5.5-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:aa7d032c1d84726aa9edeb6accf079b4caa87151ca9fabacef31fa028186c66d"},
-    {url = "https://files.pythonhosted.org/packages/f7/bd/a1cf5020abc1fbbc71bde9b645748f6dcd0f5303f7fc907ce54e09e823e6/regex-2023.5.5-cp38-cp38-win_amd64.whl", hash = "sha256:4035d6945cb961c90c3e1c1ca2feb526175bcfed44dfb1cc77db4fdced060d3e"},
-    {url = "https://files.pythonhosted.org/packages/f7/d4/4c3eb7cdda7aafc3b17b620f5f52af985ed01a23b51ddadc639229e453b3/regex-2023.5.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:cd46f30e758629c3ee91713529cfbe107ac50d27110fdcc326a42ce2acf4dafc"},
-    {url = "https://files.pythonhosted.org/packages/f9/5f/f6b642b6b8be39e3bd081992b11bed06e78604431bce64e412b3d0735253/regex-2023.5.5-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:5e3f4468b8c6fd2fd33c218bbd0a1559e6a6fcf185af8bb0cc43f3b5bfb7d636"},
-    {url = "https://files.pythonhosted.org/packages/f9/d5/e31e1f8e3bad5fa2c988915e52f5899b0d5aa7ac823414ef0242c2454462/regex-2023.5.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:c64d5abe91a3dfe5ff250c6bb267ef00dbc01501518225b45a5f9def458f31fb"},
-    {url = "https://files.pythonhosted.org/packages/fa/84/21e97a9fd11d2156fc23b1b438514a3d6a40834c355d880c081a998f2eea/regex-2023.5.5-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a6e4b0e0531223f53bad07ddf733af490ba2b8367f62342b92b39b29f72735a"},
-    {url = "https://files.pythonhosted.org/packages/fb/5f/b1aad255ac39b12cd0c78ddaf4d55835653b0b0f790605e6117bbd8eb706/regex-2023.5.5-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:23d86ad2121b3c4fc78c58f95e19173790e22ac05996df69b84e12da5816cb17"},
+"regex 2023.6.3" = [
+    {url = "https://files.pythonhosted.org/packages/05/bb/72408a1c713e470abe144bce3622d7b1feadd74fab1f9c7fc5e1e4d5917b/regex-2023.6.3-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:cf67ca618b4fd34aee78740bea954d7c69fdda419eb208c2c0c7060bb822d747"},
+    {url = "https://files.pythonhosted.org/packages/09/f5/a9d7f45433797945c3b48e3d19c81378d3d245c5a914a8362351a239e82c/regex-2023.6.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:aad51907d74fc183033ad796dd4c2e080d1adcc4fd3c0fd4fd499f30c03011cd"},
+    {url = "https://files.pythonhosted.org/packages/0c/11/68fe788f176d86cfdec7c8efc70c7dd084d3f6f6a4f2e8c13af8fd09d398/regex-2023.6.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b862c2b9d5ae38a68b92e215b93f98d4c5e9454fa36aae4450f61dd33ff48487"},
+    {url = "https://files.pythonhosted.org/packages/0e/61/6792590a31015cb352a30dd4a09039babbaaa5666d6108f3462a5cd2deb0/regex-2023.6.3-cp37-cp37m-win32.whl", hash = "sha256:9beb322958aaca059f34975b0df135181f2e5d7a13b84d3e0e45434749cb20f7"},
+    {url = "https://files.pythonhosted.org/packages/13/c1/59afc5f6d3c3d34c601df340e51adb3770303b50469b7ab8bcd2348ea279/regex-2023.6.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b4598b1897837067a57b08147a68ac026c1e73b31ef6e36deeeb1fa60b2933c9"},
+    {url = "https://files.pythonhosted.org/packages/14/f3/bfbc8ebdda009249feaf11e51d64b9f5703b570bc71e08132988f9a8d752/regex-2023.6.3-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b6192d5af2ccd2a38877bfef086d35e6659566a335b1492786ff254c168b1693"},
+    {url = "https://files.pythonhosted.org/packages/18/d1/a4571e2050a8fe9e5f6c22e2504693bcf354132ba05333fbaf95846e528d/regex-2023.6.3-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:c2b867c17a7a7ae44c43ebbeb1b5ff406b3e8d5b3e14662683e5e66e6cc868d3"},
+    {url = "https://files.pythonhosted.org/packages/18/df/401fd39ffd50062ff1e0344f95f8e2c141de4fd1eca1677d2f29609e5389/regex-2023.6.3.tar.gz", hash = "sha256:72d1a25bf36d2050ceb35b517afe13864865268dfb45910e2e17a84be6cbfeb0"},
+    {url = "https://files.pythonhosted.org/packages/1c/24/2ba9ef65389e08fc7663d683da5b4ca9ac8731d36861642f8777c99b099c/regex-2023.6.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a99b50300df5add73d307cf66abea093304a07eb017bce94f01e795090dea87c"},
+    {url = "https://files.pythonhosted.org/packages/1e/99/47006c83a6f8aa28a4a22d47803e9d0795f4a2ad25e68c22dbeeb5066b6c/regex-2023.6.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:a8105e9af3b029f243ab11ad47c19b566482c150c754e4c717900a798806b222"},
+    {url = "https://files.pythonhosted.org/packages/21/02/be48cfb817d4c34c3817d245cb3ba232166bfe061237021b601f71d40bf8/regex-2023.6.3-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:61474f0b41fe1a80e8dfa70f70ea1e047387b7cd01c85ec88fa44f5d7561d787"},
+    {url = "https://files.pythonhosted.org/packages/22/db/b004d91e1636f5dd4923bf530017289624d2f38cc9bec37cbb92d163093e/regex-2023.6.3-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:12b74fbbf6cbbf9dbce20eb9b5879469e97aeeaa874145517563cca4029db65c"},
+    {url = "https://files.pythonhosted.org/packages/27/ae/65cb8bacd6c11ebb82b0d72261533cae9115c47fc72984a00b47f9439484/regex-2023.6.3-cp36-cp36m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:87b2a5bb5e78ee0ad1de71c664d6eb536dc3947a46a69182a90f4410f5e3f7dd"},
+    {url = "https://files.pythonhosted.org/packages/28/fd/f5947c44a520a71f7994b2d5e4cf832e4c100f667ad19abdda0287d510f8/regex-2023.6.3-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:36efeba71c6539d23c4643be88295ce8c82c88bbd7c65e8a24081d2ca123da3f"},
+    {url = "https://files.pythonhosted.org/packages/2a/ef/aea4f21dd4c6fc086015ef508763b42a0f5a02eb5d8e89c84bc9b90df9dd/regex-2023.6.3-cp36-cp36m-musllinux_1_1_s390x.whl", hash = "sha256:ee2d1a9a253b1729bb2de27d41f696ae893507c7db224436abe83ee25356f5c1"},
+    {url = "https://files.pythonhosted.org/packages/35/e4/1affff5a828bb63435a73c29ce319d5f9b078ccf3ca45c931b841e713d03/regex-2023.6.3-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:8e3f1316c2293e5469f8f09dc2d76efb6c3982d3da91ba95061a7e69489a14ef"},
+    {url = "https://files.pythonhosted.org/packages/39/22/db126ddbcfd224acb821664f3381ab69c68cceea7c8c05f6ceabb16dfdb7/regex-2023.6.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d77f09bc4b55d4bf7cc5eba785d87001d6757b7c9eec237fe2af57aba1a071d9"},
+    {url = "https://files.pythonhosted.org/packages/4d/bf/5b9039fc53f8ff3905719bca594865ef78cf14b286fe5c493ea0a1c17eb7/regex-2023.6.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:b956231ebdc45f5b7a2e1f90f66a12be9610ce775fe1b1d50414aac1e9206c06"},
+    {url = "https://files.pythonhosted.org/packages/50/6a/cd59b2e1d6817858e3f332b4128e9246bf8408a7a791f8b77b08633a959d/regex-2023.6.3-cp311-cp311-win_amd64.whl", hash = "sha256:09e4a1a6acc39294a36b7338819b10baceb227f7f7dbbea0506d419b5a1dd8af"},
+    {url = "https://files.pythonhosted.org/packages/53/21/0709782f2883c151eeda433116f363289967c60cb0cd9fdd1992d38d3e29/regex-2023.6.3-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:8abbc5d54ea0ee80e37fef009e3cec5dafd722ed3c829126253d3e22f3846f1e"},
+    {url = "https://files.pythonhosted.org/packages/54/90/20898bc1103bc4a493d117ce677195820a7468f48c2f8e70a57502f10fc8/regex-2023.6.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:457b6cce21bee41ac292d6753d5e94dcbc5c9e3e3a834da285b0bde7aa4a11e9"},
+    {url = "https://files.pythonhosted.org/packages/57/64/334ac6ed71e30eb370eeef457e899a176b99bfd367937c0f7e723c604e76/regex-2023.6.3-cp310-cp310-win_amd64.whl", hash = "sha256:c5f8037000eb21e4823aa485149f2299eb589f8d1fe4b448036d230c3f4e68e0"},
+    {url = "https://files.pythonhosted.org/packages/5a/a9/02c49ceb346a0bc6fbfe591c25cbd436a85a9af3458d418563c72c3ac738/regex-2023.6.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c123f662be8ec5ab4ea72ea300359023a5d1df095b7ead76fedcd8babbedf969"},
+    {url = "https://files.pythonhosted.org/packages/5e/a8/2e3626392c4fcf7e3920cae166155542838be2048384989e2c6f024b793d/regex-2023.6.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:051da80e6eeb6e239e394ae60704d2b566aa6a7aed6f2890a7967307267a5dc6"},
+    {url = "https://files.pythonhosted.org/packages/5f/59/773cf93716a073555d2245bc85efd47ae36d042ba21a306927c58e4aeb8b/regex-2023.6.3-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:43e1dd9d12df9004246bacb79a0e5886b3b6071b32e41f83b0acbf293f820ee8"},
+    {url = "https://files.pythonhosted.org/packages/62/eb/5a94c917a2b94ad467854110c880b9e92e2127925ac82e6ea6b6f36f502d/regex-2023.6.3-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:3e5219bf9e75993d73ab3d25985c857c77e614525fac9ae02b1bebd92f7cecac"},
+    {url = "https://files.pythonhosted.org/packages/66/60/a46aa9c8c4a806676d384036858f12720c975d47d4306dd8dfecfec24093/regex-2023.6.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:d54af539295392611e7efbe94e827311eb8b29668e2b3f4cadcfe6f46df9c777"},
+    {url = "https://files.pythonhosted.org/packages/66/bc/c328b4cba36217a5b865c36e0908f198eb030ebd8a138c630ed7f3ee3cdd/regex-2023.6.3-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:65ba8603753cec91c71de423a943ba506363b0e5c3fdb913ef8f9caa14b2c7e0"},
+    {url = "https://files.pythonhosted.org/packages/6e/e7/2750bbfb1241d22a3be92c5c9905d1cd64c13ab3f1698970aa130d9f3094/regex-2023.6.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ea353ecb6ab5f7e7d2f4372b1e779796ebd7b37352d290096978fea83c4dba0c"},
+    {url = "https://files.pythonhosted.org/packages/70/a6/b5b6fbe09e7e3be38715877dbbd28b47d026bb90e2aa93e7d0cec54ddf59/regex-2023.6.3-cp36-cp36m-win_amd64.whl", hash = "sha256:bbb02fd4462f37060122e5acacec78e49c0fbb303c30dd49c7f493cf21fc5b27"},
+    {url = "https://files.pythonhosted.org/packages/71/44/81329377dd62a53dfb03cc9fac08e1d9285e3d81195c6dd9f0f0e6513edc/regex-2023.6.3-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:25be746a8ec7bc7b082783216de8e9473803706723b3f6bef34b3d0ed03d57e2"},
+    {url = "https://files.pythonhosted.org/packages/75/cc/1a954e73611375ecf9ccb41521c4e1d46c4b05bb31832acdffca453cfe1b/regex-2023.6.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:837328d14cde912af625d5f303ec29f7e28cdab588674897baafaf505341f2fc"},
+    {url = "https://files.pythonhosted.org/packages/77/0b/05c9e0d2dec2631d552a82e744fecdac3ae2ddf0fe65c8d23174af3a7075/regex-2023.6.3-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:e2fbd6236aae3b7f9d514312cdb58e6494ee1c76a9948adde6eba33eb1c4264f"},
+    {url = "https://files.pythonhosted.org/packages/77/2e/976df13a2aae664271d2c0af547fed4388614d662f8e9621f98a8c3fce9a/regex-2023.6.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:af4dd387354dc83a3bff67127a124c21116feb0d2ef536805c454721c5d7993d"},
+    {url = "https://files.pythonhosted.org/packages/78/26/16a1d719b9867ae7580ad11be9933bfa7efcfc7909fb4ac92c3c893ac1d0/regex-2023.6.3-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:3676f1dd082be28b1266c93f618ee07741b704ab7b68501a173ce7d8d0d0ca18"},
+    {url = "https://files.pythonhosted.org/packages/7a/2b/202aa672ad6963d61033de28fc5077f4fbe2cea391ffc13f0965b38381d8/regex-2023.6.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:d2da3abc88711bce7557412310dfa50327d5769a31d1c894b58eb256459dc289"},
+    {url = "https://files.pythonhosted.org/packages/7a/58/586acf6a0acc3584101865b8a8e6f434c645e3626f738dc28c59fca77c0d/regex-2023.6.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:b28f5024a3a041009eb4c333863d7894d191215b39576535c6734cd88b0fcb68"},
+    {url = "https://files.pythonhosted.org/packages/7a/9d/2f1149fa0ce3bd0d9b5aa40483f88a580d39db7685f3bd7fb2cffb87bf6d/regex-2023.6.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:2d44dc13229905ae96dd2ae2dd7cebf824ee92bc52e8cf03dcead37d926da019"},
+    {url = "https://files.pythonhosted.org/packages/7c/0d/3bef95986d04572a546b750668f0af88d82a7cdb7f5e1aacfb2b5e4159f6/regex-2023.6.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:ccf91346b7bd20c790310c4147eee6ed495a54ddb6737162a36ce9dbef3e4751"},
+    {url = "https://files.pythonhosted.org/packages/84/e7/2ae56083cd0da3da1fe79d61fe4fe6e3ab5f114660a751fecefa77a78225/regex-2023.6.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8f56fcb7ff7bf7404becdfc60b1e81a6d0561807051fd2f1860b0d0348156a07"},
+    {url = "https://files.pythonhosted.org/packages/88/08/7ce5845ffb8a17fb65e6508af6423ace4ff8f6934706ec44d632f97365b5/regex-2023.6.3-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9a5bfb3004f2144a084a16ce19ca56b8ac46e6fd0651f54269fc9e230edb5e4a"},
+    {url = "https://files.pythonhosted.org/packages/8c/0c/020e099c742242b9aa4b378aae99b2c121e6a989168aa1755e1c6da76529/regex-2023.6.3-cp39-cp39-win32.whl", hash = "sha256:20326216cc2afe69b6e98528160b225d72f85ab080cbdf0b11528cbbaba2248f"},
+    {url = "https://files.pythonhosted.org/packages/8d/f2/dbefb119076d67172e032ef325dcfb56dad6bffa690035b3b962294e1946/regex-2023.6.3-cp39-cp39-win_amd64.whl", hash = "sha256:bdff5eab10e59cf26bc479f565e25ed71a7d041d1ded04ccf9aee1d9f208487a"},
+    {url = "https://files.pythonhosted.org/packages/8e/52/647c065f62f113daafda19b4b15af3ce034840e756f95a1f7e21e03fc81c/regex-2023.6.3-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5708089ed5b40a7b2dc561e0c8baa9535b77771b64a8330b684823cfd5116036"},
+    {url = "https://files.pythonhosted.org/packages/8f/16/a80fc1e09a9c9012827197fe1721c2b9e994f9dc36e99a5a397b67564a45/regex-2023.6.3-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:c6a57b742133830eec44d9b2290daf5cbe0a2f1d6acee1b3c7b1c7b2f3606df7"},
+    {url = "https://files.pythonhosted.org/packages/93/99/efdfa7095440c7b29dbe34745b7ec8fbcc578ebf90a9bd40557cd4518824/regex-2023.6.3-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:463b6a3ceb5ca952e66550a4532cef94c9a0c80dc156c4cc343041951aec1697"},
+    {url = "https://files.pythonhosted.org/packages/95/bf/b102bd6c3ffe15520cc363064be5f230d2f9dabba2c58bf2f07a584d02e5/regex-2023.6.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dcba6dae7de533c876255317c11f3abe4907ba7d9aa15d13e3d9710d4315ec0e"},
+    {url = "https://files.pythonhosted.org/packages/98/a1/877f80246e3a5158574d7344a6e7adda9ddb9ddc427120928bdf74879383/regex-2023.6.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:890e5a11c97cf0d0c550eb661b937a1e45431ffa79803b942a057c4fb12a2da2"},
+    {url = "https://files.pythonhosted.org/packages/99/f2/aec602e73e83d752a5bf8b0b2c78ec3750c02877c8347fba84b33588b02e/regex-2023.6.3-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:6b2675068c8b56f6bfd5a2bda55b8accbb96c02fd563704732fd1c95e2083461"},
+    {url = "https://files.pythonhosted.org/packages/9b/dd/107ec7fb8878e0ebfb88431654f6ba4b57c6c5780a03771185771f05aa29/regex-2023.6.3-cp38-cp38-win32.whl", hash = "sha256:f415f802fbcafed5dcc694c13b1292f07fe0befdb94aa8a52905bd115ff41e88"},
+    {url = "https://files.pythonhosted.org/packages/9b/fd/f2997b42d40b1efbfdf14f7d0955df148a3ba3bfbc881927cde95e1f7467/regex-2023.6.3-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:742e19a90d9bb2f4a6cf2862b8b06dea5e09b96c9f2df1779e53432d7275331f"},
+    {url = "https://files.pythonhosted.org/packages/9d/1e/8eb13233ac58edecdd58aa7de0d5b68fc04f7141891c1934036b0b34890a/regex-2023.6.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7178bbc1b2ec40eaca599d13c092079bf529679bf0371c602edaa555e10b41c3"},
+    {url = "https://files.pythonhosted.org/packages/a2/65/a829d07e13818d720b2aca34550a4f166b86ad729997372b65c5a4aff281/regex-2023.6.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e5087a3c59eef624a4591ef9eaa6e9a8d8a94c779dade95d27c0bc24650261cd"},
+    {url = "https://files.pythonhosted.org/packages/a4/06/85618f80ae552ac309ead9702c6826edda27884e26e07fdc8fa93f283546/regex-2023.6.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4959e8bcbfda5146477d21c3a8ad81b185cd252f3d0d6e4724a5ef11c012fb06"},
+    {url = "https://files.pythonhosted.org/packages/a6/2f/4a0afe16db5ee680d346aed1bfc1ef73c185e84749b7de870440e7abf740/regex-2023.6.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:0385e73da22363778ef2324950e08b689abdf0b108a7d8decb403ad7f5191938"},
+    {url = "https://files.pythonhosted.org/packages/a6/69/43403293ea75b7581355b44f2323f21af54473fc2932743b4290b539fc08/regex-2023.6.3-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:6343c6928282c1f6a9db41f5fd551662310e8774c0e5ebccb767002fcf663ca9"},
+    {url = "https://files.pythonhosted.org/packages/aa/0d/e2e195252b00a1a265e93b8b03ff4b71f59e1ce543b302110f96f1725335/regex-2023.6.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:9edce5281f965cf135e19840f4d93d55b3835122aa76ccacfd389e880ba4cf82"},
+    {url = "https://files.pythonhosted.org/packages/aa/fd/3f117ca6778e373fa73ecb9f0ca2b7bf6b65d0546556876055fb59e8f4b1/regex-2023.6.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:10cb847aeb1728412c666ab2e2000ba6f174f25b2bdc7292e7dd71b16db07568"},
+    {url = "https://files.pythonhosted.org/packages/ac/c2/0775e121b4e57de3b79eb140b4e1f0af5d9069f27e82e18d39e28ec0111f/regex-2023.6.3-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:83320a09188e0e6c39088355d423aa9d056ad57a0b6c6381b300ec1a04ec3d16"},
+    {url = "https://files.pythonhosted.org/packages/ac/e1/5647cd9d8131d2d8b39cf02ded3799b21ab17434d1764fc2df9523ea3ad1/regex-2023.6.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0c29ca1bd61b16b67be247be87390ef1d1ef702800f91fbd1991f5c4421ebae8"},
+    {url = "https://files.pythonhosted.org/packages/b0/f9/edd425bc07291257380b6805662123bceb684b027ea4b8878368da8192e5/regex-2023.6.3-cp36-cp36m-musllinux_1_1_ppc64le.whl", hash = "sha256:d831c2f8ff278179705ca59f7e8524069c1a989e716a1874d6d1aab6119d91d1"},
+    {url = "https://files.pythonhosted.org/packages/b4/f0/7d5ea7e4a9badd4a7313ce1819d11b992ae531dfcf054eb3fa81bfb6fd19/regex-2023.6.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:74419d2b50ecb98360cfaa2974da8689cb3b45b9deff0dcf489c0d333bcc1477"},
+    {url = "https://files.pythonhosted.org/packages/b6/1a/c0219bdc19572a62a1506267d680cfadf2e0b21739f8d350eaf77e6e77e1/regex-2023.6.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:7117d10690c38a622e54c432dfbbd3cbd92f09401d622902c32f6d377e2300ee"},
+    {url = "https://files.pythonhosted.org/packages/c2/ef/f4756e6f12acebf3fddaab1c4424a7de671ed177d570977b9045b2412065/regex-2023.6.3-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:5c6b48d0fa50d8f4df3daf451be7f9689c2bde1a52b1225c5926e3f54b6a9ed1"},
+    {url = "https://files.pythonhosted.org/packages/c4/3d/d7ed16c298101bc7f5e3a65aef1ab34c1d7e1a89893491a4b1faf20701aa/regex-2023.6.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4d3850beab9f527f06ccc94b446c864059c57651b3f911fddb8d9d3ec1d1b25d"},
+    {url = "https://files.pythonhosted.org/packages/c4/6d/f00a81a218f05538dd13b1fb4cd7fabf313fde41670f7b5265b52d50cbce/regex-2023.6.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e8915cc96abeb8983cea1df3c939e3c6e1ac778340c17732eb63bb96247b91d2"},
+    {url = "https://files.pythonhosted.org/packages/c6/6b/1d3757fe15d8df87ec0e10bed569d1818cc6ea312b5769ebfac12da81319/regex-2023.6.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:10590510780b7541969287512d1b43f19f965c2ece6c9b1c00fc367b29d8dce7"},
+    {url = "https://files.pythonhosted.org/packages/c7/fa/7959acb8578faa8f386cf6add5a85685d147f2695756b0411c082cc36fcf/regex-2023.6.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:976d7a304b59ede34ca2921305b57356694f9e6879db323fd90a80f865d355a3"},
+    {url = "https://files.pythonhosted.org/packages/ca/6f/8280b66724aa5443af51fdf9fd20899237b7d0e8cb87d2a7bea208c22ff8/regex-2023.6.3-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:29cdd471ebf9e0f2fb3cac165efedc3c58db841d83a518b082077e612d3ee5df"},
+    {url = "https://files.pythonhosted.org/packages/ca/af/13ecdd9a0f82de8f888917d08327f0e5e56875f6d3751bad9906ec994902/regex-2023.6.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:271f0bdba3c70b58e6f500b205d10a36fb4b58bd06ac61381b68de66442efddb"},
+    {url = "https://files.pythonhosted.org/packages/cd/c3/c97e8ed1ba9cdd35aaa82aa5c2be752a0cda44e77aeb22810e547877405b/regex-2023.6.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:05ed27acdf4465c95826962528f9e8d41dbf9b1aa8531a387dee6ed215a3e9ef"},
+    {url = "https://files.pythonhosted.org/packages/d5/9d/735ff91370569d5df0f3c26f0e95485728483e85da31daed2a0fd964eb8f/regex-2023.6.3-cp310-cp310-win32.whl", hash = "sha256:dbbbfce33cd98f97f6bffb17801b0576e653f4fdb1d399b2ea89638bc8d08ae1"},
+    {url = "https://files.pythonhosted.org/packages/db/63/b6d7bd7a7c496d02b8ebed4bb2aa3e72f3a5e63e566a4012b976543e8514/regex-2023.6.3-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:0654bca0cdf28a5956c83839162692725159f4cda8d63e0911a2c0dc76166525"},
+    {url = "https://files.pythonhosted.org/packages/dd/90/100a9544f5ada8160e8b47a6c85e1a34dfd9aa8fef349c5e619808ba62be/regex-2023.6.3-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:74390d18c75054947e4194019077e243c06fbb62e541d8817a0fa822ea310c14"},
+    {url = "https://files.pythonhosted.org/packages/dd/f4/4ca224e4366eb9605c78e4005c7abe6af77cf81d9754e1d39251a27d0731/regex-2023.6.3-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:9427a399501818a7564f8c90eced1e9e20709ece36be701f394ada99890ea4b3"},
+    {url = "https://files.pythonhosted.org/packages/e1/35/b9152dc20b385459b2533cc8f81212eb9835469e5aa0ce3d38386df788bd/regex-2023.6.3-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:bb60b503ec8a6e4e3e03a681072fa3a5adcbfa5479fa2d898ae2b4a8e24c4591"},
+    {url = "https://files.pythonhosted.org/packages/e3/66/7fead0a8c429d2b0c2a0507546395f10b0317ff59a28b02ade491b163277/regex-2023.6.3-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:687ea9d78a4b1cf82f8479cab23678aff723108df3edeac098e5b2498879f4a7"},
+    {url = "https://files.pythonhosted.org/packages/e5/8d/f4ab1cc6c34a664eab76a141d3184ffe58bc91f8e51f81609b11709ce03c/regex-2023.6.3-cp36-cp36m-win32.whl", hash = "sha256:0b71e63226e393b534105fcbdd8740410dc6b0854c2bfa39bbda6b0d40e59a54"},
+    {url = "https://files.pythonhosted.org/packages/e5/92/12ba400c17f36b48c62c3bbfada39efce1757f41b72e52930b55bcdb71c5/regex-2023.6.3-cp311-cp311-win32.whl", hash = "sha256:fb5ec16523dc573a4b277663a2b5a364e2099902d3944c9419a40ebd56a118f9"},
+    {url = "https://files.pythonhosted.org/packages/e6/92/e13fc1421ed8d8a2abf8e3e5e115ce863eb97e4f1548285d9ef9c27f4e7a/regex-2023.6.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a4c3b7fa4cdaa69268748665a1a6ff70c014d39bb69c50fda64b396c9116cf77"},
+    {url = "https://files.pythonhosted.org/packages/e7/fc/6e4fab6dc7b1a2d521f2e9dd5380c6b2453770a0f425021d744d29c47a89/regex-2023.6.3-cp37-cp37m-win_amd64.whl", hash = "sha256:fea75c3710d4f31389eed3c02f62d0b66a9da282521075061ce875eb5300cf23"},
+    {url = "https://files.pythonhosted.org/packages/ec/1a/54672edc40464035adcb4df336399882c39bc8cec32f0cafc2a589bd423a/regex-2023.6.3-cp38-cp38-win_amd64.whl", hash = "sha256:d4f03bb71d482f979bda92e1427f3ec9b220e62a7dd337af0aa6b47bf4498f72"},
+    {url = "https://files.pythonhosted.org/packages/f1/d7/a207054d18af0a086566bed2b51a85c00a1a631fdcf7cdcb942554e85211/regex-2023.6.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:841d6e0e5663d4c7b4c8099c9997be748677d46cbf43f9f471150e560791f7ff"},
+    {url = "https://files.pythonhosted.org/packages/f4/59/de8f00338fa853b1616e3ea3a335565dea69057fd68c8d159055a90a563f/regex-2023.6.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:2239d95d8e243658b8dbb36b12bd10c33ad6e6933a54d36ff053713f129aa536"},
+    {url = "https://files.pythonhosted.org/packages/f4/78/23a351b0aa381cb38ed7b6da8ced8522a57c1f333b78872c1940cde63da7/regex-2023.6.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:824bf3ac11001849aec3fa1d69abcb67aac3e150a933963fb12bda5151fe1bfd"},
+    {url = "https://files.pythonhosted.org/packages/f4/89/3c20ba852caf53109664be290bc1cc0802bffd2a8f2390175d157fdbecab/regex-2023.6.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e0bb18053dfcfed432cc3ac632b5e5e5c5b7e55fb3f8090e867bfd9b054dbcbf"},
+    {url = "https://files.pythonhosted.org/packages/f8/bc/01e6a5597904147d13c1a6dc16ec334b73cddb190b6b8f05fca2c0bfbe89/regex-2023.6.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:9edcbad1f8a407e450fbac88d89e04e0b99a08473f666a3f3de0fd292badb6aa"},
+    {url = "https://files.pythonhosted.org/packages/f9/a5/703d590158a252b3e96332d7a420669b0395b7b98a2b34395af1f4f8f95f/regex-2023.6.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0b49c764f88a79160fa64f9a7b425620e87c9f46095ef9c9920542ab2495c8bc"},
 ]
 "requests 2.24.0" = [
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
-"rich 13.3.5" = [
-    {url = "https://files.pythonhosted.org/packages/39/03/6de23bdd88f5ee7f8b03f94f6e88108f5d7ffe6d207e95cdb06d9aa4cd57/rich-13.3.5-py3-none-any.whl", hash = "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"},
-    {url = "https://files.pythonhosted.org/packages/3d/0b/8dd34d20929c4b5e474db2e64426175469c2b7fea5ba71c6d4b3397a9729/rich-13.3.5.tar.gz", hash = "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c"},
+"rich 13.4.1" = [
+    {url = "https://files.pythonhosted.org/packages/02/97/0046b5e3c6a5057b5817e5e6c51a776d410b953e6a9c67ae249dafdd2999/rich-13.4.1.tar.gz", hash = "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1"},
+    {url = "https://files.pythonhosted.org/packages/ea/93/c68645c689d10a035010e3ae314b6b2855d040ce0d11fdfdfbb8be416581/rich-13.4.1-py3-none-any.whl", hash = "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"},
 ]
 "ruff 0.0.270" = [
     {url = "https://files.pythonhosted.org/packages/02/d1/77f9425bea1e5a929ecbeb3fd9e2e0931e30751b4d75bbe8b46e14408ada/ruff-0.0.270-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:643de865fd35cb76c4f0739aea5afe7b8e4d40d623df7e9e6ea99054e5cead0a"},
     {url = "https://files.pythonhosted.org/packages/06/56/39079c40dc7e995f26f630d28dec11b1b63f498bfb56409adda27300bf2f/ruff-0.0.270-py3-none-win_amd64.whl", hash = "sha256:0012f9b7dc137ab7f1f0355e3c4ca49b562baf6c9fa1180948deeb6648c52957"},
     {url = "https://files.pythonhosted.org/packages/36/21/aa8e1d22756e1d3bcdb43f4d25451f8978cacd9d6896e365bb7c1f9037fa/ruff-0.0.270-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:08188f8351f4c0b6216e8463df0a76eb57894ca59a3da65e4ed205db980fd3ae"},
     {url = "https://files.pythonhosted.org/packages/36/ab/ff2870e22556c780d6b0b2934152e824ca0d3d40d9e3dedb44a158a979dc/ruff-0.0.270-py3-none-musllinux_1_2_i686.whl", hash = "sha256:0bbfbf6fd2436165566ca85f6e57be03ed2f0a994faf40180cfbb3604c9232ef"},
     {url = "https://files.pythonhosted.org/packages/40/82/c393794c4cd462ffbd0afe45b8e77c174c7f3d5df4340ecead9a42d1fa53/ruff-0.0.270-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0827b074635d37984fc98d99316bfab5c8b1231bb83e60dacc83bd92883eedb4"},
@@ -3113,17 +3113,17 @@
     {url = "https://files.pythonhosted.org/packages/39/c3/205e88f02959712b62008502952707313640369144a7fded4cbc61f48321/traitlets-5.9.0.tar.gz", hash = "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"},
     {url = "https://files.pythonhosted.org/packages/77/75/c28e9ef7abec2b7e9ff35aea3e0be6c1aceaf7873c26c95ae1f0d594de71/traitlets-5.9.0-py3-none-any.whl", hash = "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8"},
 ]
 "typer 0.7.0" = [
     {url = "https://files.pythonhosted.org/packages/0d/44/56c3f48d2bb83d76f5c970aef8e2c3ebd6a832f09e3621c5395371fe6999/typer-0.7.0-py3-none-any.whl", hash = "sha256:b5e704f4e48ec263de1c0b3a2387cd405a13767d2f907f44c1a08cbad96f606d"},
     {url = "https://files.pythonhosted.org/packages/e1/45/bcbc581f87c8d8f2a56b513eb994d07ea4546322818d95dc6a3caf2c928b/typer-0.7.0.tar.gz", hash = "sha256:ff797846578a9f2a201b53442aedeb543319466870fbe1c701eab66dd7681165"},
 ]
-"typing-extensions 4.6.2" = [
-    {url = "https://files.pythonhosted.org/packages/38/60/300ad6f93adca578bf05d5f6cd1d854b7d140bebe2f9829561aa9977d9f3/typing_extensions-4.6.2-py3-none-any.whl", hash = "sha256:3a8b36f13dd5fdc5d1b16fe317f5668545de77fa0b8e02006381fd49d731ab98"},
-    {url = "https://files.pythonhosted.org/packages/be/fc/3d12393d634fcb31d5f4231c28feaf4ead225124ba08021046317d5f450d/typing_extensions-4.6.2.tar.gz", hash = "sha256:06006244c70ac8ee83fa8282cb188f697b8db25bc8b4df07be1873c43897060c"},
+"typing-extensions 4.6.3" = [
+    {url = "https://files.pythonhosted.org/packages/42/56/cfaa7a5281734dadc842f3a22e50447c675a1c5a5b9f6ad8a07b467bffe7/typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
+    {url = "https://files.pythonhosted.org/packages/5f/86/d9b1518d8e75b346a33eb59fa31bdbbee11459a7e2cc5be502fa779e96c5/typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
 ]
 "tzdata 2023.3" = [
     {url = "https://files.pythonhosted.org/packages/70/e5/81f99b9fced59624562ab62a33df639a11b26c582be78864b339dafa420d/tzdata-2023.3.tar.gz", hash = "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a"},
     {url = "https://files.pythonhosted.org/packages/d5/fb/a79efcab32b8a1f1ddca7f35109a50e4a80d42ac1c9187ab46522b2407d7/tzdata-2023.3-py2.py3-none-any.whl", hash = "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"},
 ]
 "tzlocal 5.0.1" = [
     {url = "https://files.pythonhosted.org/packages/84/d2/730a87f0dbf184760394a85088d0d2366a5a8a32bc32ffd869a83f1de854/tzlocal-5.0.1-py3-none-any.whl", hash = "sha256:f3596e180296aaf2dbd97d124fe76ae3a0e3d32b258447de7b939b3fd4be992f"},
@@ -3313,49 +3313,62 @@
     {url = "https://files.pythonhosted.org/packages/fb/2d/060ab740f64ea6ea2088e375c3046839faaf4bbba2b65a5364668bd765e7/yarl-1.9.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59"},
     {url = "https://files.pythonhosted.org/packages/fe/7d/9d85f658b6f7c041ca3ba371d133040c4dc41eb922aef0a6ba917291d187/yarl-1.9.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb"},
 ]
 "yt-dlp 2023.3.4" = [
     {url = "https://files.pythonhosted.org/packages/a7/df/498c57f641e9993376cf52489047158e6d660e8bab06b72c470ad5cce2bd/yt_dlp-2023.3.4-py2.py3-none-any.whl", hash = "sha256:40ca421407ce07c8fd700854fd978d58526ec6fff3468caa34ff1c7333b8dc34"},
     {url = "https://files.pythonhosted.org/packages/e8/4a/1e01f24fcb49191626e2b17d00e13a093315d03a9da09fccb1c75913e420/yt-dlp-2023.3.4.tar.gz", hash = "sha256:265d5da97a76c15d7d9a4088a67b78acd5dcf6f8cfd8257c52f581ff996ff515"},
 ]
-"zeroconf 0.63.0" = [
-    {url = "https://files.pythonhosted.org/packages/02/80/9aa80564b42f6d62c3395569b13533e0bef3a5c03ac6df8e5bdc376ff8d4/zeroconf-0.63.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8142e423ce780ef45229ae47f0df8474eb9fab41b6ccea25206330a40c79cbbe"},
-    {url = "https://files.pythonhosted.org/packages/08/77/364326b5600326e115e982fc6bdb53c80e922e35ac0759ffc26cce4cf295/zeroconf-0.63.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:867b0aefd32239e69a7919d95a8bcaf97e3e40fd05c25f5cd5c1e5e50326ca6e"},
-    {url = "https://files.pythonhosted.org/packages/11/f3/c0a9098ee84bfef2eb57b7aca04f244dece53197e0d3cad1e6bea72bb22d/zeroconf-0.63.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:934d468f91885ceb4a530507689c416a1e158a11170f2a90bad3643090c19bac"},
-    {url = "https://files.pythonhosted.org/packages/13/85/4a85da8c81beda97d0a85b81bbcadb66959491fd83dbfa0edcad1bcdb4bc/zeroconf-0.63.0-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:ce5ff7ee9e27cd45567d7f9335426c95dd23b3a80f4c47e3edd2db5560861f96"},
-    {url = "https://files.pythonhosted.org/packages/14/fa/d015cd3ad08a137b5e5d6ede2c6da7493dbd47ca0d3f02b2d8efd1313a00/zeroconf-0.63.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:bc4e5fc6e5ac1d9bcf538fdbbbcb4794c8f19039e9cb344a23260507e506cb10"},
-    {url = "https://files.pythonhosted.org/packages/15/0b/e8214d69531f054db380ead35b2ea1c14be1ce19eceb863be6fcc94418b3/zeroconf-0.63.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:c360ee0fed2776f4f95008159d59fae1080a91308865297a29941895d8da0de4"},
-    {url = "https://files.pythonhosted.org/packages/19/9a/9cb1ddeedd774e7e1c9350806bbcf8e06af054dc85b7ce9bce5f7877a1c6/zeroconf-0.63.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:fa11e9ee5436c5a4436c72a23bb08e509b38157611eecece0a8e44191129442c"},
-    {url = "https://files.pythonhosted.org/packages/1a/8d/328a856d217f2248a926803309841fdcd1121b8f6c387af5207fe883cf9b/zeroconf-0.63.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d9837c1a2952c72b75e906e353801822bde6e0d2521c1572d2c0e39d840d648e"},
-    {url = "https://files.pythonhosted.org/packages/36/53/b51a621fc7b18a8006626e3a2a046f27d98b0f4091e08866c0c082e09947/zeroconf-0.63.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:545f433782e2c114b0ab4301d015ee0347036896591238fb0f18433e5eacfc1c"},
-    {url = "https://files.pythonhosted.org/packages/38/ae/b534effd941cc0a2b1cea84b50b2b31f8fe33eb4d439625f3ecc2caaa7e3/zeroconf-0.63.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:a7a6f4afc6c951098f15b9064d5d2b749b64cff8df7f553a5cc38b7b37cce166"},
-    {url = "https://files.pythonhosted.org/packages/41/20/8a12dc796fba28deed4e89417ad7278704b99eace362a98c9253a0b14ad3/zeroconf-0.63.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b864e25bb6cf0d588559caa70177e11bf1bc1c8f78911587cc280f382980c596"},
-    {url = "https://files.pythonhosted.org/packages/46/64/f3f55dc5dba216ce9d20062b6fe5862e49a63b7ecce1c941388618f89224/zeroconf-0.63.0.tar.gz", hash = "sha256:2643b1c9c6ffdfaa1313cf3d12ea0099482fcb3da77929a08be87fc8354d0b3d"},
-    {url = "https://files.pythonhosted.org/packages/50/0f/abab207c6b628ff39cec1bb63ed3469b4aa61eec3b2e6b0bfe45bfe507db/zeroconf-0.63.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:62d634a2e6eb5fd38930ad571d6e44e3095f1482966d7af31470738991c652af"},
-    {url = "https://files.pythonhosted.org/packages/57/54/00e810344ec1be1ad7999438c56a4f7d1f71c2bd5fd860386bce56dd2a11/zeroconf-0.63.0-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:08c91b62f0e21bd55a89718957397d671e439b917404102da2d24acb42e718cb"},
-    {url = "https://files.pythonhosted.org/packages/60/0e/f486a01b052981281c7b376dda078df6b84f817ec3824441cbb3c342d6d7/zeroconf-0.63.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0525f0c1ae03b695c6a1e181e17d35cc563494edb5e12424828f4cb8d7599228"},
-    {url = "https://files.pythonhosted.org/packages/6e/bb/12ddf36fd85db0b15d446ceb740cf1d05d1df205ba84888edf03c519f561/zeroconf-0.63.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:34caa7a1640c84457f517421401214122134a0979046925741d51e881e1012e1"},
-    {url = "https://files.pythonhosted.org/packages/79/54/924592e816205f57d934e02e4175667d9571bd40cb210cd9cef1340b9f5c/zeroconf-0.63.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:e14b99b35d7df8fdc9fa88f3792f523da89eddbc41ad4e3ecc289a42e7145665"},
-    {url = "https://files.pythonhosted.org/packages/8a/f3/526afcb7f35476876fdc55f4256edd974233466d70891e44ff01d610c4c3/zeroconf-0.63.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3c293358918fb511aae4ea0602f20845854406cfc6e9606b5b3b5afa7b68a3b4"},
-    {url = "https://files.pythonhosted.org/packages/90/7a/79e216875ef7b59019673fe45b0997eb305ecb5af51371303d0bff8081be/zeroconf-0.63.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:18a804537b5cfa96715ed32afac454981dbd152e031d87e2504a6ca24865ff8b"},
-    {url = "https://files.pythonhosted.org/packages/91/43/1aa906bd9cefcd99e64f4dcbb60d693253d5bbd335ae658afd49f44b9635/zeroconf-0.63.0-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:2b4c4f256c16129da53553a99a95eaded4e6dd9bd094fcd48478eb7273f7c7c1"},
-    {url = "https://files.pythonhosted.org/packages/9c/e8/03f37a2fb6260db133fc975e159f308345b2d487eea3c1974de28658a3cf/zeroconf-0.63.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:be7b119699c2e91d922d4a70fc12514e2b49522e95b17eeddcbca38f3409035b"},
-    {url = "https://files.pythonhosted.org/packages/9e/55/3fb6a4382ce45e61d1ed0ad2027767759e6760fdc7c357be39d29d2326c5/zeroconf-0.63.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e6763fb33a66664b24c0674d0188943e93e7ac6e0e8cf6fe104658f0697bf670"},
-    {url = "https://files.pythonhosted.org/packages/b1/e9/afcae6888a52538082b4659be5308d2804a10e0533934c2cc4c564b786b7/zeroconf-0.63.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6947b13576667122b03b02f580c6f532b134e097efbf1f0660ba84620c6fa4b2"},
-    {url = "https://files.pythonhosted.org/packages/c4/cc/928066b3947f802a412de71df59019d382468c116d3969d332bb4f6e6e4d/zeroconf-0.63.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:f439a5fe58d0c736484017fc49c847e8a00aafe035f199cce35a32b6c76f6e95"},
-    {url = "https://files.pythonhosted.org/packages/c9/9a/6a53221cae1f0233a56137b329945f32b8eda3410b88bcc0f195ed84c8a5/zeroconf-0.63.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:23dc430300e78c1515bd2c42fdff1fc813f12f16e6cfe7faccaa89893d193b92"},
-    {url = "https://files.pythonhosted.org/packages/cf/00/6bc23edb28fd1b5d87b993a24326568e721b202545e8c5b309a0ea08136d/zeroconf-0.63.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:764206721e29395b7d5f0427006b168ca1c30cadac6b0414f83c9c62584b1447"},
-    {url = "https://files.pythonhosted.org/packages/d2/26/3cb6925dc295b0a018fb99aeb7e2299a71e48004356e7ff60092e44a73a0/zeroconf-0.63.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:a3b2bd53e9c95c9c7f63feb6238fc046866cc86cf511dd64c926836e33ba8f85"},
-    {url = "https://files.pythonhosted.org/packages/e1/39/d4ac426bac2aef9cf3d4e8223905b5aa6f3f18909dc7e4556fdc3d85919e/zeroconf-0.63.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:981c8cce4571733a96d6f6f32b3cde30608f0fb316f073694713b3f18506ba8c"},
-    {url = "https://files.pythonhosted.org/packages/e5/37/7a8b72a5f7a1b0c6a4339c25adbc5a61dbf3c0e3e0cdc4ff897a85f57db9/zeroconf-0.63.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:7028ae059f01891a257a83a7c25db266d0c61f963b4f03c905084bf21fcea810"},
-    {url = "https://files.pythonhosted.org/packages/e7/18/f046e990e8055ed324655849a914127b2320699df38cb8b70c121e4f7e05/zeroconf-0.63.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:90764ba95fc410cd5da89d6b60c3e5a52a506ac9d841d3f78a95f44ea8ef23f0"},
-    {url = "https://files.pythonhosted.org/packages/eb/11/5ca71b5f173e5fde9180f151bc323c53eba42d2792966edb12cf755a3959/zeroconf-0.63.0-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:664678b9e271a4a6d983366f4241049795f71c0f53025293ed83901d4e19007e"},
-    {url = "https://files.pythonhosted.org/packages/ec/ac/76652d5ffed387d2a43d98a0cb23bdbe3a8c13ca3d7f87aa57ccec1aebe2/zeroconf-0.63.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:d4cd16ccd966d55378737c8ec772795528dc7d58048379c7bc5111a54df38c35"},
-    {url = "https://files.pythonhosted.org/packages/f4/21/f354720c0eee7398b3b81a26913664535a5209af770115ca411b22ec5721/zeroconf-0.63.0-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:f4d09317893e618cf3dd3b0a56abb2c008f3ae0148ffed8409120a3801ecad8d"},
-    {url = "https://files.pythonhosted.org/packages/f7/10/ceb9a1ff94be25a151dc15724ac95a2b0d9446aff39e9b980908d061402f/zeroconf-0.63.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:0ca4d685d441b9acf9c078f0a25d32e9af78a01070afbbf7441084eff90c69bd"},
-    {url = "https://files.pythonhosted.org/packages/f7/7d/6b05abbb1162f02ceb25b94caa3edde44c1aaf10d5d2d2a83563074a89e0/zeroconf-0.63.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:a4c68e89762eee873ec949c43c2190f5f6a75380f4648f7dcf0de7463f79e259"},
-    {url = "https://files.pythonhosted.org/packages/ff/a2/4cea466717eea9d33e0a0dedcfe7d01b1f133cdcccebe93f526958bf5b3d/zeroconf-0.63.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2dafe39f657e0d009663332d1a4466666c5047c5f66a6ddacb1a577b1dffac3c"},
+"zeroconf 0.64.1" = [
+    {url = "https://files.pythonhosted.org/packages/00/d8/f458e724741859bbd95b28c37bf3f35ad3c1400fc33795a330922eb4bb2d/zeroconf-0.64.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5f6f15be681889bbdcd2ef98ddd9753f5d158bf45a3d29708cefd84a5b704f7e"},
+    {url = "https://files.pythonhosted.org/packages/1d/a9/68534a61caea8345ff7358e24f99732d44fbefba9bb01af731dc375a4c03/zeroconf-0.64.1-cp311-cp311-win_amd64.whl", hash = "sha256:f13d20fccda4a8e0d1f654336f0163b3a64e6ce111573245d88e15e4598fddc1"},
+    {url = "https://files.pythonhosted.org/packages/21/06/3d9381e80714da1ba2f6887708c0dfe8c6903ee4b3509249704d78478d0a/zeroconf-0.64.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:1698e085ea350772dd0cf828888bf83d3f25ae94f213fff31a01c77f498511b0"},
+    {url = "https://files.pythonhosted.org/packages/31/8f/ce3402ec68b11429880a1dc840ea5f3c0792268350db248996be4d8e92bb/zeroconf-0.64.1-cp38-cp38-win32.whl", hash = "sha256:23c37b785a5141bf392f809fd7f21267f57458042081c76b3fcf5a1305890dff"},
+    {url = "https://files.pythonhosted.org/packages/37/88/fac09749a3d98016237c914d1d002d33c04e7788f087e3992e94e4c86d28/zeroconf-0.64.1-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:3e3da076095a575bdecd2e0fa03294d0ae243d20de8aa40d352ce98fa403b866"},
+    {url = "https://files.pythonhosted.org/packages/3d/53/26b929bed81f50597bb3b8abedad6bef2b98d7b59107c2276bee66ab0099/zeroconf-0.64.1-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:4cf58733440a17d92190c0b70b71f4a8920559d1c83fcf340415689eb2eec510"},
+    {url = "https://files.pythonhosted.org/packages/44/54/2c725573d61839ec17646ff62931a2f10249dc02bf52236d7c4f1784b7e7/zeroconf-0.64.1-cp310-cp310-win_amd64.whl", hash = "sha256:8daa679bdb0ccc2747127dbfc38b74988229236bab12dc3ee8d8a4d2411070d6"},
+    {url = "https://files.pythonhosted.org/packages/47/be/a15556a8b80a34b92f386cf36f388cd9ca30489a7466a5c658d3813aba0f/zeroconf-0.64.1-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8619e5d0873a27a86bb3739a6b2d30dc4ede35b04814aee7896fe3006f8dbceb"},
+    {url = "https://files.pythonhosted.org/packages/4a/2e/fafb26b35c0c51173ee28ce448db77553df064447895e7858b105fcebac8/zeroconf-0.64.1-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:c6eebc50f8428b16739ac410352c9b80e87587bdd741937055f7ef0860e57623"},
+    {url = "https://files.pythonhosted.org/packages/4b/c8/64f2f42b95ff8cdc020ed2fd8326d60100bd45b21746b3909eac213ce957/zeroconf-0.64.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:718d5c5cbdecffad3ad4c8aee0f0982752bbfd070e0a3f001780840340551d2f"},
+    {url = "https://files.pythonhosted.org/packages/4e/95/e0af3ec7f96265b580199925a10e148c08e5200fea1e1857eaa6257c393e/zeroconf-0.64.1-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:10f6ec14b6c48faf770dc9ebf081659595ed333a9c539acf520c3d898feaeae5"},
+    {url = "https://files.pythonhosted.org/packages/51/31/02a544c2ecf466a992ae620f297eb958b2404f6aaa365a37fe8c796fc80d/zeroconf-0.64.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:b076156e6ea1e4888b019690c60fce96cba967c8fcb28c8bf6d0cc3dc66b600f"},
+    {url = "https://files.pythonhosted.org/packages/53/4e/c16299bc06adca837091538d424303fe3b37ce7322fa61e5d3f102adc66e/zeroconf-0.64.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d58730a1a3ea97e9bd84cda310637eb8eebec76d218e69b13226abb73fe71dbb"},
+    {url = "https://files.pythonhosted.org/packages/59/06/08d2f0139c8993262086babf63367bf721a1f217f90c9229ca98b21e9b1a/zeroconf-0.64.1-cp39-cp39-win_amd64.whl", hash = "sha256:b0b837a2a44d074a859255bf090acd6de2d381994d6b69b873356bdfc1e07f49"},
+    {url = "https://files.pythonhosted.org/packages/6b/1e/75047ca027e5b04ea15f39a573d577fe972f5e639a951f4708a076d34ba9/zeroconf-0.64.1-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:4dc87631691c2c3c0b812c25dfabc78dec903029875216d567e86f08fa7d2c5b"},
+    {url = "https://files.pythonhosted.org/packages/6c/77/b43efbfaa87afa5d72dc6c37c99d309e57015fd8af19e36a527d7cdbd7ed/zeroconf-0.64.1-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:8b7118535d151e604f980c1836a78d6229f10c0c672baeda6e686c512baed8b0"},
+    {url = "https://files.pythonhosted.org/packages/70/b1/304b7bf1db4d8a7cd9a551e3e71091a20300970bd641cfab4e87f0a91a61/zeroconf-0.64.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e8044365e0158d5d0d86c0bcec7e36aa1d8bae0ac639714816352175710230e1"},
+    {url = "https://files.pythonhosted.org/packages/72/36/66a0d78f683e33359802c7ade25fe1623c24a6aaf1ae6d528bf3f2e50d36/zeroconf-0.64.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:5844ae653dc8a96250a91bb6b067ede254ff54af26d9a829ce7c49926679bea0"},
+    {url = "https://files.pythonhosted.org/packages/77/30/c1d765594c551675fa777481727b2b5efb221df97e2a91500541849aabdb/zeroconf-0.64.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:96e4f9fa87ab46c392143aa64cd318ac200c709c66f04556ed3af5783543d415"},
+    {url = "https://files.pythonhosted.org/packages/77/81/dba620d9381a18c2d63c948534f8a45450a09514a83744b7e54afbc9a8e2/zeroconf-0.64.1-cp37-cp37m-win32.whl", hash = "sha256:0c67d13fa459b4e1a660456a3db5fcf43501be5743392f20c75e950dbb036aeb"},
+    {url = "https://files.pythonhosted.org/packages/7a/42/135f53a02178424313168a07d5a520215a78ed13673b11314b5c17fb2a7f/zeroconf-0.64.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4e492f4104879a80fb4320f0577d18982b9deb9333360ff056f823551e1a951d"},
+    {url = "https://files.pythonhosted.org/packages/7a/8e/79223c855c4abf13a5aa7b7ecbf53bf3e504d77abae202488e52b12fcceb/zeroconf-0.64.1.tar.gz", hash = "sha256:e90b2d5d247474b6ccf49bc7e02de516cc459efca6e3ac052b48eeb4a11985af"},
+    {url = "https://files.pythonhosted.org/packages/7e/f0/a09a29b336e9270eff923a457ad87891929503c4b70e5977c5845faba83e/zeroconf-0.64.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:13d18b7a583fe3b1c7825eba4a0c540bc1bcbd9b07763e14b5b684fa4c7bd911"},
+    {url = "https://files.pythonhosted.org/packages/85/02/ad7ed46298e39152dc9b0ddc31a22397db6f5f3b6997224122f8ce87778d/zeroconf-0.64.1-cp38-cp38-win_amd64.whl", hash = "sha256:4eea37ef58a914e0e16f3048011faf137b103ed5f97afa990a166ca91d3c3285"},
+    {url = "https://files.pythonhosted.org/packages/87/85/84b30557b9d62e59ff6e26f6729a686f48882e81fca537b7d2ed53cc727d/zeroconf-0.64.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:c7142fc4a77c58edbd772a73dcd4ce6ac9c5545ea93cf8fb303714e32070544e"},
+    {url = "https://files.pythonhosted.org/packages/8f/e3/e1792a57482e337b2515a9dcba94a44741e4624edf97aa3a79e62cbb1718/zeroconf-0.64.1-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:8eff98ff2f83aaa01d8ada4bf0efa3286b15739f8308cf85fbffbb9f177f10a4"},
+    {url = "https://files.pythonhosted.org/packages/94/41/fedf65eb4802c98ab75644344f2b8b722b04d237754667a391a2909e0d73/zeroconf-0.64.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7a31eba6720e0b58188c66e4b70879bb45b11c41092acbbfd265fe192b428c0c"},
+    {url = "https://files.pythonhosted.org/packages/99/7b/385ec5a78f1c6f6baa23114c09790049be7fce5abcfce5df88af9b2d26ef/zeroconf-0.64.1-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:573d1fe384be94dabe58610bdca3200f9c3505a513d379cf802367d4196a386b"},
+    {url = "https://files.pythonhosted.org/packages/9b/94/bc42ba7bfbe3b83b64b64abe863e2e48948bb5c1f42c29675d7e1d6802a5/zeroconf-0.64.1-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:0a7732a7a6b0b32c8132b7ab2216d492bcb5291bbc6dc3a5afdefe0bc6dbfef5"},
+    {url = "https://files.pythonhosted.org/packages/9f/37/63a17631cbc3cd20ccc563b72c245260e178aa77b47aacce48ba65cafbc5/zeroconf-0.64.1-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:d6bbfb5c297d29e0a3c0ee5a64018001c5e66ea058435197a58edbe73455f4af"},
+    {url = "https://files.pythonhosted.org/packages/a0/7e/07eb46301a8860dde7db6a7be13ebf56e9b3a533e442862d85f6c5013cd6/zeroconf-0.64.1-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:9f8ebbff504bad200275167bfd496a1e1348138f8e92d5d2bd67b650b9677336"},
+    {url = "https://files.pythonhosted.org/packages/a5/54/3ae0de65d5fdb0fa97625c19667d5f02412d3a009b05bc8c4b732a5fc364/zeroconf-0.64.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8dd1f353da75c3a5aef03654826caa3cfed244d1a13675ac6d52816f69d62427"},
+    {url = "https://files.pythonhosted.org/packages/a5/7d/719e02d5b0fd1f8b512685904b12d252c2b05f320e5509b8e5603d6ac0ae/zeroconf-0.64.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:88314f29df7bf568a085decc15c7b60b1b228f646b8e1ffa0ae3c418f8cd28d0"},
+    {url = "https://files.pythonhosted.org/packages/a6/ec/73462bce7b7e8d4c20b0a571bdcc762a32810c696084e87af64775ff5566/zeroconf-0.64.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a74ccda6490bf44ee776850d16df8680a908884c41d800095ca7e716a0e75502"},
+    {url = "https://files.pythonhosted.org/packages/b3/c6/22ee7eeff35e06151162f77c7fe4b506cda1c530742dbdb573e7b331b942/zeroconf-0.64.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:e722131b9fe9e74d5682bc146d5271677154c1af3b45638bf9880d04d9edb869"},
+    {url = "https://files.pythonhosted.org/packages/b5/e4/077c0d84cb7afc28cc70299a74208a698010a1d358bca0661736bb2ad631/zeroconf-0.64.1-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:f5a9766743eac52f91e6dc2d4ac5e7f8f25466f58c0ef51f01f3461920911fdf"},
+    {url = "https://files.pythonhosted.org/packages/b6/cf/1f82d2a6ae12f3d1518318438e74e2973db40a32979c68d440c3e810d774/zeroconf-0.64.1-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:f4551b21aaa42061ffc69af1c32e79775665ac32f662f20f6ee2a7c4db83af6b"},
+    {url = "https://files.pythonhosted.org/packages/c0/86/d49cb22e79a8077dd363f1a3871dc0e14365910fc856f614d887c189a5fd/zeroconf-0.64.1-cp37-cp37m-win_amd64.whl", hash = "sha256:0de5eeeeda68056ba6cab252a1946f67d0aaa950215aa59e5840171561b41f7d"},
+    {url = "https://files.pythonhosted.org/packages/c2/06/7046b7408a6df0f38f7402a34cdd90542a726463a630c7743f7866ad617d/zeroconf-0.64.1-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:06c07e578963fb4448bd1759f241b3ce2cd6062974a1ed8c438bc86f01aed61e"},
+    {url = "https://files.pythonhosted.org/packages/cb/4a/6bc84fdb60aebc9fba701b2c2fe2938fe99682c715001c6b7833b7ec38bf/zeroconf-0.64.1-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:60bdb7a2baa54907854b7d64f71e4da3bedae4a630de576a71a740acaba29957"},
+    {url = "https://files.pythonhosted.org/packages/ce/03/55744d3954d6b7da2b5ae628db1384090f3a27fccfb15fbdfd4b957500f6/zeroconf-0.64.1-cp310-cp310-win32.whl", hash = "sha256:97fbe8c6846b3bc4f4d24c0794fcda05c7e916e91acddae0075500857d5809f5"},
+    {url = "https://files.pythonhosted.org/packages/d3/d2/05f8232bff9d26bdd72ef7f24947e96019d65d909bf7c43c1a61c81f43c0/zeroconf-0.64.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:e9abee5ef2cdd56c866646540c1b75113bb88db16e4860f8abc85aade136fd24"},
+    {url = "https://files.pythonhosted.org/packages/d8/19/e9d5c03cc14a2cc70bb0aa98f2cdc7baa4c496f274e0091eb4d80de52fb1/zeroconf-0.64.1-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:76ef331202523598d6b197a6459551e1d7aaef9f5d60fc1014dc2e23a1a4dde5"},
+    {url = "https://files.pythonhosted.org/packages/dc/3b/e7dbc3ca10f05d0f60d4879282eafd651f252f9ba3ed4a8ed2d921a6c198/zeroconf-0.64.1-cp39-cp39-win32.whl", hash = "sha256:7b5b56df376a74c56d5f3cbaf0f988cfdd86828ac049c81d29aadf4e563eb2f8"},
+    {url = "https://files.pythonhosted.org/packages/e2/73/576a008aed4db514e22709eab6ada3b27ba2092af40d64b13d3d61a40289/zeroconf-0.64.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:66275596a39bb55b0a3d10ee0213080d8087b4dabe500e4fdb851f4eb3c5a597"},
+    {url = "https://files.pythonhosted.org/packages/ed/87/58648e72a28f196a3790520555a8b0ad9fac352f9b0acbf200bc9786ef77/zeroconf-0.64.1-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:1a09997044cf3dd5f24d11b8f17b41a59ee8d04d5cec5b040bd8a3e7b8c86f35"},
+    {url = "https://files.pythonhosted.org/packages/f5/16/94ce16f23aafdab975b9d90f56c9b614800dddc5bf42a0ca7ff0526f3a5a/zeroconf-0.64.1-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:10d3ba25a0d43b4daadc3089fc0446db332e5db6bf1fc41cd6b8a8808082b14e"},
+    {url = "https://files.pythonhosted.org/packages/f7/07/3394fbe745bd7e673569395829b33f40739a65f3329dfed14d4e67f69131/zeroconf-0.64.1-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d7ac86caa31a613d306a35ffd521c83f9420a55e3f6aa279c0edf24f932a2044"},
+    {url = "https://files.pythonhosted.org/packages/fa/0c/31f03decd88171224291c70c8d77c92b927ab751e8378976be38201d69f3/zeroconf-0.64.1-cp311-cp311-win32.whl", hash = "sha256:958465c5229788b685ad4f2b503c4a80aa4376452bbb486fa798655afb2e293e"},
 ]
 "zipp 3.15.0" = [
     {url = "https://files.pythonhosted.org/packages/00/27/f0ac6b846684cecce1ee93d32450c45ab607f65c2e0255f0092032d91f07/zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
     {url = "https://files.pythonhosted.org/packages/5b/fa/c9e82bbe1af6266adf08afb563905eb87cab83fde00a0a08963510621047/zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
 ]
```

### Comparing `xklb-1.29.8/readme.py` & `xklb-1.30.2/readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         f"""
 <details><summary>{title}</summary>
 
     $ library {subcommand} -h
     usage: {getattr(usage, subcommand.replace('-','_'))}
 
 </details>
-"""
+""",
     )
 
 expand_all_js = """```js
 (() => { const readmeDiv = document.getElementById("readme"); const detailsElements = readmeDiv.getElementsByTagName("details"); for (let i = 0; i < detailsElements.length; i++) { detailsElements[i].setAttribute("open", "true"); } })();
 ```"""
 
 print(
```

### Comparing `xklb-1.29.8/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.30.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.30.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/.github/workflows/push.yaml` & `xklb-1.30.2/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/sql/transfer.sql` & `xklb-1.30.2/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/av.py` & `xklb-1.30.2/xklb/av.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         for subtitle_path in internal_subtitles + external_subtitles:
             try:
                 captions = subtitle.read_sub(subtitle_path)
             except UnicodeDecodeError:
                 log.warning(f"[{path}] Could not decode subtitle {subtitle_path}")
             else:
-                subtitles.extend([{"path": path, **d} for d in captions])
+                subtitles.extend(captions)
     else:
         external_subtitles = []
 
     video_tags = {
         "subtitle_count": internal_subtitles_count + len(external_subtitles),
         "attachment_count": attachment_count,
         "subtitles": subtitles,
@@ -211,15 +211,15 @@
     video_count = sum(1 for s in codec_types if s == "video")
     audio_count = sum(1 for s in codec_types if s == "audio")
 
     chapters = getattr(probe, "chapters", [])
     chapter_count = len(chapters)
     if chapter_count > 0:
         chapters = [
-            {"path": path, "time": int(float(d["start_time"])), "text": d["tags"]["title"]}
+            {"time": int(float(d["start_time"])), "text": d["tags"]["title"]}
             for d in chapters
             if "tags" in d and "title" in d["tags"] and not utils.is_generic_title(d["tags"]["title"])
         ]
 
     media = {
         **media,
         "video_count": video_count,
```

### Comparing `xklb-1.29.8/xklb/books.py` & `xklb-1.30.2/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/consts.py` & `xklb-1.30.2/xklb/consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 
 TEMP_DIR = gettempdir()
 FAKE_SUBTITLE = str(Path(TEMP_DIR) / "sub.srt")  # https://github.com/skorokithakis/catt/issues/393
 CAST_NOW_PLAYING = str(Path(TEMP_DIR) / "catt_playing")
 DEFAULT_MPV_SOCKET = str(Path(TEMP_DIR) / "mpv_socket")
 DEFAULT_MPV_WATCH_LATER = str(Path("~/.config/mpv/watch_later/").expanduser().resolve())
 SUB_TEMP_DIR = str(Path(TEMP_DIR) / "library_temp_subtitles" / random_string())
-BLOCK_THE_CHANNEL = "__BLOCKLIST_ENTRY_"
 
 LOG_INFO = 1
 LOG_DEBUG = 2
 LOG_DEBUG_SQL = 3
 SIMILAR = 1
 SIMILAR_NO_FILTER = 2
 SIMILAR_NO_FILTER_NO_FTS = 3
 SIMILAR_NO_FILTER_NO_FTS_PARENT = 4
 RELATED = 1
 RELATED_NO_FILTER = 2
+DIRS = 1
+DIRS_NO_FILTER = 2
 
 SQLITE_PARAM_LIMIT = 32765
 DEFAULT_PLAY_QUEUE = 120
 DEFAULT_MULTIPLE_PLAYBACK = -1
 DEFAULT_SUBTITLE_MIX = 0.35
 PYTEST_RUNNING = "pytest" in sys.modules
 REGEX_ANSI_ESCAPE = re.compile(r"(?:\x1B[@-_]|[\x80-\x9F])[0-?]*[ -/]*[@-~]")
@@ -178,23 +179,18 @@
 
 time_facets = [
     "watching",
     "watched",
     "deleted",
     "created",
     "modified",
+    "downloaded",
 ]
 
-frequency = [
-    "daily",
-    "weekly",
-    "monthly",
-    "quarterly",
-    "yearly",
-]
+frequency = ["daily", "weekly", "monthly", "quarterly", "yearly"]
 
 
 TUBE_IGNORE_KEYS = (
     "track_id",
     "track_number",
     "repost_count",
     "fragments",
```

### Comparing `xklb-1.29.8/xklb/db.py` & `xklb-1.30.2/xklb/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,18 @@
     db.enable_wal()
     return db
 
 
 config = {
     "media": {
         "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album"],
-        "column_order": ["path", "webpath", "id", "ie_key", "playlist_path"],
-        "ignore_columns": ["id"],
-    },
-    "captions": {
-        "search_columns": ["text"],
+        "column_order": ["path", "webpath", "tube_id", "ie_key", "playlist_path"],
+        "ignore_columns": ["id", "tube_id"],
     },
+    "captions": {"search_columns": ["text"]},
     "reddit_posts": {
         "search_columns": ["title", "selftext"],
         "column_order": ["playlist_path", "path"],
     },
     "reddit_comments": {
         "search_columns": ["body"],
     },
```

### Comparing `xklb-1.29.8/xklb/dl_config.py` & `xklb-1.30.2/xklb/dl_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 .*members-only content
 .*not available in your location
 .*linked to an account
 .*This video is only available to Music Premium members
 .*episode is not currently available
 .*This channel has no uploads
 .*Could not send HEAD request
-.*Unable to download JSON metadata
 .*Failed to parse JSON Expecting
 .*expected string or bytes-like object
 .*Connection refused
 .*Failed to download MPD manifest:
 .*not currently available
 .*copyright claim""".splitlines(),
     ),
@@ -127,14 +126,15 @@
 .*Falling back on generic
 .*Some formats are possibly damaged
 .*WARNING: unable to obtain file audio codec with ffprobe
 .*matching opening tag for closing p tag not found
 .*the JSON object must be str, bytes or bytearray, not dict
 .*list indices must be integers
 .*The read operation timed out
+.*Unable to download JSON metadata
 .*Unable to recognize playlist.
 .*Premieres in""".splitlines(),
     ),
 )
 
 yt_unrecoverable_errors = re.compile(
     "|".join(
```

### Comparing `xklb-1.29.8/xklb/dl_extract.py` & `xklb-1.30.2/xklb/dl_extract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import argparse, os, sys
 from typing import List, Tuple
 
-from xklb import consts, db, play_actions, player, tube_backend, usage, utils
+from xklb import db, play_actions, player, tube_backend, usage, utils
 from xklb.consts import SC, DBType
 from xklb.utils import log
 
 
-def parse_args(action, usage):
+def parse_args():
     parser = argparse.ArgumentParser(
-        prog="library " + action,
-        usage=usage,
+        prog="library download",
+        usage=usage.download,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     subp_profile = parser.add_mutually_exclusive_group()
     subp_profile.add_argument(
         "--audio",
         "-A",
@@ -47,20 +47,19 @@
         default={},
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend downloader configuration",
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
-    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
 
     parser.add_argument("--subs", action="store_true")
     parser.add_argument("--auto-subs", "--autosubs", action="store_true")
-    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action="extend", nargs="+")
+    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=utils.ArgparseList)
 
     parser.add_argument("--prefix", default=os.getcwd(), help=argparse.SUPPRESS)
     parser.add_argument("--ext", default="DEFAULT")
 
     parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
     parser.add_argument("--cols", "-cols", "-col", nargs="*", help=argparse.SUPPRESS)
     parser.add_argument("--sort", "-u", nargs="+", default=["random"], help=argparse.SUPPRESS)
@@ -74,39 +73,36 @@
     parser.add_argument(
         "--retry-delay",
         "-r",
         default="14 days",
         help="Must be specified in SQLITE Modifiers format: N hours, days, months, or years",
     )
 
-    if action == SC.block:
-        parser.add_argument("--all-deleted-playlists", "--all", action="store_true", help=argparse.SUPPRESS)
-
+    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("database", help=argparse.SUPPRESS)
     parser.add_argument("playlists", nargs="*", help=argparse.SUPPRESS)
     args = parser.parse_intermixed_args()
 
-    if action == SC.download:
-        if args.duration:
-            args.duration = utils.parse_human_to_sql(utils.human_to_seconds, "duration", args.duration)
-
-        if not args.profile and not args.print:
-            log.error("Download profile must be specified. Use one of: --video --audio")
-            raise SystemExit(1)
+    if args.duration:
+        args.duration = utils.parse_human_to_sql(utils.human_to_seconds, "duration", args.duration)
+
+    if not args.profile and not args.print:
+        log.error("Download profile must be specified. Use one of: --video --audio")
+        raise SystemExit(1)
 
     if args.db:
         args.database = args.db
     args.db = db.connect(args)
 
     args.playlists = utils.conform(args.playlists)
 
-    args.action = action
+    args.action = SC.download
     play_actions.parse_args_sort(args)
 
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
@@ -128,48 +124,44 @@
 
     args.filter_sql.append(
         f"""and cast(STRFTIME('%s',
           datetime( COALESCE(time_modified,0), 'unixepoch', '+{args.retry_delay}')
         ) as int) < STRFTIME('%s', datetime()) """,
     )
 
-    if "uploader" in m_columns:
-        args.filter_sql.append(
-            f"and (m.uploader is NULL or m.uploader not in (select uploader from playlists where category='{consts.BLOCK_THE_CHANNEL}'))",
-        )
-
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     if "playlist_path" in m_columns:
         query = f"""select
-                m.path
+                m.id
+                , m.path
                 , playlist_path
                 , m.title
                 {', m.duration' if 'duration' in m_columns else ''}
                 , m.time_created
                 {', m.size' if 'size' in m_columns else ''}
                 {', m.ie_key' if 'ie_key' in m_columns else ''}
                 {', m.time_modified' if 'time_modified' in m_columns else ''}
                 {', m.time_downloaded' if 'time_downloaded' in m_columns else ''}
                 {', m.time_deleted' if 'time_deleted' in m_columns else ''}
                 {', m.error' if 'error' in m_columns else ''}
-                {', m.id' if 'id' in m_columns else ''}
                 {', p.dl_config' if 'dl_config' in pl_columns else ''}
                 , coalesce(p.category, p.ie_key) category
             FROM media m
             LEFT JOIN playlists p on (p.path = m.playlist_path {"and p.ie_key != 'Local' and p.ie_key = m.ie_key" if 'ie_key' in m_columns else ''})
             WHERE 1=1
                 and COALESCE(m.time_downloaded,0) = 0
                 and COALESCE(m.time_deleted,0) = 0
                 and COALESCE(p.time_deleted,0) = 0
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
                 , play_count
+                , COALESCE(m.time_modified,0) = 0 DESC
                 {', ' + args.sort if args.sort else ''}
                 , random()
         {LIMIT}
         """
     else:
         query = f"""select
                 m.path
@@ -178,25 +170,25 @@
                 , m.time_created
                 {', m.size' if 'size' in m_columns else ''}
                 {', m.ie_key' if 'ie_key' in m_columns else ''}
                 {', m.time_modified' if 'time_modified' in m_columns else ''}
                 {', m.time_downloaded' if 'time_downloaded' in m_columns else ''}
                 {', m.time_deleted' if 'time_deleted' in m_columns else ''}
                 {', m.error' if 'error' in m_columns else ''}
-                {', m.id' if 'id' in m_columns else ''}
             FROM media m
             WHERE 1=1
                 and COALESCE(m.time_downloaded,0) = 0
                 and COALESCE(m.time_deleted,0) = 0
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
                 , play_count
+                , COALESCE(m.time_modified,0) = 0 DESC
                 {', ' + args.sort if args.sort else ''}
                 , random()
         {LIMIT}
         """
 
     return query, args.filter_bindings
 
@@ -208,22 +200,25 @@
         player.printer(args, query, bindings)
         return []
 
     media = list(args.db.query(query, bindings))
     if not media:
         utils.no_media_found()
 
+    if "blocklist" in args.db.table_names():
+        media = utils.block_dicts_like_sql(media, [{d["key"]: d["value"]} for d in args.db["blocklist"].rows])
+
     return media
 
 
 def dl_download(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args(SC.download, usage=usage.download)
+    args = parse_args()
     m_columns = args.db["media"].columns_dict
 
     if "media" in args.db.table_names() and "webpath" in m_columns:
         with args.db.conn:
             args.db.conn.execute("DELETE from media WHERE webpath is NULL and path in (select webpath from media)")
 
     media = process_downloadqueue(args)
@@ -253,65 +248,7 @@
             try:
                 tube_backend.yt(args, m)
             except Exception:
                 print("db:", args.database)
                 raise
         else:
             raise NotImplementedError
-
-
-def dl_block(args=None) -> None:
-    if args:
-        sys.argv = ["lb", *args]
-
-    args = parse_args(SC.block, usage=usage.block)
-
-    if not any([args.playlists, args.all_deleted_playlists]):
-        raise RuntimeError("Specific URLs or --all-deleted-playlists must be supplied")
-
-    log.info(utils.dict_filter_bool(args.__dict__))
-    args.category = consts.BLOCK_THE_CHANNEL
-    args.extra_playlist_data = {"time_deleted": consts.APPLICATION_START}
-    args.extra_media_data = {"time_deleted": consts.APPLICATION_START}
-    for p in args.playlists:
-        tube_backend.process_playlist(args, p, tube_backend.tube_opts(args, func_opts={"playlistend": 30}))
-
-    if args.playlists:
-        with args.db.conn:
-            args.db.conn.execute(
-                f"""UPDATE playlists
-                SET time_deleted={consts.APPLICATION_START}
-                ,   category='{consts.BLOCK_THE_CHANNEL}'
-                WHERE path IN ("""
-                + ",".join(["?"] * len(args.playlists))
-                + ")",
-                (*args.playlists,),
-            )
-
-    paths_to_delete = [
-        d["path"]
-        for d in args.db.query(
-            """SELECT path FROM media
-        WHERE time_downloaded > 0
-        AND playlist_path IN ("""
-            + ",".join(["?"] * len(args.playlists))
-            + ")",
-            (*args.playlists,),
-        )
-    ]
-
-    if args.all_deleted_playlists:
-        paths_to_delete = [
-            d["path"]
-            for d in args.db.query(
-                """SELECT path FROM media
-            WHERE time_downloaded > 0
-            AND playlist_path IN (
-                select path from playlists where time_deleted > 0
-            ) """,
-            )
-        ]
-
-    if paths_to_delete:
-        print(paths_to_delete)
-        if not consts.PYTEST_RUNNING and utils.confirm("Delete?"):
-            player.delete_media(args, paths_to_delete)
```

### Comparing `xklb-1.29.8/xklb/fs_extract.py` & `xklb-1.30.2/xklb/fs_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,34 +193,42 @@
 def extract_chunk(args, media) -> None:
     if args.profile == DBType.image:
         media = books.extract_image_metadata_chunk(media)
 
     if args.scan_subtitles:
         clean_up_temp_dirs()
 
-    captions_t0 = []
+    captions = []
     for d in media:
-        chapters = d.pop("chapters", None) or []
-        if len(chapters) > 0:
-            args.db["captions"].insert_all(chapters, alter=True)
-
-        subtitles = d.pop("subtitles", None) or []
-        if len(subtitles) > 0:
-            args.db["captions"].insert_all(subtitles, alter=True)
+        caption = {}
+        caption["path"] = d["path"]
+
+        caption["chapters"] = d.pop("chapters", None) or []
+        caption["subtitles"] = d.pop("subtitles", None) or []
 
         tags = d.pop("tags", None) or ""
         description = d.pop("description", None) or ""
         if description:
             tags += "\n" + description
         if tags:
-            captions_t0.append({"path": d["path"], "time": 0, "text": tags})
-    args.db["captions"].insert_all(captions_t0, alter=True)
+            caption["captions_t0"] = {"time": 0, "text": tags}
+
+        captions.append(caption)
 
     media = utils.list_dict_filter_bool(media)
-    args.db["media"].insert_all(utils.list_dict_filter_bool(media), pk="path", alter=True, replace=True)
+    args.db["media"].insert_all(utils.list_dict_filter_bool(media), pk="id", alter=True, replace=True)
+
+    for d in captions:
+        media_id = args.db.pop("select id from media where path = ?", [d["path"]])
+        if len(d["chapters"]) > 0:
+            args.db["captions"].insert_all([{**d, "media_id": media_id} for d in d["chapters"]], alter=True)
+        if len(d["subtitles"]) > 0:
+            args.db["captions"].insert_all([{**d, "media_id": media_id} for d in d["subtitles"]], alter=True)
+        if d.get("caption_t0"):
+            args.db["captions"].insert({**d["caption_t0"], "media_id": media_id}, alter=True)
 
 
 def find_new_files(args, path: Path) -> List[str]:
     if path.is_file():
         scanned_files = [str(path)]
     else:
         try:
```

### Comparing `xklb-1.29.8/xklb/gui.py` & `xklb-1.30.2/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/hn_extract.py` & `xklb-1.30.2/xklb/hn_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 
 def hacker_news_add() -> None:
     args = parse_args(prog="library hnadd", usage=usage.hnadd)
     try:
         import aiohttp
     except ModuleNotFoundError:
-        log.error("aiohttp is required for hn_extract. Install with pip install aiohttp or pip install xklb[full]")
+        log.error("aiohttp is required for hn_extract. Install with pip install aiohttp or pip install xklb[deluxe]")
         raise
 
     args.db.enable_wal()
 
     max_item_id = get("https://hacker-news.firebaseio.com/v0/maxitem.json")
     tables = args.db.table_names()
     r = list(
```

### Comparing `xklb-1.29.8/xklb/lb.py` & `xklb-1.30.2/xklb/lb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import argparse, sys
 
 from xklb import __version__, utils
 from xklb.consts import SC
-from xklb.dl_extract import dl_block, dl_download
+from xklb.dl_extract import dl_download
 from xklb.fs_extract import fs_add, fs_update
 from xklb.hn_extract import hacker_news_add
 from xklb.play_actions import filesystem, listen, read, view, watch
 from xklb.playback import playback_next, playback_now, playback_pause, playback_stop
 from xklb.praw_extract import reddit_add, reddit_update
 from xklb.scripts.bigdirs import bigdirs
+from xklb.scripts.block import block
 from xklb.scripts.christen import christen
 from xklb.scripts.cluster_sort import cluster_sort
 from xklb.scripts.copy_play_counts import copy_play_counts
 from xklb.scripts.dedupe import dedupe
 from xklb.scripts.download_status import download_status
 from xklb.scripts.history import history
 from xklb.scripts.merge_dbs import merge_dbs
@@ -191,15 +192,15 @@
 
     subp_hnadd = add_parser(subparsers, "hnadd")
     subp_hnadd.set_defaults(func=hacker_news_add)
 
     subp_download = add_parser(subparsers, "download", ["dl"])
     subp_download.set_defaults(func=dl_download)
     subp_block = add_parser(subparsers, "block")
-    subp_block.set_defaults(func=dl_block)
+    subp_block.set_defaults(func=block)
     subp_redownload = add_parser(subparsers, "redownload", ["redl"])
     subp_redownload.set_defaults(func=redownload)
 
     subp_playlist = add_parser(subparsers, "playlists", ["pl", "folders"])
     subp_playlist.set_defaults(func=playlists)
     subp_history = add_parser(subparsers, "history", ["hi", "log"])
     subp_history.set_defaults(func=history)
```

### Comparing `xklb-1.29.8/xklb/play_actions.py` & `xklb-1.30.2/xklb/play_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from random import random
 from typing import Dict, Tuple
 
 from xklb import consts, db, player, subtitle, tube_backend, usage, utils
 from xklb.consts import SC
 from xklb.playback import now_playing
 from xklb.player import mark_media_deleted, override_sort
+from xklb.scripts.bigdirs import process_bigdirs
 from xklb.utils import cmd_interactive, log, random_filename, safe_unpack
 
 
 def parse_args_sort(args) -> None:
     if args.sort:
         args.sort = " ".join(args.sort)
     elif not args.sort and hasattr(args, "defaults"):
@@ -69,19 +70,20 @@
 
 def parse_args(action, default_chromecast=None) -> argparse.Namespace:
     DEFAULT_PLAYER_ARGS_SUB = ["--speed=1"]
     DEFAULT_PLAYER_ARGS_NO_SUB = ["--speed=1.46"]
 
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage.play(action))
 
-    parser.add_argument("--play-in-order", "-O", action="count", default=0, help=argparse.SUPPRESS)
-    parser.add_argument("--related", "-R", action="count", default=0, help=argparse.SUPPRESS)
-    parser.add_argument("--cluster", "-C", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--random", "-r", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--big-dirs", "-B", action="count", default=0, help=argparse.SUPPRESS)
+    parser.add_argument("--related", "-R", action="count", default=0, help=argparse.SUPPRESS)
+    parser.add_argument("--cluster", "-C", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--play-in-order", "-O", action="count", default=0, help=argparse.SUPPRESS)
 
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--no-fts", action="store_true")
 
     parser.add_argument("--created-within", help=argparse.SUPPRESS)
@@ -163,24 +165,25 @@
     parser.add_argument("--online-media-only", "--online-only", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--local-media-only", "--local-only", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
 
     parser.add_argument("--sibling", "--episode", action="store_true")
     parser.add_argument("--solo", action="store_true")
 
-    parser.add_argument("--sort-by", action="store_true")
+    parser.add_argument("--sort-by")
     parser.add_argument("--depth", "-D", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
 
+    parser.add_argument("--prefetch", type=int, default=1)
     parser.add_argument("--prefix", default="", help=argparse.SUPPRESS)
     parser.add_argument(
         "--folder",
         action="store_true",
-        help="Experimental escape hatch to open folder which breaks a lot of features like post-actions",
+        help="Experimental escape hatch to open folder; breaks a lot of features like post-actions",
     )
     parser.add_argument(
         "--folder-glob",
         "--folderglob",
         type=int,
         default=False,
         const=10,
@@ -203,14 +206,17 @@
     if args.include == ["."]:
         args.include = [str(Path().cwd().resolve())]
 
     if args.db:
         args.database = args.db
     args.db = db.connect(args)
 
+    if args.big_dirs:
+        args.local_media_only = True
+
     if not args.limit:
         args.defaults.append("limit")
         if not any([args.print and len(args.print.replace("p", "")) > 0, args.partial, args.lower, args.upper]):
             if args.action in (SC.listen, SC.watch, SC.read):
                 args.limit = consts.DEFAULT_PLAY_QUEUE
             elif args.action in (SC.view):
                 args.limit = consts.DEFAULT_PLAY_QUEUE * 4
@@ -584,24 +590,31 @@
         media = utils.mpv_enrich(args, media)
         log.debug("utils.mpv_enrich: %s", t.elapsed())
 
     if args.safe:
         media = [d for d in media if tube_backend.is_supported(d["path"]) or Path(d["path"]).exists()]
         log.debug("tube_backend.is_supported: %s", t.elapsed())
 
+    if args.big_dirs:
+        media_keyed = {d["path"]: d for d in media}
+        dirs = process_bigdirs(args, media)
+        dirs = list(reversed(list(d["path"] for d in dirs)))
+        if "limit" in args.defaults:
+            media = player.get_dir_media(args, dirs)
+        else:
+            media = [media_keyed[key] for dir in dirs for key in media_keyed.keys() if key.startswith(dir)]
+        log.debug("big_dirs: %s", t.elapsed())
+
     if args.related >= consts.RELATED:
         media = player.get_related_media(args, media[0])
         log.debug("player.get_related_media: %s", t.elapsed())
 
     if args.cluster:
-        media_keyed = {d["path"]: d for d in media}
-        groups = utils.cluster_paths([d["path"] for d in media])
-        groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
-        sorted_paths = utils.flatten(d["grouped_paths"] for d in groups)
-        media = [media_keyed[p] for p in sorted_paths]
+        media = utils.cluster_dicts(media)
+        log.debug("cluster: %s", t.elapsed())
 
     if args.print:
         if args.play_in_order >= consts.SIMILAR:
             media = [player.get_ordinal_media(args, d) for d in media]
         player.media_printer(args, media)
     elif args.multiple_playback:
         args.gui = True
@@ -610,15 +623,15 @@
         try:
             mp_args = argparse.Namespace(**{k: v for k, v in args.__dict__.items() if k not in {"db"}})
             media.reverse()  # because media.pop()
             ignore_paths = []
             futures = deque()
             with ThreadPoolExecutor(max_workers=1) as executor:
                 while media or futures:
-                    while media and len(futures) < 3:
+                    while media and len(futures) < args.prefetch:
                         m = media.pop()
                         if m["path"] in ignore_paths:
                             continue
                         future = executor.submit(prep_media, mp_args, m, ignore_paths)
                         ignore_paths.append(m["path"])
                         futures.append(future)
```

### Comparing `xklb-1.29.8/xklb/playback.py` & `xklb-1.30.2/xklb/playback.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             path
             + "\n"
             + "\n".join(
                 line
                 for line in cmd("ffprobe", "-hide_banner", "-loglevel", "info", path).stderr.splitlines()
                 if path not in line
             )
+            + "\n"
         )
 
     try:
         text.encode()
         return text
     except UnicodeEncodeError:
         try:
```

### Comparing `xklb-1.29.8/xklb/player.py` & `xklb-1.30.2/xklb/player.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from time import sleep
 from typing import Dict, List, Optional, Tuple, Union
 
 from tabulate import tabulate
 
 from xklb import consts, db, utils
 from xklb.consts import SC
-from xklb.scripts.bigdirs import process_bigdirs
 from xklb.utils import cmd, cmd_interactive, human_time, log
 
 try:
     import tkinter  # noqa
 
     from xklb import gui
 except ModuleNotFoundError:
@@ -43,27 +42,27 @@
 
     duration = m.get("duration", 20 * 60)
     if args.start:
         playhead = m.get("playhead")
 
         if args.start.isnumeric() and int(args.start) > 0:
             start = int(args.start)
-        elif args.start.endswith("%") and duration:
+        elif "%" in args.start:
             start_percent = int(args.start[:-1])
             start = int(duration * start_percent / 100)
         elif playhead and any([end == 0, end > minimum_duration]):
             start = playhead
         elif args.start == "wadsworth":
             start = duration * 0.3
         else:
             start = int(args.start)
     if args.end:
         if args.end == "dawsworth":
             end = duration * 0.65
-        elif args.end.endswith("%") and duration:
+        elif "%" in args.end:
             end_percent = int(args.end[:-1])
             end = int(duration * end_percent / 100)
         elif "+" in args.end:
             end = int(args.start) + int(args.end)
         else:
             end = int(args.end)
 
@@ -184,35 +183,35 @@
 
     return modified_row_count
 
 
 def set_playhead(args, path: str, playhead: int) -> int:
     with args.db.conn:
         cursor = args.db.conn.execute(
-            """UPDATE media
+            f"""UPDATE media
             SET playhead = :playhead
-                , time_played = cast(STRFTIME('%s') as int)
+                , time_played = {consts.now()}
             WHERE path = :path
             """,
             {"playhead": playhead, "path": path},
         )
     return cursor.rowcount
 
 
-def mark_media_watched(args, files) -> int:
-    files = utils.conform(files)
+def mark_media_watched(args, paths, time_watched=consts.now()) -> int:
+    paths = utils.conform(paths)
     modified_row_count = 0
-    if files:
-        df_chunked = utils.chunks(files, consts.SQLITE_PARAM_LIMIT)
+    if paths:
+        df_chunked = utils.chunks(paths, consts.SQLITE_PARAM_LIMIT)
         for chunk_paths in df_chunked:
             with args.db.conn:
                 cursor = args.db.conn.execute(
-                    """UPDATE media
+                    f"""UPDATE media
                     SET play_count = play_count + 1
-                        , time_played = cast(STRFTIME('%s') as int)
+                        , time_played = {time_watched}
                     WHERE path in ("""
                     + ",".join(["?"] * len(chunk_paths))
                     + ")",
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
@@ -261,18 +260,18 @@
 
     return modified_row_count
 
 
 def delete_media(args, paths) -> int:
     paths = utils.conform(paths)
     for p in paths:
-        if args.prefix:
+        if getattr(args, "prefix", False):
             Path(p).unlink(missing_ok=True)
         else:
-            utils.trash(p)
+            utils.trash(p, detach=len(paths) < 30)
 
     return mark_media_deleted(args, paths)
 
 
 def delete_playlists(args, playlists) -> None:
     with args.db.conn:
         playlist_paths = playlists + [p.rstrip(os.sep) for p in playlists]
@@ -498,14 +497,58 @@
 
     related_videos = list(args.db.query(query, bindings))
     log.debug(related_videos)
 
     return [m, *related_videos]
 
 
+def get_dir_media(args, dirs: List, include_subdirs=False) -> List[Dict]:
+    if len(dirs) == 0:
+        return utils.no_media_found()
+
+    m_columns = args.db["media"].columns_dict
+
+    if include_subdirs:
+        filter_paths = "AND (" + " OR ".join([f"path LIKE :subpath{i}" for i in range(len(dirs))]) + ")"
+    else:
+        filter_paths = (
+            "AND ("
+            + " OR ".join([f"(path LIKE :subpath{i} and path not like :subpath{i} || '/%')" for i in range(len(dirs))])
+            + ")"
+        )
+
+    query = f"""
+        SELECT
+            {args.select_sql}
+        FROM {args.table} m
+        WHERE 1=1
+            {filter_args_sql(args, m_columns)}
+            {filter_paths}
+            {'' if args.related >= consts.DIRS_NO_FILTER else (" ".join(args.filter_sql) or '')}
+        ORDER BY play_count
+            , m.path LIKE "http%"
+            {'' if 'sort' in args.defaults else ', ' + args.sort}
+            , path
+        {"LIMIT 10000" if 'limit' in args.defaults else str(args.limit)} {args.offset_sql}
+    """
+    subpath_params = {f"subpath{i}": value + "%" for i, value in enumerate(dirs)}
+
+    bindings = {**subpath_params}
+    if args.related >= consts.DIRS_NO_FILTER:
+        bindings = {**bindings, "query": args.filter_bindings["query"]}
+    else:
+        bindings = {**bindings, **args.filter_bindings}
+
+    subpath_videos = list(args.db.query(query, bindings))
+    log.debug(subpath_videos)
+    log.info("len(subpath_videos) = %s", len(subpath_videos))
+
+    return subpath_videos
+
+
 def watch_chromecast(args, m: dict, subtitles_file=None) -> Optional[subprocess.CompletedProcess]:
     if "vlc" in args.player:
         catt_log = cmd(
             "vlc",
             "--sout",
             "#chromecast",
             f"--sout-chromecast-ip={args.cc_ip}",
@@ -807,27 +850,29 @@
             sleep(delay)
 
     return r
 
 
 def historical_usage(args, freq="monthly", time_column="time_played", where=""):
     if freq == "daily":
-        time_format = "%Y-%m-%d"
+        time_period = f"strftime('%Y-%m-%d', datetime({time_column}, 'unixepoch'))"
     elif freq == "weekly":
-        time_format = "%Y-%W"
+        time_period = f"strftime('%Y-%W', datetime({time_column}, 'unixepoch'))"
     elif freq == "monthly":
-        time_format = "%Y-%m"
+        time_period = f"strftime('%Y-%m', datetime({time_column}, 'unixepoch'))"
+    elif freq == "quarterly":
+        time_period = f"strftime('%Y', datetime({time_column}, 'unixepoch', '-3 months')) || '-Q' || ((strftime('%m', datetime({time_column}, 'unixepoch', '-3 months')) - 1) / 3 + 1)"
     elif freq == "yearly":
-        time_format = "%Y"
+        time_period = f"strftime('%Y', datetime({time_column}, 'unixepoch'))"
     else:
         raise ValueError(f"Invalid value for 'freq': {freq}")
 
     query = f"""
     SELECT
-        strftime('{time_format}', datetime({time_column}, 'unixepoch')) AS time_period
+        {time_period} AS time_period
         , SUM(duration) AS duration_sum
         , AVG(duration) AS duration_avg
         , SUM(size) AS size_sum
         , AVG(size) AS size_avg
     FROM media
     WHERE coalesce(time_period, 0)>0 and {time_column}>0 {where}
     GROUP BY time_period
@@ -841,17 +886,14 @@
     except statistics.StatisticsError:
         return duration
 
     return duration / historical_daily * 86400 * 30.42
 
 
 def media_printer(args, media) -> None:
-    if "b" in args.print:
-        media = process_bigdirs(args, media)
-
     if args.verbose >= consts.LOG_DEBUG and args.cols and "*" in args.cols:
         breakpoint()
 
     if not media:
         utils.no_media_found()
 
     if "f" not in args.print and "limit" in getattr(args, "defaults", []):
@@ -890,15 +932,15 @@
 
     if "f" in args.print:
         if args.limit == 1:
             path = media[0]["path"]
             if not Path(path).exists():
                 mark_media_deleted(args, path)
                 raise FileNotFoundError
-            utils.pipe_print(quote(path))
+            utils.pipe_print(path)
             return
         else:
             if not args.cols:
                 args.cols = ["path"]
 
             selected_cols = [{k: d.get(k, None) for k in args.cols} for d in media]
             virtual_csv = StringIO()
```

### Comparing `xklb-1.29.8/xklb/praw_extract.py` & `xklb-1.30.2/xklb/praw_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
                 log.error(f"[{path}]: Skipping unknown URL")
                 continue
 
         args.db["playlists"].upsert(
             utils.dict_filter_bool(
                 {
                     "path": path,
-                    "id": name,
+                    "playlist_id": name,
                     "config": utils.filter_namespace(args, ["limit", "lookback", "praw_site"]),
                     "category": args.category or ie_key,
                     "ie_key": ie_key,
                     "time_deleted": 0,
                 },
             ),
             pk="path",
@@ -407,10 +407,10 @@
     )
 
     for playlist in playlists:
         config = json.loads(playlist["config"])
         args_env = args if not config else argparse.Namespace(**{**config, **args.__dict__})
 
         if playlist["ie_key"] == "reddit_praw_subreddit":
-            process_subreddits(args_env, [{"path": playlist["path"], "name": playlist["id"]}])
+            process_subreddits(args_env, [{"path": playlist["path"], "name": playlist["playlist_id"]}])
         elif playlist["ie_key"] == "reddit_praw_subreddit":
-            process_redditors(args_env, [{"path": playlist["path"], "name": playlist["id"]}])
+            process_redditors(args_env, [{"path": playlist["path"], "name": playlist["playlist_id"]}])
```

### Comparing `xklb-1.29.8/xklb/search.py` & `xklb-1.30.2/xklb/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     parser.add_argument("--csv", action="store_true")
     parser.add_argument("--json", action="store_true")
     parser.add_argument("--table", action="store_true")
     parser.add_argument("--aggregate", "-a", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--cols", "-cols", "-col", nargs="*", help=argparse.SUPPRESS)
     parser.add_argument("--limit", "-L", "-l", help=argparse.SUPPRESS)
 
+    parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
     parser.add_argument("--action", default="search", help=argparse.SUPPRESS)
     parser.add_argument("--folder", action="store_true", help="Experimental escape hatch to open folder")
     parser.add_argument(
         "--folder-glob",
         "--folderglob",
         type=int,
         default=False,
@@ -86,50 +87,54 @@
         tbl = utils.col_resize(tbl, "text", 35)
         tbl = utils.list_dict_filter_bool(tbl)
         print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
         print(f"{len(captions)} captions")
     else:
         print(f"{len(captions)} captions")
         for path, path_group in groupby(tbl, key=lambda x: x["path"]):
-            print(path)
+            path_group = list(path_group)
+            title = path_group[0].get("title")
+            print(" - ".join(utils.concat(title, path)))
             for caption in path_group:
                 for line in textwrap.wrap(caption["text"], subsequent_indent=" " * 9, initial_indent=f"{caption['time']} ", width=consts.TERMINAL_SIZE.columns - 2):  # type: ignore
                     print(line)
             print()
 
 
 def construct_query(args) -> Tuple[str, dict]:
-    m_columns = args.db["captions"].columns_dict
+    m_columns = args.db["media"].columns_dict
+    c_columns = args.db["captions"].columns_dict
     args.filter_sql = []
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     table = "captions"
     if args.db["captions"].detect_fts():
         if args.include:
             table = db.fts_flexible_search(args, "captions")
-            m_columns = {**m_columns, "rank": int}
+            c_columns = {**c_columns, "rank": int}
         elif args.exclude:
-            db.construct_search_bindings(args, m_columns)
+            db.construct_search_bindings(args, c_columns)
     else:
-        db.construct_search_bindings(args, m_columns)
+        db.construct_search_bindings(args, c_columns)
 
-    cols = args.cols or ["path", "text", "time", "rank"]
-    args.select = [c for c in cols if c in m_columns or c in ["*"]]
+    cols = args.cols or ["path", "text", "time", "rank", "title"]
+    args.select = [c for c in cols if c in {**c_columns, **m_columns, **{"*": "Any"}}]
     args.select_sql = "\n        , ".join(args.select)
     args.limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
-    query = f"""WITH m as (
+    query = f"""WITH c as (
     SELECT rowid, * FROM {table}
     WHERE 1=1
-        {player.filter_args_sql(args, m_columns)}
+        {player.filter_args_sql(args, c_columns)}
     )
     SELECT
         {args.select_sql}
-    FROM m
+    FROM c
+    JOIN media m on m.id = c.media_id
     WHERE 1=1
         {" ".join(args.filter_sql)}
     ORDER BY 1=1
         , {args.sort}
     {args.limit_sql}
     """
 
@@ -138,18 +143,19 @@
 
 def merge_captions(args, captions):
     def get_end(caption):
         return caption["time"] + (len(caption["text"]) / 4.2 / 220 * 60)
 
     merged_captions = []
     for path, group in groupby(
-        captions, key=lambda x: x["path"]
+        captions,
+        key=lambda x: x["path"],
     ):  # group by only does contiguous items with the same key
         group = list(group)
-        merged_group = {"path": path, "time": group[0]["time"], "end": get_end(group[0]), "text": group[0]["text"]}  # type: ignore
+        merged_group = {"path": path, "title": group[0]["title"], "time": group[0]["time"], "end": get_end(group[0]), "text": group[0]["text"]}  # type: ignore
         for i in range(1, len(group)):
             end = get_end(group[i])
 
             if (
                 abs(group[i]["time"] - merged_group["end"]) <= args.overlap  # type: ignore
                 or abs(group[i]["time"] - merged_group["time"]) <= args.overlap  # type: ignore
             ):
```

### Comparing `xklb-1.29.8/xklb/subtitle.py` & `xklb-1.30.2/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/tabs_actions.py` & `xklb-1.30.2/xklb/tabs_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from xklb.consts import SC
 from xklb.player import generic_player, mark_media_watched, override_sort, printer
 from xklb.utils import cmd, flatten, log
 
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="library tabs", formatter_class=argparse.ArgumentDefaultsHelpFormatter, usage=usage.tabs
+        prog="library tabs",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        usage=usage.tabs,
     )
 
     parser.add_argument("--sort", "-u", nargs="+")
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[])
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[])
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[])
     parser.add_argument("--print", "-p", default=False, const="p", nargs="?")
```

### Comparing `xklb-1.29.8/xklb/tabs_extract.py` & `xklb-1.30.2/xklb/tabs_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library tabsadd", usage=usage.tabsadd)
     parser.add_argument(
         "--frequency",
         "--freqency",
         "-f",
         metavar="frequency",
-        choices=consts.frequency,
         default="monthly",
         const="monthly",
         type=str.lower,
         nargs="?",
-        help=f"One of: %(choices)s (default: %(default)s)",
+        help="One of: %(choices)s (default: %(default)s)",
     )
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
 
+    args.frequency = utils.partial_startswith(args.frequency, consts.frequency)
+
     if args.db:
         args.database = args.db
 
     Path(args.database).touch()
     args.db = db.connect(args)
 
     log.info(utils.dict_filter_bool(args.__dict__))
```

### Comparing `xklb-1.29.8/xklb/tube_backend.py` & `xklb-1.30.2/xklb/tube_backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,86 +49,14 @@
         "youtube_include_hls_manifest": False,
         "no_check_certificate": True,
         "check_formats": False,
         "ignore_no_formats_error": True,
         "skip_playlist_after_errors": 21,
         "clean_infojson": False,
         "playlistend": 20000,
-        "rejecttitle": "|".join(
-            [
-                " AWARD",
-                " Clip",
-                " GPU ",
-                " Scene",
-                " Terror",
-                "360",
-                "Advert",
-                "Announcement",
-                "Apology",
-                "Best of",
-                "Bitcoin",
-                "campaign",
-                "Ceremony",
-                "Clip ",
-                "Compilation",
-                "Crypto ",
-                "Event",
-                "Final Look",
-                "First Look",
-                "Graphics Card",
-                "Horror",
-                "In Theaters",
-                "Live ",
-                "Makeup",
-                "Meetup",
-                "Montage",
-                "Now Playing",
-                "Outtakes",
-                "Panel",
-                "Preview",
-                "Promo",
-                "Red Carpet Premiere",
-                "Sneak Peek",
-                "Stream",
-                "Teaser",
-                "1 Hour",
-                "2 Hour",
-                "3 Hour",
-                "4 Hour",
-                "5 Hour",
-                "6 Hour",
-                "7 Hour",
-                "8 Hour",
-                "9 Hour",
-                "10 Hour",
-                "100 Hour",
-                "Top 10",
-                "Top 2",
-                "Top 3",
-                "Top 4",
-                "Top 5",
-                "Top 6",
-                "Top 7",
-                "Top 8",
-                "Top 9",
-                "Top Eight",
-                "Top Five",
-                "Top Four",
-                "Top Nine",
-                "Top Seven",
-                "Top Six",
-                "Top Ten",
-                "Top Three",
-                "Top Two",
-                "Trailer",
-                "TV Spot",
-                "Twitch",
-                "World Premiere",
-            ],
-        ),
     }
 
     all_opts = {
         **default_opts,
         **func_opts,
         **json.loads(playlist_opts),
         **cli_opts,
@@ -221,16 +149,16 @@
     cv["tags"] = combine(
         "language:" + language if language else None,
         v.pop("description", None),
         v.pop("categories", None),
         v.pop("genre", None),
         v.pop("tags", None),
     )
-    cv["id"] = v.pop("id", None)
-    if cv["id"] is None:
+    cv["tube_id"] = v.pop("id", None)
+    if cv["tube_id"] is None:
         log.warning("No id found in %s", v)
     cv["ie_key"] = safe_unpack(v.pop("ie_key", None), v.pop("extractor_key", None), v.pop("extractor", None))
     cv["title"] = safe_unpack(v.pop("title", None), v.get("playlist_title"))
     cv["view_count"] = v.pop("view_count", None)
     cv["width"] = v.pop("width", None)
     cv["height"] = v.pop("height", None)
     fps = v.pop("fps", None)
@@ -266,22 +194,22 @@
 def _add_playlist(args, playlist_path, pl: dict, media_path: Optional[str] = None) -> None:
     extractor = safe_unpack(pl.get("ie_key"), pl.get("extractor_key"), pl.get("extractor"))
     playlist = {
         "ie_key": extractor,
         "title": pl.get("playlist_title"),
         "path": playlist_path,
         "uploader": safe_unpack(pl.get("playlist_uploader_id"), pl.get("playlist_uploader")),
-        "id": pl.get("playlist_id"),
+        "playlist_id": pl.get("playlist_id"),
         "dl_config": args.dl_config,
         "time_deleted": 0,
         "category": args.category or extractor,
         **args.extra_playlist_data,
     }
 
-    if not playlist.get("id") or media_path == playlist["path"]:
+    if not playlist.get("playlist_id") or media_path == playlist["path"]:
         log.warning("Importing playlist-less media %s", playlist["path"])
     else:
         args.db["playlists"].upsert(utils.dict_filter_bool(playlist), pk="path", alter=True)
 
 
 def save_undownloadable(args, playlist_path) -> None:
     entry = {
@@ -294,14 +222,27 @@
     args.db["playlists"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)
 
 
 playlists_of_playlists = []
 added_media_count = 0
 
 
+def save_entry(args, entry):
+    tags = entry.pop("tags", None) or ""
+    media_id = args.db.pop("select id from media where path = ?", [entry["path"]])
+    if media_id:
+        entry["id"] = media_id
+        args.db["media"].upsert(utils.dict_filter_bool(entry), pk="id", alter=True)
+    else:
+        args.db["media"].insert(utils.dict_filter_bool(entry), pk="id", alter=True)
+        media_id = args.db.pop("select id from media where path = ?", [entry["path"]])
+    if tags:
+        args.db["captions"].insert({"media_id": media_id, "time": 0, "text": tags}, alter=True)
+
+
 def process_playlist(args, playlist_path, ydl_opts, playlist_root=True) -> Optional[List[Dict]]:
     yt_dlp = load_module_level_yt_dlp()
 
     for k, v in args.extra_playlist_data.items():
         setattr(args, k, v)
 
     class ExistingPlaylistVideoReached(yt_dlp.DownloadCancelled):
@@ -333,15 +274,15 @@
                     entry["playlist_path"] = playlist_path
                     _add_playlist(args, playlist_path, deepcopy(info), entry["path"])
 
                     if is_video_known(args, playlist_path, entry["path"]) and not args.ignore_errors:
                         raise ExistingPlaylistVideoReached
 
                     entry = {**entry, **args.extra_media_data}
-                    args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)
+                    save_entry(args, entry)
 
                     added_media_count += 1
                     if added_media_count > 1:
                         sys.stdout.write("\033[K\r")
                         print(f"[{playlist_path}] Added {added_media_count} media", end="\r", flush=True)
 
             return [], info
@@ -360,14 +301,39 @@
             if added_media_count > count_before_extract:
                 sys.stdout.write("\n")
             if not pl and not args.safe:
                 log.warning("Logging undownloadable media")
                 save_undownloadable(args, playlist_path)
 
 
+def get_video_metadata(args, playlist_path) -> Optional[Dict]:
+    yt_dlp = load_module_level_yt_dlp()
+
+    with yt_dlp.YoutubeDL(
+        tube_opts(
+            args,
+            func_opts={
+                "skip_download": True,
+                "extract_flat": True,
+                "lazy_playlist": True,
+                "check_formats": False,
+                "ignoreerrors": False,
+                "playlistend": None,
+                "playlist_items": "1",
+                "noplaylist": True,
+            },
+        ),
+    ) as ydl:
+        entry = ydl.extract_info(playlist_path, download=False)
+        if entry and "entries" in entry:
+            entries = entry.pop("entries")[0]
+            entry = {**entry, **entries}
+        return entry
+
+
 def get_extra_metadata(args, playlist_path, playlist_dl_opts=None) -> Optional[List[Dict]]:
     yt_dlp = load_module_level_yt_dlp()
 
     m_columns = args.db["media"].columns_dict
 
     with yt_dlp.YoutubeDL(
         tube_opts(
@@ -390,15 +356,16 @@
             },
             playlist_opts=playlist_dl_opts,
         ),
     ) as ydl:
         videos = args.db.execute(
             f"""
             SELECT
-                path
+              id
+            , path
             , ie_key
             , play_count
             , time_played
             , playhead
             FROM media
             WHERE 1=1
                 {'and width is null' if 'width' in m_columns else ''}
@@ -406,24 +373,24 @@
                 and playlist_path = ?
             ORDER by random()
             """,
             [playlist_path],
         ).fetchall()
 
         current_video_count = 0
-        for path, ie_key, play_count, time_played, playhead in videos:
+        for id, path, ie_key, play_count, time_played, playhead in videos:
             entry = ydl.extract_info(path, ie_key=ie_key)
             if entry is None:
                 continue
 
             chapters = getattr(entry, "chapters", [])
             chapter_count = len(chapters)
             if chapter_count > 0:
                 chapters = [
-                    {"path": path, "time": int(float(d["start_time"])), "text": d.get("title")}
+                    {"media_id": id, "time": int(float(d["start_time"])), "text": d.get("title")}
                     for d in chapters
                     if d.get("title") and not utils.is_generic_title(d)
                 ]
                 if len(chapters) > 0:
                     args.db["captions"].insert_all(chapters, alter=True)
 
             if entry["requested_subtitles"]:
@@ -432,28 +399,30 @@
                 captions = []
                 for subtitle_path in downloaded_subtitles:
                     try:
                         file_captions = subtitle.read_sub(subtitle_path)
                     except UnicodeDecodeError:
                         log.warning(f"[{path}] Could not decode subtitle {subtitle_path}")
                     else:
-                        captions.extend([{"path": path, **d} for d in file_captions])
+                        captions.extend([{"media_id": id, **d} for d in file_captions])
                 if len(captions) > 0:
                     args.db["captions"].insert_all(captions, alter=True)
 
             entry = consolidate(entry)
             if entry is None:
                 continue
 
+            entry["id"] = id
             entry["playlist_path"] = playlist_path
             entry["play_count"] = play_count
             entry["chapter_count"] = chapter_count
             entry["time_played"] = time_played
             entry["playhead"] = playhead
-            args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)
+
+            save_entry(args, entry)
 
             current_video_count += 1
             sys.stdout.write("\033[K\r")
             print(
                 f"[{playlist_path}] {current_video_count} of {len(videos)} extra metadata fetched",
                 end="\r",
                 flush=True,
@@ -472,27 +441,27 @@
             log.warning("[%s]: Getting extra metadata", d["path"])
             get_extra_metadata(args, d["path"], playlist_dl_opts=d.get("dl_config", "{}"))
 
 
 def save_tube_entry(args, m, info: Optional[dict] = None, error=None, unrecoverable_error=False) -> None:
     webpath = m["path"]
 
-    v_id = m.get("id")
-    if v_id:
-        error = None if not error else error.replace(v_id, "").replace(" :", ":")
+    tube_id = m.get("tube_id")
+    if tube_id:
+        error = None if not error else error.replace(tube_id, "").replace(" :", ":")
 
     if not info:  # not downloaded or already downloaded
         entry = {
             "path": webpath,
             "time_downloaded": 0,
             "time_modified": consts.now(),
             "time_deleted": consts.APPLICATION_START if unrecoverable_error else 0,
             "error": error,
         }
-        args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)  # type: ignore
+        save_entry(args, entry)
         return
 
     assert info["local_path"] != ""
     if Path(info["local_path"]).exists():
         fs_args = argparse.Namespace(
             profile=args.profile,
             scan_subtitles=args.profile == DBType.video,
@@ -518,15 +487,15 @@
         **fs_tags,
         "webpath": webpath,
         "time_modified": consts.now(),
         "time_downloaded": 0 if error else consts.APPLICATION_START,
         "time_deleted": consts.APPLICATION_START if unrecoverable_error else 0,
         "error": error,
     }
-    args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)  # type: ignore
+    save_entry(args, entry)
 
     if fs_tags:
         try:
             args.db["media"].delete(webpath)  # from sqlite_utils.db import NotFoundError
         except Exception as e:
             log.debug(e)
```

### Comparing `xklb-1.29.8/xklb/tube_extract.py` & `xklb-1.30.2/xklb/tube_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
     parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
     parser.add_argument("--playlist-db", action="store_true", help="Fetch metadata for paths in a table")
     parser.add_argument("--subs", action="store_true")
     parser.add_argument("--auto-subs", "--autosubs", action="store_true")
-    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action="extend", nargs="+")
+    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=utils.ArgparseList)
     parser.add_argument("--extra-media-data", default={})
     parser.add_argument("--extra-playlist-data", default={})
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", "-f", action="store_true", help=argparse.SUPPRESS)
 
     if action in (SC.tubeadd, SC.tubeupdate):
         parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
```

### Comparing `xklb-1.29.8/xklb/usage.py` & `xklb-1.30.2/xklb/usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-download = r"""library download database [--prefix /mnt/d/] --video | --audio
+download = r"""library download [--prefix /mnt/d/] [--safe] [--subs] [--auto-subs] [--small] DATABASE --video | --audio
 
     Download stuff in a random order.
 
         library download dl.db --prefix ~/output/path/root/
 
     Download stuff in a random order, limited to the specified playlist URLs.
 
@@ -34,27 +34,28 @@
         │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
         │                     │            │ and 20 minutes   │                    │          │
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
 """
 
-block = r"""library block database [playlists ...]
+block = r"""library block DATABASE URLS ...
 
     Blocklist specific URLs (eg. YouTube channels, etc). With YT URLs this will block
     videos from the playlist uploader
 
-        library block dl.db https://annoyingwebsite/etc/
-
-    Use with the all-deleted-playlists flag to delete any previously downloaded files from the playlist uploader
+        library block dl.db --match-column playlist_path 'https://youtube.com/playlist?list=PLVoczRgDnXDLWV1UJ_tO70VT_ON0tuEdm'
 
-        library block dl.db --all-deleted-playlists https://annoyingwebsite/etc/
+        library block dl.db https://annoyingwebsite/etc/
+        library block dl.db "%fastcompany.com%"
+        library block dl.db --match-column title "% bitcoin%"
+        library block dl.db --force --match-column uploader Zeducation
 """
 
-fsadd = """library fsadd [--audio | --video | --image |  --text | --filesystem] -c CATEGORY [database] paths ...
+fsadd = """library fsadd [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATHS ...
 
     The default database type is video:
         library fsadd tv.db ./tv/
         library fsadd --video tv.db ./tv/  # equivalent
 
     You can also create audio databases. Both audio and video use ffmpeg to read metadata:
         library fsadd --audio audio.db ./music/
@@ -93,22 +94,22 @@
 
         library fsadd --force audio.db /mnt/d/Youtube/
         [/mnt/d/Youtube] Path does not exist
         [/mnt/d/Youtube] Building file list...
         [/mnt/d/Youtube] Marking 28932 orphaned metadata records as deleted
 """
 
-fsupdate = """library fsupdate database
+fsupdate = """library fsupdate DATABASE
 
     Update each path previously saved:
 
-        library fsupdate database
+        library fsupdate video.db
 """
 
-hnadd = """library hnadd [--oldest] database
+hnadd = """library hnadd [--oldest] DATABASE
 
     Fetch latest stories first:
 
         library hnadd hn.db -v
         Fetching 154873 items (33212696 to 33367569)
         Saving comment 33367568
         Saving comment 33367543
@@ -118,15 +119,15 @@
     Fetch oldest stories first:
 
         library hnadd --oldest hn.db
 """
 
 
 def play(action) -> str:
-    return f"""library {action} [database] [optional args]
+    return f"""library {action} DATABASE [optional args]
 
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
         Create global shortcuts in your desktop environment by sending commands to mpv_socket:
         echo 'playlist-next force' | socat - /tmp/mpv_socket
 
@@ -144,19 +145,23 @@
         library {action} --play-in-order
         There are multiple strictness levels of --play-in-order:
         library {action} -O    # equivalent
         library {action} -OO   # above, plus ignores most filters
         library {action} -OOO  # above, plus ignores fts and (include/exclude) filter during ordinal search
         library {action} -OOOO # above, plus starts search with parent folder
 
-        library {action} --related  # similar to -O but uses fts to find similar content
+        library {action} --related  # Similar to -O but uses fts to find similar content
         library {action} -R         # equivalent
         library {action} -RR        # above, plus ignores most filters
 
-        library {action} --cluster  # cluster-sort to put similar paths closer together
+        library {action} --cluster  # cluster-sort to put similar-named paths closer together
+        library {action} -C         # equivalent
+
+        library {action} --big-dirs # Recommended to use with --duration or --depth filters; see `lb big-dirs -h` for more info
+        library {action} -B         # equivalent
 
         All of these options can be used together but it will be a bit slow and the results might be mid-tier
         as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
         library {action} -RRCOO
 
     Filter media by file siblings of parent directory:
         library {action} --sibling   # only include files which have more than or equal to one sibling
@@ -170,25 +175,29 @@
         library {action} --lower 3   # only include files which have three or more siblings
         library {action} --upper 3   # only include files which have fewer than three siblings
         library {action} --lower 3 --upper 3   # only include files which are three siblings inclusive
         library {action} --lower 12 --upper 25 -OOO  # on my machine this launches My Mister 2018
 
     Play recent partially-watched videos (requires mpv history):
         library {action} --partial       # play newest first
+
         library {action} --partial old   # play oldest first
         library {action} -P o            # equivalent
-        library {action} -P p            # sort by progress / duration
+
+        library {action} -P p            # sort by percent remaining
+        library {action} -P t            # sort by time remaining
         library {action} -P s            # skip partially watched (only show unseen)
 
         The default time used is "last-viewed" (ie. the most recent time you closed the video)
         If you want to use the "first-viewed" time (ie. the very first time you opened the video)
         library {action} -P f            # use watch_later file creation time instead of modified time
 
         You can combine most of these options, though some will be overridden by others.
         library {action} -P fo           # this means "show the oldest videos using the time I first opened them"
+        library {action} -P pt           # weighted remaining (percent * time remaining)
 
     Print instead of play:
         library {action} --print --limit 10  # print the next 10 files
         library {action} -p -L 10  # print the next 10 files
         library {action} -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
@@ -378,37 +387,42 @@
         library {action} -m 4 --hstack          # use hstack style
 """
 
 
 watch = play("watch")
 
 
-redditadd = """library redditadd [--lookback N_DAYS] [--praw-site bot1] [database] paths ...
+redditadd = """library redditadd [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
 
     Fetch data for redditors and reddits:
 
-        library redditadd https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
+        library redditadd interesting.db https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
 
     If you have a file with a list of subreddits you can do this:
 
-        library redditadd --subreddits --db 96_Weird_History.db (cat ~/mc/96_Weird_History-reddit.txt)
+        library redditadd 96_Weird_History.db --subreddits (cat ~/mc/96_Weird_History-reddit.txt)
 
     Likewise for redditors:
 
-        library redditadd --redditors --db idk.db (cat ~/mc/shadow_banned.txt)
+        library redditadd shadow_banned.db --redditors (cat ~/mc/shadow_banned.txt)
+
+    Note that reddit's API is limited to 1000 posts and it usually doesn't go back very far historically.
+    Also, it may be the case that reddit's API (praw) will stop working in the near future. For both of these problems
+    my suggestion is to use pushshift data.
+    You can find more info here: https://github.com/chapmanjacobd/reddit_mining#how-was-this-made
 """
 
-redditupdate = """library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] [database]
+redditupdate = """library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 """
 
-search = """library search
+search = """library search DATABASE QUERY
 
     Search text databases and subtitles
 
     $ library search fts.db boil
         7 captions
         /mnt/d/70_Now_Watching/DidubeTheLastStop-720p.mp4
            33:46 I brought a real stainless steel boiler
@@ -416,18 +430,18 @@
            34:02 The boiler is old and authentic
            34:30 - This boiler? - Yes
            34:44 I am not forcing you to buy this boiler…
            34:52 Who will give her a one liter stainless steel boiler for one Lari?
            34:54 Glass boilers cost two
 
     Search and open file
-    $ library search fts.db dashi --open
+    $ library search fts.db 'two words' --open
 """
 
-history = """library history [--frequency daily|weekly|{monthly}|quarterly|yearly] [--limit LIMIT] DATABASE [{all}|watching|watched|deleted|created|modified]
+history = """library history [--frequency daily weekly (monthly) yearly] [--limit LIMIT] DATABASE [(all) watching watched created modified deleted]
 
     Explore history through different facets
 
     $ library history video.db watched
     Finished watching:
     ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
     │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
@@ -441,14 +455,76 @@
     │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
     ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
     │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
     ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
     │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
     ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
 
+    $ library history video.db created --frequency yearly
+    Created media:
+    ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │   time_period │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │          2005 │ 9.78 minutes                               │ 1.95 minutes   │ 16.9 MB    │ 3.4 MB     │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2006 │ 7 hours and 10.67 minutes                  │ 5 minutes      │ 891.1 MB   │ 10.4 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2007 │ 1 day, 17 hours and 33 minutes             │ 8.55 minutes   │ 5.9 GB     │ 20.3 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2008 │ 5 days, 16 hours and 10 minutes            │ 17.02 minutes  │ 20.7 GB    │ 43.1 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2009 │ 24 days, 2 hours and 56 minutes            │ 33.68 minutes  │ 108.4 GB   │ 105.2 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2010 │ 1 month, 1 days and 1 minutes              │ 35.52 minutes  │ 124.2 GB   │ 95.7 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2011 │ 2 months, 14 days, 1 hour and 22 minutes   │ 55.93 minutes  │ 222.0 GB   │ 114.9 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2012 │ 2 months, 22 days, 19 hours and 17 minutes │ 45.50 minutes  │ 343.6 GB   │ 129.6 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2013 │ 3 months, 11 days, 21 hours and 48 minutes │ 42.72 minutes  │ 461.1 GB   │ 131.7 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2014 │ 3 months, 7 days, 10 hours and 22 minutes  │ 46.80 minutes  │ 529.6 GB   │ 173.1 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2015 │ 2 months, 21 days, 23 hours and 36 minutes │ 36.73 minutes  │ 452.7 GB   │ 139.2 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2016 │ 3 months, 26 days, 7 hours and 59 minutes  │ 39.48 minutes  │ 603.4 GB   │ 139.9 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2017 │ 3 months, 10 days, 2 hours and 19 minutes  │ 31.78 minutes  │ 543.5 GB   │ 117.5 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2018 │ 3 months, 21 days, 20 hours and 56 minutes │ 30.98 minutes  │ 607.5 GB   │ 114.8 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2019 │ 5 months, 23 days, 2 hours and 30 minutes  │ 35.77 minutes  │ 919.7 GB   │ 129.7 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2020 │ 7 months, 16 days, 10 hours and 58 minutes │ 26.15 minutes  │ 1.2 TB     │ 93.9 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2021 │ 7 months, 21 days, 9 hours and 40 minutes  │ 39.93 minutes  │ 1.3 TB     │ 149.9 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2022 │ 17 years, 3 months, 0 days and 21 hours    │ 19.62 minutes  │ 35.8 TB    │ 77.5 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2023 │ 15 years, 3 months, 24 days and 1 hours    │ 17.57 minutes  │ 27.6 TB    │ 60.2 MB    │
+    ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
+    ╒════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤════════════════╕
+    │ title_path                                                                                 │ duration      │ time_created   │
+    ╞════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪════════════════╡
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 07/20 | Adam Cheng | 2009 #Chinesedrama │ 43.85 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=zntYD1yLrG8                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 08/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=zQnSfoWrh-4                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 06/20 | Adam Cheng | 2009 #Chinesedrama │ 43.60 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=Qiax1kFyGWU                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 04/20 | Adam Cheng | 2009 #Chinesedrama │ 43.45 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=NT9C3PRrlTA                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 02/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=MjpCiTawlTE                                                │               │                │
+    ╘════════════════════════════════════════════════════════════════════════════════════════════╧═══════════════╧════════════════╛
+
     $ library history video.db deleted
     Deleted media:
     ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
     │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
     ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
     │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
     ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
@@ -462,15 +538,15 @@
     ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
     │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
     │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
     ...
 
 """
 
-playlists = """library playlists [database] [--aggregate] [--fields] [--json] [--delete ...]
+playlists = """library playlists DATABASE [--aggregate] [--fields] [--json] [--delete ...]
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
         │ ie_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
@@ -494,15 +570,15 @@
         https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n
 
     Remove a playlist/channel and all linked videos:
         library playlists --remove https://vimeo.com/canal180
 
 """
 
-download_status = """library download-status [database]
+download_status = """library download-status DATABASE
 
     Print download queue groups
 
         library download-status video.db
         ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
@@ -622,15 +698,15 @@
 
     Importing from a line-delimitated file:
 
         library tabsadd -f yearly -c reddit ~/lb/tabs.db (cat ~/mc/yearly-subreddit.cron)
 
 """
 
-tubeadd = r"""library tubeadd [--audio | --video] [-c CATEGORY] [database] playlists ...
+tubeadd = r"""library tubeadd [-c CATEGORY] [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
@@ -656,15 +732,15 @@
         By default tubeadd will quickly add media at the expense of less metadata.
         If you plan on using `library download` then it doesn't make sense to use `--extra`.
         Downloading will add the extra metadata automatically to the database.
         You can always fetch more metadata later via tubeupdate:
         library tubeupdate tw.db --extra
 """
 
-tubeupdate = """library tubeupdate [--audio | --video] [-c CATEGORY] [database]
+tubeupdate = """library tubeupdate [--audio | --video] [-c CATEGORY] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
     Or limit to specific categories...
 
@@ -678,15 +754,15 @@
 
         By default tubeupdate will quickly add media.
         You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
 
         library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 """
 
-bigdirs = """library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
+bigdirs = """library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
 
     See what folders take up space
 
         library bigdirs video.db
         library bigdirs audio.db
         library bigdirs fs.db
 """
@@ -719,20 +795,37 @@
         library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 """
 dedupe = """library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
     Dedupe your files
 """
 
-merge_dbs = """library merge-dbs DEST_DB SOURCE_DB ... [--upsert pk1[,pk2]]
+merge_dbs = """library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
+
+    Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
+    and there is an existing row with the same PK, the default action is to delete the existing row and insert the new row
+    replacing all existing fields.
+
+    Upsert mode will update matching PK rows such that if a source row has a NULL field and
+    the destination row has a value then the value will be preserved instead of changed to the source row's NULL value.
+
+    Ignore mode (--only-new-rows) will insert only rows which don't already exist in the destination db
+
+    Test first by using temp databases as the destination db.
+    Try out different modes / flags until you are satisfied with the behavior of the program
+
+        library merge-dbs --pk path (mktemp --suffix .db) tv.db movies.db
 
     Merge database data and tables
 
         library merge-dbs --upsert --pk path video.db tv.db movies.db
-        library merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
+        library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path audio-fts.db audio.db
+
+        library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
+        library merge-dbs --only-new-rows --pk playlist_path,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
 """
 
 merge_online_local = """library merge-online-local DATABASE
 
     If you have previously downloaded YouTube or other online media, you can dedupe
     your database and combine the online and local media records as long as your
     files have the youtube-dl / yt-dlp id in the filename.
@@ -793,15 +886,15 @@
 
         # move new music for this week
         library relmv (
             library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 """
 
-scatter = """library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS database relative_paths ...
+scatter = """library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS DATABASE RELATIVE_PATHS ...
 
     Balance size
 
         $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
@@ -869,15 +962,15 @@
     You will likely want to use this setting in `about:config`
 
         browser.tabs.loadDivertedInBackground = True
 
     If you prefer GUI, check out https://unli.xyz/tabsender/
 """
 
-pushshift = """library pushshift [database] < stdin
+pushshift = """library pushshift DATABASE < stdin
 
     Download data (about 600GB jsonl.zst; 6TB uncompressed)
 
         wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
 
     Load data from files via unzstd
```

### Comparing `xklb-1.29.8/xklb/utils.py` & `xklb-1.30.2/xklb/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import argparse, csv, enum, functools, hashlib, logging, math, multiprocessing, os, platform, random, re, shlex, shutil, signal, string, subprocess, sys, tempfile, textwrap, time
+import argparse, csv, functools, hashlib, logging, math, multiprocessing, os, platform, random, re, shlex, shutil, signal, string, subprocess, sys, tempfile, time
 from ast import literal_eval
 from collections.abc import Iterable
+from copy import deepcopy
 from datetime import datetime, timedelta, timezone
 from functools import wraps
 from pathlib import Path
 from random import shuffle
 from shutil import which
 from timeit import default_timer
 from typing import Any, Dict, Generator, List, NoReturn, Optional, Union
@@ -369,14 +370,18 @@
 def safe_int(s) -> Optional[int]:
     try:
         return int(float(s))
     except Exception:
         return None
 
 
+def concat(*args):
+    return (part for part in args if part)
+
+
 def extract_words(string):
     if not string:
         return None
 
     cleaned_string = re.sub(r"[^\w\s]", " ", string)
     words = [remove_consecutive_whitespace(s) for s in cleaned_string.split()]
     words = [
@@ -503,40 +508,42 @@
     paths = set(Path(args.watch_later_directory).glob("*"))
 
     previously_watched = [
         {
             **(md5s.get(p.stem) or {}),
             "time_partial_first": int(p.stat().st_ctime),
             "time_partial_last": int(p.stat().st_mtime),
-            "progress": safe_int(mpv_watchlater_value(p, "start")),
+            "playhead": safe_int(mpv_watchlater_value(p, "start")),
         }
         for p in paths
         if md5s.get(p.stem)
     ]
     if "s" in args.partial:  # skip; only play unseen
         previously_watched_paths = [m["path"] for m in previously_watched]
         return [m for m in media if m["path"] not in previously_watched_paths]
 
     def mpv_progress(m):
-        progress = m.get("progress")
+        playhead = m.get("playhead")
         duration = m.get("duration")
-        if not progress:
-            return 0.0
+        if not playhead:
+            return float("-inf")
         if not duration:
-            return progress / 100  # TODO: idk
+            return float("-max")
 
-        if "w" in args.partial:  # weight by total time
-            return progress / duration * progress
+        if "p" in args.partial and "t" in args.partial:
+            return (duration / playhead) * -(duration - playhead)  # weighted remaining
+        elif "t" in args.partial:
+            return -(duration - playhead)  # time remaining
         else:
-            return progress / duration
+            return playhead / duration  # percent remaining
 
     def sorting_hat():
         if "f" in args.partial:  # first-viewed
             return lambda m: m.get("time_partial_first") or 0
-        elif "p" in args.partial:  # sort by remaining duration
+        elif "p" in args.partial or "t" in args.partial:  # sort by remaining duration
             return mpv_progress
 
         return lambda m: m.get("time_partial_last") or m.get("time_partial_first") or 0
 
     reverse_chronology = True
     if "o" in args.partial:  # oldest first
         reverse_chronology = False
@@ -639,18 +646,38 @@
 
     try:
         return list_[idx]
     except IndexError:
         return None
 
 
+def path_fill(text, size):
+    width = max(10, int(size * (consts.TERMINAL_SIZE.columns / 80)))
+    lines = []
+    current_line = ""
+    for char in text:
+        if char == "\r":
+            continue  # Ignore carriage return character
+        elif char == "\n":
+            lines.append(current_line)
+            current_line = ""
+        else:
+            current_line += char
+            if len(current_line) == width:
+                lines.append(current_line)
+                current_line = ""
+    if current_line:
+        lines.append(current_line)
+    return "\n".join(lines)
+
+
 def col_resize(tbl: List[Dict], col: str, size=10) -> List[Dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
-            tbl[idx][col] = textwrap.fill(tbl[idx][col], max(10, int(size * (consts.TERMINAL_SIZE.columns / 80))))
+            tbl[idx][col] = path_fill(tbl[idx][col], size)
 
     return tbl
 
 
 def col_naturaldate(tbl: List[Dict], col: str) -> List[Dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
@@ -716,16 +743,15 @@
     return tbl
 
 
 class ArgparseList(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         items = getattr(namespace, self.dest, None) or []
 
-        for value in values or []:
-            items.extend(value.split(","))
+        items.extend(values.split(","))  # type: ignore
 
         setattr(namespace, self.dest, items)
 
 
 class ArgparseDict(argparse.Action):
     def __call__(self, parser, args, values, option_string=None):
         try:
@@ -1111,14 +1137,23 @@
             "grouped_paths": sorted(paths),
         }
         result.append(metadata)
 
     return result
 
 
+def cluster_dicts(media):
+    media_keyed = {d["path"]: d for d in media}
+    groups = cluster_paths([d["path"] for d in media])
+    groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
+    sorted_paths = flatten(d["grouped_paths"] for d in groups)
+    media = [media_keyed[p] for p in sorted_paths]
+    return media
+
+
 def is_timecode_like(text):
     for char in text:
         if not (char in ":,_-;. " or char.isdigit()):
             return False
     return True
 
 
@@ -1140,7 +1175,83 @@
 
 def order_set(items):
     seen = set()
     for item in items:
         if item not in seen:
             yield item
             seen.add(item)
+
+
+def partial_startswith(original_string, startswith_match_list):
+    matching_strings = []
+
+    candidate = deepcopy(original_string)
+    while len(matching_strings) == 0 and len(candidate) > 0:
+        for s in startswith_match_list:
+            if s.startswith(candidate):
+                matching_strings.append(s)
+
+        if len(matching_strings) == 0:
+            candidate = candidate[:-1]  # remove the last char
+
+    if len(matching_strings) == 1:
+        return matching_strings[0]
+    else:
+        msg = f"{original_string} does not match any of {startswith_match_list}"
+        raise ValueError(msg)
+
+
+def compare_block_strings(value, media_value):
+    value = value.lower()
+    media_value = media_value.lower()
+
+    starts_with_wild = value.startswith("%")
+    ends_with_wild = value.endswith("%")
+    inner_value = value.lstrip("%").rstrip("%")
+    inner_wild = "%" in inner_value
+
+    if inner_wild:
+        regex_pattern = value.replace("%", ".*")
+        return bool(re.match(regex_pattern, media_value))
+    elif not ends_with_wild and not starts_with_wild:
+        return media_value.startswith(value)
+    elif ends_with_wild and not starts_with_wild:
+        return media_value.startswith(value.rstrip("%"))
+    elif starts_with_wild and not ends_with_wild:
+        return media_value.endswith(value.lstrip("%"))
+    elif starts_with_wild and ends_with_wild:
+        return inner_value in media_value
+    raise ValueError("Unreachable?")
+
+
+def block_dicts_like_sql(media, blocklist):
+    not_blocked_media = []
+    for m in media:
+        is_blocked = False
+        for block_dict in blocklist:
+            for key, value in block_dict.items():
+                if key in m and compare_block_strings(value, m[key]):
+                    is_blocked = True
+                    break
+            if is_blocked:
+                break
+        if not is_blocked:
+            not_blocked_media.append(m)
+
+    return not_blocked_media
+
+
+def allow_dicts_like_sql(media, allowlist):
+    allowed_media = []
+    for m in media:
+        is_blocked = False
+        for block_dict in allowlist:
+            for key, value in block_dict.items():
+                if key in m and compare_block_strings(value, m[key]):
+                    is_blocked = True
+                    break
+            if is_blocked:
+                break
+        if is_blocked:
+            allowed_media.append(m)
+
+    return allowed_media
```

### Comparing `xklb-1.29.8/xklb/scripts/bigdirs.py` & `xklb-1.30.2/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/christen.py` & `xklb-1.30.2/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/cluster_sort.py` & `xklb-1.30.2/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/copy_play_counts.py` & `xklb-1.30.2/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/dedupe.py` & `xklb-1.30.2/xklb/scripts/dedupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
         "--audio",
         action="store_const",
         dest="profile",
         const=DBType.audio,
         help="Dedupe database by artist + album + title",
     )
     profile.add_argument(
-        "--id",
+        "--tube-id",
         action="store_const",
         dest="profile",
-        const="id",
-        help="Dedupe database by id + ie_key",
+        const="tube_id",
+        help="Dedupe database by tube_id + ie_key",
     )
     profile.add_argument(
         "--title",
         action="store_const",
         dest="profile",
         const="title",
         help="Dedupe database by title + uploader",
@@ -121,23 +121,23 @@
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
         , m2.path duplicate_path
         , m2.size duplicate_size
     FROM
         media m1
     JOIN media m2 on 1=1
-        and m1.id = m2.id
+        and m1.tube_id = m2.tube_id
         and m1.duration >= m2.duration - 4
         and m1.duration <= m2.duration + 4
         and m1.ie_key in (m2.ie_key, 'Local')
         and m2.path != m1.path
     WHERE 1=1
         and m1.time_deleted = 0 and m2.time_deleted = 0
         and abs(m1.sparseness - 1) < 0.1
-        and m1.id != '' and m1.ie_key != ''
+        and m1.tube_id != '' and m1.ie_key != ''
     ORDER BY 1=1
         , m1.video_count > 0 DESC
         , m1.subtitle_count > 0 DESC
         , m1.audio_count DESC
         , length(m1.path)-length(REPLACE(m1.path, '/', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
         , length(m1.path)
@@ -193,15 +193,15 @@
 
 
 def dedupe() -> None:
     args = parse_args()
 
     if args.profile == DBType.audio:
         duplicates = get_music_duplicates(args)
-    elif args.profile == "id":
+    elif args.profile == "tube_id":
         duplicates = get_id_duplicates(args)
     elif args.profile == "title":
         duplicates = get_title_duplicates(args)
     elif args.profile == DBType.filesystem:
         print(
             """
         You should use `rmlint` instead:
```

### Comparing `xklb-1.29.8/xklb/scripts/download_status.py` & `xklb-1.30.2/xklb/scripts/download_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse, json
 from copy import deepcopy
-from typing import Tuple
 
 from tabulate import tabulate
 
 from xklb import consts, db, dl_extract, play_actions, tube_backend, usage, utils
 from xklb.player import delete_playlists
 from xklb.utils import log
 
@@ -44,55 +43,23 @@
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     args.action = consts.SC.stats
     return args
 
 
-def construct_query(args) -> Tuple[str, dict]:
-    utils.ensure_playlists_exists(args)
-    pl_columns = args.db["playlists"].columns_dict
-    args.filter_sql = []
-    args.filter_bindings = {}
-
-    args.filter_sql.extend([" and " + w for w in args.where])
-
-    args.table = "playlists"
-    if args.db["playlists"].detect_fts():
-        if args.include:
-            args.table = db.fts_flexible_search(args)
-        elif args.exclude:
-            db.construct_search_bindings(args, pl_columns)
-    else:
-        db.construct_search_bindings(args, pl_columns)
-
-    LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
-    query = f"""SELECT
-        *
-    FROM {args.table}
-    WHERE 1=1
-        and COALESCE(time_deleted,0) = 0
-        {" ".join(args.filter_sql)}
-        and (category is null or category != '{consts.BLOCK_THE_CHANNEL}')
-    ORDER BY 1=1
-        {', ' + args.sort if args.sort else ''}
-        , path
-        , random()
-    {LIMIT}
-    """
-
-    return query, args.filter_bindings
-
-
 def printer(args, query, bindings) -> None:
     media = list(args.db.query(query, bindings))
     media = utils.list_dict_filter_bool(media)
     if not media:
         utils.no_media_found()
 
+    if "blocklist" in args.db.table_names():
+        media = utils.block_dicts_like_sql(media, [{d["key"]: d["value"]} for d in args.db["blocklist"].rows])
+
     tbl = deepcopy(media)
     utils.col_naturaldate(tbl, "avg_time_since_download")
     utils.col_naturalsize(tbl, "size")
     utils.col_duration(tbl, "duration")
     utils.col_duration(tbl, "avg_playlist_duration")
 
     if args.print and "f" in args.print:
```

### Comparing `xklb-1.29.8/xklb/scripts/history.py` & `xklb-1.30.2/xklb/scripts/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, enum
+import argparse
 
 from tabulate import tabulate
 
 from xklb import consts, db, player, usage, utils
 from xklb.utils import log
 
 
@@ -13,20 +13,19 @@
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument(
         "--frequency",
         "--freqency",
         "-f",
         metavar="frequency",
-        choices=consts.frequency,
         default="monthly",
         const="monthly",
         type=str.lower,
         nargs="?",
-        help=f"One of: %(choices)s (default: %(default)s)",
+        help="One of: %(choices)s (default: %(default)s)",
     )
 
     parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
@@ -35,23 +34,26 @@
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     parser.add_argument(
         "facet",
         metavar="facet",
-        choices=["all", *consts.time_facets],
         type=str.lower,
         default="all",
         const="all",
         nargs="?",
-        help=f"One of: %(choices)s (default: %(default)s)",
+        help="One of: %(choices)s (default: %(default)s)",
     )
 
     args = parser.parse_args()
+
+    args.facet = utils.partial_startswith(args.facet, consts.time_facets)
+    args.frequency = utils.partial_startswith(args.frequency, consts.frequency)
+
     if args.db:
         args.database = args.db
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
@@ -63,21 +65,23 @@
     utils.col_naturalsize(tbl, "size_avg")
     tbl = utils.list_dict_filter_bool(tbl)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
 
 def print_recent(tbl, time_column=None):
     utils.col_duration(tbl, "duration")
+    utils.col_duration(tbl, "playhead")
     if time_column:
         utils.col_naturaldate(tbl, time_column)
-    tbl = [{"title_path": f"{d['title']}\n{d['path']}" if d["title"] is not None else d["path"], **d} for d in tbl]
+    tbl = [{"title_path": "\n".join(utils.concat(d["title"], d["path"])), **d} for d in tbl]
     tbl = [{k: v for k, v in d.items() if k not in ("title", "path")} for d in tbl]
 
     tbl = utils.col_resize(tbl, "title_path", 40)
     tbl = utils.col_resize(tbl, "duration", 5)
+    tbl = utils.col_resize(tbl, "playhead", 5)
     tbl = utils.list_dict_filter_bool(tbl)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
 
 def recent_media(args, time_column):
     query = f"""
     SELECT
@@ -95,36 +99,36 @@
 
 
 def history() -> None:
     args = parse_args()
 
     if args.facet.startswith(("all", "watching")):
         print("Partially watched:")
-        tbl = player.historical_usage(args, args.frequency, f"time_played", "and coalesce(play_count, 0)=0")
+        tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)=0")
         print_history(tbl)
         query = f"""SELECT
                 path
                 , title
                 , duration
                 , subtitle_count
                 , time_played
                 , playhead
             FROM media
-            WHERE coalesce(time_deleted, 0)=0
-                and coalesce(playhead, 0)>0
-                and coalesce(play_count, 0)=0
+            WHERE coalesce(time_deleted, 0) = 0
+                and coalesce(playhead, 0) > 60
+                and coalesce(play_count, 0) = 0
             ORDER BY time_played desc, playhead desc
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_played")
 
     elif args.facet.startswith(("all", "watched")):
         print("Finished watching:")
-        tbl = player.historical_usage(args, args.frequency, f"time_played", "and coalesce(play_count, 0)>0")
+        tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)>0")
         print_history(tbl)
         query = f"""SELECT
                 path
                 , title
                 , duration
                 , subtitle_count
                 , time_played
```

### Comparing `xklb-1.29.8/xklb/scripts/merge_dbs.py` & `xklb-1.30.2/xklb/scripts/merge_dbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 from xklb import db, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-dbs", usage=usage.merge_dbs)
-    parser.add_argument("--pk", nargs="+", action=utils.ArgparseList, help="Comma separated primary keys")
-    parser.add_argument("--table", "-t", nargs="+", action=utils.ArgparseList, help="Limit to specific table(s)")
+    parser.add_argument("--pk", action=utils.ArgparseList, help="Comma separated primary keys")
     parser.add_argument("--upsert", action="store_true")
     parser.add_argument("--ignore", "--only-new-rows", action="store_true")
+    parser.add_argument("--only-tables", "-t", action=utils.ArgparseList, help="Comma separated specific table(s)")
     parser.add_argument("--only-target-columns", action="store_true")
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("database")
     parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
@@ -30,15 +30,15 @@
 
 
 def merge_db(args, source_db) -> None:
     source_db = str(Path(source_db).resolve())
 
     s_db = db.connect(argparse.Namespace(database=source_db, verbose=args.verbose))
     for table in [s for s in s_db.table_names() if "_fts" not in s and not s.startswith("sqlite_")]:
-        if args.table and table not in args.table:
+        if args.only_tables and table not in args.only_tables:
             log.info("[%s]: Skipping %s", source_db, table)
             continue
         else:
             log.info("[%s]: %s", source_db, table)
 
         source_columns = s_db[table].columns_dict
         if args.only_target_columns:
```

### Comparing `xklb-1.29.8/xklb/scripts/merge_online_local.py` & `xklb-1.30.2/xklb/scripts/merge_online_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             and time_deleted = 0
             and id is null
             and title is null
     ) m2
     JOIN media_fts on m2.rowid = media_fts.rowid
     WHERE m2.ie_key = 'Local'
         AND m1.ie_key NOT IN ('NBCStations', 'TedTalk', 'ThisAmericanLife', 'InfoQ', 'NFB', 'KickStarter')
-        AND media_fts.path MATCH '"'||m1.id||'"'
-        AND m2.PATH LIKE '%['||m1.id||']%'
+        AND media_fts.path MATCH '"'||m1.tube_id||'"'
+        AND m2.PATH LIKE '%['||m1.tube_id||']%'
     ORDER BY 1=1
         , length(m2.path)-length(REPLACE(m2.path, '/', '')) desc
         , length(m2.path)-length(REPLACE(m2.path, '.', ''))
         , length(m2.path)
         , m2.time_modified desc
         , m2.time_created desc
         , m2.duration desc
@@ -94,24 +94,24 @@
             webpath = d["duplicate_path"]
             if webpath in merged or fspath == webpath:
                 continue
 
             tube_entry = get_dict(args, webpath)
             fs_tags = get_dict(args, fspath)
 
-            if not tube_entry or not fs_tags or tube_entry["id"] not in fs_tags["path"]:
+            if not tube_entry or not fs_tags or tube_entry["tube_id"] not in fs_tags["path"]:
                 continue
 
             if fs_tags["time_modified"] is None or fs_tags["time_modified"] == 0:
                 fs_tags["time_modified"] = consts.now()
             if fs_tags["time_downloaded"] is None or fs_tags["time_downloaded"] == 0:
                 fs_tags["time_downloaded"] = consts.APPLICATION_START
 
             entry = {**tube_entry, **fs_tags, "webpath": webpath}
-            args.db["media"].insert(utils.dict_filter_bool(entry), pk="path", alter=True, replace=True)  # type: ignore
+            args.db["media"].insert(utils.dict_filter_bool(entry), pk="id", alter=True, replace=True)  # type: ignore
             args.db["media"].delete(webpath)
             merged.append(webpath)
 
         print(len(merged), "merged")
 
 
 if __name__ == "__main__":
```

### Comparing `xklb-1.29.8/xklb/scripts/move_list.py` & `xklb-1.30.2/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/optimize_db.py` & `xklb-1.30.2/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/playlists.py` & `xklb-1.30.2/xklb/scripts/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     query = f"""SELECT
         *
     FROM {args.table}
     WHERE 1=1
         and COALESCE(time_deleted,0) = 0
         {" ".join(args.filter_sql)}
-        and (category is null or category != '{consts.BLOCK_THE_CHANNEL}')
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
         , path
         , random()
     {LIMIT}
     """
```

### Comparing `xklb-1.29.8/xklb/scripts/redownload.py` & `xklb-1.30.2/xklb/scripts/redownload.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,17 @@
         d["time_downloaded"] = 0
         d.pop("error", None)
 
         if "webpath" in m_columns and (d.get("webpath") or "").startswith("http"):
             args.db["media"].delete(d["path"])  # type: ignore
 
             d["path"] = d["webpath"]
-            args.db["media"].upsert(d, pk="path", alter=True)  # type: ignore
+            args.db["media"].upsert(d, pk="id", alter=True)  # type: ignore
         else:
-            args.db["media"].upsert(d, pk="path", alter=True)  # type: ignore
+            args.db["media"].upsert(d, pk="id", alter=True)  # type: ignore
 
 
 def print_deletions(args, deletions) -> None:
     print("Deletions:")
     tbl = deepcopy(deletions)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
     print(f"Showing most recent {args.limit} deletions. Use -l to change this limit")
@@ -134,15 +134,15 @@
     else:
         deletions = list_deletions(args)
         print_deletions(args, deletions)
         raise SystemExit(0)
 
     print_deleted(args, deleted_media)
     paths = [d["path"] for d in deleted_media]
-    redownload_ids = [d["id"] for d in deleted_media if d.get("id")]
+    redownload_ids = [d["tube_id"] for d in deleted_media if d.get("tube_id")]
     print(len(redownload_ids), "tube ids found")
     if deleted_media and utils.confirm("Redownload media?"):  # type: ignore
         if len(redownload_ids) > 0:
             download_archive = Path(args.download_archive).expanduser().resolve()
             if download_archive.exists():
                 utils.filter_file(str(download_archive), redownload_ids)
```

### Comparing `xklb-1.29.8/xklb/scripts/relmv.py` & `xklb-1.30.2/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/scatter.py` & `xklb-1.30.2/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/streaming_tab_loader.py` & `xklb-1.30.2/xklb/scripts/streaming_tab_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def streaming_tab_loader() -> None:
     args = parse_args()
 
     try:
         from brotab.api import SingleMediatorAPI
         from brotab.main import create_clients
     except ModuleNotFoundError:
-        print("brotab is required for surfing. Install with pip install brotab or pip install xklb[full]")
+        print("brotab is required for surfing. Install with pip install brotab or pip install xklb[deluxe]")
         raise
     else:
         logging.getLogger("brotab").setLevel(log.level)
         args.bt_api = SingleMediatorAPI(create_clients(args.target_hosts))  # type: ignore
 
     tabs_opened = 0
     initial_count = len(list_tabs(args))
```

### Comparing `xklb-1.29.8/xklb/scripts/mining/data.py` & `xklb-1.30.2/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/mining/extract_links.py` & `xklb-1.30.2/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/mining/nouns.py` & `xklb-1.30.2/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/mining/pushshift.py` & `xklb-1.30.2/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.30.2/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/xklb/assets/kotobago.png` & `xklb-1.30.2/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/.gitignore` & `xklb-1.30.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/LICENSE` & `xklb-1.30.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.29.8/README.md` & `xklb-1.30.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,91 @@
+Metadata-Version: 2.1
+Name: xklb
+Version: 1.30.2
+Summary: xk library
+Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
+Project-URL: homepage, https://github.com/chapmanjacobd/library/
+Project-URL: repository, https://github.com/chapmanjacobd/library/
+Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
+License: BSD 3-Clause No Nuclear License
+        
+        Copyright (c) 2021, Jacob Chapman
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+        You acknowledge that this software is not designed nor intended for use in the
+        design, construction, operation or maintenance of any nuclear facility.
+License-File: LICENSE
+Requires-Python: >=3.8
+Requires-Dist: catt
+Requires-Dist: ffmpeg-python
+Requires-Dist: ftfy
+Requires-Dist: gallery-dl
+Requires-Dist: humanize
+Requires-Dist: ipython
+Requires-Dist: markdown
+Requires-Dist: mutagen
+Requires-Dist: natsort
+Requires-Dist: praw
+Requires-Dist: pysubs2
+Requires-Dist: python-mpv-jsonipc
+Requires-Dist: regex
+Requires-Dist: rich
+Requires-Dist: screeninfo
+Requires-Dist: sqlite-utils>=3.30
+Requires-Dist: subliminal
+Requires-Dist: tabulate
+Requires-Dist: tinytag
+Requires-Dist: yt-dlp
+Provides-Extra: all
+Requires-Dist: xklb[deluxe,dev,test]; extra == 'all'
+Provides-Extra: deluxe
+Requires-Dist: aiohttp; extra == 'deluxe'
+Requires-Dist: brotab; extra == 'deluxe'
+Requires-Dist: orjson; extra == 'deluxe'
+Requires-Dist: pandas; extra == 'deluxe'
+Requires-Dist: pyexiftool; extra == 'deluxe'
+Requires-Dist: sklearn; extra == 'deluxe'
+Requires-Dist: spacy; extra == 'deluxe'
+Requires-Dist: textract; extra == 'deluxe'
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: ipdb; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: scalene; extra == 'dev'
+Requires-Dist: ssort; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: ruff; extra == 'test'
+Description-Content-Type: text/markdown
+
 # xk media library
 
 A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
@@ -139,15 +223,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.008)
+    xk media library subcommands (v1.30.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -316,15 +400,15 @@
 
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
 
     library scatter -h
-    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS database relative_paths ...
+    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS DATABASE RELATIVE_PATHS ...
 
     Balance size
 
         $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
@@ -518,15 +602,15 @@
 
 ## Usage
 
 
 <details><summary>Add local media (fsadd)</summary>
 
     $ library fsadd -h
-    usage: library fsadd [--audio | --video | --image |  --text | --filesystem] -c CATEGORY [database] paths ...
+    usage: library fsadd [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATHS ...
 
     The default database type is video:
         library fsadd tv.db ./tv/
         library fsadd --video tv.db ./tv/  # equivalent
 
     You can also create audio databases. Both audio and video use ffmpeg to read metadata:
         library fsadd --audio audio.db ./music/
@@ -570,15 +654,15 @@
 
 
 </details>
 
 <details><summary>Add online media (tubeadd)</summary>
 
     $ library tubeadd -h
-    usage: library tubeadd [--audio | --video] [-c CATEGORY] [database] playlists ...
+    usage: library tubeadd [-c CATEGORY] [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
@@ -609,35 +693,40 @@
 
 
 </details>
 
 <details><summary>Add reddit media (redditadd)</summary>
 
     $ library redditadd -h
-    usage: library redditadd [--lookback N_DAYS] [--praw-site bot1] [database] paths ...
+    usage: library redditadd [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
 
     Fetch data for redditors and reddits:
 
-        library redditadd https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
+        library redditadd interesting.db https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
 
     If you have a file with a list of subreddits you can do this:
 
-        library redditadd --subreddits --db 96_Weird_History.db (cat ~/mc/96_Weird_History-reddit.txt)
+        library redditadd 96_Weird_History.db --subreddits (cat ~/mc/96_Weird_History-reddit.txt)
 
     Likewise for redditors:
 
-        library redditadd --redditors --db idk.db (cat ~/mc/shadow_banned.txt)
+        library redditadd shadow_banned.db --redditors (cat ~/mc/shadow_banned.txt)
+
+    Note that reddit's API is limited to 1000 posts and it usually doesn't go back very far historically.
+    Also, it may be the case that reddit's API (praw) will stop working in the near future. For both of these problems
+    my suggestion is to use pushshift data.
+    You can find more info here: https://github.com/chapmanjacobd/reddit_mining#how-was-this-made
 
 
 </details>
 
 <details><summary>Create / Update a Hacker News database (hnadd)</summary>
 
     $ library hnadd -h
-    usage: library hnadd [--oldest] database
+    usage: library hnadd [--oldest] DATABASE
 
     Fetch latest stories first:
 
         library hnadd hn.db -v
         Fetching 154873 items (33212696 to 33367569)
         Saving comment 33367568
         Saving comment 33367543
@@ -675,15 +764,15 @@
 
 
 </details>
 
 <details><summary>Watch / Listen</summary>
 
     $ library watch -h
-    usage: library watch [database] [optional args]
+    usage: library watch DATABASE [optional args]
 
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
         Create global shortcuts in your desktop environment by sending commands to mpv_socket:
         echo 'playlist-next force' | socat - /tmp/mpv_socket
 
@@ -701,19 +790,23 @@
         library watch --play-in-order
         There are multiple strictness levels of --play-in-order:
         library watch -O    # equivalent
         library watch -OO   # above, plus ignores most filters
         library watch -OOO  # above, plus ignores fts and (include/exclude) filter during ordinal search
         library watch -OOOO # above, plus starts search with parent folder
 
-        library watch --related  # similar to -O but uses fts to find similar content
+        library watch --related  # Similar to -O but uses fts to find similar content
         library watch -R         # equivalent
         library watch -RR        # above, plus ignores most filters
 
-        library watch --cluster  # cluster-sort to put similar paths closer together
+        library watch --cluster  # cluster-sort to put similar-named paths closer together
+        library watch -C         # equivalent
+
+        library watch --big-dirs # Recommended to use with --duration or --depth filters; see `lb big-dirs -h` for more info
+        library watch -B         # equivalent
 
         All of these options can be used together but it will be a bit slow and the results might be mid-tier
         as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
         library watch -RRCOO
 
     Filter media by file siblings of parent directory:
         library watch --sibling   # only include files which have more than or equal to one sibling
@@ -727,25 +820,29 @@
         library watch --lower 3   # only include files which have three or more siblings
         library watch --upper 3   # only include files which have fewer than three siblings
         library watch --lower 3 --upper 3   # only include files which are three siblings inclusive
         library watch --lower 12 --upper 25 -OOO  # on my machine this launches My Mister 2018
 
     Play recent partially-watched videos (requires mpv history):
         library watch --partial       # play newest first
+
         library watch --partial old   # play oldest first
         library watch -P o            # equivalent
-        library watch -P p            # sort by progress / duration
+
+        library watch -P p            # sort by percent remaining
+        library watch -P t            # sort by time remaining
         library watch -P s            # skip partially watched (only show unseen)
 
         The default time used is "last-viewed" (ie. the most recent time you closed the video)
         If you want to use the "first-viewed" time (ie. the very first time you opened the video)
         library watch -P f            # use watch_later file creation time instead of modified time
 
         You can combine most of these options, though some will be overridden by others.
         library watch -P fo           # this means "show the oldest videos using the time I first opened them"
+        library watch -P pt           # weighted remaining (percent * time remaining)
 
     Print instead of play:
         library watch --print --limit 10  # print the next 10 files
         library watch -p -L 10  # print the next 10 files
         library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
@@ -936,15 +1033,15 @@
 
 
 </details>
 
 <details><summary>Search captions / subtitles</summary>
 
     $ library search -h
-    usage: library search
+    usage: library search DATABASE QUERY
 
     Search text databases and subtitles
 
     $ library search fts.db boil
         7 captions
         /mnt/d/70_Now_Watching/DidubeTheLastStop-720p.mp4
            33:46 I brought a real stainless steel boiler
@@ -952,23 +1049,23 @@
            34:02 The boiler is old and authentic
            34:30 - This boiler? - Yes
            34:44 I am not forcing you to buy this boiler…
            34:52 Who will give her a one liter stainless steel boiler for one Lari?
            34:54 Glass boilers cost two
 
     Search and open file
-    $ library search fts.db dashi --open
+    $ library search fts.db 'two words' --open
 
 
 </details>
 
 <details><summary>History</summary>
 
     $ library history -h
-    usage: library history [--frequency daily|weekly|{monthly}|quarterly|yearly] [--limit LIMIT] DATABASE [{all}|watching|watched|deleted|created|modified]
+    usage: library history [--frequency daily weekly (monthly) yearly] [--limit LIMIT] DATABASE [(all) watching watched created modified deleted]
 
     Explore history through different facets
 
     $ library history video.db watched
     Finished watching:
     ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
     │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
@@ -982,14 +1079,76 @@
     │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
     ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
     │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
     ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
     │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
     ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
 
+    $ library history video.db created --frequency yearly
+    Created media:
+    ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │   time_period │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │          2005 │ 9.78 minutes                               │ 1.95 minutes   │ 16.9 MB    │ 3.4 MB     │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2006 │ 7 hours and 10.67 minutes                  │ 5 minutes      │ 891.1 MB   │ 10.4 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2007 │ 1 day, 17 hours and 33 minutes             │ 8.55 minutes   │ 5.9 GB     │ 20.3 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2008 │ 5 days, 16 hours and 10 minutes            │ 17.02 minutes  │ 20.7 GB    │ 43.1 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2009 │ 24 days, 2 hours and 56 minutes            │ 33.68 minutes  │ 108.4 GB   │ 105.2 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2010 │ 1 month, 1 days and 1 minutes              │ 35.52 minutes  │ 124.2 GB   │ 95.7 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2011 │ 2 months, 14 days, 1 hour and 22 minutes   │ 55.93 minutes  │ 222.0 GB   │ 114.9 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2012 │ 2 months, 22 days, 19 hours and 17 minutes │ 45.50 minutes  │ 343.6 GB   │ 129.6 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2013 │ 3 months, 11 days, 21 hours and 48 minutes │ 42.72 minutes  │ 461.1 GB   │ 131.7 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2014 │ 3 months, 7 days, 10 hours and 22 minutes  │ 46.80 minutes  │ 529.6 GB   │ 173.1 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2015 │ 2 months, 21 days, 23 hours and 36 minutes │ 36.73 minutes  │ 452.7 GB   │ 139.2 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2016 │ 3 months, 26 days, 7 hours and 59 minutes  │ 39.48 minutes  │ 603.4 GB   │ 139.9 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2017 │ 3 months, 10 days, 2 hours and 19 minutes  │ 31.78 minutes  │ 543.5 GB   │ 117.5 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2018 │ 3 months, 21 days, 20 hours and 56 minutes │ 30.98 minutes  │ 607.5 GB   │ 114.8 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2019 │ 5 months, 23 days, 2 hours and 30 minutes  │ 35.77 minutes  │ 919.7 GB   │ 129.7 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2020 │ 7 months, 16 days, 10 hours and 58 minutes │ 26.15 minutes  │ 1.2 TB     │ 93.9 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2021 │ 7 months, 21 days, 9 hours and 40 minutes  │ 39.93 minutes  │ 1.3 TB     │ 149.9 MB   │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2022 │ 17 years, 3 months, 0 days and 21 hours    │ 19.62 minutes  │ 35.8 TB    │ 77.5 MB    │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │          2023 │ 15 years, 3 months, 24 days and 1 hours    │ 17.57 minutes  │ 27.6 TB    │ 60.2 MB    │
+    ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
+    ╒════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤════════════════╕
+    │ title_path                                                                                 │ duration      │ time_created   │
+    ╞════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪════════════════╡
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 07/20 | Adam Cheng | 2009 #Chinesedrama │ 43.85 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=zntYD1yLrG8                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 08/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=zQnSfoWrh-4                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 06/20 | Adam Cheng | 2009 #Chinesedrama │ 43.60 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=Qiax1kFyGWU                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 04/20 | Adam Cheng | 2009 #Chinesedrama │ 43.45 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=NT9C3PRrlTA                                                │               │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼────────────────┤
+    │ [Eng Sub] TVB Drama | The King Of Snooker 桌球天王 02/20 | Adam Cheng | 2009 #Chinesedrama │ 43.63 minutes │ yesterday      │
+    │ https://www.youtube.com/watch?v=MjpCiTawlTE                                                │               │                │
+    ╘════════════════════════════════════════════════════════════════════════════════════════════╧═══════════════╧════════════════╛
+
     $ library history video.db deleted
     Deleted media:
     ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
     │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
     ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
     │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
     ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
@@ -1080,15 +1239,15 @@
 
 
 </details>
 
 <details><summary>Download media</summary>
 
     $ library download -h
-    usage: library download database [--prefix /mnt/d/] --video | --audio
+    usage: library download [--prefix /mnt/d/] [--safe] [--subs] [--auto-subs] [--small] DATABASE --video | --audio
 
     Download stuff in a random order.
 
         library download dl.db --prefix ~/output/path/root/
 
     Download stuff in a random order, limited to the specified playlist URLs.
 
@@ -1125,15 +1284,15 @@
 
 
 </details>
 
 <details><summary>Download Status (download-status)</summary>
 
     $ library download-status -h
-    usage: library download-status [database]
+    usage: library download-status DATABASE
 
     Print download queue groups
 
         library download-status video.db
         ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
@@ -1171,27 +1330,27 @@
 
 
 </details>
 
 <details><summary>Update local media (fsupdate)</summary>
 
     $ library fsupdate -h
-    usage: library fsupdate database
+    usage: library fsupdate DATABASE
 
     Update each path previously saved:
 
-        library fsupdate database
+        library fsupdate video.db
 
 
 </details>
 
 <details><summary>Update online media (tubeupdate)</summary>
 
     $ library tubeupdate -h
-    usage: library tubeupdate [--audio | --video] [-c CATEGORY] [database]
+    usage: library tubeupdate [--audio | --video] [-c CATEGORY] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
     Or limit to specific categories...
 
@@ -1210,27 +1369,27 @@
 
 
 </details>
 
 <details><summary>Update reddit media (redditupdate)</summary>
 
     $ library redditupdate -h
-    usage: library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] [database]
+    usage: library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 
 
 </details>
 
 <details><summary>Convert pushshift data to reddit.db format</summary>
 
     $ library pushshift -h
-    usage: library pushshift [database] < stdin
+    usage: library pushshift DATABASE < stdin
 
     Download data (about 600GB jsonl.zst; 6TB uncompressed)
 
         wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
 
     Load data from files via unzstd
 
@@ -1245,15 +1404,15 @@
 
 
 </details>
 
 <details><summary>List playlists</summary>
 
     $ library playlists -h
-    usage: library playlists [database] [--aggregate] [--fields] [--json] [--delete ...]
+    usage: library playlists DATABASE [--aggregate] [--fields] [--json] [--delete ...]
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
         │ ie_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
@@ -1282,32 +1441,33 @@
 
 
 </details>
 
 <details><summary>Blocklist a channel</summary>
 
     $ library block -h
-    usage: library block database [playlists ...]
+    usage: library block DATABASE URLS ...
 
     Blocklist specific URLs (eg. YouTube channels, etc). With YT URLs this will block
     videos from the playlist uploader
 
-        library block dl.db https://annoyingwebsite/etc/
-
-    Use with the all-deleted-playlists flag to delete any previously downloaded files from the playlist uploader
+        library block dl.db --match-column playlist_path 'https://youtube.com/playlist?list=PLVoczRgDnXDLWV1UJ_tO70VT_ON0tuEdm'
 
-        library block dl.db --all-deleted-playlists https://annoyingwebsite/etc/
+        library block dl.db https://annoyingwebsite/etc/
+        library block dl.db "%fastcompany.com%"
+        library block dl.db --match-column title "% bitcoin%"
+        library block dl.db --force --match-column uploader Zeducation
 
 
 </details>
 
 <details><summary>Show large folders (bigdirs)</summary>
 
     $ library bigdirs -h
-    usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
+    usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
 
     See what folders take up space
 
         library bigdirs video.db
         library bigdirs audio.db
         library bigdirs fs.db
 
@@ -1411,20 +1571,37 @@
 
 
 </details>
 
 <details><summary>Merge SQLITE databases (merge-dbs)</summary>
 
     $ library merge-dbs -h
-    usage: library merge-dbs DEST_DB SOURCE_DB ... [--upsert pk1[,pk2]]
+    usage: library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
+
+    Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
+    and there is an existing row with the same PK, the default action is to delete the existing row and insert the new row
+    replacing all existing fields.
+
+    Upsert mode will update matching PK rows such that if a source row has a NULL field and
+    the destination row has a value then the value will be preserved instead of changed to the source row's NULL value.
+
+    Ignore mode (--only-new-rows) will insert only rows which don't already exist in the destination db
+
+    Test first by using temp databases as the destination db.
+    Try out different modes / flags until you are satisfied with the behavior of the program
+
+        library merge-dbs --pk path (mktemp --suffix .db) tv.db movies.db
 
     Merge database data and tables
 
         library merge-dbs --upsert --pk path video.db tv.db movies.db
-        library merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
+        library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path audio-fts.db audio.db
+
+        library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
+        library merge-dbs --only-new-rows --pk playlist_path,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
 
 
 </details>
 
 <details><summary>Sort lines by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
```

### Comparing `xklb-1.29.8/pyproject.toml` & `xklb-1.30.2/pyproject.toml`

 * *Files identical despite different names*

