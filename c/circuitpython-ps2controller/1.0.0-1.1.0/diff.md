# Comparing `tmp/circuitpython-ps2controller-1.0.0.tar.gz` & `tmp/circuitpython-ps2controller-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ps2controller-1.0.0.tar", last modified: Sat Jun  3 21:03:15 2023, max compression
+gzip compressed data, was "circuitpython-ps2controller-1.1.0.tar", last modified: Sun Jun  4 23:41:54 2023, max compression
```

## Comparing `circuitpython-ps2controller-1.0.0.tar` & `circuitpython-ps2controller-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.332897 circuitpython-ps2controller-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-03 21:03:15.000000 circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-03 21:03:15.000000 circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:03:15.000000 circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-03 21:03:15.000000 circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-03 21:03:15.000000 circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-03 21:03:08.000000 circuitpython-ps2controller-1.0.0/examples/ps2controller_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-06-03 21:03:08.000000 circuitpython-ps2controller-1.0.0/ps2controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-03 21:03:08.000000 circuitpython-ps2controller-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-03 21:03:01.000000 circuitpython-ps2controller-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 21:03:15.336897 circuitpython-ps2controller-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.975868 circuitpython-ps2controller-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 23:41:54.000000 circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/examples/ps2controller_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/examples/ps2controller_usbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/ps2controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-04 23:41:47.000000 circuitpython-ps2controller-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-04 23:41:39.000000 circuitpython-ps2controller-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:41:54.979867 circuitpython-ps2controller-1.1.0/setup.cfg
```

### Comparing `circuitpython-ps2controller-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-ps2controller-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/.github/workflows/release_gh.yml` & `circuitpython-ps2controller-1.1.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/.gitignore` & `circuitpython-ps2controller-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/.pre-commit-config.yaml` & `circuitpython-ps2controller-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/.pylintrc` & `circuitpython-ps2controller-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/CODE_OF_CONDUCT.md` & `circuitpython-ps2controller-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/LICENSE` & `circuitpython-ps2controller-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-ps2controller-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/LICENSES/MIT.txt` & `circuitpython-ps2controller-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/LICENSES/Unlicense.txt` & `circuitpython-ps2controller-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/PKG-INFO` & `circuitpython-ps2controller-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: circuitpython-ps2controller
-Version: 1.0.0
+Version: 1.1.0
 Summary: CircuitPython library to read Sony PS2 game controllers
 Author-email: Tod Kurt <tod@todbot.com>
 License: MIT
 Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
-Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,controller,gamepad,sony,dualshock
+Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
@@ -49,16 +49,14 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-ps2controller/>`_.
 To install for current user:
 
 .. code-block:: shell
 
@@ -117,14 +115,29 @@
     while True:
         events = ps2.update()
         if events:
             print("events", events)
             print("sticks: L:", ps2.analog_left(), "R:", ps2.analog_right())
 
 
+References
+==========
+
+This library is a fairly direct port of `madsci1016/Arduino-PS2X <https://github.com/madsci1016/Arduino-PS2X>`_.
+
+Other resources that have been helpful:
+
+* https://store.curiousinventor.com/guides/PS2/
+* https://gist.github.com/scanlime/5042071
+* https://gamesx.com/wiki/doku.php?id=controls:playstation_controller
+* https://github.com/SukkoPera/PsxNewLib
+* https://github.com/nandanhere/PiPyPS2
+* https://github.com/veroxzik/arduino-psx-controller
+* https://github.com/madsci1016/Arduino-PS2X
+
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-ps2controller.readthedocs.io/>`_.
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `circuitpython-ps2controller-1.0.0/README.rst` & `circuitpython-ps2controller-1.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-ps2controller/>`_.
 To install for current user:
 
 .. code-block:: shell
 
@@ -99,14 +97,29 @@
     while True:
         events = ps2.update()
         if events:
             print("events", events)
             print("sticks: L:", ps2.analog_left(), "R:", ps2.analog_right())
 
 
+References
+==========
+
+This library is a fairly direct port of `madsci1016/Arduino-PS2X <https://github.com/madsci1016/Arduino-PS2X>`_.
+
+Other resources that have been helpful:
+
+* https://store.curiousinventor.com/guides/PS2/
+* https://gist.github.com/scanlime/5042071
+* https://gamesx.com/wiki/doku.php?id=controls:playstation_controller
+* https://github.com/SukkoPera/PsxNewLib
+* https://github.com/nandanhere/PiPyPS2
+* https://github.com/veroxzik/arduino-psx-controller
+* https://github.com/madsci1016/Arduino-PS2X
+
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-ps2controller.readthedocs.io/>`_.
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/PKG-INFO` & `circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: circuitpython-ps2controller
-Version: 1.0.0
+Version: 1.1.0
 Summary: CircuitPython library to read Sony PS2 game controllers
 Author-email: Tod Kurt <tod@todbot.com>
 License: MIT
 Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
-Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,controller,gamepad,sony,dualshock
+Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
@@ -49,16 +49,14 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-ps2controller/>`_.
 To install for current user:
 
 .. code-block:: shell
 
@@ -117,14 +115,29 @@
     while True:
         events = ps2.update()
         if events:
             print("events", events)
             print("sticks: L:", ps2.analog_left(), "R:", ps2.analog_right())
 
 
+References
+==========
+
+This library is a fairly direct port of `madsci1016/Arduino-PS2X <https://github.com/madsci1016/Arduino-PS2X>`_.
+
+Other resources that have been helpful:
+
+* https://store.curiousinventor.com/guides/PS2/
+* https://gist.github.com/scanlime/5042071
+* https://gamesx.com/wiki/doku.php?id=controls:playstation_controller
+* https://github.com/SukkoPera/PsxNewLib
+* https://github.com/nandanhere/PiPyPS2
+* https://github.com/veroxzik/arduino-psx-controller
+* https://github.com/madsci1016/Arduino-PS2X
+
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-ps2controller.readthedocs.io/>`_.
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `circuitpython-ps2controller-1.0.0/circuitpython_ps2controller.egg-info/SOURCES.txt` & `circuitpython-ps2controller-1.1.0/circuitpython_ps2controller.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
-examples/ps2controller_simpletest.py
+examples/ps2controller_simpletest.py
+examples/ps2controller_usbkeys.py
```

### Comparing `circuitpython-ps2controller-1.0.0/docs/_static/favicon.ico` & `circuitpython-ps2controller-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/docs/conf.py` & `circuitpython-ps2controller-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/docs/index.rst` & `circuitpython-ps2controller-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.0.0/ps2controller.py` & `circuitpython-ps2controller-1.1.0/ps2controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Tod Kurt
 #
 # SPDX-License-Identifier: MIT
 """
 `ps2controller`
 ================================================================================
 
@@ -15,104 +14,120 @@
 --------------------
 
 **Hardware:**
 
 * Sony PS2 Controller or compatible gamepad
 
 
-
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 
 """
 
 # imports
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __repo__ = "https://github.com/todbot/CircuitPython_PS2Controller.git"
 
 
 from collections import namedtuple
 import time
+from micropython import const
 import digitalio
 
-# magic config strings sent to the controller
+# config strings sent to the controller
 _enter_config = (0x01, 0x43, 0x00, 0x01, 0x00)
 _set_mode = (0x01, 0x44, 0x00, 0x01, 0x03, 0x00, 0x00, 0x00, 0x00)
 _set_bytes_large = (0x01, 0x4F, 0x00, 0xFF, 0xFF, 0x03, 0x00, 0x00, 0x00)
 _exit_config = (0x01, 0x43, 0x00, 0x00, 0x5A, 0x5A, 0x5A, 0x5A, 0x5A)
-_enable_rumble = (0x01, 0x4D, 0x00, 0x00, 0x01)
+# _enable_rumble = (0x01, 0x4D, 0x00, 0x00, 0x01)
+_enable_rumble = (0x01, 0x4D, 0x00, 0x01, 0x01, 0xFF, 0xFF, 0xFF, 0xFF)
 _type_read = (0x01, 0x45, 0x00, 0x5A, 0x5A, 0x5A, 0x5A, 0x5A, 0x5A)
 
-_CTRL_BYTE_DELAY_MICROS = 4  # microseconds
-_CTRL_CLK_DELAY_MICROS = 5  # microseconds
+_CTRL_BYTE_DELAY_MICROS = const(4)  # microseconds
+_CTRL_CLK_DELAY_MICROS = const(5)  # microseconds
 
 
 def _delay_micros(usec):
     time.sleep(usec / 1_000_000)
 
 
 def _delay_millis(msec):
     time.sleep(msec / 1_000)
 
 
-ButtonEvent = namedtuple("ButtonEvent", ("number", "presssed", "released", "name"))
+#
+PS2ButtonEvent = namedtuple("PS2ButtonEvent", ("id", "pressed", "released", "name"))
+
+
+# pylint: disable-msg=(invalid-name, too-few-public-methods)
+class PS2Button:
+    """PS2 Button constants mapping button name to number"""
+
+    SELECT = 0
+    L3 = 1
+    R3 = 2
+    START = 3
+    UP = 4
+    RIGHT = 5
+    DOWN = 6
+    LEFT = 7
+    L2 = 8
+    R2 = 9
+    L1 = 10
+    R1 = 11
+    TRIANGLE = 12
+    CIRCLE = 13
+    CROSS = 14
+    SQUARE = 15
+
+    # fmt: off
+    button_to_analog_id = (-1, -1, -1, -1, 11, 9, 12, 10, 19, 20, 17, 18, 13, 14, 15, 16)
+
+    names = ("SELECT", "L3", "R3", "START", "UP", "RIGHT", "DOWN", "LEFT",
+             "L2", "R2", "L1", "R1", "TRIANGLE", "CIRCLE", "CROSS", "SQUARE")
+    # fmt: on
 
-button_names = (
-    "SELECT",
-    "L3",
-    "R3",
-    "START",
-    "UP",
-    "RIGHT",
-    "DOWN",
-    "LEFT",
-    "L2",
-    "R2",
-    "L1",
-    "R1",
-    "TRIANGLE",
-    "CIRCLE",
-    "CROSS",
-    "SQUARE",
-)
 
+# pylint: enable-msg=(invalid-name, too-few-public-methods)
 
-class PS2Controller:
+
+class PS2Controller:  # pylint: disable=too-many-instance-attributes
     """
     Driver to read and control a Sony PS2 controller
 
     :param ~microcontroller.Pin clk: PS2 clock pin (blue wire)
     :param ~microcontroller.Pin cmd: PS2 command pin (orange wire)
     :param ~microcontroller.Pin att: PS2 attention pin (yellow wire)
     :param ~microcontroller.Pin dat: PS2 data pin (brown wire)
-    :param bool enable_pressue: True to enable reading analog button pressure
-    :param bool enable_rumbling: True to enable controlling rumble motors
+    :param bool enable_pressure: True to enable reading analog button pressure
+    :param bool enable_rumble: True to enable controlling rumble motors
                                  (needs extra voltage and current)
     """
 
     def __init__(
-        self, clk, cmd, att, dat, enable_pressure=False, enable_rumbling=False
+        self, clk, cmd, att, dat, enable_pressure=False, enable_rumble=False
     ):  # pylint: disable=(too-many-arguments)
         self.clk_pin = digitalio.DigitalInOut(clk)
         self.att_pin = digitalio.DigitalInOut(att)
         self.cmd_pin = digitalio.DigitalInOut(cmd)
         self.dat_pin = digitalio.DigitalInOut(dat)
         self.clk_pin.switch_to_output(value=False)
         self.att_pin.switch_to_output(value=False)
         self.cmd_pin.switch_to_output(value=False)
         self.dat_pin.switch_to_input(pull=digitalio.Pull.UP)
 
         self.ps2data = [0] * 21  # holds raw data from controller
 
         self.enable_pressure = enable_pressure
-        self.enable_rumbling = enable_rumbling
+        self.enable_rumble = enable_rumble
+        self.rumble_motors = [0, 0]  # left, right?
 
         self._read_delay_millis = 1
 
         self.cmd_pin.value = True  # CMD_SET()
         self.clk_pin.value = True  # CLK_SET()
 
         self._buttons = 0
@@ -120,40 +135,60 @@
 
         if not self._config_gamepad():
             print("could not configure controller")
             return  # TODO: throw exception?
         self.update()  # get initial values
 
     def update(self):
-        """Read the controller and return a list of ButtonEvents"""
+        """Read the controller and return a list of PS2ButtonEvents"""
         self._read_gamepad()
 
         self._last_buttons = self._buttons
         self._buttons = self.ps2data[4] << 8 | self.ps2data[3]
 
         events = []
         for i in range(16):
             if self._last_buttons & (1 << i) != self._buttons & (1 << i):
                 pressed = (self._buttons & (1 << i)) == 0
                 released = not pressed
-                events.append(ButtonEvent(i, pressed, released, button_names[i]))
+                events.append(PS2ButtonEvent(i, pressed, released, PS2Button.names[i]))
         return events
 
     def buttons(self):
         """Return a 16-bit bitfield of the state of all buttons"""
         return self._buttons
 
+    def button(self, button_id):
+        """Return True if button is currently pressed
+        :param int button_id: 0-15 id number from PS2ButtonEvent.id or PS2Button.*
+        """
+        return (self._buttons & (1 << button_id)) == 0
+
+    def analog_button(self, button_id):
+        """Return analog pressure value for button
+        :param int button_id 0-15 id number PS2ButtonEvent.id or PS2Button.*
+        """
+        return self.ps2data[PS2Button.button_to_analog_id[button_id]] / 255
+
     def analog_right(self):
         """Return a (x,y) tuple of the right analog stick"""
         return (self.ps2data[5], self.ps2data[6])
 
     def analog_left(self):
         """Return a (x,y) tuple of the left analog stick"""
         return (self.ps2data[7], self.ps2data[8])
 
+    def set_rumble(self, motor_num, strength):
+        """
+        Set rumble motor strength. Set on next update() call.
+        :param int motor_num: whiich motor to affect: 0, 1
+        :param float stregnth amount of rumble, 0-1
+        """
+        self.rumble_motors[motor_num] = min(max(strength, 0), 1)
+
     def _config_gamepad(self):
         # "new error checking. First, read gamepad a few times to see if it's talking"
         self._read_gamepad()
         self._read_gamepad()
 
         if self.ps2data[1] not in (0x41, 0x42, 0x73, 0x79):
             print("PS2Controller mode not matched or no controller found")
@@ -176,16 +211,16 @@
                 temp[i] = self._gamepad_shiftinout(_type_read[i])
 
             self.att_pin.value = False  # "HIGH disable joytick" (raise CS, that is)
 
             self.controller_type = temp[3]
 
             self._send_command_string(_set_mode)
-            # if self.enable_rumble:
-            #  self._send_command_string(_enable_rumble)
+            if self.enable_rumble:
+                self._send_command_string(_enable_rumble)
             if self.enable_pressure:
                 self._send_command_string(_set_bytes_large)
             self._send_command_string(_exit_config)
 
             self._read_gamepad()
 
             if self.enable_pressure:
@@ -202,16 +237,16 @@
 
         # couldn't get controller to do what we wanted
         print("PS2Controller: Controller not accepting commands.")
         print("\tMode still at %02x" % self.ps2data[1])
         return False
 
     def _read_gamepad(self):  # motor1=False, motor2=False):
-        motor1_val = 0  # tbd
-        motor2_val = 0  # tbd
+        motor1_val = int(self.rumble_motors[0] * 255)
+        motor2_val = int(self.rumble_motors[1] * 255)
 
         dword1 = (0x01, 0x42, 0, motor1_val, motor2_val, 0, 0, 0, 0)  # 9 values
         dword2 = (0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0)  # 12 values, all zero
 
         retry_count = 5
         for _ in range(retry_count):
             self.cmd_pin.value = True
@@ -221,15 +256,15 @@
             _delay_micros(_CTRL_BYTE_DELAY_MICROS)
 
             # "Send the command to send button and joystick data"
             for i in range(9):
                 self.ps2data[i] = self._gamepad_shiftinout(dword1[i])
 
             # "if controller is in full data return mode, get the rest of data"
-            if self.ps2data[1] == 0x79:
+            if self.ps2data[1] == 0x79:  # 0x79 == Dual Shock 2
                 for i in range(12):
                     self.ps2data[9 + i] = self._gamepad_shiftinout(dword2[i])
 
             self.att_pin.value = True  # "HIGH disable joystick"
 
             # "Check to see if we received valid data or not."
             # "We should be in analog mode for our data to be valid (analog == 0x7_)"
@@ -241,16 +276,16 @@
             self._reconfig_gamepad()
             # "try to get back into Analog mode."
             _delay_micros(self._read_delay_millis)
 
     def _reconfig_gamepad(self):
         self._send_command_string(_enter_config)
         self._send_command_string(_set_mode)
-        # if enable_rumble:
-        # self._send_command_string(_enable_rumble)
+        if self.enable_rumble:
+            self._send_command_string(_enable_rumble)
         if self.enable_pressure:
             self._send_command_string(_set_bytes_large)
         self._send_command_string(_exit_config)
 
     def _send_command_string(self, cmdstr):
         self.att_pin.value = False  # "low enable joystick"
         _delay_micros(_CTRL_BYTE_DELAY_MICROS)
```

### Comparing `circuitpython-ps2controller-1.0.0/pyproject.toml` & `circuitpython-ps2controller-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,28 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-ps2controller"
 description = "CircuitPython library to read Sony PS2 game controllers"
-version = "1.0.0"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Tod Kurt", email = "tod@todbot.com"}
 ]
 urls = {Homepage = "https://github.com/todbot/CircuitPython_PS2Controller"}
 keywords = [
     "adafruit",
     "blinka",
     "circuitpython",
     "micropython",
     "ps2controller",
     "ps2",
+    "psx",
     "controller",
     "gamepad",
     "sony",
     "dualshock",
 ]
 license = {text = "MIT"}
 classifiers = [
```

