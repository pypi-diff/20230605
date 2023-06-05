# Comparing `tmp/stc-tools-1.2.0.tar.gz` & `tmp/stc-tools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-tools-1.2.0.tar", last modified: Sat Jun  3 17:51:05 2023, max compression
+gzip compressed data, was "stc-tools-1.2.1.tar", last modified: Mon Jun  5 12:43:31 2023, max compression
```

## Comparing `stc-tools-1.2.0.tar` & `stc-tools-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 17:51:05.026045 stc-tools-1.2.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.2.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-03 17:51:05.025719 stc-tools-1.2.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.2.0/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      560 2023-06-03 17:50:38.000000 stc-tools-1.2.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-03 17:46:10.000000 stc-tools-1.2.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-03 17:51:05.026168 stc-tools-1.2.0/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 17:51:05.020744 stc-tools-1.2.0/stc_tools/
--rw-r--r--   0 pasha      (501) staff       (20)     4499 2023-06-03 16:05:24.000000 stc-tools-1.2.0/stc_tools/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     2770 2023-06-03 11:42:04.000000 stc-tools-1.2.0/stc_tools/client.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 17:51:05.025058 stc-tools-1.2.0/stc_tools.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      290 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       49 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       44 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:43:31.840297 stc-tools-1.2.1/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.2.1/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-05 12:43:31.839478 stc-tools-1.2.1/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.2.1/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      560 2023-06-05 12:42:41.000000 stc-tools-1.2.1/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-03 20:43:36.000000 stc-tools-1.2.1/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-05 12:43:31.840606 stc-tools-1.2.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:43:31.826269 stc-tools-1.2.1/stc_tools/
+-rw-r--r--   0 pasha      (501) staff       (20)     4499 2023-06-03 16:05:24.000000 stc-tools-1.2.1/stc_tools/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3037 2023-06-05 12:42:31.000000 stc-tools-1.2.1/stc_tools/client.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:43:31.836189 stc-tools-1.2.1/stc_tools.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      290 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       49 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       44 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/top_level.txt
```

### Comparing `stc-tools-1.2.0/pyproject.toml` & `stc-tools-1.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-tools"
-version = "1.2.0"
+version = "1.2.1"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Standard Template Construct Client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-tools-1.2.0/stc_tools/cli.py` & `stc-tools-1.2.1/stc_tools/cli.py`

 * *Files identical despite different names*

### Comparing `stc-tools-1.2.0/stc_tools/client.py` & `stc-tools-1.2.1/stc_tools/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,20 +35,28 @@
     async def start(self):
         for path in self.paths:
             full_path = self.ipfs_http_endpoint + path
             headers_template = {"range": "bytes={start}-{end}"}
             if host_header := await detect_host_header(full_path):
                 headers_template['host'] = host_header
             index_name = path.rstrip('/').rsplit('/', 1)[1]
-            description = await self.index_registry.add({'remote': {
-                'method': 'GET',
-                'url_template': f'{full_path}{{file_name}}',
-                'headers_template': headers_template,
-                'cache_config': {'cache_size': self.cache_size},
-            }}, index_name=index_name)
+            field_aliases = {
+                'references.doi': 'rd',
+                'metadata.issns': 'issns',
+                'metadata.isbns': 'isbns'
+            }
+            description = await self.index_registry.add({
+                'remote': {
+                    'method': 'GET',
+                    'url_template': f'{full_path}{{file_name}}',
+                    'headers_template': headers_template,
+                    'cache_config': {'cache_size': self.cache_size},
+                },
+                'field_aliases': field_aliases
+            }, index_name=index_name)
             self.descriptions[description.default_index_name] = description
         return self.descriptions
 
     async def search(self, query: List[dict]):
         return await self.index_registry.search(query)
 
     async def get_one_by_field_value(self, index_alias, field, value):
```

