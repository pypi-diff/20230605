# Comparing `tmp/edgetest-2023.4.0.tar.gz` & `tmp/edgetest-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-2023.4.0.tar", last modified: Mon Apr 10 19:37:55 2023, max compression
+gzip compressed data, was "edgetest-2023.6.0.tar", last modified: Mon Jun  5 18:07:04 2023, max compression
```

## Comparing `edgetest-2023.4.0.tar` & `edgetest-2023.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.486532 edgetest-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:37:17.000000 edgetest-2023.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 19:37:17.000000 edgetest-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:37:17.000000 edgetest-2023.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-10 19:37:55.486532 edgetest-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-10 19:37:17.000000 edgetest-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.482532 edgetest-2023.4.0/edgetest/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.486532 edgetest-2023.4.0/edgetest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:37:47.000000 edgetest-2023.4.0/edgetest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-10 19:37:17.000000 edgetest-2023.4.0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-10 19:37:17.000000 edgetest-2023.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-10 19:37:55.490532 edgetest-2023.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 19:37:17.000000 edgetest-2023.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.486532 edgetest-2023.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_integration_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_integration_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_interface_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_interface_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 18:06:33.000000 edgetest-2023.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:06:33.000000 edgetest-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-05 18:06:33.000000 edgetest-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-05 18:07:04.553540 edgetest-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-05 18:06:33.000000 edgetest-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/edgetest/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/edgetest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:06:37.000000 edgetest-2023.6.0/edgetest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-05 18:06:33.000000 edgetest-2023.6.0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 18:06:33.000000 edgetest-2023.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-05 18:07:04.557540 edgetest-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-05 18:06:33.000000 edgetest-2023.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_integration_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_integration_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_interface_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_interface_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_utils.py
```

### Comparing `edgetest-2023.4.0/LICENSE` & `edgetest-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/PKG-INFO` & `edgetest-2023.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
```

### Comparing `edgetest-2023.4.0/README.md` & `edgetest-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest/core.py` & `edgetest-2023.6.0/edgetest/core.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest/hookspecs.py` & `edgetest-2023.6.0/edgetest/hookspecs.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest/interface.py` & `edgetest-2023.6.0/edgetest/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             package_dir=str(Path(requirements).parent),
         )
     # Validate the configuration file
     docstructure = Schema()
     pm.hook.addoption(schema=docstructure)
     validator = EdgetestValidator(schema=docstructure.schema)
     if not validator.validate(conf):
-        click.echo("Unable to validate configuration file.")
+        click.echo(f"Unable to validate configuration file. Error: {validator.errors}")
         raise ValueError("Unable to validate configuration file.")
     conf = validator.document
 
     if environment:
         conf["envs"] = [env for env in conf["envs"] if env["name"] == environment]
 
     # Run the pre-test hook
```

### Comparing `edgetest-2023.4.0/edgetest/lib.py` & `edgetest-2023.6.0/edgetest/lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest/logger.py` & `edgetest-2023.6.0/edgetest/logger.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest/report.py` & `edgetest-2023.6.0/edgetest/report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest/schema.py` & `edgetest-2023.6.0/edgetest/schema.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest/utils.py` & `edgetest-2023.6.0/edgetest/utils.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest.egg-info/PKG-INFO` & `edgetest-2023.6.0/edgetest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
```

### Comparing `edgetest-2023.4.0/edgetest.egg-info/SOURCES.txt` & `edgetest-2023.6.0/edgetest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/edgetest.egg-info/requires.txt` & `edgetest-2023.6.0/edgetest.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/pull_request_template.md` & `edgetest-2023.6.0/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/requirements.txt` & `edgetest-2023.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/setup.cfg` & `edgetest-2023.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 	bumpver
 
 [options.entry_points]
 console_scripts = 
 	edgetest = edgetest.interface:cli
 
 [bumpver]
-current_version = "2023.4.0"
+current_version = "2023.6.0"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "Bump {old_version} to {new_version}"
 commit = True
 
 [bumpver:file_patterns]
 docs/source/conf.py = 
 	version = "{version}"
```

### Comparing `edgetest-2023.4.0/tests/conftest.py` & `edgetest-2023.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_core.py` & `edgetest-2023.6.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_integration_cfg.py` & `edgetest-2023.6.0/tests/test_integration_cfg.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_integration_toml.py` & `edgetest-2023.6.0/tests/test_integration_toml.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_interface_cfg.py` & `edgetest-2023.6.0/tests/test_interface_cfg.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_interface_toml.py` & `edgetest-2023.6.0/tests/test_interface_toml.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_lib.py` & `edgetest-2023.6.0/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_report.py` & `edgetest-2023.6.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_schema.py` & `edgetest-2023.6.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.4.0/tests/test_utils.py` & `edgetest-2023.6.0/tests/test_utils.py`

 * *Files identical despite different names*

