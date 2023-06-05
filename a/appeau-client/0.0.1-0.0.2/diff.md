# Comparing `tmp/appeau_client-0.0.1.tar.gz` & `tmp/appeau_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeau_client-0.0.1.tar", last modified: Fri Jun  2 15:15:11 2023, max compression
+gzip compressed data, was "appeau_client-0.0.2.tar", last modified: Mon Jun  5 13:13:04 2023, max compression
```

## Comparing `appeau_client-0.0.1.tar` & `appeau_client-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:15:11.323871 appeau_client-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-02 15:15:11.323871 appeau_client-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-02 15:14:56.000000 appeau_client-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:15:11.323871 appeau_client-0.0.1/appeau_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-02 15:15:11.000000 appeau_client-0.0.1/appeau_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-02 15:15:11.000000 appeau_client-0.0.1/appeau_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:15:11.000000 appeau_client-0.0.1/appeau_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 15:15:11.000000 appeau_client-0.0.1/appeau_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 15:15:11.000000 appeau_client-0.0.1/appeau_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:15:11.323871 appeau_client-0.0.1/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_calculdirect_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_date_calcul_parcelleId_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_donnees_meteomulti_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcelles_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcelles_id_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcelles_id_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcelles_id_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcelles_parcelleIddonnees_meteo_dateDebut_dateFin_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcelles_parcelleIdresultat_dateDebut_dateFin_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcelles_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcellesattente_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcellesdetails_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcellesdetails_listParcellesId_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/api_parcellesmulti_listParcellesIdresultat_dateDebut_dateFin_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 15:14:56.000000 appeau_client-0.0.1/sample/login_check_post.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:15:11.327871 appeau_client-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-02 15:14:56.000000 appeau_client-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:13:04.335482 appeau_client-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:13:04.335482 appeau_client-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 13:12:54.000000 appeau_client-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:13:04.335482 appeau_client-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-05 13:12:54.000000 appeau_client-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:13:04.335482 appeau_client-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:13:04.335482 appeau_client-0.0.2/src/appeau_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:13:04.000000 appeau_client-0.0.2/src/appeau_client.egg-info/top_level.txt
```

### Comparing `appeau_client-0.0.1/PKG-INFO` & `appeau_client-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appeau_client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A client for http://appeau.api.vignevin-epicure.com API
 Author: Guilhem Heinrich
 Author-email: guilhem.heinrich@id2l.fr
 License: Apache 2.0
```

### Comparing `appeau_client-0.0.1/README.md` & `appeau_client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.1/appeau_client.egg-info/PKG-INFO` & `appeau_client-0.0.2/src/appeau_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appeau-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A client for http://appeau.api.vignevin-epicure.com API
 Author: Guilhem Heinrich
 Author-email: guilhem.heinrich@id2l.fr
 License: Apache 2.0
```

### Comparing `appeau_client-0.0.1/setup.py` & `appeau_client-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Voir https://blog.engineering.publicissapient.fr/2020/06/04/packaging-python-setup-py-et-setuptools/
 setup(name="appeau_client",
-version="0.0.1",
+version="0.0.2",
 description="A client for http://appeau.api.vignevin-epicure.com API",
 author="Guilhem Heinrich",
 author_email="guilhem.heinrich@id2l.fr",
-packages=["sample"],
+# packages=["src"],
+package_dir={'':'src'},
+packages=find_packages('src'),
 install_requires=["requests"],
+# format=["tar.gz", "zip"],
 # extras_require={
 # "dev": ["requests-mock"],
 # },
+# options={"sdist": {
+#     "formats": ['zip', 'tar.gz']
+# }},
 license="Apache 2.0",
 long_description=long_description)
```

