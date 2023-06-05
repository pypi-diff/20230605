# Comparing `tmp/pyBiocFileCache-0.2.1.tar.gz` & `tmp/pyBiocFileCache-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBiocFileCache-0.2.1.tar", last modified: Mon Mar  6 22:46:11 2023, max compression
+gzip compressed data, was "pyBiocFileCache-0.2.2.tar", last modified: Mon Jun  5 17:43:07 2023, max compression
```

## Comparing `pyBiocFileCache-0.2.1.tar` & `pyBiocFileCache-0.2.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.419057 pyBiocFileCache-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.423057 pyBiocFileCache-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-06 22:46:11.431057 pyBiocFileCache-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.423057 pyBiocFileCache-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-06 22:46:11.000000 pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-06 22:46:11.000000 pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 22:46:11.000000 pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 22:45:30.000000 pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-06 22:46:11.000000 pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-06 22:46:11.000000 pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/src/pybiocfilecache/
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/src/pybiocfilecache/BiocFileCache.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/src/pybiocfilecache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/src/pybiocfilecache/db/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/src/pybiocfilecache/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/src/pybiocfilecache/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/src/pybiocfilecache/db/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/src/pybiocfilecache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:46:11.427057 pyBiocFileCache-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/tests/data/test1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/tests/data/test2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-06 22:45:22.000000 pyBiocFileCache-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.145129 pyBiocFileCache-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.153129 pyBiocFileCache-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.157129 pyBiocFileCache-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.157129 pyBiocFileCache-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.145129 pyBiocFileCache-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.157129 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:42:24.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.161129 pyBiocFileCache-0.2.2/src/pybiocfilecache/
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/BiocFileCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.161129 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/temp.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.161129 pyBiocFileCache-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/data/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/data/test2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tox.ini
```

### Comparing `pyBiocFileCache-0.2.1/.coveragerc` & `pyBiocFileCache-0.2.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/.github/workflows/pypi-publish.yml` & `pyBiocFileCache-0.2.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/.github/workflows/pypi-test.yml` & `pyBiocFileCache-0.2.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/.gitignore` & `pyBiocFileCache-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/CONTRIBUTING.rst` & `pyBiocFileCache-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/LICENSE.txt` & `pyBiocFileCache-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/PKG-INFO` & `pyBiocFileCache-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.2.1
+Version: 0.2.2
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `pyBiocFileCache-0.2.1/README.md` & `pyBiocFileCache-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/docs/Makefile` & `pyBiocFileCache-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/docs/conf.py` & `pyBiocFileCache-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/docs/index.md` & `pyBiocFileCache-0.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/docs/readme.md` & `pyBiocFileCache-0.2.2/docs/readme.md`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/setup.cfg` & `pyBiocFileCache-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/setup.py` & `pyBiocFileCache-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/PKG-INFO` & `pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.2.1
+Version: 0.2.2
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `pyBiocFileCache-0.2.1/src/pyBiocFileCache.egg-info/SOURCES.txt` & `pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 CHANGELOG.md
 CONTRIBUTING.rst
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+temp.txt
 tox.ini
 .github/workflows/pypi-publish.yml
 .github/workflows/pypi-test.yml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
 docs/conf.py
@@ -26,14 +27,15 @@
 src/pyBiocFileCache.egg-info/SOURCES.txt
 src/pyBiocFileCache.egg-info/dependency_links.txt
 src/pyBiocFileCache.egg-info/not-zip-safe
 src/pyBiocFileCache.egg-info/requires.txt
 src/pyBiocFileCache.egg-info/top_level.txt
 src/pybiocfilecache/BiocFileCache.py
 src/pybiocfilecache/__init__.py
+src/pybiocfilecache/_exceptions.py
 src/pybiocfilecache/utils.py
 src/pybiocfilecache/db/Base.py
 src/pybiocfilecache/db/__init__.py
 src/pybiocfilecache/db/schema.py
 tests/conftest.py
 tests/test_cache.py
 tests/data/test1.txt
```

### Comparing `pyBiocFileCache-0.2.1/src/pybiocfilecache/db/Base.py` & `pyBiocFileCache-0.2.2/src/pybiocfilecache/db/Base.py`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/src/pybiocfilecache/db/schema.py` & `pyBiocFileCache-0.2.2/src/pybiocfilecache/db/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from sqlalchemy import Column, Integer, String, DateTime
+from sqlalchemy import Column, DateTime, Integer, String
 from sqlalchemy.sql import func
+
 from .Base import Base
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
```

### Comparing `pyBiocFileCache-0.2.1/src/pybiocfilecache/utils.py` & `pyBiocFileCache-0.2.2/src/pybiocfilecache/utils.py`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/tests/test_cache.py` & `pyBiocFileCache-0.2.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.1/tox.ini` & `pyBiocFileCache-0.2.2/tox.ini`

 * *Files identical despite different names*

