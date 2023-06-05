# Comparing `tmp/godto-0.0.3.tar.gz` & `tmp/godto-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godto-0.0.3.tar", last modified: Sun Jun  4 21:36:43 2023, max compression
+gzip compressed data, was "godto-0.0.4.tar", last modified: Mon Jun  5 21:20:09 2023, max compression
```

## Comparing `godto-0.0.3.tar` & `godto-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.496627 godto-0.0.3/
--rw-rw-r--   0 louis     (1000) louis     (1000)      145 2023-06-03 11:01:33.000000 godto-0.0.3/.gitignore
--rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-06-02 22:46:58.000000 godto-0.0.3/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)     1950 2023-06-04 21:36:43.496627 godto-0.0.3/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      843 2023-06-04 21:34:04.000000 godto-0.0.3/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)      100 2023-06-04 21:17:59.000000 godto-0.0.3/direct_dependency_requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       24 2023-06-04 21:15:51.000000 godto-0.0.3/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-06-04 21:36:43.496627 godto-0.0.3/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     3273 2023-06-04 21:16:42.000000 godto-0.0.3/setup.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.484627 godto-0.0.3/src/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto/
--rw-rw-r--   0 louis     (1000) louis     (1000)      442 2023-06-04 21:34:38.000000 godto-0.0.3/src/godto/__init__.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.484627 godto-0.0.3/src/godto/data/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto/data/openapi/
--rw-rw-r--   0 louis     (1000) louis     (1000)       94 2023-06-02 23:16:49.000000 godto-0.0.3/src/godto/data/openapi/README.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto/data/openapi/v2.0/
--rw-rw-r--   0 louis     (1000) louis     (1000)      248 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v2.0/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)    40247 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v2.0/schema.json
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.492627 godto-0.0.3/src/godto/data/openapi/v3.0/
--rw-rw-r--   0 louis     (1000) louis     (1000)      890 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v3.0/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)    35817 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v3.0/schema.json
--rw-rw-r--   0 louis     (1000) louis     (1000)    22670 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v3.0/schema.yaml
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.492627 godto-0.0.3/src/godto/openapi/
--rw-rw-r--   0 louis     (1000) louis     (1000)    14214 2023-06-04 20:46:08.000000 godto-0.0.3/src/godto/openapi/v3.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     1950 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      560 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)      100 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      113 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        6 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.922971 godto-0.0.4/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      145 2023-06-03 11:01:33.000000 godto-0.0.4/.gitignore
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-06-02 22:46:58.000000 godto-0.0.4/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1871 2023-06-05 21:20:09.922971 godto-0.0.4/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      764 2023-06-05 20:31:50.000000 godto-0.0.4/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)       40 2023-06-05 20:31:50.000000 godto-0.0.4/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-06-05 21:20:09.922971 godto-0.0.4/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3135 2023-06-05 20:31:50.000000 godto-0.0.4/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.910972 godto-0.0.4/src/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.914972 godto-0.0.4/src/godto/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      442 2023-06-04 21:34:38.000000 godto-0.0.4/src/godto/__init__.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.910972 godto-0.0.4/src/godto/data/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.918972 godto-0.0.4/src/godto/data/openapi/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       94 2023-06-02 23:16:49.000000 godto-0.0.4/src/godto/data/openapi/README.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.918972 godto-0.0.4/src/godto/data/openapi/v2.0/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      248 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v2.0/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    40247 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v2.0/schema.json
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.922971 godto-0.0.4/src/godto/data/openapi/v3.0/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      890 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v3.0/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    35817 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v3.0/schema.json
+-rw-rw-r--   0 louis     (1000) louis     (1000)    22670 2023-06-02 23:13:14.000000 godto-0.0.4/src/godto/data/openapi/v3.0/schema.yaml
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.922971 godto-0.0.4/src/godto/openapi/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      680 2023-06-05 21:07:01.000000 godto-0.0.4/src/godto/openapi/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    12592 2023-06-05 20:41:15.000000 godto-0.0.4/src/godto/openapi/v3.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-05 21:20:09.914972 godto-0.0.4/src/godto.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1871 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      553 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        6 2023-06-05 21:20:09.000000 godto-0.0.4/src/godto.egg-info/top_level.txt
```

### Comparing `godto-0.0.3/LICENSE` & `godto-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `godto-0.0.3/PKG-INFO` & `godto-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godto
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Transfer Object (DTO) codegen from JSON schemas following the OpenAPI spec
 Home-page: https://github.com/lmmx/godto
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
@@ -31,20 +31,20 @@
 # godto
 
 Data Transfer Object (DTO) codegen from JSON schemas following the OpenAPI spec 
 
 ## Usage
 
 To work with an OpenAPI schema, load it with the `Model` class,
-which is a [Dataclass Wizard](https://github.com/rnag/dataclass-wizard/) deserialiser.
+which is a Pydantic model (however note that the class name 'Model' comes from the OpenAPI spec).
 
 ```py
 from godto.openapi.v3 import Model
 
-model = Model.from_json(schema_json)
+model = Model.parse_raw(schema_json)
 ```
 
 For example the Transport for London `StopPoint` API schema
 is [shipped as package data][StopPoint_schema] in `tubeulator`.
 
 [StopPoint_schema]: https://github.com/lmmx/tubeulator/blob/master/src/tubeulator/data/openapi/StopPoint/StopPoint.json
 
@@ -53,10 +53,8 @@
 
 path_to_schema = Path("data/openapi/StopPoint/StopPoint.json")
 schema_json = path_to_schema.read_text()
 ```
 
 ## Requirements
 
-Python 3.9 or 3.10
-
-- Awaiting [bugfix](https://github.com/rnag/dataclass-wizard/issues/89) for 3.11+
+Python 3.9+
```

### Comparing `godto-0.0.3/setup.py` & `godto-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet :: WWW/HTTP",
 ]
 INSTALL_REQUIRES = Path("requirements.txt").read_text().splitlines()
-INSTALL_DEPENDENCIES = Path("direct_dependency_requirements.txt").read_text().splitlines()
 EXTRAS_REQUIRE = {
     "docs": [
         #"sphinx>=4",
         #"sphinx_rtd_theme",
         #"sphinx-autodoc-typehints",
     ],
     "tests": ["coverage[toml]>=5.5", "pytest"],
@@ -94,11 +93,10 @@
         setup_requires=["setuptools_scm"],
         entry_points={
             "console_scripts": [
                 # "godto = godto.cli:main",
             ],
         },
         install_requires=INSTALL_REQUIRES,
-        dependency_links=INSTALL_DEPENDENCIES,
         extras_require=EXTRAS_REQUIRE,
         python_requires=PYTHON_REQUIRES,
     )
```

### Comparing `godto-0.0.3/src/godto/data/openapi/v2.0/schema.json` & `godto-0.0.4/src/godto/data/openapi/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `godto-0.0.3/src/godto/data/openapi/v3.0/README.md` & `godto-0.0.4/src/godto/data/openapi/v3.0/README.md`

 * *Files identical despite different names*

### Comparing `godto-0.0.3/src/godto/data/openapi/v3.0/schema.json` & `godto-0.0.4/src/godto/data/openapi/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `godto-0.0.3/src/godto/data/openapi/v3.0/schema.yaml` & `godto-0.0.4/src/godto/data/openapi/v3.0/schema.yaml`

 * *Files identical despite different names*

### Comparing `godto-0.0.3/src/godto.egg-info/PKG-INFO` & `godto-0.0.4/src/godto.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godto
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Transfer Object (DTO) codegen from JSON schemas following the OpenAPI spec
 Home-page: https://github.com/lmmx/godto
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
@@ -31,20 +31,20 @@
 # godto
 
 Data Transfer Object (DTO) codegen from JSON schemas following the OpenAPI spec 
 
 ## Usage
 
 To work with an OpenAPI schema, load it with the `Model` class,
-which is a [Dataclass Wizard](https://github.com/rnag/dataclass-wizard/) deserialiser.
+which is a Pydantic model (however note that the class name 'Model' comes from the OpenAPI spec).
 
 ```py
 from godto.openapi.v3 import Model
 
-model = Model.from_json(schema_json)
+model = Model.parse_raw(schema_json)
 ```
 
 For example the Transport for London `StopPoint` API schema
 is [shipped as package data][StopPoint_schema] in `tubeulator`.
 
 [StopPoint_schema]: https://github.com/lmmx/tubeulator/blob/master/src/tubeulator/data/openapi/StopPoint/StopPoint.json
 
@@ -53,10 +53,8 @@
 
 path_to_schema = Path("data/openapi/StopPoint/StopPoint.json")
 schema_json = path_to_schema.read_text()
 ```
 
 ## Requirements
 
-Python 3.9 or 3.10
-
-- Awaiting [bugfix](https://github.com/rnag/dataclass-wizard/issues/89) for 3.11+
+Python 3.9+
```

### Comparing `godto-0.0.3/src/godto.egg-info/SOURCES.txt` & `godto-0.0.4/src/godto.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .gitignore
 LICENSE
 README.md
-direct_dependency_requirements.txt
 requirements.txt
 setup.py
 src/godto/__init__.py
 src/godto.egg-info/PKG-INFO
 src/godto.egg-info/SOURCES.txt
 src/godto.egg-info/dependency_links.txt
 src/godto.egg-info/not-zip-safe
@@ -13,8 +12,9 @@
 src/godto.egg-info/top_level.txt
 src/godto/data/openapi/README.md
 src/godto/data/openapi/v2.0/README.md
 src/godto/data/openapi/v2.0/schema.json
 src/godto/data/openapi/v3.0/README.md
 src/godto/data/openapi/v3.0/schema.json
 src/godto/data/openapi/v3.0/schema.yaml
+src/godto/openapi/README.md
 src/godto/openapi/v3.py
```

