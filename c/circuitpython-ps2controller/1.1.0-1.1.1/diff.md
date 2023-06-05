# Comparing `tmp/circuitpython-ps2controller-1.1.0.tar.gz` & `tmp/circuitpython-ps2controller-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ps2controller-1.1.0.tar", last modified: Sun Jun  4 23:41:54 2023, max compression
+gzip compressed data, was "circuitpython-ps2controller-1.1.1.tar", last modified: Sun Jun  4 23:58:43 2023, max compression
```

## Comparing `circuitpython-ps2controller-1.1.0.tar` & `circuitpython-ps2controller-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.975868 circuitpython-ps2controller-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/examples/ps2controller_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/examples/ps2controller_usbkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/ps2controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.198391 circuitpython-ps2controller-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.190391 circuitpython-ps2controller-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-04 23:58:43.000000 circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-04 23:58:43.000000 circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:58:43.000000 circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-04 23:58:43.000000 circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 23:58:43.000000 circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:58:43.194391 circuitpython-ps2controller-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 23:58:34.000000 circuitpython-ps2controller-1.1.1/examples/ps2controller_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-04 23:58:34.000000 circuitpython-ps2controller-1.1.1/examples/ps2controller_usbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-06-04 23:58:34.000000 circuitpython-ps2controller-1.1.1/ps2controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-04 23:58:34.000000 circuitpython-ps2controller-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-04 23:58:20.000000 circuitpython-ps2controller-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:58:43.198391 circuitpython-ps2controller-1.1.1/setup.cfg
```

### Comparing `circuitpython-ps2controller-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-ps2controller-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/.github/workflows/release_gh.yml` & `circuitpython-ps2controller-1.1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/.gitignore` & `circuitpython-ps2controller-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/.pre-commit-config.yaml` & `circuitpython-ps2controller-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/.pylintrc` & `circuitpython-ps2controller-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/CODE_OF_CONDUCT.md` & `circuitpython-ps2controller-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/LICENSE` & `circuitpython-ps2controller-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-ps2controller-1.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/LICENSES/MIT.txt` & `circuitpython-ps2controller-1.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/LICENSES/Unlicense.txt` & `circuitpython-ps2controller-1.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/PKG-INFO` & `circuitpython-ps2controller-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ps2controller
-Version: 1.1.0
+Version: 1.1.1
 Summary: CircuitPython library to read Sony PS2 game controllers
 Author-email: Tod Kurt <tod@todbot.com>
 License: MIT
 Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
 Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ps2controller-1.1.0/README.rst` & `circuitpython-ps2controller-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/PKG-INFO` & `circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ps2controller
-Version: 1.1.0
+Version: 1.1.1
 Summary: CircuitPython library to read Sony PS2 game controllers
 Author-email: Tod Kurt <tod@todbot.com>
 License: MIT
 Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
 Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/SOURCES.txt` & `circuitpython-ps2controller-1.1.1/circuitpython_ps2controller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/docs/_static/favicon.ico` & `circuitpython-ps2controller-1.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/docs/conf.py` & `circuitpython-ps2controller-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/docs/index.rst` & `circuitpython-ps2controller-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/examples/ps2controller_usbkeys.py` & `circuitpython-ps2controller-1.1.1/examples/ps2controller_usbkeys.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.0/ps2controller.py` & `circuitpython-ps2controller-1.1.1/ps2controller.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   https://circuitpython.org/downloads
 
 
 """
 
 # imports
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/todbot/CircuitPython_PS2Controller.git"
 
 
 from collections import namedtuple
 import time
 from micropython import const
 import digitalio
@@ -63,29 +63,45 @@
 
 
 # pylint: disable-msg=(invalid-name, too-few-public-methods)
 class PS2Button:
     """PS2 Button constants mapping button name to number"""
 
     SELECT = 0
+    """SELECT button, digital only"""
     L3 = 1
+    """L3 button (left stick push), digital only"""
     R3 = 2
+    """R3 button (right stick push), digital only"""
     START = 3
+    """START button, digital only (pressure)"""
     UP = 4
+    """D-pad UP, digital and analog (pressure)"""
     RIGHT = 5
+    """D-pad RIGHT, digital and analog (pressure)"""
     DOWN = 6
+    """D-pad DOWN, digital and analog (pressure)"""
     LEFT = 7
+    """D-pad LEFT, digital and analog (pressure)"""
     L2 = 8
+    """Left lower shoulder trigger button, digital and analog (pressure)"""
     R2 = 9
+    """Right lower shoulder trigger button, digital and analog (pressure)"""
     L1 = 10
+    """Left upper shoulder trigger button, digital and analog (pressure)"""
     R1 = 11
+    """Right upper shoulder trigger button, digital and analog (pressure)"""
     TRIANGLE = 12
+    """Triangle (green) action button, digital and analog (pressure)"""
     CIRCLE = 13
+    """Circle (red) action button, digital and analog (pressure)"""
     CROSS = 14
+    """Cross (blue) action button, digital and analog (pressure)"""
     SQUARE = 15
+    """Square (pink) action button, digital and analog (pressure)"""
 
     # fmt: off
     button_to_analog_id = (-1, -1, -1, -1, 11, 9, 12, 10, 19, 20, 17, 18, 13, 14, 15, 16)
 
     names = ("SELECT", "L3", "R3", "START", "UP", "RIGHT", "DOWN", "LEFT",
              "L2", "R2", "L1", "R1", "TRIANGLE", "CIRCLE", "CROSS", "SQUARE")
     # fmt: on
```

### Comparing `circuitpython-ps2controller-1.1.0/pyproject.toml` & `circuitpython-ps2controller-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-ps2controller"
 description = "CircuitPython library to read Sony PS2 game controllers"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.rst"
 authors = [
     {name = "Tod Kurt", email = "tod@todbot.com"}
 ]
 urls = {Homepage = "https://github.com/todbot/CircuitPython_PS2Controller"}
 keywords = [
     "adafruit",
```

