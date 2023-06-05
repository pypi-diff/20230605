# Comparing `tmp/EdgeGPT-0.8.1.tar.gz` & `tmp/EdgeGPT-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.8.1.tar", last modified: Sun Jun  4 13:13:14 2023, max compression
+gzip compressed data, was "EdgeGPT-0.8.2.tar", last modified: Mon Jun  5 11:28:10 2023, max compression
```

## Comparing `EdgeGPT-0.8.1.tar` & `EdgeGPT-0.8.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-04 13:13:13.000000 EdgeGPT-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:13:14.020337 EdgeGPT-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34686 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34817 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/src/EdgeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/src/ImageGen.py
```

### Comparing `EdgeGPT-0.8.1/LICENSE` & `EdgeGPT-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.8.1/PKG-INFO` & `EdgeGPT-0.8.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.8.1
+Version: 0.8.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -54,49 +54,61 @@
 ```bash
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
-- A Microsoft Account with access to <https://bing.com/chat> (Optional)
+- A Microsoft Account with access to <https://bing.com/chat> (Optional, depending on your region)
 - Required in a supported country or region with New Bing (Chinese mainland VPN required)
 - [Selenium](https://pypi.org/project/selenium/) (for automatic cookie setup)
 
+</details>
 <details>
 
 <summary>
 
 # Chatbot
 
 </summary>
 
 ## Authentication
 
-!!! NOT REQUIRED ANYMORE !!!
-Microsoft has made the chat feature available to everyone, so you don't need to use cookies from a logged-in Microsoft account any more.  However, if you wish to cycle through multiple cookies/accounts, please look at the `EdgeUtils.Cookie` methods.
+!!! POSSIBLY NOT REQUIRED ANYMORE !!!
+In some regions, Microsoft has made the chat feature available to everyone, so you might be able to skip this step. You can check this with a browser (with user-agent set to reflect Edge), by trying to start a chat without logging in.
+
+It was also found that it might depend on your IP address. For example, if you try to access the chat features from an IP that is known to belong to a datacenter range (vServers, root servers, VPN, common proxies, ...), you might be required to log in while being able to access the features just fine from your home IP address. If you receive the following error, you can try providing a cookie and see if it works then:
+`Exception: Authentication failed. You have not been accepted into the beta.`
 
-1. Install the latest version of Microsoft Edge
 <details>
 
-2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+<summary>
+  
+### Collecting cookies
 
-</details>
+</summary>
+
+1. Get a browser that looks like Microsoft Edge.
+  
+ * a) (Easy) Install the latest version of Microsoft Edge
+ * b) (Advanced) Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+  
+2. Open [bing.com/chat](https://bing.com/chat)
+3. If you see a chat feature, you are good to continue...
+4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+5. Go to [bing.com](https://bing.com)
+6. Open the extension
+7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
+8. Paste your cookies into a file `cookies.json`
 
-3. Open [bing.com/chat](https://bing.com/chat)
-4. If you see a chat feature, you are good to continue...
-5. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
-6. Go to [bing.com](https://bing.com)
-7. Open the extension
-8. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-9. Paste your cookies into a file `cookies.json`
+</details>
 
 ### In code:
 ```python
-cookies = json.loads(open("./path/to/cookies.json", encoding="utf-8").read())
+cookies = json.loads(open("./path/to/cookies.json", encoding="utf-8").read())  # might omit cookies option
 bot = await Chatbot.create(cookies=cookies)
 ```
 
 ## Running from the Command Line
 
 ```
  $ python3 -m EdgeGPT -h
@@ -138,15 +150,15 @@
 Use Async for the best experience, for example:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
-    bot = await Chatbot.create() # Passing cookies is optional
+    bot = await Chatbot.create() # Passing cookies is "optional", as explained above
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,71 +1,80 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
  version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
   # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
 ``` ### Requirements - python 3.8+ - A Microsoft Account with access to
-bing.com/chat> (Optional) - Required in a supported country or region with New
-Bing (Chinese mainland VPN required) - [Selenium](https://pypi.org/project/
-selenium/) (for automatic cookie setup)   # Chatbot  ## Authentication !!! NOT
-REQUIRED ANYMORE !!! Microsoft has made the chat feature available to everyone,
-so you don't need to use cookies from a logged-in Microsoft account any more.
-However, if you wish to cycle through multiple cookies/accounts, please look at
-the `EdgeUtils.Cookie` methods. 1. Install the latest version of Microsoft Edge
-2. Alternatively, you can use any browser and set the user-agent to look like
-you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
+bing.com/chat> (Optional, depending on your region) - Required in a supported
+country or region with New Bing (Chinese mainland VPN required) - [Selenium]
+(https://pypi.org/project/selenium/) (for automatic cookie setup)    # Chatbot
+## Authentication !!! POSSIBLY NOT REQUIRED ANYMORE !!! In some regions,
+Microsoft has made the chat feature available to everyone, so you might be able
+to skip this step. You can check this with a browser (with user-agent set to
+reflect Edge), by trying to start a chat without logging in. It was also found
+that it might depend on your IP address. For example, if you try to access the
+chat features from an IP that is known to belong to a datacenter range
+(vServers, root servers, VPN, common proxies, ...), you might be required to
+log in while being able to access the features just fine from your home IP
+address. If you receive the following error, you can try providing a cookie and
+see if it works then: `Exception: Authentication failed. You have not been
+accepted into the beta.`   ### Collecting cookies  1. Get a browser that looks
+like Microsoft Edge. * a) (Easy) Install the latest version of Microsoft Edge *
+b) (Advanced) Alternatively, you can use any browser and set the user-agent to
+look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/
 111.0.1661.51`). You can do this easily with an extension like "User-Agent
 Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
 user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
 (https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat feature,
-you are good to continue... 5. Install the cookie editor extension for [Chrome]
+2. Open [bing.com/chat](https://bing.com/chat) 3. If you see a chat feature,
+you are good to continue... 4. Install the cookie editor extension for [Chrome]
 (https://chrome.google.com/webstore/detail/cookie-editor/
 hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
-US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
-the extension 8. Click "Export" on the bottom right, then "Export as JSON"
-(This saves your cookies to clipboard) 9. Paste your cookies into a file
-`cookies.json` ### In code: ```python cookies = json.loads(open("./path/to/
-cookies.json", encoding="utf-8").read()) bot = await Chatbot.create
-(cookies=cookies) ``` ## Running from the Command Line ``` $ python3 -m EdgeGPT
--h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
-github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
-exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--
-rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
+US/firefox/addon/cookie-editor/) 5. Go to [bing.com](https://bing.com) 6. Open
+the extension 7. Click "Export" on the bottom right, then "Export as JSON"
+(This saves your cookies to clipboard) 8. Paste your cookies into a file
+`cookies.json`  ### In code: ```python cookies = json.loads(open("./path/to/
+cookies.json", encoding="utf-8").read()) # might omit cookies option bot =
+await Chatbot.create(cookies=cookies) ``` ## Running from the Command Line ```
+$ python3 -m EdgeGPT -h EdgeGPT - A demo of reverse engineering the Bing GPT
+chatbot Repo: github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help
+Type !exit to exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--
+no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
 {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE] [--
 history-file HISTORY_FILE] [--locale LOCALE] options: -h, --help show this help
 message and exit --enter-once --search-result --no-stream --rich --proxy PROXY
 Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g. wss:/
 /sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --prompt
 PROMPT prompt to start with --cookie-file COOKIE_FILE path to cookie file --
 history-file HISTORY_FILE path to history file --locale LOCALE your locale
 (e.g. en-US, zh-CN, en-IE, en-GB) ``` (China/US/UK/Norway has enhanced support
 for locale) ## Running in Python ### 1. The `Chatbot` class and `asyncio` for
 more granular control Use Async for the best experience, for example: ```python
 import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
-bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
-(prompt="Hello world", conversation_style=ConversationStyle.creative)) await
-bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
-`Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
-the 'precise' conversation style by default) and see just the main text output
-rather than the whole API response: Remeber to store your cookies in a specific
-format: `bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q
-= Query("What are you? Give your answer as Python code") print(q) ``` Or change
-the conversation style or cookie file to be used: ```python q = Query( "What
-are you? Give your answer as Python code", style="creative", # or 'balanced'
+bot = await Chatbot.create() # Passing cookies is "optional", as explained
+above print(await bot.ask(prompt="Hello world",
+conversation_style=ConversationStyle.creative)) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
+classes  Create a simple Bing Chat AI query (using the 'precise' conversation
+style by default) and see just the main text output rather than the whole API
+response: Remeber to store your cookies in a specific format:
+`bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q = Query
+("What are you? Give your answer as Python code") print(q) ``` Or change the
+conversation style or cookie file to be used: ```python q = Query( "What are
+you? Give your answer as Python code", style="creative", # or 'balanced'
 cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
 output, code snippets, list of sources/references, or suggested follow-on
 questions using the following attributes: ```python q.output q.code
 q.suggestions q.sources # for the full json output q.sources_dict # for a
 dictionary of titles and urls ``` Get the orginal prompt and the conversation
 style you specified: ```python q.prompt q.style repr(q) ``` Access previous
 Queries made since importing `Query`: ```python Query.index # A list of Query
```

### Comparing `EdgeGPT-0.8.1/README.md` & `EdgeGPT-0.8.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,49 +35,61 @@
 ```bash
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
-- A Microsoft Account with access to <https://bing.com/chat> (Optional)
+- A Microsoft Account with access to <https://bing.com/chat> (Optional, depending on your region)
 - Required in a supported country or region with New Bing (Chinese mainland VPN required)
 - [Selenium](https://pypi.org/project/selenium/) (for automatic cookie setup)
 
+</details>
 <details>
 
 <summary>
 
 # Chatbot
 
 </summary>
 
 ## Authentication
 
-!!! NOT REQUIRED ANYMORE !!!
-Microsoft has made the chat feature available to everyone, so you don't need to use cookies from a logged-in Microsoft account any more.  However, if you wish to cycle through multiple cookies/accounts, please look at the `EdgeUtils.Cookie` methods.
+!!! POSSIBLY NOT REQUIRED ANYMORE !!!
+In some regions, Microsoft has made the chat feature available to everyone, so you might be able to skip this step. You can check this with a browser (with user-agent set to reflect Edge), by trying to start a chat without logging in.
+
+It was also found that it might depend on your IP address. For example, if you try to access the chat features from an IP that is known to belong to a datacenter range (vServers, root servers, VPN, common proxies, ...), you might be required to log in while being able to access the features just fine from your home IP address. If you receive the following error, you can try providing a cookie and see if it works then:
+`Exception: Authentication failed. You have not been accepted into the beta.`
 
-1. Install the latest version of Microsoft Edge
 <details>
 
-2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+<summary>
+  
+### Collecting cookies
 
-</details>
+</summary>
+
+1. Get a browser that looks like Microsoft Edge.
+  
+ * a) (Easy) Install the latest version of Microsoft Edge
+ * b) (Advanced) Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+  
+2. Open [bing.com/chat](https://bing.com/chat)
+3. If you see a chat feature, you are good to continue...
+4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+5. Go to [bing.com](https://bing.com)
+6. Open the extension
+7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
+8. Paste your cookies into a file `cookies.json`
 
-3. Open [bing.com/chat](https://bing.com/chat)
-4. If you see a chat feature, you are good to continue...
-5. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
-6. Go to [bing.com](https://bing.com)
-7. Open the extension
-8. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-9. Paste your cookies into a file `cookies.json`
+</details>
 
 ### In code:
 ```python
-cookies = json.loads(open("./path/to/cookies.json", encoding="utf-8").read())
+cookies = json.loads(open("./path/to/cookies.json", encoding="utf-8").read())  # might omit cookies option
 bot = await Chatbot.create(cookies=cookies)
 ```
 
 ## Running from the Command Line
 
 ```
  $ python3 -m EdgeGPT -h
@@ -119,15 +131,15 @@
 Use Async for the best experience, for example:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
-    bot = await Chatbot.create() # Passing cookies is optional
+    bot = await Chatbot.create() # Passing cookies is "optional", as explained above
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,61 +1,70 @@
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
  version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
   # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
 ``` ### Requirements - python 3.8+ - A Microsoft Account with access to
-bing.com/chat> (Optional) - Required in a supported country or region with New
-Bing (Chinese mainland VPN required) - [Selenium](https://pypi.org/project/
-selenium/) (for automatic cookie setup)   # Chatbot  ## Authentication !!! NOT
-REQUIRED ANYMORE !!! Microsoft has made the chat feature available to everyone,
-so you don't need to use cookies from a logged-in Microsoft account any more.
-However, if you wish to cycle through multiple cookies/accounts, please look at
-the `EdgeUtils.Cookie` methods. 1. Install the latest version of Microsoft Edge
-2. Alternatively, you can use any browser and set the user-agent to look like
-you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
+bing.com/chat> (Optional, depending on your region) - Required in a supported
+country or region with New Bing (Chinese mainland VPN required) - [Selenium]
+(https://pypi.org/project/selenium/) (for automatic cookie setup)    # Chatbot
+## Authentication !!! POSSIBLY NOT REQUIRED ANYMORE !!! In some regions,
+Microsoft has made the chat feature available to everyone, so you might be able
+to skip this step. You can check this with a browser (with user-agent set to
+reflect Edge), by trying to start a chat without logging in. It was also found
+that it might depend on your IP address. For example, if you try to access the
+chat features from an IP that is known to belong to a datacenter range
+(vServers, root servers, VPN, common proxies, ...), you might be required to
+log in while being able to access the features just fine from your home IP
+address. If you receive the following error, you can try providing a cookie and
+see if it works then: `Exception: Authentication failed. You have not been
+accepted into the beta.`   ### Collecting cookies  1. Get a browser that looks
+like Microsoft Edge. * a) (Easy) Install the latest version of Microsoft Edge *
+b) (Advanced) Alternatively, you can use any browser and set the user-agent to
+look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/
 111.0.1661.51`). You can do this easily with an extension like "User-Agent
 Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
 user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
 (https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat feature,
-you are good to continue... 5. Install the cookie editor extension for [Chrome]
+2. Open [bing.com/chat](https://bing.com/chat) 3. If you see a chat feature,
+you are good to continue... 4. Install the cookie editor extension for [Chrome]
 (https://chrome.google.com/webstore/detail/cookie-editor/
 hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
-US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
-the extension 8. Click "Export" on the bottom right, then "Export as JSON"
-(This saves your cookies to clipboard) 9. Paste your cookies into a file
-`cookies.json` ### In code: ```python cookies = json.loads(open("./path/to/
-cookies.json", encoding="utf-8").read()) bot = await Chatbot.create
-(cookies=cookies) ``` ## Running from the Command Line ``` $ python3 -m EdgeGPT
--h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
-github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
-exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--
-rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
+US/firefox/addon/cookie-editor/) 5. Go to [bing.com](https://bing.com) 6. Open
+the extension 7. Click "Export" on the bottom right, then "Export as JSON"
+(This saves your cookies to clipboard) 8. Paste your cookies into a file
+`cookies.json`  ### In code: ```python cookies = json.loads(open("./path/to/
+cookies.json", encoding="utf-8").read()) # might omit cookies option bot =
+await Chatbot.create(cookies=cookies) ``` ## Running from the Command Line ```
+$ python3 -m EdgeGPT -h EdgeGPT - A demo of reverse engineering the Bing GPT
+chatbot Repo: github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help
+Type !exit to exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--
+no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
 {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE] [--
 history-file HISTORY_FILE] [--locale LOCALE] options: -h, --help show this help
 message and exit --enter-once --search-result --no-stream --rich --proxy PROXY
 Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g. wss:/
 /sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --prompt
 PROMPT prompt to start with --cookie-file COOKIE_FILE path to cookie file --
 history-file HISTORY_FILE path to history file --locale LOCALE your locale
 (e.g. en-US, zh-CN, en-IE, en-GB) ``` (China/US/UK/Norway has enhanced support
 for locale) ## Running in Python ### 1. The `Chatbot` class and `asyncio` for
 more granular control Use Async for the best experience, for example: ```python
 import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
-bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
-(prompt="Hello world", conversation_style=ConversationStyle.creative)) await
-bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
-`Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
-the 'precise' conversation style by default) and see just the main text output
-rather than the whole API response: Remeber to store your cookies in a specific
-format: `bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q
-= Query("What are you? Give your answer as Python code") print(q) ``` Or change
-the conversation style or cookie file to be used: ```python q = Query( "What
-are you? Give your answer as Python code", style="creative", # or 'balanced'
+bot = await Chatbot.create() # Passing cookies is "optional", as explained
+above print(await bot.ask(prompt="Hello world",
+conversation_style=ConversationStyle.creative)) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
+classes  Create a simple Bing Chat AI query (using the 'precise' conversation
+style by default) and see just the main text output rather than the whole API
+response: Remeber to store your cookies in a specific format:
+`bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q = Query
+("What are you? Give your answer as Python code") print(q) ``` Or change the
+conversation style or cookie file to be used: ```python q = Query( "What are
+you? Give your answer as Python code", style="creative", # or 'balanced'
 cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
 output, code snippets, list of sources/references, or suggested follow-on
 questions using the following attributes: ```python q.output q.code
 q.suggestions q.sources # for the full json output q.sources_dict # for a
 dictionary of titles and urls ``` Get the orginal prompt and the conversation
 style you specified: ```python q.prompt q.style repr(q) ``` Access previous
 Queries made since importing `Query`: ```python Query.index # A list of Query
```

### Comparing `EdgeGPT-0.8.1/setup.py` & `EdgeGPT-0.8.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.8.1",
+    version="0.8.2",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
@@ -35,15 +35,15 @@
         "prompt_toolkit",
         "requests",
         "aiofiles",
         "BingImageCreator>=0.3.0",
     ],
     long_description=Path.open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    py_modules=["EdgeGPT", "ImageGen"],
+    py_modules=["EdgeGPT", "EdgeUtils", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `EdgeGPT-0.8.1/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.8.2/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.8.1
+Version: 0.8.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -54,49 +54,61 @@
 ```bash
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
-- A Microsoft Account with access to <https://bing.com/chat> (Optional)
+- A Microsoft Account with access to <https://bing.com/chat> (Optional, depending on your region)
 - Required in a supported country or region with New Bing (Chinese mainland VPN required)
 - [Selenium](https://pypi.org/project/selenium/) (for automatic cookie setup)
 
+</details>
 <details>
 
 <summary>
 
 # Chatbot
 
 </summary>
 
 ## Authentication
 
-!!! NOT REQUIRED ANYMORE !!!
-Microsoft has made the chat feature available to everyone, so you don't need to use cookies from a logged-in Microsoft account any more.  However, if you wish to cycle through multiple cookies/accounts, please look at the `EdgeUtils.Cookie` methods.
+!!! POSSIBLY NOT REQUIRED ANYMORE !!!
+In some regions, Microsoft has made the chat feature available to everyone, so you might be able to skip this step. You can check this with a browser (with user-agent set to reflect Edge), by trying to start a chat without logging in.
+
+It was also found that it might depend on your IP address. For example, if you try to access the chat features from an IP that is known to belong to a datacenter range (vServers, root servers, VPN, common proxies, ...), you might be required to log in while being able to access the features just fine from your home IP address. If you receive the following error, you can try providing a cookie and see if it works then:
+`Exception: Authentication failed. You have not been accepted into the beta.`
 
-1. Install the latest version of Microsoft Edge
 <details>
 
-2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+<summary>
+  
+### Collecting cookies
 
-</details>
+</summary>
+
+1. Get a browser that looks like Microsoft Edge.
+  
+ * a) (Easy) Install the latest version of Microsoft Edge
+ * b) (Advanced) Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+  
+2. Open [bing.com/chat](https://bing.com/chat)
+3. If you see a chat feature, you are good to continue...
+4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+5. Go to [bing.com](https://bing.com)
+6. Open the extension
+7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
+8. Paste your cookies into a file `cookies.json`
 
-3. Open [bing.com/chat](https://bing.com/chat)
-4. If you see a chat feature, you are good to continue...
-5. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
-6. Go to [bing.com](https://bing.com)
-7. Open the extension
-8. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-9. Paste your cookies into a file `cookies.json`
+</details>
 
 ### In code:
 ```python
-cookies = json.loads(open("./path/to/cookies.json", encoding="utf-8").read())
+cookies = json.loads(open("./path/to/cookies.json", encoding="utf-8").read())  # might omit cookies option
 bot = await Chatbot.create(cookies=cookies)
 ```
 
 ## Running from the Command Line
 
 ```
  $ python3 -m EdgeGPT -h
@@ -138,15 +150,15 @@
 Use Async for the best experience, for example:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
-    bot = await Chatbot.create() # Passing cookies is optional
+    bot = await Chatbot.create() # Passing cookies is "optional", as explained above
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,71 +1,80 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
  version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
   # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
 ``` ### Requirements - python 3.8+ - A Microsoft Account with access to
-bing.com/chat> (Optional) - Required in a supported country or region with New
-Bing (Chinese mainland VPN required) - [Selenium](https://pypi.org/project/
-selenium/) (for automatic cookie setup)   # Chatbot  ## Authentication !!! NOT
-REQUIRED ANYMORE !!! Microsoft has made the chat feature available to everyone,
-so you don't need to use cookies from a logged-in Microsoft account any more.
-However, if you wish to cycle through multiple cookies/accounts, please look at
-the `EdgeUtils.Cookie` methods. 1. Install the latest version of Microsoft Edge
-2. Alternatively, you can use any browser and set the user-agent to look like
-you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
+bing.com/chat> (Optional, depending on your region) - Required in a supported
+country or region with New Bing (Chinese mainland VPN required) - [Selenium]
+(https://pypi.org/project/selenium/) (for automatic cookie setup)    # Chatbot
+## Authentication !!! POSSIBLY NOT REQUIRED ANYMORE !!! In some regions,
+Microsoft has made the chat feature available to everyone, so you might be able
+to skip this step. You can check this with a browser (with user-agent set to
+reflect Edge), by trying to start a chat without logging in. It was also found
+that it might depend on your IP address. For example, if you try to access the
+chat features from an IP that is known to belong to a datacenter range
+(vServers, root servers, VPN, common proxies, ...), you might be required to
+log in while being able to access the features just fine from your home IP
+address. If you receive the following error, you can try providing a cookie and
+see if it works then: `Exception: Authentication failed. You have not been
+accepted into the beta.`   ### Collecting cookies  1. Get a browser that looks
+like Microsoft Edge. * a) (Easy) Install the latest version of Microsoft Edge *
+b) (Advanced) Alternatively, you can use any browser and set the user-agent to
+look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/
 111.0.1661.51`). You can do this easily with an extension like "User-Agent
 Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
 user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
 (https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat feature,
-you are good to continue... 5. Install the cookie editor extension for [Chrome]
+2. Open [bing.com/chat](https://bing.com/chat) 3. If you see a chat feature,
+you are good to continue... 4. Install the cookie editor extension for [Chrome]
 (https://chrome.google.com/webstore/detail/cookie-editor/
 hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
-US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
-the extension 8. Click "Export" on the bottom right, then "Export as JSON"
-(This saves your cookies to clipboard) 9. Paste your cookies into a file
-`cookies.json` ### In code: ```python cookies = json.loads(open("./path/to/
-cookies.json", encoding="utf-8").read()) bot = await Chatbot.create
-(cookies=cookies) ``` ## Running from the Command Line ``` $ python3 -m EdgeGPT
--h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
-github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
-exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--
-rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
+US/firefox/addon/cookie-editor/) 5. Go to [bing.com](https://bing.com) 6. Open
+the extension 7. Click "Export" on the bottom right, then "Export as JSON"
+(This saves your cookies to clipboard) 8. Paste your cookies into a file
+`cookies.json`  ### In code: ```python cookies = json.loads(open("./path/to/
+cookies.json", encoding="utf-8").read()) # might omit cookies option bot =
+await Chatbot.create(cookies=cookies) ``` ## Running from the Command Line ```
+$ python3 -m EdgeGPT -h EdgeGPT - A demo of reverse engineering the Bing GPT
+chatbot Repo: github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help
+Type !exit to exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--
+no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
 {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE] [--
 history-file HISTORY_FILE] [--locale LOCALE] options: -h, --help show this help
 message and exit --enter-once --search-result --no-stream --rich --proxy PROXY
 Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g. wss:/
 /sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --prompt
 PROMPT prompt to start with --cookie-file COOKIE_FILE path to cookie file --
 history-file HISTORY_FILE path to history file --locale LOCALE your locale
 (e.g. en-US, zh-CN, en-IE, en-GB) ``` (China/US/UK/Norway has enhanced support
 for locale) ## Running in Python ### 1. The `Chatbot` class and `asyncio` for
 more granular control Use Async for the best experience, for example: ```python
 import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
-bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
-(prompt="Hello world", conversation_style=ConversationStyle.creative)) await
-bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
-`Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
-the 'precise' conversation style by default) and see just the main text output
-rather than the whole API response: Remeber to store your cookies in a specific
-format: `bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q
-= Query("What are you? Give your answer as Python code") print(q) ``` Or change
-the conversation style or cookie file to be used: ```python q = Query( "What
-are you? Give your answer as Python code", style="creative", # or 'balanced'
+bot = await Chatbot.create() # Passing cookies is "optional", as explained
+above print(await bot.ask(prompt="Hello world",
+conversation_style=ConversationStyle.creative)) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
+classes  Create a simple Bing Chat AI query (using the 'precise' conversation
+style by default) and see just the main text output rather than the whole API
+response: Remeber to store your cookies in a specific format:
+`bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q = Query
+("What are you? Give your answer as Python code") print(q) ``` Or change the
+conversation style or cookie file to be used: ```python q = Query( "What are
+you? Give your answer as Python code", style="creative", # or 'balanced'
 cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
 output, code snippets, list of sources/references, or suggested follow-on
 questions using the following attributes: ```python q.output q.code
 q.suggestions q.sources # for the full json output q.sources_dict # for a
 dictionary of titles and urls ``` Get the orginal prompt and the conversation
 style you specified: ```python q.prompt q.style repr(q) ``` Access previous
 Queries made since importing `Query`: ```python Query.index # A list of Query
```

### Comparing `EdgeGPT-0.8.1/src/EdgeGPT.py` & `EdgeGPT-0.8.2/src/EdgeGPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,19 +180,19 @@
 LOCATION_HINT_TYPES = Optional[Union[LocationHint, Literal["USA", "CHINA", "EU", "UK"]]]
 
 
 def get_location_hint_from_locale(locale: str) -> dict | None:
     locale = locale.lower()
     if locale == "en-us":
         hint = LocationHint.USA.value
-    if locale == "zh-cn":
+    elif locale == "zh-cn":
         hint = LocationHint.CHINA.value
-    if locale == "en-gb":
+    elif locale == "en-gb":
         hint = LocationHint.UK.value
-    if locale == "en-ie":
+    elif locale == "en-ie":
         hint = LocationHint.EU.value
     else:
         hint = LocationHint.USA.value
     return hint.get("LocationHint")
 
 
 def guess_locale() -> str:
@@ -587,14 +587,17 @@
                 print(response.url)
                 raise Exception("Update web page context failed")
             # Construct a ChatHub request
             self.request.update(
                 prompt=prompt,
                 conversation_style=conversation_style,
                 options=options,
+                webpage_context=webpage_context,
+                search_result=search_result,
+                locale=locale,
             )
         # Send request
         await self.wss.send_str(_append_identifier(self.request.struct))
         final = False
         draw = False
         resp_txt = ""
         result_text = ""
```

