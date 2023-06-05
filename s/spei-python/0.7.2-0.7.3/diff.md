# Comparing `tmp/spei_python-0.7.2.tar.gz` & `tmp/spei_python-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei_python-0.7.2.tar", max compression
+gzip compressed data, was "spei_python-0.7.3.tar", max compression
```

## Comparing `spei_python-0.7.2.tar` & `spei_python-0.7.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.7.2/README.md
--rw-r--r--   0        0        0      856 2023-06-05 18:39:44.695448 spei_python-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.7.2/spei/__init__.py
--rw-r--r--   0        0        0     2733 2023-05-30 00:46:55.019167 spei_python-0.7.2/spei/client.py
--rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.7.2/spei/resources/__init__.py
--rw-r--r--   0        0        0     4633 2023-06-05 18:38:40.204867 spei_python-0.7.2/spei/resources/ordenes.py
--rw-r--r--   0        0        0     1791 2023-05-30 01:26:04.772295 spei_python-0.7.2/spei/types.py
--rw-r--r--   0        0        0     2272 2023-05-30 01:00:59.645173 spei_python-0.7.2/spei/utils.py
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.7.3/README.md
+-rw-r--r--   0        0        0      856 2023-06-05 18:41:56.756641 spei_python-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.7.3/spei/__init__.py
+-rw-r--r--   0        0        0     2733 2023-05-30 00:46:55.019167 spei_python-0.7.3/spei/client.py
+-rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.7.3/spei/resources/__init__.py
+-rw-r--r--   0        0        0     4647 2023-06-05 18:40:50.959265 spei_python-0.7.3/spei/resources/ordenes.py
+-rw-r--r--   0        0        0     1791 2023-05-30 01:26:04.772295 spei_python-0.7.3/spei/types.py
+-rw-r--r--   0        0        0     2272 2023-05-30 01:00:59.645173 spei_python-0.7.3/spei/utils.py
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.7.3/PKG-INFO
```

### Comparing `spei_python-0.7.2/README.md` & `spei_python-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.2/pyproject.toml` & `spei_python-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spei-python"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["gonz <gonzasestopal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "spei"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -27,13 +27,13 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.2"
+version = "0.7.3"
 tag_format = "v$version"
 bump_message = "bump: Semantic Release Bot: Release Version: $new_version 🤖🚀 [skip ci]"
 version_files = [
     "pyproject.toml:version",
 ]
```

### Comparing `spei_python-0.7.2/spei/client.py` & `spei_python-0.7.3/spei/client.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.2/spei/resources/ordenes.py` & `spei_python-0.7.3/spei/resources/ordenes.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 
 class Respuesta(BaseModel):
     categoria: types.CategoriaOrdenPago
 
     id: str
     fecha_oper: int
-    err_codigo: int
+    err_codigo: types.CodigoError
     err_descripcion: str
 
     class Config:  # noqa: WPS306, WPS431
         use_enum_values = True
 
     def build_xml(self):
         mensaje = etree.Element('mensaje', categoria=self.categoria)
```

### Comparing `spei_python-0.7.2/spei/types.py` & `spei_python-0.7.3/spei/types.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.2/spei/utils.py` & `spei_python-0.7.3/spei/utils.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.2/PKG-INFO` & `spei_python-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei-python
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 Author: gonz
 Author-email: gonzasestopal@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

