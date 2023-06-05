# Comparing `tmp/caqui-1.0.7.tar.gz` & `tmp/caqui-1.0.8.tar.gz`

## Comparing `caqui-1.0.7.tar` & `caqui-1.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 caqui-1.0.7/sample.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.0.7/test-requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.7/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/__init__.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/exceptions.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/helper.py
--rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/constants.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/fake_responses.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/test_sniffer.py
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/feature/test_sync_and_async.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/html/playground.html
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/__initi__.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/test_helper.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.0.7/utils/coverage.sh
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.7/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.7/LICENSE
--rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.7/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 caqui-1.0.8/sample.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.0.8/test-requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/__init__.py
+-rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/exceptions.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/helper.py
+-rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/constants.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/fake_responses.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/test_sniffer.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/html/playground.html
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.0.8/utils/coverage.sh
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.8/LICENSE
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.8/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.0.8/PKG-INFO
```

### Comparing `caqui-1.0.7/CODE_OF_CONDUCT.md` & `caqui-1.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/sample.py` & `caqui-1.0.8/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,56 @@
 from caqui import synchronous, asynchronous
 from os import getcwd
 from tests.constants import PAGE_URL
 
 BASE_DIR = getcwd()
 
 MAX_CONCURRENCY = 5  # number of webdriver instances running
-sem = asyncio.Semaphore(MAX_CONCURRENCY)
+all_anchors = []
+semaphore = asyncio.Semaphore(MAX_CONCURRENCY)
 
 
 async def get_all_links():
-    async with sem:
+    async with semaphore:
         driver_url = "http://127.0.0.1:9999"
         capabilities = {
             "desiredCapabilities": {
-                "browserName": "firefox",
+                "browserName": "chrome",
                 "marionette": True,
                 "acceptInsecureCerts": True,
+                "pageLoadStrategy": "normal",
+                "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
             }
         }
 
         session = await asynchronous.get_session(driver_url, capabilities)
         await asynchronous.go_to_page(
             driver_url,
             session,
             PAGE_URL,
         )
 
+        all_anchors = []
         for i in range(4):
             i += 1
             locator_value = f"//a[@id='a{i}']"
             locator_type = "xpath"
             anchors = []
 
             anchors = await asynchronous.find_elements(
                 driver_url, session, locator_type, locator_value
             )
-            print(f"Found {len(anchors)} links")
+            all_anchors.extend(anchors)
 
-        for anchor in anchors:
+        texts = []
+        for anchor in all_anchors:
             text = await asynchronous.get_property(driver_url, session, anchor, "href")
+            texts.append(text)
+
+        for text in texts:
             print(f"Link found '{text}'")
 
         synchronous.close_session(driver_url, session)
 
 
 # Reference: https://stackoverflow.com/questions/48483348/how-to-limit-concurrency-with-python-asyncio
 async def main():
@@ -58,8 +66,9 @@
     loop = asyncio.get_event_loop()
     try:
         loop.run_until_complete(main())
     finally:
         loop.run_until_complete(loop.shutdown_asyncgens())
         loop.close()
         end = time.time()
+        print(f"Found 40 links")  # 10 websites with 4 links each
         print(f"Time: {end-start:.2f} sec")
```

### Comparing `caqui-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-1.0.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-1.0.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/.github/workflows/python-app.yml` & `caqui-1.0.8/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/.github/workflows/python-publish.yml` & `caqui-1.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/caqui/__init__.py` & `caqui-1.0.8/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/caqui/asynchronous.py` & `caqui-1.0.8/caqui/asynchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 async def __delete(url):
     try:
         async with aiohttp.ClientSession() as session:
             async with session.delete(url, headers=HEADERS) as resp:
                 response = await resp.json()
                 return response
     except Exception as error:
-        raise WebDriverError("'POST' request failed.") from error
+        raise WebDriverError("'DELETE' request failed.") from error
 
 
 async def __post(url, payload):
     try:
         async with aiohttp.ClientSession() as session:
             async with session.post(url, data=payload, headers=HEADERS) as resp:
                 response = await resp.json()
@@ -31,14 +31,34 @@
             async with session.get(url, headers=HEADERS) as resp:
                 response = await resp.json()
                 return response
     except Exception as error:
         raise WebDriverError("'GET' request failed.") from error
 
 
+async def close_window(driver_url, session):
+    """Close active window"""
+    try:
+        url = f"{driver_url}/session/{session}/window"
+        response = await __delete(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to close active window.") from error
+
+
+async def get_window(driver_url, session):
+    """Get window handle"""
+    try:
+        url = f"{driver_url}/session/{session}/window"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get window.") from error
+
+
 async def go_back(driver_url, session):
     """
     This command causes the browser to traverse one step backward in the joint session history of the
     current browse. This is equivalent to pressing the back button in the browser.
     """
     try:
         url = f"{driver_url}/session/{session}/back"
@@ -118,41 +138,45 @@
     try:
         url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
+
 async def get_attribute(driver_url, session, element, attribute):
     """Get the given HTML attribute of an element, for example, 'aria-valuenow'"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/attribute/{attribute}"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
+
 async def get_text(driver_url, session, element):
     """Get the text of an element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/text"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get text from element.") from error
 
+
 async def get_cookies(driver_url, session):
     """Get the page cookies"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get page cookies.") from error
 
+
 async def close_session(driver_url, session):
     """Close an opened session and close the browser"""
     try:
         url = f"{driver_url}/session/{session}"
         await __delete(url)
         return True
     except Exception as error:
```

### Comparing `caqui-1.0.7/caqui/synchronous.py` & `caqui-1.0.8/caqui/synchronous.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,32 @@
 def __delete(url):
     try:
         return requests.request("DELETE", url, headers={}, data={}).json()
     except Exception as error:
         raise WebDriverError("'DELETE' request failed.") from error
 
 
+def close_window(driver_url, session):
+    """Close active window"""
+    try:
+        url = f"{driver_url}/session/{session}/window"
+        return __delete(url).get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to close active window.") from error
+
+
+def get_window(driver_url, session):
+    """Get window handle"""
+    try:
+        url = f"{driver_url}/session/{session}/window"
+        return __get(url).get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to get window.") from error
+
+
 def go_back(driver_url, session):
     """
     This command causes the browser to traverse one step backward in the joint session history of the
     current browse. This is equivalent to pressing the back button in the browser.
     """
     try:
         url = f"{driver_url}/session/{session}/back"
@@ -114,32 +132,35 @@
     try:
         url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
         response = __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
+
 def get_attribute(driver_url, session, element, attribute):
     """Get the given HTML attribute of an element, for example, 'aria-valuenow'"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/attribute/{attribute}"
         response = __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
+
 def get_cookies(driver_url, session):
     """Get the page cookies"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         response = __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get page cookies.") from error
 
+
 def go_to_page(driver_url, session, page_url):
     """Navigate to 'page_url'"""
     try:
         url = f"{driver_url}/session/{session}/url"
         payload = json.dumps({"url": page_url})
         __post(url, payload)
         return True
```

### Comparing `caqui-1.0.7/tests/fake_responses.py` & `caqui-1.0.8/tests/fake_responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,25 @@
 
 FIND_ELEMENT = DEFAULT
 SEND_KEYS = DEFAULT
 CLICK = DEFAULT
 CLOSE_SESSION = DEFAULT
 GO_TO_PAGE = DEFAULT
 
+CLOSE_WINDOW = dict_to_json(
+    {"sessionId": "48399161591a0bc1dffaa2ff2d65aa0f", "status": 0, "value": []}
+)
+GET_WINDOW = dict_to_json(
+    {
+        "sessionId": "ce68162d420e9cb2b1617c2d1a800f85",
+        "status": 0,
+        "value": "845623CAE8115F2B60C9AE8596F13D94",
+    }
+)
+
 GET_URL = dict_to_json(
     {
         "sessionId": "af67b8ef665d30a687f37365d229fb53",
         "status": 0,
         "value": "file:///html/playground.html",
     }
 )
```

### Comparing `caqui-1.0.7/tests/test_sniffer.py` & `caqui-1.0.8/tests/test_sniffer.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/tests/feature/test_sync_and_async.py` & `caqui-1.0.8/tests/feature/test_sync_and_async.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,29 +4,77 @@
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
     capabilities = {
         "desiredCapabilities": {
+            "name": "webdriver",
             "browserName": "firefox",
             "marionette": True,
             "acceptInsecureCerts": True,
+            "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
         }
     }
     session = synchronous.get_session(driver_url, capabilities)
     synchronous.go_to_page(
         driver_url,
         session,
         PAGE_URL,
     )
     yield driver_url, session
     synchronous.close_session(driver_url, session)
 
 
+def test_close_window_sync(__setup):
+    driver_url, session = __setup
+    assert isinstance(synchronous.close_window(driver_url, session), list)
+
+
+@mark.asyncio
+async def test_close_window_async(__setup):
+    driver_url, session = __setup
+
+    response = await asynchronous.close_window(driver_url, session)
+    assert isinstance(response, list)
+
+
+@mark.asyncio
+async def test_get_window(__setup):
+    driver_url, session = __setup
+
+    assert synchronous.get_window(driver_url, session) is not None
+    assert await asynchronous.get_window(driver_url, session) is not None
+
+
+@mark.asyncio
+async def test_get_attribute(__setup):
+    driver_url, session = __setup
+    attribute = "href"
+    element = synchronous.find_element(driver_url, session, "xpath", "//a[@id='a1']")
+
+    assert (
+        synchronous.get_attribute(driver_url, session, element, attribute)
+        == "http://any1.com/"
+    )
+    assert (
+        await asynchronous.get_attribute(driver_url, session, element, attribute)
+        == "http://any1.com/"
+    )
+
+
+@mark.asyncio
+async def test_get_cookies(__setup):
+    driver_url, session = __setup
+
+    assert isinstance(synchronous.get_cookies(driver_url, session), list)
+    cookies = await asynchronous.get_cookies(driver_url, session)
+    assert isinstance(cookies, list)
+
+
 @mark.asyncio
 async def test_go_back(__setup):
     driver_url, session = __setup
 
     assert synchronous.go_back(driver_url, session) is True
     assert await asynchronous.go_back(driver_url, session) is True
```

### Comparing `caqui-1.0.7/tests/html/playground.html` & `caqui-1.0.8/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/tests/integration/test_async_scenarios.py` & `caqui-1.0.8/tests/integration/test_async_scenarios.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 def __setup():
     driver_url = "http://127.0.0.1:9999"
     capabilities = {
         "desiredCapabilities": {
             "browserName": "firefox",
             "marionette": True,
             "acceptInsecureCerts": True,
+            "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
         }
     }
     session = synchronous.get_session(driver_url, capabilities)
     synchronous.go_to_page(
         driver_url,
         session,
         PAGE_URL,
```

### Comparing `caqui-1.0.7/tests/integration/test_sync_scenarios.py` & `caqui-1.0.8/tests/integration/test_sync_scenarios.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 def __setup():
     driver_url = "http://127.0.0.1:9999"
     capabilities = {
         "desiredCapabilities": {
             "browserName": "firefox",
             "marionette": True,
             "acceptInsecureCerts": True,
+            "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
         }
     }
     session = get_session(driver_url, capabilities)
     go_to_page(
         driver_url,
         session,
         PAGE_URL,
```

### Comparing `caqui-1.0.7/tests/unit/test_async_unit.py` & `caqui-1.0.8/tests/unit/test_async_unit.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,36 @@
 
 
 async def mock_post(*args):
     pass
 
 
 @mark.asyncio
+async def test_close_window():
+    expected = []
+
+    async def mock_post(*args):
+        return fake_responses.CLOSE_WINDOW
+
+    with patch("caqui.asynchronous.__delete", mock_post):
+        assert await asynchronous.close_window("", "") == expected
+
+
+@mark.asyncio
+async def test_get_window():
+    expected = "845623CAE8115F2B60C9AE8596F13D94"
+
+    async def mock_post(*args):
+        return fake_responses.GET_WINDOW
+
+    with patch("caqui.asynchronous.__get", mock_post):
+        assert await asynchronous.get_window("", "") == expected
+
+
+@mark.asyncio
 async def test_go_back():
     with patch("caqui.asynchronous.__post", mock_post):
         assert await asynchronous.go_back("", "") is True
 
 
 @mark.asyncio
 async def test_get_property():
@@ -23,24 +45,26 @@
 
     async def mock_post(*args):
         return fake_responses.GET_PROPERTY_VALUE
 
     with patch("caqui.asynchronous.__get", mock_post):
         assert await asynchronous.get_property("", "", "", "") == expected
 
+
 @mark.asyncio
 async def test_get_attribute():
     expected = "any_value"
 
     async def mock_post(*args):
         return fake_responses.GET_ATTRIBUTE_VALUE
 
     with patch("caqui.asynchronous.__get", mock_post):
         assert await asynchronous.get_attribute("", "", "", "") == expected
 
+
 @mark.asyncio
 async def test_get_url():
     expected = "playground.html"
 
     async def mock_post(*args):
         return fake_responses.GET_URL
 
@@ -77,24 +101,26 @@
 
     async def mock_post(*args):
         return fake_responses.GET_TITLE
 
     with patch("caqui.asynchronous.__get", mock_post):
         assert await asynchronous.get_title("", "") == expected
 
+
 @mark.asyncio
 async def test_get_cookies():
     expected = []
 
     async def mock_post(*args):
         return fake_responses.GET_COOKIES
 
     with patch("caqui.asynchronous.__get", mock_post):
         assert await asynchronous.get_cookies("", "") == expected
 
+
 @mark.asyncio
 async def test_get_text():
     expected = "any"
 
     async def mock_post(*args):
         return fake_responses.GET_TEXT
```

### Comparing `caqui-1.0.7/tests/unit/test_helper.py` & `caqui-1.0.8/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/tests/unit/test_sync_unit.py` & `caqui-1.0.8/tests/unit/test_sync_unit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 from unittest.mock import patch
 from caqui import synchronous
 from tests import fake_responses
 
 
+@patch("requests.request", return_value=fake_responses.CLOSE_WINDOW)
+def test_close_window(*args):
+    expected = []
+
+    assert synchronous.close_window("", "") == expected
+
+
+@patch("requests.request", return_value=fake_responses.GET_WINDOW)
+def test_get_window(*args):
+    expected = "845623CAE8115F2B60C9AE8596F13D94"
+
+    assert expected in synchronous.get_window("", "")
+
+
 @patch("requests.request", return_value=fake_responses.GET_URL)
 def test_get_url(*args):
     expected = "playground.html"
 
     assert expected in synchronous.get_url("", "")
 
 
@@ -24,20 +38,22 @@
 
 @patch("requests.request", return_value=fake_responses.GET_TITLE)
 def test_get_title(*args):
     expected = "Sample page"
 
     assert synchronous.get_title("", "") == expected
 
+
 @patch("requests.request", return_value=fake_responses.GET_COOKIES)
 def test_get_cookies(*args):
     expected = []
 
     assert synchronous.get_cookies("", "") == expected
 
+
 @patch("requests.request", return_value=fake_responses.FIND_ELEMENTS)
 def test_find_elements(*args):
     element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
 
     elements = synchronous.find_elements("", "", "", "")
 
     assert element in elements
@@ -46,20 +62,22 @@
 
 @patch("requests.request", return_value=fake_responses.GET_PROPERTY_VALUE)
 def test_get_property(*args):
     expected = "any_value"
 
     assert synchronous.get_property("", "", "", "") == expected
 
+
 @patch("requests.request", return_value=fake_responses.GET_ATTRIBUTE_VALUE)
 def test_get_attribute(*args):
     expected = "any_value"
 
     assert synchronous.get_attribute("", "", "", "") == expected
 
+
 @patch("requests.request", return_value=fake_responses.GO_TO_PAGE)
 def test_go_to_page(*args):
     assert synchronous.go_to_page("", "", "") is True
 
 
 @patch("requests.request", return_value=fake_responses.CLOSE_SESSION)
 def test_close_session(*args):
```

### Comparing `caqui-1.0.7/.gitignore` & `caqui-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/LICENSE` & `caqui-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.0.7/README.md` & `caqui-1.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 **Caqui** can be used in remote calls. As it needs just the server URL, the user can start the Driver as a server in any host and provide the URL to **Caqui** clients.
 
 # Tested WebDrivers
 
 | WebDriver               | Version       |
 | ----------------------- | ------------- |
-| Google Chrome           | 113           |
+| Google Chrome           | 113, 114      |
 | Firefox (geckodriver)   | 113           |
 
 # Simple start
 Install the lastest version of **Caqui**
 
 ```
 pip install caqui
```

#### html2text {}

```diff
@@ -11,19 +11,19 @@
 the motivation to create **Caqui** was feed by the inspiration in [Arsenic]
 (https://github.com/HENNGE/arsenic) library. **Caqui** is planned to be Driver
 agnostic, so the user can start any Driver as a server and just inform the
 server URL. Hence, the code is decoupled from the chosen Driver. **Caqui** can
 be used in remote calls. As it needs just the server URL, the user can start
 the Driver as a server in any host and provide the URL to **Caqui** clients. #
 Tested WebDrivers | WebDriver | Version | | ----------------------- | ---------
----- | | Google Chrome | 113 | | Firefox (geckodriver) | 113 | # Simple start
-Install the lastest version of **Caqui** ``` pip install caqui ``` Download the
-same [ChromeDriver](https://chromedriver.chromium.org/downloads) version as
-your installed Chrome and start the Driver as a server using the port "9999"
-``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
+---- | | Google Chrome | 113, 114 | | Firefox (geckodriver) | 113 | # Simple
+start Install the lastest version of **Caqui** ``` pip install caqui ```
+Download the same [ChromeDriver](https://chromedriver.chromium.org/downloads)
+version as your installed Chrome and start the Driver as a server using the
+port "9999" ``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
 (418b78f5838ed0b1c69bb4e51ea0252171854915-refs/branch-heads/4606@{#1204}) on
 port 9999 Only local connections are allowed. Please see https://
 chromedriver.chromium.org/security-considerations for suggestions on keeping
 ChromeDriver safe. ChromeDriver was started successfully. ``` Given the HTML
 content in `playground.html` ```
 ****** Basic page ******
 This is a sample page to be used to sanity check
```

### Comparing `caqui-1.0.7/pyproject.toml` & `caqui-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `caqui-1.0.7/PKG-INFO` & `caqui-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caqui
-Version: 1.0.7
+Version: 1.0.8
 Summary: Run asynchronous commands in WebDrivers
 Project-URL: Homepage, https://github.com/douglasdcm/caqui
 Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso <noemail@noemail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 
 **Caqui** can be used in remote calls. As it needs just the server URL, the user can start the Driver as a server in any host and provide the URL to **Caqui** clients.
 
 # Tested WebDrivers
 
 | WebDriver               | Version       |
 | ----------------------- | ------------- |
-| Google Chrome           | 113           |
+| Google Chrome           | 113, 114      |
 | Firefox (geckodriver)   | 113           |
 
 # Simple start
 Install the lastest version of **Caqui**
 
 ```
 pip install caqui
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.0.7 Summary: Run asynchronous
+Metadata-Version: 2.1 Name: caqui Version: 1.0.8 Summary: Run asynchronous
 commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
 caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso
 noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
@@ -19,19 +19,19 @@
 the motivation to create **Caqui** was feed by the inspiration in [Arsenic]
 (https://github.com/HENNGE/arsenic) library. **Caqui** is planned to be Driver
 agnostic, so the user can start any Driver as a server and just inform the
 server URL. Hence, the code is decoupled from the chosen Driver. **Caqui** can
 be used in remote calls. As it needs just the server URL, the user can start
 the Driver as a server in any host and provide the URL to **Caqui** clients. #
 Tested WebDrivers | WebDriver | Version | | ----------------------- | ---------
----- | | Google Chrome | 113 | | Firefox (geckodriver) | 113 | # Simple start
-Install the lastest version of **Caqui** ``` pip install caqui ``` Download the
-same [ChromeDriver](https://chromedriver.chromium.org/downloads) version as
-your installed Chrome and start the Driver as a server using the port "9999"
-``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
+---- | | Google Chrome | 113, 114 | | Firefox (geckodriver) | 113 | # Simple
+start Install the lastest version of **Caqui** ``` pip install caqui ```
+Download the same [ChromeDriver](https://chromedriver.chromium.org/downloads)
+version as your installed Chrome and start the Driver as a server using the
+port "9999" ``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
 (418b78f5838ed0b1c69bb4e51ea0252171854915-refs/branch-heads/4606@{#1204}) on
 port 9999 Only local connections are allowed. Please see https://
 chromedriver.chromium.org/security-considerations for suggestions on keeping
 ChromeDriver safe. ChromeDriver was started successfully. ``` Given the HTML
 content in `playground.html` ```
 ****** Basic page ******
 This is a sample page to be used to sanity check
```

