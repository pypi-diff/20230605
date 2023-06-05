# Comparing `tmp/pydash2hls-2.1.2.tar.gz` & `tmp/pydash2hls-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash2hls-2.1.2.tar", last modified: Sun Jun  4 14:12:12 2023, max compression
+gzip compressed data, was "pydash2hls-2.1.3.tar", last modified: Mon Jun  5 17:21:50 2023, max compression
```

## Comparing `pydash2hls-2.1.2.tar` & `pydash2hls-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:12:12.689725 pydash2hls-2.1.2/
--rw-rw-rw-   0        0        0    35823 2023-06-03 12:20:09.000000 pydash2hls-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     3387 2023-06-04 14:12:12.688723 pydash2hls-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2461 2023-06-04 14:04:17.000000 pydash2hls-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 14:12:12.669157 pydash2hls-2.1.2/pydash2hls/
--rw-rw-rw-   0        0        0       51 2023-06-04 14:10:39.000000 pydash2hls-2.1.2/pydash2hls/__init__.py
--rw-rw-rw-   0        0        0     7234 2023-06-04 11:59:35.000000 pydash2hls-2.1.2/pydash2hls/converter.py
--rw-rw-rw-   0        0        0      469 2023-06-03 13:17:40.000000 pydash2hls-2.1.2/pydash2hls/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:12:12.687732 pydash2hls-2.1.2/pydash2hls.egg-info/
--rw-rw-rw-   0        0        0     3387 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 14:12:12.689725 pydash2hls-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-06-04 14:10:39.000000 pydash2hls-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:21:50.440164 pydash2hls-2.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-06-05 16:27:43.000000 pydash2hls-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3385 2023-06-05 17:21:50.439171 pydash2hls-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2459 2023-06-05 16:27:43.000000 pydash2hls-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 17:21:50.421283 pydash2hls-2.1.3/pydash2hls/
+-rw-rw-rw-   0        0        0       51 2023-06-05 17:18:03.000000 pydash2hls-2.1.3/pydash2hls/__init__.py
+-rw-rw-rw-   0        0        0     7397 2023-06-05 17:16:44.000000 pydash2hls-2.1.3/pydash2hls/converter.py
+-rw-rw-rw-   0        0        0      469 2023-06-05 16:27:43.000000 pydash2hls-2.1.3/pydash2hls/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:21:50.439171 pydash2hls-2.1.3/pydash2hls.egg-info/
+-rw-rw-rw-   0        0        0     3385 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 17:21:50.000000 pydash2hls-2.1.3/pydash2hls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:21:50.440164 pydash2hls-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-06-05 17:18:03.000000 pydash2hls-2.1.3/setup.py
```

### Comparing `pydash2hls-2.1.2/LICENSE` & `pydash2hls-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydash2hls-2.1.2/PKG-INFO` & `pydash2hls-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -101,8 +101,7 @@
 - `InvalidFileContent`: Raised when the contents of the file are not in DASH format or are incompatible.
 - `InvalidProfile`: Raised when the selected profile is invalid.
 - `MissingRemoteUrl`: Raised when a remote file URL is required but not provided.
 
 ### License
 
 This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE).
-
```

### Comparing `pydash2hls-2.1.2/README.md` & `pydash2hls-2.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
 - `InvalidFileContent`: Raised when the contents of the file are not in DASH format or are incompatible.
 - `InvalidProfile`: Raised when the selected profile is invalid.
 - `MissingRemoteUrl`: Raised when a remote file URL is required but not provided.
 
 ### License
 
 This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE).
-
```

### Comparing `pydash2hls-2.1.2/pydash2hls/converter.py` & `pydash2hls-2.1.3/pydash2hls/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 
 import requests
 import xmltodict
 
 from pydash2hls.exceptions import InvalidFileContent, InvalidPath, InvalidProfile, MissingRemoteUrl
 
 
+def _get_drm(adaptation: dict) -> dict:
+    drm = {}
+    for protection in adaptation.get("ContentProtection", []):
+        keys = {
+            "kid": "@cenc:default_KID",
+            "widevine": "cenc:pssh",
+            "playready": "mspr:pro",
+            "license": "ms:laurl"
+        }
+
+        for key, value in keys.items():
+            if value in protection:
+                item = protection[value]
+                drm[key] = item if isinstance(item, str) else item["#text"]
+    return drm
+
+
 class Converter:
 
     def __init__(self, mdp_srt: str, mdp_dict: dict, url: str = None):
         self.mdp_srt = mdp_srt
         self.mdp_dict = mdp_dict
         self.mdp_url = url
         self.profiles = self._manifest_profiles()
@@ -49,28 +66,14 @@
         raise InvalidProfile(f"Profile does not exist: {profile_id}")
 
     def _manifest_profiles(self) -> list:
         source = None if self.mdp_url is None else "/".join(self.mdp_url.split("/")[:-1])
         profiles = []
 
         for adaptation in self.mdp_dict["MPD"]["Period"]["AdaptationSet"]:
-            drm = {}
-            if "ContentProtection" in adaptation:
-                for protection in adaptation["ContentProtection"]:
-                    keys = {
-                        "kid": "@cenc:default_KID",
-                        "widevine": "cenc:pssh",
-                        "playready": "mspr:pro",
-                        "license": "ms:laurl"
-                    }
-
-                    for key, value in keys.items():
-                        if value in protection:
-                            drm[key] = protection[value]
-
             if isinstance(adaptation["Representation"], list):
                 for representation in adaptation["Representation"]:
                     mime_type = self._get_key(adaptation, representation, "@mimeType") or ("video/mp4" if "avc" in representation["@codecs"] else "audio/m4a")
                     start_with_sap = self._get_key(adaptation, representation, "@startWithSAP") or "1"
                     profile = {
                         "id": representation["@id"],
                         "mimeType": mime_type,
@@ -84,43 +87,50 @@
                         profile["width"] = int(representation["@width"])
                         profile["height"] = int(representation["@height"])
                         frame_rate = representation.get("@frameRate") or adaptation.get("@maxFrameRate") or "1/1"
                         frame_rate = frame_rate if "/" in frame_rate else f"{frame_rate}/1"
                         profile["frameRate"] = round(int(frame_rate.split("/")[0]) / int(frame_rate.split("/")[1]), 3)
                         profile["sar"] = representation.get("@sar", "1:1")
 
+                    drm = _get_drm(adaptation)
+                    item = adaptation.get("SegmentTemplate")
+                    if not item:
+                        item = representation.get("SegmentTemplate")
+                        drm = _get_drm(representation)
+
                     fragments = []
-                    if "SegmentTemplate" in adaptation:
+                    if item:
                         position = 0
-                        number = int(adaptation["SegmentTemplate"].get("@startNumber", 1)) - 1
-                        timescale = int(adaptation["SegmentTemplate"]["@timescale"])
-                        timelines = adaptation["SegmentTemplate"]["SegmentTimeline"]["S"]
+                        number = int(item.get("@startNumber", 1)) - 1
+                        timescale = int(item["@timescale"])
+                        timelines = item["SegmentTimeline"]["S"]
                         for timeline in timelines:
                             for _ in range(int(timeline.get("@r", 1))):
                                 number += 1
                                 extinf = int(timelines[position]["@d"]) / timescale
-                                media = adaptation["SegmentTemplate"]["@media"]
+                                media = item["@media"]
                                 if not media.startswith("http"):
                                     if source is None:
                                         raise MissingRemoteUrl("Remote manifest URL required.")
                                     media = f"{source}/{media}"
 
                                 media = media.replace("$Number$", str(number))
-                                time = timelines[position].get("@t", 0) + int(timelines[position]["@d"])
+                                time = int(timelines[position].get("@t", 0)) + int(timelines[position]["@d"])
                                 media = media.replace("$Time$", str(time))
                                 media = media.replace("$RepresentationID$", profile["id"])
                                 media = media.replace("$Bandwidth$", str(profile["bandwidth"]))
 
                                 fragments.append({
                                     "range": "0-",
                                     "extinf": f"{extinf:.3f}",
                                     "media": media
                                 })
                             position += 1
                     else:
+                        drm = _get_drm(adaptation)
                         segment = representation["SegmentBase"]["@indexRange"]
                         start, end = map(int, segment.split("-"))
                         extinf = (end - start) / 1000
                         fragments.append({
                             "range": segment,
                             "extinf": f"{extinf:.3f}",
                             "media": f"{source}/{representation['BaseURL']}"
```

### Comparing `pydash2hls-2.1.2/pydash2hls.egg-info/PKG-INFO` & `pydash2hls-2.1.3/pydash2hls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -101,8 +101,7 @@
 - `InvalidFileContent`: Raised when the contents of the file are not in DASH format or are incompatible.
 - `InvalidProfile`: Raised when the selected profile is invalid.
 - `MissingRemoteUrl`: Raised when a remote file URL is required but not provided.
 
 ### License
 
 This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE).
-
```

### Comparing `pydash2hls-2.1.2/setup.py` & `pydash2hls-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pydash2hls",
-    version="2.1.2",
+    version="2.1.3",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for converting DASH manifest files to HLS format.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pydash2hls",
     packages=find_packages(),
```

