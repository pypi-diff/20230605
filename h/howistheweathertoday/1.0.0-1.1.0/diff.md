# Comparing `tmp/howistheweathertoday-1.0.0.tar.gz` & `tmp/howistheweathertoday-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "howistheweathertoday-1.0.0.tar", last modified: Mon Jun  5 17:10:16 2023, max compression
+gzip compressed data, was "howistheweathertoday-1.1.0.tar", last modified: Mon Jun  5 17:30:57 2023, max compression
```

## Comparing `howistheweathertoday-1.0.0.tar` & `howistheweathertoday-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:10:16.417246 howistheweathertoday-1.0.0/
--rw-rw-rw-   0        0        0      218 2023-06-05 17:10:16.417246 howistheweathertoday-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 17:10:16.401109 howistheweathertoday-1.0.0/howistheweathertoday/
--rw-rw-rw-   0        0        0       61 2023-06-05 17:09:33.000000 howistheweathertoday-1.0.0/howistheweathertoday/__init__.py
--rw-rw-rw-   0        0        0     1290 2023-06-05 16:43:55.000000 howistheweathertoday-1.0.0/howistheweathertoday/howistheweathertoday.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:10:16.416245 howistheweathertoday-1.0.0/howistheweathertoday.egg-info/
--rw-rw-rw-   0        0        0      218 2023-06-05 17:10:16.000000 howistheweathertoday-1.0.0/howistheweathertoday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-05 17:10:16.000000 howistheweathertoday-1.0.0/howistheweathertoday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:10:16.000000 howistheweathertoday-1.0.0/howistheweathertoday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 17:10:16.000000 howistheweathertoday-1.0.0/howistheweathertoday.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-05 17:10:16.000000 howistheweathertoday-1.0.0/howistheweathertoday.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 17:10:16.418247 howistheweathertoday-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      365 2023-06-05 17:08:54.000000 howistheweathertoday-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:30:57.559330 howistheweathertoday-1.1.0/
+-rw-rw-rw-   0        0        0      218 2023-06-05 17:30:57.559330 howistheweathertoday-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 17:30:57.548292 howistheweathertoday-1.1.0/howistheweathertoday/
+-rw-rw-rw-   0        0        0       61 2023-06-05 17:09:33.000000 howistheweathertoday-1.1.0/howistheweathertoday/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-06-05 17:20:37.000000 howistheweathertoday-1.1.0/howistheweathertoday/howistheweathertoday.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:30:57.558329 howistheweathertoday-1.1.0/howistheweathertoday.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-06-05 17:30:57.000000 howistheweathertoday-1.1.0/howistheweathertoday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-06-05 17:30:57.000000 howistheweathertoday-1.1.0/howistheweathertoday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:30:57.000000 howistheweathertoday-1.1.0/howistheweathertoday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 17:30:57.000000 howistheweathertoday-1.1.0/howistheweathertoday.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-05 17:30:57.000000 howistheweathertoday-1.1.0/howistheweathertoday.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:30:57.559330 howistheweathertoday-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      365 2023-06-05 17:30:50.000000 howistheweathertoday-1.1.0/setup.py
```

### Comparing `howistheweathertoday-1.0.0/howistheweathertoday/howistheweathertoday.py` & `howistheweathertoday-1.1.0/howistheweathertoday/howistheweathertoday.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 
     def next_12h(self):
         return self.data["list"][:4]
 
     def next_12h_simplified(self):
         simple_data = []
         for dicty in self.data["list"][:4]:
-            simple_data.append((dicty["dt_txt"],dicty["main"]["temp"],dicty["weather"][0]["description"]))
+            simple_data.append((dicty["dt_txt"],dicty["main"]["temp"],dicty["weather"][0]["description"],dicty["weather"][0]["icon"]))
         return simple_data
```

