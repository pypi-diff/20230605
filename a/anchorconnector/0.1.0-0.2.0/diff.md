# Comparing `tmp/anchorconnector-0.1.0.tar.gz` & `tmp/anchorconnector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchorconnector-0.1.0.tar", last modified: Tue May  2 11:23:45 2023, max compression
+gzip compressed data, was "anchorconnector-0.2.0.tar", last modified: Mon Jun  5 14:10:45 2023, max compression
```

## Comparing `anchorconnector-0.1.0.tar` & `anchorconnector-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-05-02 11:23:45.391338 anchorconnector-0.1.0/
--rw-r--r--   0 mendler    (501) staff       (20)     1085 2023-04-25 10:18:29.000000 anchorconnector-0.1.0/LICENSE
--rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-05-02 11:23:45.391186 anchorconnector-0.1.0/PKG-INFO
--rw-r--r--   0 mendler    (501) staff       (20)     3328 2023-04-28 18:54:28.000000 anchorconnector-0.1.0/README.md
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-05-02 11:23:45.389402 anchorconnector-0.1.0/anchorconnector/
--rw-r--r--   0 mendler    (501) staff       (20)      202 2023-04-28 14:11:24.000000 anchorconnector-0.1.0/anchorconnector/__init__.py
--rw-r--r--   0 mendler    (501) staff       (20)     4083 2023-05-02 10:43:43.000000 anchorconnector-0.1.0/anchorconnector/__main__.py
--rw-r--r--   0 mendler    (501) staff       (20)    11124 2023-04-28 18:56:50.000000 anchorconnector-0.1.0/anchorconnector/connector.py
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-05-02 11:23:45.390951 anchorconnector-0.1.0/anchorconnector.egg-info/
--rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-05-02 11:23:45.000000 anchorconnector-0.1.0/anchorconnector.egg-info/PKG-INFO
--rw-r--r--   0 mendler    (501) staff       (20)      347 2023-05-02 11:23:45.000000 anchorconnector-0.1.0/anchorconnector.egg-info/SOURCES.txt
--rw-r--r--   0 mendler    (501) staff       (20)        1 2023-05-02 11:23:45.000000 anchorconnector-0.1.0/anchorconnector.egg-info/dependency_links.txt
--rw-r--r--   0 mendler    (501) staff       (20)       66 2023-05-02 11:23:45.000000 anchorconnector-0.1.0/anchorconnector.egg-info/entry_points.txt
--rw-r--r--   0 mendler    (501) staff       (20)       32 2023-05-02 11:23:45.000000 anchorconnector-0.1.0/anchorconnector.egg-info/requires.txt
--rw-r--r--   0 mendler    (501) staff       (20)       16 2023-05-02 11:23:45.000000 anchorconnector-0.1.0/anchorconnector.egg-info/top_level.txt
--rw-r--r--   0 mendler    (501) staff       (20)       38 2023-05-02 11:23:45.391377 anchorconnector-0.1.0/setup.cfg
--rw-r--r--   0 mendler    (501) staff       (20)      552 2023-04-28 14:11:24.000000 anchorconnector-0.1.0/setup.py
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 14:10:45.132185 anchorconnector-0.2.0/
+-rw-r--r--   0 mendler    (501) staff       (20)     1085 2023-04-25 10:18:29.000000 anchorconnector-0.2.0/LICENSE
+-rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-06-05 14:10:45.132063 anchorconnector-0.2.0/PKG-INFO
+-rw-r--r--   0 mendler    (501) staff       (20)     3328 2023-04-28 18:54:28.000000 anchorconnector-0.2.0/README.md
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 14:10:45.131295 anchorconnector-0.2.0/anchorconnector/
+-rw-r--r--   0 mendler    (501) staff       (20)      202 2023-04-28 14:11:24.000000 anchorconnector-0.2.0/anchorconnector/__init__.py
+-rw-r--r--   0 mendler    (501) staff       (20)     4073 2023-06-05 14:07:47.000000 anchorconnector-0.2.0/anchorconnector/__main__.py
+-rw-r--r--   0 mendler    (501) staff       (20)     9952 2023-06-05 14:08:01.000000 anchorconnector-0.2.0/anchorconnector/connector.py
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 14:10:45.131913 anchorconnector-0.2.0/anchorconnector.egg-info/
+-rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/PKG-INFO
+-rw-r--r--   0 mendler    (501) staff       (20)      347 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 mendler    (501) staff       (20)        1 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       66 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/entry_points.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       32 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/requires.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       16 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/top_level.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       38 2023-06-05 14:10:45.132219 anchorconnector-0.2.0/setup.cfg
+-rw-r--r--   0 mendler    (501) staff       (20)      552 2023-06-05 14:07:19.000000 anchorconnector-0.2.0/setup.py
```

### Comparing `anchorconnector-0.1.0/LICENSE` & `anchorconnector-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anchorconnector-0.1.0/PKG-INFO` & `anchorconnector-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchorconnector
-Version: 0.1.0
+Version: 0.2.0
 Summary: Anchor Connector for Podcast Data
 Author: Open Podcast
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Anchor Connector
```

### Comparing `anchorconnector-0.1.0/README.md` & `anchorconnector-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `anchorconnector-0.1.0/anchorconnector/__main__.py` & `anchorconnector-0.2.0/anchorconnector/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     plays_by_gender = connector.plays_by_gender(start, end)
     logger.info(
         "Plays by Gender = {}",
         json.dumps(plays_by_gender, indent=4),
     )
 
-    plays_by_geo = connector.plays_by_geo(start, end)
+    plays_by_geo = connector.plays_by_geo()
     logger.info(
         "Plays by Geo = {}",
         json.dumps(plays_by_geo, indent=4),
     )
 
     unique_listeners = connector.unique_listeners()
     logger.info("Podcast Unique Listeners = {}", json.dumps(unique_listeners, indent=4))
```

### Comparing `anchorconnector-0.1.0/anchorconnector/connector.py` & `anchorconnector-0.2.0/anchorconnector/connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,23 +19,15 @@
             base_url (str): Base URL for the API.
             webstation_id (str): Anchor Podcast ID for the API
             anchorpw_s (str): Anchor API token (from anchorpw_s cookie)
         """
 
         self.base_url = base_url
         self.webstation_id = webstation_id
-        self.cookies = {
-            "anchorpw_s": anchorpw_s,
-            "reduxPersist%3AlocalStorage": "{%22lastPlayedSegment%22:{}%2C%22playbackSpeed%22:1}",
-            "reduxPersistIndex": "[%22reduxPersist:localStorage%22%2C%22reduxPersist:tutorial%22%2C%22reduxPersist:voiceMessageCreationModalScreen%22]",
-            "__stripe_mid": "4e63f9ff-86bf-4445-b554-a6a62b2c80d84b2114",
-            "__stripe_sid": "00752db1-345e-4967-b550-67db82320dd360d7ac",
-            "reduxPersist%3Atutorial": "{%22dismissedBanners%22:{}%2C%22dismissedTutorialPopups%22:{}%2C%22isOptedOutOfDistribution%22:false%2C%22isShortMetadataFormModalShowing%22:false}",
-            "reduxPersist%3AvoiceMessageCreationModalScreen": "{%22voiceMessageRecording%22:null%2C%22isVoiceMessageRehydrating%22:false%2C%22isVoiceMessagePlaying%22:false%2C%22isShowingRecordAgainConfirmationOverlay%22:false%2C%22isShowingExitConfirmationOverlay%22:false%2C%22loginEmail%22:%22%22%2C%22loginPassword%22:%22%22%2C%22signupName%22:%22%22%2C%22signupEmail%22:%22%22%2C%22signupPassword%22:%22%22%2C%22currentUserEmail%22:null%2C%22captcha%22:null%2C%22email%22:%22%22%2C%22voiceMessageTitle%22:%22%22%2C%22isLoading%22:false%2C%22isNewUser%22:false%2C%22isError%22:false}",
-        }
+        self.cookies = {"anchorpw_s": anchorpw_s}
         self._auth_lock = RLock()
 
     def _build_url(self, *args) -> str:
         return f"{self.base_url}/{'/'.join(args)}"
 
     def _date_params(self, start: datetime, end: datetime) -> Dict[str, str]:
         return {
@@ -224,22 +216,23 @@
             "station",
             format(f"webStationId:{self.webstation_id}"),
             "playsByGender",
         )
         params = self._date_params(start, end)
         return self._request(url, params)
 
-    def plays_by_geo(self, limit: int, result_geo: str) -> dict:
+    def plays_by_geo(self, limit: int = 200) -> dict:
         url = self._build_url(
             "analytics",
             "station",
             format(f"webStationId:{self.webstation_id}"),
             "playsByGeo",
         )
-        params = {"limit": str(limit), "resultGeo": result_geo}
+        # Only `resultGeo=geo2` returns data.
+        params = {"limit": str(limit), "resultGeo": "geo2"}
         return self._request(url, params)
 
     def podcast_episode(self) -> dict:
         """
         Get the podcast episodes for the webstation.
         This is an outlier in the API, as it's not a sub-endpoint of the station.
         The URL is hardcoded here, as it doesn't follow the usual pattern and
```

### Comparing `anchorconnector-0.1.0/anchorconnector.egg-info/PKG-INFO` & `anchorconnector-0.2.0/anchorconnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchorconnector
-Version: 0.1.0
+Version: 0.2.0
 Summary: Anchor Connector for Podcast Data
 Author: Open Podcast
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Anchor Connector
```

### Comparing `anchorconnector-0.1.0/setup.py` & `anchorconnector-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="anchorconnector",
     packages=find_packages(include=["anchorconnector"]),
-    version="0.1.0",
+    version="0.2.0",
     description="Anchor Connector for Podcast Data",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Open Podcast",
     license="MIT",
     entry_points={
         "console_scripts": [
```

