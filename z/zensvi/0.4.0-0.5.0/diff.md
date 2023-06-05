# Comparing `tmp/zensvi-0.4.0.tar.gz` & `tmp/zensvi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.4.0.tar", max compression
+gzip compressed data, was "zensvi-0.5.0.tar", max compression
```

## Comparing `zensvi-0.4.0.tar` & `zensvi-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.4.0/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.4.0/README.md
--rwxr-xr-x   0        0        0      713 2023-06-01 06:20:51.150956 zensvi-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.4.0/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.4.0/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.4.0/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    39841 2023-05-25 00:58:05.893778 zensvi-0.4.0/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.4.0/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    46724 2023-05-30 09:53:14.670233 zensvi-0.4.0/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.4.0/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.4.0/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8291 2023-05-26 09:00:45.660707 zensvi-0.4.0/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.4.0/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.4.0/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.4.0/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.4.0/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.4.0/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.4.0/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.4.0/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 zensvi-0.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.5.0/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.5.0/README.md
+-rwxr-xr-x   0        0        0      713 2023-06-05 08:56:03.272061 zensvi-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.5.0/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.5.0/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.5.0/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    39841 2023-06-05 07:31:29.453652 zensvi-0.5.0/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.5.0/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.344850 zensvi-0.5.0/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.5.0/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.5.0/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.345206 zensvi-0.5.0/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.345880 zensvi-0.5.0/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.5.0/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.346254 zensvi-0.5.0/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.5.0/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.5.0/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.5.0/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.5.0/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 zensvi-0.5.0/PKG-INFO
```

### Comparing `zensvi-0.4.0/LICENSE` & `zensvi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.4.0/README.md` & `zensvi-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.4.0/pyproject.toml` & `zensvi-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.4.0"
+version = "0.5.0"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zensvi-0.4.0/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.5.0/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.4.0/src/zensvi/download/streetview_downloader.py` & `zensvi-0.5.0/src/zensvi/download/streetview_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import glob
 import shutil
 import numpy as np
 import osmnx as ox
 from abc import ABC, abstractmethod
 import mapillary.interface as mly
 from shapely import wkt
+from PIL import Image
 
 from zensvi.download.utils.imtool import ImageTool
 from zensvi.download.utils.get_pids import panoids
 from zensvi.download.utils.geoprocess import GeoProcessor
 from zensvi.download.utils.helpers import standardize_column_names, create_buffer_gdf
 
 # set logging level to warning
@@ -228,15 +229,15 @@
         if self.cache_pids_raw.exists():
             self.cache_pids_raw.unlink()
         # delete the cache directory
         if dir_cache_augmented_metadata.exists():
             shutil.rmtree(dir_cache_augmented_metadata)
         return df
 
-    def _get_pids_from_df(self, df, id_columns=None, closest=False, disp=False):
+    def _get_pids_from_df(self, df, id_columns=None):
         # 1. Create a new directory called "pids" to store each batch pids
         dir_cache_pids = self.dir_cache / 'raw_pids'
         dir_cache_pids.mkdir(parents=True, exist_ok=True)
 
         # 2. Load all the checkpoint csv files
         checkpoints = glob.glob(str(dir_cache_pids / '*.csv'))
         checkpoint_start_index = len(checkpoints)
@@ -256,15 +257,15 @@
             # Merge on the ID column, keeping track of where each row originates
             merged = df.merge(completed_ids, on='lat_lon_id', how='outer', indicator=True)
 
             # Filter out rows that come from the 'completed_ids' DataFrame
             df = merged[merged['_merge'] == 'left_only'].drop(columns='_merge')
 
         def get_street_view_info(longitude, latitude, proxies):
-            results = panoids(latitude, longitude, proxies, closest=closest, disp=disp)
+            results = panoids(latitude, longitude, proxies, )
             return results
 
         def worker(row):
             input_longitude = row.longitude
             input_latitude = row.latitude
             lat_lon_id = row.lat_lon_id
             id_dict = {column: getattr(row, column) for column in id_columns} if id_columns else {}
@@ -337,37 +338,37 @@
         results_df.to_csv(self.cache_pids_raw, index=False)
 
         # delete the cache directory
         if dir_cache_pids.exists():
             shutil.rmtree(dir_cache_pids)
         return results_df
 
-    def _get_pids_from_gdf(self, gdf, id_columns, closest=False, disp=False):  
+    def _get_pids_from_gdf(self, gdf, **kwargs):  
         if self.cache_lat_lon.exists():
             df = pd.read_csv(self.cache_lat_lon)
             print("The lat and lon have been read from the cache")
         else:
             if gdf.crs is None:
                 gdf = gdf.set_crs('EPSG:4326')
             elif gdf.crs != 'EPSG:4326':
                 # convert to EPSG:4326
                 gdf = gdf.to_crs('EPSG:4326')
             # read shapefile
-            gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
+            gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, **kwargs)
             df = gp.get_lat_lon()
             df['lat_lon_id'] = np.arange(1, len(df) + 1)
             # save df to cache
             df.to_csv(self.cache_lat_lon, index=False)
 
         if self.cache_pids_raw.exists():
             print("The raw panorama IDs have been read from the cache")
             results_df = pd.read_csv(self.cache_pids_raw)
         else:
             # Use _get_pids_from_df to get pids from df
-            results_df = self._get_pids_from_df(df, id_columns, closest=closest, disp=disp)
+            results_df = self._get_pids_from_df(df, kwargs["id_columns"])
 
         # Check if lat and lon are within input polygons
         polygons = gpd.GeoSeries([geom for geom in gdf['geometry'] if geom.type in ['Polygon', 'MultiPolygon']])
 
         # the rest is only for polygons, so return results_df if there's no polygons
         if len(polygons) == 0:
             return results_df
@@ -401,86 +402,71 @@
         # Return only those points within polygons
         results_within_polygons_df = results_df[results_df['within_polygon']]
         # Drop the 'within_polygon' column
         results_within_polygons_df = results_within_polygons_df.drop(columns='within_polygon')
         return results_within_polygons_df
 
     def _get_raw_pids(self, **kwargs):
-        defaults = {
-            'lat': None, 'lon': None, 'input_csv_file': "", 'input_shp_file': "",
-            'input_place_name': "", 'id_columns': None, 'buffer': 0, 
-            'closest': False, 'disp': False
-        }
-        
-        defaults.update(kwargs)
-
         if self.cache_pids_raw.exists():
             pid = pd.read_csv(self.cache_pids_raw)
             print("The raw panorama IDs have been read from the cache")
             return pid
 
-        if defaults['lat'] is not None and defaults['lon'] is not None:
-            pid = panoids(defaults['lat'], defaults['lon'], self.proxies, closest=defaults['closest'], disp=defaults['disp'])
+        if kwargs['lat'] is not None and kwargs['lon'] is not None:
+            pid = panoids(kwargs['lat'], kwargs['lon'], self.proxies)
             pid = pd.DataFrame(pid)
             # add input_lat and input_lon
-            pid['input_latitude'] = defaults['lat']
-            pid['input_longitude'] = defaults['lon']
-        elif defaults['input_csv_file'] != "":
-            df = pd.read_csv(defaults['input_csv_file'])
+            pid['input_latitude'] = kwargs['lat']
+            pid['input_longitude'] = kwargs['lon']
+        elif kwargs['input_csv_file'] != "":
+            df = pd.read_csv(kwargs['input_csv_file'])
             df = standardize_column_names(df)
-            if defaults['buffer'] > 0:
+            if kwargs['buffer'] > 0:
                 gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs='EPSG:4326')
-                gdf = create_buffer_gdf(gdf, defaults['buffer'])
-                pid = self._get_pids_from_gdf(gdf, defaults['id_columns'], closest=False, disp=False)
+                gdf = create_buffer_gdf(gdf, kwargs['buffer'])
+                pid = self._get_pids_from_gdf(gdf, **kwargs)
             else:
-                pid = self._get_pids_from_df(df, defaults['id_columns'], closest=False, disp=False)
-        elif defaults['input_shp_file'] != "":
-            gdf = gpd.read_file(defaults['input_shp_file'])
-            if defaults['buffer'] > 0:
-                gdf = create_buffer_gdf(gdf, defaults['buffer'])
-            pid = self._get_pids_from_gdf(gdf, defaults['id_columns'], closest=False, disp=False)
-        elif defaults['input_place_name'] != "":
+                pid = self._get_pids_from_df(df, kwargs['id_columns'])
+        elif kwargs['input_shp_file'] != "":
+            gdf = gpd.read_file(kwargs['input_shp_file'])
+            if kwargs['buffer'] > 0:
+                gdf = create_buffer_gdf(gdf, kwargs['buffer'])
+            pid = self._get_pids_from_gdf(gdf, **kwargs)
+        elif kwargs['input_place_name'] != "":
             print("Geocoding the input place name")
-            gdf = ox.geocoder.geocode_to_gdf(defaults['input_place_name'])
+            gdf = ox.geocoder.geocode_to_gdf(kwargs['input_place_name'])
             # raise error if the input_place_name is not found
             if len(gdf) == 0:
                 raise ValueError("The input_place_name is not found. Please try another place name.")
-            if defaults['buffer'] > 0:
-                gdf = create_buffer_gdf(gdf, defaults['buffer'])
-            pid = self._get_pids_from_gdf(gdf, defaults['id_columns'], closest=False, disp=False) 
+            if kwargs['buffer'] > 0:
+                gdf = create_buffer_gdf(gdf, kwargs['buffer'])
+            pid = self._get_pids_from_gdf(gdf, **kwargs) 
         else:
             raise ValueError("Please input the lat and lon, csv file, or shapefile.")
 
         return pid
 
     def get_pids(self, path_pid, **kwargs):
-        defaults = {
-            'lat': None, 'lon': None, 'input_csv_file': "", 'input_shp_file': "",
-            'input_place_name': "", 'id_columns': None, 'buffer': 0, 
-            'closest': False, 'disp': False, 'augment_metadata': False
-        }
-        
-        defaults.update(kwargs)
-        id_columns = defaults['id_columns']
+        id_columns = kwargs['id_columns']
         if id_columns is not None:
             if isinstance(id_columns, str):
                 id_columns = [id_columns.lower()]
             elif isinstance(id_columns, list):
                 id_columns = [column.lower() for column in id_columns]
         else:
             id_columns = []
         # update id_columns
-        defaults['id_columns'] = id_columns
+        kwargs['id_columns'] = id_columns
         
         # get raw pid
-        pid = self._get_raw_pids(**defaults)
+        pid = self._get_raw_pids(**kwargs)
         
-        if defaults["augment_metadata"] & (self.gsv_api_key != None):
+        if kwargs["augment_metadata"] & (self.gsv_api_key != None):
             pid = self._augment_metadata(pid)
-        elif defaults["augment_metadata"] & (self.gsv_api_key == None):
+        elif kwargs["augment_metadata"] & (self.gsv_api_key == None):
             raise ValueError("Please set the gsv api key by calling the gsv_api_key method.")
         pid.to_csv(path_pid, index=False)
         print("The panorama IDs have been saved to {}".format(path_pid)) 
 
     def _set_dirs(self, dir_output):
         # set dir_output as attribute and create the directory
         self.dir_output = Path(dir_output)
@@ -490,32 +476,32 @@
         self.dir_cache.mkdir(parents=True, exist_ok=True)
         # set other cache directories
         self.cache_lat_lon = self.dir_cache / "lat_lon.csv"
         self.cache_pids_raw = self.dir_cache / "pids_raw.csv"
         self.cache_pids_augmented = self.dir_cache / "pids_augemented.csv"
         
     def download_svi(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
-                    lat=None, lon=None, input_csv_file="", input_shp_file = "", input_place_name = "", id_columns=None, buffer = 0, closest=False, 
-                    disp=False, augment_metadata=False, update_pids = False):
+                    lat=None, lon=None, input_csv_file="", input_shp_file = "", input_place_name = "", id_columns=None, buffer = 0, 
+                    augment_metadata=False, update_pids = False, **kwargs):
         # set necessary directories
         self._set_dirs(dir_output)
         
         # call get_pids function first if path_pid is None
         if (path_pid is None) & (self.cache_pids_augmented.exists() == False):
             print("Getting pids...")
-            path_pid = self.dir_output / "pids.csv"
+            path_pid = self.dir_output / "gsv_pids.csv"
             if path_pid.exists() & (update_pids == False):
                 print("update_pids is set to False. So the following csv file will be used: {}".format(path_pid))
             else:
                 self.get_pids(path_pid, lat=lat, lon=lon,
                             input_csv_file=input_csv_file, input_shp_file = input_shp_file, input_place_name = input_place_name, 
-                            id_columns=id_columns, buffer = buffer, closest=closest, disp=disp, augment_metadata=augment_metadata)
+                            id_columns=id_columns, buffer = buffer, augment_metadata=augment_metadata, **kwargs)
         elif self.cache_pids_augmented.exists():
             # copy the cache pids_augmented to path_pid
-            path_pid = self.dir_output / "pids.csv"
+            path_pid = self.dir_output / "gsv_pids.csv"
             shutil.copy2(self.cache_pids_augmented, path_pid)
             print("The augmented panorama IDs have been saved to {}".format(path_pid))
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
         # zoom = 2
         # h_tiles = 4  # 26
         # v_tiles = 2  # 13
@@ -699,37 +685,37 @@
         results_df.to_csv(self.cache_pids_raw, index=False)
 
         # delete the cache directory
         if dir_cache_pids.exists():
             shutil.rmtree(dir_cache_pids)
         return results_df
 
-    def _get_pids_from_gdf(self, gdf, id_columns, **kwargs):
+    def _get_pids_from_gdf(self, gdf, mly_kwargs, **kwargs):
         if self.cache_lat_lon.exists():
             df = pd.read_csv(self.cache_lat_lon)
             print("The lat and lon have been read from the cache")
         else:
             if gdf.crs is None:
                 gdf = gdf.set_crs('EPSG:4326')
             elif gdf.crs != 'EPSG:4326':
                 # convert to EPSG:4326
                 gdf = gdf.to_crs('EPSG:4326')
             # read shapefile
-            gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
+            gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, **kwargs)
             df = gp.get_lat_lon()
             df['lat_lon_id'] = np.arange(1, len(df) + 1)
             # save df to cache
             df.to_csv(self.cache_lat_lon, index=False)
 
         if self.cache_pids_raw.exists():
             print("The raw panorama IDs have been read from the cache")
             results_df = pd.read_csv(self.cache_pids_raw)
         else:
             # Use _get_pids_from_df to get pids from df
-            results_df = self._get_pids_from_df(df, id_columns, **kwargs)
+            results_df = self._get_pids_from_df(df, kwargs["id_columns"], **mly_kwargs)
             
         if not isinstance(results_df, pd.DataFrame):
             return
         
         # Check if lat and lon are within input polygons
         polygons = gpd.GeoSeries([geom for geom in gdf['geometry'] if geom.type in ['Polygon', 'MultiPolygon']])
 
@@ -766,16 +752,16 @@
         # Return only those points within polygons
         results_within_polygons_df = results_df[results_df['within_polygon']]
         # Drop the 'within_polygon' column
         results_within_polygons_df = results_within_polygons_df.drop(columns='within_polygon')
         return results_within_polygons_df
         
     def _get_raw_pids(self, **kwargs):
-        allowed_keys = {'fields', 'zoom', 'radius', 'image_type', 'min_captured_at', 'max_captured_at', 'organization_id'} 
-        mly_kwargs = {k: v for k, v in kwargs.items() if k in allowed_keys}
+        mly_allowed_keys = {'fields', 'zoom', 'radius', 'image_type', 'min_captured_at', 'max_captured_at', 'organization_id'} 
+        mly_kwargs = {k: v for k, v in kwargs.items() if k in mly_allowed_keys}
         if self.cache_pids_raw.exists():
             pid = pd.read_csv(self.cache_pids_raw)
             print("The raw panorama IDs have been read from the cache")
             return pid
 
         if kwargs['lat'] is not None and kwargs['lon'] is not None:
             pid = mly.get_image_close_to(kwargs['lat'], kwargs['lon'], **mly_kwargs)
@@ -791,31 +777,31 @@
             pid['input_longitude'] = kwargs['lon']
         elif kwargs['input_csv_file'] != "":
             df = pd.read_csv(kwargs['input_csv_file'])
             df = standardize_column_names(df)
             if kwargs['buffer'] > 0:
                 gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs='EPSG:4326')
                 gdf = create_buffer_gdf(gdf, kwargs['buffer'])
-                pid = self._get_pids_from_gdf(gdf, kwargs['id_columns'], **mly_kwargs)
+                pid = self._get_pids_from_gdf(gdf, mly_kwargs, **kwargs)
             else:
-                pid = self._get_pids_from_df(df, kwargs['id_columns'], **mly_kwargs)
+                pid = self._get_pids_from_df(df, kwargs['id_columns'], mly_kwargs)
         elif kwargs['input_shp_file'] != "":
             gdf = gpd.read_file(kwargs['input_shp_file'])
             if kwargs['buffer'] > 0:
                 gdf = create_buffer_gdf(gdf, kwargs['buffer'])
-            pid = self._get_pids_from_gdf(gdf, kwargs['id_columns'], **mly_kwargs)
+            pid = self._get_pids_from_gdf(gdf, mly_kwargs, **kwargs)
         elif kwargs['input_place_name'] != "":
             print("Geocoding the input place name")
             gdf = ox.geocoder.geocode_to_gdf(kwargs['input_place_name'])
             # raise error if the input_place_name is not found
             if len(gdf) == 0:
                 raise ValueError("The input_place_name is not found. Please try another place name.")
             if kwargs['buffer'] > 0:
                 gdf = create_buffer_gdf(gdf, kwargs['buffer'])
-            pid = self._get_pids_from_gdf(gdf, kwargs['id_columns'], **mly_kwargs) 
+            pid = self._get_pids_from_gdf(gdf, mly_kwargs, **kwargs) 
         else:
             raise ValueError("Please input the lat and lon, csv file, or shapefile.")
 
         return pid
     
     def get_pids(self, path_pid, **kwargs):
         id_columns = kwargs['id_columns']
@@ -913,64 +899,72 @@
         results_df = pd.concat([pd.read_csv(checkpoint) for checkpoint in glob.glob(str(dir_cache_urls / '*.csv'))], ignore_index=True)
         results_df.to_csv(self.pids_url, index=False)
 
         if dir_cache_urls.exists():
             shutil.rmtree(dir_cache_urls)
 
     
-    def _download_images_mly(self):
+    def _download_images_mly(self, cropped):
         checkpoints = glob.glob(str(self.panorama_output / '*.png'))
 
         # Read already downloaded images and convert to ids
         downloaded_ids = set([Path(file_path).stem for file_path in checkpoints])  # Use set for faster operations
 
         urls_df = pd.read_csv(self.pids_url)
 
         # Filter out the ids that have already been processed
         urls_df = urls_df[~urls_df['id'].isin(downloaded_ids)]  # Use isin for efficient operation
 
-        def worker(row, output_dir):
+        def worker(row, output_dir, cropped):
             url, panoid = row.url, row.id
             user_agent = random.choice(self.user_agents)
             proxy = random.choice(self.proxies)
 
             image_name = f'{panoid}.png'  # Use id for file name
             image_path = output_dir / image_name
             try:
-                response = requests.get(url, headers = user_agent, proxies=proxy, timeout=10)
+                response = requests.get(url, headers=user_agent, proxies=proxy, timeout=10)
                 if response.status_code == 200:
                     with open(image_path, 'wb') as f:
                         f.write(response.content)
+                    
+                    if cropped:
+                        img = Image.open(image_path)
+                        w, h = img.size
+                        img_cropped = img.crop((0, 0, w, h // 2))
+                        img_cropped.save(image_path)
+
                 else:
                     self._log_write(panoid)
             except Exception as e:
                 self._log_write(panoid)
-                print(f"Error: {e}")
+                print(f"Error: {e}" )
+
 
         batch_size = 1000
         num_batches = (len(urls_df) + batch_size - 1) // batch_size
 
         for i in tqdm(range(num_batches), desc=f"Downloading images by batch size {min(batch_size, len(urls_df))}"):
             with ThreadPoolExecutor() as executor:
-                batch_futures = {executor.submit(worker, row, self.panorama_output): row.id for row in urls_df.iloc[i*batch_size : (i+1)*batch_size].itertuples()}
+                batch_futures = {executor.submit(worker, row, self.panorama_output, cropped): row.id for row in urls_df.iloc[i*batch_size : (i+1)*batch_size].itertuples()}
                 for future in tqdm(as_completed(batch_futures), total=len(batch_futures), desc=f"Downloading images for batch #{i+1}"):
                     try:
                         future.result()
                     except Exception as e:
                         print(f"Error: {e}")
                 
     def download_svi(self, dir_output, path_pid = None, lat=None, lon=None, input_csv_file="", input_shp_file = "", input_place_name =
-                    "", id_columns=None, buffer = 0, update_pids = False, resolution = 1024, **kwargs):
+                    "", id_columns=None, buffer = 0, update_pids = False, resolution = 1024, cropped = False, **kwargs):
         # set necessary directories
         self._set_dirs(dir_output)
         
         # call get_pids function first if path_pid is None
         if path_pid is None:
             print("Getting pids...")
-            path_pid = self.dir_output / "pids.csv"
+            path_pid = self.dir_output / "mly_pids.csv"
             if path_pid.exists() & (update_pids == False):
                 print("update_pids is set to False. So the following csv file will be used: {}".format(path_pid))
             else:
                 self.get_pids(path_pid, lat=lat, lon=lon,
                             input_csv_file=input_csv_file, input_shp_file = input_shp_file, input_place_name = input_place_name, 
                             id_columns=id_columns, buffer = buffer, **kwargs)
         else:
@@ -986,15 +980,15 @@
         self.panorama_output = self.dir_output / "mly_svi"
         self.panorama_output.mkdir(parents=True, exist_ok=True)
         
         # get urls
         if path_pid.exists():
             self._get_urls_mly(path_pid, resolution=resolution) 
             # download images
-            self._download_images_mly()
+            self._download_images_mly(cropped)
         else: 
             print("There is no panorama ID to download within the given input parameters")
         
         # delete the cache directory
         if self.dir_cache.exists():
             shutil.rmtree(self.dir_cache)
             print("The cache directory has been deleted")
```

### Comparing `zensvi-0.4.0/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.5.0/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.4.0/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.5.0/src/zensvi/download/utils/geoprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,38 @@
 tqdm.pandas()
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
 import numpy as np
 from pyproj import Transformer
 import networkx
 
 class GeoProcessor:
-    def __init__(self, gdf, distance=1, grid = False, grid_size = 1, id_columns=[]):
+    def __init__(self, gdf, distance=1, grid = False, grid_size = 1, id_columns=[], **kwargs):
         self.gdf = gdf
         self.distance = distance
         self.processing_functions = {
             'Point': self.process_point,
             'MultiPoint': self.process_multipoint,
             'LineString': self.process_linestring,
             'MultiLineString': self.process_multilinestring,
             'Polygon': self.process_polygon,
             'MultiPolygon': self.process_multipolygon
         }
         self.grid = grid
         self.grid_size = grid_size
         self.utm_crs = None
         self.id_columns = id_columns
+        if "network_type" in kwargs:
+            self.network_type = kwargs["network_type"]
+        else:
+            self.network_type = "all"
+            
+        if "custom_filter" in kwargs:
+            self.custom_filter = kwargs["custom_filter"]
+        else:
+            self.custom_filter = None
 
     def get_lat_lon(self):
         self.gdf['feature_type'] = self.gdf['geometry'].apply(lambda x: x.geom_type)
         gdf_list = []
 
         for feature_type, func in self.processing_functions.items():
             sub_gdf = self.gdf[self.gdf['feature_type'] == feature_type]
@@ -71,15 +80,15 @@
         # Explode the multilinestring into individual linestrings
         gdf = gdf.explode('geometry').reset_index(drop=True)
 
         # Call process_linestring on the exploded GeoDataFrame
         return self.process_linestring(gdf)
 
     def get_street_points(self, polygon):
-        graph = ox.graph_from_polygon(polygon, network_type='all')
+        graph = ox.graph_from_polygon(polygon, network_type=self.network_type, custom_filter=self.custom_filter)
         _, edges = ox.graph_to_gdfs(graph)
         # Project the street network to UTM
         edges_utm = ox.projection.project_gdf(edges)
         utm_crs = edges_utm.crs
 
         # Use osmnx.utils_geo.interpolate_points function to interpolate points along LineStrings
         edges_utm['sample_points'] = edges_utm['geometry'].apply(lambda geom: list(ox.utils_geo.interpolate_points(geom, dist=self.distance)))
```

### Comparing `zensvi-0.4.0/src/zensvi/download/utils/get_pids.py` & `zensvi-0.5.0/src/zensvi/download/utils/get_pids.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         try:
             resp = requests.get(url, proxies=proxy, timeout=5)
             return resp.text
         except Exception as e:
             print(f"Proxy {proxy} is not working. Exception: {e}")
             continue
 
-def panoids(lat, lon, proxies, closest=False, disp=False):
+def panoids(lat, lon, proxies):
     resp = _panoids_data(lat, lon, proxies)
 
     # Get all the panorama ids and coordinates
     pans = re.findall('\[[0-9]+,"(.+?)"\].+?\[\[null,null,(-?[0-9]+.[0-9]+),(-?[0-9]+.[0-9]+)', resp)
     pans = [{"panoid": p[0], "lat": float(p[1]), "lon": float(p[2])} for p in pans]
 
     # Get all the dates
@@ -41,15 +41,8 @@
         pans[0].update({'year': year, "month": month})
 
         # The dates then apply in reverse order to the bottom panoramas
         dates.reverse()
         for i, (year, month) in enumerate(dates):
             pans[-1-i].update({'year': year, "month": month})
 
-    if disp:
-        for pan in pans:
-            print(pan)
-
-    if closest and len(dates) > 0:
-        return [pans[i] for i in range(len(dates))]
-    else:
-        return pans
+    return pans
```

### Comparing `zensvi-0.4.0/src/zensvi/download/utils/helpers.py` & `zensvi-0.5.0/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.4.0/src/zensvi/download/utils/imtool.py` & `zensvi-0.5.0/src/zensvi/download/utils/imtool.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,40 +37,43 @@
             im2 (undefined): second PIL image
 
         """
         dst = Image.new('RGB', (im1.width, im1.height + im2.height))
         dst.paste(im1, (0, 0))
         dst.paste(im2, (0, im1.height))
         return dst
-    
+                
     @staticmethod
-    def compose_folder(in_path, out_path, how='horizontally'):
+    def fetch_image_with_proxy(pano_id, zoom, x, y, ua, proxies):
         """
-        Description of compose_folder
-        concatenates all the images in a folder; the second part of each 
-        image must follow the first once sorted by filename.
+        Fetches an image using a proxy.
 
         Args:
-            in_path (undefined): input folder path
-            out_path (undefined): output folder path
-            how='horizontally' (undefined): concatenation direction
+            pano_id (str): GSV panorama id
+            zoom (int): Zoom level for the image
+            x (int): The x coordinate of the tile
+            y (int): The y coordinate of the tile
+            ua (str): User agent string
+            proxies (list): A list of available proxies
 
+        Returns:
+            Image: The fetched image
         """
-        images = sorted(os.listdir(in_path))
-            
-        for name1, name2 in zip(images[0::2], images[1::2]):
-            
-            im1 = Image.open(in_path + name1)
-            im2 = Image.open(in_path + name2)
-            
-            if how == 'horizontally':
-                ImageTool.concat_horizontally(im1, im2).save(out_path + '_'.join(name1.split('_')[1:]))
-            else:
-                ImageTool.concat_vertically(im1, im2).save(out_path + '_'.join(name1.split('_')[1:]))
-                
+        while True:
+            # Choose a random proxy for each request
+            proxy = random.choice(proxies)
+            url_img = f'https://cbk0.google.com/cbk?output=tile&panoid={pano_id}&zoom={zoom}&x={x}&y={y}'
+            try:
+                image = Image.open(requests.get(url_img, headers=ua, proxies=proxy, stream=True).raw)
+                return image
+            except ProxyError as e:
+                print(f"Proxy {proxy} is not working. Exception: {e}")
+                continue
+
+
     @staticmethod
     def get_and_save_image(pano_id, identif, zoom, vertical_tiles, horizontal_tiles, out_path, ua, proxies, cropped=False, full=True):
         """
         Description of get_and_save_image
         
         Downloads an image tile by tile and composes them together.
 
@@ -81,73 +84,46 @@
             vertical_tiles (undefined): number of vertical tiles
             horizontal_tiles (undefined): number of horizontal tiles
             out_path (undefined): output path
             cropped=False (undefined): set True if the image split horizontally in half is needed
             full=True (undefined): set to True if the full image is needed
 
         """
-        while True:
-            # Choose a random proxy for each request
-            proxy = random.choice(proxies)
-            first_url_img = f'https://cbk0.google.com/cbk?output=tile&panoid={pano_id}&zoom={zoom}&x={0}&y={0}'
-            try:
-                first = Image.open(requests.get(first_url_img, headers=ua, proxies=proxy, stream=True).raw)
-                break
-            except ProxyError as e:
-                print(f"Proxy {proxy} is not working. Exception: {e}")
-                continue
-            finally:
-                break
+        for x in range(horizontal_tiles):
+            for y in range(vertical_tiles):
+                new_img = ImageTool.fetch_image_with_proxy(pano_id, zoom, x, y, ua, proxies)
+                if not full:
+                    new_img.save(f'{out_path}/{identif}_x{x}_y{y}.jpg')
+                if y == 0:
+                    first_slice = new_img
+                else:
+                    first_slice = ImageTool.concat_vertically(first_slice, new_img)
 
-        # first_vert = False
-
-        for y in range(1, vertical_tiles):
-            #new_img = Image.open(f'./images/test_x0_y{y}.png')
-            url_new_img = f'https://cbk0.google.com/cbk?output=tile&panoid={pano_id}&zoom={zoom}&x={0}&y={y}'
-            new_img = Image.open(requests.get(url_new_img, headers=ua, proxies=proxy, stream=True).raw)
-            first = ImageTool.concat_vertically(first, new_img)
-        first_slice = first
-
-        for x in range(1, horizontal_tiles):
-
-            first_url_img = f'https://cbk0.google.com/cbk?output=tile&panoid={pano_id}&zoom={zoom}&x={x}&y={0}'
-            first = Image.open(requests.get(first_url_img, headers=ua, proxies=proxy, stream=True).raw)
-            
-            for y in range(1, vertical_tiles):
-                #new_img = Image.open(f'./images/test_x{x}_y{y}.png')
-                url_new_img = f'https://cbk0.google.com/cbk?output=tile&panoid={pano_id}&zoom={zoom}&x={x}&y={y}'
-                new_img = Image.open(requests.get(url_new_img, headers=ua, proxies=proxy, stream=True).raw)
-                first = ImageTool.concat_vertically(first, new_img)
-
-            new_slice = first
-            first_slice = ImageTool.concat_horizontally(first_slice, new_slice)
+            if x == 0:
+                final_image = first_slice
+            else:
+                final_image = ImageTool.concat_horizontally(final_image, first_slice)
 
-        # first_slice.thumbnail(size, Image.ANTIALIAS)
-        name = f'{out_path}/{identif}'
         if full:
-            image = np.array(first_slice)
-            sun_i = sum(image[-5, :, 1])
-            h, w, c = image.shape
-            h_c = int(h * 0.812)
-            w_c = int(w * 0.812)
-            if sun_i == 0:
-                pre_image = image[0:h_c, 0:w_c]
-            else:
-                pre_image = image
-            pillow_image = Image.fromarray(pre_image)
+            name = f'{out_path}/{identif}'
+            if cropped:
+                h_cropped = final_image.shape[0] // 2
+                final_image = final_image[0:h_cropped, :]
+
             # Validate image before saving
-            if pillow_image.size[0] > 0 and pillow_image.size[1] > 0:
-                pillow_image.save(f'{name}.jpg')
+            if final_image.size[0] > 0 and final_image.size[1] > 0:
+                final_image.save(f'{name}.jpg')
             else:
                 raise ValueError(f"Invalid image for pano_id {pano_id}")
 
-            return identif
+        return identif
+
 
     @staticmethod
-    def dwl_multiple(panoids, zoom, v_tiles, h_tiles, out_path, uas, proxies, cropped=True, full=False, log_path=None):
+    def dwl_multiple(panoids, zoom, v_tiles, h_tiles, out_path, uas, proxies, cropped, full, log_path=None):
         """
         Description of dwl_multiple
         
         Calls the get_and_save_image function using multiple threads.
         
         Args:
             panoids (undefined): GSV anorama id
```

### Comparing `zensvi-0.4.0/src/zensvi/download/utils/proxies.csv` & `zensvi-0.5.0/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.4.0/src/zensvi/transform/transform_image.py` & `zensvi-0.5.0/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.4.0/PKG-INFO` & `zensvi-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.4.0
+Version: 0.5.0
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

