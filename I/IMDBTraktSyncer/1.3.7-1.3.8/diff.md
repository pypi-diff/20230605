# Comparing `tmp/IMDBTraktSyncer-1.3.7.tar.gz` & `tmp/IMDBTraktSyncer-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.3.7.tar", last modified: Mon May 29 23:54:34 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.3.8.tar", last modified: Mon Jun  5 07:50:41 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.3.7.tar` & `IMDBTraktSyncer-1.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 23:54:34.263412 IMDBTraktSyncer-1.3.7/
-drwxrwxrwx   0        0        0        0 2023-05-29 23:54:34.240860 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    23158 2023-05-29 23:53:46.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-05-28 12:08:18.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-29 23:54:34.260413 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    11969 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.7/LICENSE
--rw-rw-rw-   0        0        0    11969 2023-05-29 23:54:34.261414 IMDBTraktSyncer-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    11226 2023-05-29 23:50:45.000000 IMDBTraktSyncer-1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 23:54:34.263412 IMDBTraktSyncer-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-05-29 23:54:31.000000 IMDBTraktSyncer-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:50:41.410135 IMDBTraktSyncer-1.3.8/
+drwxrwxrwx   0        0        0        0 2023-06-05 07:50:41.376122 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    23157 2023-06-02 06:24:33.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:50:41.407122 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12090 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 07:50:41.000000 IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.8/LICENSE
+-rw-rw-rw-   0        0        0    12090 2023-06-05 07:50:41.409122 IMDBTraktSyncer-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11346 2023-06-05 07:47:27.000000 IMDBTraktSyncer-1.3.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:50:41.411122 IMDBTraktSyncer-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-06-05 07:47:51.000000 IMDBTraktSyncer-1.3.8/setup.py
```

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                     response = EH.make_trakt_request(url, payload=data)
                     if response:
                         print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                     else:
                         print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                         print("Error Response:", response.content, response.status_code)
 
-                print('Trakt Watchlist Items Set Successfully')
+                print('Setting IMDB Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
 
             # Set IMDB Watchlist Items
             if imdb_watchlist_to_set:
                 print('Setting IMDB Watchlist Items')
```

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/checkChromedriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,24 +36,24 @@
         except:
             return None
 
     return None
 
 def install_chromedriver(version):
     # Install the chromedriver-py package using the Python interpreter
-    subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir' f'chromedriver-py=={version}'])
+    subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir', f'chromedriver-py=={version}'])
 
 def install_chromedriver_fallback_method():
     print("Using install chromedriver-py fallback method")
     # Install the chromedriver-py package using the Python interpreter
     feed = feedparser.parse('https://pypi.org/rss/project/chromedriver-py/releases.xml')
     # Get the second latest release version
     version = feed.entries[1].title.split()[-1]
     # Install the chromedriver-py package using pip
-    subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir' f'chromedriver-py=={version}'])
+    subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir', f'chromedriver-py=={version}'])
 
 # Check if chromedriver-py is already installed
 try:
     dist = pkg_resources.get_distribution('chromedriver-py')
     installed_version = dist.version.split('.')[0]  # Retrieve only the prefix
     chrome_version = get_chrome_version()
```

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.7
+Version: 1.3.8
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
 
-The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
+The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
@@ -70,14 +70,15 @@
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
+- Add optional setting to remove watched items from watchlists [Issue #44](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/44)
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
```

### Comparing `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.3.8/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.7/LICENSE` & `IMDBTraktSyncer-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.7/PKG-INFO` & `IMDBTraktSyncer-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.7
+Version: 1.3.8
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
 
-The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
+The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
@@ -70,14 +70,15 @@
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
+- Add optional setting to remove watched items from watchlists [Issue #44](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/44)
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
```

### Comparing `IMDBTraktSyncer-1.3.7/README.md` & `IMDBTraktSyncer-1.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
 
-The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
+The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
@@ -54,14 +54,15 @@
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
+- Add optional setting to remove watched items from watchlists [Issue #44](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/44)
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
```

### Comparing `IMDBTraktSyncer-1.3.7/setup.py` & `IMDBTraktSyncer-1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.7'
+VERSION = '1.3.8'
 DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

