# Comparing `tmp/dcentrapi-0.2.4.tar.gz` & `tmp/dcentrapi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dcentrapi-0.2.4.tar", last modified: Thu Jun  1 15:26:29 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.5.tar", last modified: Mon Jun  5 07:36:54 2023, max compression
```

## Comparing `dcentrapi-0.2.4.tar` & `dcentrapi-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-06-01 15:26:29.671601 dcentrapi-0.2.4/
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     1073 2022-06-21 11:33:40.000000 dcentrapi-0.2.4/LICENSE.rst
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     6741 2023-06-01 15:26:29.671413 dcentrapi-0.2.4/PKG-INFO
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     6211 2022-09-26 09:54:00.000000 dcentrapi-0.2.4/README.md
-drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-06-01 15:26:29.670482 dcentrapi-0.2.4/dcentrapi/
--rw-r--r--   0 jovanvuleta   (501) staff       (20)      829 2023-05-09 15:11:33.000000 dcentrapi-0.2.4/dcentrapi/Base.py
--rw-r--r--   0 jovanvuleta   (501) staff       (20)      280 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/dcentrapi/__init__.py
--rw-r--r--   0 jovanvuleta   (501) staff       (20)       63 2023-06-01 15:06:39.000000 dcentrapi-0.2.4/dcentrapi/common.py
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     8714 2023-06-01 15:10:16.000000 dcentrapi-0.2.4/dcentrapi/eventPolling.py
--rw-r--r--   0 jovanvuleta   (501) staff       (20)      491 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/dcentrapi/gasMonitor.py
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     3078 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/dcentrapi/merkleTree.py
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     3850 2023-06-01 14:51:58.000000 dcentrapi-0.2.4/dcentrapi/rpcAggregation.py
--rw-r--r--   0 jovanvuleta   (501) staff       (20)      804 2023-06-01 14:51:58.000000 dcentrapi-0.2.4/dcentrapi/web3Index.py
-drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-06-01 15:26:29.671183 dcentrapi-0.2.4/dcentrapi.egg-info/
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     6741 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 jovanvuleta   (501) staff       (20)      379 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 jovanvuleta   (501) staff       (20)        1 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 jovanvuleta   (501) staff       (20)        9 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 jovanvuleta   (501) staff       (20)       10 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 jovanvuleta   (501) staff       (20)       38 2023-06-01 15:26:29.671656 dcentrapi-0.2.4/setup.cfg
--rw-r--r--   0 jovanvuleta   (501) staff       (20)     1167 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/setup.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-05 07:36:54.163551 dcentrapi-0.2.5/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.5/LICENSE.rst
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-06-05 07:36:54.163414 dcentrapi-0.2.5/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.5/README.md
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-05 07:36:54.162538 dcentrapi-0.2.5/dcentrapi/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.5/dcentrapi/Base.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.2.5/dcentrapi/__init__.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-06-05 07:36:32.000000 dcentrapi-0.2.5/dcentrapi/common.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     8714 2023-06-05 07:36:17.000000 dcentrapi-0.2.5/dcentrapi/eventPolling.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.5/dcentrapi/gasMonitor.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.5/dcentrapi/merkleTree.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3059 2023-06-05 07:36:17.000000 dcentrapi-0.2.5/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      804 2023-05-31 13:35:59.000000 dcentrapi-0.2.5/dcentrapi/web3Index.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-05 07:36:54.163254 dcentrapi-0.2.5/dcentrapi.egg-info/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-05 07:36:54.163613 dcentrapi-0.2.5/setup.cfg
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.5/setup.py
```

### Comparing `dcentrapi-0.2.4/LICENSE.rst` & `dcentrapi-0.2.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.4/PKG-INFO` & `dcentrapi-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.4
+Version: 0.2.5
 Summary: Dcentralab Pypi packages
+Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -103,7 +105,9 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+
+
```

### Comparing `dcentrapi-0.2.4/README.md` & `dcentrapi-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.4/dcentrapi/Base.py` & `dcentrapi-0.2.5/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.4/dcentrapi/eventPolling.py` & `dcentrapi-0.2.5/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.4/dcentrapi/merkleTree.py` & `dcentrapi-0.2.5/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.4/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.5/dcentrapi/rpcAggregation.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,42 +36,28 @@
 
     def get_reserves_from_pair(self, pool, network, rpc_url=None):
         url = self.url + "getReservesFromPair"
         data = {"network": network, "lp_token": pool, "rpc_url": rpc_url}
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
-    # DEPRECATED, use get_reserves_from_pools instead, it is more general
-    def get_reserves_from_pairs(self, pools: list, network, rpc_url=None):
-        url = self.url + "getReservesFromPairs"
-        data = {"network": network, "lp_tokens": pools, "rpc_url": rpc_url}
-        response = requests.post(url, json=data, headers=self.headers)
-        return response.json()
-
     # Accepted values for factory_type (May 2023):
     # UNI_V2, UNI_V3, CURVE, BALANCER
 
     def get_reserves_from_pools(self, factory_type, pools: list, network, rpc_url=None):
         url = self.url + "getReservesFromPools"
         data = {
             "factory_type": factory_type,
             "pools": pools,
             "network": network,
             "rpc_url": rpc_url
         }
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
-    # DEPRECATED, use get_pool_data_from_factory instead, it is more general
-    def get_pair_data_from_factory(self, factory, indices: list, network, rpc_url=None):
-        url = self.url + "getPairDataFromFactory"
-        data = {"factory": factory, "indices": indices, "network": network, "rpc_url": rpc_url}
-        response = requests.post(url, json=data, headers=self.headers)
-        return response.json()
-
     # Same accepted factory_type values as for get_reserves_from_pools above
     def get_pool_data_from_factory(self, factory_type, factory, indices: list, network, rpc_url=None):
         url = self.url + "getPoolDataFromFactory"
         data = {
             "factory_type": factory_type,
             "factory": factory,
             "indices": indices,
```

### Comparing `dcentrapi-0.2.4/dcentrapi/web3Index.py` & `dcentrapi-0.2.5/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.4/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.5/dcentrapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.4
+Version: 0.2.5
 Summary: Dcentralab Pypi packages
+Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -103,7 +105,9 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+
+
```

### Comparing `dcentrapi-0.2.4/setup.py` & `dcentrapi-0.2.5/setup.py`

 * *Files identical despite different names*

