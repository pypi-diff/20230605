# Comparing `tmp/stc-tools-1.2.1.tar.gz` & `tmp/stc-tools-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-tools-1.2.1.tar", last modified: Mon Jun  5 12:43:31 2023, max compression
+gzip compressed data, was "stc-tools-1.2.2.tar", last modified: Mon Jun  5 12:53:25 2023, max compression
```

## Comparing `stc-tools-1.2.1.tar` & `stc-tools-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:43:31.840297 stc-tools-1.2.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.2.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-05 12:43:31.839478 stc-tools-1.2.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.2.1/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      560 2023-06-05 12:42:41.000000 stc-tools-1.2.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-03 20:43:36.000000 stc-tools-1.2.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-05 12:43:31.840606 stc-tools-1.2.1/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:43:31.826269 stc-tools-1.2.1/stc_tools/
--rw-r--r--   0 pasha      (501) staff       (20)     4499 2023-06-03 16:05:24.000000 stc-tools-1.2.1/stc_tools/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     3037 2023-06-05 12:42:31.000000 stc-tools-1.2.1/stc_tools/client.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:43:31.836189 stc-tools-1.2.1/stc_tools.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      290 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       49 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       44 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-05 12:43:31.000000 stc-tools-1.2.1/stc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:53:25.386661 stc-tools-1.2.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.2.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-05 12:53:25.385378 stc-tools-1.2.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.2.2/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      560 2023-06-05 12:52:34.000000 stc-tools-1.2.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-03 20:43:36.000000 stc-tools-1.2.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-05 12:53:25.387004 stc-tools-1.2.2/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:53:25.373047 stc-tools-1.2.2/stc_tools/
+-rw-r--r--   0 pasha      (501) staff       (20)     4499 2023-06-03 16:05:24.000000 stc-tools-1.2.2/stc_tools/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3037 2023-06-05 12:52:55.000000 stc-tools-1.2.2/stc_tools/client.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-05 12:53:25.381457 stc-tools-1.2.2/stc_tools.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-05 12:53:25.000000 stc-tools-1.2.2/stc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      290 2023-06-05 12:53:25.000000 stc-tools-1.2.2/stc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-05 12:53:25.000000 stc-tools-1.2.2/stc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       49 2023-06-05 12:53:25.000000 stc-tools-1.2.2/stc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       44 2023-06-05 12:53:25.000000 stc-tools-1.2.2/stc_tools.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-05 12:53:25.000000 stc-tools-1.2.2/stc_tools.egg-info/top_level.txt
```

### Comparing `stc-tools-1.2.1/pyproject.toml` & `stc-tools-1.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-tools"
-version = "1.2.1"
+version = "1.2.2"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Standard Template Construct Client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-tools-1.2.1/stc_tools/cli.py` & `stc-tools-1.2.2/stc_tools/cli.py`

 * *Files identical despite different names*

### Comparing `stc-tools-1.2.1/stc_tools/client.py` & `stc-tools-1.2.2/stc_tools/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,17 @@
         for path in self.paths:
             full_path = self.ipfs_http_endpoint + path
             headers_template = {"range": "bytes={start}-{end}"}
             if host_header := await detect_host_header(full_path):
                 headers_template['host'] = host_header
             index_name = path.rstrip('/').rsplit('/', 1)[1]
             field_aliases = {
-                'references.doi': 'rd',
-                'metadata.issns': 'issns',
-                'metadata.isbns': 'isbns'
+                'rd': 'references.doi',
+                'issns': 'metadata.issns',
+                'isbns': 'metadata.isbns'
             }
             description = await self.index_registry.add({
                 'remote': {
                     'method': 'GET',
                     'url_template': f'{full_path}{{file_name}}',
                     'headers_template': headers_template,
                     'cache_config': {'cache_size': self.cache_size},
```

