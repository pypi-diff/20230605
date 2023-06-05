# Comparing `tmp/eFatura-1.0.7.tar.gz` & `tmp/eFatura-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.0.7.tar", last modified: Thu May 25 13:26:55 2023, max compression
+gzip compressed data, was "eFatura-1.0.8.tar", last modified: Mon Jun  5 13:39:41 2023, max compression
```

## Comparing `eFatura-1.0.7.tar` & `eFatura-1.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.245590 eFatura-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 13:26:27.000000 eFatura-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-25 13:26:55.245590 eFatura-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-25 13:26:27.000000 eFatura-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.241590 eFatura-1.0.7/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-25 13:26:27.000000 eFatura-1.0.7/Shared/org.KekikAkademi.eFatura.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-25 13:26:27.000000 eFatura-1.0.7/Shared/org.KekikAkademi.eFatura.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-25 13:26:27.000000 eFatura-1.0.7/Shared/org.KekikAkademi.eFatura.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.245590 eFatura-1.0.7/eFatura/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.245590 eFatura-1.0.7/eFatura/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/Assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.245590 eFatura-1.0.7/eFatura/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.245590 eFatura-1.0.7/eFatura/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/GUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.245590 eFatura-1.0.7/eFatura/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-25 13:26:27.000000 eFatura-1.0.7/eFatura/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:26:55.245590 eFatura-1.0.7/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-25 13:26:55.000000 eFatura-1.0.7/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 13:26:55.000000 eFatura-1.0.7/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:26:55.000000 eFatura-1.0.7/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 13:26:55.000000 eFatura-1.0.7/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 13:26:55.000000 eFatura-1.0.7/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 13:26:55.000000 eFatura-1.0.7/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:26:55.245590 eFatura-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-25 13:26:27.000000 eFatura-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 13:39:13.000000 eFatura-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-05 13:39:41.812302 eFatura-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-05 13:39:13.000000 eFatura-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-05 13:39:13.000000 eFatura-1.0.8/Shared/org.KekikAkademi.eFatura.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-05 13:39:13.000000 eFatura-1.0.8/Shared/org.KekikAkademi.eFatura.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-05 13:39:13.000000 eFatura-1.0.8/Shared/org.KekikAkademi.eFatura.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/eFatura/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/eFatura/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/eFatura/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/eFatura/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/eFatura/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-05 13:39:13.000000 eFatura-1.0.8/eFatura/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:39:41.812302 eFatura-1.0.8/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-05 13:39:41.000000 eFatura-1.0.8/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 13:39:41.000000 eFatura-1.0.8/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:39:41.000000 eFatura-1.0.8/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 13:39:41.000000 eFatura-1.0.8/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 13:39:41.000000 eFatura-1.0.8/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 13:39:41.000000 eFatura-1.0.8/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:39:41.812302 eFatura-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-05 13:39:13.000000 eFatura-1.0.8/setup.py
```

### Comparing `eFatura-1.0.7/PKG-INFO` & `eFatura-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.7
+Version: 1.0.8
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/eFatura
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.7 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.8 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
```

### Comparing `eFatura-1.0.7/README.md` & `eFatura-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.7/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.0.8/Shared/org.KekikAkademi.eFatura.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `eFatura-1.0.7/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.0.8/Shared/org.KekikAkademi.eFatura.appdata.xml`

```diff
@@ -28,15 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.7" date="2023-5-25">
+    <release version="1.0.8" date="2023-6-5">
       <description>
         <p>Çeşitli iyileştirmeler yapıldı..</p>
       </description>
     </release>
     <release version="1.0.5" date="2023-5-23"/>
     <release version="0.0.1" date="2022-8-13"/>
   </releases>
```

### Comparing `eFatura-1.0.7/Shared/org.KekikAkademi.eFatura.svg` & `eFatura-1.0.8/Shared/org.KekikAkademi.eFatura.svg`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.7/eFatura/Assets/logo.png` & `eFatura-1.0.8/eFatura/Assets/logo.png`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.7/eFatura/Core/__init__.py` & `eFatura-1.0.8/eFatura/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.7/eFatura/Libs/Oturum.py` & `eFatura-1.0.8/eFatura/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.7/eFatura/konsol.py` & `eFatura-1.0.8/eFatura/konsol.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.7/eFatura.egg-info/PKG-INFO` & `eFatura-1.0.8/eFatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.7
+Version: 1.0.8
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/eFatura
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.7 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.8 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
```

### Comparing `eFatura-1.0.7/eFatura.egg-info/SOURCES.txt` & `eFatura-1.0.8/eFatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.7/setup.py` & `eFatura-1.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.0.7",
+    version      = "1.0.8",
     url          = "https://github.com/keyiflerolsun/eFatura",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

