# Comparing `tmp/lesscode_charts-0.0.3.tar.gz` & `tmp/lesscode_charts-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_charts-0.0.3.tar", last modified: Wed May 31 10:57:16 2023, max compression
+gzip compressed data, was "dist/lesscode_charts-0.0.4.tar", last modified: Mon Jun  5 09:16:39 2023, max compression
```

## Comparing `lesscode_charts-0.0.3.tar` & `lesscode_charts-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.3/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.3/lesscode_charts/__init__.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts/utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.3/lesscode_charts/utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.3/lesscode_charts/utils/common_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts/v1/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.3/lesscode_charts/v1/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.3/lesscode_charts/v1/forest_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     2106 2023-05-19 07:48:32.000000 lesscode_charts-0.0.3/lesscode_charts/v1/histogram_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.3/lesscode_charts/v1/k_line_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1437 2023-05-19 03:41:10.000000 lesscode_charts-0.0.3/lesscode_charts/v1/pie_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1058 2023-05-19 07:29:22.000000 lesscode_charts-0.0.3/lesscode_charts/v1/pyramid_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.3/lesscode_charts/v1/radar_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 10:57:13.000000 lesscode_charts-0.0.3/lesscode_charts/v1/sankey_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.3/lesscode_charts/v1/table_chart.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-05-31 10:57:13.000000 lesscode_charts-0.0.3/lesscode_charts/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      611 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.3/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.4/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.4/lesscode_charts/__init__.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts/utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.4/lesscode_charts/utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.4/lesscode_charts/utils/common_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts/v1/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.4/lesscode_charts/v1/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.4/lesscode_charts/v1/forest_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3459 2023-06-05 09:16:34.000000 lesscode_charts-0.0.4/lesscode_charts/v1/histogram_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.4/lesscode_charts/v1/k_line_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1437 2023-05-19 03:41:10.000000 lesscode_charts-0.0.4/lesscode_charts/v1/pie_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1058 2023-05-19 07:29:22.000000 lesscode_charts-0.0.4/lesscode_charts/v1/pyramid_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.4/lesscode_charts/v1/radar_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 11:03:04.000000 lesscode_charts-0.0.4/lesscode_charts/v1/sankey_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.4/lesscode_charts/v1/table_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-05 09:16:34.000000 lesscode_charts-0.0.4/lesscode_charts/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      611 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/lesscode_charts.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-05 09:16:39.000000 lesscode_charts-0.0.4/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.4/setup.py
```

### Comparing `lesscode_charts-0.0.3/lesscode_charts/utils/common_utils.py` & `lesscode_charts-0.0.4/lesscode_charts/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/lesscode_charts/v1/forest_chart.py` & `lesscode_charts-0.0.4/lesscode_charts/v1/forest_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/lesscode_charts/v1/k_line_chart.py` & `lesscode_charts-0.0.4/lesscode_charts/v1/k_line_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/lesscode_charts/v1/pie_chart.py` & `lesscode_charts-0.0.4/lesscode_charts/v1/pie_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/lesscode_charts/v1/pyramid_chart.py` & `lesscode_charts-0.0.4/lesscode_charts/v1/pyramid_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/lesscode_charts/v1/radar_chart.py` & `lesscode_charts-0.0.4/lesscode_charts/v1/radar_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/lesscode_charts/v1/sankey_chart.py` & `lesscode_charts-0.0.4/lesscode_charts/v1/sankey_chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class SankeyChart:
     @staticmethod
     def sankey(data: List[dict], title: str = "", data_key="id", parent_key="parent_id", **kwargs):
         """
         :param parent_key: 父级key
         :param data_key: 数据key
         :param title: 图题
-        :param data: 数据,示例：[{"id": "INB133001", "config": {"title": "感知设备与服务", "value": "value1", "depth": 2}, "parent_id": "INB1330"},
-                                {"id": "INB1330", "config": {"title": "感知设备", "value": "value2", "depth": 1}, "parent_id": None}]
+        :param data: 数据,示例：[{"id": "INB133001", "config": {"label": "感知设备与服务", "value": "value1", "depth": 2}, "parent_id": "INB1330"},
+                                {"id": "INB1330", "config": {"label": "感知设备", "value": "value2", "depth": 1}, "parent_id": None}]
         :return:
         """
         data_list = []
         link_list = []
         data_map = {item.get(data_key): item for item in data if item.get(data_key)}
         tmp = dict()
         for item in data:
```

### Comparing `lesscode_charts-0.0.3/lesscode_charts/v1/table_chart.py` & `lesscode_charts-0.0.4/lesscode_charts/v1/table_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/lesscode_charts.egg-info/SOURCES.txt` & `lesscode_charts-0.0.4/lesscode_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.3/setup.py` & `lesscode_charts-0.0.4/setup.py`

 * *Files identical despite different names*

