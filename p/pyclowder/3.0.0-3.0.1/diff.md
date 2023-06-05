# Comparing `tmp/pyclowder-3.0.0.tar.gz` & `tmp/pyclowder-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyclowder-3.0.0.tar", last modified: Thu Apr  6 18:05:10 2023, max compression
+gzip compressed data, was "dist/pyclowder-3.0.1.tar", last modified: Mon Jun  5 21:00:01 2023, max compression
```

## Comparing `pyclowder-3.0.0.tar` & `pyclowder-3.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:10.000000 pyclowder-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-06 18:05:00.000000 pyclowder-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-06 18:05:00.000000 pyclowder-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-06 18:05:10.000000 pyclowder-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-06 18:05:00.000000 pyclowder-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-06 18:05:00.000000 pyclowder-3.0.0/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/api/v1/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/api/v1/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/api/v2/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/api/v2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    48150 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/geostreams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-04-06 18:05:00.000000 pyclowder-3.0.0/pyclowder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 18:05:10.000000 pyclowder-3.0.0/pyclowder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 18:05:10.000000 pyclowder-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-06 18:05:00.000000 pyclowder-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-05 20:59:53.000000 pyclowder-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 20:59:53.000000 pyclowder-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-05 21:00:01.000000 pyclowder-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-06-05 20:59:53.000000 pyclowder-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-05 20:59:53.000000 pyclowder-3.0.1/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v1/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v1/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v2/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48150 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/geostreams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:00:01.000000 pyclowder-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-05 20:59:53.000000 pyclowder-3.0.1/setup.py
```

### Comparing `pyclowder-3.0.0/LICENSE` & `pyclowder-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/PKG-INFO` & `pyclowder-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclowder
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python SDK for the Clowder Data Management System
 Home-page: https://clowderframework.org
 Author: Rob Kooper
 Author-email: kooper@illinois.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/clowder-framework/pyclowder/issues
 Project-URL: Source, https://github.com/clowder-framework/pyclowder
```

### Comparing `pyclowder-3.0.0/README.md` & `pyclowder-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/description.rst` & `pyclowder-3.0.1/description.rst`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/api/v1/datasets.py` & `pyclowder-3.0.1/pyclowder/api/v1/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json
 import logging
 import os
 import tempfile
 
 import requests
-import pyclowder.api.v2.datasets as v2datasets
-import pyclowder.api.v1.datasets as v1datasets
 from pyclowder.client import ClowderClient
 from pyclowder.collections import get_datasets, get_child_collections, delete as delete_collection
 from pyclowder.utils import StatusMessage
 
 
 def create_empty(connector, client, datasetname, description, parentid=None, spaceid=None):
     """Create a new dataset in Clowder.
@@ -59,17 +57,15 @@
     """Delete dataset from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to delete
     """
-    headers = {"Authorization": "Bearer " + client.key}
-
-    url = "%s/api/v2/datasets/%s" % (client.host, datasetid)
+    url = "%s/api/datasets/%s?key=%s" % (client.host, datasetid, client.key)
 
     result = requests.delete(url, verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
     return json.loads(result.text)
 
 # TODO collection not implemented yet in v2
@@ -123,94 +119,84 @@
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to fetch metadata of
     extractor -- extractor name to filter results (if only one extractor's metadata is desired)
     """
-    headers = {"Authorization": "Bearer " + client.key}
-
     filterstring = "" if extractor is None else "&extractor=%s" % extractor
-    url = '%s/api/v2/datasets/%s/metadata' % (client.host, datasetid)
+    url = '%s/api/datasets/%s/metadata?key=%s' % (client.host, datasetid, client.key + filterstring)
 
     # fetch data
-    result = requests.get(url, stream=True, headers=headers,
+    result = requests.get(url, stream=True,
                           verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
     return result.json()
 
 def get_info(connector, client, datasetid):
     """Get basic dataset information from UUID.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to get info of
     """
-    headers = {"Authorization": "Bearer " + client.key}
 
-    url = "%s/api/v2/datasets/%s" % (client.host, datasetid)
+    url = "%s/api/datasets/%s?key=%s" % (client.host, datasetid, client.key)
 
-    result = requests.get(url, headers=headers,
-                          verify=connector.ssl_verify if connector else True)
+    result = requests.get(url, verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
     return json.loads(result.text)
 
 def get_file_list(connector, client, datasetid):
     """Get list of files in a dataset as JSON object.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to get filelist of
     """
-    headers = {"Authorization": "Bearer " + client.key}
+    url = "%s/api/datasets/%s/files?key=%s" % (client.host, datasetid, client.key)
 
-    url = "%s/api/v2/datasets/%s/files" % (client.host, datasetid)
-
-    result = requests.get(url, headers=headers, verify=connector.ssl_verify if connector else True)
+    result = requests.get(url, verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
     return json.loads(result.text)
 
 def remove_metadata(connector, client, datasetid, extractor=None):
     """Delete dataset JSON-LD metadata from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to fetch metadata of
     extractor -- extractor name to filter deletion
                     !!! ALL JSON-LD METADATA WILL BE REMOVED IF NO extractor PROVIDED !!!
     """
-    headers = {"Authorization": "Bearer " + client.key}
-
     filterstring = "" if extractor is None else "&extractor=%s" % extractor
-    url = '%s/api/v2/datasets/%s/metadata' % (client.host, datasetid)
+    url = '%s/api/datasets/%s/metadata?key=%s' % (client.host, datasetid, client.key)
 
     # fetch data
-    result = requests.delete(url, stream=True, headers=headers,
-                             verify=connector.ssl_verify if connector else True)
+    result = requests.delete(url, stream=True, verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
 def submit_extraction(connector, client, datasetid, extractorname):
     """Submit dataset for extraction by given extractor.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset UUID to submit
     extractorname -- registered name of extractor to trigger
     """
-    headers = {'Content-Type': 'application/json',
-               "Authorization": "Bearer " + client.key}
+    headers = {'Content-Type': 'application/json'}
 
-    url = "%s/api/v2/datasets/%s/extractions?key=%s" % (client.host, datasetid)
+    url = "%s/api/datasets/%s/extractions?key=%s" % (client.host, datasetid, client.key)
 
     result = requests.post(url,
                            headers=headers,
                            data=json.dumps({"extractor": extractorname}),
                            verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
@@ -262,19 +248,18 @@
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset that is currently being processed
     metadata -- the metadata to be uploaded
     """
-    headers = {'Content-Type': 'application/json',
-               "Authorization": "Bearer " + client.key}
+    headers = {'Content-Type': 'application/json'}
     connector.message_process({"type": "dataset", "id": datasetid}, "Uploading dataset metadata.")
 
-    url = '%s/api/v2/datasets/%s/metadata' % (client.host, datasetid)
+    url = '%s/api/datasets/%s/metadata?key=%s' % (client.host, datasetid, client.key)
     result = requests.post(url, headers=headers, data=json.dumps(metadata),
                            verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
 
 # TODO not done yet, need more testing
 class DatasetsApi(object):
```

### Comparing `pyclowder-3.0.0/pyclowder/api/v1/files.py` & `pyclowder-3.0.1/pyclowder/api/v1/files.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/api/v2/datasets.py` & `pyclowder-3.0.1/pyclowder/api/v2/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     spaceid -- id of the space to add dataset to
     """
 
     logger = logging.getLogger(__name__)
 
     url = '%s/api/v2/datasets' % client.host
     headers = {"Content-Type": "application/json",
-               "Authorization": "Bearer " + client.key}
+               "X-API-KEY": client.key}
     result = requests.post(url, headers=headers,
                            data=json.dumps({"name": datasetname, "description": description}),
                            verify=connector.ssl_verify if connector else True)
 
     result.raise_for_status()
 
     datasetid = result.json()['id']
@@ -48,16 +48,15 @@
     """Delete dataset from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to delete
     """
-    headers = {"Authorization": "Bearer " + client.key}
-
+    headers = {"X-API-KEY": client.key}
     url = "%s/api/v2/datasets/%s" % (client.host, datasetid)
 
     result = requests.delete(url, headers=headers, verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
     return json.loads(result.text)
 
@@ -93,15 +92,15 @@
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the file that is currently being processed
     """
 
     connector.message_process({"type": "dataset", "id": datasetid}, "Downloading dataset.")
 
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
     # fetch dataset zipfile
     url = '%s/api/v2/datasets/%s/download' % (client.host, datasetid)
     result = requests.get(url, stream=True, headers=headers,
                           verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
     (filedescriptor, zipfile) = tempfile.mkstemp(suffix=".zip")
@@ -117,15 +116,15 @@
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to fetch metadata of
     extractor -- extractor name to filter results (if only one extractor's metadata is desired)
     """
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
 
     filterstring = "" if extractor is None else "&extractor=%s" % extractor
     url = '%s/api/v2/datasets/%s/metadata' % (client.host, datasetid)
 
     # fetch data
     result = requests.get(url, stream=True, headers=headers,
                           verify=connector.ssl_verify if connector else True)
@@ -138,15 +137,15 @@
     """Get basic dataset information from UUID.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to get info of
     """
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
 
     url = "%s/api/v2/datasets/%s" % (client.host, datasetid)
 
     result = requests.get(url, headers=headers,
                           verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
@@ -157,15 +156,15 @@
     """Get list of files in a dataset as JSON object.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to get filelist of
     """
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
 
     url = "%s/api/v2/datasets/%s/files" % (client.host, datasetid)
 
     result = requests.get(url, headers=headers, verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
 
     return json.loads(result.text)
@@ -177,15 +176,15 @@
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset to fetch metadata of
     extractor -- extractor name to filter deletion
                     !!! ALL JSON-LD METADATA WILL BE REMOVED IF NO extractor PROVIDED !!!
     """
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
 
     filterstring = "" if extractor is None else "&extractor=%s" % extractor
     url = '%s/api/v2/datasets/%s/metadata' % (client.host, datasetid)
 
     # fetch data
     result = requests.delete(url, stream=True, headers=headers,
                              verify=connector.ssl_verify if connector else True)
@@ -198,15 +197,15 @@
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset UUID to submit
     extractorname -- registered name of extractor to trigger
     """
     headers = {'Content-Type': 'application/json',
-                "Authorization": "Bearer " + client.key}
+                "X-API-KEY": client.key}
 
     url = "%s/api/v2/datasets/%s/extractions?key=%s" % (client.host, datasetid)
 
     result = requests.post(url,
                            headers=headers,
                            data=json.dumps({"extractor": extractorname}),
                            verify=connector.ssl_verify if connector else True)
@@ -221,15 +220,15 @@
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     datasetid -- the dataset that is currently being processed
     metadata -- the metadata to be uploaded
     """
     headers = {'Content-Type': 'application/json',
-               "Authorization": "Bearer " + client.key}
+               "X-API-KEY": client.key}
     connector.message_process({"type": "dataset", "id": datasetid}, "Uploading dataset metadata.")
 
 
     url = '%s/api/v2/datasets/%s/metadata' % (client.host, datasetid)
     result = requests.post(url, headers=headers, data=json.dumps(metadata),
                            verify=connector.ssl_verify if connector else True)
     result.raise_for_status()
```

### Comparing `pyclowder-3.0.0/pyclowder/api/v2/files.py` & `pyclowder-3.0.1/pyclowder/api/v2/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 
     # TODO: intermediateid doesn't really seem to be used here, can we remove entirely?
     if not intermediatefileid:
         intermediatefileid = fileid
 
     url = '%s/api/v2/files/%s' % (client.host, intermediatefileid)
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
     result = connector.get(url, stream=True, verify=connector.ssl_verify if connector else True, headers=headers)
 
     (inputfile, inputfilename) = tempfile.mkstemp(suffix=ext)
 
     try:
         with os.fdopen(inputfile, "wb") as outputfile:
             for chunk in result.iter_content(chunk_size=10 * 1024):
@@ -86,15 +86,15 @@
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     fileid -- the file to fetch metadata of
     """
 
     url = '%s/api/v2/files/%s/metadata' % (client.host, fileid)
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
     # fetch data
     result = connector.get(url, stream=True, verify=connector.ssl_verify if connector else True, headers=headers)
 
     return result
 
 
 def download_metadata(connector,client, fileid, extractor=None):
@@ -105,15 +105,15 @@
     client -- ClowderClient containing authentication credentials
     fileid -- the file to fetch metadata of
     extractor -- extractor name to filter results (if only one extractor's metadata is desired)
     """
 
     filterstring = "" if extractor is None else "?extractor=%s" % extractor
     url = '%s/api/v2/files/%s/metadata?%s' % (client.host, fileid, filterstring)
-    headers = {"Authorization": "Bearer " + client.key}
+    headers = {"X-API-KEY": client.key}
 
     # fetch data
     result = connector.get(url, stream=True, verify=connector.ssl_verify if connector else True, headers=headers)
 
     return result
 
 
@@ -126,15 +126,15 @@
     fileid -- the file UUID to submit
     extractorname -- registered name of extractor to trigger
     """
 
     url = "%s/api/v2/files/%s/extractions?key=%s" % (client.host, fileid, client.key)
     result = connector.post(url,
                             headers={'Content-Type': 'application/json',
-                                     "Authorization": "Bearer " + client.key},
+                                     "X-API-KEY": client.key},
                             data=json.dumps({"extractor": extractorname}),
                             verify=connector.ssl_verify if connector else True)
 
     return result
 
 
 def upload_metadata(connector, client, fileid, metadata):
@@ -145,17 +145,15 @@
     client -- ClowderClient containing authentication credentials
     fileid -- the file that is currently being processed
     metadata -- the metadata to be uploaded
     """
 
     connector.message_process({"type": "file", "id": fileid}, "Uploading file metadata.")
     headers = {'Content-Type': 'application/json',
-               'Authorization':'Bearer ' + client.key}
-    print(metadata)
-    as_json = json.dumps(metadata)
+               'X-API-KEY': client.key}
     url = '%s/api/v2/files/%s/metadata' % (client.host, fileid)
     result = connector.post(url, headers=headers, data=json.dumps(metadata),
                             verify=connector.ssl_verify if connector else True)
 
 
 
 # TODO not implemented in v2
@@ -281,15 +279,15 @@
     url = '%s/api/v2/datasets/%s/files' % (client.host, datasetid)
 
     if os.path.exists(filepath):
         filename = os.path.basename(filepath)
         m = MultipartEncoder(
             fields={'file': (filename, open(filepath, 'rb'))}
         )
-        headers = {"Authorization": "Bearer " + client.key,
+        headers = {"X-API-KEY": client.key,
                     'Content-Type': m.content_type}
         result = connector.post(url, data=m, headers=headers,
                                 verify=connector.ssl_verify if connector else True)
 
         uploadedfileid = result.json()['id']
         logger.debug("uploaded file id = [%s]", uploadedfileid)
 
@@ -318,15 +316,15 @@
                                             source_path)
                 break
 
         filename = os.path.basename(filepath)
         m = MultipartEncoder(
             fields={'file': (filename, open(filepath, 'rb'))}
         )
-        headers = {"Authorization": "Bearer " + client.key,
+        headers = {"X-API-KEY": client.key,
                     'Content-Type': m.content_type}
         result = connector.post(url, data=m, headers=headers,
                                 verify=connector.ssl_verify if connector else True)
 
         uploadedfileid = result.json()['id']
         logger.debug("uploaded file id = [%s]", uploadedfileid)
```

### Comparing `pyclowder-3.0.0/pyclowder/client.py` & `pyclowder-3.0.1/pyclowder/client.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/collections.py` & `pyclowder-3.0.1/pyclowder/collections.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/connectors.py` & `pyclowder-3.0.1/pyclowder/connectors.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/datasets.py` & `pyclowder-3.0.1/pyclowder/datasets.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/extractors.py` & `pyclowder-3.0.1/pyclowder/extractors.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/files.py` & `pyclowder-3.0.1/pyclowder/files.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/geostreams.py` & `pyclowder-3.0.1/pyclowder/geostreams.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/sections.py` & `pyclowder-3.0.1/pyclowder/sections.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder/utils.py` & `pyclowder-3.0.1/pyclowder/utils.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/pyclowder.egg-info/PKG-INFO` & `pyclowder-3.0.1/pyclowder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclowder
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python SDK for the Clowder Data Management System
 Home-page: https://clowderframework.org
 Author: Rob Kooper
 Author-email: kooper@illinois.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/clowder-framework/pyclowder/issues
 Project-URL: Source, https://github.com/clowder-framework/pyclowder
```

### Comparing `pyclowder-3.0.0/pyclowder.egg-info/SOURCES.txt` & `pyclowder-3.0.1/pyclowder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.0/setup.py` & `pyclowder-3.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'description.rst').read_text(encoding='utf-8')
 
 setup(
     name='pyclowder',
-    version='3.0.0',
+    version='3.0.1',
     description='Python SDK for the Clowder Data Management System',
     long_description=long_description,
 
     author='Rob Kooper',
     author_email='kooper@illinois.edu',
 
     url='https://clowderframework.org',
```

