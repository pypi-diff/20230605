# Comparing `tmp/db2ixf-0.1.4.tar.gz` & `tmp/db2ixf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2ixf-0.1.4.tar", last modified: Wed May 31 22:57:53 2023, max compression
+gzip compressed data, was "db2ixf-0.1.5.tar", last modified: Mon Jun  5 14:55:15 2023, max compression
```

## Comparing `db2ixf-0.1.4.tar` & `db2ixf-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:57:53.687338 db2ixf-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-31 22:56:48.000000 db2ixf-0.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-05-31 22:56:48.000000 db2ixf-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-31 22:57:53.687338 db2ixf-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-05-31 22:56:48.000000 db2ixf-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-31 22:56:48.000000 db2ixf-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:57:53.687338 db2ixf-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 22:56:48.000000 db2ixf-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:57:53.683338 db2ixf-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:57:53.683338 db2ixf-0.1.4/src/db2ixf/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 22:57:53.000000 db2ixf-0.1.4/src/db2ixf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/ixf.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 22:56:48.000000 db2ixf-0.1.4/src/db2ixf/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:57:53.687338 db2ixf-0.1.4/src/db2ixf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-31 22:57:53.000000 db2ixf-0.1.4/src/db2ixf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 22:57:53.000000 db2ixf-0.1.4/src/db2ixf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:57:53.000000 db2ixf-0.1.4/src/db2ixf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 22:57:53.000000 db2ixf-0.1.4/src/db2ixf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:57:52.000000 db2ixf-0.1.4/src/db2ixf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 22:57:53.000000 db2ixf-0.1.4/src/db2ixf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 22:57:53.000000 db2ixf-0.1.4/src/db2ixf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:55:15.833371 db2ixf-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-05 14:54:00.000000 db2ixf-0.1.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-06-05 14:54:00.000000 db2ixf-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-06-05 14:55:15.833371 db2ixf-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-05 14:54:00.000000 db2ixf-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-05 14:54:00.000000 db2ixf-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:55:15.833371 db2ixf-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 14:54:00.000000 db2ixf-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:55:15.829371 db2ixf-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:55:15.829371 db2ixf-0.1.5/src/db2ixf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/ixf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-05 14:54:00.000000 db2ixf-0.1.5/src/db2ixf/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:55:15.829371 db2ixf-0.1.5/src/db2ixf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 14:55:15.000000 db2ixf-0.1.5/src/db2ixf.egg-info/top_level.txt
```

### Comparing `db2ixf-0.1.4/CHANGELOG.md` & `db2ixf-0.1.5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,27 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres
 to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the
-changes for the upcoming release can be found
-in [here](https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md).
+changes for the upcoming release may be found
+in [here](https://github.com/ismailhammounou/db2ixf/tree/main/resources/changelog).
+
 
 <!-- release notes start -->
 
+## [0.1.5](https://github.com/ismailhammounou/db2ixf/tree/0.1.5) - 2023-06-03
+
+### Added
+
+- Support of floating point data
+  type [db2ixf-14](https://github.com/ismailhammounou/db2ixf/issues/14)
+
 ## [0.1.4](https://github.com/ismailhammounou/db2ixf/tree/0.1.4) - 2023-06-01
 
 ### Changed
 
 - Improve ci and fix
   issues [db2ixf-12](https://github.com/ismailhammounou/db2ixf/issues/12)
 - Improve ci-cd [db2ixf-2](https://github.com/ismailhammounou/db2ixf/issues/2)
```

### Comparing `db2ixf-0.1.4/LICENSE` & `db2ixf-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.4/PKG-INFO` & `db2ixf-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.4
+Version: 0.1.5
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
-Project-URL: homepage, https://github.com/ismailhammounou/db2ixf
-Project-URL: documentation, https://github.com/ismailhammounou/db2ixf/blob/main/README.md
+Project-URL: homepage, https://pypi.org/project/db2ixf/
+Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
 Project-URL: changelog, https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md
 Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format,Data,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.7
@@ -158,15 +158,15 @@
 │ parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                                                                                                                                                                         │
 └─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
 
  Made with heart :D
 ```
 
 For a detailed story and usage, please refer to the
-[documentation](https://github.com/ismailhammounou/db2ixf).
+[documentation](https://ismailhammounou.github.io/db2ixf/).
 
 ## Contributing
 
 IXF Parser is actively seeking contributions to enhance its features and
 reliability. Your participation is valuable in shaping the future of the
 project.
 
@@ -181,22 +181,23 @@
 Thank you for considering contributing to IXF Parser. Let's work together to
 create a powerful and dependable tool for working with DB2's IXF files.
 
 ### Todo
 
 - [ ] Search for contributors/maintainers/sponsors.
 - [ ] Add tests (Manual testing was done but need write unit tests).
-- [ ] Adding new collectors for other ixf data types: floating point ... etc.
+- [x] Adding new collector for the floating point data type.
+- [ ] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
-- [ ] Add better ci-cd.
-- [ ] Improve Makefile.
-- [ ] ~~Support multiprocessing.~~
-- [ ] ~~Support archived inputs: only python not CLI ?~~
+- [x] Add better ci-cd.
+- [x] Improve Makefile.
+- [x] ~~Support multiprocessing.~~ 
+- [x] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

### Comparing `db2ixf-0.1.4/README.md` & `db2ixf-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 │ parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                                                                                                                                                                         │
 └─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
 
  Made with heart :D
 ```
 
 For a detailed story and usage, please refer to the
-[documentation](https://github.com/ismailhammounou/db2ixf).
+[documentation](https://ismailhammounou.github.io/db2ixf/).
 
 ## Contributing
 
 IXF Parser is actively seeking contributions to enhance its features and
 reliability. Your participation is valuable in shaping the future of the
 project.
 
@@ -157,22 +157,23 @@
 Thank you for considering contributing to IXF Parser. Let's work together to
 create a powerful and dependable tool for working with DB2's IXF files.
 
 ### Todo
 
 - [ ] Search for contributors/maintainers/sponsors.
 - [ ] Add tests (Manual testing was done but need write unit tests).
-- [ ] Adding new collectors for other ixf data types: floating point ... etc.
+- [x] Adding new collector for the floating point data type.
+- [ ] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
-- [ ] Add better ci-cd.
-- [ ] Improve Makefile.
-- [ ] ~~Support multiprocessing.~~
-- [ ] ~~Support archived inputs: only python not CLI ?~~
+- [x] Add better ci-cd.
+- [x] Improve Makefile.
+- [x] ~~Support multiprocessing.~~ 
+- [x] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

### Comparing `db2ixf-0.1.4/pyproject.toml` & `db2ixf-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 
 [project.optional-dependencies]
 
 [project.scripts]
 db2ixf = 'db2ixf.cli:app'
 
 [project.urls]
-homepage = 'https://github.com/ismailhammounou/db2ixf'
-documentation = 'https://github.com/ismailhammounou/db2ixf/blob/main/README.md'
+homepage = 'https://pypi.org/project/db2ixf/'
+documentation = 'https://ismailhammounou.github.io/db2ixf/'
 repository = 'https://github.com/ismailhammounou/db2ixf.git'
 changelog = 'https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md'
 
 
 
 [tool.setuptools]
 zip-safe = false
```

### Comparing `db2ixf-0.1.4/src/db2ixf/__init__.py` & `db2ixf-0.1.5/src/db2ixf/__init__.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.4/src/db2ixf/cli.py` & `db2ixf-0.1.5/src/db2ixf/cli.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.4/src/db2ixf/collectors.py` & `db2ixf-0.1.5/src/db2ixf/collectors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 """Collects data from fields extracted from data records."""
-from datetime import datetime, date, time
+from datetime import datetime
 from struct import unpack
 from typing import Union
 
 
 def collect_smallint(c, fields, pos, encoding) -> int:
     """Collects SMALLINT data type from ixf as an integer.
 
@@ -70,14 +70,77 @@
     int:
         Integer.
     """
     field = int(unpack('<q', fields[pos:pos + 8])[0])
     return field
 
 
+def collect_decimal(c, fields, pos, encoding) -> Union[int, float]:
+    """Collects DECIMAL data type from ixf as a integer or a float.
+
+    Parameters
+    ----------
+    c : dict
+        Column descriptor extracted from IXF.
+    fields : str
+        Binary string containing data of the row.
+    pos : int
+        Position of the column in the `fields`.
+    encoding : str
+        Encoding of the ixf file.
+
+    Returns
+    -------
+    Union[int, float]:
+        Integer or Float
+    """
+    p = int(c['IXFCLENG'][0:3])
+    s = int(c['IXFCLENG'][3:5])
+    length = int((p + 2) / 2)
+    field = fields[pos:pos + length]
+
+    dec = 0.0
+    for b in range(0, min(len(field), length) - 1):
+        dec = dec * 100 + int(field[b] >> 4) * 10 + int(field[b] & 0x0f)
+    dec = dec * 10 + int(field[-1] >> 4)
+
+    if int(field[-1] & 0x0f) != 12:
+        dec = -dec
+
+    if s == 0:
+        return int(dec)
+
+    return dec / pow(10, s)
+
+
+def collect_floating_point(c, fields, pos, encoding) -> float:
+    """Collects FLOATING POINT data type from ixf as a float.
+
+    Parameters
+    ----------
+    c : dict
+        Column descriptor extracted from IXF.
+    fields : str
+        Binary string containing data of the row.
+    pos : int
+        Position of the column in the `fields`.
+    encoding : str
+        Encoding of the ixf file.
+
+    Returns
+    -------
+    float
+        A python float object.
+    """
+    length = int(c['IXFCLENG'])
+    fmt = '!d' if length == 8 else '!f'
+    field = float(unpack(fmt, fields[pos:pos + length])[0])
+    return field
+
+
 def collect_char(c, fields, pos, encoding) -> str:
     """Collects CHAR data type from ixf as a string.
 
     Parameters
     ----------
     c : dict
         Column descriptor extracted from IXF.
@@ -186,45 +249,7 @@
     Returns
     -------
     timestamp:
         Timestamp of format yyyy-mm-dd-HH.MM.SS.UUUUUU
     """
     field = str(fields[pos:pos + 26], encoding=encoding)
     return datetime.strptime(field, '%Y-%m-%d-%H.%M.%S.%f')
-
-
-def collect_decimal(c, fields, pos, encoding) -> Union[int, float]:
-    """Collects DECIMAL data type from ixf as a integer or a float.
-
-    Parameters
-    ----------
-    c : dict
-        Column descriptor extracted from IXF.
-    fields : str
-        Binary string containing data of the row.
-    pos : int
-        Position of the column in the `fields`.
-    encoding : str
-        Encoding of the ixf file.
-
-    Returns
-    -------
-    Union[int, float]:
-        Integer or Float
-    """
-    p = int(c['IXFCLENG'][0:3])
-    s = int(c['IXFCLENG'][3:5])
-    length = int((p + 2) / 2)
-    field = fields[pos:pos + length]
-
-    dec = 0.0
-    for b in range(0, min(len(field), length) - 1):
-        dec = dec * 100 + int(field[b] >> 4) * 10 + int(field[b] & 0x0f)
-    dec = dec * 10 + int(field[-1] >> 4)
-
-    if int(field[-1] & 0x0f) != 12:
-        dec = -dec
-
-    if s == 0:
-        return int(dec)
-
-    return dec / pow(10, s)
```

### Comparing `db2ixf-0.1.4/src/db2ixf/constants.py` & `db2ixf-0.1.5/src/db2ixf/constants.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.4/src/db2ixf/exceptions.py` & `db2ixf-0.1.5/src/db2ixf/exceptions.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.4/src/db2ixf/helpers.py` & `db2ixf-0.1.5/src/db2ixf/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,33 +23,38 @@
 
     mapper = {
         'DATE': pyarrow.date32(),
         'TIME': pyarrow.time64('ns'),
         'TIMESTAMP': pyarrow.timestamp('ns'),
         'VARCHAR': pyarrow.string(),
         'CHAR': pyarrow.string(),
+        'FLOATING POINT': pyarrow.float64(),
         'DECIMAL': pyarrow.decimal128(19),
         'BIGINT': pyarrow.int64(),
         'INTEGER': pyarrow.int32(),
         'SMALLINT': pyarrow.int16(),
     }
 
     schema = {}
     for c in cols:
         cname = c['IXFCNAME'].decode('utf-8').strip()
         ctype = int(c['IXFCTYPE'])
         dtype = mapper[IXF_DTYPES[ctype]]
 
+        if ctype == 480:
+            length = int(c['IXFCLENG'])
+            dtype = pyarrow.float32() if length == 4 else dtype
+
         if ctype == 484:
             precision = int(c['IXFCLENG'][0:3])
             scale = int(c['IXFCLENG'][3:5])
             if scale == 0:
                 dtype = pyarrow.int64()
             else:
-                dtype = pyarrow.decimal128(precision, scale)
+                dtype = pyarrow.decimal256(precision, scale)
 
         if ctype == 392:
             fsp = int(c['IXFCLENG'])
             if fsp == 0:
                 dtype = pyarrow.timestamp('s')
             elif 0 < fsp <= 3:
                 dtype = pyarrow.timestamp('ms')
@@ -82,26 +87,31 @@
 
     mapper = {
         'DATE': 'datetime64[ns]',
         'TIME': 'datetime64[ns]',
         'TIMESTAMP': 'datetime64[ns]',
         'VARCHAR': object,
         'CHAR': object,
+        'FLOATING POINT': 'float64',
         'DECIMAL': 'float32',
         'BIGINT': 'int64',
         'INTEGER': 'int64',
         'SMALLINT': 'int64',
     }
 
     schema = {}
     for c in cols:
         cname = str(c['IXFCNAME'], encoding='utf-8').strip()
         ctype = int(c['IXFCTYPE'])
         dtype = mapper[IXF_DTYPES[ctype]]
 
+        if ctype == 480:
+            length = int(c['IXFCLENG'])
+            dtype = 'float32' if length == 4 else dtype
+
         if ctype == 484:
             precision = int(c['IXFCLENG'][0:3])
             scale = int(c['IXFCLENG'][3:5])
             if scale == 0:
                 dtype = 'int64'
             else:
                 dtype = 'float32'
```

### Comparing `db2ixf-0.1.4/src/db2ixf/ixf.py` & `db2ixf-0.1.5/src/db2ixf/ixf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 
 import sys
 
 import csv
 import json
 import pyarrow.parquet
 from db2ixf.collectors import (collect_bigint,
-                                                     collect_char,
-                                                     collect_date,
-                                                     collect_decimal,
-                                                     collect_integer,
-                                                     collect_time,
-                                                     collect_timestamp,
-                                                     collect_varchar,
-                                                     collect_smallint)
+                               collect_char,
+                               collect_date,
+                               collect_decimal,
+                               collect_integer,
+                               collect_time,
+                               collect_timestamp,
+                               collect_varchar,
+                               collect_smallint,
+                               collect_floating_point)
 from db2ixf.constants import (HEADER_RECORD_TYPE,
-                                                    TABLE_RECORD_TYPE,
-                                                    COL_DESCRIPTOR_RECORD_TYPE,
-                                                    DATA_RECORD_TYPE)
+                              TABLE_RECORD_TYPE,
+                              COL_DESCRIPTOR_RECORD_TYPE,
+                              DATA_RECORD_TYPE)
 from db2ixf.encoders import CustomJSONEncoder
 from db2ixf.exceptions import (
     NotValidColumnDescriptorException,
     UnknownDataTypeException)
 from db2ixf.helpers import get_batch, get_pyarrow_schema
 from db2ixf.logger import logger
 from os import PathLike
@@ -255,14 +256,15 @@
             # Collect data
             switcher = {
                 384: collect_date,
                 388: collect_time,
                 392: collect_timestamp,
                 448: collect_varchar,
                 452: collect_char,
+                480: collect_floating_point,
                 484: collect_decimal,
                 492: collect_bigint,
                 496: collect_integer,
                 500: collect_smallint,
             }
             func = switcher.get(col_type, None)
             try:
```

### Comparing `db2ixf-0.1.4/src/db2ixf/logger.py` & `db2ixf-0.1.5/src/db2ixf/logger.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.4/src/db2ixf.egg-info/PKG-INFO` & `db2ixf-0.1.5/src/db2ixf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.4
+Version: 0.1.5
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
-Project-URL: homepage, https://github.com/ismailhammounou/db2ixf
-Project-URL: documentation, https://github.com/ismailhammounou/db2ixf/blob/main/README.md
+Project-URL: homepage, https://pypi.org/project/db2ixf/
+Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
 Project-URL: changelog, https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md
 Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format,Data,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.7
@@ -158,15 +158,15 @@
 │ parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                                                                                                                                                                         │
 └─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
 
  Made with heart :D
 ```
 
 For a detailed story and usage, please refer to the
-[documentation](https://github.com/ismailhammounou/db2ixf).
+[documentation](https://ismailhammounou.github.io/db2ixf/).
 
 ## Contributing
 
 IXF Parser is actively seeking contributions to enhance its features and
 reliability. Your participation is valuable in shaping the future of the
 project.
 
@@ -181,22 +181,23 @@
 Thank you for considering contributing to IXF Parser. Let's work together to
 create a powerful and dependable tool for working with DB2's IXF files.
 
 ### Todo
 
 - [ ] Search for contributors/maintainers/sponsors.
 - [ ] Add tests (Manual testing was done but need write unit tests).
-- [ ] Adding new collectors for other ixf data types: floating point ... etc.
+- [x] Adding new collector for the floating point data type.
+- [ ] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
-- [ ] Add better ci-cd.
-- [ ] Improve Makefile.
-- [ ] ~~Support multiprocessing.~~
-- [ ] ~~Support archived inputs: only python not CLI ?~~
+- [x] Add better ci-cd.
+- [x] Improve Makefile.
+- [x] ~~Support multiprocessing.~~ 
+- [x] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

### Comparing `db2ixf-0.1.4/src/db2ixf.egg-info/SOURCES.txt` & `db2ixf-0.1.5/src/db2ixf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

