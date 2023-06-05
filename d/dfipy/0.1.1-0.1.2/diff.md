# Comparing `tmp/dfipy-0.1.1.tar.gz` & `tmp/dfipy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-0.1.1.tar", max compression
+gzip compressed data, was "dfipy-0.1.2.tar", max compression
```

## Comparing `dfipy-0.1.1.tar` & `dfipy-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      557 2023-05-30 11:17:43.850642 dfipy-0.1.1/LICENCE
--rw-r--r--   0        0        0     1733 2023-05-30 11:17:43.850642 dfipy-0.1.1/README.md
--rw-r--r--   0        0        0      122 2023-05-30 11:17:43.854642 dfipy-0.1.1/dfi/__init__.py
--rw-r--r--   0        0        0     9190 2023-05-30 11:17:43.854642 dfipy-0.1.1/dfi/analysis.py
--rw-r--r--   0        0        0     3741 2023-05-30 11:17:43.854642 dfipy-0.1.1/dfi/connection.py
--rw-r--r--   0        0        0    13621 2023-05-30 11:17:43.854642 dfipy-0.1.1/dfi/getters.py
--rw-r--r--   0        0        0     1356 2023-05-30 11:17:43.854642 dfipy-0.1.1/dfi/logging.py
--rw-r--r--   0        0        0    14626 2023-05-30 11:17:43.854642 dfipy-0.1.1/dfi/show.py
--rw-r--r--   0        0        0     4266 2023-05-30 11:17:43.854642 dfipy-0.1.1/dfi/stream.py
--rw-r--r--   0        0        0     1994 2023-05-30 11:17:44.842678 dfipy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 dfipy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-06-05 10:12:54.483500 dfipy-0.1.2/LICENCE
+-rw-r--r--   0        0        0     1733 2023-06-05 10:12:54.483500 dfipy-0.1.2/README.md
+-rw-r--r--   0        0        0      194 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/__init__.py
+-rw-r--r--   0        0        0    16364 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/analysis.py
+-rw-r--r--   0        0        0     4631 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/connection.py
+-rw-r--r--   0        0        0    25259 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/getters.py
+-rw-r--r--   0        0        0     1537 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/logging.py
+-rw-r--r--   0        0        0    15871 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/show.py
+-rw-r--r--   0        0        0     5566 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/stream.py
+-rw-r--r--   0        0        0     1994 2023-06-05 10:12:55.427519 dfipy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 dfipy-0.1.2/PKG-INFO
```

### Comparing `dfipy-0.1.1/LICENCE` & `dfipy-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.1/README.md` & `dfipy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.1/dfi/logging.py` & `dfipy-0.1.2/dfi/logging.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
 }
 
 
 def get_logging_level() -> int:
+    """Return the env variable LOGGING_LEVEL. If not defined return the defaul INFO."""
     logging_level_env = os.getenv("LOGGING_LEVEL")
 
     if logging_level_env in LOGGING_LEVELS.keys():
         return LOGGING_LEVELS[logging_level_env]
     return logging.INFO
 
 
 def setup_logger(filename: str) -> logging.Logger:
+    """Setup log - to be removed alongside with coloredlogs and to be left to developers."""
     filepath = Path(filename)
     if len(filepath.parts) > 1:  # only affects 1st party filenames not 3rd party
         filename = filepath.stem + filepath.suffix
 
     logging.basicConfig()
     logging.Formatter.converter = gmtime
     logger = logging.getLogger(name=filename)
```

### Comparing `dfipy-0.1.1/dfi/show.py` & `dfipy-0.1.2/dfi/show.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,28 @@
 import json
 from typing import List, Optional
 
 import pandas as pd
 import pydeck as pdk
 import pyperclip
 import requests
-from IPython.display import IFrame
+from IPython.display import IFrame  # pylint: disable=import-error
 
 from dfi.connection import DFIConnect
 from dfi.logging import setup_logger
 
 logger = setup_logger(__file__)
 
+# TODO: find a way to avoid importing IPython and removing
+# ipython from requirements.
+# TODO: why not using KeplerGl as industry standard? Passing polygons via copy paste
+# is not ideal, or via passing html code is not ideal. Kepler has the methods to draw
+# map out of the box. A lightweigth alternative to kepler is https://leafmap.org/
+# also having the draw polygon option out of the box.
+
 
 VIEW_STATE_LONDON = pdk.ViewState(
     longitude=-0.1,
     latitude=51.5,
     zoom=10,
     min_zoom=5,
     max_zoom=15,
@@ -31,15 +38,15 @@
 
 class DFIShow:
     """
     Visualisation methods to build use case on top of the queries from DFI.
     Not part of the DFI API wrapper, but handy to have it embedded there for demo and functionalities.
     """
 
-    def __init__(self, dfi_conn):
+    def __init__(self, dfi_conn: DFIConnect) -> None:
         self.dfi_conn: DFIConnect = dfi_conn
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.dfi_conn!r}){self.__dict__}"
 
     def __str__(self):
         return f"""DFI Python API: instance of {self.__class__.__name__} composed with {self.dfi_conn!r}"""
@@ -68,14 +75,17 @@
         vertices: List[List[float]] = None,
         df_history: pd.DataFrame = None,
         df_hexagons: pd.DataFrame = None,
         df_colocs: pd.DataFrame = None,
         view_state=None,
         color_gradient: bool = True,
     ) -> pdk.Deck:
+        """
+        Helper method to create a heatmap from the components of a range of queries.
+        """
         layers = []
 
         if query_polygons is not None:
             for query_polygon in query_polygons:
                 my_url = self.dfi_conn.base_url + "/polygons/" + query_polygon
                 my_headers = self.dfi_conn.synchronous_headers
                 response = requests.get(
@@ -205,14 +215,22 @@
         query_polygons: List[str] = None,
         vertices: List[List[float]] = None,
         history: List[List[float]] = None,
         df_history: pd.DataFrame = None,
         view_state=None,
         tooltip: Optional[dict] = None,
     ) -> pdk.Deck:
+        """
+        Helper method to create a map from the components obtained from a range of queries.
+        """
+        # TODO (Robert):
+        # has both history and df_history.  This is confusing as it’s the same data but different forms.
+        # I believe all the function calls return histories into a dataframe,
+        # why is the history argument needed here?
+        # should plot the polygon first then the pings on top
         layers = []
 
         if history is not None:
             pdk_history = pdk.Layer(
                 "ScatterplotLayer",
                 pd.DataFrame(history, columns=["longitude", "latitude"]),
                 get_position=["longitude", "latitude"],
@@ -255,14 +273,17 @@
             )
             layers.append(pdk_df_history)
 
         if query_polygons is not None:
             for query_polygon in query_polygons:
                 my_url = self.dfi_conn.base_url + "/polygons/" + query_polygon
                 my_headers = self.dfi_conn.synchronous_headers
+
+                # TODO: this should be part of the getters method, as it is not reponsibility of
+                # the DFIShow class to submit requests.
                 response = requests.get(
                     my_url,
                     headers=my_headers,
                     timeout=self.dfi_conn.query_timeout,
                 )
                 self._check_response(response, my_url, my_headers)
 
@@ -310,15 +331,18 @@
             return pdk.Deck(layers=layers, initial_view_state=view_state, tooltip=tooltip)
         else:
             return pdk.Deck(layers=layers, initial_view_state=view_state)
 
     @staticmethod
     def ask_user_polygon(
         mapbox_api_token: str, width_pc: int = 100, height_px: int = 400, zoom: int = 8, long: float = 0, lat: float = 0
-    ):
+    ) -> IFrame:
+        """
+        Helper to input a polygon.
+        """
         srcdoc = """
 <!DOCTYPE html>
 <html>
 <head>
 <title>mapboxgl-jupyter viz</title>
 <meta charset='UTF-8' />
 <meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />
@@ -404,27 +428,27 @@
         iframe_template = (
             f'<iframe id="{frame_id}", srcdoc="{srcdoc}" style="width: {width_pc}%; height: {height_px}px;"></iframe>'
         )
         return IFrame(iframe_template, height_px, height_px)
 
     @staticmethod
     def get_user_polygon() -> List[List[float]]:
+        """Helper to create a polygon via copy paste"""
         polygon_text = pyperclip.paste()
         try:
             polygon_coordinates = json.loads(polygon_text)
-        except Exception as e:
-            msg = f"Could not parse content of clipboard: '{polygon_text}', Error {e}"
-            logger.error(msg)
+        except Exception as err:
+            logger.error("Could not parse content of clipboard: '%s', Error %s", polygon_text, err)
             return
         return polygon_coordinates
 
 
 def _create_geojson_from_coordinates(coordinates: List[List[float]]) -> dict:
     """
-    Helper function that allows us to display a polygon on a map.
+    Helper function to display a polygon on a map.
     """
     return {
         "type": "FeatureCollection",
         "features": [
             {
                 "type": "Feature",
                 "properties": {},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dfipy-0.1.1/pyproject.toml` & `dfipy-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "0.1.1"
+version = "0.1.2"
 description = "DFI api python wrapper"
 authors = [
   "Maurizio Morriello <maurizio.morriello@excession.co>",
   "Sebastiano Ferraris <sebastiano.ferraris@excession.co>",
 ]
 readme = "README.md"
 include = ["LICENCE"]
```

### Comparing `dfipy-0.1.1/PKG-INFO` & `dfipy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 0.1.1
+Version: 0.1.2
 Summary: DFI api python wrapper
 Author: Maurizio Morriello
 Author-email: maurizio.morriello@excession.co
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

