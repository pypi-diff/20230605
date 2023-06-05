# Comparing `tmp/bowtie_json_schema-2023.6.1.tar.gz` & `tmp/bowtie_json_schema-2023.6.2.tar.gz`

## Comparing `bowtie_json_schema-2023.6.1.tar` & `bowtie_json_schema-2023.6.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.flake8
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.readthedocs.yml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/test-requirements.in
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/SECURITY.md
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/release.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/images.yml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/__main__.py
--rw-r--r--   0        0        0    31383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/cli.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/requirements.in
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/README.rst
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.flake8
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.readthedocs.yml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/test-requirements.in
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/SECURITY.md
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/release.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/images.yml
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/__main__.py
+-rw-r--r--   0        0        0    31383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/cli.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/conf.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/requirements.in
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/requirements.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/_static/dreamed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/LICENSE
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/README.rst
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.6.1/.flake8` & `bowtie_json_schema-2023.6.2/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/.pre-commit-config.yaml` & `bowtie_json_schema-2023.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/noxfile.py` & `bowtie_json_schema-2023.6.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/test-requirements.txt` & `bowtie_json_schema-2023.6.2/test-requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # via
     #   aiohttp
     #   requests
 click==8.1.3
     # via
     #   bowtie-json-schema
     #   trogon
-cryptography==40.0.2
+cryptography==41.0.1
     # via pyjwt
 frozenlist==1.3.3
     # via
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
     # via bowtie-json-schema
@@ -56,15 +56,15 @@
 linkify-it-py==2.0.2
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==2.2.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 mdit-py-plugins==0.3.5
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.4
     # via
@@ -93,27 +93,27 @@
     # via -r test-requirements.in
 pytest-icdiff==0.6
     # via -r test-requirements.in
 python-dateutil==2.8.2
     # via github3-py
 requests==2.31.0
     # via github3-py
-rich==13.3.5
+rich==13.4.1
     # via
     #   bowtie-json-schema
     #   textual
 six==1.16.0
     # via python-dateutil
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.26.0
+textual==0.27.0
     # via trogon
 trogon==0.4.0
     # via bowtie-json-schema
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aiodocker
     #   textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
```

### Comparing `bowtie_json_schema-2023.6.1/.github/SECURITY.md` & `bowtie_json_schema-2023.6.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/.github/dependabot.yml` & `bowtie_json_schema-2023.6.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/.github/workflows/ci.yml` & `bowtie_json_schema-2023.6.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.6.2/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/.github/workflows/images.yml` & `bowtie_json_schema-2023.6.2/.github/workflows/images.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/.github/workflows/report.yml` & `bowtie_json_schema-2023.6.2/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/bowtie/_cli.py` & `bowtie_json_schema-2023.6.2/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/bowtie/_commands.py` & `bowtie_json_schema-2023.6.2/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/bowtie/_core.py` & `bowtie_json_schema-2023.6.2/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/bowtie/_report.py` & `bowtie_json_schema-2023.6.2/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/bowtie/exceptions.py` & `bowtie_json_schema-2023.6.2/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/docs/Makefile` & `bowtie_json_schema-2023.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/docs/cli.rst` & `bowtie_json_schema-2023.6.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/docs/conf.py` & `bowtie_json_schema-2023.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/docs/contributing.rst` & `bowtie_json_schema-2023.6.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/docs/implementers.rst` & `bowtie_json_schema-2023.6.2/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/docs/index.rst` & `bowtie_json_schema-2023.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/docs/requirements.txt` & `bowtie_json_schema-2023.6.2/docs/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 click==8.1.3
     # via
     #   bowtie-json-schema
     #   sphinx-click
     #   trogon
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via pyjwt
 cycler==0.11.0
     # via matplotlib
 docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-click
@@ -79,15 +79,15 @@
 lxml==4.9.2
     # via sphinx-json-schema-spec
 markdown-it-py[linkify,plugins]==2.2.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 matplotlib==3.7.1
     # via sphinxext-opengraph
 mdit-py-plugins==0.3.5
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
@@ -127,15 +127,15 @@
     # via
     #   github3-py
     #   matplotlib
 requests==2.31.0
     # via
     #   github3-py
     #   sphinx
-rich==13.3.5
+rich==13.4.1
     # via
     #   bowtie-json-schema
     #   textual
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
@@ -173,19 +173,19 @@
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
 sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.26.0
+textual==0.27.0
     # via trogon
 trogon==0.4.0
     # via bowtie-json-schema
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aiodocker
     #   textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
```

### Comparing `bowtie_json_schema-2023.6.1/docs/_static/dreamed.png` & `bowtie_json_schema-2023.6.2/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/tests/test_integration.py` & `bowtie_json_schema-2023.6.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.6.2/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.6.2/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.6.2/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.6.2/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/.gitignore` & `bowtie_json_schema-2023.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/LICENSE` & `bowtie_json_schema-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/README.rst` & `bowtie_json_schema-2023.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/pyproject.toml` & `bowtie_json_schema-2023.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.1/PKG-INFO` & `bowtie_json_schema-2023.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

