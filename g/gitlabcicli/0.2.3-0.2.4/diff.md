# Comparing `tmp/gitlabcicli-0.2.3.tar.gz` & `tmp/gitlabcicli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabcicli-0.2.3.tar", max compression
+gzip compressed data, was "gitlabcicli-0.2.4.tar", max compression
```

## Comparing `gitlabcicli-0.2.3.tar` & `gitlabcicli-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35069 2018-09-09 00:49:12.046406 gitlabcicli-0.2.3/LICENSE
--rw-r--r--   0        0        0      293 2020-05-01 18:06:58.428742 gitlabcicli-0.2.3/gitlabcicli/__init__.py
--rwxr-xr-x   0        0        0      210 2018-07-13 18:47:25.212540 gitlabcicli-0.2.3/gitlabcicli/__main__.py
--rw-r--r--   0        0        0        0 2020-05-04 21:16:19.337317 gitlabcicli-0.2.3/gitlabcicli/api/__init__.py
--rw-r--r--   0        0        0     2134 2023-04-27 09:33:10.249630 gitlabcicli-0.2.3/gitlabcicli/api/gitlab_api_driver.py
--rw-r--r--   0        0        0       98 2020-05-01 22:50:56.147701 gitlabcicli-0.2.3/gitlabcicli/api/models/__init__.py
--rw-r--r--   0        0        0     1485 2023-04-27 09:28:50.094831 gitlabcicli-0.2.3/gitlabcicli/api/models/pipeline.py
--rw-r--r--   0        0        0     3936 2023-04-27 09:30:07.811935 gitlabcicli-0.2.3/gitlabcicli/api/models/project.py
--rw-r--r--   0        0        0     6929 2021-03-31 17:20:49.085504 gitlabcicli-0.2.3/gitlabcicli/gitlabapiwrapper.py
--rwxr-xr-x   0        0        0    19468 2023-04-27 09:33:06.459609 gitlabcicli-0.2.3/gitlabcicli/gitlabcicli.py
--rw-r--r--   0        0        0     2442 2021-03-31 17:43:41.430511 gitlabcicli-0.2.3/gitlabcicli/gitwrapper.py
--rw-r--r--   0        0        0      423 2020-12-08 14:07:42.199276 gitlabcicli-0.2.3/gitlabcicli/managerlib/__init__.py
--rw-r--r--   0        0        0     4531 2023-04-27 09:31:07.458938 gitlabcicli-0.2.3/gitlabcicli/managerlib/api_driver.py
--rw-r--r--   0        0        0      469 2020-05-04 22:08:08.496965 gitlabcicli-0.2.3/gitlabcicli/managerlib/errors.py
--rw-r--r--   0        0        0     7252 2023-04-27 09:33:46.186499 gitlabcicli-0.2.3/gitlabcicli/managerlib/fields.py
--rw-r--r--   0        0        0     3880 2023-04-27 09:29:47.421820 gitlabcicli-0.2.3/gitlabcicli/managerlib/model.py
--rw-r--r--   0        0        0      691 2023-04-27 09:31:41.092461 gitlabcicli-0.2.3/gitlabcicli/managerlib/utils.py
--rw-r--r--   0        0        0     1004 2020-11-13 21:40:57.960798 gitlabcicli-0.2.3/gitlabcicli/script_helpers.py
--rw-r--r--   0        0        0      268 2020-12-08 14:07:42.239276 gitlabcicli-0.2.3/gitlabcicli/utils.py
--rw-r--r--   0        0        0      727 2023-04-27 09:27:37.697756 gitlabcicli-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 gitlabcicli-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35069 2018-09-09 00:49:12.046406 gitlabcicli-0.2.4/LICENSE
+-rw-r--r--   0        0        0      293 2020-05-01 18:06:58.428742 gitlabcicli-0.2.4/gitlabcicli/__init__.py
+-rwxr-xr-x   0        0        0      210 2018-07-13 18:47:25.212540 gitlabcicli-0.2.4/gitlabcicli/__main__.py
+-rw-r--r--   0        0        0        0 2020-05-04 21:16:19.337317 gitlabcicli-0.2.4/gitlabcicli/api/__init__.py
+-rw-r--r--   0        0        0     2134 2023-04-27 09:33:10.249630 gitlabcicli-0.2.4/gitlabcicli/api/gitlab_api_driver.py
+-rw-r--r--   0        0        0       98 2020-05-01 22:50:56.147701 gitlabcicli-0.2.4/gitlabcicli/api/models/__init__.py
+-rw-r--r--   0        0        0     1485 2023-04-27 09:28:50.094831 gitlabcicli-0.2.4/gitlabcicli/api/models/pipeline.py
+-rw-r--r--   0        0        0     3936 2023-04-27 09:30:07.811935 gitlabcicli-0.2.4/gitlabcicli/api/models/project.py
+-rw-r--r--   0        0        0     6929 2021-03-31 17:20:49.085504 gitlabcicli-0.2.4/gitlabcicli/gitlabapiwrapper.py
+-rwxr-xr-x   0        0        0    19805 2023-06-05 16:45:25.037104 gitlabcicli-0.2.4/gitlabcicli/gitlabcicli.py
+-rw-r--r--   0        0        0     2442 2021-03-31 17:43:41.430511 gitlabcicli-0.2.4/gitlabcicli/gitwrapper.py
+-rw-r--r--   0        0        0      423 2020-12-08 14:07:42.199276 gitlabcicli-0.2.4/gitlabcicli/managerlib/__init__.py
+-rw-r--r--   0        0        0     4531 2023-04-27 09:31:07.458938 gitlabcicli-0.2.4/gitlabcicli/managerlib/api_driver.py
+-rw-r--r--   0        0        0      469 2020-05-04 22:08:08.496965 gitlabcicli-0.2.4/gitlabcicli/managerlib/errors.py
+-rw-r--r--   0        0        0     7246 2023-05-28 20:20:46.579857 gitlabcicli-0.2.4/gitlabcicli/managerlib/fields.py
+-rw-r--r--   0        0        0     3880 2023-04-27 09:29:47.421820 gitlabcicli-0.2.4/gitlabcicli/managerlib/model.py
+-rw-r--r--   0        0        0      691 2023-04-27 09:31:41.092461 gitlabcicli-0.2.4/gitlabcicli/managerlib/utils.py
+-rw-r--r--   0        0        0     1004 2020-11-13 21:40:57.960798 gitlabcicli-0.2.4/gitlabcicli/script_helpers.py
+-rw-r--r--   0        0        0      268 2020-12-08 14:07:42.239276 gitlabcicli-0.2.4/gitlabcicli/utils.py
+-rw-r--r--   0        0        0      704 2023-06-05 16:46:10.460607 gitlabcicli-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 gitlabcicli-0.2.4/PKG-INFO
```

### Comparing `gitlabcicli-0.2.3/LICENSE` & `gitlabcicli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/api/gitlab_api_driver.py` & `gitlabcicli-0.2.4/gitlabcicli/api/gitlab_api_driver.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/api/models/pipeline.py` & `gitlabcicli-0.2.4/gitlabcicli/api/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/api/models/project.py` & `gitlabcicli-0.2.4/gitlabcicli/api/models/project.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/gitlabapiwrapper.py` & `gitlabcicli-0.2.4/gitlabcicli/gitlabapiwrapper.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/gitlabcicli.py` & `gitlabcicli-0.2.4/gitlabcicli/gitlabcicli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """Command line interface for GitLab CI."""
 
 import argparse
 import os
 import sys
 import typing
+import webbrowser
 from dataclasses import dataclass
 from functools import cached_property
 from getpass import getpass
 from pathlib import Path
 
 import keyring
 from tabulate import tabulate
@@ -334,24 +335,38 @@
 
     @cached_property
     def token(self) -> str:
         """The secret API token."""
 
         if self.args.get("ask_for_token"):
             debug("Try to get token from user input...", 2)
-            self._token = getpass(
-                f"Please enter the GitLab API Token for {self.server_url}: "
+            cprint(
+                "Generate a new token here:"
+                f" {self.server_url}-/profile/personal_access_tokens",
+                color="cyan",
             )
+            try:
+                self._token = getpass(
+                    colored(
+                        f"Please enter the GitLab API Token for {self.server_url}: ",
+                        attrs=["bold"],
+                    )
+                )
+            except (EOFError, KeyboardInterrupt):
+                print()
+                error("Interrupted")
+                exit(1)
         elif not self._token:
             debug("Try to get token for server from config...", 2)
             self._token = get_token_from_keyring(self.server_url)
 
         if not self._token:
             error(
-                "No token found in wallet or given. Please use --ask-for-token to specify your token."
+                "No token found in wallet or given."
+                " Please use --ask-for-token to specify your token."
             )
             sys.exit(501)
 
         debug(f"Using token {self._token}", 5)
 
         return self._token
 
@@ -450,15 +465,14 @@
             debug(response, 5)
 
             if not response:
                 error(
                     f"Could not {self.args['job_action']} job #{job_id} for project '{self.project}'."
                 )
             else:
-                past = {"cancel": "canceled", "retry": "retried", "erase": "erased"}
                 cprint(
                     f"Successfully {self.args['job_action']} job #{job_id} for project '{self.project}'",
                     color="green",
                     attrs=["bold"],
                 )
 
                 if self.args["job_action"] == "retry":
@@ -492,15 +506,15 @@
             for error_description in api["errors"]:
                 print(f" - {error_description}")
 
     @register_command(aliases={"web"})
     def open(self):
         """Open the current project in browser."""
         url = self.api_client.get_project_url(self.project_id)
-        os.system(f"xdg-open {url}")
+        webbrowser.open(url)
 
     @register_command(aliases={"exec"})
     def run_local(self):
         """Run pipeline on local machine."""
         raise NotImplementedError(
             "run_local is not yet implemented. Contribution is welcome."
         )
@@ -654,29 +668,29 @@
         type=argparse.FileType("r"),
         default=".gitlab-ci.yml",
         nargs="?",
         help="The gitlab-ci.yml",
     ).completer = gitlabciyml_completer
 
     # open
-    parser_open = subparsers.add_parser(
+    subparsers.add_parser(
         "open",
         aliases=COMMANDS["open"].aliases,
         help="Open the current project in your browser.",
     )
 
     # run local
-    parser_run_local = subparsers.add_parser(
+    subparsers.add_parser(
         "run-local",
         aliases=COMMANDS["run-local"].aliases,
         help="Run a stage on the local machine.",
     )
 
     # init
-    parser_init = subparsers.add_parser(
+    subparsers.add_parser(
         "init",
         aliases=COMMANDS["init"].aliases,
         help="Create a .gitlab-ci.yml",
     )
 
     if argcomplete:
         argcomplete.autocomplete(parser)
```

### Comparing `gitlabcicli-0.2.3/gitlabcicli/gitwrapper.py` & `gitlabcicli-0.2.4/gitlabcicli/gitwrapper.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/managerlib/api_driver.py` & `gitlabcicli-0.2.4/gitlabcicli/managerlib/api_driver.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/managerlib/fields.py` & `gitlabcicli-0.2.4/gitlabcicli/managerlib/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 
     @abstractproperty
     def python_type(self):
         """Return the corresponding python type."""
 
 
 class StrField(Field):
-
     python_type = str
 
     def clean(self, value, **kwargs):
         if value is not None:
             try:
                 value = str(value)
             except (ValueError, TypeError) as err:
@@ -88,15 +87,14 @@
 
         value = super().clean(value, **kwargs)
 
         return value
 
 
 class IntField(Field):
-
     python_type = int
 
     def clean(self, value, **kwargs):
         if value is not None:
             try:
                 value = int(value)
             except (ValueError, TypeError) as err:
@@ -118,15 +116,14 @@
                 else "Value must not be smaller than zero."
             )
 
         return value
 
 
 class BoolField(Field):
-
     python_type = bool
 
     def clean(self, value, **kwargs):
         if value is not None:
             try:
                 value = bool(value)
             except ValueError as err:
@@ -134,15 +131,14 @@
 
         value = super().clean(value, **kwargs)
 
         return value
 
 
 class StrIntField(Field):
-
     field = None
     python_type = None
 
     def clean(self, value, **kwargs):
         errs = []
         try:
             field = IntField(
@@ -223,15 +219,14 @@
 
         value = [clean_subvalue(entry, _field_name=_field_name) for entry in value]
 
         return value
 
 
 class DateField(Field):
-
     python_type = date
 
     def clean(self, value, **kwargs):
         if value is None:
             pass
         elif isinstance(value, date):
             pass
@@ -244,15 +239,14 @@
 
         value = super().clean(value, **kwargs)
 
         return value
 
 
 class DateTimeField(Field):
-
     python_type = datetime
 
     def clean(self, value, **kwargs):
         if value is None:
             pass
         elif isinstance(value, datetime):
             pass
```

### Comparing `gitlabcicli-0.2.3/gitlabcicli/managerlib/model.py` & `gitlabcicli-0.2.4/gitlabcicli/managerlib/model.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/managerlib/utils.py` & `gitlabcicli-0.2.4/gitlabcicli/managerlib/utils.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/gitlabcicli/script_helpers.py` & `gitlabcicli-0.2.4/gitlabcicli/script_helpers.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.3/pyproject.toml` & `gitlabcicli-0.2.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "GitLabCICli"
-version = "0.2.3"
+version = "0.2.4"
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
-dbus-python = "^1.3.2"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.28.11.17"
 pylint = "^2.17.3"
 mypy = "^1.2.0"
 black = "^22.12.0"
 pre-commit = "^2.21.0"
```

### Comparing `gitlabcicli-0.2.3/PKG-INFO` & `gitlabcicli-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: gitlabcicli
-Version: 0.2.3
+Version: 0.2.4
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
-Requires-Dist: dbus-python (>=1.3.2,<2.0.0)
 Requires-Dist: keyring (>=21.8.0,<22.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: tabulate (>=0.8.10,<0.9.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/sedrubal/gitlabcicli.git
```

