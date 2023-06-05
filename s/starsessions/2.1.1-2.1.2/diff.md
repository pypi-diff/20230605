# Comparing `tmp/starsessions-2.1.1.tar.gz` & `tmp/starsessions-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starsessions-2.1.1.tar", max compression
+gzip compressed data, was "starsessions-2.1.2.tar", max compression
```

## Comparing `starsessions-2.1.1.tar` & `starsessions-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1073 2022-11-08 21:25:23.705734 starsessions-2.1.1/LICENSE
--rw-r--r--   0        0        0    11423 2022-11-08 21:25:23.705734 starsessions-2.1.1/README.md
--rw-r--r--   0        0        0     2431 2022-11-08 21:25:23.705734 starsessions-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      927 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/__init__.py
--rw-r--r--   0        0        0      426 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/exceptions.py
--rw-r--r--   0        0        0     6232 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/middleware.py
--rw-r--r--   0        0        0        0 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/py.typed
--rw-r--r--   0        0        0      970 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/serializers.py
--rw-r--r--   0        0        0     4592 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/session.py
--rw-r--r--   0        0        0      157 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/stores/__init__.py
--rw-r--r--   0        0        0     1781 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/stores/base.py
--rw-r--r--   0        0        0     1643 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/stores/cookie.py
--rw-r--r--   0        0        0      737 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/stores/memory.py
--rw-r--r--   0        0        0     2719 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/stores/redis.py
--rw-r--r--   0        0        0      143 2022-11-08 21:25:23.705734 starsessions-2.1.1/starsessions/types.py
--rw-r--r--   0        0        0    12697 1970-01-01 00:00:00.000000 starsessions-2.1.1/setup.py
--rw-r--r--   0        0        0    12877 1970-01-01 00:00:00.000000 starsessions-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-05 19:35:34.880428 starsessions-2.1.2/LICENSE
+-rw-r--r--   0        0        0    11423 2023-06-05 19:35:34.880428 starsessions-2.1.2/README.md
+-rw-r--r--   0        0        0     2431 2023-06-05 19:35:34.880428 starsessions-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      927 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/exceptions.py
+-rw-r--r--   0        0        0     6457 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/py.typed
+-rw-r--r--   0        0        0      970 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/serializers.py
+-rw-r--r--   0        0        0     4641 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/session.py
+-rw-r--r--   0        0        0      157 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/stores/__init__.py
+-rw-r--r--   0        0        0     1781 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/stores/base.py
+-rw-r--r--   0        0        0     1643 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/stores/cookie.py
+-rw-r--r--   0        0        0      737 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/stores/memory.py
+-rw-r--r--   0        0        0     2738 2023-06-05 19:35:34.880428 starsessions-2.1.2/starsessions/stores/redis.py
+-rw-r--r--   0        0        0      143 2023-06-05 19:35:34.888419 starsessions-2.1.2/starsessions/types.py
+-rw-r--r--   0        0        0    12676 1970-01-01 00:00:00.000000 starsessions-2.1.2/PKG-INFO
```

### Comparing `starsessions-2.1.1/LICENSE` & `starsessions-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starsessions-2.1.1/README.md` & `starsessions-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `starsessions-2.1.1/pyproject.toml` & `starsessions-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starsessions"
-version = "2.1.1"
+version = "2.1.2"
 description = "Advanced sessions for Starlette and FastAPI frameworks"
 authors = ["alex.oleshkevich <alex.oleshkevich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/alex-oleshkevich/starsessions"
 repository = "https://github.com/alex-oleshkevich/starsessions"
 documentation = "https://github.com/alex-oleshkevich/starsessions"
```

### Comparing `starsessions-2.1.1/starsessions/__init__.py` & `starsessions-2.1.2/starsessions/__init__.py`

 * *Files identical despite different names*

### Comparing `starsessions-2.1.1/starsessions/middleware.py` & `starsessions-2.1.2/starsessions/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import re
 import typing
 from starlette.datastructures import MutableHeaders
 from starlette.requests import HTTPConnection
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
 
 from starsessions import SessionNotLoaded
@@ -15,38 +16,39 @@
 
     def __getattribute__(self, item: str) -> typing.Any:
         if item == "_raise":
             return super().__getattribute__(item)
 
         self._raise()
 
-    def __setitem__(self, key: str, value: typing.Any) -> typing.NoReturn:
+    def __setitem__(self, key: str, value: typing.Any) -> typing.NoReturn:  # pragma: nocover
         self._raise()
 
-    def __getitem__(self, key: str) -> typing.NoReturn:
+    def __getitem__(self, key: str) -> typing.NoReturn:  # pragma: nocover
         self._raise()
 
     def _raise(self) -> typing.NoReturn:
         raise SessionNotLoaded("Attempt to access session that has not been loaded yet.")
 
 
 class SessionMiddleware:
     def __init__(
         self,
         app: ASGIApp,
         store: SessionStore,
-        lifetime: int = 0,  # session-only
+        lifetime: typing.Union[int, datetime.timedelta] = 0,  # session-only
         rolling: bool = False,
         cookie_name: str = "session",
         cookie_same_site: str = "lax",
         cookie_https_only: bool = True,
         cookie_domain: typing.Optional[str] = None,
         cookie_path: typing.Optional[str] = None,
         serializer: typing.Optional[Serializer] = None,
     ) -> None:
+        lifetime = int(lifetime.total_seconds() if isinstance(lifetime, datetime.timedelta) else lifetime)
         assert lifetime >= 0, "Session lifetime cannot be less than zero seconds."
 
         self.app = app
         self.store = store
         self.rolling = rolling
         self.serializer = serializer or JsonSerializer()
         self.cookie_name = cookie_name
@@ -70,15 +72,16 @@
         scope["session_handler"] = handler
 
         async def send_wrapper(message: Message) -> None:
             if message["type"] != "http.response.start":
                 await send(message)
                 return
 
-            if not handler.is_loaded:  # session was not loaded, do nothing
+            # session was not loaded, do nothing
+            if not handler.is_loaded:  # pragma: nocover
                 await send(message)
                 return
 
             nonlocal session_id
             path = self.cookie_path or scope.get("root_path", "") or "/"
 
             if handler.is_empty:
```

### Comparing `starsessions-2.1.1/starsessions/serializers.py` & `starsessions-2.1.2/starsessions/serializers.py`

 * *Files identical despite different names*

### Comparing `starsessions-2.1.1/starsessions/session.py` & `starsessions-2.1.2/starsessions/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,16 @@
         self.serializer = serializer
         self.is_loaded = False
         self.initially_empty = False
         self.lifetime = lifetime
         self.metadata: typing.Optional[SessionMetadata] = None
 
     async def load(self) -> None:
-        if self.is_loaded:  # don't refresh existing session, it may contain user data
+        # don't refresh existing session, it may contain user data
+        if self.is_loaded:  # pragma: nocover, IDK how to test it :(
             return
 
         self.is_loaded = True
         data = {}
         if self.session_id:
             data = self.serializer.deserialize(
                 await self.store.read(
```

### Comparing `starsessions-2.1.1/starsessions/stores/base.py` & `starsessions-2.1.2/starsessions/stores/base.py`

 * *Files identical despite different names*

### Comparing `starsessions-2.1.1/starsessions/stores/cookie.py` & `starsessions-2.1.2/starsessions/stores/cookie.py`

 * *Files identical despite different names*

### Comparing `starsessions-2.1.1/starsessions/stores/memory.py` & `starsessions-2.1.2/starsessions/stores/memory.py`

 * *Files identical despite different names*

### Comparing `starsessions-2.1.1/starsessions/stores/redis.py` & `starsessions-2.1.2/starsessions/stores/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from starsessions.stores.base import SessionStore
 
 
 def prefix_factory(prefix: str, key: str) -> str:
     return prefix + key
 
 
-if typing.TYPE_CHECKING:
+if typing.TYPE_CHECKING:  # pragma: nocover
     BaseRedis = Redis[bytes]
 else:
     BaseRedis = Redis
 
 
 class RedisStore(SessionStore):
     """Stores session data in a Redis server."""
```

### Comparing `starsessions-2.1.1/setup.py` & `starsessions-2.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,408 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: starsessions
+Version: 2.1.2
+Summary: Advanced sessions for Starlette and FastAPI frameworks
+Home-page: https://github.com/alex-oleshkevich/starsessions
+License: MIT
+Keywords: starlette,fastapi,asgi,session
+Author: alex.oleshkevich
+Author-email: alex.oleshkevich@gmail.com
+Requires-Python: >=3.8.0,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Provides-Extra: redis
+Requires-Dist: itsdangerous (>=2.0.1,<3.0.0)
+Requires-Dist: redis (>=4.2.0rc1) ; extra == "redis"
+Requires-Dist: starlette (>=0,<1)
+Project-URL: Documentation, https://github.com/alex-oleshkevich/starsessions
+Project-URL: Repository, https://github.com/alex-oleshkevich/starsessions
+Description-Content-Type: text/markdown
 
-packages = \
-['starsessions', 'starsessions.stores']
+## Starsessions
 
-package_data = \
-{'': ['*']}
+Advanced sessions for Starlette and FastAPI frameworks
 
-install_requires = \
-['itsdangerous>=2.0.1,<3.0.0', 'starlette>=0,<1']
-
-extras_require = \
-{'redis': ['redis>=4.2.0rc1']}
-
-setup_kwargs = {
-    'name': 'starsessions',
-    'version': '2.1.1',
-    'description': 'Advanced sessions for Starlette and FastAPI frameworks',
-    'long_description': '## Starsessions\n\nAdvanced sessions for Starlette and FastAPI frameworks\n\n![PyPI](https://img.shields.io/pypi/v/starsessions)\n![GitHub Workflow Status](https://img.shields.io/github/workflow/status/alex-oleshkevich/starsessions/Lint%20and%20test)\n![GitHub](https://img.shields.io/github/license/alex-oleshkevich/starsessions)\n![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/starsessions)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/starsessions)\n![GitHub Release Date](https://img.shields.io/github/release-date/alex-oleshkevich/starsessions)\n\n## Installation\n\nInstall `starsessions` using PIP or poetry:\n\n```bash\npip install starsessions\n# or\npoetry add starsessions\n```\n\nUse `redis` extra for [Redis support](#redis).\n\n## Quick start\n\nSee example application in [`examples/`](examples) directory of this repository.\n\n## Usage\n\n1. Add `starsessions.SessionMiddleware` to your application to enable session support,\n2. Configure session store and pass it to the middleware,\n3. Load session in your view/middleware by calling `load_session(connection)` utility.\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\n\nfrom starsessions import CookieStore, load_session, SessionMiddleware\n\n\nasync def index_view(request):\n    await load_session(request)\n\n    session_data = request.session\n    return JSONResponse(session_data)\n\n\nsession_store = CookieStore(secret_key=\'TOP SECRET\')\n\napp = Starlette(\n    middleware=[\n        Middleware(SessionMiddleware, store=session_store, lifetime=3600 * 24 * 14),\n    ],\n    routes=[\n        Route(\'/\', index_view),\n    ]\n)\n```\n\n### Cookie security\n\nBy default, the middleware uses strict defaults.\nThe cookie lifetime is limited to the browser session and sent via HTTPS protocol only.\nYou can change these defaults by changing `cookie_https_only` and `lifetime` arguments:\n\n```python\nfrom starlette.middleware import Middleware\n\nfrom starsessions import CookieStore, SessionMiddleware\n\nsession_store = CookieStore(secret_key=\'TOP SECRET\')\n\nmiddleware = [\n    Middleware(SessionMiddleware, store=session_store, cookie_https_only=False, lifetime=3600 * 24 * 14),\n]\n```\n\nThe example above will let session usage over insecure HTTP transport and the session lifetime will be set to 14 days.\n\n### Loading session\n\nThe session data is not loaded by default. Call `load_session` to load data from the store.\n\n```python\nasync def index_view(request):\n    await load_session(request)\n    request.session[\'key\'] = \'value\'\n```\n\nHowever, if you try to access uninitialized session, `SessionNotLoaded` exception will be raised.\n\n```python\nasync def index_view(request):\n    request.session[\'key\'] = \'value\'  # raises SessionNotLoaded\n```\n\nYou can automatically load session by using `SessionAutoloadMiddleware` middleware.\n\n### Session autoload\n\nFor performance reasons session is not autoloaded by default. Sometimes it is annoying to call `load_session` too often.\nWe provide `SessionAutoloadMiddleware` to reduce amount of boilerplate code by autoloading session for you.\n\nThere are two options: always autoload or autoload for specific paths only.\nHere are examples:\n\n```python\nfrom starlette.middleware import Middleware\n\nfrom starsessions import CookieStore, SessionAutoloadMiddleware, SessionMiddleware\n\nsession_store = CookieStore(secret_key=\'TOP SECRET\')\n\n# Always autoload\n\nmiddleware = [\n    Middleware(SessionMiddleware, store=session_store),\n    Middleware(SessionAutoloadMiddleware),\n]\n\n# Autoload session for selected paths\n\nmiddleware = [\n    Middleware(SessionMiddleware, store=session_store),\n    Middleware(SessionAutoloadMiddleware, paths=[\'/admin\', \'/app\']),\n]\n\n# regex patterns also supported\nimport re\n\nadmin_rx = re.compile(\'/admin*\')\n\nmiddleware = [\n    Middleware(SessionMiddleware, store=session_store),\n    Middleware(SessionAutoloadMiddleware, paths=[admin_rx]),\n]\n```\n\n### Rolling sessions\n\nThe default behavior of `SessionMiddleware` is to expire cookie after `lifetime` seconds after it was set.\nFor example, if you create a session with `lifetime=3600` then the session will be terminated exactly in 3600 seconds.\nSometimes this may not be what you need, so we provide alternate expiration strategy - rolling sessions.\n\nWhen rolling sessions in use, the cookie expiration time will be extended by `lifetime` value on every response.\nLet\'s see how it works on example. First, on the first response you create a new session with `lifetime=3600`,\nthen user does another request and session gets extended by another 3600 seconds and so on.\nThis approach is useful when you want to have short-timed sessions but don\'t want them to interrupt in the middle of\nuser\'s operation. With rolling strategy, session cookie will be expired only after some period of user\'s inactivity.\n\nTo enable rolling strategy set `rolling=True`.\n\n```python\nfrom starlette.middleware import Middleware\nfrom starsessions import SessionMiddleware\n\nmiddleware = [\n    Middleware(SessionMiddleware, lifetime=300, rolling=True),\n]\n```\n\nThe snippet above demonstrates an example setup where session will be dropped after 300 seconds (5 minutes) of\ninactivity, but will be automatically extended by another 5 minutes while the user is online.\n\n### Cookie path\n\nYou can pass `cookie_path` argument to bind session cookie to specific URLs. For example, to activate session cookie\nonly for admin area, use `cookie_path="/admin"` middleware argument.\n\n```python\nfrom starlette.middleware import Middleware\nfrom starsessions import SessionMiddleware\n\nmiddleware = [\n    Middleware(SessionMiddleware, cookie_path=\'/admin\'),\n]\n```\n\nAll other URLs not matching value of `cookie_path` will not receive cookie thus session will be unavailable.\n\n### Cookie domain\n\nYou can also specify which hosts can receive a cookie by passing `cookie_domain` argument to the middleware.\n\n```python\nfrom starlette.middleware import Middleware\nfrom starsessions import SessionMiddleware\n\nmiddleware = [\n    Middleware(SessionMiddleware, cookie_domain=\'example.com\'),\n]\n```\n\n> Note, this makes session cookie available for subdomains too.\n> For example, when you set `cookie_domain=example.com` then session cookie will be available on subdomains\n> like `app.example.com`.\n\n### Session-only cookies\n\nIf you want session cookie to automatically remove from tbe browser when tab closes then set `lifetime` to `0`.\n> Note, this depends on browser implementation!\n\n```python\nfrom starlette.middleware import Middleware\nfrom starsessions import SessionMiddleware\n\nmiddleware = [\n    Middleware(SessionMiddleware, lifetime=0),\n]\n```\n\n## Built-in stores\n\n### Memory\n\nClass: `starsessions.InMemoryStore`\n\nSimply stores data in memory. The data is cleared after server restart. Mostly for use with unit tests.\n\n### CookieStore\n\nClass: `starsessions.CookieStore`\n\nStores session data in a signed cookie on the client.\n\n### Redis\n\nClass: `starsessions.stores.redis.RedisStore`\n\nStores session data in a Redis server. The store accepts either connection URL or an instance of `Redis`.\n\n> Requires [redis-py](https://github.com/redis/redis-py),\n> use `pip install starsessions[redis]` or `poetry add starsessions[redis]`\n\n```python\nfrom redis.asyncio.utils import from_url\n\nfrom starsessions.stores.redis import RedisStore\n\nstore = RedisStore(\'redis://localhost\')\n# or\nredis = from_url(\'redis://localhost\')\n\nstore = RedisStore(connection=redis)\n```\n\n#### Redis key prefix\n\nBy default, all keys in Redis prefixed with `starsessions.`. If you want to change this use `prefix` argument.\n\n```python\nfrom starsessions.stores.redis import RedisStore\n\nstore = RedisStore(url=\'redis://localhost\', prefix=\'my_sessions\')\n```\n\nPrefix can be a callable:\n\n```python\nfrom starsessions.stores.redis import RedisStore\n\n\ndef make_prefix(key: str) -> str:\n    return \'my_sessions_\' + key\n\n\nstore = RedisStore(url=\'redis://localhost\', prefix=make_prefix)\n```\n\n#### Key expiration\n\nThe library automatically manages key expiration, usually you have nothing to do with it.\nBut for cases when `lifetime=0` we don\'t know when the session will over, and we have to heuristically calculate TTL\notherwise the data will remain in Redis forever. At this moment, we just set 30 days TTL. You can change it by\nsetting `gc_ttl` value on the store.\n\n```python\nfrom starsessions.stores.redis import RedisStore\n\nstore = RedisStore(url=\'redis://localhost\', gc_ttl=3600)  # max 1 hour\n```\n\n## Custom store\n\nCreating new stores is quite simple. All you need is to extend `starsessions.SessionStore`\nclass and implement abstract methods.\n\nHere is an example of how we can create a memory-based session store. Note, it is important that `write` method\nreturns session ID as a string value.\n\n```python\nfrom typing import Dict\n\nfrom starsessions import SessionStore\n\n\n# instance of class which manages session persistence\n\nclass InMemoryStore(SessionStore):\n    def __init__(self):\n        self._storage = {}\n\n    async def read(self, session_id: str, lifetime: int) -> Dict:\n        """ Read session data from a data source using session_id. """\n        return self._storage.get(session_id, {})\n\n    async def write(self, session_id: str, data: Dict, lifetime: int, ttl: int) -> str:\n        """ Write session data into data source and return session id. """\n        self._storage[session_id] = data\n        return session_id\n\n    async def remove(self, session_id: str):\n        """ Remove session data. """\n        del self._storage[session_id]\n\n    async def exists(self, session_id: str) -> bool:\n        return session_id in self._storage\n```\n\n### lifetime and ttl\n\nThe `write` accepts two special arguments: `lifetime` and `ttl`.\nThe difference is that `lifetime` is a total session duration (set by the middleware)\nand `ttl` is a remaining session time. After `ttl` seconds the data can be safely deleted from the storage.\n\n> Your custom backend has to correctly handle setups when `lifetime = 0`.\nIn such cases you don\'t have exact expiration value, and you have to find a way how to extend session TTL at the storage\nside, if any.\n\n## Serializers\n\nThe library automatically serializes session data to string using JSON.\nBy default, we use `starsessions.JsonSerializer` but you can implement your own by extending `starsessions.Serializer`\nclass.\n\n```python\nimport json\nimport typing\n\nfrom starlette.middleware import Middleware\n\nfrom starsessions import Serializer, SessionMiddleware\n\n\nclass MySerializer(Serializer):\n    def serialize(self, data: typing.Any) -> bytes:\n        return json.dumps(data).encode(\'utf-8\')\n\n    def deserialize(self, data: bytes) -> typing.Dict[str, typing.Any]:\n        return json.loads(data)\n\n\nmiddleware = [\n    Middleware(SessionMiddleware, serializer=MySerializer()),\n]\n```\n\n## Session termination\n\nThe middleware will remove session data and cookie if session has no data. Use `request.session.clear` to empty data.\n\n## Regenerating session ID\n\nSometimes you need a new session ID to avoid session fixation attacks (for example, after successful signs in).\nFor that, use `starsessions.session.regenerate_session_id(connection)` utility.\n\n```python\nfrom starsessions.session import regenerate_session_id\nfrom starlette.responses import Response\n\n\ndef login(request):\n    regenerate_session_id(request)\n    return Response(\'successfully signed in\')\n```\n',
-    'author': 'alex.oleshkevich',
-    'author_email': 'alex.oleshkevich@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/alex-oleshkevich/starsessions',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8.0,<4.0.0',
-}
+![PyPI](https://img.shields.io/pypi/v/starsessions)
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/alex-oleshkevich/starsessions/Lint%20and%20test)
+![GitHub](https://img.shields.io/github/license/alex-oleshkevich/starsessions)
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/starsessions)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/starsessions)
+![GitHub Release Date](https://img.shields.io/github/release-date/alex-oleshkevich/starsessions)
 
+## Installation
+
+Install `starsessions` using PIP or poetry:
+
+```bash
+pip install starsessions
+# or
+poetry add starsessions
+```
+
+Use `redis` extra for [Redis support](#redis).
+
+## Quick start
+
+See example application in [`examples/`](examples) directory of this repository.
+
+## Usage
+
+1. Add `starsessions.SessionMiddleware` to your application to enable session support,
+2. Configure session store and pass it to the middleware,
+3. Load session in your view/middleware by calling `load_session(connection)` utility.
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+from starlette.responses import JSONResponse
+from starlette.routing import Route
+
+from starsessions import CookieStore, load_session, SessionMiddleware
+
+
+async def index_view(request):
+    await load_session(request)
+
+    session_data = request.session
+    return JSONResponse(session_data)
+
+
+session_store = CookieStore(secret_key='TOP SECRET')
+
+app = Starlette(
+    middleware=[
+        Middleware(SessionMiddleware, store=session_store, lifetime=3600 * 24 * 14),
+    ],
+    routes=[
+        Route('/', index_view),
+    ]
+)
+```
+
+### Cookie security
+
+By default, the middleware uses strict defaults.
+The cookie lifetime is limited to the browser session and sent via HTTPS protocol only.
+You can change these defaults by changing `cookie_https_only` and `lifetime` arguments:
+
+```python
+from starlette.middleware import Middleware
+
+from starsessions import CookieStore, SessionMiddleware
+
+session_store = CookieStore(secret_key='TOP SECRET')
+
+middleware = [
+    Middleware(SessionMiddleware, store=session_store, cookie_https_only=False, lifetime=3600 * 24 * 14),
+]
+```
+
+The example above will let session usage over insecure HTTP transport and the session lifetime will be set to 14 days.
+
+### Loading session
+
+The session data is not loaded by default. Call `load_session` to load data from the store.
+
+```python
+async def index_view(request):
+    await load_session(request)
+    request.session['key'] = 'value'
+```
+
+However, if you try to access uninitialized session, `SessionNotLoaded` exception will be raised.
+
+```python
+async def index_view(request):
+    request.session['key'] = 'value'  # raises SessionNotLoaded
+```
+
+You can automatically load session by using `SessionAutoloadMiddleware` middleware.
+
+### Session autoload
+
+For performance reasons session is not autoloaded by default. Sometimes it is annoying to call `load_session` too often.
+We provide `SessionAutoloadMiddleware` to reduce amount of boilerplate code by autoloading session for you.
+
+There are two options: always autoload or autoload for specific paths only.
+Here are examples:
+
+```python
+from starlette.middleware import Middleware
+
+from starsessions import CookieStore, SessionAutoloadMiddleware, SessionMiddleware
+
+session_store = CookieStore(secret_key='TOP SECRET')
+
+# Always autoload
+
+middleware = [
+    Middleware(SessionMiddleware, store=session_store),
+    Middleware(SessionAutoloadMiddleware),
+]
+
+# Autoload session for selected paths
+
+middleware = [
+    Middleware(SessionMiddleware, store=session_store),
+    Middleware(SessionAutoloadMiddleware, paths=['/admin', '/app']),
+]
+
+# regex patterns also supported
+import re
+
+admin_rx = re.compile('/admin*')
+
+middleware = [
+    Middleware(SessionMiddleware, store=session_store),
+    Middleware(SessionAutoloadMiddleware, paths=[admin_rx]),
+]
+```
+
+### Rolling sessions
+
+The default behavior of `SessionMiddleware` is to expire cookie after `lifetime` seconds after it was set.
+For example, if you create a session with `lifetime=3600` then the session will be terminated exactly in 3600 seconds.
+Sometimes this may not be what you need, so we provide alternate expiration strategy - rolling sessions.
+
+When rolling sessions in use, the cookie expiration time will be extended by `lifetime` value on every response.
+Let's see how it works on example. First, on the first response you create a new session with `lifetime=3600`,
+then user does another request and session gets extended by another 3600 seconds and so on.
+This approach is useful when you want to have short-timed sessions but don't want them to interrupt in the middle of
+user's operation. With rolling strategy, session cookie will be expired only after some period of user's inactivity.
+
+To enable rolling strategy set `rolling=True`.
+
+```python
+from starlette.middleware import Middleware
+from starsessions import SessionMiddleware
+
+middleware = [
+    Middleware(SessionMiddleware, lifetime=300, rolling=True),
+]
+```
+
+The snippet above demonstrates an example setup where session will be dropped after 300 seconds (5 minutes) of
+inactivity, but will be automatically extended by another 5 minutes while the user is online.
+
+### Cookie path
+
+You can pass `cookie_path` argument to bind session cookie to specific URLs. For example, to activate session cookie
+only for admin area, use `cookie_path="/admin"` middleware argument.
+
+```python
+from starlette.middleware import Middleware
+from starsessions import SessionMiddleware
+
+middleware = [
+    Middleware(SessionMiddleware, cookie_path='/admin'),
+]
+```
+
+All other URLs not matching value of `cookie_path` will not receive cookie thus session will be unavailable.
+
+### Cookie domain
+
+You can also specify which hosts can receive a cookie by passing `cookie_domain` argument to the middleware.
+
+```python
+from starlette.middleware import Middleware
+from starsessions import SessionMiddleware
+
+middleware = [
+    Middleware(SessionMiddleware, cookie_domain='example.com'),
+]
+```
+
+> Note, this makes session cookie available for subdomains too.
+> For example, when you set `cookie_domain=example.com` then session cookie will be available on subdomains
+> like `app.example.com`.
+
+### Session-only cookies
+
+If you want session cookie to automatically remove from tbe browser when tab closes then set `lifetime` to `0`.
+> Note, this depends on browser implementation!
+
+```python
+from starlette.middleware import Middleware
+from starsessions import SessionMiddleware
+
+middleware = [
+    Middleware(SessionMiddleware, lifetime=0),
+]
+```
+
+## Built-in stores
+
+### Memory
+
+Class: `starsessions.InMemoryStore`
+
+Simply stores data in memory. The data is cleared after server restart. Mostly for use with unit tests.
+
+### CookieStore
+
+Class: `starsessions.CookieStore`
+
+Stores session data in a signed cookie on the client.
+
+### Redis
+
+Class: `starsessions.stores.redis.RedisStore`
+
+Stores session data in a Redis server. The store accepts either connection URL or an instance of `Redis`.
+
+> Requires [redis-py](https://github.com/redis/redis-py),
+> use `pip install starsessions[redis]` or `poetry add starsessions[redis]`
+
+```python
+from redis.asyncio.utils import from_url
+
+from starsessions.stores.redis import RedisStore
+
+store = RedisStore('redis://localhost')
+# or
+redis = from_url('redis://localhost')
+
+store = RedisStore(connection=redis)
+```
+
+#### Redis key prefix
+
+By default, all keys in Redis prefixed with `starsessions.`. If you want to change this use `prefix` argument.
+
+```python
+from starsessions.stores.redis import RedisStore
+
+store = RedisStore(url='redis://localhost', prefix='my_sessions')
+```
+
+Prefix can be a callable:
+
+```python
+from starsessions.stores.redis import RedisStore
+
+
+def make_prefix(key: str) -> str:
+    return 'my_sessions_' + key
+
+
+store = RedisStore(url='redis://localhost', prefix=make_prefix)
+```
+
+#### Key expiration
+
+The library automatically manages key expiration, usually you have nothing to do with it.
+But for cases when `lifetime=0` we don't know when the session will over, and we have to heuristically calculate TTL
+otherwise the data will remain in Redis forever. At this moment, we just set 30 days TTL. You can change it by
+setting `gc_ttl` value on the store.
+
+```python
+from starsessions.stores.redis import RedisStore
+
+store = RedisStore(url='redis://localhost', gc_ttl=3600)  # max 1 hour
+```
+
+## Custom store
+
+Creating new stores is quite simple. All you need is to extend `starsessions.SessionStore`
+class and implement abstract methods.
+
+Here is an example of how we can create a memory-based session store. Note, it is important that `write` method
+returns session ID as a string value.
+
+```python
+from typing import Dict
+
+from starsessions import SessionStore
+
+
+# instance of class which manages session persistence
+
+class InMemoryStore(SessionStore):
+    def __init__(self):
+        self._storage = {}
+
+    async def read(self, session_id: str, lifetime: int) -> Dict:
+        """ Read session data from a data source using session_id. """
+        return self._storage.get(session_id, {})
+
+    async def write(self, session_id: str, data: Dict, lifetime: int, ttl: int) -> str:
+        """ Write session data into data source and return session id. """
+        self._storage[session_id] = data
+        return session_id
+
+    async def remove(self, session_id: str):
+        """ Remove session data. """
+        del self._storage[session_id]
+
+    async def exists(self, session_id: str) -> bool:
+        return session_id in self._storage
+```
+
+### lifetime and ttl
+
+The `write` accepts two special arguments: `lifetime` and `ttl`.
+The difference is that `lifetime` is a total session duration (set by the middleware)
+and `ttl` is a remaining session time. After `ttl` seconds the data can be safely deleted from the storage.
+
+> Your custom backend has to correctly handle setups when `lifetime = 0`.
+In such cases you don't have exact expiration value, and you have to find a way how to extend session TTL at the storage
+side, if any.
+
+## Serializers
+
+The library automatically serializes session data to string using JSON.
+By default, we use `starsessions.JsonSerializer` but you can implement your own by extending `starsessions.Serializer`
+class.
+
+```python
+import json
+import typing
+
+from starlette.middleware import Middleware
+
+from starsessions import Serializer, SessionMiddleware
+
+
+class MySerializer(Serializer):
+    def serialize(self, data: typing.Any) -> bytes:
+        return json.dumps(data).encode('utf-8')
+
+    def deserialize(self, data: bytes) -> typing.Dict[str, typing.Any]:
+        return json.loads(data)
+
+
+middleware = [
+    Middleware(SessionMiddleware, serializer=MySerializer()),
+]
+```
+
+## Session termination
+
+The middleware will remove session data and cookie if session has no data. Use `request.session.clear` to empty data.
+
+## Regenerating session ID
+
+Sometimes you need a new session ID to avoid session fixation attacks (for example, after successful signs in).
+For that, use `starsessions.session.regenerate_session_id(connection)` utility.
+
+```python
+from starsessions.session import regenerate_session_id
+from starlette.responses import Response
+
+
+def login(request):
+    regenerate_session_id(request)
+    return Response('successfully signed in')
+```
 
-setup(**setup_kwargs)
```

