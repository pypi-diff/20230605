# Comparing `tmp/pycsw-rpi-0.1.1.tar.gz` & `tmp/pycsw-rpi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsw-rpi-0.1.1.tar", max compression
+gzip compressed data, was "pycsw-rpi-0.1.2.tar", max compression
```

## Comparing `pycsw-rpi-0.1.1.tar` & `pycsw-rpi-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1728 2022-05-03 14:14:41.137968 pycsw-rpi-0.1.1/Readme.md
--rw-r--r--   0        0        0     1400 2022-05-03 09:44:13.824152 pycsw-rpi-0.1.1/pycsw_rpi/admin.py
--rw-r--r--   0        0        0     1164 2022-05-03 09:43:44.492229 pycsw-rpi-0.1.1/pycsw_rpi/apiso.py
--rw-r--r--   0        0        0      796 2022-05-03 09:37:07.229339 pycsw-rpi-0.1.1/pycsw_rpi/config.py
--rw-r--r--   0        0        0     2963 2022-05-03 09:47:15.643655 pycsw-rpi-0.1.1/pycsw_rpi/metadata.py
--rw-r--r--   0        0        0      601 2022-04-28 17:34:10.402387 pycsw-rpi-0.1.1/pycsw_rpi/wsgi.py
--rw-r--r--   0        0        0      957 2022-05-03 14:19:25.396720 pycsw-rpi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2646 2022-05-03 14:19:29.645564 pycsw-rpi-0.1.1/setup.py
--rw-r--r--   0        0        0     2483 2022-05-03 14:19:29.646055 pycsw-rpi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1728 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/Readme.md
+-rw-r--r--   0        0        0     1400 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/admin.py
+-rw-r--r--   0        0        0     1164 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/apiso.py
+-rw-r--r--   0        0        0      796 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/config.py
+-rw-r--r--   0        0        0     3064 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/metadata.py
+-rw-r--r--   0        0        0      601 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/wsgi.py
+-rw-r--r--   0        0        0      957 2023-06-05 11:37:10.633764 pycsw-rpi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2646 2023-06-05 11:37:17.166885 pycsw-rpi-0.1.2/setup.py
+-rw-r--r--   0        0        0     2483 2023-06-05 11:37:17.167250 pycsw-rpi-0.1.2/PKG-INFO
```

### Comparing `pycsw-rpi-0.1.1/Readme.md` & `pycsw-rpi-0.1.2/Readme.md`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.1/pycsw_rpi/admin.py` & `pycsw-rpi-0.1.2/pycsw_rpi/admin.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.1/pycsw_rpi/apiso.py` & `pycsw-rpi-0.1.2/pycsw_rpi/apiso.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.1/pycsw_rpi/config.py` & `pycsw-rpi-0.1.2/pycsw_rpi/config.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.1/pycsw_rpi/metadata.py` & `pycsw-rpi-0.1.2/pycsw_rpi/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,15 +89,16 @@
         "is_viewable": False,
         "is_searchable": False,
     }
 
     if check_type not in check_types:
         raise ValueError(f"Check type {check_type} not supported")
 
-    qparams = parse_qs(urlparse(url).query)
+    # parse query params and normalize qparams names to lowercase
+    qparams = {k.lower(): v for k, v in parse_qs(urlparse(url).query).items()}
 
     # request contains all the needed ows query params
     if {"service", "version", "request"}.issubset(qparams.keys()):
         check_types["is_ows"] = True
 
         if qparams["service"][0].lower() in ["wms", "wmts"]:
             if qparams["request"][0].lower() in ["getmap", "gettile"]:
```

### Comparing `pycsw-rpi-0.1.1/pycsw_rpi/wsgi.py` & `pycsw-rpi-0.1.2/pycsw_rpi/wsgi.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.1/pyproject.toml` & `pycsw-rpi-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycsw-rpi"
-version = "0.1.1"
+version = "0.1.2"
 description = "PyCSW monkey patched for Slovak national catalogue service"
 authors = ["Peter Mozolík <petermozolik@gmail.com>"]
 license = "MIT"
 readme = "Readme.md"
 repository = "https://gitlab.com/mzpsr/minzp/geocloud.sk/applications/pycsw-rpi"
 
 [tool.poetry.dependencies]
```

### Comparing `pycsw-rpi-0.1.1/setup.py` & `pycsw-rpi-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['SQLAlchemy>=1.4,<2.0', 'pycsw>=2.6,<3.0']
 
 entry_points = \
 {'console_scripts': ['pycsw_rpi-admin = pycsw_rpi.admin:run']}
 
 setup_kwargs = {
     'name': 'pycsw-rpi',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'PyCSW monkey patched for Slovak national catalogue service',
     'long_description': '# PyCSW RPI `pycsw-rpi`\n\n[Monkey patched](https://en.wikipedia.org/wiki/Monkey_patch) `pycsw` for Slovak national catalogue service. \n\nCheck [original `pycsw` documentation ](https://docs.pycsw.org/en/2.6.1/index.html) for more details.\n\n---\n\n## Setup\n\nUse exactly like original `pycsw`\n\n### Install\n\n```bash\npip install --user pycsw-rpi\n```\n\n### Create configuration file\n\nConfiguration file is not distributed with package. \n\nSample configuration can be downloaded from `<<url>>`\n\n### Administrative command (CLI)\n\n`pycsw_rpi-admin` script is installed with package in `$PATH`, this script is replacement for original `pycsw-admin.py` script supporting modified beahaviour and can be used exactly like original one.\n\n#### Create database\n\n```bash\npycsw_rpi-admin -c setup_db -f <<pconfiguration_file>>\n```\n\n#### Load records\n\n```bash\npycsw_rpi-admin -c load_records -f <<pconfiguration_file>> -p <<path_to_records_directory>>\n```\n\nCheck [original documentation](https://docs.pycsw.org/en/2.6.1/administration.html) for `pycsw-admin.py` administrative command.\n\n### Run "dev" self contained (toy) server\n\n```bash\npython -m pycsw_rpi.wsgi\n```\n\n### Deploy as WSGI application\n\n`pycsw_rpi.wsgi` module contains WSGI `application` object (function) ready to be deployed with WSGI server (e.g. `gunicorn`, `uwsgi`). No WSGI server is installed with this package as dependecy. \n\nTo deploy with `gunicorn`:\n\n```bash\n# `gunicorn` package need to installed separately\npip install --user gunicorn\ngunicorn pycsw_rpi.wsgi:application\n```\n\n---\n\n## Modifications implemented (via monkey patches) to original `pycsw`\n\nAdded queryables to APISO plugin:\n- `rpi:OrganizationUUID`\n- `rpi:IsViewable`\n- `rpi:IsSearchable`\n\n---\n\n## Contributions\n\n',
     'author': 'Peter Mozolík',
     'author_email': 'petermozolik@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/mzpsr/minzp/geocloud.sk/applications/pycsw-rpi',
```

### Comparing `pycsw-rpi-0.1.1/PKG-INFO` & `pycsw-rpi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycsw-rpi
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyCSW monkey patched for Slovak national catalogue service
 Home-page: https://gitlab.com/mzpsr/minzp/geocloud.sk/applications/pycsw-rpi
 License: MIT
 Author: Peter Mozolík
 Author-email: petermozolik@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

