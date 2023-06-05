# Comparing `tmp/thunder-ase-0.2.4.tar.gz` & `tmp/thunder-ase-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.2.4.tar", last modified: Sun Jun  4 14:14:36 2023, max compression
+gzip compressed data, was "thunder-ase-0.3.1.tar", last modified: Mon Jun  5 05:04:06 2023, max compression
```

## Comparing `thunder-ase-0.2.4.tar` & `thunder-ase-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:14:36.150967 thunder-ase-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-04 14:14:36.150967 thunder-ase-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-04 14:14:23.000000 thunder-ase-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-04 14:14:23.000000 thunder-ase-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 14:14:36.150967 thunder-ase-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 14:14:23.000000 thunder-ase-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:14:36.150967 thunder-ase-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-04 14:14:23.000000 thunder-ase-0.2.4/tests/test_Si_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:14:36.150967 thunder-ase-0.2.4/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:14:23.000000 thunder-ase-0.2.4/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30732 2023-06-04 14:14:23.000000 thunder-ase-0.2.4/thunder_ase/fireball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:14:36.150967 thunder-ase-0.2.4/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-04 14:14:36.000000 thunder-ase-0.2.4/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-04 14:14:36.000000 thunder-ase-0.2.4/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 14:14:36.000000 thunder-ase-0.2.4/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 14:14:36.000000 thunder-ase-0.2.4/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 14:14:36.000000 thunder-ase-0.2.4/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/tests/test_Si_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30732 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/thunder_ase/fireball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.2.4/PKG-INFO` & `thunder-ase-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.2.4
+Version: 0.3.1
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,13 +34,12 @@
 
 * v0.1: run basic fireball calculation and read basic result from it.
   * v0.1.1: jupyter-notebook for examples
   * v0.1.2: multiple atoms for one calculator
   * v0.1.3: read fireball input to construct calculator
 * v0.2: band structure calculation.
   * v0.2.1: DOS calculation.
-  * v0.2.2: fit basis to gaussian.
-  * v0.2.3: write basis to mwfn.
-  * v0.2.4: interface to multiwfn.
-* v0.3: MD calculation.
-* v0.4: Fdata management.
-* v0.5: interactive running.
+* v0.3.1: fit basis to gaussian, write orbitals to mwfn.
+  * v0.3.2: interface to multiwfn.
+* v0.4: MD calculation.
+* v0.5: Fdata management.
+* v0.6: interactive running.
```

### Comparing `thunder-ase-0.2.4/README.md` & `thunder-ase-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,13 +21,12 @@
 
 * v0.1: run basic fireball calculation and read basic result from it.
   * v0.1.1: jupyter-notebook for examples
   * v0.1.2: multiple atoms for one calculator
   * v0.1.3: read fireball input to construct calculator
 * v0.2: band structure calculation.
   * v0.2.1: DOS calculation.
-  * v0.2.2: fit basis to gaussian.
-  * v0.2.3: write basis to mwfn.
-  * v0.2.4: interface to multiwfn.
-* v0.3: MD calculation.
-* v0.4: Fdata management.
-* v0.5: interactive running.
+* v0.3.1: fit basis to gaussian, write orbitals to mwfn.
+  * v0.3.2: interface to multiwfn.
+* v0.4: MD calculation.
+* v0.5: Fdata management.
+* v0.6: interactive running.
```

### Comparing `thunder-ase-0.2.4/pyproject.toml` & `thunder-ase-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.2.4"
+version = "0.3.1"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thunder-ase-0.2.4/tests/test_Si_lightning.py` & `thunder-ase-0.3.1/tests/test_Si_lightning.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.2.4/thunder_ase/fireball.py` & `thunder-ase-0.3.1/thunder_ase/fireball.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.2.4/thunder_ase.egg-info/PKG-INFO` & `thunder-ase-0.3.1/thunder_ase.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.2.4
+Version: 0.3.1
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,13 +34,12 @@
 
 * v0.1: run basic fireball calculation and read basic result from it.
   * v0.1.1: jupyter-notebook for examples
   * v0.1.2: multiple atoms for one calculator
   * v0.1.3: read fireball input to construct calculator
 * v0.2: band structure calculation.
   * v0.2.1: DOS calculation.
-  * v0.2.2: fit basis to gaussian.
-  * v0.2.3: write basis to mwfn.
-  * v0.2.4: interface to multiwfn.
-* v0.3: MD calculation.
-* v0.4: Fdata management.
-* v0.5: interactive running.
+* v0.3.1: fit basis to gaussian, write orbitals to mwfn.
+  * v0.3.2: interface to multiwfn.
+* v0.4: MD calculation.
+* v0.5: Fdata management.
+* v0.6: interactive running.
```

