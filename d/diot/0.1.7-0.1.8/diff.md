# Comparing `tmp/diot-0.1.7.tar.gz` & `tmp/diot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diot-0.1.7.tar", max compression
+gzip compressed data, was "diot-0.1.8.tar", max compression
```

## Comparing `diot-0.1.7.tar` & `diot-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-03-22 01:33:15.823228 diot-0.1.7/LICENSE
--rw-r--r--   0        0        0     5283 2023-03-22 01:33:15.823228 diot-0.1.7/README.md
--rw-r--r--   0        0        0      195 2023-03-22 01:33:15.823228 diot-0.1.7/diot/__init__.py
--rw-r--r--   0        0        0    27959 2023-03-22 01:33:15.823228 diot-0.1.7/diot/diot.py
--rw-r--r--   0        0        0     3070 2023-03-22 01:33:15.823228 diot-0.1.7/diot/transforms.py
--rw-r--r--   0        0        0     1510 2023-03-22 01:33:15.823228 diot-0.1.7/diot/utils.py
--rw-r--r--   0        0        0     1011 2023-03-22 01:33:15.823228 diot-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 diot-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-05 16:01:50.758986 diot-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5283 2023-06-05 16:01:50.758986 diot-0.1.8/README.md
+-rw-r--r--   0        0        0      195 2023-06-05 16:01:50.758986 diot-0.1.8/diot/__init__.py
+-rw-r--r--   0        0        0    27959 2023-06-05 16:01:50.758986 diot-0.1.8/diot/diot.py
+-rw-r--r--   0        0        0     3070 2023-06-05 16:01:50.758986 diot-0.1.8/diot/transforms.py
+-rw-r--r--   0        0        0     1587 2023-06-05 16:01:50.758986 diot-0.1.8/diot/utils.py
+-rw-r--r--   0        0        0     1059 2023-06-05 16:01:50.758986 diot-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 diot-0.1.8/setup.py
+-rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 diot-0.1.8/PKG-INFO
```

### Comparing `diot-0.1.7/LICENSE` & `diot-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `diot-0.1.7/README.md` & `diot-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `diot-0.1.7/diot/diot.py` & `diot-0.1.8/diot/diot.py`

 * *Files identical despite different names*

### Comparing `diot-0.1.7/diot/transforms.py` & `diot-0.1.8/diot/transforms.py`

 * *Files identical despite different names*

### Comparing `diot-0.1.7/diot/utils.py` & `diot-0.1.8/diot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         out = [nest(val, types, dest_type, frozen) for val in value]
         try:
             return value.__class__(out)
         except Exception:  # pragma: no cover
             return out
 
     if dict in types and isinstance(value, dict):  # type: ignore
+        if issubclass(value.__class__, dest_type):
+            return value
+
         return dest_type(
             [
                 (key, nest(val, types, dest_type, frozen))
                 for key, val in value.items()
             ]
         )
     return value
```

### Comparing `diot-0.1.7/pyproject.toml` & `diot-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "diot"
-version = "0.1.7"
+version = "0.1.8"
 description = "Python dictionary with dot notation."
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/diot"
 repository = "https://github.com/pwwang/diot"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 inflection = "^0.5"
 
+[tool.poetry.build]
+generate-setup-file = true
+
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
 pyyaml = "^6"
 rtoml = "^0.8"
 
 [tool.mypy]
```

### Comparing `diot-0.1.7/PKG-INFO` & `diot-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diot
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python dictionary with dot notation.
 Home-page: https://github.com/pwwang/diot
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

