# Comparing `tmp/robocorp_browser-0.4.3.tar.gz` & `tmp/robocorp_browser-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.4.3.tar", max compression
+gzip compressed data, was "robocorp_browser-0.4.4.tar", max compression
```

## Comparing `robocorp_browser-0.4.3.tar` & `robocorp_browser-0.4.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       94 2023-06-05 12:23:19.605558 robocorp_browser-0.4.3/README.md
--rw-r--r--   0        0        0      638 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     7819 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0     6898 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0        0 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 robocorp_browser-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/README.md
+-rw-r--r--   0        0        0      638 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     7819 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0     6898 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 robocorp_browser-0.4.4/PKG-INFO
```

### Comparing `robocorp_browser-0.4.3/pyproject.toml` & `robocorp_browser-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "0.4.3"
+version = "0.4.4"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 playwright = "^1.32.1"
-robocorp-tasks = "^0.3"
+robocorp-tasks = "^0.4"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_browser-0.4.3/src/robocorp/browser/__init__.py` & `robocorp_browser-0.4.4/src/robocorp/browser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     BrowserContext,
     ElementHandle,
     Locator,
     Page,
     Playwright,
 )
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
```

### Comparing `robocorp_browser-0.4.3/src/robocorp/browser/_browser_context.py` & `robocorp_browser-0.4.4/src/robocorp/browser/_browser_context.py`

 * *Files identical despite different names*

