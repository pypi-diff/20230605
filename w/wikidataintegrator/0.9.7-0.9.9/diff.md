# Comparing `tmp/wikidataintegrator-0.9.7.tar.gz` & `tmp/wikidataintegrator-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/WikidataIntegrator/WikidataIntegrator/dist/tmpubun_d7t/wikidataintegrator-0.9.7.tar", last modified: Wed Aug 25 22:26:28 2021, max compression
+gzip compressed data, was "/home/runner/work/WikidataIntegrator/WikidataIntegrator/dist/tmp_mgqaoih/wikidataintegrator-0.9.9.tar", last modified: Thu Aug 26 17:52:23 2021, max compression
```

## Comparing `wikidataintegrator-0.9.7.tar` & `wikidataintegrator-0.9.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (116)     1099 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)    19357 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    18272 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      402 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1582 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator/
--rw-r--r--   0 runner    (1001) docker     (116)      297 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/
--rw-r--r--   0 runner    (1001) docker     (116)      239 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      245 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/strict_overwrite.py
--rw-r--r--   0 runner    (1001) docker     (116)    10220 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/test_update_retrieved_if_new.py
--rw-r--r--   0 runner    (1001) docker     (116)     3749 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/update_release.py
--rw-r--r--   0 runner    (1001) docker     (116)     2352 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/update_retrieved_if_new.py
--rw-r--r--   0 runner    (1001) docker     (116)     3269 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/update_retrieved_if_new_multiple_refs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1563 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (116)     9359 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_fastrun.py
--rw-r--r--   0 runner    (1001) docker     (116)    13166 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_handle_refs.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_item_creation.py
--rw-r--r--   0 runner    (1001) docker     (116)      549 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_item_generator.py
--rw-r--r--   0 runner    (1001) docker     (116)      371 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_wd_search.py
--rw-r--r--   0 runner    (1001) docker     (116)     2598 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_wdi_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)      416 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/test_wdi_login.py
--rw-r--r--   0 runner    (1001) docker     (116)     8027 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (116)     1315 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_backoff.py
--rw-r--r--   0 runner    (1001) docker     (116)   260018 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_config.py
--rwxr-xr-x   0 runner    (1001) docker     (116)   158499 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_core.py
--rw-r--r--   0 runner    (1001) docker     (116)    25659 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_fastrun.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/
--rw-r--r--   0 runner    (1001) docker     (116)    11715 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/mapping_relation_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)    25939 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/publication.py
--rw-r--r--   0 runner    (1001) docker     (116)     5484 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/release.py
--rw-r--r--   0 runner    (1001) docker     (116)     6569 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/wikibase_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     9937 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_login.py
--rw-r--r--   0 runner    (1001) docker     (116)    25567 2021-08-25 22:26:20.000000 wikidataintegrator-0.9.7/wikidataintegrator/wdi_rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    19357 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1524 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      100 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       97 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2021-08-25 22:26:28.000000 wikidataintegrator-0.9.7/wikidataintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1099 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    19357 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    18272 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      402 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1582 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator/
+-rw-r--r--   0 runner    (1001) docker     (116)      297 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/
+-rw-r--r--   0 runner    (1001) docker     (116)      239 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      245 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/strict_overwrite.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10220 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/test_update_retrieved_if_new.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3749 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/update_release.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2352 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/update_retrieved_if_new.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3269 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/update_retrieved_if_new_multiple_refs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1563 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9359 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_fastrun.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13166 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_handle_refs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_item_creation.py
+-rw-r--r--   0 runner    (1001) docker     (116)      549 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_item_generator.py
+-rw-r--r--   0 runner    (1001) docker     (116)      371 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_wd_search.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2598 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_wdi_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      416 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/test_wdi_login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8027 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1315 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (116)   260018 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)   158498 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_core.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25659 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_fastrun.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/
+-rw-r--r--   0 runner    (1001) docker     (116)    11715 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2171 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/mapping_relation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25939 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/publication.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5484 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/release.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6569 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/wikibase_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9937 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_login.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25959 2021-08-26 17:52:15.000000 wikidataintegrator-0.9.9/wikidataintegrator/wdi_rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    19357 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1524 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      100 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       97 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2021-08-26 17:52:23.000000 wikidataintegrator-0.9.9/wikidataintegrator.egg-info/top_level.txt
```

### Comparing `wikidataintegrator-0.9.7/LICENSE.txt` & `wikidataintegrator-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/PKG-INFO` & `wikidataintegrator-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidataintegrator
-Version: 0.9.7
+Version: 0.9.9
 Summary: Python package for reading and writing to/from Wikidata
 Home-page: https://github.com/sulab/WikidataIntegrator
 Author: Andra Waagmeester, Greg Stupp, Sebastian Burgstaller-Muehlbacher 
 Author-email: andra@micel.io
 License: MIT
 Keywords: Wikidata genewiki biology chemistry medicine ShEx citations
 Platform: UNKNOWN
```

### Comparing `wikidataintegrator-0.9.7/README.md` & `wikidataintegrator-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/setup.py` & `wikidataintegrator-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.9.7"
+VERSION = "0.9.9"
 
 setup(
     name='wikidataintegrator',
     version=VERSION,
     author='Andra Waagmeester, Greg Stupp, Sebastian Burgstaller-Muehlbacher ',
     author_email='andra@micel.io',
     description='Python package for reading and writing to/from Wikidata',
```

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/test_update_retrieved_if_new.py` & `wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/test_update_retrieved_if_new.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/update_release.py` & `wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/update_release.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/update_retrieved_if_new.py` & `wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/update_retrieved_if_new.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/ref_handlers/update_retrieved_if_new_multiple_refs.py` & `wikidataintegrator-0.9.9/wikidataintegrator/ref_handlers/update_retrieved_if_new_multiple_refs.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/tests/test_backoff.py` & `wikidataintegrator-0.9.9/wikidataintegrator/tests/test_backoff.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/tests/test_fastrun.py` & `wikidataintegrator-0.9.9/wikidataintegrator/tests/test_fastrun.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/tests/test_handle_refs.py` & `wikidataintegrator-0.9.9/wikidataintegrator/tests/test_handle_refs.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/tests/test_item_creation.py` & `wikidataintegrator-0.9.9/wikidataintegrator/tests/test_item_creation.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/tests/test_item_generator.py` & `wikidataintegrator-0.9.9/wikidataintegrator/tests/test_item_generator.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/tests/test_wdi_helpers.py` & `wikidataintegrator-0.9.9/wikidataintegrator/tests/test_wdi_helpers.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/tests/tests.py` & `wikidataintegrator-0.9.9/wikidataintegrator/tests/tests.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_backoff.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_backoff.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_config.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_config.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_core.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1215,15 +1215,14 @@
         :return: The interwiki/sitelink string for the specified Wikipedia will be returned.
         """
         if site in self.sitelinks:
             return self.sitelinks[site]
         else:
             return None
 
-
     def write(self, login, bot_account=True, edit_summary='', entity_type='item', property_datatype='string',
               max_retries=1000, retry_after=60):
         """
         Writes the WD item Json to WD and after successful write, updates the object with new ids and hashes generated
         by WD. For new items, also returns the new QIDs.
         :param login: a instance of the class PBB_login which provides edit-cookies and edit-tokens
         :param bot_account: Tell the Wikidata API whether the script should be run as part of a bot account or not.
```

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_fastrun.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_fastrun.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/__init__.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/mapping_relation_helper.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/mapping_relation_helper.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/publication.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/publication.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/release.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/release.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_helpers/wikibase_helper.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_helpers/wikibase_helper.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_login.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_login.py`

 * *Files identical despite different names*

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator/wdi_rdf.py` & `wikidataintegrator-0.9.9/wikidataintegrator/wdi_rdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,24 @@
 """
 
 __author__ = 'Andra Waagmeester'
 __license__ = 'MIT'
 
 
 class WDqidRDFEngine(object):
-    def __init__(self, qid, fetch_provenance_rdf=True, fetch_metadata_rdf=True, fetch_truthy_rdf=False,
+    def __init__(self, qid=None, json_data=None, fetch_provenance_rdf=True, fetch_metadata_rdf=True, fetch_truthy_rdf=False,
                  fetch_normalized_rdf=False, fetch_sitelinks_rdf=False,
                  fetch_merged_items_rdf=False, fetch_property_descriptions_rdf=False, fetch_labels_rdf=True,
                  fetch_linked_items_rdf=False, fetch_all=False):
+        if not bool(qid) and not bool(json_data):
+            raise ValueError('Please provide either a QID or a json object of a Wikidata item')
+
+        if bool(qid) and bool(data):
+            raise ValueError('Please provide only a QID or a JSON object of a Wikidata item, not both')
+
         self.qid = qid
         if fetch_all:
             self.fetch_provenance_rdf = True
             self.fetch_labels_rdf = True
             self.fetch_metadata_rdf = True
             self.fetch_merged_items_rdf = True
             self.fetch_normalized_rdf = True
@@ -38,17 +44,19 @@
             self.fetch_metadata_rdf = fetch_metadata_rdf
             self.fetch_merged_items_rdf = fetch_merged_items_rdf
             self.fetch_normalized_rdf = fetch_normalized_rdf
             self.fetch_property_descriptions_rdf = fetch_property_descriptions_rdf
             self.fetch_sitelinks_rdf = fetch_sitelinks_rdf
             self.fetch_truthy_rdf = fetch_truthy_rdf
             self.fetch_linked_items_rdf = fetch_linked_items_rdf
-
-        self.json_item = json.loads(requests.get("http://www.wikidata.org/entity/" + qid + ".json").text)["entities"][
-            qid]
+        if bool(qid):
+            self.json_item = json.loads(requests.get("http://www.wikidata.org/entity/" + qid + ".json").text)["entities"][
+                qid]
+        else:
+            self.json_item = json_data
         self.rdf_item = Graph()
         self.ns = dict()
         self.linked_items = []
         self.metadata = {"identifiers": 0, "sitelinks": 0, "statements": 0}
         self.ns = dict()
         for prefix in wdi_config.prefix.keys():
             self.ns[prefix] = Namespace(wdi_config.prefix[prefix])
```

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator.egg-info/PKG-INFO` & `wikidataintegrator-0.9.9/wikidataintegrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidataintegrator
-Version: 0.9.7
+Version: 0.9.9
 Summary: Python package for reading and writing to/from Wikidata
 Home-page: https://github.com/sulab/WikidataIntegrator
 Author: Andra Waagmeester, Greg Stupp, Sebastian Burgstaller-Muehlbacher 
 Author-email: andra@micel.io
 License: MIT
 Keywords: Wikidata genewiki biology chemistry medicine ShEx citations
 Platform: UNKNOWN
```

### Comparing `wikidataintegrator-0.9.7/wikidataintegrator.egg-info/SOURCES.txt` & `wikidataintegrator-0.9.9/wikidataintegrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

