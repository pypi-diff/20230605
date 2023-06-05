# Comparing `tmp/config_mgmt_server-1.0.6.tar.gz` & `tmp/config_mgmt_server-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_mgmt_server-1.0.6.tar", last modified: Mon Jun  5 21:21:18 2023, max compression
+gzip compressed data, was "config_mgmt_server-1.0.7.tar", last modified: Mon Jun  5 21:52:35 2023, max compression
```

## Comparing `config_mgmt_server-1.0.6.tar` & `config_mgmt_server-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:21:18.116829 config_mgmt_server-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:21:18.116829 config_mgmt_server-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:21:18.116829 config_mgmt_server-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:21:18.112829 config_mgmt_server-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:21:18.116829 config_mgmt_server-1.0.6/src/config_mgmt_server/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/src/config_mgmt_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/src/config_mgmt_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:21:18.116829 config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:21:18.000000 config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-05 21:21:18.000000 config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:21:18.000000 config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 21:21:18.000000 config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 21:21:18.000000 config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:21:18.000000 config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:21:18.116829 config_mgmt_server-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/tests/test_my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-05 21:21:00.000000 config_mgmt_server-1.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/src/config_mgmt_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/src/config_mgmt_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/src/config_mgmt_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/tests/test_my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/tox.ini
```

### Comparing `config_mgmt_server-1.0.6/PKG-INFO` & `config_mgmt_server-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config_mgmt_server
-Version: 1.0.6
+Version: 1.0.7
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config_mgmt_server-1.0.6/README.md` & `config_mgmt_server-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `config_mgmt_server-1.0.6/pyproject.toml` & `config_mgmt_server-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "config_mgmt_server"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.6"  # Required
+version = "1.0.7"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Suncoast Systems Core Router Config Mgmt Server"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `config_mgmt_server-1.0.6/requirements.txt` & `config_mgmt_server-1.0.7/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ./vscode/settings.json use binaries that must be installed with this requirements : `pip install -r requirements.txt`
 # A formatter for Python code
 pep8==1.4.4
 autopep8==1.4.4
 
-backports.zoneinfo;python_version<"3.9"
+backports.zoneinfo;python_version<"3.2"
 
 # Python code static checker
 pylint==2.3.1
 # simple powerful testing with Python
 pytest==4.5.0
 # plugin for pytest to produces coverage reports
 pytest-cov==2.7.1
```

### Comparing `config_mgmt_server-1.0.6/src/config_mgmt_server/app.py` & `config_mgmt_server-1.0.7/src/config_mgmt_server/app.py`

 * *Files identical despite different names*

### Comparing `config_mgmt_server-1.0.6/src/config_mgmt_server.egg-info/PKG-INFO` & `config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-mgmt-server
-Version: 1.0.6
+Version: 1.0.7
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config_mgmt_server-1.0.6/tests/requirements.txt` & `config_mgmt_server-1.0.7/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `config_mgmt_server-1.0.6/tox.ini` & `config_mgmt_server-1.0.7/tox.ini`

 * *Files identical despite different names*

