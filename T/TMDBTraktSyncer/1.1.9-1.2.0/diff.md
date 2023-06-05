# Comparing `tmp/TMDBTraktSyncer-1.1.9.tar.gz` & `tmp/TMDBTraktSyncer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.1.9.tar", last modified: Sun May 28 13:33:31 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.2.0.tar", last modified: Mon Jun  5 08:05:09 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.1.9.tar` & `TMDBTraktSyncer-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 13:33:31.546707 TMDBTraktSyncer-1.1.9/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.9/LICENSE
--rw-rw-rw-   0        0        0    10672 2023-05-28 13:33:31.546707 TMDBTraktSyncer-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     9927 2023-05-28 12:50:14.000000 TMDBTraktSyncer-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 13:33:31.520036 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    10142 2023-05-24 01:26:25.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:31:50.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8916 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     3952 2023-05-24 00:42:48.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     3037 2023-05-24 00:45:06.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     3325 2023-05-24 00:34:12.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:33:31.544038 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    10672 2023-05-28 13:33:31.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-05-28 13:33:31.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 13:33:31.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-28 13:33:31.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 13:33:31.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 13:33:31.000000 TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 13:33:31.547709 TMDBTraktSyncer-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1334 2023-05-28 13:33:16.000000 TMDBTraktSyncer-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:05:09.555062 TMDBTraktSyncer-1.2.0/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10794 2023-06-05 08:05:09.554074 TMDBTraktSyncer-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10048 2023-06-05 08:01:07.000000 TMDBTraktSyncer-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 08:05:09.523999 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    10142 2023-06-02 06:29:12.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:31:50.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8916 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     3952 2023-05-24 00:42:48.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     3046 2023-05-31 11:17:57.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     3325 2023-05-24 00:34:12.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:05:09.552073 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    10794 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 08:05:09.555062 TMDBTraktSyncer-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1334 2023-06-05 08:04:41.000000 TMDBTraktSyncer-1.2.0/setup.py
```

### Comparing `TMDBTraktSyncer-1.1.9/LICENSE` & `TMDBTraktSyncer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.9/PKG-INFO` & `TMDBTraktSyncer-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.9
+Version: 1.2.0
 Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,16 @@
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `localhost`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
 6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
@@ -79,14 +79,15 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add optional setting to remove watched items from watchlists [Issue #15](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/15)
 * Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 ## Sponsorships, Donations, and Custom Projects:
```

### Comparing `TMDBTraktSyncer-1.1.9/README.md` & `TMDBTraktSyncer-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `localhost`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
 6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
@@ -63,14 +63,15 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add optional setting to remove watched items from watchlists [Issue #15](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/15)
 * Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 ## Sponsorships, Donations, and Custom Projects:
```

### Comparing `TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                     response = EH.make_trakt_request(url, payload=data)
                     if response:
                         print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                     else:
                         print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist (TMDB ID: {item['ID']})")
                         print("Error Response:", response.content, response.status_code)
 
-                print('Trakt Watchlist Items Set Successfully')
+                print('Setting Trakt Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
 
         if tmdb_ratings_to_set:
             print('Setting TMDB Ratings')
             
             # Count the total number of items to rate
```

### Comparing `TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/traktData.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,10 +64,10 @@
                 'Episode': episode.get('number'),
                 'ShowID': show_tmdb_id,
                 'Type': 'episode'
             })
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
-    print('Processing Trakt Data')
+    print('Processing Trakt Data Complete')
     
     return trakt_watchlist, trakt_ratings
```

### Comparing `TMDBTraktSyncer-1.1.9/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.9/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.9
+Version: 1.2.0
 Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,16 @@
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `localhost`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
 6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
@@ -79,14 +79,15 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add optional setting to remove watched items from watchlists [Issue #15](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/15)
 * Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 ## Sponsorships, Donations, and Custom Projects:
```

### Comparing `TMDBTraktSyncer-1.1.9/setup.py` & `TMDBTraktSyncer-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.9'
+VERSION = '1.2.0'
 DESCRIPTION = 'This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

