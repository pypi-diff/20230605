# Comparing `tmp/anchorconnector-0.2.0.tar.gz` & `tmp/anchorconnector-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchorconnector-0.2.0.tar", last modified: Mon Jun  5 14:10:45 2023, max compression
+gzip compressed data, was "anchorconnector-0.3.0.tar", last modified: Mon Jun  5 18:33:22 2023, max compression
```

## Comparing `anchorconnector-0.2.0.tar` & `anchorconnector-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 14:10:45.132185 anchorconnector-0.2.0/
--rw-r--r--   0 mendler    (501) staff       (20)     1085 2023-04-25 10:18:29.000000 anchorconnector-0.2.0/LICENSE
--rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-06-05 14:10:45.132063 anchorconnector-0.2.0/PKG-INFO
--rw-r--r--   0 mendler    (501) staff       (20)     3328 2023-04-28 18:54:28.000000 anchorconnector-0.2.0/README.md
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 14:10:45.131295 anchorconnector-0.2.0/anchorconnector/
--rw-r--r--   0 mendler    (501) staff       (20)      202 2023-04-28 14:11:24.000000 anchorconnector-0.2.0/anchorconnector/__init__.py
--rw-r--r--   0 mendler    (501) staff       (20)     4073 2023-06-05 14:07:47.000000 anchorconnector-0.2.0/anchorconnector/__main__.py
--rw-r--r--   0 mendler    (501) staff       (20)     9952 2023-06-05 14:08:01.000000 anchorconnector-0.2.0/anchorconnector/connector.py
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 14:10:45.131913 anchorconnector-0.2.0/anchorconnector.egg-info/
--rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/PKG-INFO
--rw-r--r--   0 mendler    (501) staff       (20)      347 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/SOURCES.txt
--rw-r--r--   0 mendler    (501) staff       (20)        1 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/dependency_links.txt
--rw-r--r--   0 mendler    (501) staff       (20)       66 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/entry_points.txt
--rw-r--r--   0 mendler    (501) staff       (20)       32 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/requires.txt
--rw-r--r--   0 mendler    (501) staff       (20)       16 2023-06-05 14:10:45.000000 anchorconnector-0.2.0/anchorconnector.egg-info/top_level.txt
--rw-r--r--   0 mendler    (501) staff       (20)       38 2023-06-05 14:10:45.132219 anchorconnector-0.2.0/setup.cfg
--rw-r--r--   0 mendler    (501) staff       (20)      552 2023-06-05 14:07:19.000000 anchorconnector-0.2.0/setup.py
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 18:33:22.720263 anchorconnector-0.3.0/
+-rw-r--r--   0 mendler    (501) staff       (20)     1085 2023-04-25 10:18:29.000000 anchorconnector-0.3.0/LICENSE
+-rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-06-05 18:33:22.720141 anchorconnector-0.3.0/PKG-INFO
+-rw-r--r--   0 mendler    (501) staff       (20)     3328 2023-04-28 18:54:28.000000 anchorconnector-0.3.0/README.md
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 18:33:22.718449 anchorconnector-0.3.0/anchorconnector/
+-rw-r--r--   0 mendler    (501) staff       (20)      202 2023-04-28 14:11:24.000000 anchorconnector-0.3.0/anchorconnector/__init__.py
+-rw-r--r--   0 mendler    (501) staff       (20)     4555 2023-06-05 18:32:27.000000 anchorconnector-0.3.0/anchorconnector/__main__.py
+-rw-r--r--   0 mendler    (501) staff       (20)    10492 2023-06-05 18:18:51.000000 anchorconnector-0.3.0/anchorconnector/connector.py
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-06-05 18:33:22.719884 anchorconnector-0.3.0/anchorconnector.egg-info/
+-rw-r--r--   0 mendler    (501) staff       (20)     3527 2023-06-05 18:33:22.000000 anchorconnector-0.3.0/anchorconnector.egg-info/PKG-INFO
+-rw-r--r--   0 mendler    (501) staff       (20)      347 2023-06-05 18:33:22.000000 anchorconnector-0.3.0/anchorconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 mendler    (501) staff       (20)        1 2023-06-05 18:33:22.000000 anchorconnector-0.3.0/anchorconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       66 2023-06-05 18:33:22.000000 anchorconnector-0.3.0/anchorconnector.egg-info/entry_points.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       32 2023-06-05 18:33:22.000000 anchorconnector-0.3.0/anchorconnector.egg-info/requires.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       16 2023-06-05 18:33:22.000000 anchorconnector-0.3.0/anchorconnector.egg-info/top_level.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       38 2023-06-05 18:33:22.720467 anchorconnector-0.3.0/setup.cfg
+-rw-r--r--   0 mendler    (501) staff       (20)      552 2023-06-05 18:33:11.000000 anchorconnector-0.3.0/setup.py
```

### Comparing `anchorconnector-0.2.0/LICENSE` & `anchorconnector-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anchorconnector-0.2.0/PKG-INFO` & `anchorconnector-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchorconnector
-Version: 0.2.0
+Version: 0.3.0
 Summary: Anchor Connector for Podcast Data
 Author: Open Podcast
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Anchor Connector
```

### Comparing `anchorconnector-0.2.0/README.md` & `anchorconnector-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `anchorconnector-0.2.0/anchorconnector/__main__.py` & `anchorconnector-0.3.0/anchorconnector/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,26 @@
 
     plays_by_geo = connector.plays_by_geo()
     logger.info(
         "Plays by Geo = {}",
         json.dumps(plays_by_geo, indent=4),
     )
 
+    # If the list of countries is not empty, get the first country in the list
+    if plays_by_geo["data"]["rows"]:
+        # Get the first entry in the list of plays by geo
+        country = plays_by_geo["data"]["rows"][0][0]
+
+        # Now use the geo to get the plays by geo on a city level
+        plays_by_geo_city = connector.plays_by_geo_city(country)
+        logger.info(
+            "Plays by Geo City = {}",
+            json.dumps(plays_by_geo_city, indent=4),
+        )
+
     unique_listeners = connector.unique_listeners()
     logger.info("Podcast Unique Listeners = {}", json.dumps(unique_listeners, indent=4))
 
     audience_size = connector.audience_size()
     logger.info("Podcast Audience Size = {}", json.dumps(audience_size, indent=4))
 
     total_plays_by_episode = connector.total_plays_by_episode()
```

### Comparing `anchorconnector-0.2.0/anchorconnector/connector.py` & `anchorconnector-0.3.0/anchorconnector/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,24 +217,40 @@
             format(f"webStationId:{self.webstation_id}"),
             "playsByGender",
         )
         params = self._date_params(start, end)
         return self._request(url, params)
 
     def plays_by_geo(self, limit: int = 200) -> dict:
+        """
+        Get the number of plays by country for the webstation.
+        """
         url = self._build_url(
             "analytics",
             "station",
             format(f"webStationId:{self.webstation_id}"),
             "playsByGeo",
         )
-        # Only `resultGeo=geo2` returns data.
+        # `resultGeo=geo2` returns country data.
         params = {"limit": str(limit), "resultGeo": "geo2"}
         return self._request(url, params)
 
+    def plays_by_geo_city(self, country: str, limit: int = 200) -> dict:
+        """
+        Get the number of plays by city for the webstation.
+        """
+        url = self._build_url(
+            "analytics",
+            "station",
+            format(f"webStationId:{self.webstation_id}"),
+            "playsByGeo",
+        )
+        params = {"limit": str(limit), "resultGeo": "geo3", "geo2": country}
+        return self._request(url, params)
+
     def podcast_episode(self) -> dict:
         """
         Get the podcast episodes for the webstation.
         This is an outlier in the API, as it's not a sub-endpoint of the station.
         The URL is hardcoded here, as it doesn't follow the usual pattern and
         is only used once.
         """
```

### Comparing `anchorconnector-0.2.0/anchorconnector.egg-info/PKG-INFO` & `anchorconnector-0.3.0/anchorconnector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchorconnector
-Version: 0.2.0
+Version: 0.3.0
 Summary: Anchor Connector for Podcast Data
 Author: Open Podcast
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Anchor Connector
```

### Comparing `anchorconnector-0.2.0/setup.py` & `anchorconnector-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="anchorconnector",
     packages=find_packages(include=["anchorconnector"]),
-    version="0.2.0",
+    version="0.3.0",
     description="Anchor Connector for Podcast Data",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Open Podcast",
     license="MIT",
     entry_points={
         "console_scripts": [
```

