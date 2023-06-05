# Comparing `tmp/pytyper_weather_forecast-0.1.0.tar.gz` & `tmp/pytyper_weather_forecast-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytyper_weather_forecast-0.1.0.tar", max compression
+gzip compressed data, was "pytyper_weather_forecast-0.2.0.tar", max compression
```

## Comparing `pytyper_weather_forecast-0.1.0.tar` & `pytyper_weather_forecast-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      548 2023-06-04 15:20:41.743472 pytyper_weather_forecast-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 12:01:41.658708 pytyper_weather_forecast-0.1.0/pytyper_weather_forecast/__init__.py
--rw-r--r--   0        0        0     2474 2023-06-04 15:25:15.467838 pytyper_weather_forecast-0.1.0/pytyper_weather_forecast/main.py
--rw-r--r--   0        0        0        0 2023-06-04 12:01:41.658708 pytyper_weather_forecast-0.1.0/README.md
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 pytyper_weather_forecast-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-06-05 06:46:23.501351 pytyper_weather_forecast-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-04 12:01:41.658708 pytyper_weather_forecast-0.2.0/pytyper_weather_forecast/__init__.py
+-rw-r--r--   0        0        0     2474 2023-06-04 15:25:15.467838 pytyper_weather_forecast-0.2.0/pytyper_weather_forecast/main.py
+-rw-r--r--   0        0        0      463 2023-06-05 06:45:18.453339 pytyper_weather_forecast-0.2.0/README.md
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 pytyper_weather_forecast-0.2.0/PKG-INFO
```

### Comparing `pytyper_weather_forecast-0.1.0/pyproject.toml` & `pytyper_weather_forecast-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pytyper-weather-forecast"
-version = "0.1.0"
-description = ""
+version = "0.2.0"
+description = "Weather Forecasting Package"
 authors = ["anugoyal998 <anugoyal998@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pytyper_weather_forecast"}]
 
 [tool.poetry.scripts]
 pytyper-weather-forecast = "pytyper_weather_forecast.main:app"
```

### Comparing `pytyper_weather_forecast-0.1.0/pytyper_weather_forecast/main.py` & `pytyper_weather_forecast-0.2.0/pytyper_weather_forecast/main.py`

 * *Files identical despite different names*

