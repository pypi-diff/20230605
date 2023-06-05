# Comparing `tmp/getmodelspec-1.0.15.tar.gz` & `tmp/getmodelspec-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.15.tar", last modified: Mon Jun  5 15:48:15 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.16.tar", last modified: Mon Jun  5 16:12:24 2023, max compression
```

## Comparing `getmodelspec-1.0.15.tar` & `getmodelspec-1.0.16.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/
--rw-rw-rw-   0        0        0      126 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.15/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec/
--rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.15/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.15/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0     9866 2023-06-05 15:47:40.000000 getmodelspec-1.0.15/getmodelspec/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.15/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0      906 2023-06-05 14:59:18.000000 getmodelspec-1.0.15/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-05 15:47:57.000000 getmodelspec-1.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/
+-rw-rw-rw-   0        0        0      126 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.16/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec/
+-rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.16/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.16/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0     9864 2023-06-05 16:10:23.000000 getmodelspec-1.0.16/getmodelspec/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.16/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0      906 2023-06-05 14:59:18.000000 getmodelspec-1.0.16/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:12:24.000000 getmodelspec-1.0.16/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-05 16:12:06.000000 getmodelspec-1.0.16/setup.py
```

### Comparing `getmodelspec-1.0.15/getmodelspec/src/sony.py` & `getmodelspec-1.0.16/getmodelspec/src/sony.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         for cntTry in range(5):
             try:
                 dictSpec = {}
                 wd = WebDriver.get_crome()
                 wd.get(url=url)
                 wait = WebDriverWait(wd, self.watingTime)
-                # self.waitingPage(1)
+                self.waitingPage(1)
 
                 #모델 정보 확인
                 model = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'product-intro__code'))).text.replace("Model: ", "")
                 dictSpec["Descr"] = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'product-intro__title'))).text.strip()
 
                 #가격 정보 확인
                 try: dictSpec["price"] = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'custom-product-summary__price'))).text
```

### Comparing `getmodelspec-1.0.15/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.16/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

