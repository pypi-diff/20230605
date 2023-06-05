# Comparing `tmp/bayes_lol_client-1.0.1.tar.gz` & `tmp/bayes_lol_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayes_lol_client-1.0.1.tar", max compression
+gzip compressed data, was "bayes_lol_client-1.0.2.tar", max compression
```

## Comparing `bayes_lol_client-1.0.1.tar` & `bayes_lol_client-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      221 2022-12-26 09:09:13.780633 bayes_lol_client-1.0.1/bayes_lol_client/__init__.py
--rw-r--r--   0        0        0     8877 2022-12-26 09:08:44.443260 bayes_lol_client-1.0.1/bayes_lol_client/api.py
--rw-r--r--   0        0        0     6458 2022-12-26 19:05:37.676464 bayes_lol_client-1.0.1/bayes_lol_client/emh.py
--rw-r--r--   0        0        0      567 2022-12-26 04:47:33.588019 bayes_lol_client-1.0.1/bayes_lol_client/errors.py
--rw-r--r--   0        0        0     5158 2022-12-26 18:47:15.120987 bayes_lol_client-1.0.1/bayes_lol_client/historic.py
--rw-r--r--   0        0        0      990 2022-12-26 07:23:47.939276 bayes_lol_client-1.0.1/bayes_lol_client/sleep.py
--rw-r--r--   0        0        0     1866 2022-12-26 18:43:08.156574 bayes_lol_client-1.0.1/bayes_lol_client/utils.py
--rw-r--r--   0        0        0    35821 2022-12-24 02:50:06.266967 bayes_lol_client-1.0.1/LICENSE
--rw-r--r--   0        0        0      486 2022-12-26 09:09:17.067328 bayes_lol_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      649 2022-12-24 03:59:42.326926 bayes_lol_client-1.0.1/README.md
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.1/setup.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      221 2023-06-05 01:27:21.470972 bayes_lol_client-1.0.2/bayes_lol_client/__init__.py
+-rw-r--r--   0        0        0     8917 2023-06-05 01:29:40.964470 bayes_lol_client-1.0.2/bayes_lol_client/api.py
+-rw-r--r--   0        0        0     6521 2023-06-05 01:29:44.616481 bayes_lol_client-1.0.2/bayes_lol_client/emh.py
+-rw-r--r--   0        0        0      567 2023-06-05 01:27:21.472972 bayes_lol_client-1.0.2/bayes_lol_client/errors.py
+-rw-r--r--   0        0        0     5158 2023-06-05 01:27:21.473973 bayes_lol_client-1.0.2/bayes_lol_client/historic.py
+-rw-r--r--   0        0        0      990 2023-06-05 01:27:21.473973 bayes_lol_client-1.0.2/bayes_lol_client/sleep.py
+-rw-r--r--   0        0        0     1866 2023-06-05 01:27:21.474973 bayes_lol_client-1.0.2/bayes_lol_client/utils.py
+-rw-r--r--   0        0        0    35821 2023-06-05 01:27:21.469971 bayes_lol_client-1.0.2/LICENSE
+-rw-r--r--   0        0        0      466 2023-06-05 01:27:43.601824 bayes_lol_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-06-05 01:27:21.469971 bayes_lol_client-1.0.2/README.md
+-rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.2/setup.py
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.2/PKG-INFO
```

### Comparing `bayes_lol_client-1.0.1/bayes_lol_client/api.py` & `bayes_lol_client-1.0.2/bayes_lol_client/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,68 +141,69 @@
         )
 
     def sleep_and_retry(
         self,
         sleeper: Sleeper,
         method: str,
         service: str,
+        endpoint: str,
         data: dict = None,
         exception: Exception = None,
         sleep_time: int = None,
     ):
         sleeper.sleep(exception, sleep_time)
         return self.do_api_call(
-            method, service, data, ensure_login=False, sleeper=sleeper
+            method,
+            service,
+            data,
+            ensure_login=False,
+            sleeper=sleeper,
+            endpoint=endpoint,
         )
 
     def handle_response(
         self,
         sleeper: Sleeper,
         response: requests.Response,
         method: str,
         service: str,
         allow_retry: bool,
+        endpoint: str,
         data: dict = None,
     ):
         if response.status_code == 401:
-            if not allow_retry:
-                raise UnauthorizedError(response.status_code)
-            return self.sleep_and_retry(
-                method=method,
-                sleeper=sleeper,
-                service=service,
-                data=data,
-                exception=self.make_http_exception_from_status_code(response),
-            )
+            raise UnauthorizedError(response.status_code)
         elif response.status_code == 429:
             if not allow_retry or not self.wait_on_ratelimit:
                 raise TooManyRequests(response.status_code)
             if "x-rate-limit-retry-after-seconds" in response.headers:
                 sleep_time = int(response.headers["x-rate-limit-retry-after-seconds"])
             else:
                 sleep_time = None
             return self.sleep_and_retry(
                 method=method,
                 sleeper=sleeper,
                 service=service,
                 data=data,
                 exception=self.make_http_exception_from_status_code(response),
                 sleep_time=sleep_time,
+                endpoint=endpoint,
             )
         elif response.status_code == 404:
             raise NotFoundError(response.status_code)
         elif response.status_code >= 500:
             if not allow_retry:
                 raise ServerError(response.status_code)
             return self.sleep_and_retry(
                 method=method,
                 sleeper=sleeper,
                 service=service,
                 data=data,
                 exception=self.make_http_exception_from_status_code(response),
+                endpoint=endpoint,
             )
         elif 499 >= response.status_code >= 400:
             raise ClientError(response.status_code)
         response.raise_for_status()
         return response.json()
 
     def do_api_call(
@@ -235,18 +236,24 @@
             ConnectTimeout,
             Timeout,
             ReadTimeout,
         ) as e:
             if not allow_retry:
                 raise e
             return self.sleep_and_retry(
-                method=method, sleeper=sleeper, service=service, data=data, exception=e
+                method=method,
+                sleeper=sleeper,
+                service=service,
+                data=data,
+                exception=e,
+                endpoint=endpoint,
             )
 
         return self.handle_response(
             method=method,
             service=service,
             data=data,
             sleeper=sleeper,
             response=response,
             allow_retry=allow_retry,
+            endpoint=endpoint,
         )
```

### Comparing `bayes_lol_client-1.0.1/bayes_lol_client/emh.py` & `bayes_lol_client-1.0.2/bayes_lol_client/emh.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,94 +5,102 @@
 from requests import Response
 from datetime import datetime
 
 
 class BayesEMH(object):
     """
     This class makes requests to the /emh/v1 endpoint in the Bayes API.
-    Useful to get summary/details/replay files for professional games.
+    Useful to get summary/details/replay files for professional games
     """
+
     endpoint = "https://lolesports-api.bayesesports.com/emh/v1/"
     DEFAULT_MAX_PAGE_SIZE = 500
 
     def __init__(
         self,
-        username: str = None,
-        password: str = None,
-        wait_on_ratelimit: bool = True,
-        retry_interval: int = 2,
-        max_retries: int = 5,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        wait_on_ratelimit: Optional[bool] = True,
+        retry_interval: Optional[int] = 2,
+        max_retries: Optional[int] = 5,
     ):
         self.api = BayesAPIClient(
             endpoint=self.endpoint,
             username=username,
             password=password,
             wait_on_ratelimit=wait_on_ratelimit,
             retry_interval=retry_interval,
             max_retries=max_retries,
         )
 
     def get_game_summary(self, platform_game_id: str) -> dict:
         """
         Returns the game summary as a json file
+
         :param platform_game_id: A Riot esports game ID
         :return: The game summary as a json file
         """
         return self.get_asset(platform_game_id, "GAMH_SUMMARY").json()
 
     def get_game_details(self, platform_game_id: str) -> dict:
         """
         Returns the game details (timeline) as a json file
+
         :param platform_game_id: A Riot esports game ID
         :return: The game details as a json file
         """
         return self.get_asset(platform_game_id, "GAMH_DETAILS").json()
 
-    def get_game_replay(self, platform_game_id: str) -> Response.content:
+    def get_game_replay(self, platform_game_id: str) -> bytes:
         """
         Returns a replay file as bytes which can later be saved locally
+
         :param platform_game_id: A Riot esports game ID
         :return: Replay file as bytes
         """
         return self.get_asset(platform_game_id, "ROFL_REPLAY").content
 
     def get_asset(self, platform_game_id: str, asset_name: str) -> Response:
         """
         Gets a generic asset for a game by its name (SUMMARY, DETAILS, or REPLAY)
+
         :param platform_game_id: A Riot esports game ID
         :param asset_name: The name of the asset to return (GAMH_SUMMARY, GAMH_DETAILS, ROFL_REPLAY)
         :return: An asset for a specific game
         """
         asset_url = self.api.do_api_call(
             "GET",
             f"games/{platform_game_id}/download",
             data={"type": asset_name},
         )["url"]
         return utils.download_game_asset(self.api, asset_url)
 
     def get_game_data(self, platform_game_id: str) -> tuple:
         """
         Returns both the game summary and details as a tuple
+
         :param platform_game_id: A Riot esports game ID
         :return: Game summary and details as a tuple
         """
         summary = self.get_game_summary(platform_game_id)
         details = self.get_game_details(platform_game_id)
         return summary, details
 
-    def get_tags_list(self) -> list:
+    def get_tags_list(self) -> List[str]:
         """
         Gets all the available game tags in EMH
+
         :return: A list of game tags
         """
         return self.api.do_api_call("GET", "tags")
 
     def get_games_info(self, platform_game_ids: Union[str, list]) -> dict:
         """
         Gets basic metadata for a list of games
+
         :param platform_game_ids: Riot esports game IDs as a list or a comma-separated string
         :return: A dict containing each platform game ID as a key
         """
         if isinstance(platform_game_ids, str):
             platform_game_ids = platform_game_ids.split(",")
         ret = {}
         for platform_game_id in platform_game_ids:
@@ -102,14 +110,15 @@
             except NotFoundError:
                 ret[platform_game_id] = {"success": False}
         return ret
 
     def get_game_info(self, platform_game_id: str) -> dict:
         """
         Gets basic metadata for a specific game
+
         :param platform_game_id: A riot esports game ID
         :return: Metadata for a game as a dict
         """
         return self.api.do_api_call("GET", f"games/{platform_game_id}")
 
     def get_games_list(
         self,
@@ -121,19 +130,20 @@
         team1: Optional[str] = None,
         team2: Optional[str] = None,
         max_page_size: Optional[int] = None,
     ) -> list:
         """
         Gets a list of games which can be filtered using the different function arguments
         If no limit is specified, the function will make multiple requests and return every matched game
+
         :param tags: Only return games containing these tags, as a comma-separated string, or a list
-        :param from_timestamp: Only return games after this moment, can be a unix epoch timestamp as int or float,
-        or a datetime object
-        :param to_timestamp: Only return games before this moment, can be a unix epoch timestamp as int or float,
-        or a datetime object
+        :param from_timestamp: Only return games after this moment, can be a unix epoch timestamp as int or float, or a
+        datetime object
+        :param to_timestamp: Only return games before this moment, can be a unix epoch timestamp as int or float, or a
+        datetime object
         :param limit: Maximum number of games to return
         :param team1: Only return games where this team played, this should be the team tricode
         :param team2: Only return games where this team and team1 played, this should be the team tricode
         :param max_page_size: Maximum size for each request, this is only useful for tweaking performance
         :return: A dict of games with the ID as a key and metadata for each one
         """
         if max_page_size is None:
```

### Comparing `bayes_lol_client-1.0.1/bayes_lol_client/errors.py` & `bayes_lol_client-1.0.2/bayes_lol_client/errors.py`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.1/bayes_lol_client/historic.py` & `bayes_lol_client-1.0.2/bayes_lol_client/historic.py`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.1/bayes_lol_client/sleep.py` & `bayes_lol_client-1.0.2/bayes_lol_client/sleep.py`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.1/bayes_lol_client/utils.py` & `bayes_lol_client-1.0.2/bayes_lol_client/utils.py`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.1/LICENSE` & `bayes_lol_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.1/README.md` & `bayes_lol_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.1/setup.py` & `bayes_lol_client-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['bayes_lol_client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['backoff>=2.2.1,<3.0.0', 'pytz>=2022.7,<2023.0', 'requests>=2.28.1,<3.0.0']
+['pytz>=2022.7,<2023.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bayes-lol-client',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Wrapper for Bayes League of Legends API',
     'long_description': '# Bayes LoL Client\n\nThis library is used to make queries to the Bayes EMH API, which provides data for League of Legends esports games.\n\n## Install\n```\npip install bayes_lol_client\n```\n\nIf you wish to install the latest development version:\n```\npip install -U git+https://github.com/arbolitoloco1/bayes_lol_client\n```\n\n## Bayes Credentials\nIn order to use the Bayes API, you must have login credentials, which will be prompted the first time you use the library.\nThese will be stored in a file in your user config path.\n\n## EMH Docs\nThe full documentation to use EMH can be found [here](https://docs.bayesesports.com/api/emh_riot)',
     'author': 'Santiago Kozak',
     'author_email': 'kozaksantiago@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/arbolitoloco1/bayes_lol_client',
```

### Comparing `bayes_lol_client-1.0.1/PKG-INFO` & `bayes_lol_client-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: bayes-lol-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper for Bayes League of Legends API
 Home-page: https://github.com/arbolitoloco1/bayes_lol_client
 License: GPL-3.0-or-later
 Author: Santiago Kozak
 Author-email: kozaksantiago@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: pytz (>=2022.7,<2023.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Bayes LoL Client
 
 This library is used to make queries to the Bayes EMH API, which provides data for League of Legends esports games.
```

