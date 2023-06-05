# Comparing `tmp/repo_review-0.7.0b2.tar.gz` & `tmp/repo_review-0.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jun  4 00:22:47 2023, max compression
+gzip compressed data, last modified: Mon Jun  5 19:10:05 2023, max compression
```

## Comparing `repo_review-0.7.0b2.tar` & `repo_review-0.7.0b3.tar`

### file list

```diff
@@ -1,36 +1,43 @@
--rw-r--r--   0        0        0     2061 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1591 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2324 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      630 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1501 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/docs/.nojekyll
--rw-r--r--   0        0        0     1778 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/docs/index.html
--rw-r--r--   0        0        0     9739 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/docs/webapp.js
--rw-r--r--   0        0        0      222 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/__init__.py
--rw-r--r--   0        0        0     5329 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/__main__.py
--rw-r--r--   0        0        0     1021 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/checks.py
--rw-r--r--   0        0        0     1014 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/families.py
--rw-r--r--   0        0        0     2004 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     3412 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     4241 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     3734 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_checks.py
--rw-r--r--   0        0        0      450 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_package.py
--rw-r--r--   0        0        0     1921 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_self.py
--rw-r--r--   0        0        0     3886 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0       15 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/LICENSE
--rw-r--r--   0        0        0     3758 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/README.md
--rw-r--r--   0        0        0     4314 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/pyproject.toml
--rw-r--r--   0        0        0     6779 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/PKG-INFO
+-rw-r--r--   0        0        0     2061 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      399 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.readthedocs.yml
+-rw-r--r--   0        0        0     2293 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2544 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      630 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1524 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/.nojekyll
+-rw-r--r--   0        0        0     3355 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/checks.md
+-rw-r--r--   0        0        0      694 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/cli.md
+-rw-r--r--   0        0        0      277 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/families.md
+-rw-r--r--   0        0        0     2023 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/fixtures.md
+-rw-r--r--   0        0        0     1778 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/index.html
+-rw-r--r--   0        0        0      151 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/index.md
+-rw-r--r--   0        0        0     9739 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/docs/webapp.js
+-rw-r--r--   0        0        0      222 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     6945 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/__main__.py
+-rw-r--r--   0        0        0     1311 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/checks.py
+-rw-r--r--   0        0        0      494 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/families.py
+-rw-r--r--   0        0        0     2004 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     3412 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     4669 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_checks.py
+-rw-r--r--   0        0        0      450 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_package.py
+-rw-r--r--   0        0        0     1921 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_self.py
+-rw-r--r--   0        0        0     3981 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/LICENSE
+-rw-r--r--   0        0        0     4667 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/README.md
+-rw-r--r--   0        0        0     4520 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/pyproject.toml
+-rw-r--r--   0        0        0     7975 2023-06-05 19:10:05.000000 repo_review-0.7.0b3/PKG-INFO
```

### Comparing `repo_review-0.7.0b2/.pre-commit-config.yaml` & `repo_review-0.7.0b3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/noxfile.py` & `repo_review-0.7.0b3/noxfile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
+import argparse
 import shutil
 from pathlib import Path
 
 import nox
 
 DIR = Path(__file__).parent.resolve()
 
 nox.options.sessions = ["lint", "pylint", "tests"]
 
 
 @nox.session(reuse_venv=True)
 def run(session: nox.Session) -> None:
     """
-    Run the program.
+    Run the program with a few example checks.
     """
 
     session.install("-e", ".[cli]")
+    session.install("-e", "tests/test_utilities")
     session.run("python", "-m", "repo_review", *session.posargs)
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
     """
     Run the linter.
@@ -65,10 +67,29 @@
 
 @nox.session(venv_backend="none")
 def serve(session: nox.Session) -> None:
     """
     Serve the webapp.
     """
 
-    session.cd("docs")
+    session.cd("webapp")
     session.log("Serving on http://localhost:8080")
     session.run("python3", "-m", "http.server", "8080")
+
+
+@nox.session(reuse_venv=True)
+def docs(session: nox.Session) -> None:
+    """
+    Build the docs. Pass "--serve" to serve.
+    """
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--serve", action="store_true", help="Serve after building")
+    args = parser.parse_args(session.posargs)
+
+    session.install(".[docs]")
+    session.chdir("docs")
+    session.run("sphinx-build", "-M", "html", ".", "_build")
+
+    if args.serve:
+        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
+        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
```

### Comparing `repo_review-0.7.0b2/.github/CONTRIBUTING.md` & `repo_review-0.7.0b3/.github/CONTRIBUTING.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 See the [Scientific-Python Development Pages][] for a
 detailed description of best practices for developing Scikit-HEP packages.
 
 [scientific-python development pages]: https://learn.scientific-python.org/development
 
-# Quick development
+## Quick development
 
 The fastest way to start with development is to use nox. If you don't have nox,
 you can use `pipx run nox` to run it without installing, or `pipx install nox`.
 If you don't have pipx (pip for applications), then you can install with with
 `pip install pipx` (the only case were installing an application with regular
 pip is reasonable). If you use macOS, then pipx and nox are both in brew, use
 `brew install pipx nox`.
@@ -22,15 +22,17 @@
 $ nox -s docs -- serve  # Build and serve the docs
 $ nox -s build  # Make an SDist and wheel
 ```
 
 Nox handles everything for you, including setting up an temporary virtual
 environment for each run.
 
-# Setting up a development environment manually
+You can also use `nox -s run -- .` to run an example set of checks on a repo.
+
+## Setting up a development environment manually
 
 You can set up a development environment by running:
 
 ```bash
 python3 -m venv .venv
 source ./.venv/bin/activate
 pip install -v -e .[dev]
@@ -52,40 +54,45 @@
 ```bash
 pip install pre-commit # or brew install pre-commit on macOS
 pre-commit install # Will install a pre-commit hook into the git repo
 ```
 
 You can also/alternatively run `pre-commit run` (changes only) or `pre-commit run --all-files` to check even without installing the hook.
 
-# Testing
+## Testing
 
 Use pytest to run the unit checks:
 
 ```bash
 pytest
 ```
 
-# Building docs
+## Building docs
 
 You can build the docs using:
 
 ```bash
 nox -s docs
 ```
 
 You can see a preview with:
 
 ```bash
 nox -s docs -- serve
 ```
 
-# Pre-commit
+## Pre-commit
 
 This project uses pre-commit for all style checking. While you can run it with
 nox, this is such an important tool that it deserves to be installed on its
 own. Install pre-commit and run:
 
 ```bash
 pre-commit run -a
 ```
 
 to check all files.
+
+## Running DevContainer
+
+You can use DevContainer, such as in GitHub Codespaces or locally. Nox and a
+local install will be available.
```

### Comparing `repo_review-0.7.0b2/.github/matchers/pylint.json` & `repo_review-0.7.0b3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/.github/workflows/cd.yml` & `repo_review-0.7.0b3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/.github/workflows/ci.yml` & `repo_review-0.7.0b3/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     types:
       - published
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
+env:
+  FORCE_COLOR: 3
+
 jobs:
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
```

### Comparing `repo_review-0.7.0b2/docs/index.html` & `repo_review-0.7.0b3/docs/index.html`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/docs/webapp.js` & `repo_review-0.7.0b3/docs/webapp.js`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/src/repo_review/__main__.py` & `repo_review-0.7.0b3/src/repo_review/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,334 +1,435 @@
 00000000: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
 00000010: 696d 706f 7274 2061 6e6e 6f74 6174 696f  import annotatio
 00000020: 6e73 0a0a 696d 706f 7274 2062 7569 6c74  ns..import built
 00000030: 696e 730a 696d 706f 7274 2066 756e 6374  ins.import funct
 00000040: 6f6f 6c73 0a69 6d70 6f72 7420 696f 0a69  ools.import io.i
 00000050: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
-00000060: 696d 706f 7274 206a 736f 6e0a 6672 6f6d  import json.from
-00000070: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-00000080: 2069 6d70 6f72 7420 4d61 7070 696e 670a   import Mapping.
-00000090: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
-000000a0: 6f72 7420 5061 7468 0a66 726f 6d20 7479  ort Path.from ty
-000000b0: 7069 6e67 2069 6d70 6f72 7420 4c69 7465  ping import Lite
-000000c0: 7261 6c0a 0a69 6d70 6f72 7420 636c 6963  ral..import clic
-000000d0: 6b0a 696d 706f 7274 206d 6172 6b64 6f77  k.import markdow
-000000e0: 6e5f 6974 0a69 6d70 6f72 7420 7269 6368  n_it.import rich
-000000f0: 2e63 6f6e 736f 6c65 0a69 6d70 6f72 7420  .console.import 
-00000100: 7269 6368 2e6d 6172 6b64 6f77 6e0a 696d  rich.markdown.im
-00000110: 706f 7274 2072 6963 682e 7465 726d 696e  port rich.termin
-00000120: 616c 5f74 6865 6d65 0a69 6d70 6f72 7420  al_theme.import 
-00000130: 7269 6368 2e74 6578 740a 696d 706f 7274  rich.text.import
-00000140: 2072 6963 682e 7472 6163 6562 6163 6b0a   rich.traceback.
-00000150: 696d 706f 7274 2072 6963 682e 7472 6565  import rich.tree
-00000160: 0a0a 6672 6f6d 202e 6661 6d69 6c69 6573  ..from .families
-00000170: 2069 6d70 6f72 7420 4661 6d69 6c79 0a66   import Family.f
-00000180: 726f 6d20 2e67 6870 6174 6820 696d 706f  rom .ghpath impo
-00000190: 7274 2047 4850 6174 680a 6672 6f6d 202e  rt GHPath.from .
-000001a0: 7072 6f63 6573 736f 7220 696d 706f 7274  processor import
-000001b0: 2052 6573 756c 742c 2061 735f 7369 6d70   Result, as_simp
-000001c0: 6c65 5f64 6963 742c 2070 726f 6365 7373  le_dict, process
-000001d0: 0a0a 7269 6368 2e74 7261 6365 6261 636b  ..rich.traceback
-000001e0: 2e69 6e73 7461 6c6c 2873 7570 7072 6573  .install(suppres
-000001f0: 733d 5b63 6c69 636b 2c20 7269 6368 5d2c  s=[click, rich],
-00000200: 2073 686f 775f 6c6f 6361 6c73 3d54 7275   show_locals=Tru
-00000210: 652c 2077 6964 7468 3d4e 6f6e 6529 0a0a  e, width=None)..
-00000220: 2320 5573 6520 6d6f 6475 6c65 2d6c 6576  # Use module-lev
-00000230: 656c 2065 6e74 7279 206e 616d 6573 0a23  el entry names.#
-00000240: 2072 6570 6f5f 7265 7669 6577 5f66 6978   repo_review_fix
-00000250: 7475 7265 7320 3d20 7b22 7079 7072 6f6a  tures = {"pyproj
-00000260: 6563 7422 7d0a 2320 7265 706f 5f72 6576  ect"}.# repo_rev
-00000270: 6965 775f 6368 6563 6b73 203d 2073 6574  iew_checks = set
-00000280: 2870 2e5f 5f6e 616d 655f 5f5f 2066 6f72  (p.__name___ for
-00000290: 2070 2069 6e20 4765 6e65 7261 6c2e 5f5f   p in General.__
-000002a0: 7375 6263 6c61 7373 6573 5f5f 2829 290a  subclasses__()).
-000002b0: 0a0a 6465 6620 7269 6368 5f70 7269 6e74  ..def rich_print
-000002c0: 6572 280a 2020 2020 6661 6d69 6c69 6573  er(.    families
-000002d0: 3a20 4d61 7070 696e 675b 7374 722c 2046  : Mapping[str, F
-000002e0: 616d 696c 795d 2c20 7072 6f63 6573 7365  amily], processe
-000002f0: 643a 206c 6973 745b 5265 7375 6c74 5d2c  d: list[Result],
-00000300: 202a 2c20 6f75 7470 7574 3a20 5061 7468   *, output: Path
-00000310: 207c 204e 6f6e 650a 2920 2d3e 204e 6f6e   | None.) -> Non
-00000320: 653a 0a20 2020 2063 6f6e 736f 6c65 203d  e:.    console =
-00000330: 2072 6963 682e 636f 6e73 6f6c 652e 436f   rich.console.Co
-00000340: 6e73 6f6c 6528 7265 636f 7264 3d54 7275  nsole(record=Tru
-00000350: 6529 0a0a 2020 2020 666f 7220 6661 6d69  e)..    for fami
-00000360: 6c79 2c20 7265 7375 6c74 735f 6c69 7374  ly, results_list
-00000370: 2069 6e20 6974 6572 746f 6f6c 732e 6772   in itertools.gr
-00000380: 6f75 7062 7928 7072 6f63 6573 7365 642c  oupby(processed,
-00000390: 206c 616d 6264 6120 723a 2072 2e66 616d   lambda r: r.fam
-000003a0: 696c 7929 3a0a 2020 2020 2020 2020 6661  ily):.        fa
-000003b0: 6d69 6c79 5f6e 616d 6520 3d20 6661 6d69  mily_name = fami
-000003c0: 6c69 6573 5b66 616d 696c 795d 2e67 6574  lies[family].get
-000003d0: 2822 6e61 6d65 222c 2066 616d 696c 7929  ("name", family)
-000003e0: 0a20 2020 2020 2020 2074 7265 6520 3d20  .        tree = 
-000003f0: 7269 6368 2e74 7265 652e 5472 6565 2866  rich.tree.Tree(f
-00000400: 225b 626f 6c64 5d7b 6661 6d69 6c79 5f6e  "[bold]{family_n
-00000410: 616d 657d 5b2f 626f 6c64 5d3a 2229 0a20  ame}[/bold]:"). 
-00000420: 2020 2020 2020 2066 6f72 2072 6573 756c         for resul
-00000430: 7420 696e 2072 6573 756c 7473 5f6c 6973  t in results_lis
-00000440: 743a 0a20 2020 2020 2020 2020 2020 206d  t:.            m
-00000450: 7367 203d 2072 6963 682e 7465 7874 2e54  sg = rich.text.T
-00000460: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
-00000470: 2020 6d73 672e 6170 7065 6e64 2872 6573    msg.append(res
-00000480: 756c 742e 6e61 6d65 2c20 7374 796c 653d  ult.name, style=
-00000490: 2262 6f6c 6422 290a 2020 2020 2020 2020  "bold").        
-000004a0: 2020 2020 6d73 672e 6170 7065 6e64 2822      msg.append("
-000004b0: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
-000004c0: 6966 2072 6573 756c 742e 7265 7375 6c74  if result.result
-000004d0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000004e0: 2020 2020 2020 2020 2020 6d73 672e 6170            msg.ap
-000004f0: 7065 6e64 2872 6573 756c 742e 6465 7363  pend(result.desc
-00000500: 7269 7074 696f 6e2c 2073 7479 6c65 3d22  ription, style="
-00000510: 7965 6c6c 6f77 2229 0a20 2020 2020 2020  yellow").       
-00000520: 2020 2020 2020 2020 206d 7367 2e61 7070           msg.app
-00000530: 656e 6428 2220 5b73 6b69 7070 6564 5d22  end(" [skipped]"
-00000540: 2c20 7374 796c 653d 2279 656c 6c6f 7720  , style="yellow 
-00000550: 626f 6c64 2229 0a20 2020 2020 2020 2020  bold").         
-00000560: 2020 2020 2020 2074 7265 652e 6164 6428         tree.add(
-00000570: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
-00000580: 2065 6c69 6620 7265 7375 6c74 2e72 6573   elif result.res
-00000590: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
-000005a0: 2020 2020 206d 7367 2e61 7070 656e 6428       msg.append(
-000005b0: 6622 7b72 6573 756c 742e 6465 7363 7269  f"{result.descri
-000005c0: 7074 696f 6e7d 3f20 222c 2073 7479 6c65  ption}? ", style
-000005d0: 3d22 6772 6565 6e22 290a 2020 2020 2020  ="green").      
-000005e0: 2020 2020 2020 2020 2020 6d73 672e 6170            msg.ap
-000005f0: 7065 6e64 2872 6963 682e 7465 7874 2e54  pend(rich.text.T
-00000600: 6578 742e 6672 6f6d 5f6d 6172 6b75 7028  ext.from_markup(
-00000610: 223a 7768 6974 655f 6368 6563 6b5f 6d61  ":white_check_ma
-00000620: 726b 3a22 2929 0a20 2020 2020 2020 2020  rk:")).         
-00000630: 2020 2020 2020 2074 7265 652e 6164 6428         tree.add(
-00000640: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
-00000650: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00000660: 2020 2020 2020 206d 7367 2e61 7070 656e         msg.appen
-00000670: 6428 6622 7b72 6573 756c 742e 6465 7363  d(f"{result.desc
-00000680: 7269 7074 696f 6e7d 3f20 222c 2073 7479  ription}? ", sty
-00000690: 6c65 3d22 7265 6422 290a 2020 2020 2020  le="red").      
-000006a0: 2020 2020 2020 2020 2020 6d73 672e 6170            msg.ap
-000006b0: 7065 6e64 2872 6963 682e 7465 7874 2e54  pend(rich.text.T
-000006c0: 6578 742e 6672 6f6d 5f6d 6172 6b75 7028  ext.from_markup(
-000006d0: 223a 783a 2229 290a 2020 2020 2020 2020  ":x:")).        
-000006e0: 2020 2020 2020 2020 6465 7461 696c 203d          detail =
-000006f0: 2072 6963 682e 6d61 726b 646f 776e 2e4d   rich.markdown.M
-00000700: 6172 6b64 6f77 6e28 7265 7375 6c74 2e65  arkdown(result.e
-00000710: 7272 5f6d 7367 290a 2020 2020 2020 2020  rr_msg).        
-00000720: 2020 2020 2020 2020 6d73 675f 6772 7020          msg_grp 
-00000730: 3d20 7269 6368 2e63 6f6e 736f 6c65 2e47  = rich.console.G
-00000740: 726f 7570 286d 7367 2c20 6465 7461 696c  roup(msg, detail
-00000750: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00000760: 2020 7472 6565 2e61 6464 286d 7367 5f67    tree.add(msg_g
-00000770: 7270 290a 0a20 2020 2020 2020 2063 6f6e  rp)..        con
-00000780: 736f 6c65 2e70 7269 6e74 2874 7265 6529  sole.print(tree)
-00000790: 0a20 2020 2020 2020 2063 6f6e 736f 6c65  .        console
-000007a0: 2e70 7269 6e74 2829 0a0a 2020 2020 6966  .print()..    if
-000007b0: 206f 7574 7075 7420 6973 206e 6f74 204e   output is not N
-000007c0: 6f6e 653a 0a20 2020 2020 2020 2063 6f6e  one:.        con
-000007d0: 736f 6c65 2e73 6176 655f 7376 6728 7374  sole.save_svg(st
-000007e0: 7228 6f75 7470 7574 292c 2074 6865 6d65  r(output), theme
-000007f0: 3d72 6963 682e 7465 726d 696e 616c 5f74  =rich.terminal_t
-00000800: 6865 6d65 2e44 4546 4155 4c54 5f54 4552  heme.DEFAULT_TER
-00000810: 4d49 4e41 4c5f 5448 454d 4529 0a0a 0a64  MINAL_THEME)...d
-00000820: 6566 2074 6f5f 6874 6d6c 2866 616d 696c  ef to_html(famil
-00000830: 6965 733a 204d 6170 7069 6e67 5b73 7472  ies: Mapping[str
-00000840: 2c20 4661 6d69 6c79 5d2c 2070 726f 6365  , Family], proce
-00000850: 7373 6564 3a20 6c69 7374 5b52 6573 756c  ssed: list[Resul
-00000860: 745d 2920 2d3e 2073 7472 3a0a 2020 2020  t]) -> str:.    
-00000870: 6f75 7420 3d20 696f 2e53 7472 696e 6749  out = io.StringI
-00000880: 4f28 290a 2020 2020 7072 696e 7420 3d20  O().    print = 
-00000890: 6675 6e63 746f 6f6c 732e 7061 7274 6961  functools.partia
-000008a0: 6c28 6275 696c 7469 6e73 2e70 7269 6e74  l(builtins.print
-000008b0: 2c20 6669 6c65 3d6f 7574 290a 2020 2020  , file=out).    
-000008c0: 6d64 203d 206d 6172 6b64 6f77 6e5f 6974  md = markdown_it
-000008d0: 2e4d 6172 6b64 6f77 6e49 7428 290a 0a20  .MarkdownIt().. 
-000008e0: 2020 2066 6f72 2066 616d 696c 792c 2072     for family, r
-000008f0: 6573 756c 7473 5f6c 6973 7420 696e 2069  esults_list in i
-00000900: 7465 7274 6f6f 6c73 2e67 726f 7570 6279  tertools.groupby
-00000910: 2870 726f 6365 7373 6564 2c20 6c61 6d62  (processed, lamb
-00000920: 6461 2072 3a20 722e 6661 6d69 6c79 293a  da r: r.family):
-00000930: 0a20 2020 2020 2020 2066 616d 696c 795f  .        family_
-00000940: 6e61 6d65 203d 2066 616d 696c 6965 735b  name = families[
-00000950: 6661 6d69 6c79 5d2e 6765 7428 226e 616d  family].get("nam
-00000960: 6522 2c20 6661 6d69 6c79 290a 2020 2020  e", family).    
-00000970: 2020 2020 7072 696e 7428 6622 3c68 323e      print(f"<h2>
-00000980: 7b66 616d 696c 795f 6e61 6d65 7d3c 2f68  {family_name}</h
-00000990: 323e 2229 0a20 2020 2020 2020 2070 7269  2>").        pri
-000009a0: 6e74 2822 3c74 6162 6c65 3e22 290a 2020  nt("<table>").  
-000009b0: 2020 2020 2020 7072 696e 7428 223c 7472        print("<tr
-000009c0: 3e3c 7468 3e52 6573 756c 743c 2f74 683e  ><th>Result</th>
-000009d0: 3c74 683e 4e61 6d65 3c2f 7468 3e3c 7468  <th>Name</th><th
-000009e0: 3e44 6573 6372 6970 7469 6f6e 3c2f 7468  >Description</th
-000009f0: 3e3c 2f74 723e 2229 0a20 2020 2020 2020  ></tr>").       
-00000a00: 2066 6f72 2072 6573 756c 7420 696e 2072   for result in r
-00000a10: 6573 756c 7473 5f6c 6973 743a 0a20 2020  esults_list:.   
-00000a20: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00000a30: 3c74 723e 2229 0a20 2020 2020 2020 2020  <tr>").         
-00000a40: 2020 2069 6620 7265 7375 6c74 2e72 6573     if result.res
-00000a50: 756c 7420 6973 204e 6f6e 653a 0a20 2020  ult is None:.   
-00000a60: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00000a70: 6e74 2822 3c74 643e 536b 6970 7065 643c  nt("<td>Skipped<
-00000a80: 2f74 643e 2229 0a20 2020 2020 2020 2020  /td>").         
-00000a90: 2020 2065 6c69 6620 7265 7375 6c74 2e72     elif result.r
-00000aa0: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
-00000ab0: 2020 2020 2020 2070 7269 6e74 2822 3c74         print("<t
-00000ac0: 643e 5061 7373 6564 3c2f 7464 3e22 290a  d>Passed</td>").
-00000ad0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00000ae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000af0: 2020 7072 696e 7428 223c 7464 3e46 6169    print("<td>Fai
-00000b00: 6c65 643c 2f74 643e 2229 0a20 2020 2020  led</td>").     
-00000b10: 2020 2020 2020 2070 7269 6e74 2866 223c         print(f"<
-00000b20: 7464 3e7b 7265 7375 6c74 2e6e 616d 657d  td>{result.name}
-00000b30: 3c2f 7464 3e22 290a 2020 2020 2020 2020  </td>").        
-00000b40: 2020 2020 6966 2072 6573 756c 742e 7265      if result.re
-00000b50: 7375 6c74 2069 7320 4e6f 6e65 206f 7220  sult is None or 
-00000b60: 7265 7375 6c74 2e72 6573 756c 743a 0a20  result.result:. 
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00000b80: 7269 6e74 2866 223c 7464 3e7b 7265 7375  rint(f"<td>{resu
-00000b90: 6c74 2e64 6573 6372 6970 7469 6f6e 7d3c  lt.description}<
-00000ba0: 2f74 643e 2229 0a20 2020 2020 2020 2020  /td>").         
-00000bb0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00000bc0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00000bd0: 3c74 643e 2229 0a20 2020 2020 2020 2020  <td>").         
-00000be0: 2020 2020 2020 2070 7269 6e74 2872 6573         print(res
-00000bf0: 756c 742e 6465 7363 7269 7074 696f 6e29  ult.description)
+00000060: 696d 706f 7274 206a 736f 6e0a 696d 706f  import json.impo
+00000070: 7274 2074 7970 696e 670a 6672 6f6d 2063  rt typing.from c
+00000080: 6f6c 6c65 6374 696f 6e73 2e61 6263 2069  ollections.abc i
+00000090: 6d70 6f72 7420 4d61 7070 696e 670a 6672  mport Mapping.fr
+000000a0: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
+000000b0: 7420 5061 7468 0a66 726f 6d20 7479 7069  t Path.from typi
+000000c0: 6e67 2069 6d70 6f72 7420 4c69 7465 7261  ng import Litera
+000000d0: 6c0a 0a69 6620 7479 7069 6e67 2e54 5950  l..if typing.TYP
+000000e0: 455f 4348 4543 4b49 4e47 3a0a 2020 2020  E_CHECKING:.    
+000000f0: 696d 706f 7274 2063 6c69 636b 0a65 6c73  import click.els
+00000100: 653a 0a20 2020 2069 6d70 6f72 7420 7269  e:.    import ri
+00000110: 6368 5f63 6c69 636b 2061 7320 636c 6963  ch_click as clic
+00000120: 6b0a 0a69 6d70 6f72 7420 6d61 726b 646f  k..import markdo
+00000130: 776e 5f69 740a 696d 706f 7274 2072 6963  wn_it.import ric
+00000140: 682e 636f 6e73 6f6c 650a 696d 706f 7274  h.console.import
+00000150: 2072 6963 682e 6d61 726b 646f 776e 0a69   rich.markdown.i
+00000160: 6d70 6f72 7420 7269 6368 2e74 6572 6d69  mport rich.termi
+00000170: 6e61 6c5f 7468 656d 650a 696d 706f 7274  nal_theme.import
+00000180: 2072 6963 682e 7465 7874 0a69 6d70 6f72   rich.text.impor
+00000190: 7420 7269 6368 2e74 7261 6365 6261 636b  t rich.traceback
+000001a0: 0a69 6d70 6f72 7420 7269 6368 2e74 7265  .import rich.tre
+000001b0: 650a 0a66 726f 6d20 2e5f 636f 6d70 6174  e..from ._compat
+000001c0: 2e69 6d70 6f72 746c 6962 2e72 6573 6f75  .importlib.resou
+000001d0: 7263 6573 2e61 6263 2069 6d70 6f72 7420  rces.abc import 
+000001e0: 5472 6176 6572 7361 626c 650a 6672 6f6d  Traversable.from
+000001f0: 202e 6661 6d69 6c69 6573 2069 6d70 6f72   .families impor
+00000200: 7420 4661 6d69 6c79 0a66 726f 6d20 2e67  t Family.from .g
+00000210: 6870 6174 6820 696d 706f 7274 2047 4850  hpath import GHP
+00000220: 6174 680a 6672 6f6d 202e 7072 6f63 6573  ath.from .proces
+00000230: 736f 7220 696d 706f 7274 2052 6573 756c  sor import Resul
+00000240: 742c 205f 636f 6c6c 6563 745f 616c 6c2c  t, _collect_all,
+00000250: 2061 735f 7369 6d70 6c65 5f64 6963 742c   as_simple_dict,
+00000260: 2070 726f 6365 7373 0a0a 7269 6368 2e74   process..rich.t
+00000270: 7261 6365 6261 636b 2e69 6e73 7461 6c6c  raceback.install
+00000280: 2873 7570 7072 6573 733d 5b63 6c69 636b  (suppress=[click
+00000290: 2c20 7269 6368 5d2c 2073 686f 775f 6c6f  , rich], show_lo
+000002a0: 6361 6c73 3d54 7275 652c 2077 6964 7468  cals=True, width
+000002b0: 3d4e 6f6e 6529 0a0a 2320 5573 6520 6d6f  =None)..# Use mo
+000002c0: 6475 6c65 2d6c 6576 656c 2065 6e74 7279  dule-level entry
+000002d0: 206e 616d 6573 0a23 2072 6570 6f5f 7265   names.# repo_re
+000002e0: 7669 6577 5f66 6978 7475 7265 7320 3d20  view_fixtures = 
+000002f0: 7b22 7079 7072 6f6a 6563 7422 7d0a 2320  {"pyproject"}.# 
+00000300: 7265 706f 5f72 6576 6965 775f 6368 6563  repo_review_chec
+00000310: 6b73 203d 2073 6574 2870 2e5f 5f6e 616d  ks = set(p.__nam
+00000320: 655f 5f5f 2066 6f72 2070 2069 6e20 4765  e___ for p in Ge
+00000330: 6e65 7261 6c2e 5f5f 7375 6263 6c61 7373  neral.__subclass
+00000340: 6573 5f5f 2829 290a 0a0a 6465 6620 7269  es__())...def ri
+00000350: 6368 5f70 7269 6e74 6572 280a 2020 2020  ch_printer(.    
+00000360: 6661 6d69 6c69 6573 3a20 4d61 7070 696e  families: Mappin
+00000370: 675b 7374 722c 2046 616d 696c 795d 2c20  g[str, Family], 
+00000380: 7072 6f63 6573 7365 643a 206c 6973 745b  processed: list[
+00000390: 5265 7375 6c74 5d2c 202a 2c20 6f75 7470  Result], *, outp
+000003a0: 7574 3a20 5061 7468 207c 204e 6f6e 650a  ut: Path | None.
+000003b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2063  ) -> None:.    c
+000003c0: 6f6e 736f 6c65 203d 2072 6963 682e 636f  onsole = rich.co
+000003d0: 6e73 6f6c 652e 436f 6e73 6f6c 6528 7265  nsole.Console(re
+000003e0: 636f 7264 3d54 7275 6529 0a0a 2020 2020  cord=True)..    
+000003f0: 666f 7220 6661 6d69 6c79 2c20 7265 7375  for family, resu
+00000400: 6c74 735f 6c69 7374 2069 6e20 6974 6572  lts_list in iter
+00000410: 746f 6f6c 732e 6772 6f75 7062 7928 7072  tools.groupby(pr
+00000420: 6f63 6573 7365 642c 206c 616d 6264 6120  ocessed, lambda 
+00000430: 723a 2072 2e66 616d 696c 7929 3a0a 2020  r: r.family):.  
+00000440: 2020 2020 2020 6661 6d69 6c79 5f6e 616d        family_nam
+00000450: 6520 3d20 6661 6d69 6c69 6573 5b66 616d  e = families[fam
+00000460: 696c 795d 2e67 6574 2822 6e61 6d65 222c  ily].get("name",
+00000470: 2066 616d 696c 7929 0a20 2020 2020 2020   family).       
+00000480: 2074 7265 6520 3d20 7269 6368 2e74 7265   tree = rich.tre
+00000490: 652e 5472 6565 2866 225b 626f 6c64 5d7b  e.Tree(f"[bold]{
+000004a0: 6661 6d69 6c79 5f6e 616d 657d 5b2f 626f  family_name}[/bo
+000004b0: 6c64 5d3a 2229 0a20 2020 2020 2020 2066  ld]:").        f
+000004c0: 6f72 2072 6573 756c 7420 696e 2072 6573  or result in res
+000004d0: 756c 7473 5f6c 6973 743a 0a20 2020 2020  ults_list:.     
+000004e0: 2020 2020 2020 2063 6f6c 6f72 203d 2028         color = (
+000004f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000500: 2022 7965 6c6c 6f77 220a 2020 2020 2020   "yellow".      
+00000510: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+00000520: 756c 742e 7265 7375 6c74 2069 7320 4e6f  ult.result is No
+00000530: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00000540: 2020 2065 6c73 6520 2267 7265 656e 220a     else "green".
+00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000560: 6966 2072 6573 756c 742e 7265 7375 6c74  if result.result
+00000570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000580: 2065 6c73 6520 2272 6564 220a 2020 2020   else "red".    
+00000590: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000005a0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+000005b0: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
+000005c0: 2020 2020 2020 6622 5b6c 696e 6b3d 7b72        f"[link={r
+000005d0: 6573 756c 742e 7572 6c7d 5d7b 7265 7375  esult.url}]{resu
+000005e0: 6c74 2e64 6573 6372 6970 7469 6f6e 7d5b  lt.description}[
+000005f0: 2f6c 696e 6b5d 220a 2020 2020 2020 2020  /link]".        
+00000600: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
+00000610: 742e 7572 6c0a 2020 2020 2020 2020 2020  t.url.          
+00000620: 2020 2020 2020 656c 7365 2072 6573 756c        else resul
+00000630: 742e 6465 7363 7269 7074 696f 6e0a 2020  t.description.  
+00000640: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00000650: 2020 2020 2020 2020 6d73 6720 3d20 7269          msg = ri
+00000660: 6368 2e74 6578 742e 5465 7874 2829 0a20  ch.text.Text(). 
+00000670: 2020 2020 2020 2020 2020 206d 7367 2e61             msg.a
+00000680: 7070 656e 6428 7265 7375 6c74 2e6e 616d  ppend(result.nam
+00000690: 652c 2073 7479 6c65 3d22 626f 6c64 2229  e, style="bold")
+000006a0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+000006b0: 2e61 7070 656e 6428 2220 2229 0a20 2020  .append(" ").   
+000006c0: 2020 2020 2020 2020 206d 7367 2e61 7070           msg.app
+000006d0: 656e 6428 7269 6368 2e74 6578 742e 5465  end(rich.text.Te
+000006e0: 7874 2e66 726f 6d5f 6d61 726b 7570 2864  xt.from_markup(d
+000006f0: 6573 6372 6970 7469 6f6e 2c20 7374 796c  escription, styl
+00000700: 653d 636f 6c6f 7229 290a 2020 2020 2020  e=color)).      
+00000710: 2020 2020 2020 6966 2072 6573 756c 742e        if result.
+00000720: 7265 7375 6c74 2069 7320 4e6f 6e65 3a0a  result is None:.
+00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000740: 6d73 672e 6170 7065 6e64 2822 205b 736b  msg.append(" [sk
+00000750: 6970 7065 645d 222c 2073 7479 6c65 3d22  ipped]", style="
+00000760: 7965 6c6c 6f77 2062 6f6c 6422 290a 2020  yellow bold").  
+00000770: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00000780: 6565 2e61 6464 286d 7367 290a 2020 2020  ee.add(msg).    
+00000790: 2020 2020 2020 2020 656c 6966 2072 6573          elif res
+000007a0: 756c 742e 7265 7375 6c74 3a0a 2020 2020  ult.result:.    
+000007b0: 2020 2020 2020 2020 2020 2020 6d73 672e              msg.
+000007c0: 6170 7065 6e64 2872 6963 682e 7465 7874  append(rich.text
+000007d0: 2e54 6578 742e 6672 6f6d 5f6d 6172 6b75  .Text.from_marku
+000007e0: 7028 2220 3a77 6869 7465 5f63 6865 636b  p(" :white_check
+000007f0: 5f6d 6172 6b3a 2229 290a 2020 2020 2020  _mark:")).      
+00000800: 2020 2020 2020 2020 2020 7472 6565 2e61            tree.a
+00000810: 6464 286d 7367 290a 2020 2020 2020 2020  dd(msg).        
+00000820: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000830: 2020 2020 2020 2020 2020 6d73 672e 6170            msg.ap
+00000840: 7065 6e64 2872 6963 682e 7465 7874 2e54  pend(rich.text.T
+00000850: 6578 742e 6672 6f6d 5f6d 6172 6b75 7028  ext.from_markup(
+00000860: 2220 3a78 3a22 2929 0a20 2020 2020 2020  " :x:")).       
+00000870: 2020 2020 2020 2020 2064 6574 6169 6c20           detail 
+00000880: 3d20 7269 6368 2e6d 6172 6b64 6f77 6e2e  = rich.markdown.
+00000890: 4d61 726b 646f 776e 2872 6573 756c 742e  Markdown(result.
+000008a0: 6572 725f 6d73 6729 0a20 2020 2020 2020  err_msg).       
+000008b0: 2020 2020 2020 2020 206d 7367 5f67 7270           msg_grp
+000008c0: 203d 2072 6963 682e 636f 6e73 6f6c 652e   = rich.console.
+000008d0: 4772 6f75 7028 6d73 672c 2064 6574 6169  Group(msg, detai
+000008e0: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
+000008f0: 2020 2074 7265 652e 6164 6428 6d73 675f     tree.add(msg_
+00000900: 6772 7029 0a0a 2020 2020 2020 2020 636f  grp)..        co
+00000910: 6e73 6f6c 652e 7072 696e 7428 7472 6565  nsole.print(tree
+00000920: 290a 2020 2020 2020 2020 636f 6e73 6f6c  ).        consol
+00000930: 652e 7072 696e 7428 290a 0a20 2020 2069  e.print()..    i
+00000940: 6620 6f75 7470 7574 2069 7320 6e6f 7420  f output is not 
+00000950: 4e6f 6e65 3a0a 2020 2020 2020 2020 636f  None:.        co
+00000960: 6e73 6f6c 652e 7361 7665 5f73 7667 2873  nsole.save_svg(s
+00000970: 7472 286f 7574 7075 7429 2c20 7468 656d  tr(output), them
+00000980: 653d 7269 6368 2e74 6572 6d69 6e61 6c5f  e=rich.terminal_
+00000990: 7468 656d 652e 4445 4641 554c 545f 5445  theme.DEFAULT_TE
+000009a0: 524d 494e 414c 5f54 4845 4d45 290a 0a0a  RMINAL_THEME)...
+000009b0: 6465 6620 746f 5f68 746d 6c28 6661 6d69  def to_html(fami
+000009c0: 6c69 6573 3a20 4d61 7070 696e 675b 7374  lies: Mapping[st
+000009d0: 722c 2046 616d 696c 795d 2c20 7072 6f63  r, Family], proc
+000009e0: 6573 7365 643a 206c 6973 745b 5265 7375  essed: list[Resu
+000009f0: 6c74 5d29 202d 3e20 7374 723a 0a20 2020  lt]) -> str:.   
+00000a00: 206f 7574 203d 2069 6f2e 5374 7269 6e67   out = io.String
+00000a10: 494f 2829 0a20 2020 2070 7269 6e74 203d  IO().    print =
+00000a20: 2066 756e 6374 6f6f 6c73 2e70 6172 7469   functools.parti
+00000a30: 616c 2862 7569 6c74 696e 732e 7072 696e  al(builtins.prin
+00000a40: 742c 2066 696c 653d 6f75 7429 0a20 2020  t, file=out).   
+00000a50: 206d 6420 3d20 6d61 726b 646f 776e 5f69   md = markdown_i
+00000a60: 742e 4d61 726b 646f 776e 4974 2829 0a0a  t.MarkdownIt()..
+00000a70: 2020 2020 666f 7220 6661 6d69 6c79 2c20      for family, 
+00000a80: 7265 7375 6c74 735f 6c69 7374 2069 6e20  results_list in 
+00000a90: 6974 6572 746f 6f6c 732e 6772 6f75 7062  itertools.groupb
+00000aa0: 7928 7072 6f63 6573 7365 642c 206c 616d  y(processed, lam
+00000ab0: 6264 6120 723a 2072 2e66 616d 696c 7929  bda r: r.family)
+00000ac0: 3a0a 2020 2020 2020 2020 6661 6d69 6c79  :.        family
+00000ad0: 5f6e 616d 6520 3d20 6661 6d69 6c69 6573  _name = families
+00000ae0: 5b66 616d 696c 795d 2e67 6574 2822 6e61  [family].get("na
+00000af0: 6d65 222c 2066 616d 696c 7929 0a20 2020  me", family).   
+00000b00: 2020 2020 2070 7269 6e74 2866 223c 6832       print(f"<h2
+00000b10: 3e7b 6661 6d69 6c79 5f6e 616d 657d 3c2f  >{family_name}</
+00000b20: 6832 3e22 290a 2020 2020 2020 2020 7072  h2>").        pr
+00000b30: 696e 7428 223c 7461 626c 653e 2229 0a20  int("<table>"). 
+00000b40: 2020 2020 2020 2070 7269 6e74 2822 3c74         print("<t
+00000b50: 723e 3c74 683e 3f3c 2f74 683e 3c74 683e  r><th>?</th><th>
+00000b60: 4e61 6d65 3c2f 7468 3e3c 7468 3e44 6573  Name</th><th>Des
+00000b70: 6372 6970 7469 6f6e 3c2f 7468 3e3c 2f74  cription</th></t
+00000b80: 723e 2229 0a20 2020 2020 2020 2066 6f72  r>").        for
+00000b90: 2072 6573 756c 7420 696e 2072 6573 756c   result in resul
+00000ba0: 7473 5f6c 6973 743a 0a20 2020 2020 2020  ts_list:.       
+00000bb0: 2020 2020 2063 6f6c 6f72 203d 2028 0a20       color = (. 
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000bd0: 6f72 616e 6765 220a 2020 2020 2020 2020  orange".        
+00000be0: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
+00000bf0: 742e 7265 7375 6c74 2069 7320 4e6f 6e65  t.result is None
 00000c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c10: 2070 7269 6e74 2822 3c62 722f 3e22 290a   print("<br/>").
-00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c30: 7072 696e 7428 6d64 2e72 656e 6465 7228  print(md.render(
-00000c40: 7265 7375 6c74 2e65 7272 5f6d 7367 2929  result.err_msg))
-00000c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c60: 2070 7269 6e74 2822 3c2f 7464 3e22 290a   print("</td>").
-00000c70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00000c80: 7428 223c 2f74 723e 2229 0a20 2020 2020  t("</tr>").     
-00000c90: 2020 2070 7269 6e74 2822 3c2f 7461 626c     print("</tabl
-00000ca0: 653e 2229 0a20 2020 2072 6574 7572 6e20  e>").    return 
-00000cb0: 6f75 742e 6765 7476 616c 7565 2829 0a0a  out.getvalue()..
-00000cc0: 0a40 636c 6963 6b2e 636f 6d6d 616e 6428  .@click.command(
-00000cd0: 636f 6e74 6578 745f 7365 7474 696e 6773  context_settings
-00000ce0: 3d7b 2268 656c 705f 6f70 7469 6f6e 5f6e  ={"help_option_n
-00000cf0: 616d 6573 223a 205b 222d 6822 2c20 222d  ames": ["-h", "-
-00000d00: 2d68 656c 7022 5d7d 290a 4063 6c69 636b  -help"]}).@click
-00000d10: 2e61 7267 756d 656e 7428 2270 6163 6b61  .argument("packa
-00000d20: 6765 222c 2074 7970 653d 636c 6963 6b2e  ge", type=click.
-00000d30: 5061 7468 2864 6972 5f6f 6b61 793d 5472  Path(dir_okay=Tr
-00000d40: 7565 2c20 7061 7468 5f74 7970 653d 5061  ue, path_type=Pa
-00000d50: 7468 2929 0a40 636c 6963 6b2e 6f70 7469  th)).@click.opti
-00000d60: 6f6e 280a 2020 2020 222d 2d6f 7574 7075  on(.    "--outpu
-00000d70: 7422 2c0a 2020 2020 7479 7065 3d63 6c69  t",.    type=cli
-00000d80: 636b 2e50 6174 6828 6669 6c65 5f6f 6b61  ck.Path(file_oka
-00000d90: 793d 5472 7565 2c20 6578 6973 7473 3d46  y=True, exists=F
-00000da0: 616c 7365 2c20 7061 7468 5f74 7970 653d  alse, path_type=
-00000db0: 5061 7468 292c 0a20 2020 2064 6566 6175  Path),.    defau
-00000dc0: 6c74 3d4e 6f6e 652c 0a20 2020 2068 656c  lt=None,.    hel
-00000dd0: 703d 2257 7269 7465 206f 7574 2066 696c  p="Write out fil
-00000de0: 652e 2057 7269 7465 7320 5356 4720 6966  e. Writes SVG if
-00000df0: 2066 6f72 6d61 7420 6973 2072 6963 682e   format is rich.
-00000e00: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
-00000e10: 6f6e 280a 2020 2020 222d 2d66 6f72 6d61  on(.    "--forma
-00000e20: 7422 2c0a 2020 2020 7479 7065 3d63 6c69  t",.    type=cli
-00000e30: 636b 2e43 686f 6963 6528 5b22 7269 6368  ck.Choice(["rich
-00000e40: 222c 2022 6a73 6f6e 222c 2022 6874 6d6c  ", "json", "html
-00000e50: 225d 292c 0a20 2020 2064 6566 6175 6c74  "]),.    default
-00000e60: 3d22 7269 6368 222c 0a20 2020 2068 656c  ="rich",.    hel
-00000e70: 703d 2253 656c 6563 7420 6f75 7470 7574  p="Select output
-00000e80: 2066 6f72 6d61 742e 222c 0a29 0a40 636c   format.",.).@cl
-00000e90: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
-00000ea0: 222d 2d69 676e 6f72 6522 2c0a 2020 2020  "--ignore",.    
-00000eb0: 6865 6c70 3d22 4967 6e6f 7265 2061 2063  help="Ignore a c
-00000ec0: 6865 636b 206f 7220 6368 6563 6b73 2c20  heck or checks, 
-00000ed0: 636f 6d6d 6120 7365 7061 7261 7465 642e  comma separated.
-00000ee0: 222c 0a20 2020 2064 6566 6175 6c74 3d22  ",.    default="
-00000ef0: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
-00000f00: 6f6e 280a 2020 2020 222d 2d70 6163 6b61  on(.    "--packa
-00000f10: 6765 2d64 6972 222c 0a20 2020 2022 2d70  ge-dir",.    "-p
-00000f20: 222c 0a20 2020 2068 656c 703d 2250 7974  ",.    help="Pyt
-00000f30: 686f 6e20 7061 636b 6167 6520 7375 6264  hon package subd
-00000f40: 6972 6563 746f 7279 222c 0a20 2020 2064  irectory",.    d
-00000f50: 6566 6175 6c74 3d22 222c 0a29 0a64 6566  efault="",.).def
-00000f60: 206d 6169 6e28 0a20 2020 2070 6163 6b61   main(.    packa
-00000f70: 6765 3a20 5061 7468 2c0a 2020 2020 6f75  ge: Path,.    ou
-00000f80: 7470 7574 3a20 5061 7468 207c 204e 6f6e  tput: Path | Non
-00000f90: 652c 0a20 2020 2066 6f72 6d61 743a 204c  e,.    format: L
-00000fa0: 6974 6572 616c 5b22 7269 6368 222c 2022  iteral["rich", "
-00000fb0: 6a73 6f6e 222c 2022 6874 6d6c 225d 2c0a  json", "html"],.
-00000fc0: 2020 2020 6967 6e6f 7265 3a20 7374 722c      ignore: str,
-00000fd0: 0a20 2020 2070 6163 6b61 6765 5f64 6972  .    package_dir
-00000fe0: 3a20 7374 722c 0a29 202d 3e20 4e6f 6e65  : str,.) -> None
-00000ff0: 3a0a 2020 2020 2222 220a 2020 2020 5061  :.    """.    Pa
-00001000: 7373 2069 6e20 6120 6c6f 6361 6c20 5061  ss in a local Pa
-00001010: 7468 206f 7220 6768 3a6f 7267 2f72 6570  th or gh:org/rep
-00001020: 6f40 6272 616e 6368 2e0a 2020 2020 2222  o@branch..    ""
-00001030: 220a 2020 2020 6967 6e6f 7265 5f6c 6973  ".    ignore_lis
-00001040: 7420 3d20 5b78 2e73 7472 6970 2829 2066  t = [x.strip() f
-00001050: 6f72 2078 2069 6e20 6967 6e6f 7265 2e73  or x in ignore.s
-00001060: 706c 6974 2822 2c22 295d 0a0a 2020 2020  plit(",")]..    
-00001070: 6966 2073 7472 2870 6163 6b61 6765 292e  if str(package).
-00001080: 7374 6172 7473 7769 7468 2822 6768 3a22  startswith("gh:"
-00001090: 293a 0a20 2020 2020 2020 205f 2c20 6f72  ):.        _, or
-000010a0: 675f 7265 706f 5f62 7261 6e63 682c 202a  g_repo_branch, *
-000010b0: 7020 3d20 7374 7228 7061 636b 6167 6529  p = str(package)
-000010c0: 2e73 706c 6974 2822 3a22 2c20 6d61 7873  .split(":", maxs
-000010d0: 706c 6974 3d32 290a 2020 2020 2020 2020  plit=2).        
-000010e0: 6f72 675f 7265 706f 2c20 6272 616e 6368  org_repo, branch
-000010f0: 203d 206f 7267 5f72 6570 6f5f 6272 616e   = org_repo_bran
-00001100: 6368 2e73 706c 6974 2822 4022 2c20 6d61  ch.split("@", ma
-00001110: 7873 706c 6974 3d31 290a 2020 2020 2020  xsplit=1).      
-00001120: 2020 6768 7061 636b 6167 6520 3d20 4748    ghpackage = GH
-00001130: 5061 7468 2872 6570 6f3d 6f72 675f 7265  Path(repo=org_re
-00001140: 706f 2c20 6272 616e 6368 3d62 7261 6e63  po, branch=branc
-00001150: 682c 2070 6174 683d 705b 305d 2069 6620  h, path=p[0] if 
-00001160: 7020 656c 7365 2022 2229 0a20 2020 2020  p else "").     
-00001170: 2020 2069 6620 666f 726d 6174 203d 3d20     if format == 
-00001180: 2272 6963 6822 3a0a 2020 2020 2020 2020  "rich":.        
-00001190: 2020 2020 7269 6368 2e70 7269 6e74 2866      rich.print(f
-000011a0: 225b 626f 6c64 5d50 726f 6365 7373 696e  "[bold]Processin
-000011b0: 6720 5b62 6c75 655d 7b70 6163 6b61 6765  g [blue]{package
-000011c0: 7d5b 2f62 6c75 655d 2066 726f 6d20 4769  }[/blue] from Gi
-000011d0: 7448 7562 5c6e 2229 0a20 2020 2020 2020  tHub\n").       
-000011e0: 2066 616d 696c 6965 732c 2070 726f 6365   families, proce
-000011f0: 7373 6564 203d 2070 726f 6365 7373 2867  ssed = process(g
-00001200: 6870 6163 6b61 6765 2c20 6967 6e6f 7265  hpackage, ignore
-00001210: 3d69 676e 6f72 655f 6c69 7374 2c20 7375  =ignore_list, su
-00001220: 6264 6972 3d70 6163 6b61 6765 5f64 6972  bdir=package_dir
-00001230: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00001240: 2020 2020 6661 6d69 6c69 6573 2c20 7072      families, pr
-00001250: 6f63 6573 7365 6420 3d20 7072 6f63 6573  ocessed = proces
-00001260: 7328 7061 636b 6167 652c 2069 676e 6f72  s(package, ignor
-00001270: 653d 6967 6e6f 7265 5f6c 6973 742c 2073  e=ignore_list, s
-00001280: 7562 6469 723d 7061 636b 6167 655f 6469  ubdir=package_di
-00001290: 7229 0a0a 2020 2020 6966 2066 6f72 6d61  r)..    if forma
-000012a0: 7420 3d3d 2022 7269 6368 223a 0a20 2020  t == "rich":.   
-000012b0: 2020 2020 2072 6963 685f 7072 696e 7465       rich_printe
-000012c0: 7228 6661 6d69 6c69 6573 2c20 7072 6f63  r(families, proc
-000012d0: 6573 7365 642c 206f 7574 7075 743d 6f75  essed, output=ou
-000012e0: 7470 7574 290a 2020 2020 656c 6966 2066  tput).    elif f
-000012f0: 6f72 6d61 7420 3d3d 2022 6a73 6f6e 223a  ormat == "json":
-00001300: 0a20 2020 2020 2020 206a 203d 206a 736f  .        j = jso
-00001310: 6e2e 6475 6d70 7328 0a20 2020 2020 2020  n.dumps(.       
-00001320: 2020 2020 207b 2266 616d 696c 6965 7322       {"families"
-00001330: 3a20 6661 6d69 6c69 6573 2c20 2263 6865  : families, "che
-00001340: 636b 7322 3a20 6173 5f73 696d 706c 655f  cks": as_simple_
-00001350: 6469 6374 2870 726f 6365 7373 6564 297d  dict(processed)}
-00001360: 2c20 696e 6465 6e74 3d32 0a20 2020 2020  , indent=2.     
-00001370: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00001380: 6f75 7470 7574 3a0a 2020 2020 2020 2020  output:.        
-00001390: 2020 2020 6f75 7470 7574 2e77 7269 7465      output.write
-000013a0: 5f74 6578 7428 6a29 0a20 2020 2020 2020  _text(j).       
-000013b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000013c0: 2020 2072 6963 682e 7072 696e 745f 6a73     rich.print_js
-000013d0: 6f6e 286a 290a 2020 2020 656c 6966 2066  on(j).    elif f
-000013e0: 6f72 6d61 7420 3d3d 2022 6874 6d6c 223a  ormat == "html":
-000013f0: 0a20 2020 2020 2020 2068 746d 6c20 3d20  .        html = 
-00001400: 746f 5f68 746d 6c28 6661 6d69 6c69 6573  to_html(families
-00001410: 2c20 7072 6f63 6573 7365 6429 0a20 2020  , processed).   
-00001420: 2020 2020 2069 6620 6f75 7470 7574 3a0a       if output:.
-00001430: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00001440: 7574 2e77 7269 7465 5f74 6578 7428 6874  ut.write_text(ht
-00001450: 6d6c 290a 2020 2020 2020 2020 656c 7365  ml).        else
-00001460: 3a0a 2020 2020 2020 2020 2020 2020 7269  :.            ri
-00001470: 6368 2e70 7269 6e74 2868 746d 6c29 0a0a  ch.print(html)..
-00001480: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00001490: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-000014a0: 6d61 696e 2829 2020 2320 7079 6c69 6e74  main()  # pylint
-000014b0: 3a20 6469 7361 626c 653d 6e6f 2d76 616c  : disable=no-val
-000014c0: 7565 2d66 6f72 2d70 6172 616d 6574 6572  ue-for-parameter
-000014d0: 0a                                       .
+00000c10: 2065 6c73 6520 2267 7265 656e 220a 2020   else "green".  
+00000c20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000c30: 2072 6573 756c 742e 7265 7375 6c74 0a20   result.result. 
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00000c50: 6c73 6520 2272 6564 220a 2020 2020 2020  lse "red".      
+00000c60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00000c70: 2020 2020 6963 6f6e 203d 2022 e29a a0ef      icon = "....
+00000c80: b88f 2220 6966 2072 6573 756c 742e 7265  .." if result.re
+00000c90: 7375 6c74 2069 7320 4e6f 6e65 2065 6c73  sult is None els
+00000ca0: 6520 22e2 9c85 2220 6966 2072 6573 756c  e "..." if resul
+00000cb0: 742e 7265 7375 6c74 2065 6c73 6520 22e2  t.result else ".
+00000cc0: 9d8c 220a 2020 2020 2020 2020 2020 2020  ..".            
+00000cd0: 7265 7375 6c74 5f74 7874 203d 2028 0a20  result_txt = (. 
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000cf0: 536b 6970 7065 6422 0a20 2020 2020 2020  Skipped".       
+00000d00: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
+00000d10: 6c74 2e72 6573 756c 7420 6973 204e 6f6e  lt.result is Non
+00000d20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00000d30: 2020 656c 7365 2022 5061 7373 6564 220a    else "Passed".
+00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d50: 6966 2072 6573 756c 742e 7265 7375 6c74  if result.result
+00000d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d70: 2065 6c73 6520 2246 6169 6c65 6422 0a20   else "Failed". 
+00000d80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00000d90: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00000da0: 7469 6f6e 203d 2028 0a20 2020 2020 2020  tion = (.       
+00000db0: 2020 2020 2020 2020 2066 273c 6120 6872           f'<a hr
+00000dc0: 6566 3d22 7b72 6573 756c 742e 7572 6c7d  ef="{result.url}
+00000dd0: 223e 7b72 6573 756c 742e 6465 7363 7269  ">{result.descri
+00000de0: 7074 696f 6e7d 3c2f 613e 270a 2020 2020  ption}</a>'.    
+00000df0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00000e00: 6573 756c 742e 7572 6c0a 2020 2020 2020  esult.url.      
+00000e10: 2020 2020 2020 2020 2020 656c 7365 2072            else r
+00000e20: 6573 756c 742e 6465 7363 7269 7074 696f  esult.descriptio
+00000e30: 6e0a 2020 2020 2020 2020 2020 2020 290a  n.            ).
+00000e40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000e50: 7428 6627 3c74 7220 7374 796c 653d 2263  t(f'<tr style="c
+00000e60: 6f6c 6f72 3a20 7b63 6f6c 6f72 7d3b 223e  olor: {color};">
+00000e70: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
+00000e80: 7269 6e74 2866 273c 7464 3e3c 7370 616e  rint(f'<td><span
+00000e90: 2072 6f6c 653d 2269 6d67 2220 6172 6961   role="img" aria
+00000ea0: 2d6c 6162 656c 3d22 7b72 6573 756c 745f  -label="{result_
+00000eb0: 7478 747d 223e 7b69 636f 6e7d 3c2f 7370  txt}">{icon}</sp
+00000ec0: 616e 3e3c 2f74 643e 2729 0a20 2020 2020  an></td>').     
+00000ed0: 2020 2020 2020 2070 7269 6e74 2866 223c         print(f"<
+00000ee0: 7464 3e7b 7265 7375 6c74 2e6e 616d 657d  td>{result.name}
+00000ef0: 3c2f 7464 3e22 290a 2020 2020 2020 2020  </td>").        
+00000f00: 2020 2020 6966 2072 6573 756c 742e 7265      if result.re
+00000f10: 7375 6c74 2069 7320 4e6f 6e65 206f 7220  sult is None or 
+00000f20: 7265 7375 6c74 2e72 6573 756c 743a 0a20  result.result:. 
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00000f40: 7269 6e74 2866 223c 7464 3e7b 6465 7363  rint(f"<td>{desc
+00000f50: 7269 7074 696f 6e7d 3c2f 7464 3e22 290a  ription}</td>").
+00000f60: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00000f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000f80: 2020 7072 696e 7428 223c 7464 3e22 290a    print("<td>").
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fa0: 7072 696e 7428 6465 7363 7269 7074 696f  print(descriptio
+00000fb0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
+00000fc0: 2020 2070 7269 6e74 2822 3c62 722f 3e22     print("<br/>"
+00000fd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00000fe0: 2020 7072 696e 7428 6d64 2e72 656e 6465    print(md.rende
+00000ff0: 7228 7265 7375 6c74 2e65 7272 5f6d 7367  r(result.err_msg
+00001000: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00001010: 2020 2070 7269 6e74 2822 3c2f 7464 3e22     print("</td>"
+00001020: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00001030: 696e 7428 223c 2f74 723e 2229 0a20 2020  int("</tr>").   
+00001040: 2020 2020 2070 7269 6e74 2822 3c2f 7461       print("</ta
+00001050: 626c 653e 2229 0a0a 2020 2020 6966 206c  ble>")..    if l
+00001060: 656e 2870 726f 6365 7373 6564 2920 3d3d  en(processed) ==
+00001070: 2030 3a0a 2020 2020 2020 2020 7072 696e   0:.        prin
+00001080: 7428 273c 7370 616e 2073 7479 6c65 3d22  t('<span style="
+00001090: 636f 6c6f 723a 2072 6564 3b22 3e4e 6f20  color: red;">No 
+000010a0: 6368 6563 6b73 2072 616e 2e3c 2f73 7061  checks ran.</spa
+000010b0: 6e3e 2729 0a0a 2020 2020 7265 7475 726e  n>')..    return
+000010c0: 206f 7574 2e67 6574 7661 6c75 6528 290a   out.getvalue().
+000010d0: 0a0a 4063 6c69 636b 2e63 6f6d 6d61 6e64  ..@click.command
+000010e0: 2863 6f6e 7465 7874 5f73 6574 7469 6e67  (context_setting
+000010f0: 733d 7b22 6865 6c70 5f6f 7074 696f 6e5f  s={"help_option_
+00001100: 6e61 6d65 7322 3a20 5b22 2d68 222c 2022  names": ["-h", "
+00001110: 2d2d 6865 6c70 225d 7d29 0a40 636c 6963  --help"]}).@clic
+00001120: 6b2e 6172 6775 6d65 6e74 2822 7061 636b  k.argument("pack
+00001130: 6167 6522 2c20 7479 7065 3d63 6c69 636b  age", type=click
+00001140: 2e50 6174 6828 6469 725f 6f6b 6179 3d54  .Path(dir_okay=T
+00001150: 7275 652c 2070 6174 685f 7479 7065 3d50  rue, path_type=P
+00001160: 6174 6829 290a 4063 6c69 636b 2e6f 7074  ath)).@click.opt
+00001170: 696f 6e28 0a20 2020 2022 2d2d 6f75 7470  ion(.    "--outp
+00001180: 7574 222c 0a20 2020 2074 7970 653d 636c  ut",.    type=cl
+00001190: 6963 6b2e 5061 7468 2866 696c 655f 6f6b  ick.Path(file_ok
+000011a0: 6179 3d54 7275 652c 2065 7869 7374 733d  ay=True, exists=
+000011b0: 4661 6c73 652c 2070 6174 685f 7479 7065  False, path_type
+000011c0: 3d50 6174 6829 2c0a 2020 2020 6465 6661  =Path),.    defa
+000011d0: 756c 743d 4e6f 6e65 2c0a 2020 2020 6865  ult=None,.    he
+000011e0: 6c70 3d22 5772 6974 6520 6f75 7420 6669  lp="Write out fi
+000011f0: 6c65 2e20 5772 6974 6573 2053 5647 2069  le. Writes SVG i
+00001200: 6620 666f 726d 6174 2069 7320 7269 6368  f format is rich
+00001210: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
+00001220: 696f 6e28 0a20 2020 2022 2d2d 666f 726d  ion(.    "--form
+00001230: 6174 222c 0a20 2020 2074 7970 653d 636c  at",.    type=cl
+00001240: 6963 6b2e 4368 6f69 6365 285b 2272 6963  ick.Choice(["ric
+00001250: 6822 2c20 226a 736f 6e22 2c20 2268 746d  h", "json", "htm
+00001260: 6c22 5d29 2c0a 2020 2020 6465 6661 756c  l"]),.    defaul
+00001270: 743d 2272 6963 6822 2c0a 2020 2020 6865  t="rich",.    he
+00001280: 6c70 3d22 5365 6c65 6374 206f 7574 7075  lp="Select outpu
+00001290: 7420 666f 726d 6174 2e22 2c0a 290a 4063  t format.",.).@c
+000012a0: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
+000012b0: 2022 2d2d 7365 6c65 6374 222c 0a20 2020   "--select",.   
+000012c0: 2068 656c 703d 224f 6e6c 7920 7275 6e20   help="Only run 
+000012d0: 6365 7274 6169 6e20 6368 6563 6b73 2c20  certain checks, 
+000012e0: 636f 6d6d 6120 7365 7061 7261 7465 642e  comma separated.
+000012f0: 2041 6c6c 2063 6865 636b 7320 7275 6e20   All checks run 
+00001300: 6966 2065 6d70 7479 2e22 2c0a 2020 2020  if empty.",.    
+00001310: 6465 6661 756c 743d 2222 2c0a 290a 4063  default="",.).@c
+00001320: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
+00001330: 2022 2d2d 6967 6e6f 7265 222c 0a20 2020   "--ignore",.   
+00001340: 2068 656c 703d 2249 676e 6f72 6520 6120   help="Ignore a 
+00001350: 6368 6563 6b20 6f72 2063 6865 636b 732c  check or checks,
+00001360: 2063 6f6d 6d61 2073 6570 6172 6174 6564   comma separated
+00001370: 2e22 2c0a 2020 2020 6465 6661 756c 743d  .",.    default=
+00001380: 2222 2c0a 290a 4063 6c69 636b 2e6f 7074  "",.).@click.opt
+00001390: 696f 6e28 0a20 2020 2022 2d2d 7061 636b  ion(.    "--pack
+000013a0: 6167 652d 6469 7222 2c0a 2020 2020 222d  age-dir",.    "-
+000013b0: 7022 2c0a 2020 2020 6865 6c70 3d22 5061  p",.    help="Pa
+000013c0: 7468 2074 6f20 7079 7468 6f6e 2070 6163  th to python pac
+000013d0: 6b61 6765 2e22 2c0a 2020 2020 6465 6661  kage.",.    defa
+000013e0: 756c 743d 2222 2c0a 290a 6465 6620 6d61  ult="",.).def ma
+000013f0: 696e 280a 2020 2020 7061 636b 6167 653a  in(.    package:
+00001400: 2054 7261 7665 7273 6162 6c65 2c0a 2020   Traversable,.  
+00001410: 2020 6f75 7470 7574 3a20 5061 7468 207c    output: Path |
+00001420: 204e 6f6e 652c 0a20 2020 2066 6f72 6d61   None,.    forma
+00001430: 743a 204c 6974 6572 616c 5b22 7269 6368  t: Literal["rich
+00001440: 222c 2022 6a73 6f6e 222c 2022 6874 6d6c  ", "json", "html
+00001450: 225d 2c0a 2020 2020 7365 6c65 6374 3a20  "],.    select: 
+00001460: 7374 722c 0a20 2020 2069 676e 6f72 653a  str,.    ignore:
+00001470: 2073 7472 2c0a 2020 2020 7061 636b 6167   str,.    packag
+00001480: 655f 6469 723a 2073 7472 2c0a 2920 2d3e  e_dir: str,.) ->
+00001490: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
+000014a0: 2020 2050 6173 7320 696e 2061 206c 6f63     Pass in a loc
+000014b0: 616c 2050 6174 6820 6f72 2067 683a 6f72  al Path or gh:or
+000014c0: 672f 7265 706f 4062 7261 6e63 682e 0a20  g/repo@branch.. 
+000014d0: 2020 2022 2222 0a20 2020 2069 676e 6f72     """.    ignor
+000014e0: 655f 6c69 7374 203d 207b 782e 7374 7269  e_list = {x.stri
+000014f0: 7028 2920 666f 7220 7820 696e 2069 676e  p() for x in ign
+00001500: 6f72 652e 7370 6c69 7428 222c 2229 2069  ore.split(",") i
+00001510: 6620 787d 0a20 2020 2073 656c 6563 745f  f x}.    select_
+00001520: 6c69 7374 203d 207b 782e 7374 7269 7028  list = {x.strip(
+00001530: 2920 666f 7220 7820 696e 2073 656c 6563  ) for x in selec
+00001540: 742e 7370 6c69 7428 222c 2229 2069 6620  t.split(",") if 
+00001550: 787d 0a0a 2020 2020 5f2c 2063 6865 636b  x}..    _, check
+00001560: 732c 205f 203d 205f 636f 6c6c 6563 745f  s, _ = _collect_
+00001570: 616c 6c28 7061 636b 6167 652c 2073 7562  all(package, sub
+00001580: 6469 723d 7061 636b 6167 655f 6469 7229  dir=package_dir)
+00001590: 0a20 2020 2069 6620 6c65 6e28 6368 6563  .    if len(chec
+000015a0: 6b73 2920 3d3d 2030 3a0a 2020 2020 2020  ks) == 0:.      
+000015b0: 2020 6d73 6720 3d20 224e 6f20 6368 6563    msg = "No chec
+000015c0: 6b73 2072 6567 6973 7465 7265 642e 2050  ks registered. P
+000015d0: 6c65 6173 6520 696e 7374 616c 6c20 6120  lease install a 
+000015e0: 7265 706f 2d72 6576 6965 7720 706c 7567  repo-review plug
+000015f0: 696e 2e22 0a20 2020 2020 2020 2072 6169  in.".        rai
+00001600: 7365 2063 6c69 636b 2e43 6c69 636b 4578  se click.ClickEx
+00001610: 6365 7074 696f 6e28 6d73 6729 0a0a 2020  ception(msg)..  
+00001620: 2020 6966 2073 7472 2870 6163 6b61 6765    if str(package
+00001630: 292e 7374 6172 7473 7769 7468 2822 6768  ).startswith("gh
+00001640: 3a22 293a 0a20 2020 2020 2020 205f 2c20  :"):.        _, 
+00001650: 6f72 675f 7265 706f 5f62 7261 6e63 682c  org_repo_branch,
+00001660: 202a 7020 3d20 7374 7228 7061 636b 6167   *p = str(packag
+00001670: 6529 2e73 706c 6974 2822 3a22 2c20 6d61  e).split(":", ma
+00001680: 7873 706c 6974 3d32 290a 2020 2020 2020  xsplit=2).      
+00001690: 2020 6f72 675f 7265 706f 2c20 6272 616e    org_repo, bran
+000016a0: 6368 203d 206f 7267 5f72 6570 6f5f 6272  ch = org_repo_br
+000016b0: 616e 6368 2e73 706c 6974 2822 4022 2c20  anch.split("@", 
+000016c0: 6d61 7873 706c 6974 3d31 290a 2020 2020  maxsplit=1).    
+000016d0: 2020 2020 7061 636b 6167 6520 3d20 4748      package = GH
+000016e0: 5061 7468 2872 6570 6f3d 6f72 675f 7265  Path(repo=org_re
+000016f0: 706f 2c20 6272 616e 6368 3d62 7261 6e63  po, branch=branc
+00001700: 682c 2070 6174 683d 705b 305d 2069 6620  h, path=p[0] if 
+00001710: 7020 656c 7365 2022 2229 0a20 2020 2020  p else "").     
+00001720: 2020 2069 6620 666f 726d 6174 203d 3d20     if format == 
+00001730: 2272 6963 6822 3a0a 2020 2020 2020 2020  "rich":.        
+00001740: 2020 2020 7269 6368 2e70 7269 6e74 2866      rich.print(f
+00001750: 225b 626f 6c64 5d50 726f 6365 7373 696e  "[bold]Processin
+00001760: 6720 5b62 6c75 655d 7b70 6163 6b61 6765  g [blue]{package
+00001770: 7d5b 2f62 6c75 655d 2066 726f 6d20 4769  }[/blue] from Gi
+00001780: 7448 7562 5c6e 2229 0a0a 2020 2020 6661  tHub\n")..    fa
+00001790: 6d69 6c69 6573 2c20 7072 6f63 6573 7365  milies, processe
+000017a0: 6420 3d20 7072 6f63 6573 7328 0a20 2020  d = process(.   
+000017b0: 2020 2020 2070 6163 6b61 6765 2c20 7365       package, se
+000017c0: 6c65 6374 3d73 656c 6563 745f 6c69 7374  lect=select_list
+000017d0: 2c20 6967 6e6f 7265 3d69 676e 6f72 655f  , ignore=ignore_
+000017e0: 6c69 7374 2c20 7375 6264 6972 3d70 6163  list, subdir=pac
+000017f0: 6b61 6765 5f64 6972 0a20 2020 2029 0a0a  kage_dir.    )..
+00001800: 2020 2020 6966 2066 6f72 6d61 7420 3d3d      if format ==
+00001810: 2022 7269 6368 223a 0a20 2020 2020 2020   "rich":.       
+00001820: 2072 6963 685f 7072 696e 7465 7228 6661   rich_printer(fa
+00001830: 6d69 6c69 6573 2c20 7072 6f63 6573 7365  milies, processe
+00001840: 642c 206f 7574 7075 743d 6f75 7470 7574  d, output=output
+00001850: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+00001860: 2870 726f 6365 7373 6564 2920 3d3d 2030  (processed) == 0
+00001870: 3a0a 2020 2020 2020 2020 2020 2020 7269  :.            ri
+00001880: 6368 2e70 7269 6e74 2822 5b62 6f6c 6420  ch.print("[bold 
+00001890: 7265 645d 4e6f 2063 6865 636b 7320 7261  red]No checks ra
+000018a0: 6e5b 2f62 6f6c 6420 7265 645d 2229 0a20  n[/bold red]"). 
+000018b0: 2020 2065 6c69 6620 666f 726d 6174 203d     elif format =
+000018c0: 3d20 226a 736f 6e22 3a0a 2020 2020 2020  = "json":.      
+000018d0: 2020 6a20 3d20 6a73 6f6e 2e64 756d 7073    j = json.dumps
+000018e0: 280a 2020 2020 2020 2020 2020 2020 7b22  (.            {"
+000018f0: 6661 6d69 6c69 6573 223a 2066 616d 696c  families": famil
+00001900: 6965 732c 2022 6368 6563 6b73 223a 2061  ies, "checks": a
+00001910: 735f 7369 6d70 6c65 5f64 6963 7428 7072  s_simple_dict(pr
+00001920: 6f63 6573 7365 6429 7d2c 2069 6e64 656e  ocessed)}, inden
+00001930: 743d 320a 2020 2020 2020 2020 290a 2020  t=2.        ).  
+00001940: 2020 2020 2020 6966 206f 7574 7075 743a        if output:
+00001950: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00001960: 7075 742e 7772 6974 655f 7465 7874 286a  put.write_text(j
+00001970: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00001980: 2020 2020 2020 2020 2020 2020 7269 6368              rich
+00001990: 2e70 7269 6e74 5f6a 736f 6e28 6a29 0a20  .print_json(j). 
+000019a0: 2020 2065 6c69 6620 666f 726d 6174 203d     elif format =
+000019b0: 3d20 2268 746d 6c22 3a0a 2020 2020 2020  = "html":.      
+000019c0: 2020 6874 6d6c 203d 2074 6f5f 6874 6d6c    html = to_html
+000019d0: 2866 616d 696c 6965 732c 2070 726f 6365  (families, proce
+000019e0: 7373 6564 290a 2020 2020 2020 2020 6966  ssed).        if
+000019f0: 206f 7574 7075 743a 0a20 2020 2020 2020   output:.       
+00001a00: 2020 2020 206f 7574 7075 742e 7772 6974       output.writ
+00001a10: 655f 7465 7874 2868 746d 6c29 0a20 2020  e_text(html).   
+00001a20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00001a30: 2020 2020 2020 2072 6963 682e 7072 696e         rich.prin
+00001a40: 7428 6874 6d6c 290a 0a20 2020 2069 6620  t(html)..    if 
+00001a50: 616e 7928 702e 7265 7375 6c74 2069 7320  any(p.result is 
+00001a60: 4661 6c73 6520 666f 7220 7020 696e 2070  False for p in p
+00001a70: 726f 6365 7373 6564 293a 0a20 2020 2020  rocessed):.     
+00001a80: 2020 2072 6169 7365 2053 7973 7465 6d45     raise SystemE
+00001a90: 7869 7428 3229 0a20 2020 2069 6620 6c65  xit(2).    if le
+00001aa0: 6e28 7072 6f63 6573 7365 6429 203d 3d20  n(processed) == 
+00001ab0: 303a 0a20 2020 2020 2020 2072 6169 7365  0:.        raise
+00001ac0: 2053 7973 7465 6d45 7869 7428 3229 0a0a   SystemExit(2)..
+00001ad0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00001ae0: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
+00001af0: 6d61 696e 2829 2020 2320 7079 6c69 6e74  main()  # pylint
+00001b00: 3a20 6469 7361 626c 653d 6e6f 2d76 616c  : disable=no-val
+00001b10: 7565 2d66 6f72 2d70 6172 616d 6574 6572  ue-for-parameter
+00001b20: 0a                                       .
```

### Comparing `repo_review-0.7.0b2/src/repo_review/fixtures.py` & `repo_review-0.7.0b3/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/src/repo_review/ghpath.py` & `repo_review-0.7.0b3/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/src/repo_review/processor.py` & `repo_review-0.7.0b3/src/repo_review/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from __future__ import annotations
 
 import dataclasses
 import graphlib
 import textwrap
 import typing
-from collections.abc import Sequence
+from collections.abc import Set
+from typing import Any
 
 import markdown_it
 
 from ._compat.importlib.resources.abc import Traversable
 from .checks import Check, collect_checks, is_allowed
 from .families import Family, collect_families
 from .fixtures import apply_fixtures, collect_fixtures, compute_fixtures, pyproject
 
-__all__ = ["Result", "ResultDict", "ProcessReturn", "process", "as_simple_dict"]
+__all__ = [
+    "Result",
+    "ResultDict",
+    "ProcessReturn",
+    "process",
+    "as_simple_dict",
+    "_collect_all",
+]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 md = markdown_it.MarkdownIt()
@@ -47,16 +55,43 @@
 
 
 class ProcessReturn(typing.NamedTuple):
     families: dict[str, Family]
     results: list[Result]
 
 
+def _collect_all(
+    root: Traversable, subdir: str = ""
+) -> tuple[dict[str, Any], dict[str, Check], dict[str, Family]]:
+    package = root.joinpath(subdir) if subdir else root
+
+    # Collect the fixtures
+    fixture_functions = collect_fixtures()
+    fixtures = compute_fixtures(root, package, fixture_functions)
+
+    # Collect the checks
+    checks = collect_checks(fixtures)
+
+    # Collect families.
+    families = collect_families()
+
+    # These are optional, so fill in missing families.
+    for name in {c.family for c in checks.values()}:
+        if name not in families:
+            families[name] = Family()
+
+    return fixtures, checks, families
+
+
 def process(
-    root: Traversable, *, ignore: Sequence[str] = (), subdir: str = ""
+    root: Traversable,
+    *,
+    select: Set[str] = frozenset(),
+    ignore: Set[str] = frozenset(),
+    subdir: str = "",
 ) -> ProcessReturn:
     """
     Process the package and return a dictionary of results.
 
     Parameters
     ----------
     root: Traversable | Path
@@ -64,40 +99,23 @@
 
     ignore: Sequence[str]
         A list of checks to ignore
 
     subidr: str
         The path to the package in the subdirectory, if not at the root of the repository.
     """
-
     package = root.joinpath(subdir) if subdir else root
 
-    # Collect the fixtures
-    fixture_functions = collect_fixtures()
-    fixtures = compute_fixtures(root, package, fixture_functions)
-
-    # Collect the checks
-    checks = collect_checks(fixtures)
-
-    # Collect families.
-    families = collect_families()
-
-    # These are optional, so fill in missing families.
-    for name in {c.family for c in checks.values()}:
-        if name not in families:
-            families[name] = Family()
+    fixtures, tasks, families = _collect_all(root, subdir)
 
     # Collect our own config
     config = pyproject(package).get("tool", {}).get("repo-review", {})
-    skip_checks = set(ignore) | set(config.get("ignore", ()))
+    select_checks = select if select else set(config.get("select", ()))
+    skip_checks = ignore if ignore else set(config.get("ignore", ()))
 
-    # Make list of filtered checks to run
-    tasks: dict[str, Check] = {
-        n: r for n, r in checks.items() if is_allowed(skip_checks, n)
-    }
     # Make a graph of the check's interdependencies
     graph: dict[str, set[str]] = {
         n: getattr(t, "requires", set()) for n, t in tasks.items()
     }
     # Keep track of which checks have been completed
     completed: dict[str, str | None] = {}
 
@@ -119,21 +137,24 @@
         tasks.items(),
         key=lambda x: (families[x[1].family].get("order", 0), x[1].family, x[0]),
     ):
         result = None if completed[task_name] is None else not completed[task_name]
         doc = check.__doc__ or ""
         err_msg = completed[task_name] or ""
 
+        if not is_allowed(select_checks, skip_checks, task_name):
+            continue
+
         result_list.append(
             Result(
                 family=check.family,
                 name=task_name,
                 description=doc,
                 result=result,
-                err_msg=textwrap.dedent(err_msg.format(cls=check)),
+                err_msg=textwrap.dedent(err_msg.format(self=check, name=task_name)),
                 url=getattr(check, "url", ""),
             )
         )
 
     return ProcessReturn(families, result_list)
```

### Comparing `repo_review-0.7.0b2/tests/test_checks.py` & `repo_review-0.7.0b3/tests/test_checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,32 +94,54 @@
 
 def test_ignore_filter_single(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"D100": D100, "D200": D200},
     )
-    _, results = repo_review.processor.process(Path("."), ignore=["D100"])
+    _, results = repo_review.processor.process(Path("."), ignore={"D100"})
 
     assert len(results) == 1
     assert results[0].name == "D200"
     assert results[0].result
 
 
 def test_ignore_filter_letter(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"D100": D100(), "D200": D200()},
     )
-    _, results = repo_review.processor.process(Path("."), ignore=["D"])
+    _, results = repo_review.processor.process(Path("."), ignore={"D"})
 
     assert not results
 
 
+def test_select_filter_letter(monkeypatch: pytest.MonkeyPatch) -> None:
+    monkeypatch.setattr(
+        repo_review.processor,
+        "collect_checks",
+        lambda _: {"D100": D100(), "D200": D200(), "C100": C100(fail=True)},
+    )
+    _, results = repo_review.processor.process(Path("."), select={"D"})
+
+    assert len(results) == 2
+
+
+def test_select_filter_exact(monkeypatch: pytest.MonkeyPatch) -> None:
+    monkeypatch.setattr(
+        repo_review.processor,
+        "collect_checks",
+        lambda _: {"D100": D100(), "D200": D200()},
+    )
+    _, results = repo_review.processor.process(Path("."), select={"D100"})
+
+    assert len(results) == 1
+
+
 def test_string_result(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(
         repo_review.processor,
         "collect_checks",
         lambda _: {"C100": C100(fail=False), "C101": C100(fail=True)},
     )
     _, results = repo_review.processor.process(Path("."))
```

### Comparing `repo_review-0.7.0b2/tests/test_fixtures.py` & `repo_review-0.7.0b3/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/tests/test_package.py` & `repo_review-0.7.0b3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/tests/test_self.py` & `repo_review-0.7.0b3/tests/test_self.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,13 +58,13 @@
     assert len(results) == 9
 
     assert (
         sum(result.result is None for result in results if result.family == "pyproject")
         == 1
     )
     assert (
-        sum(result.result for result in results if isinstance(result.result, bool)) == 4
+        sum(result.result for result in results if isinstance(result.result, bool)) == 6
     )
     assert (
         sum(result.result is None for result in results if result.family == "general")
         == 0
     )
```

### Comparing `repo_review-0.7.0b2/tests/test_utilities/pyproject.py` & `repo_review-0.7.0b3/tests/test_utilities/pyproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     family = "pyproject"
 
 
 class PP002(PyProject):
     "Has a proper build-system table"
 
     requires = {"PY001"}
+    url = "https://packaging.python.org/en/latest/specifications/declaring-build-dependencies"
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Must have `build-system.requires` *and* `build-system.backend`. Both
         should be present in all modern packages.
         """
```

### Comparing `repo_review-0.7.0b2/.gitignore` & `repo_review-0.7.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/LICENSE` & `repo_review-0.7.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b2/README.md` & `repo_review-0.7.0b3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,56 @@
 
 [![Actions Status][actions-badge]][actions-link]
 [![Code style: black][black-badge]][black-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
-This tool can check the style of a repository. Use like this:
+<!-- SPHINX-START -->
 
-```bash
-pipx run 'repo-review[cli]' <path to repository>
+This is a framework for building checks designed to check to see if a
+repository follows guidelines. By itself, it does nothing - it requires at
+least one plugin to be installed..
+
+With one or more plugins, it will produce a list of results - green checkmarks
+mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
+means that the check was skipped because a previous required check failed.
+
+`sp-repo-review` provides checks based on the
+[Scientific-Python Development Guide][] at [scientific-python/cookie][].
+
+## Running repo-review
+
+Repo-review supports running multiple ways:
+
+- From the command line on a local folder
+- From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
+- From WebAssembly in Pyodide (example in `docs/index.html`)
+
+If the root of a package is not the repository root, pass `--package-dir a/b/c`.
+
+## Configuration
+
+Repo-review supports configuration via `pyproject.toml`:
+
+```toml
+[tool.repo-review]
+select = ["A", "B", "C100"]
+ignore = ["A100"]
 ```
 
-This will produce a list of results - green checkmarks mean this rule is
-followed, red x’s mean the rule is not. A yellow warning sign means that the
-check was skipped because a previous required check failed.
-
-Checks are defined by plugins. `sp-repo-review` provides checks based on
-the [Scientific-Python Development Pages][] at [scientific-python/cookie][].
-
-### Development
-
-This repository is intended to be fun to develop - it requires and uses Python
-3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
-entirely conventional, but it's fun.
+If `--select` or `--ignore` are given on the command line, they will override
+the `pyproject.toml` config.
+
+## Development of repo-review and plugins
+
+This repository is intended to be fun and easy to develop - it requires and uses
+Python 3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
+entirely conventional, but it enables very simple plugin development. It works
+locally, remotely, and in WebAssembly (using Pyodide).
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
@@ -54,24 +78,27 @@
 cached.
 
 The runner will topologically sort the checks, and checks that do not run will
 get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
-# Links
+## Links
 
 This project inspired [Try-PyHF](https://kratsg.github.io/try-pyhf/), an
 interface for a High Energy Physics package in Scikit-HEP.
 
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
 
+This was developed for [Scikit-HEP][] before moving to Scientific-Python.
+
 [actions-badge]: https://github.com/scientific-python/repo-review/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/repo-review/actions
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
 [pypi-link]: https://pypi.org/project/repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/repo-review
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
-[scientific-python development guidelines]: https://learn.scientific-python.org/development
+[scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
+[scikit-hep]: https://scikit-hep.org
```

### Comparing `repo_review-0.7.0b2/pyproject.toml` & `repo_review-0.7.0b3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
 name = "repo_review"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 license = { file = "LICENSE" }
 
-description = "Review repos for compliance to the Scikit-HEP developer guidelines"
+description = "Framework that can run checks on repos"
 readme = "README.md"
 
 requires-python = ">=3.10"
 
 classifiers = [
   "License :: OSI Approved :: BSD License",
   "Topic :: Scientific/Engineering",
@@ -38,20 +38,28 @@
   "markdown-it-py",
 ]
 
 [project.optional-dependencies]
 cli = [
   "click>=8",
   "rich>=12.2",
+  "rich-click",
 ]
 test = [
   "pytest >=7",
 ]
 dev = [
-  "pytest >=7",
+  "repo-review[test,cli]",
+]
+docs = [
+  "repo-review[cli]",
+  "furo",
+  "myst_parser >=0.13",
+  "sphinx >=4.0",
+  "sphinxcontrib-programoutput",
 ]
 
 [project.urls]
 homepage = "https://github.com/scientific-python/repo-review"
 webpage = "https://scientific-python.github.io/repo-review"
 
 [project.scripts]
@@ -74,27 +82,29 @@
   'ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest',
 ]
 testpaths = ["tests"]
 pythonpath = ["tests/test_utilities"]
 
 
 [tool.mypy]
+mypy_path = ["src"]
 files = ["src", "web", "tests"]
 python_version = "3.10"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 
 [[tool.mypy.overrides]]
 module = "repo_review.*"
 disallow_untyped_defs = true
 
+
 [tool.pylint]
 master.py-version = "3.10"
 master.ignore-paths= ["src/repo_review/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
@@ -104,14 +114,15 @@
   "redefined-builtin",
   "missing-module-docstring",
   "missing-class-docstring",
   "missing-function-docstring",
   "invalid-name",
   "redefined-outer-name",
   "no-member",  # better handled by mypy, etc.
+  "used-before-assignment",  # False positive on conditional import
 ]
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
   "B", "B904",   # flake8-bugbear
```

### Comparing `repo_review-0.7.0b2/PKG-INFO` & `repo_review-0.7.0b3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b2
-Summary: Review repos for compliance to the Scikit-HEP developer guidelines
+Version: 0.7.0b3
+Summary: Framework that can run checks on repos
 Project-URL: homepage, https://github.com/scientific-python/repo-review
 Project-URL: webpage, https://scientific-python.github.io/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Henry Schreiner.
         All rights reserved.
@@ -48,47 +48,78 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Requires-Dist: markdown-it-py
 Requires-Dist: pyyaml
 Requires-Dist: tomli; python_version < '3.11'
 Provides-Extra: cli
 Requires-Dist: click>=8; extra == 'cli'
+Requires-Dist: rich-click; extra == 'cli'
 Requires-Dist: rich>=12.2; extra == 'cli'
 Provides-Extra: dev
-Requires-Dist: pytest>=7; extra == 'dev'
+Requires-Dist: repo-review[cli,test]; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: myst-parser>=0.13; extra == 'docs'
+Requires-Dist: repo-review[cli]; extra == 'docs'
+Requires-Dist: sphinx>=4.0; extra == 'docs'
+Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
 
 # repo-review
 
 [![Actions Status][actions-badge]][actions-link]
 [![Code style: black][black-badge]][black-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
-This tool can check the style of a repository. Use like this:
+<!-- SPHINX-START -->
 
-```bash
-pipx run 'repo-review[cli]' <path to repository>
+This is a framework for building checks designed to check to see if a
+repository follows guidelines. By itself, it does nothing - it requires at
+least one plugin to be installed..
+
+With one or more plugins, it will produce a list of results - green checkmarks
+mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
+means that the check was skipped because a previous required check failed.
+
+`sp-repo-review` provides checks based on the
+[Scientific-Python Development Guide][] at [scientific-python/cookie][].
+
+## Running repo-review
+
+Repo-review supports running multiple ways:
+
+- From the command line on a local folder
+- From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
+- From WebAssembly in Pyodide (example in `docs/index.html`)
+
+If the root of a package is not the repository root, pass `--package-dir a/b/c`.
+
+## Configuration
+
+Repo-review supports configuration via `pyproject.toml`:
+
+```toml
+[tool.repo-review]
+select = ["A", "B", "C100"]
+ignore = ["A100"]
 ```
 
-This will produce a list of results - green checkmarks mean this rule is
-followed, red x’s mean the rule is not. A yellow warning sign means that the
-check was skipped because a previous required check failed.
-
-Checks are defined by plugins. `sp-repo-review` provides checks based on
-the [Scientific-Python Development Pages][] at [scientific-python/cookie][].
-
-### Development
-
-This repository is intended to be fun to develop - it requires and uses Python
-3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
-entirely conventional, but it's fun.
+If `--select` or `--ignore` are given on the command line, they will override
+the `pyproject.toml` config.
+
+## Development of repo-review and plugins
+
+This repository is intended to be fun and easy to develop - it requires and uses
+Python 3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
+entirely conventional, but it enables very simple plugin development. It works
+locally, remotely, and in WebAssembly (using Pyodide).
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
@@ -115,24 +146,27 @@
 cached.
 
 The runner will topologically sort the checks, and checks that do not run will
 get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
-# Links
+## Links
 
 This project inspired [Try-PyHF](https://kratsg.github.io/try-pyhf/), an
 interface for a High Energy Physics package in Scikit-HEP.
 
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
 
+This was developed for [Scikit-HEP][] before moving to Scientific-Python.
+
 [actions-badge]: https://github.com/scientific-python/repo-review/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/repo-review/actions
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
 [pypi-link]: https://pypi.org/project/repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/repo-review
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
-[scientific-python development guidelines]: https://learn.scientific-python.org/development
+[scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
+[scikit-hep]: https://scikit-hep.org
```

