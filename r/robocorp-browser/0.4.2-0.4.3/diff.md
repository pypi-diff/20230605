# Comparing `tmp/robocorp_browser-0.4.2.tar.gz` & `tmp/robocorp_browser-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.4.2.tar", max compression
+gzip compressed data, was "robocorp_browser-0.4.3.tar", max compression
```

## Comparing `robocorp_browser-0.4.2.tar` & `robocorp_browser-0.4.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       94 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/README.md
--rw-r--r--   0        0        0      640 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7225 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0     6898 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0        0 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 robocorp_browser-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-06-05 12:23:19.605558 robocorp_browser-0.4.3/README.md
+-rw-r--r--   0        0        0      638 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     7819 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0     6898 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:23:19.609558 robocorp_browser-0.4.3/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 robocorp_browser-0.4.3/PKG-INFO
```

### Comparing `robocorp_browser-0.4.2/pyproject.toml` & `robocorp_browser-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "0.4.2"
+version = "0.4.3"
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
-robocorp-tasks = "^0.3.0"
+robocorp-tasks = "^0.3"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_browser-0.4.2/src/robocorp/browser/__init__.py` & `robocorp_browser-0.4.3/src/robocorp/browser/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,19 @@
-from typing import Literal, Optional
+from typing import Literal, Optional, Union
 
-from playwright.sync_api import Browser, BrowserContext, Page, Playwright
+from playwright.sync_api import (
+    Browser,
+    BrowserContext,
+    ElementHandle,
+    Locator,
+    Page,
+    Playwright,
+)
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
 
@@ -121,16 +128,17 @@
     """
     from . import _browser_context
 
     return _browser_context.context()
 
 
 def open_browser(
-    browser_engine: Literal["firefox", "chrome"] = "chrome",
+    browser_engine: Optional[Literal["chrome", "firefox"]] = None,
     headless: Optional[bool] = None,
+    **kwargs,
 ) -> Browser:
     """Shortcut to configure and launch a browser instance (using Playwright).
 
     Note that if the browser was already previously launched the previous
     instance will be returned and any configuration passed will be ignored.
 
     Args:
@@ -145,84 +153,98 @@
         The arguments related to browser initialization will only be used
         if this is the first call, on subsequent calls the same browser instance
         will be used and the current page will open the given url.
 
     Returns:
         The browser instance.
     """
-    configure(browser_engine=browser_engine, headless=headless)
+    if browser_engine is not None:
+        kwargs["browser_engine"] = browser_engine
+    if headless is not None:
+        kwargs["headless"] = headless
+    if kwargs:
+        configure(**kwargs)
     return browser()
 
 
 def open_url(
     url: str,
-    browser_engine: Literal["firefox", "chrome"] = "chrome",
+    browser_engine: Optional[Literal["chrome", "firefox"]] = None,
     headless: Optional[bool] = None,
+    **kwargs,
 ) -> Page:
     """
     Changes the url of the current page (creating a page if needed).
 
     Args:
         url: Navigates to the provided URL.
 
         browser: Specifies which browser to use. Supported browsers are:
             ``chrome`` and ``firefox``.
 
         headless: If set to False the browser UI will be shown. If set to True
             the browser UI will be kept hidden. If unset or set to None it'll
             show the browser UI only if a debugger is detected.
 
+        kwargs: Other keyword arguments to be passed to the
+            `configure` function (besides `browser` and `headless`).
+
     Note:
         The arguments related to browser initialization will only be used
         if this is the first call, on subsequent calls the same browser instance
         will be used and the current page will open the given url.
 
     Returns:
         The page instance managed by the robocorp.tasks framework
         (it will be automatically closed when the task finishes).
     """
-    configure(browser_engine=browser_engine, headless=headless)
+    if browser_engine is not None:
+        kwargs["browser_engine"] = browser_engine
+    if headless is not None:
+        kwargs["headless"] = headless
+    if kwargs:
+        configure(**kwargs)
     p = page()
     p.goto(url)
     return p
 
 
 def screenshot(
-    page: Optional[Page] = None,
+    element: Optional[Union[Page, ElementHandle, Locator]] = None,
     timeout: int = 5000,
     image_type: Literal["png", "jpeg"] = "png",
     log_level: Literal["INFO", "WARN", "ERROR"] = "INFO",
 ) -> bytes:
     """
-    Takes a screenshot of the given page and saves it to the log. If no page
-    is provided the current page is saved.
+    Takes a screenshot of the given page/element/locator and saves it to the
+    log. If no element is provided the screenshot will target the current page.
 
-    Note: the page.screenshot can be used if the screenshot is not expected
+    Note: the element.screenshot can be used if the screenshot is not expected
     to be added to the log.
 
     Args:
-        page: The page which should have its screenshot taken. If not given
-        the managed page instance will be used.
+        element: The page/element/locator which should have its screenshot taken. If not
+        given the managed page instance will be used.
 
     Returns:
         The bytes from the screenshot.
     """
     import base64
 
     from robocorp import log
 
-    if page is None:
+    if element is None:
         from . import _browser_context
 
-        page = _browser_context.page()
+        element = _browser_context.page()
 
     with log.suppress():
         # Suppress log because we don't want the bytes to appear at
         # the screenshot and then as the final html.
-        in_bytes = page.screenshot(timeout=timeout, type=image_type)
+        in_bytes = element.screenshot(timeout=timeout, type=image_type)
         in_base64 = base64.b64encode(in_bytes).decode("ascii")
 
     log.html(
         f'<img src="data:image/{image_type};base64,{in_base64}"/>', level=log_level
     )
 
     return in_bytes
```

### Comparing `robocorp_browser-0.4.2/src/robocorp/browser/_browser_context.py` & `robocorp_browser-0.4.3/src/robocorp/browser/_browser_context.py`

 * *Files identical despite different names*

