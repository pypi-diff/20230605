# Comparing `tmp/poetry_plugin_tweak_dependencies_version-1.3.0.tar.gz` & `tmp/poetry_plugin_tweak_dependencies_version-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_tweak_dependencies_version-1.3.0.tar", max compression
+gzip compressed data, was "poetry_plugin_tweak_dependencies_version-1.4.0.tar", max compression
```

## Comparing `poetry_plugin_tweak_dependencies_version-1.3.0.tar` & `poetry_plugin_tweak_dependencies_version-1.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1289 2023-03-02 17:32:19.071446 poetry_plugin_tweak_dependencies_version-1.3.0/LICENSE
--rw-r--r--   0        0        0      791 2023-03-02 17:32:19.071446 poetry_plugin_tweak_dependencies_version-1.3.0/README.md
--rw-r--r--   0        0        0     8908 2023-03-02 17:32:19.071446 poetry_plugin_tweak_dependencies_version-1.3.0/poetry_plugin_tweak_dependencies_version/__init__.py
--rw-r--r--   0        0        0     1374 2023-03-02 17:33:49.486917 poetry_plugin_tweak_dependencies_version-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 poetry_plugin_tweak_dependencies_version-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1289 2023-06-05 07:11:56.476182 poetry_plugin_tweak_dependencies_version-1.4.0/LICENSE
+-rw-r--r--   0        0        0      917 2023-06-05 07:11:56.476182 poetry_plugin_tweak_dependencies_version-1.4.0/README.md
+-rw-r--r--   0        0        0     8908 2023-06-05 07:11:56.476182 poetry_plugin_tweak_dependencies_version-1.4.0/poetry_plugin_tweak_dependencies_version/__init__.py
+-rw-r--r--   0        0        0     1375 2023-06-05 07:14:53.298833 poetry_plugin_tweak_dependencies_version-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 poetry_plugin_tweak_dependencies_version-1.4.0/PKG-INFO
```

### Comparing `poetry_plugin_tweak_dependencies_version-1.3.0/LICENSE` & `poetry_plugin_tweak_dependencies_version-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_tweak_dependencies_version-1.3.0/README.md` & `poetry_plugin_tweak_dependencies_version-1.4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -17,7 +17,16 @@
 default = "(present|major|minor|patch|full)" # Default to `full`
 "<package>" = "(present|major|minor|patch|full|<alternate>)"
 
 ```
 
 `present` => `*`, `major` => `x.*`, `minor` => `x.y.*`, `patch` => `x.y.z`, `full` => keep the original version.
 Or just specify an alternate version constraint.
+
+## Contributing
+
+Install the pre-commit hooks:
+
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
```

### Comparing `poetry_plugin_tweak_dependencies_version-1.3.0/poetry_plugin_tweak_dependencies_version/__init__.py` & `poetry_plugin_tweak_dependencies_version-1.4.0/poetry_plugin_tweak_dependencies_version/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_tweak_dependencies_version-1.3.0/pyproject.toml` & `poetry_plugin_tweak_dependencies_version-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 target-version = ['py38']
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "poetry-plugin-tweak-dependencies-version"
-version = "1.3.0"
+version = "1.4.0"
 description = "Poetry plugin used to tweak dependency versions"
 readme = "README.md"
 repository = "https://github.com/sbrunner/poetry-plugin-tweak-dependencies-version"
 keywords = ["poetry", "plugin", "version", "versioning", "dynamic"]
 authors = ["Stéphane Brunner <stephane.brunner@camptocamp.com>"]
 license = "BSD-2-Clause"
 classifiers = [
@@ -22,19 +22,19 @@
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-poetry = "==1.4.*"
+poetry = "==1.5.*"
 
 [tool.poetry.dev-dependencies]
 # pylint = "2.15.6"
-prospector = { version = "1.9.0", extras = ["with_bandit", "with_mypy", "with_pyroma"] }
+prospector = { version = "1.10.2", extras = ["with_bandit", "with_mypy", "with_pyroma"] }
 
 [tool.poetry.plugins."poetry.application.plugin"]
 tweak_dependencies_version = "poetry_plugin_tweak_dependencies_version:Plugin"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `poetry_plugin_tweak_dependencies_version-1.3.0/PKG-INFO` & `poetry_plugin_tweak_dependencies_version-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-tweak-dependencies-version
-Version: 1.3.0
+Version: 1.4.0
 Summary: Poetry plugin used to tweak dependency versions
 Home-page: https://github.com/sbrunner/poetry-plugin-tweak-dependencies-version
 License: BSD-2-Clause
 Keywords: poetry,plugin,version,versioning,dynamic
 Author: Stéphane Brunner
 Author-email: stephane.brunner@camptocamp.com
 Requires-Python: >=3.8,<3.12
@@ -15,16 +15,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: poetry (>=1.4.0,<1.5.0)
+Requires-Dist: poetry (==1.5.*)
 Project-URL: Repository, https://github.com/sbrunner/poetry-plugin-tweak-dependencies-version
 Description-Content-Type: text/markdown
 
 # Poetry plugin tweak dependencies version
 
 Plugin use to tweak the dependencies of the project.
 
@@ -44,7 +43,16 @@
 "<package>" = "(present|major|minor|patch|full|<alternate>)"
 
 ```
 
 `present` => `*`, `major` => `x.*`, `minor` => `x.y.*`, `patch` => `x.y.z`, `full` => keep the original version.
 Or just specify an alternate version constraint.
 
+## Contributing
+
+Install the pre-commit hooks:
+
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
+
```

