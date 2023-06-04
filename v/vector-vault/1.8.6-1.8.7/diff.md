# Comparing `tmp/vector_vault-1.8.6.tar.gz` & `tmp/vector_vault-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.8.6.tar", last modified: Sun Jun  4 23:14:15 2023, max compression
+gzip compressed data, was "vector_vault-1.8.7.tar", last modified: Sun Jun  4 23:35:41 2023, max compression
```

## Comparing `vector_vault-1.8.6.tar` & `vector_vault-1.8.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:14:15.409090 vector_vault-1.8.6/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.6/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 23:14:15.408923 vector_vault-1.8.6/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.6/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 23:14:15.409134 vector_vault-1.8.6/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 23:13:52.000000 vector_vault-1.8.6/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:14:15.405344 vector_vault-1.8.6/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 23:14:15.000000 vector_vault-1.8.6/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 23:14:15.000000 vector_vault-1.8.6/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 23:14:15.000000 vector_vault-1.8.6/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 23:14:15.000000 vector_vault-1.8.6/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 23:14:15.000000 vector_vault-1.8.6/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:14:15.408516 vector_vault-1.8.6/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.6/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    10755 2023-06-04 18:24:37.000000 vector_vault-1.8.6/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.6/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.6/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.6/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-04 22:09:16.000000 vector_vault-1.8.6/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.6/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    28069 2023-06-04 23:13:42.000000 vector_vault-1.8.6/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-1.8.6/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.6/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:35:41.067160 vector_vault-1.8.7/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.7/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 23:35:41.066989 vector_vault-1.8.7/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.7/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 23:35:41.067198 vector_vault-1.8.7/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 23:35:34.000000 vector_vault-1.8.7/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:35:41.063967 vector_vault-1.8.7/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:35:41.066665 vector_vault-1.8.7/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.7/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    10755 2023-06-04 18:24:37.000000 vector_vault-1.8.7/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.7/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.7/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.7/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-04 22:09:16.000000 vector_vault-1.8.7/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.7/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    28069 2023-06-04 23:35:21.000000 vector_vault-1.8.7/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-1.8.7/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.7/vectorvault/wrap.py
```

### Comparing `vector_vault-1.8.6/LICENSE` & `vector_vault-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/PKG-INFO` & `vector_vault-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.8.6
+Version: 1.8.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.6/README.md` & `vector_vault-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/setup.py` & `vector_vault-1.8.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.8.6",
+    version="1.8.7",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.8.6/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.8.7/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.8.6
+Version: 1.8.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.6/vectorvault/__init__.py` & `vector_vault-1.8.7/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/ai.py` & `vector_vault-1.8.7/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/cloudmanager.py` & `vector_vault-1.8.7/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/creds.py` & `vector_vault-1.8.7/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/download.py` & `vector_vault-1.8.7/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/itemize.py` & `vector_vault-1.8.7/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/signup.py` & `vector_vault-1.8.7/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/vault.py` & `vector_vault-1.8.7/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 import re
 import openai
 import json
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from .cloudmanager import CloudManager
 from .ai import AI
-from .itemize import itemize, name_vecs, get_item, get_vectors
-from .vecreq import call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat, build_return, cloud_name
+from .itemize import itemize, name_vecs, get_item, get_vectors, build_return, cloud_name
+from .vecreq import call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
 
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
```

### Comparing `vector_vault-1.8.6/vectorvault/vecreq.py` & `vector_vault-1.8.7/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.6/vectorvault/wrap.py` & `vector_vault-1.8.7/vectorvault/wrap.py`

 * *Files identical despite different names*

