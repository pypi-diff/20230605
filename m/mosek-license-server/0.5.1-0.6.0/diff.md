# Comparing `tmp/mosek_license_server-0.5.1.tar.gz` & `tmp/mosek_license_server-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.5.1.tar", max compression
+gzip compressed data, was "mosek_license_server-0.6.0.tar", max compression
```

## Comparing `mosek_license_server-0.5.1.tar` & `mosek_license_server-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11346 2023-05-28 05:36:24.382351 mosek_license_server-0.5.1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-28 05:36:24.382351 mosek_license_server-0.5.1/mosek_license/__init__.py
--rw-r--r--   0        0        0      499 2023-05-28 05:36:24.382351 mosek_license_server-0.5.1/mosek_license/license.py
--rw-r--r--   0        0        0      520 2023-05-28 05:36:42.690482 mosek_license_server-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2389 2023-05-28 05:36:24.386351 mosek_license_server-0.5.1/readme.md
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 mosek_license_server-0.5.1/setup.py
--rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 mosek_license_server-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-05 04:57:24.903367 mosek_license_server-0.6.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-05 04:57:24.903367 mosek_license_server-0.6.0/mosek_license/__init__.py
+-rw-r--r--   0        0        0      558 2023-06-05 04:57:24.903367 mosek_license_server-0.6.0/mosek_license/license.py
+-rw-r--r--   0        0        0      520 2023-06-05 04:57:41.767634 mosek_license_server-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2389 2023-06-05 04:57:24.903367 mosek_license_server-0.6.0/readme.md
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 mosek_license_server-0.6.0/setup.py
+-rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 mosek_license_server-0.6.0/PKG-INFO
```

### Comparing `mosek_license_server-0.5.1/LICENSE` & `mosek_license_server-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.5.1/pyproject.toml` & `mosek_license_server-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosek-license-server"
-version = "v0.5.1"
+version = "v0.6.0"
 description = "Expose a mosek license via a nginx server"
 authors = ["Thomas Schmelzer <thomas.schmelzer@gmail.com>"]
 license = "Apache 2.0"
 readme = "readme.md"
 repository = "https://github.com/tschm/mosek-license-server"
 packages = [{include = "mosek_license"}]
```

### Comparing `mosek_license_server-0.5.1/readme.md` & `mosek_license_server-0.6.0/readme.md`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.5.1/setup.py` & `mosek_license_server-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['mosek_license']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mosek-license-server',
-    'version': '0.5.1',
+    'version': '0.6.0',
     'description': 'Expose a mosek license via a nginx server',
     'long_description': '# Mosek License Server\n\n[![Linting](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml/badge.svg)](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml)\n[![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)\n[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)\n[![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\nWe solve a common problem here. Assume $20$ researchers work on $50$ different strategies.\nUsing local copies of the same license file is a tedious exercise as\nthe file needs to get updated once a year.\nRather, each strategy would connect to the server to fetch a license using the mosek_license\nPython package. Once the strategy expires we only need to update the server.\nNo change for the strategies is required.\n\n## License server\n\n### Copy your license file into folder\n\nCopy the license file you have received (from Mosek) into the `web` folder.\nName it `mosek`.\n\nThe file should look like\n\n```bash\nSTART_LICENSE\nVENDOR MOSEKLM\n# PSN-4183\nFEATURE PTS MOSEKLM 10 31-jan-2024 uncounted ...\n# PSN-4182\nFEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...\nEND_LICENSE\n```\n\n### Start the nginx server\n\nShare the web folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/web:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via `http://localhost:8080/mosek`\n\nAs an alternative you can run the script\n\n```bash\n./start_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\n\nand then\n\n```python\nfrom mosek_license import license\n\n# It\'s important to upsert the license before you import mosek\nlicense.upsert(server="http://localhost:8080/mosek")\n\n# only now import mosek\nimport mosek\n```\n',
     'author': 'Thomas Schmelzer',
     'author_email': 'thomas.schmelzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tschm/mosek-license-server',
```

### Comparing `mosek_license_server-0.5.1/PKG-INFO` & `mosek_license_server-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.5.1
+Version: 0.6.0
 Summary: Expose a mosek license via a nginx server
 Home-page: https://github.com/tschm/mosek-license-server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
```

