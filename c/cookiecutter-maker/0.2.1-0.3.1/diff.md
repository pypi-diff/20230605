# Comparing `tmp/cookiecutter_maker-0.2.1.tar.gz` & `tmp/cookiecutter_maker-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_maker-0.2.1.tar", last modified: Tue Feb 21 00:59:11 2023, max compression
+gzip compressed data, was "cookiecutter_maker-0.3.1.tar", last modified: Mon Jun  5 00:24:16 2023, max compression
```

## Comparing `cookiecutter_maker-0.2.1.tar` & `cookiecutter_maker-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-21 00:59:11.910910 cookiecutter_maker-0.2.1/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1128 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      326 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     6039 2023-02-21 00:59:11.910752 cookiecutter_maker-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     4879 2023-02-21 00:58:03.000000 cookiecutter_maker-0.2.1/README.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)       32 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/chore.txt
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-21 00:59:11.909499 cookiecutter_maker-0.2.1/cookiecutter_maker/
--rw-r--r--   0 sanhehu    (505) staff       (20)      327 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/cookiecutter_maker/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-02-21 00:46:11.000000 cookiecutter_maker-0.2.1/cookiecutter_maker/_version.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-21 00:59:11.910519 cookiecutter_maker-0.2.1/cookiecutter_maker/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/cookiecutter_maker/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     7042 2023-02-21 00:40:15.000000 cookiecutter_maker-0.2.1/cookiecutter_maker/maker.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      461 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/cookiecutter_maker/strutils.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-21 00:59:11.910249 cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     6039 2023-02-21 00:59:11.000000 cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      532 2023-02-21 00:59:11.000000 cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-02-21 00:59:11.000000 cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      171 2023-02-21 00:59:11.000000 cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       19 2023-02-21 00:59:11.000000 cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      683 2023-02-21 00:44:01.000000 cookiecutter_maker-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      289 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      183 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        0 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-02-21 00:59:11.910961 cookiecutter_maker-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7713 2023-02-15 16:08:21.000000 cookiecutter_maker-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-05 00:24:16.995371 cookiecutter_maker-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1128 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      326 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6574 2023-06-05 00:24:16.995233 cookiecutter_maker-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5465 2023-06-05 00:21:45.000000 cookiecutter_maker-0.3.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/chore.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-05 00:24:16.993372 cookiecutter_maker-0.3.1/cookiecutter_maker/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      263 2023-06-04 22:26:11.000000 cookiecutter_maker-0.3.1/cookiecutter_maker/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-04 21:36:16.000000 cookiecutter_maker-0.3.1/cookiecutter_maker/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-04 22:26:24.000000 cookiecutter_maker-0.3.1/cookiecutter_maker/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-05 00:24:16.994276 cookiecutter_maker-0.3.1/cookiecutter_maker/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/cookiecutter_maker/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       75 2023-06-04 22:14:17.000000 cookiecutter_maker-0.3.1/cookiecutter_maker/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10718 2023-06-05 00:19:00.000000 cookiecutter_maker-0.3.1/cookiecutter_maker/maker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1234 2023-06-04 22:25:52.000000 cookiecutter_maker-0.3.1/cookiecutter_maker/strutils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-05 00:24:16.994157 cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6574 2023-06-05 00:24:16.000000 cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      648 2023-06-05 00:24:16.000000 cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-05 00:24:16.000000 cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-05 00:24:16.000000 cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       19 2023-06-05 00:24:16.000000 cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1093 2023-06-05 00:23:06.000000 cookiecutter_maker-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      289 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-06-04 21:35:24.000000 cookiecutter_maker-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-05 00:24:16.995419 cookiecutter_maker-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7664 2023-06-05 00:17:34.000000 cookiecutter_maker-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-05 00:24:16.994944 cookiecutter_maker-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-04 22:45:21.000000 cookiecutter_maker-0.3.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5133 2023-06-05 00:21:37.000000 cookiecutter_maker-0.3.1/tests/test_maker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1041 2023-06-04 22:47:49.000000 cookiecutter_maker-0.3.1/tests/test_stringutils.py
```

### Comparing `cookiecutter_maker-0.2.1/LICENSE.txt` & `cookiecutter_maker-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cookiecutter_maker-0.2.1/PKG-INFO` & `cookiecutter_maker-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cookiecutter_maker
-Version: 0.2.1
+Version: 0.3.1
 Summary: Convert any git repo into a cookiecutter projects template.
 Home-page: https://github.com/MacHu-GWU/cookiecutter_maker-project
-Download-URL: https://pypi.python.org/pypi/cookiecutter_maker/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/cookiecutter_maker/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -15,27 +15,26 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 
-.. image:: https://readthedocs.org/projects/cookiecutter_maker/badge/?version=latest
+.. .. image:: https://readthedocs.org/projects/cookiecutter_maker/badge/?version=latest
     :target: https://cookiecutter_maker.readthedocs.io/index.html
     :alt: Documentation Status
 
 .. image:: https://github.com/MacHu-GWU/cookiecutter_maker-project/workflows/CI/badge.svg
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/cookiecutter_maker-project/branch/main/graph/badge.svg
@@ -52,21 +51,21 @@
 
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project
 
 ------
 
 
-.. image:: https://img.shields.io/badge/Link-Document-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/index.html
 
-.. image:: https://img.shields.io/badge/Link-API-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-API-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/py-modindex.html
 
-.. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
     :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project
@@ -94,28 +93,29 @@
 
 Usage Example
 ------------------------------------------------------------------------------
 Run the following python script to convert your concrete project into a template project:
 
 .. code-block:: python
 
-    from cookiecutter_maker.maker import Maker
+    from cookiecutter_maker.api import Maker
 
     maker = Maker.new(
         # the input concrete project directory
         input_dir="/path-to-input-dir/my_awesome_project",
         # the output template project directory
         output_dir="/path-to-output-dir",
-        # define the pair of ``concrete string`` and ``parameter name``
+        # define the ``string to replace``, ``parameter name`` and ``default parameter value``
         mapper=[
-            ("my_awesome_project", "package_name"),
+            ("my_awesome_project", "package_name", "default_package_name"),
         ],
         # define what to include in the input directory
         # it is the relative path from the input directory
         # the rule is 'explicit exclude' > 'explicit include' > 'default include'
+        # if empty, then include all files and directories
         include=[],
         # define what to exclude in the input directory
         # it is the relative path from the input directory
         exclude=[
             # dir
             ".venv",
             ".pytest_cache",
@@ -123,16 +123,27 @@
             ".idea",
             "build",
             "dist",
             "htmlcov",
             # file
             ".coverage",
         ],
+        # define what to copy as it is without rending
+        # usually you should ignore jinja template files
+        no_render=[
+            "*.tpl",
+        ],
         # over write the output location if already exists
         overwrite=True,
+        # mapper could have one key is substring of another key
+        # if this is True, it will ignore the error
+        ignore_mapper_error=False,
+        # when mapper could have one key is substring of another key
+        # it will prompt you to confirm to continue
+        skip_mapper_prompt=True,
         # do you want to print debug information?
         debug=True,
     )
     maker.templaterize()
 
 In this example, it will create a directory ``{{ cookiecutter.package_name }}`` and a json file ``cookiecutter.json``. Now you can follow the `cookiecutter instruction <https://cookiecutter.readthedocs.io>`_ to generate more concrete projects.
```

### Comparing `cookiecutter_maker-0.2.1/README.rst` & `cookiecutter_maker-0.3.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-.. image:: https://readthedocs.org/projects/cookiecutter_maker/badge/?version=latest
+.. .. image:: https://readthedocs.org/projects/cookiecutter_maker/badge/?version=latest
     :target: https://cookiecutter_maker.readthedocs.io/index.html
     :alt: Documentation Status
 
 .. image:: https://github.com/MacHu-GWU/cookiecutter_maker-project/workflows/CI/badge.svg
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/cookiecutter_maker-project/branch/main/graph/badge.svg
@@ -20,21 +20,21 @@
 
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project
 
 ------
 
 
-.. image:: https://img.shields.io/badge/Link-Document-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/index.html
 
-.. image:: https://img.shields.io/badge/Link-API-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-API-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/py-modindex.html
 
-.. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
     :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project
@@ -62,28 +62,29 @@
 
 Usage Example
 ------------------------------------------------------------------------------
 Run the following python script to convert your concrete project into a template project:
 
 .. code-block:: python
 
-    from cookiecutter_maker.maker import Maker
+    from cookiecutter_maker.api import Maker
 
     maker = Maker.new(
         # the input concrete project directory
         input_dir="/path-to-input-dir/my_awesome_project",
         # the output template project directory
         output_dir="/path-to-output-dir",
-        # define the pair of ``concrete string`` and ``parameter name``
+        # define the ``string to replace``, ``parameter name`` and ``default parameter value``
         mapper=[
-            ("my_awesome_project", "package_name"),
+            ("my_awesome_project", "package_name", "default_package_name"),
         ],
         # define what to include in the input directory
         # it is the relative path from the input directory
         # the rule is 'explicit exclude' > 'explicit include' > 'default include'
+        # if empty, then include all files and directories
         include=[],
         # define what to exclude in the input directory
         # it is the relative path from the input directory
         exclude=[
             # dir
             ".venv",
             ".pytest_cache",
@@ -91,16 +92,27 @@
             ".idea",
             "build",
             "dist",
             "htmlcov",
             # file
             ".coverage",
         ],
+        # define what to copy as it is without rending
+        # usually you should ignore jinja template files
+        no_render=[
+            "*.tpl",
+        ],
         # over write the output location if already exists
         overwrite=True,
+        # mapper could have one key is substring of another key
+        # if this is True, it will ignore the error
+        ignore_mapper_error=False,
+        # when mapper could have one key is substring of another key
+        # it will prompt you to confirm to continue
+        skip_mapper_prompt=True,
         # do you want to print debug information?
         debug=True,
     )
     maker.templaterize()
 
 In this example, it will create a directory ``{{ cookiecutter.package_name }}`` and a json file ``cookiecutter.json``. Now you can follow the `cookiecutter instruction <https://cookiecutter.readthedocs.io>`_ to generate more concrete projects.
 
@@ -116,8 +128,8 @@
 
     $ pip install cookiecutter_maker
 
 To upgrade to latest version:
 
 .. code-block:: console
 
-    $ pip install --upgrade cookiecutter_maker
+    $ pip install --upgrade cookiecutter_maker
```

### Comparing `cookiecutter_maker-0.2.1/cookiecutter_maker/maker.py` & `cookiecutter_maker-0.3.1/cookiecutter_maker/maker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 
 import json
+import shutil
 import dataclasses
 from pathlib import Path
 from collections import OrderedDict
 
-from .strutils import replace
+from .exc import MapperValidationError
+from .strutils import validate_mapper, replace
 
 
 @dataclasses.dataclass
 class Maker:
+    """
+    Cookiecutter maker.
+    """
+
     input_dir: Path = dataclasses.field()
     output_dir: Path = dataclasses.field()
-    mapper: T.List[T.Tuple[str, str]] = dataclasses.field()
+    mapper: T.List[T.Tuple[str, str, str]] = dataclasses.field()
     processed_mapper: T.List[T.Tuple[str, str]] = dataclasses.field()
     include: T.List[str] = dataclasses.field(default_factory=list)
     exclude: T.List[str] = dataclasses.field(default_factory=list)
     no_render: T.List[str] = dataclasses.field(default_factory=list)
     overwrite: T.Optional[bool] = dataclasses.field(default=False)
     debug: bool = dataclasses.field(default=False)
 
@@ -26,165 +32,249 @@
     _after_dir: T.Optional[Path] = dataclasses.field(default=None)
 
     @classmethod
     def new(
         cls,
         input_dir: T.Union[str, Path],
         output_dir: T.Union[str, Path],
-        mapper: T.List[T.Tuple[str, str]],
+        mapper: T.List[T.Tuple[str, str, str]],
         include: T.Optional[T.List[str]] = None,
         exclude: T.Optional[T.List[str]] = None,
         no_render: T.Optional[T.List[str]] = None,
         overwrite: bool = False,
+        ignore_mapper_error: bool = False,
+        skip_mapper_prompt: bool = False,
         debug: bool = False,
         _skip_validate: bool = False,
     ):
+        """
+        Create a new :class:`Maker` instance.
+
+        :param input_dir: the directory you want to templaterize.
+        :param output_dir: where to put the generated template project?
+        :param mapper: a list of tuple. each tuple include three items. 1 is the
+            concrete string you want to replace, 2 is the parameter name, 3 is the
+            default value for cookiecutter to prompt user to input.
+        :param include: list of file path pattern that we include from the input dir
+            if empty, we include all files and directories.
+        :param exclude: list of file path pattern that we exclude from the input dir
+        :param no_render: list of file path pattern that we copy it without
+            rendering (as it is)
+        :param overwrite: allow overwrite the output dir if already exists
+        :param ignore_mapper_error: ignore mapper validation error
+        :param skip_mapper_prompt: skip prompt asking you to confirm the mapper
+        :param debug: if True, show debug info
+        :param _skip_validate: internal use only, don't set this parameter.
+        """
         maker = cls(
             input_dir=cls._preprocess_input_dir(input_dir, _skip_validate),
             output_dir=cls._preprocess_output_dir(output_dir),
             mapper=mapper,
-            processed_mapper=cls._preprocess_mapper(mapper),
+            processed_mapper=cls._preprocess_mapper(
+                mapper,
+                ignore_mapper_error=ignore_mapper_error,
+                skip_mapper_prompt=skip_mapper_prompt,
+            ),
             include=cls._preprocess_include(include),
             exclude=cls._preprocess_exclude(exclude),
             no_render=cls._preprocess_no_render(no_render),
             overwrite=overwrite,
             debug=debug,
         )
         maker._after_dir = maker.output_dir.joinpath(
             replace(maker.input_dir.name, maker.processed_mapper)
         )
         return maker
 
+    # --------------------------------------------------------------------------
+    # preprocess arguments
+    # --------------------------------------------------------------------------
     @classmethod
     def _preprocess_input_dir(
         cls,
         input_dir: T.Union[str, Path],
         _skip_validate: bool = False,
     ) -> Path:
         if isinstance(input_dir, str):
             input_dir = Path(input_dir)
         if _skip_validate is False:
             if input_dir.exists() is False:
-                raise ValueError(f"Input directory {input_dir!r} does not exist!!")
+                raise FileNotFoundError(
+                    f"Input directory {input_dir!r} does not exist!!"
+                )
         return input_dir
 
     @classmethod
-    def _preprocess_output_dir(cls, output_dir: T.Union[str, Path]) -> Path:
+    def _preprocess_output_dir(
+        cls,
+        output_dir: T.Union[str, Path],
+    ) -> Path:
         if isinstance(output_dir, str):
             output_dir = Path(output_dir)
         return output_dir
 
     @classmethod
     def _preprocess_mapper(
         cls,
-        mapper: T.List[T.Tuple[str, str]],
+        mapper: T.List[T.Tuple[str, str, str]],
+        ignore_mapper_error: bool = False,
+        skip_mapper_prompt: bool = False,
     ) -> T.List[T.Tuple[str, str]]:
         if len(mapper) == 0:
             raise ValueError("mapper cannot be empty")
+
         dict_mapper = OrderedDict()
+        # handle {{ and }} string
         dict_mapper["{{"] = "{% raw %}{{{% endraw %}"
         dict_mapper["}}"] = "{% raw %}}}{% endraw %}"
-        for before, after in mapper:
+        for before, after, _ in mapper:
             dict_mapper[before] = f"{{{{ cookiecutter.{after} }}}}"
         list_mapper = [(k, v) for k, v in dict_mapper.items()]
+
+        try:
+            validate_mapper(list_mapper)
+        except MapperValidationError as e:
+            if ignore_mapper_error:
+                return list_mapper
+            if skip_mapper_prompt:
+                return list_mapper
+            else:  # pragma: no cover
+                answer = input(
+                    f"{e}\n"
+                    f"I suggest to put substring later than the super string in mapper\n"
+                    f"Are you sure to continue? [y/n]: "
+                )
+                if answer.lower() in ["y", "yes"]:
+                    return list_mapper
+                else:
+                    raise e
+        except Exception as e:  # pragma: no cover
+            raise e
         return list_mapper
 
     @classmethod
     def _preprocess_include(
         cls,
         include: T.Optional[T.List[str]],
-    ) -> T.List[str]:
+    ) -> T.List[str]:  # pragma: no cover
         if include is None:
             include = list()
         return include
 
     @classmethod
     def _preprocess_exclude(
         cls,
         exclude: T.Optional[T.List[str]],
-    ) -> T.List[str]:
+    ) -> T.List[str]:  # pragma: no cover
         if exclude is None:
             exclude = list()
         return exclude
 
     @classmethod
     def _preprocess_no_render(
         cls,
         no_render: T.Optional[T.List[str]],
-    ) -> T.List[str]:
+    ) -> T.List[str]:  # pragma: no cover
         if no_render is None:
             no_render = list()
+        # *.jinja template itself is a template file,
+        # most likely you don't want to render it.
         no_render.append("*.jinja")
         return no_render
 
-    def _do_we_ignore(self, relpath: Path) -> bool:
-        if len(self.include):
-            match_include = False
-            for pattern in self.include:
-                if relpath.match(pattern):
-                    match_include = True
-                    break
-        else:
+    def _do_we_ignore(
+        self,
+        relpath: Path,
+        is_dir: bool
+    ) -> bool:
+        """
+        Based on the include and exclude pattern, do we ignore this file?
+
+        It has to match include rule and not match exclude rule.
+
+        If include is empty, it considered as "match include rule".
+
+        If exclude is empty, it considered as "not match exclude rule".
+        """
+        if is_dir:
             match_include = True
+        else:
+            if len(self.include):
+                match_include = False
+                for pattern in self.include:
+                    if relpath.match(pattern):
+                        match_include = True
+                        break
+            else: # pragma: no cover
+                match_include = True
 
         match_exclude = False
         for pattern in self.exclude:
             if relpath.match(pattern):
                 match_exclude = True
                 break
 
         if match_include:
             return match_exclude
         else:
-            return False
+            return True
 
     def _do_we_render(self, relpath: Path) -> bool:
         for pattern in self.no_render:
             if relpath.match(pattern):
                 return False
         return True
 
     def _templaterize_file(self, p_before: Path) -> T.Optional[Path]:
+        """
+        Create a templaterized file in the output directory.
+        """
         relpath = p_before.relative_to(self.input_dir)
 
-        if self._do_we_ignore(relpath):
+        if self._do_we_ignore(relpath, is_dir=False):
             return None
 
         new_relpath = replace(str(relpath), self.processed_mapper)
         p_after = self._after_dir.joinpath(new_relpath)
 
         if p_after.exists():
             if self.overwrite is False:
-                raise ValueError(
+                raise FileExistsError(
                     f"File already exists: {p_after!r}! maybe use 'overwrite = True'!"
                 )
 
         if self.debug:
             # print(f"{str(p_before):<160} -> {str(p_after)}")
             print(f"{p_before} -> {p_after}")
 
         if self._do_we_render(relpath) is False:
             p_after.write_bytes(p_before.read_bytes())
             return p_after
 
+        # handle binary content files
+        b = p_before.read_bytes()
+
         try:
-            b = p_before.read_bytes()
             s = b.decode("utf-8")
         except UnicodeDecodeError:
+            # copy binary file as it is
             p_after.write_bytes(b)
             return p_after
 
         text = replace(s, self.processed_mapper)
         p_after.write_text(text)
         return p_after
 
     def _templaterize_dir(self, p_before: Path) -> T.Optional[Path]:
+        """
+        Create a templaterized directory in the output directory (empty folder).
+        """
         relpath = p_before.relative_to(self.input_dir)
 
-        if self._do_we_ignore(relpath):
+        if self._do_we_ignore(relpath, is_dir=True):
             return None
 
         new_relpath = replace(str(relpath), self.processed_mapper)
         p_after = self._after_dir.joinpath(new_relpath)
         if self.debug:
             # print(f"{str(p_before):<160} -> {str(p_after)}")
             print(f"{p_before} -> {p_after}")
@@ -198,26 +288,31 @@
         """
         Recursively templaterize a directory.
         """
         p_after = self._templaterize_dir(dir_src)
 
         if (
             p_after is None
-        ):  # if this dir is ignored, then no need to work on subfolders and files
+        ):  # if this dir is ignored, then no need to work on sub-folders and files
             return
 
         for p in dir_src.iterdir():
             if p.is_dir():
                 self._templaterize(p)
             elif p.is_file():
                 self._templaterize_file(p)
-            else:
+            else:  # pragma: no cover
                 pass
 
         path_cookiecutter_json = self.output_dir.joinpath("cookiecutter.json")
         cookiecutter_json_data = dict()
-        for concrete_string, parameter_name in self.mapper:
+        for _, parameter_name, concrete_string in self.mapper:
             cookiecutter_json_data[parameter_name] = concrete_string
         path_cookiecutter_json.write_text(json.dumps(cookiecutter_json_data, indent=4))
 
-    def templaterize(self):
+    def templaterize(
+        self,
+        cleanup_output_dir: bool = False,
+    ):
+        if cleanup_output_dir:
+            shutil.rmtree(self.output_dir, ignore_errors=True)
         self._templaterize(dir_src=self.input_dir)
```

### Comparing `cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/PKG-INFO` & `cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cookiecutter-maker
-Version: 0.2.1
+Version: 0.3.1
 Summary: Convert any git repo into a cookiecutter projects template.
 Home-page: https://github.com/MacHu-GWU/cookiecutter_maker-project
-Download-URL: https://pypi.python.org/pypi/cookiecutter_maker/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/cookiecutter_maker/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -15,27 +15,26 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 
-.. image:: https://readthedocs.org/projects/cookiecutter_maker/badge/?version=latest
+.. .. image:: https://readthedocs.org/projects/cookiecutter_maker/badge/?version=latest
     :target: https://cookiecutter_maker.readthedocs.io/index.html
     :alt: Documentation Status
 
 .. image:: https://github.com/MacHu-GWU/cookiecutter_maker-project/workflows/CI/badge.svg
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/cookiecutter_maker-project/branch/main/graph/badge.svg
@@ -52,21 +51,21 @@
 
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project
 
 ------
 
 
-.. image:: https://img.shields.io/badge/Link-Document-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/index.html
 
-.. image:: https://img.shields.io/badge/Link-API-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-API-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/py-modindex.html
 
-.. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
+.. .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
     :target: https://cookiecutter_maker.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
     :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
     :target: https://github.com/MacHu-GWU/cookiecutter_maker-project
@@ -94,28 +93,29 @@
 
 Usage Example
 ------------------------------------------------------------------------------
 Run the following python script to convert your concrete project into a template project:
 
 .. code-block:: python
 
-    from cookiecutter_maker.maker import Maker
+    from cookiecutter_maker.api import Maker
 
     maker = Maker.new(
         # the input concrete project directory
         input_dir="/path-to-input-dir/my_awesome_project",
         # the output template project directory
         output_dir="/path-to-output-dir",
-        # define the pair of ``concrete string`` and ``parameter name``
+        # define the ``string to replace``, ``parameter name`` and ``default parameter value``
         mapper=[
-            ("my_awesome_project", "package_name"),
+            ("my_awesome_project", "package_name", "default_package_name"),
         ],
         # define what to include in the input directory
         # it is the relative path from the input directory
         # the rule is 'explicit exclude' > 'explicit include' > 'default include'
+        # if empty, then include all files and directories
         include=[],
         # define what to exclude in the input directory
         # it is the relative path from the input directory
         exclude=[
             # dir
             ".venv",
             ".pytest_cache",
@@ -123,16 +123,27 @@
             ".idea",
             "build",
             "dist",
             "htmlcov",
             # file
             ".coverage",
         ],
+        # define what to copy as it is without rending
+        # usually you should ignore jinja template files
+        no_render=[
+            "*.tpl",
+        ],
         # over write the output location if already exists
         overwrite=True,
+        # mapper could have one key is substring of another key
+        # if this is True, it will ignore the error
+        ignore_mapper_error=False,
+        # when mapper could have one key is substring of another key
+        # it will prompt you to confirm to continue
+        skip_mapper_prompt=True,
         # do you want to print debug information?
         debug=True,
     )
     maker.templaterize()
 
 In this example, it will create a directory ``{{ cookiecutter.package_name }}`` and a json file ``cookiecutter.json``. Now you can follow the `cookiecutter instruction <https://cookiecutter.readthedocs.io>`_ to generate more concrete projects.
```

### Comparing `cookiecutter_maker-0.2.1/cookiecutter_maker.egg-info/SOURCES.txt` & `cookiecutter_maker-0.3.1/cookiecutter_maker.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 requirements-dev.txt
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 cookiecutter_maker/__init__.py
 cookiecutter_maker/_version.py
+cookiecutter_maker/api.py
+cookiecutter_maker/exc.py
 cookiecutter_maker/maker.py
 cookiecutter_maker/strutils.py
 cookiecutter_maker.egg-info/PKG-INFO
 cookiecutter_maker.egg-info/SOURCES.txt
 cookiecutter_maker.egg-info/dependency_links.txt
 cookiecutter_maker.egg-info/requires.txt
 cookiecutter_maker.egg-info/top_level.txt
-cookiecutter_maker/docs/__init__.py
+cookiecutter_maker/docs/__init__.py
+tests/test_api.py
+tests/test_maker.py
+tests/test_stringutils.py
```

### Comparing `cookiecutter_maker-0.2.1/requirements-doc.txt` & `cookiecutter_maker-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `cookiecutter_maker-0.2.1/setup.py` & `cookiecutter_maker-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ]
     """
```

