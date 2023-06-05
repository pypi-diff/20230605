# Comparing `tmp/playwrightcapture-1.20.1.tar.gz` & `tmp/playwrightcapture-1.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.1.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.2.tar", max compression
```

## Comparing `playwrightcapture-1.20.1.tar` & `playwrightcapture-1.20.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.1/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.1/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.1/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    30154 2023-06-02 13:20:55.055317 playwrightcapture-1.20.1/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.1/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.20.1/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.1/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1734 2023-06-02 13:23:02.048025 playwrightcapture-1.20.1/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.20.1/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.2/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.2/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.2/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    30858 2023-06-05 12:58:56.111661 playwrightcapture-1.20.2/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.2/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.20.2/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.2/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1734 2023-06-05 13:05:35.154972 playwrightcapture-1.20.2/pyproject.toml
+-rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 playwrightcapture-1.20.2/PKG-INFO
```

### Comparing `playwrightcapture-1.20.1/LICENSE` & `playwrightcapture-1.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.1/README.md` & `playwrightcapture-1.20.2/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.1/playwrightcapture/capture.py` & `playwrightcapture-1.20.2/playwrightcapture/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import random
 import re
 import time
 
 from tempfile import NamedTemporaryFile
 from typing import Optional, Dict, List, Union, Any, TypedDict, Literal
+from urllib.parse import urlparse
 
 import dateparser
 
 from playwright.async_api import async_playwright, ProxySettings, Frame, ViewportSize, Cookie, Error, Page
 from playwright.async_api import TimeoutError as PlaywrightTimeoutError
 
 from playwright._impl._api_structures import SetCookieParam
@@ -441,14 +442,18 @@
         to_return: CaptureResponse = {}
         try:
             if page:
                 capturing_sub = True
             else:
                 capturing_sub = False
                 page = await self.context.new_page()
+
+            # Parse the URL. If there is a fragment, we need to scroll to it manually
+            parsed_url = urlparse(url, allow_fragments=True)
+
             try:
                 # NOTE 2022-12-02: allow 15s less than the general timeout to get a DOM
                 await page.goto(url, wait_until='domcontentloaded', timeout=self.general_timeout - 15000, referer=referer if referer else '')
             except Error as initial_error:
                 self._update_exceptions(initial_error)
                 if self._exception_is_network_error(initial_error):
                     raise initial_error
@@ -497,22 +502,30 @@
                     except Exception as e:
                         self.logger.exception(f'General error with captcha solving on {url}: {e}')
                 # ======
 
                 # check if we have anything on the page. If we don't, the page is not working properly.
                 if await self._failsafe_get_content(page):
                     # move mouse
-                    await page.mouse.move(x=500, y=400)
+                    await page.mouse.move(x=random.uniform(300, 800), y=random.uniform(200, 500))
                     await self._safe_wait(page)
                     self.logger.debug('Moved mouse')
 
+                    if parsed_url.fragment:
+                        # We got a fragment, go to it
+                        try:
+                            await page.locator(f'id={parsed_url.fragment}').scroll_into_view_if_needed()
+                            await self._safe_wait(page)
+                        except Error as e:
+                            self.logger.warning(f'Unable to go to fragment "{parsed_url.fragment}": {e}')
+
                     # scroll
                     try:
                         # NOTE using page.mouse.wheel causes the instrumentation to fail, sometimes
-                        await page.mouse.wheel(delta_y=2000, delta_x=0)
+                        await page.mouse.wheel(delta_y=random.uniform(1500, 3000), delta_x=0)
                         await self._safe_wait(page)
                     except Error as e:
                         self.logger.debug(f'Unable to scroll: {e}')
                     await page.keyboard.press('PageUp')
                     self.logger.debug('Scrolled')
 
                 await self._safe_wait(page)
@@ -606,33 +619,39 @@
             if ' at ' in name:
                 name, _ = name.split(' at ', maxsplit=1)
             elif '; ' in name:
                 name, _ = name.split('; ', maxsplit=1)
             exception.name = name.strip()
 
     def _exception_is_network_error(self, exception: Error) -> bool:
-        if exception.name in ['NS_ERROR_UNKNOWN_HOST',
-                              'NS_ERROR_CONNECTION_REFUSED',
-                              'NS_ERROR_NET_RESET',
-                              'NS_ERROR_UNEXPECTED',
-                              'NS_ERROR_NET_TIMEOUT',
-                              'NS_ERROR_REDIRECT_LOOP',
-                              'NS_ERROR_NET_INTERRUPT',
-                              'NS_ERROR_UNKNOWN_PROTOCOL',
-                              'NS_ERROR_ABORT',
-                              'net::ERR_EMPTY_RESPONSE',
-                              'net::ERR_CONNECTION_REFUSED',
-                              'net::ERR_CONNECTION_RESET',
-                              'net::ERR_ADDRESS_UNREACHABLE',
-                              'net::ERR_NAME_NOT_RESOLVED',
-                              'net::ERR_SSL_PROTOCOL_ERROR',
-                              'net::ERR_TOO_MANY_REDIRECTS',
-                              'net::ERR_TIMED_OUT',
-                              'net::ERR_ABORTED',
-                              ]:
+        if exception.name in [
+                'NS_ERROR_ABORT',
+                'NS_ERROR_CONNECTION_REFUSED',
+                'NS_ERROR_NET_INTERRUPT',
+                'NS_ERROR_NET_RESET',
+                'NS_ERROR_NET_TIMEOUT',
+                'NS_ERROR_REDIRECT_LOOP',
+                'NS_ERROR_UNEXPECTED',
+                'NS_ERROR_UNKNOWN_HOST',
+                'NS_ERROR_UNKNOWN_PROTOCOL',
+                'net::ERR_ABORTED',
+                'net::ERR_ADDRESS_UNREACHABLE',
+                'net::ERR_CONNECTION_CLOSED',
+                'net::ERR_CONNECTION_REFUSED',
+                'net::ERR_CONNECTION_RESET',
+                'net::ERR_EMPTY_RESPONSE',
+                'net::ERR_HTTP2_PROTOCOL_ERROR',
+                'net::ERR_NAME_NOT_RESOLVED',
+                'net::ERR_SOCKS_CONNECTION_FAILED',
+                'net::ERR_SSL_UNRECOGNIZED_NAME_ALERT',
+                'net::ERR_SSL_VERSION_OR_CIPHER_MISMATCH',
+                'net::ERR_SSL_PROTOCOL_ERROR',
+                'net::ERR_TIMED_OUT',
+                'net::ERR_TOO_MANY_REDIRECTS',
+        ]:
             return True
         return False
 
     async def __aexit__(self, exc_type: Any, exc: Any, tb: Any) -> None:
         if hasattr(self, '_temp_harfile'):
             os.unlink(self._temp_harfile.name)
```

### Comparing `playwrightcapture-1.20.1/playwrightcapture/helpers.py` & `playwrightcapture-1.20.2/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.1/pyproject.toml` & `playwrightcapture-1.20.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.1"
+version = "1.20.2"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.20.1/PKG-INFO` & `playwrightcapture-1.20.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.1
+Version: 1.20.2
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -12,15 +12,14 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.0,<4.0.0) ; extra == "recaptcha"
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
```

