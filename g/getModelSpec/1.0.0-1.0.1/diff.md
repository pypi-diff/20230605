# Comparing `tmp/getModelSpec-1.0.0.tar.gz` & `tmp/getModelSpec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getModelSpec-1.0.0.tar", last modified: Mon Jun  5 00:14:01 2023, max compression
+gzip compressed data, was "dist\getModelSpec-1.0.1.tar", last modified: Mon Jun  5 00:42:14 2023, max compression
```

## Comparing `getModelSpec-1.0.0.tar` & `getModelSpec-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/
--rw-rw-rw-   0        0        0      125 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getModelSpec-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/getModelSpec.egg-info/
--rw-rw-rw-   0        0        0      125 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/getModelSpec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/getModelSpec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/getModelSpec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/getModelSpec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/getModelSpec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/getModelSpec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      412 2023-06-05 00:12:47.000000 getModelSpec-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/src/
--rw-rw-rw-   0        0        0       36 2023-06-04 03:54:37.000000 getModelSpec-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     6516 2023-06-04 23:47:18.000000 getModelSpec-1.0.0/src/sony.py
--rw-rw-rw-   0        0        0     3520 2023-06-04 13:11:45.000000 getModelSpec-1.0.0/src/test.py
-drwxrwxrwx   0        0        0        0 2023-06-05 00:14:01.000000 getModelSpec-1.0.0/tools/
--rw-rw-rw-   0        0        0      169 2023-06-04 09:34:54.000000 getModelSpec-1.0.0/tools/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-06-03 16:09:43.000000 getModelSpec-1.0.0/tools/contents.py
--rw-rw-rw-   0        0        0     5685 2023-06-03 15:59:22.000000 getModelSpec-1.0.0/tools/filesf.py
--rw-rw-rw-   0        0        0      926 2023-06-04 16:42:08.000000 getModelSpec-1.0.0/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/
+-rw-rw-rw-   0        0        0      125 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getModelSpec-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      412 2023-06-05 00:40:28.000000 getModelSpec-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/src/
+-rw-rw-rw-   0        0        0       36 2023-06-04 03:54:37.000000 getModelSpec-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0     6360 2023-06-05 00:22:24.000000 getModelSpec-1.0.1/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/tools/
+-rw-rw-rw-   0        0        0      169 2023-06-04 09:34:54.000000 getModelSpec-1.0.1/tools/__init__.py
+-rw-rw-rw-   0        0        0      926 2023-06-04 16:42:08.000000 getModelSpec-1.0.1/tools/webdriver.py
```

### Comparing `getModelSpec-1.0.0/src/sony.py` & `getModelSpec-1.0.1/src/sony.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,23 @@
 
 
 class GetSONY:
     def __init__(self):
         pass
 
     def getModels(self) -> pd.DataFrame:
-        #
-        # ## 메인 페이지에서 시리즈를 추출
-        # seriesUrls = self.getPage1st(url='https://electronics.sony.com/tv-video/televisions/c/all-tvs')
-        #
-        # ## 서브 시리즈 페이지에서 모델을 추출
-        # dict_allSeries = {}
-        # for url in seriesUrls:
-        #     dict_allSeries.update(self.getPage2nd(url=url))
-        # print("Number of all Series:", len(dict_allSeries))
-
-        import pickle
-        with open('dict_b.pickle', 'rb') as file:
-            dict_allSeries = pickle.load(file)
+
+        ## 메인 페이지에서 시리즈를 추출
+        seriesUrls = self.getPage1st(url='https://electronics.sony.com/tv-video/televisions/c/all-tvs')
+
+        ## 서브 시리즈 페이지에서 모델을 추출
+        dict_allSeries = {}
+        for url in seriesUrls:
+            dict_allSeries.update(self.getPage2nd(url=url))
+        print("Number of all Series:", len(dict_allSeries))
 
         ## 모든 모델 리스트를 추출
         dfModels = pd.DataFrame()
         for model_url in dict_allSeries.values():
             try:
                 dfModel = pd.DataFrame(self.getPage3rd(model_url))
             except:
```

### Comparing `getModelSpec-1.0.0/tools/webdriver.py` & `getModelSpec-1.0.1/tools/webdriver.py`

 * *Files identical despite different names*

