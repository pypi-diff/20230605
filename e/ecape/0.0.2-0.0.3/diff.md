# Comparing `tmp/ecape-0.0.2.tar.gz` & `tmp/ecape-0.0.3.tar.gz`

## Comparing `ecape-0.0.2.tar` & `ecape-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.2/src/ecape_py/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.2/src/ecape_py/__init__.py
--rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 ecape-0.0.2/src/ecape_py/ecape.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.2/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 ecape-0.0.2/README.md
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ecape-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 ecape-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.3/src/ecape_py/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.3/src/ecape_py/__init__.py
+-rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 ecape-0.0.3/src/ecape_py/ecape.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 ecape-0.0.3/README.md
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 ecape-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 ecape-0.0.3/PKG-INFO
```

### Comparing `ecape-0.0.2/src/ecape_py/ecape.py` & `ecape-0.0.3/src/ecape_py/ecape.py`

 * *Files identical despite different names*

### Comparing `ecape-0.0.2/LICENSE.txt` & `ecape-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.2/README.md` & `ecape-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ecape-0.0.2/pyproject.toml` & `ecape-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/docs", "/tests"]
 
 [tool.hatch.build.targets.wheel]
-exclude = ["src/ecape_py"]
+packages = ["src/ecape_py"]
 
 [project]
 name = "ecape"
 dynamic = ["version"]
 description = 'Calculate the entraining CAPE (ECAPE) of a parcel.'
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ecape-0.0.2/PKG-INFO` & `ecape-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.2
+Version: 0.0.3
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

