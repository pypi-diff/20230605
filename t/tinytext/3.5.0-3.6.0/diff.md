# Comparing `tmp/tinytext-3.5.0.tar.gz` & `tmp/tinytext-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Apr 14 11:07:39 2023, max compression
+gzip compressed data, last modified: Sun Jun  4 18:38:52 2023, max compression
```

## Comparing `tinytext-3.5.0.tar` & `tinytext-3.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      329 2023-04-14 11:07:39.000000 tinytext-3.5.0/.coveragerc
--rw-r--r--   0        0        0       30 2023-04-14 11:07:39.000000 tinytext-3.5.0/.flake8
--rw-r--r--   0        0        0     1671 2023-04-14 11:07:39.000000 tinytext-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      505 2023-04-14 11:07:39.000000 tinytext-3.5.0/.zenodo.json
--rw-r--r--   0        0        0      821 2023-04-14 11:07:39.000000 tinytext-3.5.0/RELEASING.md
--rw-r--r--   0        0        0       34 2023-04-14 11:07:39.000000 tinytext-3.5.0/codecov.yml
--rw-r--r--   0        0        0       77 2023-04-14 11:07:39.000000 tinytext-3.5.0/requirements.txt
--rw-r--r--   0        0        0      502 2023-04-14 11:07:39.000000 tinytext-3.5.0/tox.ini
--rw-r--r--   0        0        0     1785 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/labels.yml
--rw-r--r--   0        0        0      900 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      443 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/renovate.json
--rw-r--r--   0        0        0     1755 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1148 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     2045 2023-04-14 11:07:39.000000 tinytext-3.5.0/src/tinytext/__init__.py
--rw-r--r--   0        0        0      104 2023-04-14 11:07:39.000000 tinytext-3.5.0/src/tinytext/__main__.py
--rw-r--r--   0        0        0      494 2023-04-14 11:07:39.000000 tinytext-3.5.0/src/tinytext/cli.py
--rw-r--r--   0        0        0        0 2023-04-14 11:07:39.000000 tinytext-3.5.0/tests/__init__.py
--rw-r--r--   0        0        0      241 2023-04-14 11:07:39.000000 tinytext-3.5.0/tests/test_tinytext.py
--rw-r--r--   0        0        0     3077 2023-04-14 11:07:39.000000 tinytext-3.5.0/.gitignore
--rw-r--r--   0        0        0     1079 2023-04-14 11:07:39.000000 tinytext-3.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1475 2023-04-14 11:07:39.000000 tinytext-3.5.0/README.md
--rw-r--r--   0        0        0     1668 2023-04-14 11:07:39.000000 tinytext-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-04-14 11:07:39.000000 tinytext-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0      329 2023-06-04 18:38:52.000000 tinytext-3.6.0/.coveragerc
+-rw-r--r--   0        0        0       30 2023-06-04 18:38:52.000000 tinytext-3.6.0/.flake8
+-rw-r--r--   0        0        0     1681 2023-06-04 18:38:52.000000 tinytext-3.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      505 2023-06-04 18:38:52.000000 tinytext-3.6.0/.zenodo.json
+-rw-r--r--   0        0        0      821 2023-06-04 18:38:52.000000 tinytext-3.6.0/RELEASING.md
+-rw-r--r--   0        0        0       34 2023-06-04 18:38:52.000000 tinytext-3.6.0/codecov.yml
+-rw-r--r--   0        0        0       77 2023-06-04 18:38:52.000000 tinytext-3.6.0/requirements.txt
+-rw-r--r--   0        0        0      498 2023-06-04 18:38:52.000000 tinytext-3.6.0/tox.ini
+-rw-r--r--   0        0        0     1785 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/labels.yml
+-rw-r--r--   0        0        0      900 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      443 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1171 2023-06-04 18:38:52.000000 tinytext-3.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1887 2023-06-04 18:38:52.000000 tinytext-3.6.0/src/tinytext/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-04 18:38:52.000000 tinytext-3.6.0/src/tinytext/__main__.py
+-rw-r--r--   0        0        0      494 2023-06-04 18:38:52.000000 tinytext-3.6.0/src/tinytext/cli.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:38:52.000000 tinytext-3.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      241 2023-06-04 18:38:52.000000 tinytext-3.6.0/tests/test_tinytext.py
+-rw-r--r--   0        0        0     3077 2023-06-04 18:38:52.000000 tinytext-3.6.0/.gitignore
+-rw-r--r--   0        0        0     1079 2023-06-04 18:38:52.000000 tinytext-3.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1475 2023-06-04 18:38:52.000000 tinytext-3.6.0/README.md
+-rw-r--r--   0        0        0     1539 2023-06-04 18:38:52.000000 tinytext-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2845 2023-06-04 18:38:52.000000 tinytext-3.6.0/PKG-INFO
```

### Comparing `tinytext-3.5.0/.pre-commit-config.yaml` & `tinytext-3.6.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
@@ -37,35 +37,35 @@
       - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         args: [--strict, --pretty, --show-error-codes]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.9.2
+    rev: 0.10.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `tinytext-3.5.0/RELEASING.md` & `tinytext-3.6.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/.github/labels.yml` & `tinytext-3.6.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/.github/release-drafter.yml` & `tinytext-3.6.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/.github/workflows/deploy.yml` & `tinytext-3.6.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/.github/workflows/release-drafter.yml` & `tinytext-3.6.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/.github/workflows/test.yml` & `tinytext-3.6.0/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.9", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy3.9", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
```

### Comparing `tinytext-3.5.0/src/tinytext/__init__.py` & `tinytext-3.6.0/src/tinytext/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import annotations
 
-try:
-    # Python 3.8+
-    import importlib.metadata as importlib_metadata
-except ImportError:
-    # Python 3.7 and lower
-    import importlib_metadata  # type: ignore
+import importlib.metadata
 
-__version__ = importlib_metadata.version(__name__)
+__version__ = importlib.metadata.version(__name__)
 
 
 __all__ = ["__version__"]
 
 tiny_letters: dict[int, str] = {
     ord("a"): "ᵃ",
     ord("b"): "ᵇ",
@@ -91,10 +86,7 @@
 }
 
 
 def tinytext(big: str) -> str:
     """convert your text ᶦᶰᵗᵒ ᵗᶦᶰᶦᵉʳ ᵗᵉˣᵗ"""
     tiny: str = big.translate(tiny_letters)
     return tiny
-
-
-# End of file
```

### Comparing `tinytext-3.5.0/.gitignore` & `tinytext-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/LICENSE.txt` & `tinytext-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/README.md` & `tinytext-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tinytext-3.5.0/pyproject.toml` & `tinytext-3.6.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -14,39 +14,35 @@
   "cute text",
   "generator",
   "tiny text",
   "tiny type",
 ]
 license = {text = "MIT"}
 authors = [{name = "Hugo van Kemenade"}]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-    "Topic :: Artistic Software",
-    "Topic :: Text Processing",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "Topic :: Artistic Software",
+  "Topic :: Text Processing",
 ]
 dynamic = [
   "version",
 ]
-dependencies = [
-  'importlib-metadata; python_version < "3.8"',
-]
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-cov",
 ]
 [project.urls]
 Changelog = "https://github.com/hugovk/tinytext/releases"
```

### Comparing `tinytext-3.5.0/PKG-INFO` & `tinytext-3.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: tinytext
-Version: 3.5.0
+Version: 3.6.0
 Summary: A helpful converter to change any normal text into cuter tinier text
 Project-URL: Changelog, https://github.com/hugovk/tinytext/releases
 Project-URL: Homepage, https://github.com/hugovk/tinytext
 Project-URL: Source, https://github.com/hugovk/tinytext
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
 Keywords: botally,cute text,generator,tiny text,tiny type
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.7
-Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Python: >=3.8
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # tinytext
```

