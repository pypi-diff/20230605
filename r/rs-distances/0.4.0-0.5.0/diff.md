# Comparing `tmp/rs_distances-0.4.0.tar.gz` & `tmp/rs_distances-0.5.0.tar.gz`

## Comparing `rs_distances-0.4.0.tar` & `rs_distances-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 rs_distances-0.4.0/Cargo.toml
--rw-r--r--   0        0        0     2807 2023-06-03 05:19:15.000000 rs_distances-0.4.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      764 2023-06-03 16:25:17.000000 rs_distances-0.4.0/.gitignore
--rw-r--r--   0        0        0     2313 2023-06-03 16:58:44.000000 rs_distances-0.4.0/README.md
--rw-r--r--   0        0        0      914 2023-06-03 18:38:08.000000 rs_distances-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1433 2023-06-03 18:37:49.000000 rs_distances-0.4.0/src/lib.rs
--rw-r--r--   0        0        0    65812 2023-06-03 18:39:05.000000 rs_distances-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 rs_distances-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 rs_distances-0.5.0/Cargo.toml
+-rw-r--r--   0        0        0     2807 2023-06-03 05:19:15.000000 rs_distances-0.5.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      764 2023-06-03 16:25:17.000000 rs_distances-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2313 2023-06-03 16:58:44.000000 rs_distances-0.5.0/README.md
+-rw-r--r--   0        0        0      914 2023-06-03 18:38:08.000000 rs_distances-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-06-04 16:25:45.000000 rs_distances-0.5.0/src/lib.rs
+-rw-r--r--   0        0        0       13 2023-06-04 16:17:27.000000 rs_distances-0.5.0/src/spkd/mod.rs
+-rw-r--r--   0        0        0     4872 2023-06-05 02:34:35.000000 rs_distances-0.5.0/src/spkd/spkd.rs
+-rw-r--r--   0        0        0    65826 2023-06-05 03:28:05.000000 rs_distances-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 rs_distances-0.5.0/PKG-INFO
```

### Comparing `rs_distances-0.4.0/.github/workflows/CI.yml` & `rs_distances-0.5.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rs_distances-0.4.0/.gitignore` & `rs_distances-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rs_distances-0.4.0/README.md` & `rs_distances-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rs_distances-0.4.0/pyproject.toml` & `rs_distances-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rs_distances-0.4.0/Cargo.lock` & `rs_distances-0.5.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1632,16 +1632,17 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rs-distances"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
+ "itertools",
  "maturin",
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `rs_distances-0.4.0/PKG-INFO` & `rs_distances-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs-distances
-Version: 0.4.0
+Version: 0.5.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A Python module implemented in Rust for efficient calculations
 Author-email: Flynn OConnell <flynnoconnell@gmail.com>
 License: MIT
 Requires-Python: >=3.7
```

