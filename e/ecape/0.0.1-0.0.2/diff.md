# Comparing `tmp/ecape-0.0.1.tar.gz` & `tmp/ecape-0.0.2.tar.gz`

## Comparing `ecape-0.0.1.tar` & `ecape-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,8 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.1/src/ecape_py/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.1/src/ecape_py/__init__.py
--rw-r--r--   0        0        0    12892 2020-02-02 00:00:00.000000 ecape-0.0.1/src/ecape_py/ecape.py
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 ecape-0.0.1/tests/.coverage
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 ecape-0.0.1/tests/intarg.txt
--rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 ecape-0.0.1/tests/mseo.txt
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 ecape-0.0.1/tests/ncape.txt
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 ecape-0.0.1/tests/sounding.txt
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 ecape-0.0.1/tests/test_ecape.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.1/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 ecape-0.0.1/README.md
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 ecape-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 ecape-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.2/src/ecape_py/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.2/src/ecape_py/__init__.py
+-rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 ecape-0.0.2/src/ecape_py/ecape.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 ecape-0.0.2/README.md
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ecape-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 ecape-0.0.2/PKG-INFO
```

### Comparing `ecape-0.0.1/src/ecape_py/ecape.py` & `ecape-0.0.2/src/ecape_py/ecape.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,7 +371,10 @@
     sr_wind = calc_sr_wind(pressure, u_wind, v_wind, height)
 
     # calculate the entraining cape (ecape)
     psi = calc_psi(el_z)
     ecape_a = calc_ecape_a(sr_wind, psi, ncape, cape)
 
     return ecape_a
+
+if __name__ == "__main__":
+    pass
```

### Comparing `ecape-0.0.1/LICENSE.txt` & `ecape-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.1/README.md` & `ecape-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ```console
 pip install ecape
 ```
 
 Documentation, Source
 -------------
 https://github.com/citylikeamradio/ecape
+
 https://citylikeamradio.github.io/ecape/html/index.html
 
 Contact
 -------------
  - Robert Capella
  - bob.capella@gmail.com
  - https://twitter.com/minusthebob
```

### Comparing `ecape-0.0.1/pyproject.toml` & `ecape-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
-exclude = ["/docs"]
+exclude = ["/docs", "/tests"]
 
 [tool.hatch.build.targets.wheel]
 exclude = ["src/ecape_py"]
 
 [project]
 name = "ecape"
 dynamic = ["version"]
```

### Comparing `ecape-0.0.1/PKG-INFO` & `ecape-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.1
+Version: 0.0.2
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -38,14 +38,15 @@
 ```console
 pip install ecape
 ```
 
 Documentation, Source
 -------------
 https://github.com/citylikeamradio/ecape
+
 https://citylikeamradio.github.io/ecape/html/index.html
 
 Contact
 -------------
  - Robert Capella
  - bob.capella@gmail.com
  - https://twitter.com/minusthebob
```

