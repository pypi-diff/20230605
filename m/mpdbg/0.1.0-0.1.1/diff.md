# Comparing `tmp/mpdbg-0.1.0.tar.gz` & `tmp/mpdbg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpdbg-0.1.0.tar", max compression
+gzip compressed data, was "mpdbg-0.1.1.tar", max compression
```

## Comparing `mpdbg-0.1.0.tar` & `mpdbg-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2170 2023-06-04 11:01:23.739006 mpdbg-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-26 13:12:10.539829 mpdbg-0.1.0/mpdbg/__init__.py
--rw-r--r--   0        0        0       62 2023-05-26 13:44:32.156382 mpdbg-0.1.0/mpdbg/__main__.py
--rw-r--r--   0        0        0     1662 2023-05-30 10:49:43.058360 mpdbg-0.1.0/mpdbg/image.py
--rw-r--r--   0        0        0     4960 2023-06-03 09:09:18.673818 mpdbg-0.1.0/mpdbg/main.py
--rw-r--r--   0        0        0     1435 2023-06-02 01:31:26.251691 mpdbg-0.1.0/mpdbg/mpd_utils.py
--rw-r--r--   0        0        0     1047 2023-05-29 13:15:42.437509 mpdbg-0.1.0/mpdbg/wallpaper.py
--rw-r--r--   0        0        0      573 2023-06-04 13:18:33.435475 mpdbg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 mpdbg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-06-05 01:11:22.161764 mpdbg-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 13:12:10.539829 mpdbg-0.1.1/mpdbg/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-26 13:44:32.156382 mpdbg-0.1.1/mpdbg/__main__.py
+-rw-r--r--   0        0        0     1662 2023-05-30 10:49:43.058360 mpdbg-0.1.1/mpdbg/image.py
+-rw-r--r--   0        0        0     4960 2023-06-03 09:09:18.673818 mpdbg-0.1.1/mpdbg/main.py
+-rw-r--r--   0        0        0     1435 2023-06-02 01:31:26.251691 mpdbg-0.1.1/mpdbg/mpd_utils.py
+-rw-r--r--   0        0        0     1047 2023-05-29 13:15:42.437509 mpdbg-0.1.1/mpdbg/wallpaper.py
+-rw-r--r--   0        0        0      573 2023-06-05 01:24:50.915096 mpdbg-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3540 1970-01-01 00:00:00.000000 mpdbg-0.1.1/PKG-INFO
```

### Comparing `mpdbg-0.1.0/README.md` & `mpdbg-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 *mpdbg* is a program that listens to a [Music Player Daemon](https://www.musicpd.org) and changes the desktop wallpaper image depending on the current song. If the song has a cover art image, it will be drawn on top of wallpaper. A couple of effects can be applied to original wallpaper in this case, if user chooses so. If the current song doesn't have a cover art image, the original wallpaper wil be displayed.
 
 Check out [mpdbg's homepage](https://git.dragonwit.dev/dragonwit/mpdbg-py) for downloads and such.
 
 ## Installation
 
-*mpdbg* is not in the [Python Package Index (PyPI)](https://pypi.org) and I have no plans currently to put it there. You can install the program by downloading *mpdbg-x.y.z-py3-none-any.whl* from project's releases page and running:
+Install from [PyPI](https://pypi.org):
+
+    pip install --user mpdbg
+
+You also can install the program by downloading *mpdbg-x.y.z-py3-none-any.whl* from project's releases page and running:
 
     pip install --user ./mpdbg-x.y.z-py3-none-any.whl
 
-This would install *mpdbg* for current user and an excutable script to *~/.local/bin/mpdbg*.
+Either of these commands would install *mpdbg* for current user and an executable script to *~/.local/bin/mpdbg*.
 
 ## Building
 
 Install [poetry](https://python-poetry.org) and execute following in the project directory:
 
     poetry build
 
@@ -34,13 +38,26 @@
                                       file.  [required]
       -e, --effect [blur|grayscale]   Effect to apply to wallpaper when displaying
                                       an album cover (multiple can be specified)
       -l, --log-level [debug|info|warning|error|critical]
                                       Set log level.
       --help                          Show this message and exit.
 
+To set MPD socket location or address and port, use environment variables *MPD_HOST* and *MPD_PORT*. If they're not set, address *localhost* and port *6600* will be used. You can set them in *~/.profile*, for example. Here's couple of examples:
+
+    # connecting to a tcp port
+    export MPD_HOST=localhost
+    export MPD_PORT=6600
+    
+    # connecting to a unix socket
+    export MPD_HOST=/path/to/mpd.socket
+    
+    # using a password
+    export MPD_HOST=MYPASSWORD@localhost
+    export MPD_PORT=6600
+
 Example for using *mpdbg* with [swww](https://github.com/Horus645/swww) wallpaper setter:
 
     mpdbg run -w ~/wallpaper.png -s 'swww img --transition-type center $image' -e blur
 
 The command above would use *~/wallpaper.png* as wallpaper and *swww* as wallpaper setter. The wallpaper would also be blurred when displaying a cover art image on top of it.
```

### Comparing `mpdbg-0.1.0/mpdbg/image.py` & `mpdbg-0.1.1/mpdbg/image.py`

 * *Files identical despite different names*

### Comparing `mpdbg-0.1.0/mpdbg/main.py` & `mpdbg-0.1.1/mpdbg/main.py`

 * *Files identical despite different names*

### Comparing `mpdbg-0.1.0/mpdbg/mpd_utils.py` & `mpdbg-0.1.1/mpdbg/mpd_utils.py`

 * *Files identical despite different names*

### Comparing `mpdbg-0.1.0/mpdbg/wallpaper.py` & `mpdbg-0.1.1/mpdbg/wallpaper.py`

 * *Files identical despite different names*

### Comparing `mpdbg-0.1.0/pyproject.toml` & `mpdbg-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpdbg"
-version = "0.1.0"
+version = "0.1.1"
 description = "Display MPD's current song's cover art on top of wallpaper"
 authors = ["dragonwit <dragonwit@dragonwit.dev>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://git.dragonwit.dev/dragonwit/mpdbg-py"
 repository = "https://git.dragonwit.dev/dragonwit/mpdbg-py"
```

### Comparing `mpdbg-0.1.0/PKG-INFO` & `mpdbg-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpdbg
-Version: 0.1.0
+Version: 0.1.1
 Summary: Display MPD's current song's cover art on top of wallpaper
 Home-page: https://git.dragonwit.dev/dragonwit/mpdbg-py
 License: GPL-3.0-only
 Author: dragonwit
 Author-email: dragonwit@dragonwit.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -26,19 +26,23 @@
 
 *mpdbg* is a program that listens to a [Music Player Daemon](https://www.musicpd.org) and changes the desktop wallpaper image depending on the current song. If the song has a cover art image, it will be drawn on top of wallpaper. A couple of effects can be applied to original wallpaper in this case, if user chooses so. If the current song doesn't have a cover art image, the original wallpaper wil be displayed.
 
 Check out [mpdbg's homepage](https://git.dragonwit.dev/dragonwit/mpdbg-py) for downloads and such.
 
 ## Installation
 
-*mpdbg* is not in the [Python Package Index (PyPI)](https://pypi.org) and I have no plans currently to put it there. You can install the program by downloading *mpdbg-x.y.z-py3-none-any.whl* from project's releases page and running:
+Install from [PyPI](https://pypi.org):
+
+    pip install --user mpdbg
+
+You also can install the program by downloading *mpdbg-x.y.z-py3-none-any.whl* from project's releases page and running:
 
     pip install --user ./mpdbg-x.y.z-py3-none-any.whl
 
-This would install *mpdbg* for current user and an excutable script to *~/.local/bin/mpdbg*.
+Either of these commands would install *mpdbg* for current user and an executable script to *~/.local/bin/mpdbg*.
 
 ## Building
 
 Install [poetry](https://python-poetry.org) and execute following in the project directory:
 
     poetry build
 
@@ -56,14 +60,27 @@
                                       file.  [required]
       -e, --effect [blur|grayscale]   Effect to apply to wallpaper when displaying
                                       an album cover (multiple can be specified)
       -l, --log-level [debug|info|warning|error|critical]
                                       Set log level.
       --help                          Show this message and exit.
 
+To set MPD socket location or address and port, use environment variables *MPD_HOST* and *MPD_PORT*. If they're not set, address *localhost* and port *6600* will be used. You can set them in *~/.profile*, for example. Here's couple of examples:
+
+    # connecting to a tcp port
+    export MPD_HOST=localhost
+    export MPD_PORT=6600
+    
+    # connecting to a unix socket
+    export MPD_HOST=/path/to/mpd.socket
+    
+    # using a password
+    export MPD_HOST=MYPASSWORD@localhost
+    export MPD_PORT=6600
+
 Example for using *mpdbg* with [swww](https://github.com/Horus645/swww) wallpaper setter:
 
     mpdbg run -w ~/wallpaper.png -s 'swww img --transition-type center $image' -e blur
 
 The command above would use *~/wallpaper.png* as wallpaper and *swww* as wallpaper setter. The wallpaper would also be blurred when displaying a cover art image on top of it.
```

