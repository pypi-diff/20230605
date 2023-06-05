# Comparing `tmp/spotON_sdk-0.0.5.22.tar.gz` & `tmp/spotON_sdk-0.0.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.5.22.tar", last modified: Fri Jun  2 15:17:51 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.5.23.tar", last modified: Mon Jun  5 09:14:46 2023, max compression
```

## Comparing `spotON_sdk-0.0.5.22.tar` & `spotON_sdk-0.0.5.23.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.22/.gitignore
--rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.22/.gitmodules
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.22/LICENSE
--rw-r--r--   0        0        0      390 2023-06-02 15:16:16.082148 spotON_sdk-0.0.5.22/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-06-01 17:11:50.585857 spotON_sdk-0.0.5.22/spotON_sdk/API/API_Call.py
--rw-r--r--   0        0        0      101 2023-06-01 17:06:55.423781 spotON_sdk-0.0.5.22/spotON_sdk/API/__init__.py
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      239 2023-06-01 17:02:39.339895 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/customBaseModel.py
--rw-r--r--   0        0        0     3012 2023-06-01 08:37:08.552222 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     8239 2023-05-29 07:59:04.654185 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-06-01 17:04:16.714855 spotON_sdk-0.0.5.22/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      478 2023-06-02 15:17:45.500099 spotON_sdk-0.0.5.22/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.22/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.22/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.22/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.22/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.22/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.23/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.23/.gitmodules
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.23/LICENSE
+-rw-r--r--   0        0        0      380 2023-06-05 09:14:07.440703 spotON_sdk-0.0.5.23/pyproject.toml
+-rw-r--r--   0        0        0     1225 2023-06-02 16:15:25.317306 spotON_sdk-0.0.5.23/spotON_sdk/API/API_Call.py
+-rw-r--r--   0        0        0      101 2023-06-01 17:06:55.423781 spotON_sdk-0.0.5.23/spotON_sdk/API/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      239 2023-06-01 17:02:39.339895 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/customBaseModel.py
+-rw-r--r--   0        0        0     3012 2023-06-01 08:37:08.552222 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     8239 2023-05-29 07:59:04.654185 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-06-01 17:04:16.714855 spotON_sdk-0.0.5.23/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-05 09:14:34.879573 spotON_sdk-0.0.5.23/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.23/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.23/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.23/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.23/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.23/PKG-INFO
```

### Comparing `spotON_sdk-0.0.5.22/.gitignore` & `spotON_sdk-0.0.5.23/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/LICENSE` & `spotON_sdk-0.0.5.23/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/API/API_Call.py` & `spotON_sdk-0.0.5.23/spotON_sdk/API/API_Call.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import aiohttp
 import json
 
 from spotON_sdk import Price_Logic,Continuous_On_Time,Markets,Timeframes
 
 async def request_Day_Ahead_Price(data:API_Call):
+           
     url = 'https://km28t5snp5.execute-api.eu-central-1.amazonaws.com/Prod/echo'
     #url = 'http://127.0.0.1:8000/echo'
 
 
 
     headers = {'Content-type': 'application/json'} # Set the content type to JSON
```

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.5.23/spotON_sdk/Logic/Price/timeframes.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.5.23/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.22/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.5.23/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

