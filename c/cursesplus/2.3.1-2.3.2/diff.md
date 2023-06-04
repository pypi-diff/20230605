# Comparing `tmp/cursesplus-2.3.1.tar.gz` & `tmp/cursesplus-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.3.1.tar", last modified: Mon May 29 23:25:58 2023, max compression
+gzip compressed data, was "cursesplus-2.3.2.tar", last modified: Sun Jun  4 23:47:50 2023, max compression
```

## Comparing `cursesplus-2.3.1.tar` & `cursesplus-2.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.126382 cursesplus-2.3.1/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.1/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1491 2023-05-29 23:25:58.126382 cursesplus-2.3.1/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      888 2023-05-29 23:25:42.000000 cursesplus-2.3.1/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-29 23:25:17.000000 cursesplus-2.3.1/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-29 23:25:58.126382 cursesplus-2.3.1/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.116382 cursesplus-2.3.1/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      317 2023-05-29 23:14:15.000000 cursesplus-2.3.1/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.126382 cursesplus-2.3.1/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.1/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    15799 2023-05-29 23:22:30.000000 cursesplus-2.3.1/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.1/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.1/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 23:25:58.126382 cursesplus-2.3.1/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1491 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-29 23:25:58.000000 cursesplus-2.3.1/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.2/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1491 2023-06-04 23:47:50.647888 cursesplus-2.3.2/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      888 2023-05-29 23:25:42.000000 cursesplus-2.3.2/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-04 23:47:15.000000 cursesplus-2.3.2/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-04 23:47:50.647888 cursesplus-2.3.2/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      317 2023-05-29 23:14:15.000000 cursesplus-2.3.2/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.2/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    15833 2023-06-04 23:47:11.000000 cursesplus-2.3.2/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.2/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.2/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1491 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.3.1/LICENSE` & `cursesplus-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.1/PKG-INFO` & `cursesplus-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.1
+Version: 2.3.2
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cursesplus-2.3.1/README.md` & `cursesplus-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.1/pyproject.toml` & `cursesplus-2.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.3.1"
+version = "2.3.2"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.3.1/src/cursesplus/__init__.py` & `cursesplus-2.3.2/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.1/src/cursesplus/cp.py` & `cursesplus-2.3.2/src/cursesplus/cp.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     return x
 
 def cursesinput(stdscr,prompt: str,lines=1,maxlen=0) -> str:
     """
     Get input from the user. Set maxlen to 0 for no maximum
     """
     ERROR = ""
+    stdscr.erase()
     mx,my = os.get_terminal_size()
     extoffscr = lines > my-3
     if extoffscr:
         lnrectmaxy = my-2
     else:
         lnrectmaxy = lines+2
     text: list[list[str]] = [[] for _ in range(lines)]
@@ -219,15 +220,15 @@
                         stdscr.clear()
     
 
 def displayops(stdscr,options: list,title="Please choose an option") -> int:
     """Display an options menu provided by options list. ALso displays title. Returns integer value of selected item."""
     mx, my = os.get_terminal_size()
     selected = 0
-    
+    stdscr.clear()
     options = [l[0:mx-3] for l in options]
     maxlen = max([len(l) for l in options])
     stdscr.addstr(0,0,title[0:mx-1])
     offset = 0
     while True:
         stdscr.addstr(0,0,title[0:mx-1])
         mx, my = os.get_terminal_size()
```

### Comparing `cursesplus-2.3.1/src/cursesplus/filedialog.py` & `cursesplus-2.3.2/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.1/src/cursesplus/messagebox.py` & `cursesplus-2.3.2/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.1/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.3.2/src/cursesplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.1
+Version: 2.3.2
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

