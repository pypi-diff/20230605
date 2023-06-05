# Comparing `tmp/redoubt_agent-0.1.95.tar.gz` & `tmp/redoubt_agent-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redoubt_agent-0.1.95.tar", last modified: Fri Jun  2 13:16:59 2023, max compression
+gzip compressed data, was "redoubt_agent-0.1.96.tar", last modified: Mon Jun  5 18:50:02 2023, max compression
```

## Comparing `redoubt_agent-0.1.95.tar` & `redoubt_agent-0.1.96.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:16:59.085777 redoubt_agent-0.1.95/
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)    11357 2023-05-31 14:59:32.000000 redoubt_agent-0.1.95/LICENSE
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2630 2023-06-02 13:16:59.085874 redoubt_agent-0.1.95/PKG-INFO
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1649 2023-06-02 13:16:55.000000 redoubt_agent-0.1.95/README.md
--rw-r--r--   0 mnechepurenko   (501) staff       (20)      104 2023-06-02 11:38:53.000000 redoubt_agent-0.1.95/pyproject.toml
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:16:59.084340 redoubt_agent-0.1.95/redoubt_agent/
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       67 2023-06-02 12:57:25.000000 redoubt_agent-0.1.95/redoubt_agent/__init__.py
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2900 2023-06-02 13:16:23.000000 redoubt_agent-0.1.95/redoubt_agent/redoubt_sdk.py
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:16:59.085609 redoubt_agent-0.1.95/redoubt_agent.egg-info/
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2630 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/PKG-INFO
--rw-r--r--   0 mnechepurenko   (501) staff       (20)      326 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/SOURCES.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/dependency_links.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 12:57:34.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/not-zip-safe
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       25 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/requires.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       14 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/top_level.txt
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1105 2023-06-02 13:16:59.086288 redoubt_agent-0.1.95/setup.cfg
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)       68 2023-06-02 11:01:57.000000 redoubt_agent-0.1.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:50:02.444700 redoubt_agent-0.1.96/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:49:50.000000 redoubt_agent-0.1.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-05 18:50:02.444700 redoubt_agent-0.1.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-05 18:49:50.000000 redoubt_agent-0.1.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 18:49:50.000000 redoubt_agent-0.1.96/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:50:02.444700 redoubt_agent-0.1.96/redoubt_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 18:49:50.000000 redoubt_agent-0.1.96/redoubt_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-05 18:49:50.000000 redoubt_agent-0.1.96/redoubt_agent/redoubt_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:50:02.444700 redoubt_agent-0.1.96/redoubt_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-05 18:50:02.000000 redoubt_agent-0.1.96/redoubt_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-05 18:50:02.000000 redoubt_agent-0.1.96/redoubt_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:50:02.000000 redoubt_agent-0.1.96/redoubt_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:50:02.000000 redoubt_agent-0.1.96/redoubt_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 18:50:02.000000 redoubt_agent-0.1.96/redoubt_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 18:50:02.000000 redoubt_agent-0.1.96/redoubt_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-05 18:50:02.444700 redoubt_agent-0.1.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 18:49:50.000000 redoubt_agent-0.1.96/setup.py
```

### Comparing `redoubt_agent-0.1.95/LICENSE` & `redoubt_agent-0.1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.95/PKG-INFO` & `redoubt_agent-0.1.96/redoubt_agent.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: redoubt_agent
-Version: 0.1.95
+Name: redoubt-agent
+Version: 0.1.96
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
 Keywords: TON,redoubt,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -44,25 +43,23 @@
 To use SDK one need to request API key from [@RedoubtAPIBot](https://t.me/RedoubtAPIBot) and pass it either directly 
 to `RedoubtEventsStream` instance or using `REDOUBT_API_KEY` environment variable.
 
 ## Examples
 
 ### New pools bot
 
-* [New pools detector](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/new_pools.py)
+* [New pools detector](./examples/new_pools.py)
 
 It is monitoring for new pools and just prints info.
 
 ### Jetton transfers bot
 
-* [Jetton transfers bot](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/jetton_transfer.py)
+* [Jetton transfers bot](./examples/jetton_transfer.py)
 
 More complicated example. It listens for all Jetton transfers and after receiving info 
 about the transfer it requests additional info over GraphQL API. In this case it
 uses additional GraphQL request to get Jetton metadata (symbol and decimals).
 
 As a result you will get such a message:
 ```
 EQ...EJ => EQ...7f 22.033882202 SCALE
 ```
-
-
```

### Comparing `redoubt_agent-0.1.95/README.md` & `redoubt_agent-0.1.96/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 To use SDK one need to request API key from [@RedoubtAPIBot](https://t.me/RedoubtAPIBot) and pass it either directly 
 to `RedoubtEventsStream` instance or using `REDOUBT_API_KEY` environment variable.
 
 ## Examples
 
 ### New pools bot
 
-* [New pools detector](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/new_pools.py)
+* [New pools detector](./examples/new_pools.py)
 
 It is monitoring for new pools and just prints info.
 
 ### Jetton transfers bot
 
-* [Jetton transfers bot](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/jetton_transfer.py)
+* [Jetton transfers bot](./examples/jetton_transfer.py)
 
 More complicated example. It listens for all Jetton transfers and after receiving info 
 about the transfer it requests additional info over GraphQL API. In this case it
 uses additional GraphQL request to get Jetton metadata (symbol and decimals).
 
 As a result you will get such a message:
 ```
```

### Comparing `redoubt_agent-0.1.95/redoubt_agent/redoubt_sdk.py` & `redoubt_agent-0.1.96/redoubt_agent/redoubt_sdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 from gql import Client, gql
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.requests import RequestsHTTPTransport
 from gql.transport.websockets import WebsocketsTransport
 from loguru import logger
 
-DEFAULT_ENDPOINT = 'ws://44.210.191.88:9080/v1/graphql'  # TODO update to wss
+DEFAULT_ENDPOINT = 'wss://graphql.redoubt.online/v1/graphql'
 
 
 class RedoubtEventsStream:
     def __init__(self, api_key=None, endpoint=DEFAULT_ENDPOINT):
         if api_key is None:
             api_key = os.environ.get('REDOUBT_API_KEY', None)
         assert api_key is not None, "API key not found"
         self.transport = WebsocketsTransport(
             url=endpoint, ping_interval=1, pong_timeout=1, headers={
                 'X-API-Key': api_key
             }
         )
 
     async def execute(self, query):
-        res = await self.session.execute(query)
-        logger.info(res)
+        async with Client(transport=self.transport, fetch_schema_from_transport=False) as session:
+            return await session.execute(gql(query))
 
     async def subscribe(self, handler, scope=None, event_type=None, event_target=None):
         now = datetime.now().astimezone(timezone.utc).strftime(
             "%Y-%m-%d %H:%M:%S")  # "2023-05-29 12:10:16.051"# int(time.time())
         logger.info(f"Starting from cursor {now}")
         filters = []
         if scope is not None:
```

### Comparing `redoubt_agent-0.1.95/redoubt_agent.egg-info/PKG-INFO` & `redoubt_agent-0.1.96/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: redoubt-agent
-Version: 0.1.95
+Name: redoubt_agent
+Version: 0.1.96
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
 Keywords: TON,redoubt,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -44,25 +43,23 @@
 To use SDK one need to request API key from [@RedoubtAPIBot](https://t.me/RedoubtAPIBot) and pass it either directly 
 to `RedoubtEventsStream` instance or using `REDOUBT_API_KEY` environment variable.
 
 ## Examples
 
 ### New pools bot
 
-* [New pools detector](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/new_pools.py)
+* [New pools detector](./examples/new_pools.py)
 
 It is monitoring for new pools and just prints info.
 
 ### Jetton transfers bot
 
-* [Jetton transfers bot](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/jetton_transfer.py)
+* [Jetton transfers bot](./examples/jetton_transfer.py)
 
 More complicated example. It listens for all Jetton transfers and after receiving info 
 about the transfer it requests additional info over GraphQL API. In this case it
 uses additional GraphQL request to get Jetton metadata (symbol and decimals).
 
 As a result you will get such a message:
 ```
 EQ...EJ => EQ...7f 22.033882202 SCALE
 ```
-
-
```

### Comparing `redoubt_agent-0.1.95/setup.cfg` & `redoubt_agent-0.1.96/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = redoubt_agent
-version = 0.1.95
+version = 0.1.96
 description = re:doubt Bot Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.redoubt.online/
 keywords = TON, redoubt, sdk
 license = Apache 2.0
 classifiers =
```

