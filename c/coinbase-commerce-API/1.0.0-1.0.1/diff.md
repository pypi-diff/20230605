# Comparing `tmp/coinbase-commerce-API-1.0.0.tar.gz` & `tmp/coinbase-commerce-API-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinbase-commerce-API-1.0.0.tar", last modified: Sat Jun  3 12:52:18 2023, max compression
+gzip compressed data, was "coinbase-commerce-API-1.0.1.tar", last modified: Mon Jun  5 15:50:45 2023, max compression
```

## Comparing `coinbase-commerce-API-1.0.0.tar` & `coinbase-commerce-API-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-03 12:52:18.877431 coinbase-commerce-API-1.0.0/
--rw-r--r--   0 macbookair   (501) staff       (20)      723 2023-06-03 12:52:18.877310 coinbase-commerce-API-1.0.0/PKG-INFO
-drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-03 12:52:18.876316 coinbase-commerce-API-1.0.0/cbc_api/
--rw-r--r--   0 macbookair   (501) staff       (20)       43 2023-06-03 12:28:35.000000 coinbase-commerce-API-1.0.0/cbc_api/ __init__.py
--rw-r--r--   0 macbookair   (501) staff       (20)     5232 2023-06-03 11:42:38.000000 coinbase-commerce-API-1.0.0/cbc_api/cbc_api.py
-drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-03 12:52:18.877127 coinbase-commerce-API-1.0.0/coinbase_commerce_API.egg-info/
--rw-r--r--   0 macbookair   (501) staff       (20)      723 2023-06-03 12:52:18.000000 coinbase-commerce-API-1.0.0/coinbase_commerce_API.egg-info/PKG-INFO
--rw-r--r--   0 macbookair   (501) staff       (20)      272 2023-06-03 12:52:18.000000 coinbase-commerce-API-1.0.0/coinbase_commerce_API.egg-info/SOURCES.txt
--rw-r--r--   0 macbookair   (501) staff       (20)        1 2023-06-03 12:52:18.000000 coinbase-commerce-API-1.0.0/coinbase_commerce_API.egg-info/dependency_links.txt
--rw-r--r--   0 macbookair   (501) staff       (20)        9 2023-06-03 12:52:18.000000 coinbase-commerce-API-1.0.0/coinbase_commerce_API.egg-info/requires.txt
--rw-r--r--   0 macbookair   (501) staff       (20)        8 2023-06-03 12:52:18.000000 coinbase-commerce-API-1.0.0/coinbase_commerce_API.egg-info/top_level.txt
--rw-r--r--   0 macbookair   (501) staff       (20)       38 2023-06-03 12:52:18.877463 coinbase-commerce-API-1.0.0/setup.cfg
--rw-r--r--   0 macbookair   (501) staff       (20)      865 2023-06-03 12:51:11.000000 coinbase-commerce-API-1.0.0/setup.py
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-05 15:50:45.870901 coinbase-commerce-API-1.0.1/
+-rw-r--r--   0 macbookair   (501) staff       (20)      723 2023-06-05 15:50:45.870779 coinbase-commerce-API-1.0.1/PKG-INFO
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-05 15:50:45.869826 coinbase-commerce-API-1.0.1/cbc_api/
+-rw-r--r--   0 macbookair   (501) staff       (20)       43 2023-06-03 12:28:35.000000 coinbase-commerce-API-1.0.1/cbc_api/ __init__.py
+-rw-r--r--   0 macbookair   (501) staff       (20)     5233 2023-06-05 15:46:52.000000 coinbase-commerce-API-1.0.1/cbc_api/cbc_api.py
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-05 15:50:45.870581 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/
+-rw-r--r--   0 macbookair   (501) staff       (20)      723 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/PKG-INFO
+-rw-r--r--   0 macbookair   (501) staff       (20)      272 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        1 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        9 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/requires.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        8 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/top_level.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)       38 2023-06-05 15:50:45.870943 coinbase-commerce-API-1.0.1/setup.cfg
+-rw-r--r--   0 macbookair   (501) staff       (20)      865 2023-06-05 15:47:39.000000 coinbase-commerce-API-1.0.1/setup.py
```

### Comparing `coinbase-commerce-API-1.0.0/PKG-INFO` & `coinbase-commerce-API-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-commerce-API
-Version: 1.0.0
+Version: 1.0.1
 Summary: Coinbase Commerce API library. See github.
 Home-page: https://github.com/Rushifakami/API-Coinbase-Commerce-cbc_api
 Author: Rushifakami
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coinbase-commerce-API-1.0.0/cbc_api/cbc_api.py` & `coinbase-commerce-API-1.0.1/cbc_api/cbc_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return response
 
     def charge_cancel(self, charge_code):
         response = requests.post(f'https://api.commerce.coinbase.com/charges/{charge_code}/cancel', headers=self.headers).json()
         return response
 
     def charge_resolve(self, charge_code):
-        response = requests.get(f'https://api.commerce.coinbase.com/charges/{charge_code}/resolve', headers=self.headers).json()
+        response = requests.post(f'https://api.commerce.coinbase.com/charges/{charge_code}/resolve', headers=self.headers).json()
         return response
 
     def checkouts_list(self):
         response = requests.get('https://api.commerce.coinbase.com/checkouts', headers=self.headers).json()
         return response
 
     def checkouts_create(self, name, description, requested_info, pricing_type='no_price', amount=None, currency='USD'):
```

### Comparing `coinbase-commerce-API-1.0.0/coinbase_commerce_API.egg-info/PKG-INFO` & `coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-commerce-API
-Version: 1.0.0
+Version: 1.0.1
 Summary: Coinbase Commerce API library. See github.
 Home-page: https://github.com/Rushifakami/API-Coinbase-Commerce-cbc_api
 Author: Rushifakami
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coinbase-commerce-API-1.0.0/setup.py` & `coinbase-commerce-API-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='coinbase-commerce-API',
-    version='1.0.0',
+    version='1.0.1',
     author='Rushifakami',
     description='Coinbase Commerce API library. See github.',
     packages=['cbc_api'],
     install_requires=[
         'requests',
     ],
     url='https://github.com/Rushifakami/API-Coinbase-Commerce-cbc_api',
```

