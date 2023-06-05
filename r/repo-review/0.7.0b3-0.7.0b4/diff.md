# Comparing `tmp/repo_review-0.7.0b3.tar.gz` & `tmp/repo_review-0.7.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jun  5 19:10:05 2023, max compression
+gzip compressed data, last modified: Mon Jun  5 21:02:57 2023, max compression
```

## Comparing `repo_review-0.7.0b3.tar` & `repo_review-0.7.0b4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2061 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      399 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.readthedocs.yml
--rw-r--r--   0        0        0     2293 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2544 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/matchers/pylint.json
--rw-r--r--   0        0        0      630 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1524 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/.nojekyll
--rw-r--r--   0        0        0     3355 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/checks.md
--rw-r--r--   0        0        0      694 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/cli.md
--rw-r--r--   0        0        0      277 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/families.md
--rw-r--r--   0        0        0     2023 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/fixtures.md
--rw-r--r--   0        0        0     1778 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/index.html
--rw-r--r--   0        0        0      151 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/index.md
--rw-r--r--   0        0        0     9739 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/webapp.js
--rw-r--r--   0        0        0      222 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/__init__.py
--rw-r--r--   0        0        0     6945 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/__main__.py
--rw-r--r--   0        0        0     1311 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/checks.py
--rw-r--r--   0        0        0      494 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/families.py
--rw-r--r--   0        0        0     2004 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     3412 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     4669 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_checks.py
--rw-r--r--   0        0        0      450 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_package.py
--rw-r--r--   0        0        0     1921 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_self.py
--rw-r--r--   0        0        0     3981 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/LICENSE
--rw-r--r--   0        0        0     4667 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/README.md
--rw-r--r--   0        0        0     4520 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/pyproject.toml
--rw-r--r--   0        0        0     7975 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/PKG-INFO
+-rw-r--r--   0        0        0     2061 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      399 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.readthedocs.yml
+-rw-r--r--   0        0        0     2293 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2544 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      630 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1524 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/.nojekyll
+-rw-r--r--   0        0        0     3355 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/checks.md
+-rw-r--r--   0        0        0      694 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/cli.md
+-rw-r--r--   0        0        0      277 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/families.md
+-rw-r--r--   0        0        0     2023 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/fixtures.md
+-rw-r--r--   0        0        0     1778 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/index.html
+-rw-r--r--   0        0        0      151 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/index.md
+-rw-r--r--   0        0        0     9739 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/webapp.js
+-rw-r--r--   0        0        0      222 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     6945 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/__main__.py
+-rw-r--r--   0        0        0     1311 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/checks.py
+-rw-r--r--   0        0        0      494 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/families.py
+-rw-r--r--   0        0        0     2004 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     3412 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     4739 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_checks.py
+-rw-r--r--   0        0        0      450 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_package.py
+-rw-r--r--   0        0        0     1921 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_self.py
+-rw-r--r--   0        0        0     3981 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/LICENSE
+-rw-r--r--   0        0        0     4667 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/README.md
+-rw-r--r--   0        0        0     4520 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/pyproject.toml
+-rw-r--r--   0        0        0     7975 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/PKG-INFO
```

### Comparing `repo_review-0.7.0b3/.pre-commit-config.yaml` & `repo_review-0.7.0b4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/noxfile.py` & `repo_review-0.7.0b4/noxfile.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/.github/CONTRIBUTING.md` & `repo_review-0.7.0b4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/.github/matchers/pylint.json` & `repo_review-0.7.0b4/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/.github/workflows/cd.yml` & `repo_review-0.7.0b4/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/.github/workflows/ci.yml` & `repo_review-0.7.0b4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/docs/checks.md` & `repo_review-0.7.0b4/docs/checks.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/docs/cli.md` & `repo_review-0.7.0b4/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/docs/families.md` & `repo_review-0.7.0b4/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/docs/fixtures.md` & `repo_review-0.7.0b4/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/docs/index.html` & `repo_review-0.7.0b4/docs/index.html`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/docs/webapp.js` & `repo_review-0.7.0b4/docs/webapp.js`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/src/repo_review/__main__.py` & `repo_review-0.7.0b4/src/repo_review/__main__.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/src/repo_review/checks.py` & `repo_review-0.7.0b4/src/repo_review/checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/src/repo_review/fixtures.py` & `repo_review-0.7.0b4/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/src/repo_review/ghpath.py` & `repo_review-0.7.0b4/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/src/repo_review/processor.py` & `repo_review-0.7.0b4/src/repo_review/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,18 +144,18 @@
         if not is_allowed(select_checks, skip_checks, task_name):
             continue
 
         result_list.append(
             Result(
                 family=check.family,
                 name=task_name,
-                description=doc,
+                description=doc.format(self=check, name=task_name),
                 result=result,
                 err_msg=textwrap.dedent(err_msg.format(self=check, name=task_name)),
-                url=getattr(check, "url", ""),
+                url=getattr(check, "url", "").format(self=check, name=task_name),
             )
         )
 
     return ProcessReturn(families, result_list)
 
 
 def as_simple_dict(results: list[Result]) -> dict[str, ResultDict]:
```

### Comparing `repo_review-0.7.0b3/tests/test_checks.py` & `repo_review-0.7.0b4/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/tests/test_fixtures.py` & `repo_review-0.7.0b4/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/tests/test_package.py` & `repo_review-0.7.0b4/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/tests/test_self.py` & `repo_review-0.7.0b4/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/tests/test_utilities/pyproject.py` & `repo_review-0.7.0b4/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/.gitignore` & `repo_review-0.7.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/LICENSE` & `repo_review-0.7.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/README.md` & `repo_review-0.7.0b4/README.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/pyproject.toml` & `repo_review-0.7.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b3/PKG-INFO` & `repo_review-0.7.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b3
+Version: 0.7.0b4
 Summary: Framework that can run checks on repos
 Project-URL: homepage, https://github.com/scientific-python/repo-review
 Project-URL: webpage, https://scientific-python.github.io/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Henry Schreiner.
```

