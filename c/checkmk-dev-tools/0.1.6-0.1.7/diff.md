# Comparing `tmp/checkmk_dev_tools-0.1.6.tar.gz` & `tmp/checkmk_dev_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmk_dev_tools-0.1.6.tar", max compression
+gzip compressed data, was "checkmk_dev_tools-0.1.7.tar", max compression
```

## Comparing `checkmk_dev_tools-0.1.6.tar` & `checkmk_dev_tools-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1056 2023-05-31 14:32:38.730307 checkmk_dev_tools-0.1.6/README.rst
--rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.6/cmk_dev/__init__.py
--rwxr-xr-x   0        0        0    13820 2023-06-05 07:24:31.924090 checkmk_dev_tools-0.1.6/cmk_dev/ci_artifacts.py
--rwxr-xr-x   0        0        0     2184 2023-05-10 11:28:30.476996 checkmk_dev_tools-0.1.6/cmk_dev/cli.py
--rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.6/cmk_dev/listen_std.py
--rw-r--r--   0        0        0     1919 2023-06-05 09:34:19.663050 checkmk_dev_tools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-06-05 17:25:55.667846 checkmk_dev_tools-0.1.7/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.7/cmk_dev/__init__.py
+-rwxr-xr-x   0        0        0    20158 2023-06-05 17:14:33.207269 checkmk_dev_tools-0.1.7/cmk_dev/ci_artifacts.py
+-rwxr-xr-x   0        0        0     2184 2023-06-05 16:21:12.072374 checkmk_dev_tools-0.1.7/cmk_dev/cli.py
+-rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.7/cmk_dev/listen_std.py
+-rw-r--r--   0        0        0     2179 2023-06-05 17:20:06.805662 checkmk_dev_tools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.7/PKG-INFO
```

### Comparing `checkmk_dev_tools-0.1.6/cmk_dev/cli.py` & `checkmk_dev_tools-0.1.7/cmk_dev/cli.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.6/cmk_dev/listen_std.py` & `checkmk_dev_tools-0.1.7/cmk_dev/listen_std.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.6/pyproject.toml` & `checkmk_dev_tools-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 [tool.poetry]
 name = "checkmk-dev-tools"
-version = "0.1.6"
+version = "0.1.7"
 description = "Checkmk DevOps tools"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/tribe29/checkmk"
-readme = "README.rst"
+readme = "Readme.md"
 packages = [
   {include = "cmk_dev/**/*.py"}
 ]
 exclude = ["cmk_dev/out"]
 
 [tool.poetry.scripts]
 cmk-dev = 'cmk_dev.cli:main'
 active-listen = 'cmk_dev.listen_std:main'
 ci-artifacts = 'cmk_dev.ci_artifacts:main'
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 python-jenkins = "^1.8.0"
+pyyaml = "^6.0"
 
-[tool.poetry.dev-dependencies]
-yamllint = "^1.29.0"
+[tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 mypy = "^1.2"
 pylint = "^2.15.3"
 ipython = "^8.8.0"
 types-pyyaml = "^6.0.12.6"
-
+twine = "^4.0.2"
+yamllint = "^1.29.0"
+pylint-per-file-ignores = "^1.2.1"
+types-requests = "^2.31.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
@@ -67,21 +70,27 @@
 warn_return_any = "True"
 warn_unused_ignores = "True"
 show_error_codes = "True"
 exclude = [
     '\.venv',
     '\.container_home_dir',
 ]
+mypy_path="typeshed"
 
 [tool.pylint]
-ignore = [".venv", "untracked"]
+#ignore = [".venv", "untracked"]
 
 # Files or directories matching the regular expression patterns are skipped. The
 # regex matches against base names, not paths. The default value ignores Emacs
 # file locks
-ignore-patterns = ["^\\.#"]
+#ignore-patterns = ["^\\.#"]
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
 # avoid hangs.
-jobs = 1
+jobs = 0
+
+[tool.pylint.MASTER]
+load-plugins=["pylint_per_file_ignores"]
 
+[tool.pylint-per-file-ignores]
+"pocketrockit/examples/" = "invalid-name"
```

