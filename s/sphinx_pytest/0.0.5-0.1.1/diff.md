# Comparing `tmp/sphinx_pytest-0.0.5.tar.gz` & `tmp/sphinx_pytest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_pytest-0.0.5.tar", last modified: Sun Sep 11 15:16:16 2022, max compression
+gzip compressed data, was "sphinx_pytest-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_pytest-0.0.5.tar` & `sphinx_pytest-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      953 2022-05-10 13:09:32.533866 sphinx_pytest-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1809 2022-05-09 20:42:44.936351 sphinx_pytest-0.0.5/.gitignore
--rw-r--r--   0        0        0     1003 2022-09-11 14:55:44.404224 sphinx_pytest-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      331 2022-05-09 21:39:19.672996 sphinx_pytest-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0     1069 2022-05-09 20:13:26.310373 sphinx_pytest-0.0.5/LICENSE
--rw-r--r--   0        0        0     1588 2022-05-10 13:37:36.828246 sphinx_pytest-0.0.5/README.md
--rw-r--r--   0        0        0     1074 2022-09-11 14:59:01.587221 sphinx_pytest-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       76 2022-09-11 15:08:51.021921 sphinx_pytest-0.0.5/src/sphinx_pytest/__init__.py
--rw-r--r--   0        0        0     1015 2022-09-11 15:08:11.230786 sphinx_pytest-0.0.5/src/sphinx_pytest/builders.py
--rw-r--r--   0        0        0     4829 2022-06-24 03:17:04.952761 sphinx_pytest-0.0.5/src/sphinx_pytest/plugin.py
--rw-r--r--   0        0        0     1365 2022-06-24 03:26:14.509488 sphinx_pytest-0.0.5/tests/test_basic.py
--rw-r--r--   0        0        0      205 2022-05-09 20:24:26.053586 sphinx_pytest-0.0.5/tox.ini
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 sphinx_pytest-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      598 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1531 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1809 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1002 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      331 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1069 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1588 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/README.md
+-rw-r--r--   0        0        0     1074 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/src/sphinx_pytest/__init__.py
+-rw-r--r--   0        0        0     1053 2023-06-05 21:48:12.308064 sphinx_pytest-0.1.1/src/sphinx_pytest/builders.py
+-rw-r--r--   0        0        0     4829 2023-06-05 21:48:12.312064 sphinx_pytest-0.1.1/src/sphinx_pytest/plugin.py
+-rw-r--r--   0        0        0     1365 2023-06-05 21:48:12.312064 sphinx_pytest-0.1.1/tests/test_basic.py
+-rw-r--r--   0        0        0      205 2023-06-05 21:48:12.312064 sphinx_pytest-0.1.1/tox.ini
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 sphinx_pytest-0.1.1/PKG-INFO
```

### Comparing `sphinx_pytest-0.0.5/.gitignore` & `sphinx_pytest-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_pytest-0.0.5/.pre-commit-config.yaml` & `sphinx_pytest-0.1.1/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
     - id: trailing-whitespace
     - id: end-of-file-fixer
     - id: check-yaml
     - id: check-added-large-files
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.37.3
+    rev: v3.4.0
     hooks:
     - id: pyupgrade
       args: [--py37-plus]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
     - id: black
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.2
+    rev: 6.0.0
     hooks:
     - id: flake8
       additional_dependencies:
         - flake8-comprehensions
         - flake8-bugbear
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.971
+    rev: v1.3.0
     hooks:
     - id: mypy
       args: [--config-file=pyproject.toml]
       additional_dependencies:
       - types-docutils
       - sphinx~=4.1
       - pytest
```

### Comparing `sphinx_pytest-0.0.5/LICENSE` & `sphinx_pytest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_pytest-0.0.5/README.md` & `sphinx_pytest-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_pytest-0.0.5/pyproject.toml` & `sphinx_pytest-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_pytest-0.0.5/src/sphinx_pytest/builders.py` & `sphinx_pytest-0.1.1/src/sphinx_pytest/builders.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     """
 
     name = "doctree"
 
     def init(self) -> None:
         self.doctrees: dict[str, nodes.document] = {}
 
-    def write_doctree(self, docname: str, doctree: nodes.document) -> None:
+    def write_doctree(
+        self, docname: str, doctree: nodes.document, *, _cache: bool = True
+    ) -> None:
         # save the doctree instead of pickling to disk
         self.doctrees[docname] = doctree
 
     def build(self, *args, **kwargs) -> None:
         # don't run anything after the initial doctree reads
         self.read()
```

### Comparing `sphinx_pytest-0.0.5/src/sphinx_pytest/plugin.py` & `sphinx_pytest-0.1.1/src/sphinx_pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `sphinx_pytest-0.0.5/tests/test_basic.py` & `sphinx_pytest-0.1.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `sphinx_pytest-0.0.5/PKG-INFO` & `sphinx_pytest-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_pytest
-Version: 0.0.5
+Version: 0.1.1
 Summary: Helpful pytest fixtures for sphinx extensions.
 Keywords: sphinx,pytest
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

