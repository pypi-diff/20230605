# Comparing `tmp/IMDBTraktSyncer-1.3.8.tar.gz` & `tmp/IMDBTraktSyncer-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.3.8.tar", last modified: Mon Jun  5 07:50:41 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.3.9.tar", last modified: Mon Jun  5 07:56:20 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.3.8.tar` & `IMDBTraktSyncer-1.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 07:50:41.410135 IMDBTraktSyncer-1.3.8/
-drwxrwxrwx   0        0        0        0 2023-06-05 07:50:41.376122 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    23157 2023-06-02 06:24:33.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:50:41.407122 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12090 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.8/LICENSE
--rw-rw-rw-   0        0        0    12090 2023-06-05 07:50:41.409122 IMDBTraktSyncer-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    11346 2023-06-05 07:47:27.000000 IMDBTraktSyncer-1.3.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 07:50:41.411122 IMDBTraktSyncer-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-06-05 07:47:51.000000 IMDBTraktSyncer-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:56:20.648797 IMDBTraktSyncer-1.3.9/
+drwxrwxrwx   0        0        0        0 2023-06-05 07:56:20.627798 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    23158 2023-06-05 07:55:19.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:56:20.646798 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12090 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0    12090 2023-06-05 07:56:20.647797 IMDBTraktSyncer-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11346 2023-06-05 07:47:27.000000 IMDBTraktSyncer-1.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:56:20.648797 IMDBTraktSyncer-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-06-05 07:56:14.000000 IMDBTraktSyncer-1.3.9/setup.py
```

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                     response = EH.make_trakt_request(url, payload=data)
                     if response:
                         print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                     else:
                         print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                         print("Error Response:", response.content, response.status_code)
 
-                print('Setting IMDB Watchlist Items Complete')
+                print('Setting Trakt Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
 
             # Set IMDB Watchlist Items
             if imdb_watchlist_to_set:
                 print('Setting IMDB Watchlist Items')
```

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.8
+Version: 1.3.9
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/LICENSE` & `IMDBTraktSyncer-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/PKG-INFO` & `IMDBTraktSyncer-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.8
+Version: 1.3.9
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.8/README.md` & `IMDBTraktSyncer-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.8/setup.py` & `IMDBTraktSyncer-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.8'
+VERSION = '1.3.9'
 DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

