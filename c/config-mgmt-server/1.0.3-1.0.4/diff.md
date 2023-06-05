# Comparing `tmp/config-mgmt-server-1.0.3.tar.gz` & `tmp/config_mgmt_server-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config-mgmt-server-1.0.3.tar", last modified: Sun Apr 23 23:06:33 2023, max compression
+gzip compressed data, was "config_mgmt_server-1.0.4.tar", last modified: Mon Jun  5 21:08:39 2023, max compression
```

## Comparing `config-mgmt-server-1.0.3.tar` & `config_mgmt_server-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:06:33.906848 config-mgmt-server-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-23 23:06:33.906848 config-mgmt-server-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 23:06:33.906848 config-mgmt-server-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:06:33.906848 config-mgmt-server-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:06:33.906848 config-mgmt-server-1.0.3/src/config_mgmt_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/src/config_mgmt_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/src/config_mgmt_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:06:33.906848 config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-23 23:06:33.000000 config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-23 23:06:33.000000 config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:06:33.000000 config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 23:06:33.000000 config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 23:06:33.000000 config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 23:06:33.000000 config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:06:33.906848 config-mgmt-server-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/tests/test_my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-23 23:06:24.000000 config-mgmt-server-1.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:08:39.318721 config_mgmt_server-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:08:39.318721 config_mgmt_server-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:08:39.318721 config_mgmt_server-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:08:39.314721 config_mgmt_server-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:08:39.314721 config_mgmt_server-1.0.4/src/config_mgmt_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/src/config_mgmt_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/src/config_mgmt_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:08:39.318721 config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:08:39.000000 config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-05 21:08:39.000000 config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:08:39.000000 config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 21:08:39.000000 config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 21:08:39.000000 config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:08:39.000000 config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:08:39.318721 config_mgmt_server-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/tests/test_my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-05 21:08:29.000000 config_mgmt_server-1.0.4/tox.ini
```

### Comparing `config-mgmt-server-1.0.3/PKG-INFO` & `config_mgmt_server-1.0.4/src/config_mgmt_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-mgmt-server
-Version: 1.0.3
+Version: 1.0.4
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config-mgmt-server-1.0.3/README.md` & `config_mgmt_server-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `config-mgmt-server-1.0.3/pyproject.toml` & `config_mgmt_server-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 # $ pip install sampleproject
 #
 # And where it will live on PyPI: https://pypi.org/project/sampleproject/
 #
 # There are some restrictions on what makes a valid project name
 # specification here:
 # https://packaging.python.org/specifications/core-metadata/#name
-name = "config-mgmt-server"  # Required
+name = "config_mgmt_server"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.3"  # Required
+version = "1.0.4"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Suncoast Systems Core Router Config Mgmt Server"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `config-mgmt-server-1.0.3/requirements.txt` & `config_mgmt_server-1.0.4/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # ./vscode/settings.json use binaries that must be installed with this requirements : `pip install -r requirements.txt`
 # A formatter for Python code
 pep8==1.4.4
 autopep8==1.4.4
+
+backports.zoneinfo==0.2.1;python_version<"3.9"
+
 # Python code static checker
 pylint==2.3.1
 # simple powerful testing with Python
 pytest==4.5.0
 # plugin for pytest to produces coverage reports
 pytest-cov==2.7.1
 # Type safety
```

### Comparing `config-mgmt-server-1.0.3/src/config_mgmt_server.egg-info/PKG-INFO` & `config_mgmt_server-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: config-mgmt-server
-Version: 1.0.3
+Name: config_mgmt_server
+Version: 1.0.4
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config-mgmt-server-1.0.3/tests/requirements.txt` & `config_mgmt_server-1.0.4/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `config-mgmt-server-1.0.3/tox.ini` & `config_mgmt_server-1.0.4/tox.ini`

 * *Files identical despite different names*

