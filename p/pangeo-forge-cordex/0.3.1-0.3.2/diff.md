# Comparing `tmp/pangeo-forge-cordex-0.3.1.tar.gz` & `tmp/pangeo-forge-cordex-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.3.1.tar", last modified: Sun May  7 20:16:27 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.3.2.tar", last modified: Mon Jun  5 11:45:04 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.3.1.tar` & `pangeo-forge-cordex-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.056574 pangeo-forge-cordex-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.068575 pangeo-forge-cordex-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.068575 pangeo-forge-cordex-0.3.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.072575 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-07 20:16:27.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-07 20:16:27.080575 pangeo-forge-cordex-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.517220 pangeo-forge-cordex-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-05 11:45:04.525220 pangeo-forge-cordex-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.3.1/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.3.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.3.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/.gitignore` & `pangeo-forge-cordex-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/LICENSE` & `pangeo-forge-cordex-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/PKG-INFO` & `pangeo-forge-cordex-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.1
+Version: 0.3.2
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/catalog.py` & `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from os import path as op
 
 from .parsing import project_from_iid
 
+# the facet names in the intake catalogs differ from those in the ESGF API
+# since the intake facets represent actual datasets attributes.
 cordex_cmip5_facets = [
     "project_id",
     "product",
     "CORDEX_domain",
     "institute_id",
     "driving_model_id",
     "experiment_id",
@@ -13,19 +15,34 @@
     "model_id",
     "rcm_version_id",
     "frequency",
     "variable_id",
     "version",
 ]
 
+cordex_adjust_facets = [
+    "project_id",
+    "product",
+    "CORDEX_domain",
+    "institute_id",
+    "driving_model_id",
+    "experiment_id",
+    "member",
+    "model_id",
+    "bias_adjustment",
+    "frequency",
+    "variable_id",
+    "version",
+]
+
 catalog_facets = {
     "CORDEX": cordex_cmip5_facets,
     "CORDEX-Reklies": cordex_cmip5_facets,
-    "CORDEX-Adjust": None,
-    "CORDEX-ESD": None,
+    "CORDEX-Adjust": cordex_adjust_facets,
+    "CORDEX-ESD": cordex_cmip5_facets,
 }
 
 
 def facets_from_iid(iid, facets=None):
     """get catalog attributes from iid"""
     if facets is None:
         project = project_from_iid(iid)
```

### Comparing `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/esgf_access.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 import ssl
 
 import requests
 
 from .utils import combine_response, parse_dataset_response, sort_files_by_dataset_id
 
 
-def logon():
+def logon(host=None):
     from pyesgf.logon import LogonManager
 
+    if host is None:
+        host = "esgf-data.dkrz.de"
     lm = LogonManager(verify=True)
     if not lm.is_logged_on():
-        myproxy_host = "esgf-data.dkrz.de"
         # if we find those in environment, use them.
         if "ESGF_USER" in os.environ and "ESGF_PASSWORD" in os.environ:
             lm.logon(
-                hostname=myproxy_host,
+                hostname=host,
                 username=os.environ["ESGF_USER"],
                 password=os.environ["ESGF_PASSWORD"],
                 interactive=False,
                 bootstrap=True,
             )
         else:
             lm.logon(
-                hostname=myproxy_host,
+                hostname=host,
                 interactive=True,
                 bootstrap=True,
             )
 
     print(f"logged on: {lm.is_logged_on()}")
 
     # create SSL context
```

### Comparing `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/recipe.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.1
+Version: 0.3.2
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/setup.cfg` & `pangeo-forge-cordex-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/tests/test_parsing.py` & `pangeo-forge-cordex-0.3.2/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.1/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.3.2/tests/test_recipe_creation.py`

 * *Files identical despite different names*

