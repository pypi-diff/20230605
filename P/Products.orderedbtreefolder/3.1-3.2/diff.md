# Comparing `tmp/Products.orderedbtreefolder-3.1.tar.gz` & `tmp/Products.orderedbtreefolder-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.orderedbtreefolder-3.1.tar", last modified: Tue Oct 19 09:27:09 2021, max compression
+gzip compressed data, was "Products.orderedbtreefolder-3.2.tar", last modified: Mon Jun  5 08:01:37 2023, max compression
```

## Comparing `Products.orderedbtreefolder-3.1.tar` & `Products.orderedbtreefolder-3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/
--rw-r--r--   0 mac        (513) staff       (20)      387 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)      167 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/.isort.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1811 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/.pre-commit-config.yaml
--rw-r--r--   0 mac        (513) staff       (20)     2152 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)    35147 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      384 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     5604 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      438 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      501 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)       23 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/pytest.ini
--rw-r--r--   0 mac        (513) staff       (20)       67 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2136 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products/
--rw-r--r--   0 mac        (513) staff       (20)       56 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/
--rw-r--r--   0 mac        (513) staff       (20)    12279 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/LICENSE.GPL
--rw-r--r--   0 mac        (513) staff       (20)      724 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)     1127 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      347 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/dtml/
--rw-r--r--   0 mac        (513) staff       (20)     6655 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/dtml/orderedBTFolderMain.dtml
--rw-r--r--   0 mac        (513) staff       (20)     1550 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/dtml/orderedFolderAdd.dtml
--rw-r--r--   0 mac        (513) staff       (20)      179 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/orderedbtreefolder.gif
--rw-r--r--   0 mac        (513) staff       (20)    10261 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/orderedbtreefolder.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/tests/
--rw-r--r--   0 mac        (513) staff       (20)       22 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    10542 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/tests/test_orderedbtreefolder.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     5604 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1081 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      135 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2021-10-19 09:27:09.000000 Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)      425 2021-10-19 09:27:08.000000 Products.orderedbtreefolder-3.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-05 08:01:37.727985 Products.orderedbtreefolder-3.2/
+-rw-r--r--   0 mac        (513) staff       (20)      387 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/.coveragerc
+-rw-r--r--   0 mac        (513) staff       (20)      167 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/.isort.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     1811 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/.pre-commit-config.yaml
+-rw-r--r--   0 mac        (513) staff       (20)     2252 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)    35147 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      384 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     4489 2023-06-05 08:01:37.728119 Products.orderedbtreefolder-3.2/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      438 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      501 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)       23 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/pytest.ini
+-rw-r--r--   0 mac        (513) staff       (20)       67 2023-06-05 08:01:37.728559 Products.orderedbtreefolder-3.2/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2240 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-05 08:01:37.716312 Products.orderedbtreefolder-3.2/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-05 08:01:37.721339 Products.orderedbtreefolder-3.2/src/Products/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-05 08:01:37.726046 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/
+-rw-r--r--   0 mac        (513) staff       (20)    12279 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/LICENSE.GPL
+-rw-r--r--   0 mac        (513) staff       (20)      724 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1127 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      347 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-05 08:01:37.726869 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/dtml/
+-rw-r--r--   0 mac        (513) staff       (20)     6655 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/dtml/orderedBTFolderMain.dtml
+-rw-r--r--   0 mac        (513) staff       (20)     1550 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/dtml/orderedFolderAdd.dtml
+-rw-r--r--   0 mac        (513) staff       (20)      179 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/orderedbtreefolder.gif
+-rw-r--r--   0 mac        (513) staff       (20)    10261 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/orderedbtreefolder.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-05 08:01:37.727647 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       22 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    10542 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/tests/test_orderedbtreefolder.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-05 08:01:37.723646 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     4489 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1081 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        9 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      135 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        9 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)      425 2023-06-05 08:01:37.000000 Products.orderedbtreefolder-3.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Products.orderedbtreefolder-3.1/.pre-commit-config.yaml` & `Products.orderedbtreefolder-3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/CHANGES.rst` & `Products.orderedbtreefolder-3.2/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 Changes
 =======
 
+3.2 (2023-06-05)
+================
+
+- Add support for Python 3.11.
+
+- Add support for Python 3.10.
+
+
 3.1 (2021-10-19)
 ================
 
 - Pin to ``setuptools < 52`` to work around and incompatibility with
   ``zc.buildout`` in that version.
 
 - Add support for Python 3.9.
```

### Comparing `Products.orderedbtreefolder-3.1/LICENSE.txt` & `Products.orderedbtreefolder-3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/setup.py` & `Products.orderedbtreefolder-3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read() + '\n\n'
 
 
-version = '3.1'
+version = '3.2'
 
 long_description = (
     '.. contents ::\n\n' +
     read('CHANGES.rst') +
     read('src', 'Products', 'orderedbtreefolder', 'README.rst')
 )
 
@@ -28,14 +28,16 @@
       classifiers=[
           "Framework :: Zope :: 4",
           "Framework :: Zope :: 5",
           "Programming Language :: Python :: 3",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
+          "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3.11",
           "Programming Language :: Python :: Implementation :: CPython",
           "Topic :: Software Development :: Libraries :: Python Modules",
           "Intended Audience :: Developers",
           "License :: OSI Approved :: GNU General Public License (GPL)",
           "Development Status :: 5 - Production/Stable",
       ],
       keywords='union.cms zope python content',
```

### Comparing `Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/LICENSE.GPL` & `Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/LICENSE.txt` & `Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/README.rst` & `Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/README.rst`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/dtml/orderedBTFolderMain.dtml` & `Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/dtml/orderedBTFolderMain.dtml`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/dtml/orderedFolderAdd.dtml` & `Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/dtml/orderedFolderAdd.dtml`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/orderedbtreefolder.py` & `Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/orderedbtreefolder.py`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/src/Products/orderedbtreefolder/tests/test_orderedbtreefolder.py` & `Products.orderedbtreefolder-3.2/src/Products/orderedbtreefolder/tests/test_orderedbtreefolder.py`

 * *Files identical despite different names*

### Comparing `Products.orderedbtreefolder-3.1/src/Products.orderedbtreefolder.egg-info/SOURCES.txt` & `Products.orderedbtreefolder-3.2/src/Products.orderedbtreefolder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

