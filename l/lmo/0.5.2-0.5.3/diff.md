# Comparing `tmp/lmo-0.5.2.tar.gz` & `tmp/lmo-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.5.2.tar", max compression
+gzip compressed data, was "lmo-0.5.3.tar", max compression
```

## Comparing `lmo-0.5.2.tar` & `lmo-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.2/LICENSE
--rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.2/README.md
--rw-r--r--   0        0        0      737 2023-06-04 10:26:56.859497 lmo-0.5.2/lmo/__init__.py
--rw-r--r--   0        0        0    22851 2023-06-05 01:00:55.316572 lmo-0.5.2/lmo/_lm.py
--rw-r--r--   0        0        0    11816 2023-06-04 14:08:29.938996 lmo-0.5.2/lmo/_lm_co.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.2/lmo/_meta.py
--rw-r--r--   0        0        0     4802 2023-06-04 14:08:29.950996 lmo-0.5.2/lmo/_pwm.py
--rw-r--r--   0        0        0     1615 2023-06-03 20:03:40.058997 lmo-0.5.2/lmo/_utils.py
--rw-r--r--   0        0        0     2240 2023-06-05 14:45:24.686312 lmo-0.5.2/lmo/diagnostic.py
--rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.5.2/lmo/linalg.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.2/lmo/py.typed
--rw-r--r--   0        0        0     5394 2023-06-05 14:17:18.849483 lmo-0.5.2/lmo/stats.py
--rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.2/lmo/typing.py
--rw-r--r--   0        0        0     2057 2023-06-05 14:48:17.622089 lmo-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 lmo-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.3/LICENSE
+-rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.3/README.md
+-rw-r--r--   0        0        0      737 2023-06-04 10:26:56.859497 lmo-0.5.3/lmo/__init__.py
+-rw-r--r--   0        0        0    22995 2023-06-05 16:35:54.551340 lmo-0.5.3/lmo/_lm.py
+-rw-r--r--   0        0        0    11816 2023-06-04 14:08:29.938996 lmo-0.5.3/lmo/_lm_co.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.3/lmo/_meta.py
+-rw-r--r--   0        0        0     4802 2023-06-04 14:08:29.950996 lmo-0.5.3/lmo/_pwm.py
+-rw-r--r--   0        0        0     1615 2023-06-03 20:03:40.058997 lmo-0.5.3/lmo/_utils.py
+-rw-r--r--   0        0        0     2240 2023-06-05 14:45:24.686312 lmo-0.5.3/lmo/diagnostic.py
+-rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.5.3/lmo/linalg.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.3/lmo/py.typed
+-rw-r--r--   0        0        0     5394 2023-06-05 14:17:18.849483 lmo-0.5.3/lmo/stats.py
+-rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.3/lmo/typing.py
+-rw-r--r--   0        0        0     2057 2023-06-05 16:36:45.192453 lmo-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 lmo-0.5.3/PKG-INFO
```

### Comparing `lmo-0.5.2/LICENSE` & `lmo-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/README.md` & `lmo-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/__init__.py` & `lmo-0.5.3/lmo/__init__.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/_lm.py` & `lmo-0.5.3/lmo/_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,19 @@
 
     l_rs = cast(
         npt.NDArray[T],
         l_moment(a, rs, trim, axis=axis, dtype=dtype, **kwargs)
     )
 
     r_eq_s = _r == _s
+    if r_eq_s.ndim < l_rs.ndim - 1:
+        r_eq_s = r_eq_s.reshape(
+            r_eq_s.shape + (1,) * (l_rs.ndim - r_eq_s.ndim - 1)
+        )
+
     with np.errstate(divide='ignore'):
         return np.where(
             r_eq_s,
             np.ones_like(l_rs[0]),
             np.divide(l_rs[0], l_rs[1], where=~r_eq_s)
         )[()]
```

### Comparing `lmo-0.5.2/lmo/_lm_co.py` & `lmo-0.5.3/lmo/_lm_co.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/_pwm.py` & `lmo-0.5.3/lmo/_pwm.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/_utils.py` & `lmo-0.5.3/lmo/_utils.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/diagnostic.py` & `lmo-0.5.3/lmo/diagnostic.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/linalg.py` & `lmo-0.5.3/lmo/linalg.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/stats.py` & `lmo-0.5.3/lmo/stats.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/lmo/typing.py` & `lmo-0.5.3/lmo/typing.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.2/pyproject.toml` & `lmo-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "lmo"
-version = "0.5.2"
+version = "0.5.3"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
```

### Comparing `lmo-0.5.2/PKG-INFO` & `lmo-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.5.2
+Version: 0.5.3
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

