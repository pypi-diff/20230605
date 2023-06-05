# Comparing `tmp/gitlabcicli-0.2.4.tar.gz` & `tmp/gitlabcicli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabcicli-0.2.4.tar", max compression
+gzip compressed data, was "gitlabcicli-0.2.5.tar", max compression
```

## Comparing `gitlabcicli-0.2.4.tar` & `gitlabcicli-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    35069 2018-09-09 00:49:12.046406 gitlabcicli-0.2.4/LICENSE
--rw-r--r--   0        0        0      293 2020-05-01 18:06:58.428742 gitlabcicli-0.2.4/gitlabcicli/__init__.py
--rwxr-xr-x   0        0        0      210 2018-07-13 18:47:25.212540 gitlabcicli-0.2.4/gitlabcicli/__main__.py
--rw-r--r--   0        0        0        0 2020-05-04 21:16:19.337317 gitlabcicli-0.2.4/gitlabcicli/api/__init__.py
--rw-r--r--   0        0        0     2134 2023-04-27 09:33:10.249630 gitlabcicli-0.2.4/gitlabcicli/api/gitlab_api_driver.py
--rw-r--r--   0        0        0       98 2020-05-01 22:50:56.147701 gitlabcicli-0.2.4/gitlabcicli/api/models/__init__.py
--rw-r--r--   0        0        0     1485 2023-04-27 09:28:50.094831 gitlabcicli-0.2.4/gitlabcicli/api/models/pipeline.py
--rw-r--r--   0        0        0     3936 2023-04-27 09:30:07.811935 gitlabcicli-0.2.4/gitlabcicli/api/models/project.py
--rw-r--r--   0        0        0     6929 2021-03-31 17:20:49.085504 gitlabcicli-0.2.4/gitlabcicli/gitlabapiwrapper.py
--rwxr-xr-x   0        0        0    19805 2023-06-05 16:45:25.037104 gitlabcicli-0.2.4/gitlabcicli/gitlabcicli.py
--rw-r--r--   0        0        0     2442 2021-03-31 17:43:41.430511 gitlabcicli-0.2.4/gitlabcicli/gitwrapper.py
--rw-r--r--   0        0        0      423 2020-12-08 14:07:42.199276 gitlabcicli-0.2.4/gitlabcicli/managerlib/__init__.py
--rw-r--r--   0        0        0     4531 2023-04-27 09:31:07.458938 gitlabcicli-0.2.4/gitlabcicli/managerlib/api_driver.py
--rw-r--r--   0        0        0      469 2020-05-04 22:08:08.496965 gitlabcicli-0.2.4/gitlabcicli/managerlib/errors.py
--rw-r--r--   0        0        0     7246 2023-05-28 20:20:46.579857 gitlabcicli-0.2.4/gitlabcicli/managerlib/fields.py
--rw-r--r--   0        0        0     3880 2023-04-27 09:29:47.421820 gitlabcicli-0.2.4/gitlabcicli/managerlib/model.py
--rw-r--r--   0        0        0      691 2023-04-27 09:31:41.092461 gitlabcicli-0.2.4/gitlabcicli/managerlib/utils.py
--rw-r--r--   0        0        0     1004 2020-11-13 21:40:57.960798 gitlabcicli-0.2.4/gitlabcicli/script_helpers.py
--rw-r--r--   0        0        0      268 2020-12-08 14:07:42.239276 gitlabcicli-0.2.4/gitlabcicli/utils.py
--rw-r--r--   0        0        0      704 2023-06-05 16:46:10.460607 gitlabcicli-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 gitlabcicli-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35069 2018-09-09 00:49:12.046406 gitlabcicli-0.2.5/LICENSE
+-rw-r--r--   0        0        0      293 2020-05-01 18:06:58.428742 gitlabcicli-0.2.5/gitlabcicli/__init__.py
+-rwxr-xr-x   0        0        0      210 2018-07-13 18:47:25.212540 gitlabcicli-0.2.5/gitlabcicli/__main__.py
+-rw-r--r--   0        0        0        0 2020-05-04 21:16:19.337317 gitlabcicli-0.2.5/gitlabcicli/api/__init__.py
+-rw-r--r--   0        0        0     2134 2023-04-27 09:33:10.249630 gitlabcicli-0.2.5/gitlabcicli/api/gitlab_api_driver.py
+-rw-r--r--   0        0        0       98 2020-05-01 22:50:56.147701 gitlabcicli-0.2.5/gitlabcicli/api/models/__init__.py
+-rw-r--r--   0        0        0     1485 2023-04-27 09:28:50.094831 gitlabcicli-0.2.5/gitlabcicli/api/models/pipeline.py
+-rw-r--r--   0        0        0     3936 2023-04-27 09:30:07.811935 gitlabcicli-0.2.5/gitlabcicli/api/models/project.py
+-rw-r--r--   0        0        0     6929 2021-03-31 17:20:49.085504 gitlabcicli-0.2.5/gitlabcicli/gitlabapiwrapper.py
+-rwxr-xr-x   0        0        0    19464 2023-06-05 17:35:36.446759 gitlabcicli-0.2.5/gitlabcicli/gitlabcicli.py
+-rw-r--r--   0        0        0     2442 2021-03-31 17:43:41.430511 gitlabcicli-0.2.5/gitlabcicli/gitwrapper.py
+-rw-r--r--   0        0        0     1105 2023-06-05 18:04:59.411829 gitlabcicli-0.2.5/gitlabcicli/keyring_wrapper.py
+-rw-r--r--   0        0        0      423 2020-12-08 14:07:42.199276 gitlabcicli-0.2.5/gitlabcicli/managerlib/__init__.py
+-rw-r--r--   0        0        0     4531 2023-04-27 09:31:07.458938 gitlabcicli-0.2.5/gitlabcicli/managerlib/api_driver.py
+-rw-r--r--   0        0        0      469 2020-05-04 22:08:08.496965 gitlabcicli-0.2.5/gitlabcicli/managerlib/errors.py
+-rw-r--r--   0        0        0     7246 2023-05-28 20:20:46.579857 gitlabcicli-0.2.5/gitlabcicli/managerlib/fields.py
+-rw-r--r--   0        0        0     3880 2023-04-27 09:29:47.421820 gitlabcicli-0.2.5/gitlabcicli/managerlib/model.py
+-rw-r--r--   0        0        0      691 2023-04-27 09:31:41.092461 gitlabcicli-0.2.5/gitlabcicli/managerlib/utils.py
+-rw-r--r--   0        0        0     1032 2023-06-05 17:40:00.708015 gitlabcicli-0.2.5/gitlabcicli/script_helpers.py
+-rw-r--r--   0        0        0      268 2020-12-08 14:07:42.239276 gitlabcicli-0.2.5/gitlabcicli/utils.py
+-rw-r--r--   0        0        0      752 2023-06-05 18:06:22.845517 gitlabcicli-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 gitlabcicli-0.2.5/PKG-INFO
```

### Comparing `gitlabcicli-0.2.4/LICENSE` & `gitlabcicli-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/api/gitlab_api_driver.py` & `gitlabcicli-0.2.5/gitlabcicli/api/gitlab_api_driver.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/api/models/pipeline.py` & `gitlabcicli-0.2.5/gitlabcicli/api/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/api/models/project.py` & `gitlabcicli-0.2.5/gitlabcicli/api/models/project.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/gitlabapiwrapper.py` & `gitlabcicli-0.2.5/gitlabcicli/gitlabapiwrapper.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/gitlabcicli.py` & `gitlabcicli-0.2.5/gitlabcicli/gitlabcicli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import typing
 import webbrowser
 from dataclasses import dataclass
 from functools import cached_property
 from getpass import getpass
 from pathlib import Path
 
-import keyring
 from tabulate import tabulate
 from termcolor import colored, cprint
 
 import gitlabcicli as info
-from gitlabcicli.gitlabapiwrapper import GitLabApiClient
-from gitlabcicli.gitwrapper import (
+
+from .gitlabapiwrapper import GitLabApiClient
+from .gitwrapper import (
     get_current_commit,
     get_long_commit_sha,
     get_project_name,
     get_server_url,
     get_shas,
 )
-from gitlabcicli.script_helpers import debug, error, set_verbosity
+from .keyring_wrapper import KeyringWrapper
+from .script_helpers import debug, error, set_verbosity
 
 try:
     import argcomplete
 except ImportError:
     argcomplete = None
 
 KNOWN_STATES = {
@@ -100,17 +101,14 @@
         )
 
         return func
 
     return inner
 
 
-KEYRING_SERVICE_NAME = "gitlabcicli"
-
-
 def sha_completer(prefix, **kwargs):
     """tab completion shas in current git"""
 
     return (s[:8] for s in get_shas() if s.startswith(prefix))
 
 
 def gitlabciyml_completer(prefix, **_):
@@ -121,29 +119,14 @@
     return [
         fn
         for fn in files
         if (os.path.isdir(fn) or ".gitlab-ci.yml".startswith(fn.split("/")[-1]))
     ]
 
 
-def get_token_from_keyring(server_url: str) -> str | None:
-    """Retreive the token for current server from keyring."""
-
-    try:
-        return keyring.get_password(KEYRING_SERVICE_NAME, server_url)
-    except Exception as exc:
-        error(
-            "No token found in wallet. Please use --ask-for-token to specify your token."
-        )
-        error(str(exc))
-        sys.exit(500)
-
-    return None
-
-
 def _color_job_status(status):
     """Return the colored job status as string"""
 
     return colored(status, attrs=["bold"], color=KNOWN_STATES[status]["color"])
 
 
 def _color_coverage(coverage):
@@ -255,21 +238,25 @@
         self._api_client: GitLabApiClient | None = None
         self._server_url: str | None = kwargs.get("server_url", None)
         self._project_id: int | None = kwargs.get("project_id", None)
         self._project_path: str | None = kwargs.get("project_path", None)
         self._project: str | None = kwargs.get("project", None)
         self._token: str | None = kwargs.get("token", None)
         self._commit_hash: str | None = kwargs.get("commit_hash", None)
+        self._keyring_wrapper = KeyringWrapper()
         self.args = kwargs
 
     def stop(self):
         """Shutdown."""
 
         if self._token:
-            keyring.set_password(KEYRING_SERVICE_NAME, self.server_url, self._token)
+            self._keyring_wrapper.set_token(
+                server_url=self.server_url,
+                token=self._token,
+            )
 
     @property
     def server_url(self) -> str:
         if not self._server_url:
             debug("Try to get server url from remote of local git repo...", 2)
             self._server_url = get_server_url()
             debug(f"Using server {self._server_url}", 1)
@@ -353,15 +340,15 @@
                 )
             except (EOFError, KeyboardInterrupt):
                 print()
                 error("Interrupted")
                 exit(1)
         elif not self._token:
             debug("Try to get token for server from config...", 2)
-            self._token = get_token_from_keyring(self.server_url)
+            self._token = self._keyring_wrapper.get_token(self.server_url)
 
         if not self._token:
             error(
                 "No token found in wallet or given."
                 " Please use --ask-for-token to specify your token."
             )
             sys.exit(501)
```

### Comparing `gitlabcicli-0.2.4/gitlabcicli/gitwrapper.py` & `gitlabcicli-0.2.5/gitlabcicli/gitwrapper.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/managerlib/api_driver.py` & `gitlabcicli-0.2.5/gitlabcicli/managerlib/api_driver.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/managerlib/fields.py` & `gitlabcicli-0.2.5/gitlabcicli/managerlib/fields.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/managerlib/model.py` & `gitlabcicli-0.2.5/gitlabcicli/managerlib/model.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/managerlib/utils.py` & `gitlabcicli-0.2.5/gitlabcicli/managerlib/utils.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.4/gitlabcicli/script_helpers.py` & `gitlabcicli-0.2.5/gitlabcicli/script_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 def set_verbosity(verbosity):
     """sets the verbosity level of this script"""
     global VERBOSITY
     VERBOSITY = verbosity
 
 
-def error(message):
+def error(message, exit_code: int = 1):
     """prints the message to stderr and exits"""
     cprint(f"[!] {message}", attrs=["bold"], color="red", file=sys.stderr)
-    sys.exit(1)
+    sys.exit(exit_code)
 
 
 def debug(message, min_debug_level):
     """prints the message to stdout if debug level >= min_debug_level"""
     if min_debug_level <= VERBOSITY:
         cprint(
             f"[i] {message}",
```

### Comparing `gitlabcicli-0.2.4/pyproject.toml` & `gitlabcicli-0.2.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "GitLabCICli"
-version = "0.2.4"
+version = "0.2.5"
 description = "Command line interface for GitLab CI"
 authors = ["sedrubal <dev@sedrubal.de>"]
 repository = "https://gitlab.com/sedrubal/gitlabcicli.git"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 argcomplete = "^1.12.3"
 keyring = "^21.8.0"
 requests = "^2.29.0"
 tabulate = "^0.8.10"
 termcolor = "^1.1.0"
 GitPython = "^3.1.31"
+dbus-python = "^1.3.2"
+secretstorage = "^3.3.3"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.28.11.17"
 pylint = "^2.17.3"
 mypy = "^1.2.0"
 black = "^22.12.0"
 pre-commit = "^2.21.0"
```

### Comparing `gitlabcicli-0.2.4/PKG-INFO` & `gitlabcicli-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: gitlabcicli
-Version: 0.2.4
+Version: 0.2.5
 Summary: Command line interface for GitLab CI
 Home-page: https://gitlab.com/sedrubal/gitlabcicli.git
 License: GPL-3.0-or-later
 Author: sedrubal
 Author-email: dev@sedrubal.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: argcomplete (>=1.12.3,<2.0.0)
+Requires-Dist: dbus-python (>=1.3.2,<2.0.0)
 Requires-Dist: keyring (>=21.8.0,<22.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: secretstorage (>=3.3.3,<4.0.0)
 Requires-Dist: tabulate (>=0.8.10,<0.9.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/sedrubal/gitlabcicli.git
```

