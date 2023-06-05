# Comparing `tmp/autosar-e2e-0.2.1.tar.gz` & `tmp/autosar-e2e-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosar-e2e-0.2.1.tar", last modified: Fri Sep 23 19:24:18 2022, max compression
+gzip compressed data, was "autosar-e2e-0.3.0.tar", last modified: Mon Jun  5 15:27:53 2023, max compression
```

## Comparing `autosar-e2e-0.2.1.tar` & `autosar-e2e-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:24:18.600890 autosar-e2e-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-09-23 19:24:18.600890 autosar-e2e-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-23 19:24:18.600890 autosar-e2e-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:24:18.600890 autosar-e2e-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:24:18.600890 autosar-e2e-0.2.1/src/autosar_e2e.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-09-23 19:24:18.000000 autosar-e2e-0.2.1/src/autosar_e2e.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-23 19:24:18.000000 autosar-e2e-0.2.1/src/autosar_e2e.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 19:24:18.000000 autosar-e2e-0.2.1/src/autosar_e2e.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-23 19:24:18.000000 autosar-e2e-0.2.1/src/autosar_e2e.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:24:18.600890 autosar-e2e-0.2.1/src/e2e/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/src/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12752 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/src/e2e/crc.c
--rw-r--r--   0 runner    (1001) docker     (121)    25095 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/src/e2e/crc.h
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/src/e2e/crc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5718 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/src/e2e/p02.c
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/src/e2e/p02.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/src/e2e/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:24:18.600890 autosar-e2e-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     9319 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/test/test_crc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-09-23 19:24:11.000000 autosar-e2e-0.2.1/test/test_p02.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.560941 autosar-e2e-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:27:53.560941 autosar-e2e-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.552940 autosar-e2e-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/src/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/crc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25095 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/crc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/crc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p01.c
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p01.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p02.c
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p02.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/test/test_crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/test/test_p01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/test/test_p02.py
```

### Comparing `autosar-e2e-0.2.1/LICENSE.txt` & `autosar-e2e-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.2.1/PKG-INFO` & `autosar-e2e-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 Metadata-Version: 2.1
 Name: autosar-e2e
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python implementation of the AUTOSAR E2E Protocol
 Author-email: Artur Drogunow <artur.drogunow@zf.com>
 License: MIT
-Project-URL: Documentation, https://github.com/zariiii9003/autosar-e2e#readme
+Project-URL: Documentation, https://autosar-e2e.readthedocs.io/en/latest
 Project-URL: Issues, https://github.com/zariiii9003/autosar-e2e/issues
 Project-URL: Source, https://github.com/zariiii9003/autosar-e2e
 Project-URL: Homepage, https://github.com/zariiii9003/autosar-e2e
 Keywords: AUTOSAR,E2E,automotive
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # autosar-e2e
 
 [![PyPI - Version](https://img.shields.io/pypi/v/autosar-e2e.svg)](https://pypi.org/project/autosar-e2e)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/autosar-e2e.svg)](https://pypi.org/project/autosar-e2e)
+[![Documentation Status](https://readthedocs.org/projects/autosar-e2e/badge/?version=latest)](https://autosar-e2e.readthedocs.io/en/latest/?badge=latest)
+
+The documentation is available [here](https://autosar-e2e.readthedocs.io/en/latest/).
 
 -----
 
 **Table of Contents**
 
 - [Description](#description)
 - [Installation](#installation)
@@ -33,16 +40,17 @@
 - [Build](#build)
 - [License](#license)
 
 ## Description
 
 This library provides fast C implementations of the E2E CRC algorithms and E2E profiles. 
 
-Currently all relevant CRC algorithms are available in module `e2e.crc`
-but only E2E profile 2 is available. If you provide example data for the other profiles i would try to implement them, too.
+Currently, all relevant CRC algorithms are available in module `e2e.crc`
+but only E2E profiles 1 and 2 are available. 
+If you provide example data for the other profiles I would try to implement them, too.
 
 ## Installation
 
 ```console
 pip install autosar-e2e
 ```
 
@@ -66,21 +74,22 @@
 # check CRC
 crc_correct: bool = e2e.p02.e2e_p02_check(data, length, data_id_list)
 ```
 
 ## Test
 
 ```console
-pip install tox
-tox
+pip install pipx
+pipx run tox
 ```
 
 ## Build
 
 ```console
-pip install build
-python -m build .
+pip install pipx
+pipx run build
+pipx run twine check dist/*
 ```
 
 ## License
 
 `autosar-e2e` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `autosar-e2e-0.2.1/README.md` & `autosar-e2e-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # autosar-e2e
 
 [![PyPI - Version](https://img.shields.io/pypi/v/autosar-e2e.svg)](https://pypi.org/project/autosar-e2e)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/autosar-e2e.svg)](https://pypi.org/project/autosar-e2e)
+[![Documentation Status](https://readthedocs.org/projects/autosar-e2e/badge/?version=latest)](https://autosar-e2e.readthedocs.io/en/latest/?badge=latest)
+
+The documentation is available [here](https://autosar-e2e.readthedocs.io/en/latest/).
 
 -----
 
 **Table of Contents**
 
 - [Description](#description)
 - [Installation](#installation)
@@ -14,16 +17,17 @@
 - [Build](#build)
 - [License](#license)
 
 ## Description
 
 This library provides fast C implementations of the E2E CRC algorithms and E2E profiles. 
 
-Currently all relevant CRC algorithms are available in module `e2e.crc`
-but only E2E profile 2 is available. If you provide example data for the other profiles i would try to implement them, too.
+Currently, all relevant CRC algorithms are available in module `e2e.crc`
+but only E2E profiles 1 and 2 are available. 
+If you provide example data for the other profiles I would try to implement them, too.
 
 ## Installation
 
 ```console
 pip install autosar-e2e
 ```
 
@@ -47,21 +51,22 @@
 # check CRC
 crc_correct: bool = e2e.p02.e2e_p02_check(data, length, data_id_list)
 ```
 
 ## Test
 
 ```console
-pip install tox
-tox
+pip install pipx
+pipx run tox
 ```
 
 ## Build
 
 ```console
-pip install build
-python -m build .
+pip install pipx
+pipx run build
+pipx run twine check dist/*
 ```
 
 ## License
 
 `autosar-e2e` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `autosar-e2e-0.2.1/pyproject.toml` & `autosar-e2e-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -15,27 +15,37 @@
 ]
 authors = [
   { name = "Artur Drogunow", email = "artur.drogunow@zf.com" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = []
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://github.com/zariiii9003/autosar-e2e#readme"
+Documentation = "https://autosar-e2e.readthedocs.io/en/latest"
 Issues = "https://github.com/zariiii9003/autosar-e2e/issues"
 Source = "https://github.com/zariiii9003/autosar-e2e"
 Homepage = "https://github.com/zariiii9003/autosar-e2e"
 
 [tool.setuptools.dynamic]
 version = {attr = "e2e.__version__"}
 
+[tool.setuptools.package-data]
+"*" = [
+  "**/py.typed",
+  "**.pyi",
+]
+
 [tool.cibuildwheel]
 test-requires = "pytest"
 test-command = "pytest {project}/test"
 build-frontend = "build"
 skip = "pp*"
```

### Comparing `autosar-e2e-0.2.1/setup.py` & `autosar-e2e-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,31 @@
 pkg_dir = Path("src") / import_pkg_name
 
 crc_module = Extension(
     f"{import_pkg_name}.crc",
     sources=[str(pkg_dir / "crc.c")],
     include_dirs=[pkg_dir.as_posix()],
 )
-
+p01_module = Extension(
+    f"{import_pkg_name}.p01",
+    sources=[
+        str(pkg_dir / "p01.c"),
+        str(pkg_dir / "crc.c"),
+    ],
+    include_dirs=[pkg_dir.as_posix()],
+)
 p02_module = Extension(
     f"{import_pkg_name}.p02",
     sources=[
         str(pkg_dir / "p02.c"),
         str(pkg_dir / "crc.c"),
     ],
     include_dirs=[pkg_dir.as_posix()],
 )
 
 setup(
     ext_modules=[
         crc_module,
+        p01_module,
         p02_module,
     ],
 )
```

### Comparing `autosar-e2e-0.2.1/src/autosar_e2e.egg-info/PKG-INFO` & `autosar-e2e-0.3.0/src/autosar_e2e.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 Metadata-Version: 2.1
 Name: autosar-e2e
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python implementation of the AUTOSAR E2E Protocol
 Author-email: Artur Drogunow <artur.drogunow@zf.com>
 License: MIT
-Project-URL: Documentation, https://github.com/zariiii9003/autosar-e2e#readme
+Project-URL: Documentation, https://autosar-e2e.readthedocs.io/en/latest
 Project-URL: Issues, https://github.com/zariiii9003/autosar-e2e/issues
 Project-URL: Source, https://github.com/zariiii9003/autosar-e2e
 Project-URL: Homepage, https://github.com/zariiii9003/autosar-e2e
 Keywords: AUTOSAR,E2E,automotive
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # autosar-e2e
 
 [![PyPI - Version](https://img.shields.io/pypi/v/autosar-e2e.svg)](https://pypi.org/project/autosar-e2e)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/autosar-e2e.svg)](https://pypi.org/project/autosar-e2e)
+[![Documentation Status](https://readthedocs.org/projects/autosar-e2e/badge/?version=latest)](https://autosar-e2e.readthedocs.io/en/latest/?badge=latest)
+
+The documentation is available [here](https://autosar-e2e.readthedocs.io/en/latest/).
 
 -----
 
 **Table of Contents**
 
 - [Description](#description)
 - [Installation](#installation)
@@ -33,16 +40,17 @@
 - [Build](#build)
 - [License](#license)
 
 ## Description
 
 This library provides fast C implementations of the E2E CRC algorithms and E2E profiles. 
 
-Currently all relevant CRC algorithms are available in module `e2e.crc`
-but only E2E profile 2 is available. If you provide example data for the other profiles i would try to implement them, too.
+Currently, all relevant CRC algorithms are available in module `e2e.crc`
+but only E2E profiles 1 and 2 are available. 
+If you provide example data for the other profiles I would try to implement them, too.
 
 ## Installation
 
 ```console
 pip install autosar-e2e
 ```
 
@@ -66,21 +74,22 @@
 # check CRC
 crc_correct: bool = e2e.p02.e2e_p02_check(data, length, data_id_list)
 ```
 
 ## Test
 
 ```console
-pip install tox
-tox
+pip install pipx
+pipx run tox
 ```
 
 ## Build
 
 ```console
-pip install build
-python -m build .
+pip install pipx
+pipx run build
+pipx run twine check dist/*
 ```
 
 ## License
 
 `autosar-e2e` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `autosar-e2e-0.2.1/src/e2e/crc.h` & `autosar-e2e-0.3.0/src/e2e/crc.h`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.2.1/src/e2e/crc.pyi` & `autosar-e2e-0.3.0/src/e2e/crc.pyi`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.2.1/test/test_crc.py` & `autosar-e2e-0.3.0/test/test_crc.py`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.2.1/test/test_p02.py` & `autosar-e2e-0.3.0/test/test_p02.py`

 * *Files identical despite different names*

