# Comparing `tmp/mecapacktools-1.0.2.tar.gz` & `tmp/mecapacktools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecapacktools-1.0.2.tar", max compression
+gzip compressed data, was "mecapacktools-1.0.3.tar", max compression
```

## Comparing `mecapacktools-1.0.2.tar` & `mecapacktools-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.0.2/LICENSE
--rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.0.2/mecapacktools/__init__.py
--rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.0.2/mecapacktools/libCfg.py
--rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.0.2/mecapacktools/libLog.py
--rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.0.2/mecapacktools/libMail.py
--rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.0.2/mecapacktools/libSql.py
--rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.0.2/mecapacktools/libTool.py
--rw-r--r--   0        0        0    20330 2023-05-24 07:28:15.036814 mecapacktools-1.0.2/mecapacktools/libWebServices.py
--rw-r--r--   0        0        0     1090 2023-05-24 10:18:52.423811 mecapacktools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      668 2023-04-27 13:23:11.491614 mecapacktools-1.0.2/README.md
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 mecapacktools-1.0.2/setup.py
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 mecapacktools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.0.3/mecapacktools/__init__.py
+-rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.0.3/mecapacktools/libCfg.py
+-rw-r--r--   0        0        0     4734 2023-06-05 12:28:18.869293 mecapacktools-1.0.3/mecapacktools/libFTP.py
+-rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.0.3/mecapacktools/libLog.py
+-rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.0.3/mecapacktools/libMail.py
+-rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.0.3/mecapacktools/libSql.py
+-rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.0.3/mecapacktools/libTool.py
+-rw-r--r--   0        0        0    20493 2023-06-05 09:14:51.310848 mecapacktools-1.0.3/mecapacktools/libWebServices.py
+-rw-r--r--   0        0        0     1160 2023-06-05 12:30:18.921073 mecapacktools-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      676 2023-06-05 11:21:37.250074 mecapacktools-1.0.3/README.md
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 mecapacktools-1.0.3/setup.py
+-rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 mecapacktools-1.0.3/PKG-INFO
```

### Comparing `mecapacktools-1.0.2/LICENSE` & `mecapacktools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.2/mecapacktools/libCfg.py` & `mecapacktools-1.0.3/mecapacktools/libCfg.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.2/mecapacktools/libLog.py` & `mecapacktools-1.0.3/mecapacktools/libLog.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.2/mecapacktools/libMail.py` & `mecapacktools-1.0.3/mecapacktools/libMail.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.2/mecapacktools/libSql.py` & `mecapacktools-1.0.3/mecapacktools/libSql.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.2/mecapacktools/libTool.py` & `mecapacktools-1.0.3/mecapacktools/libTool.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.2/mecapacktools/libWebServices.py` & `mecapacktools-1.0.3/mecapacktools/libWebServices.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,15 +389,19 @@
 # "Debugage de Request"
 # http_client.HTTPConnection.debuglevel = 1
 
 
 class webServices_S9000:
     """Class Webservices S9000"""
 
+    #: Variables
     hshParam = {}
+    hshParam["adress"] = ""
+    hshParam = {"adress": "", "user": "", "password": ""}
+    hshParam["request"] = [{"action": "", "param": ""}]
     __hshData = {}
 
     @property
     def data(self):
         """
         return data
```

### Comparing `mecapacktools-1.0.2/pyproject.toml` & `mecapacktools-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecapacktools"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 authors = ["Informatique Mecapack <informatique@mecapack.com>"]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 exclude = ["mecapacktools/libExcel.py"]
 
 
@@ -14,27 +14,29 @@
 sortedcontainers = "^2.4.0"
 requests = {version = "^2.28.2", optional = true}
 suds = {version = "^1.1.2", optional = true}
 xmltodict = {version = "^0.13.0", optional = true}
 pypyodbc = {version = "^1.3.6", optional = true}
 openpyxl = {version = "^3.1.2", optional = true}
 pywin32 = {version = "^306", optional = true}
+paramiko = {version ="^3.2.0", optional = true}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
 sphinx-markdown-builder = "^0.5.5"
 
 [tool.poetry.extras]
 excel = ["openpyxl","pywin32"]
-Sql =["pypyodbc"]
+Sql = ["pypyodbc"]
 WebServices = ["requests","xmltodict","suds"]
+FTP = ["paramiko"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mecapacktools-1.0.2/README.md` & `mecapacktools-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 `pip install mecapacktools[excel,sql,webservices]`
 
 ### Extensions diponibles :
 
 - excel 
 - Sql 
 - WebServices 
+- FTP 
 
 ## Notes pour le développement:
 
 ### Installation
 
 `poetry install --with dev --all-extras`
```

### Comparing `mecapacktools-1.0.2/setup.py` & `mecapacktools-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 {'': ['*']}
 
 install_requires = \
 ['arrow>=1.2.3,<2.0.0', 'sortedcontainers>=2.4.0,<3.0.0']
 
 extras_require = \
 {'excel': ['openpyxl>=3.1.2,<4.0.0', 'pywin32>=306,<307'],
+ 'ftp': ['paramiko>=3.2.0,<4.0.0'],
  'sql': ['pypyodbc>=1.3.6,<2.0.0'],
  'webservices': ['requests>=2.28.2,<3.0.0',
                  'suds>=1.1.2,<2.0.0',
                  'xmltodict>=0.13.0,<0.14.0']}
 
 setup_kwargs = {
     'name': 'mecapacktools',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': '',
-    'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\n\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\n- excel \n- Sql \n- WebServices \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier sur pypi `poetry publish --build`\n\n\n\n',
+    'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\n\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\n- excel \n- Sql \n- WebServices \n- FTP \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier sur pypi `poetry publish --build`\n\n\n\n',
     'author': 'Informatique Mecapack',
     'author_email': 'informatique@mecapack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mecapacktools-1.0.2/PKG-INFO` & `mecapacktools-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: mecapacktools
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: Informatique Mecapack
 Author-email: informatique@mecapack.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: excel
+Provides-Extra: ftp
 Provides-Extra: sql
 Provides-Extra: webservices
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0) ; extra == "excel"
+Requires-Dist: paramiko (>=3.2.0,<4.0.0) ; extra == "ftp"
 Requires-Dist: pypyodbc (>=1.3.6,<2.0.0) ; extra == "sql"
 Requires-Dist: pywin32 (>=306,<307) ; extra == "excel"
 Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "webservices"
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Requires-Dist: suds (>=1.1.2,<2.0.0) ; extra == "webservices"
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0) ; extra == "webservices"
 Description-Content-Type: text/markdown
@@ -36,14 +38,15 @@
 `pip install mecapacktools[excel,sql,webservices]`
 
 ### Extensions diponibles :
 
 - excel 
 - Sql 
 - WebServices 
+- FTP 
 
 ## Notes pour le développement:
 
 ### Installation
 
 `poetry install --with dev --all-extras`
```

