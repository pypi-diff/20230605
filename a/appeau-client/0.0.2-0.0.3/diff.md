# Comparing `tmp/appeau_client-0.0.2.tar.gz` & `tmp/appeau_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeau_client-0.0.2.tar", last modified: Mon Jun  5 13:13:04 2023, max compression
+gzip compressed data, was "appeau_client-0.0.3.tar", last modified: Mon Jun  5 13:31:29 2023, max compression
```

## Comparing `appeau_client-0.0.2.tar` & `appeau_client-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:13:04.335482 appeau_client-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:13:04.335482 appeau_client-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 13:12:54.000000 appeau_client-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:13:04.335482 appeau_client-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-05 13:12:54.000000 appeau_client-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:13:04.335482 appeau_client-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:13:04.335482 appeau_client-0.0.2/src/appeau_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:31:29.254434 appeau_client-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:31:29.254434 appeau_client-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 13:31:19.000000 appeau_client-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:31:29.254434 appeau_client-0.0.3/appeau_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_calculdirect_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_date_calcul_parcelleId_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_donnees_meteomulti_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcelles_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcelles_id_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcelles_id_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcelles_id_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcelles_parcelleIddonnees_meteo_dateDebut_dateFin_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcelles_parcelleIdresultat_dateDebut_dateFin_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcelles_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcellesattente_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcellesdetails_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcellesdetails_listParcellesId_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/api_parcellesmulti_listParcellesIdresultat_dateDebut_dateFin_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-05 13:31:19.000000 appeau_client-0.0.3/appeau_client/login_check_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:31:29.254434 appeau_client-0.0.3/appeau_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:31:29.000000 appeau_client-0.0.3/appeau_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-05 13:31:29.000000 appeau_client-0.0.3/appeau_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:31:29.000000 appeau_client-0.0.3/appeau_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 13:31:29.000000 appeau_client-0.0.3/appeau_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 13:31:29.000000 appeau_client-0.0.3/appeau_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:31:29.254434 appeau_client-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-05 13:31:19.000000 appeau_client-0.0.3/setup.py
```

### Comparing `appeau_client-0.0.2/PKG-INFO` & `appeau_client-0.0.3/appeau_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: appeau_client
-Version: 0.0.2
+Name: appeau-client
+Version: 0.0.3
 Summary: A client for http://appeau.api.vignevin-epicure.com API
 Author: Guilhem Heinrich
 Author-email: guilhem.heinrich@id2l.fr
 License: Apache 2.0
```

### Comparing `appeau_client-0.0.2/README.md` & `appeau_client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.2/setup.py` & `appeau_client-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Voir https://blog.engineering.publicissapient.fr/2020/06/04/packaging-python-setup-py-et-setuptools/
 setup(name="appeau_client",
-version="0.0.2",
+version="0.0.3",
 description="A client for http://appeau.api.vignevin-epicure.com API",
 author="Guilhem Heinrich",
 author_email="guilhem.heinrich@id2l.fr",
-# packages=["src"],
-package_dir={'':'src'},
-packages=find_packages('src'),
+packages=["appeau_client"],
+# package_dir={'':'src'},
+# packages=find_packages('src'),
 install_requires=["requests"],
 # format=["tar.gz", "zip"],
 # extras_require={
 # "dev": ["requests-mock"],
 # },
 # options={"sdist": {
 #     "formats": ['zip', 'tar.gz']
```

### Comparing `appeau_client-0.0.2/src/appeau_client.egg-info/PKG-INFO` & `appeau_client-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: appeau-client
-Version: 0.0.2
+Name: appeau_client
+Version: 0.0.3
 Summary: A client for http://appeau.api.vignevin-epicure.com API
 Author: Guilhem Heinrich
 Author-email: guilhem.heinrich@id2l.fr
 License: Apache 2.0
```

