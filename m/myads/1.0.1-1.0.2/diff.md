# Comparing `tmp/myads-1.0.1.tar.gz` & `tmp/myads-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myads-1.0.1.tar", last modified: Wed Apr 19 21:51:55 2023, max compression
+gzip compressed data, was "myads-1.0.2.tar", last modified: Mon Jun  5 01:14:49 2023, max compression
```

## Comparing `myads-1.0.1.tar` & `myads-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4612 2023-04-19 21:51:55.989712 myads-1.0.1/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4252 2023-04-19 21:50:51.000000 myads-1.0.1/README.md
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      732 2023-04-19 21:50:17.000000 myads-1.0.1/pyproject.toml
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-04-19 21:51:55.989712 myads-1.0.1/setup.cfg
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      769 2023-03-12 18:51:04.000000 myads-1.0.1/src/myads/__init__.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads/cite_tracker/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      595 2023-03-26 17:34:24.000000 myads-1.0.1/src/myads/cite_tracker/__init__.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     6611 2023-04-19 21:48:51.000000 myads-1.0.1/src/myads/cite_tracker/check.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2276 2023-04-19 21:46:53.000000 myads-1.0.1/src/myads/cite_tracker/report.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3256 2023-03-26 17:39:40.000000 myads-1.0.1/src/myads/cite_tracker/users.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     9957 2023-04-19 21:46:45.000000 myads-1.0.1/src/myads/query.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads/scripts/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     1684 2023-04-02 09:41:52.000000 myads-1.0.1/src/myads/scripts/myads.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads.egg-info/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4612 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      424 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/SOURCES.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/dependency_links.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/entry_points.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/requires.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/top_level.txt
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.252777 myads-1.0.2/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 01:14:49.252777 myads-1.0.2/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4241 2023-06-05 01:04:37.000000 myads-1.0.2/README.md
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      865 2023-06-05 01:13:52.000000 myads-1.0.2/pyproject.toml
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-06-05 01:14:49.252777 myads-1.0.2/setup.cfg
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.248777 myads-1.0.2/src/
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.248777 myads-1.0.2/src/myads/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      769 2023-03-12 18:51:04.000000 myads-1.0.2/src/myads/__init__.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.252777 myads-1.0.2/src/myads/cite_tracker/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      614 2023-06-05 00:53:50.000000 myads-1.0.2/src/myads/cite_tracker/__init__.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     6631 2023-06-05 01:10:30.000000 myads-1.0.2/src/myads/cite_tracker/check.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2276 2023-04-19 21:46:53.000000 myads-1.0.2/src/myads/cite_tracker/report.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3282 2023-06-05 00:51:56.000000 myads-1.0.2/src/myads/cite_tracker/users.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     9957 2023-04-19 21:46:45.000000 myads-1.0.2/src/myads/query.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.252777 myads-1.0.2/src/myads/scripts/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2620 2023-06-05 01:05:08.000000 myads-1.0.2/src/myads/scripts/myads.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.248777 myads-1.0.2/src/myads.egg-info/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      424 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/entry_points.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/requires.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/top_level.txt
```

### Comparing `myads-1.0.1/PKG-INFO` & `myads-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1
-Name: myads
-Version: 1.0.1
-Summary: Simple ADS API query package and citation tracker
-Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
-License: BSD 3-Clause License
-Keywords: nasa-ads,citations,astronomy,ads,python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 [![PyPI version](https://badge.fury.io/py/myads.svg)](https://badge.fury.io/py/myads)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/myads?logo=python)
 
 # myADS
 
 `myADS` is a simple package to keep track of citations to your (and other
 authors) papers.
 
-It both reports your current papers citation metrics, and
-checks for any new cites to your papers since the last time of checking.
+It both reports the authors current paper citation metrics, and checks for any
+new cites to the authors papers since the last time of checking.
 
 Once installed you can always run `myads --help` to see a list of available
 commands.
 
 ## Installation
 
 The easiest method is to install directly from
@@ -39,63 +28,61 @@
 * Clone the repository using ``git clone
   https://github.com/stuartmcalpine/myADS.git``
 * Navigate to the ``myADS`` folder
 * Install using `pip install .`
 
 ## Getting set up
 
-``myADS`` can keep track of the citations for multiple users. Two steps before
-you get started:
+``myADS`` can keep track of the citations for multiple authors. Two steps
+before you get started:
 
-* Add your users to the database
+* Add your authors you want to track to the database
 * Add your ADS API token to the database
 
-### Adding a user to the database
+### Adding a author to the database
 
-Once `myADS` is installed you can add users to the tracking database using:
+Once `myADS` is installed you can add the authors you wish to track using:
 
 ```bash
-myads --add_user
+myads author add
 ```
 
 You will be prompted to enter a first and last name, and an optional ORCID
-(however it is recommended you add this for each user when possible).
+(however it is recommended you add this for each author when possible).
 
-### Removing a user from the database
+### Removing a author from the database
 
-You can remove users from the tracking database using:
+You can remove authors from the tracking database using:
 
 ```bash
-myads --remove_user
+myads author remove <author id>
 ```
 
-where you will be prompted to enter the users unique tracking ID.
-
-You can get a list of tracking IDs by typing:
+You can get a list of author IDs by typing:
 
 ```bash
-myads --list_users
+myads author list
 ```
 
 ### Adding your ADS API token
 
 You must add your [ADS API token](https://ui.adsabs.harvard.edu/help/api/) so
 the package can query on your behalf. 
 
 To add it run:
 
 ```bash
---set_ads_token <YOUR-API-TOKEN-HERE>
+myads token add <YOUR-API-TOKEN-HERE>
 ```
 
 ## Usage
 
 ### Citation reporter
 
-If you run `myads --report` you will get a report of all your registered users
+If you run `myads report` you will get a report of all your tracked authors
 current citations, e.g.,
 
 ```bash
 Reporting cites for Stuart McAlpine...
 +----------------------------------------------------+--------------+---------------+---------------------+
 | Title                                              | Citations    | Publication   | Bibcode             |
 |                                                    | (per year)   | Date          |                     |
@@ -104,16 +91,16 @@
 | significant amount of black hole growth yet do     |              |               |                     |
 | increase the rate of luminous AGN                  |              |               |                     |
 +----------------------------------------------------+--------------+---------------+---------------------+
 ```
 
 ### Citation tracker
 
-If you run `myads --check` it will tell you any papers that have cited your
-users papers since the last call. 
+If you run `myads check` it will tell you any papers that have cited your
+tracked authors papers since the last call. 
 
 The first time you run this it will create a local database of your citations.
 From then on it will update the local database with your new cites and report
 the changes, e.g.,
 
 ```bash
  1 new cite(s) for Galaxy mergers in EAGLE do not induce a significant amount of black hole growth yet do increase the rate of luminous AGN
```

### Comparing `myads-1.0.1/README.md` & `myads-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,30 @@
+Metadata-Version: 2.1
+Name: myads
+Version: 1.0.2
+Summary: Simple ADS API query package and citation tracker
+Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
+License: BSD 3-Clause License
+Project-URL: homepage, https://github.com/stuartmcalpine/myADS
+Project-URL: repository, https://github.com/stuartmcalpine/myADS
+Keywords: nasa-ads,citations,astronomy,ads,python,arxiv
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 [![PyPI version](https://badge.fury.io/py/myads.svg)](https://badge.fury.io/py/myads)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/myads?logo=python)
 
 # myADS
 
 `myADS` is a simple package to keep track of citations to your (and other
 authors) papers.
 
-It both reports your current papers citation metrics, and
-checks for any new cites to your papers since the last time of checking.
+It both reports the authors current paper citation metrics, and checks for any
+new cites to the authors papers since the last time of checking.
 
 Once installed you can always run `myads --help` to see a list of available
 commands.
 
 ## Installation
 
 The easiest method is to install directly from
@@ -28,63 +41,61 @@
 * Clone the repository using ``git clone
   https://github.com/stuartmcalpine/myADS.git``
 * Navigate to the ``myADS`` folder
 * Install using `pip install .`
 
 ## Getting set up
 
-``myADS`` can keep track of the citations for multiple users. Two steps before
-you get started:
+``myADS`` can keep track of the citations for multiple authors. Two steps
+before you get started:
 
-* Add your users to the database
+* Add your authors you want to track to the database
 * Add your ADS API token to the database
 
-### Adding a user to the database
+### Adding a author to the database
 
-Once `myADS` is installed you can add users to the tracking database using:
+Once `myADS` is installed you can add the authors you wish to track using:
 
 ```bash
-myads --add_user
+myads author add
 ```
 
 You will be prompted to enter a first and last name, and an optional ORCID
-(however it is recommended you add this for each user when possible).
+(however it is recommended you add this for each author when possible).
 
-### Removing a user from the database
+### Removing a author from the database
 
-You can remove users from the tracking database using:
+You can remove authors from the tracking database using:
 
 ```bash
-myads --remove_user
+myads author remove <author id>
 ```
 
-where you will be prompted to enter the users unique tracking ID.
-
-You can get a list of tracking IDs by typing:
+You can get a list of author IDs by typing:
 
 ```bash
-myads --list_users
+myads author list
 ```
 
 ### Adding your ADS API token
 
 You must add your [ADS API token](https://ui.adsabs.harvard.edu/help/api/) so
 the package can query on your behalf. 
 
 To add it run:
 
 ```bash
---set_ads_token <YOUR-API-TOKEN-HERE>
+myads token add <YOUR-API-TOKEN-HERE>
 ```
 
 ## Usage
 
 ### Citation reporter
 
-If you run `myads --report` you will get a report of all your registered users
+If you run `myads report` you will get a report of all your tracked authors
 current citations, e.g.,
 
 ```bash
 Reporting cites for Stuart McAlpine...
 +----------------------------------------------------+--------------+---------------+---------------------+
 | Title                                              | Citations    | Publication   | Bibcode             |
 |                                                    | (per year)   | Date          |                     |
@@ -93,16 +104,16 @@
 | significant amount of black hole growth yet do     |              |               |                     |
 | increase the rate of luminous AGN                  |              |               |                     |
 +----------------------------------------------------+--------------+---------------+---------------------+
 ```
 
 ### Citation tracker
 
-If you run `myads --check` it will tell you any papers that have cited your
-users papers since the last call. 
+If you run `myads check` it will tell you any papers that have cited your
+tracked authors papers since the last call. 
 
 The first time you run this it will create a local database of your citations.
 From then on it will update the local database with your new cites and report
 the changes, e.g.,
 
 ```bash
  1 new cite(s) for Galaxy mergers in EAGLE do not induce a significant amount of black hole growth yet do increase the rate of luminous AGN
```

### Comparing `myads-1.0.1/pyproject.toml` & `myads-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 ]
 dependencies = [
     'requests',
     'toml',
     'tabulate>=0.9.0'
 ]
 requires-python = ">=3.7"
-version = "1.0.1"
-keywords = ["nasa-ads", "citations", "astronomy", "ads", "python"]
+version = "1.0.2"
+keywords = ["nasa-ads", "citations", "astronomy", "ads", "python", "arxiv"]
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 
 [project.scripts]
 myads = "myads.scripts.myads:main"
+
+[project.urls]
+homepage = "https://github.com/stuartmcalpine/myADS"
+repository = "https://github.com/stuartmcalpine/myADS"
```

### Comparing `myads-1.0.1/src/myads/__init__.py` & `myads-1.0.2/src/myads/__init__.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.1/src/myads/cite_tracker/check.py` & `myads-1.0.2/src/myads/cite_tracker/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,20 +162,20 @@
             database = toml.load(user_database)
 
             # Is there a new paper for this user that's not in the database?
             for tmp_paper in data.papers:
                 if tmp_paper.bibcode not in database.keys():
                     brand_new_paper = True
                     print(
-                        f"New paper for {FIRST_NAME} {LAST_NAME} ({bibcode})",
+                        f"New paper for {FIRST_NAME} {LAST_NAME} ({tmp_paper.bibcode})",
                         f"adding to database...",
                     )
 
                     # Add new entry to database.
-                    database[bibcode] = {"title": tmp_paper.title, "citations": []}
+                    database[tmp_paper.bibcode] = {"title": tmp_paper.title, "citations": []}
 
             new_entry = False
 
             # Loop over each paper in database.
             for bibcode in database.keys():
                 if verbose:
                     print(f"Checking {bibcode}...")
```

### Comparing `myads-1.0.1/src/myads/cite_tracker/report.py` & `myads-1.0.2/src/myads/cite_tracker/report.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.1/src/myads/cite_tracker/users.py` & `myads-1.0.2/src/myads/cite_tracker/users.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,14 +41,19 @@
     for att in data.keys():
         if "user" in att:
             print(
                 f"{att}: {data[att]['first_name']} {data[att]['last_name']}",
                 f"(ORCID={data[att]['orcid']})",
             )
 
+def display_ads_token():
+    """ Print all ADS API tokens in the database. """
+
+    data = _load_user_database()
+
     if "ads_token" in data["metadata"].keys():
         print(f"ADS token: {data['metadata']['ads_token']}")
     else:
         print("No ADS token added yet...")
 
 
 def add_user():
@@ -69,24 +74,21 @@
         # First entry.
         data = {"user1": new_user_data, "metadata": {"uid_count": 1}}
 
     # Save database-
     _save_user_database(data)
 
 
-def remove_user():
+def remove_user(removeid):
     """ Remove a user from the database. """
 
     # Does the user database exist?
     database_exists = os.path.isfile(cite_tracker.USER_DATABASE)
     assert database_exists, "No user database yet!"
 
-    # Who to remove
-    removeid = int(input("Enter user to remove (integer ID of user): "))
-
     # Load the user database.
     data = _load_user_database()
 
     # Remove user
     if f"user{removeid}" in data.keys():
         print(f"Removing user{removeid}...")
 
@@ -96,15 +98,15 @@
             os.remove(user_database)
             print(f"Deleted {user_database}")
 
         # Remove from users list.
         del data[f"user{removeid}"]
     else:
         print(
-            f"No user{removeid} in database, try 'myads --list_users' to see current users"
+            f"No user {removeid} in database, try 'myads user list' to see current users"
         )
 
     # Save database-
     _save_user_database(data)
 
 
 def set_ads_token(ads_token):
```

### Comparing `myads-1.0.1/src/myads/query.py` & `myads-1.0.2/src/myads/query.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.1/src/myads.egg-info/PKG-INFO` & `myads-1.0.2/src/myads.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: myads
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple ADS API query package and citation tracker
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
-Keywords: nasa-ads,citations,astronomy,ads,python
+Project-URL: homepage, https://github.com/stuartmcalpine/myADS
+Project-URL: repository, https://github.com/stuartmcalpine/myADS
+Keywords: nasa-ads,citations,astronomy,ads,python,arxiv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/myads.svg)](https://badge.fury.io/py/myads)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/myads?logo=python)
 
 # myADS
 
 `myADS` is a simple package to keep track of citations to your (and other
 authors) papers.
 
-It both reports your current papers citation metrics, and
-checks for any new cites to your papers since the last time of checking.
+It both reports the authors current paper citation metrics, and checks for any
+new cites to the authors papers since the last time of checking.
 
 Once installed you can always run `myads --help` to see a list of available
 commands.
 
 ## Installation
 
 The easiest method is to install directly from
@@ -39,63 +41,61 @@
 * Clone the repository using ``git clone
   https://github.com/stuartmcalpine/myADS.git``
 * Navigate to the ``myADS`` folder
 * Install using `pip install .`
 
 ## Getting set up
 
-``myADS`` can keep track of the citations for multiple users. Two steps before
-you get started:
+``myADS`` can keep track of the citations for multiple authors. Two steps
+before you get started:
 
-* Add your users to the database
+* Add your authors you want to track to the database
 * Add your ADS API token to the database
 
-### Adding a user to the database
+### Adding a author to the database
 
-Once `myADS` is installed you can add users to the tracking database using:
+Once `myADS` is installed you can add the authors you wish to track using:
 
 ```bash
-myads --add_user
+myads author add
 ```
 
 You will be prompted to enter a first and last name, and an optional ORCID
-(however it is recommended you add this for each user when possible).
+(however it is recommended you add this for each author when possible).
 
-### Removing a user from the database
+### Removing a author from the database
 
-You can remove users from the tracking database using:
+You can remove authors from the tracking database using:
 
 ```bash
-myads --remove_user
+myads author remove <author id>
 ```
 
-where you will be prompted to enter the users unique tracking ID.
-
-You can get a list of tracking IDs by typing:
+You can get a list of author IDs by typing:
 
 ```bash
-myads --list_users
+myads author list
 ```
 
 ### Adding your ADS API token
 
 You must add your [ADS API token](https://ui.adsabs.harvard.edu/help/api/) so
 the package can query on your behalf. 
 
 To add it run:
 
 ```bash
---set_ads_token <YOUR-API-TOKEN-HERE>
+myads token add <YOUR-API-TOKEN-HERE>
 ```
 
 ## Usage
 
 ### Citation reporter
 
-If you run `myads --report` you will get a report of all your registered users
+If you run `myads report` you will get a report of all your tracked authors
 current citations, e.g.,
 
 ```bash
 Reporting cites for Stuart McAlpine...
 +----------------------------------------------------+--------------+---------------+---------------------+
 | Title                                              | Citations    | Publication   | Bibcode             |
 |                                                    | (per year)   | Date          |                     |
@@ -104,16 +104,16 @@
 | significant amount of black hole growth yet do     |              |               |                     |
 | increase the rate of luminous AGN                  |              |               |                     |
 +----------------------------------------------------+--------------+---------------+---------------------+
 ```
 
 ### Citation tracker
 
-If you run `myads --check` it will tell you any papers that have cited your
-users papers since the last call. 
+If you run `myads check` it will tell you any papers that have cited your
+tracked authors papers since the last call. 
 
 The first time you run this it will create a local database of your citations.
 From then on it will update the local database with your new cites and report
 the changes, e.g.,
 
 ```bash
  1 new cite(s) for Galaxy mergers in EAGLE do not induce a significant amount of black hole growth yet do increase the rate of luminous AGN
```

