# Comparing `tmp/spei_python-0.7.3.tar.gz` & `tmp/spei_python-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei_python-0.7.3.tar", max compression
+gzip compressed data, was "spei_python-0.7.4.tar", max compression
```

## Comparing `spei_python-0.7.3.tar` & `spei_python-0.7.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.7.3/README.md
--rw-r--r--   0        0        0      856 2023-06-05 18:41:56.756641 spei_python-0.7.3/pyproject.toml
--rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.7.3/spei/__init__.py
--rw-r--r--   0        0        0     2733 2023-05-30 00:46:55.019167 spei_python-0.7.3/spei/client.py
--rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.7.3/spei/resources/__init__.py
--rw-r--r--   0        0        0     4647 2023-06-05 18:40:50.959265 spei_python-0.7.3/spei/resources/ordenes.py
--rw-r--r--   0        0        0     1791 2023-05-30 01:26:04.772295 spei_python-0.7.3/spei/types.py
--rw-r--r--   0        0        0     2272 2023-05-30 01:00:59.645173 spei_python-0.7.3/spei/utils.py
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.7.4/README.md
+-rw-r--r--   0        0        0      856 2023-06-05 20:22:53.933878 spei_python-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.7.4/spei/__init__.py
+-rw-r--r--   0        0        0     2733 2023-05-30 00:46:55.019167 spei_python-0.7.4/spei/client.py
+-rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.7.4/spei/resources/__init__.py
+-rw-r--r--   0        0        0     4669 2023-06-05 20:19:27.609996 spei_python-0.7.4/spei/resources/ordenes.py
+-rw-r--r--   0        0        0     1791 2023-05-30 01:26:04.772295 spei_python-0.7.4/spei/types.py
+-rw-r--r--   0        0        0     2272 2023-05-30 01:00:59.645173 spei_python-0.7.4/spei/utils.py
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.7.4/PKG-INFO
```

### Comparing `spei_python-0.7.3/README.md` & `spei_python-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.3/pyproject.toml` & `spei_python-0.7.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spei-python"
-version = "0.7.3"
+version = "0.7.4"
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
-version = "0.7.3"
+version = "0.7.4"
 tag_format = "v$version"
 bump_message = "bump: Semantic Release Bot: Release Version: $new_version 🤖🚀 [skip ci]"
 version_files = [
     "pyproject.toml:version",
 ]
```

### Comparing `spei_python-0.7.3/spei/client.py` & `spei_python-0.7.4/spei/client.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.3/spei/resources/ordenes.py` & `spei_python-0.7.4/spei/resources/ordenes.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     class Config:  # noqa: WPS306, WPS431
         use_enum_values = True
 
     def build_xml(self):
         mensaje = etree.Element('mensaje', categoria=self.categoria)
         orden_pago = etree.SubElement(mensaje, 'respuesta')
 
-        for element, value in self.dict().items():  # noqa: WPS110
+        for element, value in self.dict(exclude={'categoria',}).items():  # noqa: WPS110
             if element in self.__fields__:
                 upper_camel_case_element = to_upper_camel_case(element)
                 subelement = etree.SubElement(orden_pago, upper_camel_case_element)
                 subelement.text = str(value)
 
         return mensaje
```

### Comparing `spei_python-0.7.3/spei/types.py` & `spei_python-0.7.4/spei/types.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.3/spei/utils.py` & `spei_python-0.7.4/spei/utils.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.3/PKG-INFO` & `spei_python-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei-python
-Version: 0.7.3
+Version: 0.7.4
 Summary: 
 Author: gonz
 Author-email: gonzasestopal@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

