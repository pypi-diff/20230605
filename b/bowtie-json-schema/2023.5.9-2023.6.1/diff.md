# Comparing `tmp/bowtie_json_schema-2023.5.9.tar.gz` & `tmp/bowtie_json_schema-2023.6.1.tar.gz`

## Comparing `bowtie_json_schema-2023.5.9.tar` & `bowtie_json_schema-2023.6.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.flake8
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.readthedocs.yml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/test-requirements.in
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/SECURITY.md
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/release.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/images.yml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/__main__.py
--rw-r--r--   0        0        0    31313 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/cli.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/requirements.in
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/conftest.py
--rw-r--r--   0        0        0    23967 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/README.rst
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/pyproject.toml
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.flake8
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.readthedocs.yml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/test-requirements.in
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/SECURITY.md
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/release.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/images.yml
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/__main__.py
+-rw-r--r--   0        0        0    31383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/cli.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/conf.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/requirements.in
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/docs/_static/dreamed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/LICENSE
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/README.rst
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.1/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.5.9/.flake8` & `bowtie_json_schema-2023.6.1/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/.pre-commit-config.yaml` & `bowtie_json_schema-2023.6.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.4.0
     hooks:
       - id: pyupgrade
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.267"
+    rev: "v0.0.270"
     hooks:
       - id: ruff
   - repo: https://github.com/Riverside-Healthcare/djLint
-    rev: v1.27.2
+    rev: v1.29.0
     hooks:
       - id: djlint-jinja
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - name: black (python implementations & bowtie internals)
         id: black
@@ -71,12 +71,12 @@
     rev: v0.17.1
     hooks:
       - name: stylua (lua implementations)
         id: stylua
         exclude: .*/json.lua
         args: ["--config-path", "implementations/lua-jsonschema/stylua.toml"]
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v16.0.3
+    rev: v16.0.4
     hooks:
-      - name: clang-format (c/c++/c# implementations)
+      - name: clang-format (c/c++/c#/java implementations)
         id: clang-format
-        types_or: [c++, c, c#, objective-c]
+        types_or: [c++, c, c#, java, objective-c]
```

### Comparing `bowtie_json_schema-2023.5.9/noxfile.py` & `bowtie_json_schema-2023.6.1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,28 +59,27 @@
 
 
 @session(tags=["style"])
 def readme(session):
     session.install("build", "twine")
     tmpdir = session.create_tmp()
     session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("python", "-m", "twine", "check", tmpdir + "/*")
+    session.run("python", "-m", "twine", "check", "--strict", tmpdir + "/*")
 
 
 @session(tags=["style"])
 def style(session):
     session.install("ruff")
     session.run("python", "-m", "ruff", "check", BOWTIE, TESTS, __file__)
 
 
 @session()
 def typing(session):
-    # FIXME: Don't repeat dependencies.
-    session.install("pyright", "types-jsonschema", ROOT)
-    session.run("python", "-m", "pyright", BOWTIE)
+    session.install("pyright", ROOT)
+    session.run("pyright", BOWTIE)
 
 
 @session(tags=["docs"])
 @nox.parametrize(
     "builder",
     [
         nox.param(name, id=name)
```

### Comparing `bowtie_json_schema-2023.5.9/test-requirements.txt` & `bowtie_json_schema-2023.6.1/test-requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -24,39 +24,50 @@
 cffi==1.15.1
     # via cryptography
 charset-normalizer==3.1.0
     # via
     #   aiohttp
     #   requests
 click==8.1.3
-    # via bowtie-json-schema
+    # via
+    #   bowtie-json-schema
+    #   trogon
 cryptography==40.0.2
     # via pyjwt
 frozenlist==1.3.3
     # via
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
     # via bowtie-json-schema
 icdiff==2.0.6
     # via pytest-icdiff
 idna==3.4
     # via
     #   requests
     #   yarl
+importlib-metadata==6.6.0
+    # via textual
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via bowtie-json-schema
 jsonschema==4.17.3
     # via bowtie-json-schema
-markdown-it-py==2.2.0
-    # via rich
+linkify-it-py==2.0.2
+    # via markdown-it-py
+markdown-it-py[linkify,plugins]==2.2.0
+    # via
+    #   mdit-py-plugins
+    #   rich
+    #   textual
 markupsafe==2.1.2
     # via jinja2
+mdit-py-plugins==0.3.5
+    # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 packaging==23.1
@@ -80,23 +91,35 @@
     #   pytest-icdiff
 pytest-asyncio==0.21.0
     # via -r test-requirements.in
 pytest-icdiff==0.6
     # via -r test-requirements.in
 python-dateutil==2.8.2
     # via github3-py
-requests==2.30.0
+requests==2.31.0
     # via github3-py
 rich==13.3.5
-    # via bowtie-json-schema
+    # via
+    #   bowtie-json-schema
+    #   textual
 six==1.16.0
     # via python-dateutil
 structlog==23.1.0
     # via bowtie-json-schema
-typing-extensions==4.5.0
-    # via aiodocker
+textual==0.26.0
+    # via trogon
+trogon==0.4.0
+    # via bowtie-json-schema
+typing-extensions==4.6.2
+    # via
+    #   aiodocker
+    #   textual
+uc-micro-py==1.0.2
+    # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
 urllib3==2.0.2
     # via requests
 yarl==1.9.2
     # via aiohttp
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `bowtie_json_schema-2023.5.9/.github/SECURITY.md` & `bowtie_json_schema-2023.6.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/.github/dependabot.yml` & `bowtie_json_schema-2023.6.1/.github/dependabot.yml`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,19 @@
       interval: "daily"
 
   - package-ecosystem: "cargo"
     directory: "implementations/rust-boon"
     schedule:
       interval: "daily"
 
+  - package-ecosystem: "gradle"
+    directory: "implementations/java-json-schema"
+    schedule:
+      interval: "daily"
+
   # Dependabot for Dockerfiles
   # --------------------------
 
   # See dependabot/dependabot-core#1015 or dependabot/dependabot-core#2178,
   # this doesn't happen automatically, so hooray, manual list.
 
   - package-ecosystem: "docker"
@@ -136,14 +141,19 @@
 
   - package-ecosystem: "docker"
     directory: "/implementations/rust-boon"
     schedule:
       interval: "daily"
 
   - package-ecosystem: "docker"
+    directory: "/implementations/java-json-schema"
+    schedule:
+      interval: "daily"
+
+  - package-ecosystem: "docker"
     directory: "/tests/fauxmplementations/badsonschema"
     schedule:
       interval: "daily"
 
   - package-ecosystem: "docker"
     directory: "/tests/fauxmplementations/envsonschema"
     schedule:
```

### Comparing `bowtie_json_schema-2023.5.9/.github/workflows/ci.yml` & `bowtie_json_schema-2023.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.6.1/.github/workflows/dependabot-merge.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 jobs:
   dependabot:
     runs-on: ubuntu-latest
     if: ${{ github.actor == 'dependabot[bot]' }}
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.4.0
+        uses: dependabot/fetch-metadata@v1.5.1
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
       - name: Enable auto-merge for Dependabot PRs
         run: gh pr merge --auto --merge "$PR_URL"
         env:
           PR_URL: ${{ github.event.pull_request.html_url }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `bowtie_json_schema-2023.5.9/.github/workflows/images.yml` & `bowtie_json_schema-2023.6.1/.github/workflows/images.yml`

 * *Files 0% similar despite different names*

```diff
@@ -83,13 +83,13 @@
           tags: ${{ steps.build_image.outputs.tags }}
           registry: ghcr.io/${{ github.repository_owner }}
           username: ${{ github.actor }}
           password: ${{ github.token }}
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
 
       - name: Install Bowtie
-        uses: bowtie-json-schema/bowtie@v2023.05.8
+        uses: bowtie-json-schema/bowtie@v2023.05.14
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
 
       - name: Smoke Test
         run: bowtie smoke -i "${{ steps.build_image.outputs.image-with-tag }}"
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
```

### Comparing `bowtie_json_schema-2023.5.9/.github/workflows/report.yml` & `bowtie_json_schema-2023.6.1/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/bowtie/_cli.py` & `bowtie_json_schema-2023.6.1/bowtie/_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import sys
 import zipfile
 
 from attrs import asdict
 from rich import box, console, panel
 from rich.table import Column, Table
 from rich.text import Text
+from trogon import tui  # type: ignore[reportMissingTypeStubs]
 import aiodocker
 import click
 import jinja2
 import structlog
 import structlog.typing
 
 from bowtie import _report
@@ -83,14 +84,15 @@
     help="What format to use for the output",
     default=lambda: "pretty" if sys.stdout.isatty() else "json",
     show_default="pretty if stdout is a tty, otherwise JSON",
     type=click.Choice(["json", "pretty"]),
 )
 
 
+@tui()
 @click.group(context_settings=dict(help_option_names=["--help", "-h"]))
 @click.version_option(prog_name="bowtie", package_name="bowtie-json-schema")
 def main():
     """
     A meta-validator for the JSON Schema specifications.
     """
     redirect_structlog()
```

### Comparing `bowtie_json_schema-2023.5.9/bowtie/_commands.py` & `bowtie_json_schema-2023.6.1/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/bowtie/_core.py` & `bowtie_json_schema-2023.6.1/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/bowtie/_report.py` & `bowtie_json_schema-2023.6.1/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/bowtie/exceptions.py` & `bowtie_json_schema-2023.6.1/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/docs/Makefile` & `bowtie_json_schema-2023.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/docs/cli.rst` & `bowtie_json_schema-2023.6.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/docs/conf.py` & `bowtie_json_schema-2023.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/docs/contributing.rst` & `bowtie_json_schema-2023.6.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/docs/implementers.rst` & `bowtie_json_schema-2023.6.1/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/docs/index.rst` & `bowtie_json_schema-2023.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/docs/requirements.txt` & `bowtie_json_schema-2023.6.1/docs/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -33,56 +33,66 @@
     # via
     #   aiohttp
     #   requests
 click==8.1.3
     # via
     #   bowtie-json-schema
     #   sphinx-click
+    #   trogon
 contourpy==1.0.7
     # via matplotlib
 cryptography==40.0.2
     # via pyjwt
 cycler==0.11.0
     # via matplotlib
-docutils==0.19
+docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-click
 fonttools==4.39.4
     # via matplotlib
 frozenlist==1.3.3
     # via
     #   aiohttp
     #   aiosignal
-furo==2023.3.27
+furo==2023.5.20
     # via -r docs/requirements.in
 github3-py==4.0.1
     # via bowtie-json-schema
 idna==3.4
     # via
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
+importlib-metadata==6.6.0
+    # via textual
 jinja2==3.1.2
     # via
     #   bowtie-json-schema
     #   sphinx
 jsonschema==4.17.3
     # via bowtie-json-schema
 kiwisolver==1.4.4
     # via matplotlib
+linkify-it-py==2.0.2
+    # via markdown-it-py
 lxml==4.9.2
     # via sphinx-json-schema-spec
-markdown-it-py==2.2.0
-    # via rich
+markdown-it-py[linkify,plugins]==2.2.0
+    # via
+    #   mdit-py-plugins
+    #   rich
+    #   textual
 markupsafe==2.1.2
     # via jinja2
 matplotlib==3.7.1
     # via sphinxext-opengraph
+mdit-py-plugins==0.3.5
+    # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 numpy==1.24.3
@@ -113,27 +123,29 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   github3-py
     #   matplotlib
-requests==2.30.0
+requests==2.31.0
     # via
     #   github3-py
     #   sphinx
 rich==13.3.5
-    # via bowtie-json-schema
+    # via
+    #   bowtie-json-schema
+    #   textual
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==6.2.1
+sphinx==7.0.1
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
@@ -141,15 +153,15 @@
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b1
     # via furo
 sphinx-click==4.4.0
     # via -r docs/requirements.in
 sphinx-copybutton==0.5.2
     # via -r docs/requirements.in
-sphinx-json-schema-spec==2023.5.2
+sphinx-json-schema-spec==2023.5.3
     # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -161,17 +173,27 @@
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
 sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
 structlog==23.1.0
     # via bowtie-json-schema
-typing-extensions==4.5.0
-    # via aiodocker
+textual==0.26.0
+    # via trogon
+trogon==0.4.0
+    # via bowtie-json-schema
+typing-extensions==4.6.2
+    # via
+    #   aiodocker
+    #   textual
+uc-micro-py==1.0.2
+    # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
 urllib3==2.0.2
     # via requests
 yarl==1.9.2
     # via
     #   -r docs/requirements.in
     #   aiohttp
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `bowtie_json_schema-2023.5.9/docs/_static/dreamed.png` & `bowtie_json_schema-2023.6.1/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/tests/test_integration.py` & `bowtie_json_schema-2023.6.1/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             elif "case" in each:
                 cases.append(each)
             elif "did_fail_fast" in each:
                 continue
             else:
                 errors.append(each)
 
-        assert errors if expecting_errors else not errors, errors
+        assert errors if expecting_errors else not errors, pformat(errors)
         return proc.returncode, successful, errors, cases, stderr
 
     yield _send
 
 
 @pytest.mark.asyncio
 async def test_validating_on_both_sides(lintsonschema):
```

### Comparing `bowtie_json_schema-2023.5.9/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.6.1/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.6.1/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.6.1/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.6.1/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.6.1/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/.gitignore` & `bowtie_json_schema-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/LICENSE` & `bowtie_json_schema-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/README.rst` & `bowtie_json_schema-2023.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.9/pyproject.toml` & `bowtie_json_schema-2023.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
   "attrs>=22.2.0",
   "click",
   "github3.py",
   "jinja2",
   "jsonschema",
   "rich",
   "structlog",
+  "trogon>=0.4.0",
   "importlib-resources; python_version<'3.9'",
   "typing-extensions; python_version<'3.11'",
 ]
 
 [project.scripts]
 bowtie = "bowtie._cli:main"
```

### Comparing `bowtie_json_schema-2023.5.9/PKG-INFO` & `bowtie_json_schema-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.5.9
+Version: 2023.6.1
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
@@ -29,14 +29,15 @@
 Requires-Dist: click
 Requires-Dist: github3-py
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: jinja2
 Requires-Dist: jsonschema
 Requires-Dist: rich
 Requires-Dist: structlog
+Requires-Dist: trogon>=0.4.0
 Requires-Dist: typing-extensions; python_version < '3.11'
 Description-Content-Type: text/x-rst
 
 ======
 Bowtie
 ======
```

