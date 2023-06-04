# Comparing `tmp/west-1.0.0a1.tar.gz` & `tmp/west-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "west-1.0.0a1.tar", last modified: Mon Feb 20 17:22:17 2023, max compression
+gzip compressed data, was "west-1.1.0a1.tar", last modified: Fri Jun  2 19:53:16 2023, max compression
```

## Comparing `west-1.0.0a1.tar` & `west-1.1.0a1.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxrwxr-x   0 mbolivar  (1000) mbolivar  (1000)        0 2023-02-20 17:22:17.710883 west-1.0.0a1/
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)    11357 2023-01-05 06:57:58.000000 west-1.0.0a1/LICENSE
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)      105 2023-02-17 23:05:31.000000 west-1.0.0a1/MANIFEST.in
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     4334 2023-02-20 17:22:17.710883 west-1.0.0a1/PKG-INFO
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     3781 2023-01-05 06:57:58.000000 west-1.0.0a1/README.rst
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)       38 2023-02-20 17:22:17.710883 west-1.0.0a1/setup.cfg
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     1567 2023-02-17 23:05:31.000000 west-1.0.0a1/setup.py
-drwxrwxr-x   0 mbolivar  (1000) mbolivar  (1000)        0 2023-02-20 17:22:17.706883 west-1.0.0a1/src/
-drwxrwxr-x   0 mbolivar  (1000) mbolivar  (1000)        0 2023-02-20 17:22:17.706883 west-1.0.0a1/src/west/
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)      204 2023-01-05 06:57:58.000000 west-1.0.0a1/src/west/__init__.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)       39 2023-01-05 06:57:58.000000 west-1.0.0a1/src/west/__main__.py
-drwxrwxr-x   0 mbolivar  (1000) mbolivar  (1000)        0 2023-02-20 17:22:17.706883 west-1.0.0a1/src/west/app/
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)       63 2023-01-05 06:57:58.000000 west-1.0.0a1/src/west/app/__init__.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     7271 2023-02-17 23:05:31.000000 west-1.0.0a1/src/west/app/config.py
--rwxrwxr-x   0 mbolivar  (1000) mbolivar  (1000)    38218 2023-02-17 23:05:31.000000 west-1.0.0a1/src/west/app/main.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)    70675 2023-02-17 23:05:31.000000 west-1.0.0a1/src/west/app/project.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)    24619 2023-02-20 17:16:40.000000 west-1.0.0a1/src/west/commands.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)    23693 2023-02-17 23:05:31.000000 west-1.0.0a1/src/west/configuration.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     6501 2023-02-20 17:17:36.000000 west-1.0.0a1/src/west/log.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     4797 2023-01-05 06:57:58.000000 west-1.0.0a1/src/west/manifest-schema.yml
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)   100727 2023-02-14 04:03:44.000000 west-1.0.0a1/src/west/manifest.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)        0 2023-02-17 23:05:31.000000 west-1.0.0a1/src/west/py.typed
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     2926 2023-01-05 06:57:58.000000 west-1.0.0a1/src/west/util.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)      617 2023-02-20 17:21:53.000000 west-1.0.0a1/src/west/version.py
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     1001 2023-01-05 06:57:58.000000 west-1.0.0a1/src/west/west-commands-schema.yml
-drwxrwxr-x   0 mbolivar  (1000) mbolivar  (1000)        0 2023-02-20 17:22:17.706883 west-1.0.0a1/src/west.egg-info/
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)     4334 2023-02-20 17:22:17.000000 west-1.0.0a1/src/west.egg-info/PKG-INFO
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)      601 2023-02-20 17:22:17.000000 west-1.0.0a1/src/west.egg-info/SOURCES.txt
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)        1 2023-02-20 17:22:17.000000 west-1.0.0a1/src/west.egg-info/dependency_links.txt
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)       44 2023-02-20 17:22:17.000000 west-1.0.0a1/src/west.egg-info/entry_points.txt
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)        1 2023-02-20 17:22:17.000000 west-1.0.0a1/src/west.egg-info/not-zip-safe
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)       52 2023-02-20 17:22:17.000000 west-1.0.0a1/src/west.egg-info/requires.txt
--rw-rw-r--   0 mbolivar  (1000) mbolivar  (1000)        5 2023-02-20 17:22:17.000000 west-1.0.0a1/src/west.egg-info/top_level.txt
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.285008 west-1.1.0a1/
+-rw-r--r--   0 mbolivar   (501) staff       (20)    11357 2021-03-11 03:24:30.000000 west-1.1.0a1/LICENSE
+-rw-r--r--   0 mbolivar   (501) staff       (20)      105 2023-05-01 21:45:22.000000 west-1.1.0a1/MANIFEST.in
+-rw-r--r--   0 mbolivar   (501) staff       (20)     4511 2023-06-02 19:53:16.284880 west-1.1.0a1/PKG-INFO
+-rw-r--r--   0 mbolivar   (501) staff       (20)     3958 2023-05-01 21:45:22.000000 west-1.1.0a1/README.rst
+-rw-r--r--   0 mbolivar   (501) staff       (20)       38 2023-06-02 19:53:16.285047 west-1.1.0a1/setup.cfg
+-rw-r--r--   0 mbolivar   (501) staff       (20)     1567 2023-05-01 21:45:22.000000 west-1.1.0a1/setup.py
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.277415 west-1.1.0a1/src/
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.280625 west-1.1.0a1/src/west/
+-rw-r--r--   0 mbolivar   (501) staff       (20)      204 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/__init__.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)       39 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/__main__.py
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.281948 west-1.1.0a1/src/west/app/
+-rw-r--r--   0 mbolivar   (501) staff       (20)       63 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/app/__init__.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     7271 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/app/config.py
+-rwxr-xr-x   0 mbolivar   (501) staff       (20)    46302 2023-06-02 19:40:31.000000 west-1.1.0a1/src/west/app/main.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    76773 2023-06-02 19:40:31.000000 west-1.1.0a1/src/west/app/project.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    24619 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/commands.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    24014 2023-05-16 19:06:45.000000 west-1.1.0a1/src/west/configuration.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     6501 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/log.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     4797 2023-06-01 23:49:07.000000 west-1.1.0a1/src/west/manifest-schema.yml
+-rw-r--r--   0 mbolivar   (501) staff       (20)   108818 2023-06-02 19:40:31.000000 west-1.1.0a1/src/west/manifest.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)        0 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/py.typed
+-rw-r--r--   0 mbolivar   (501) staff       (20)     2926 2022-04-04 18:01:00.000000 west-1.1.0a1/src/west/util.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)      617 2023-06-02 19:50:05.000000 west-1.1.0a1/src/west/version.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     1001 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/west-commands-schema.yml
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.281465 west-1.1.0a1/src/west.egg-info/
+-rw-r--r--   0 mbolivar   (501) staff       (20)     4511 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/PKG-INFO
+-rw-r--r--   0 mbolivar   (501) staff       (20)      728 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/SOURCES.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)        1 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/dependency_links.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)       44 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/entry_points.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)        1 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/not-zip-safe
+-rw-r--r--   0 mbolivar   (501) staff       (20)       52 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/requires.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)        5 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/top_level.txt
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.284229 west-1.1.0a1/tests/
+-rw-r--r--   0 mbolivar   (501) staff       (20)      566 2023-05-01 21:45:22.000000 west-1.1.0a1/tests/test_commands.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    19522 2023-05-16 19:06:45.000000 west-1.1.0a1/tests/test_config.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     1658 2022-04-04 18:01:00.000000 west-1.1.0a1/tests/test_help.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)      795 2021-03-11 03:46:31.000000 west-1.1.0a1/tests/test_main.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)   101805 2023-06-02 19:40:31.000000 west-1.1.0a1/tests/test_manifest.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    86895 2023-05-16 19:06:45.000000 west-1.1.0a1/tests/test_project.py
```

### Comparing `west-1.0.0a1/LICENSE` & `west-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/PKG-INFO` & `west-1.1.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: west
-Version: 1.0.0a1
+Version: 1.1.0a1
 Summary: Zephyr RTOS Project meta-tool
 Home-page: https://github.com/zephyrproject-rtos/west
 Author: Zephyr Project
 Author-email: devel@lists.zephyrproject.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -34,19 +34,20 @@
 single file, called the *west manifest file*, or *manifest* for short.
 By default the manifest file is named ``west.yml``.
 You use ``west init`` to set up this directory, then ``west update`` to fetch
 and/or update the repositories named in the manifest.
 
 By default, west uses `upstream Zephyr's manifest file
 <https://github.com/zephyrproject-rtos/zephyr/blob/main/west.yml>`_, but west
-doesn't care if the manifest repository is a Zephyr tree or not.
+doesn't care if the manifest repository is zephyr or not. You can and are
+encouraged to make your own manifest repositories to meet your needs.
 
-For more details, see `Multiple Repository Management
-<https://docs.zephyrproject.org/latest/guides/west/repo-tool.html>`_ in the
-west documentation.
+For more details, see the `West guide
+<https://docs.zephyrproject.org/latest/guides/west/index.html>`_ in the Zephyr
+documentation.
 
 Example usage using the upstream manifest file::
 
   mkdir zephyrproject && cd zephyrproject
   west init
   west update
 
@@ -94,19 +95,33 @@
   tox
 
 See the tox configuration file, tox.ini, for more details.
 
 Hacking on West
 ---------------
 
+This section contains notes for getting started developing west itself.
+
+Editable Install
+~~~~~~~~~~~~~~~~
+
+To run west "live" from the current source code tree, run this command from the
+top level directory in the west repository::
+
+  pip3 install -e .
+
+This is useful if you are actively working on west and don't want to re-package
+and install a wheel each time you run it.
+
 Installing from Source
 ~~~~~~~~~~~~~~~~~~~~~~
 
-The `wheel`_ package is required to install west from source. See "Installing
-Wheel" below if you don't have ``wheel`` installed.
+You can create and install a wheel package to install west as well.
+The `wheel`_ Python package is required to do this. See "Installing Wheel"
+below if you need to do this.
 
 To build the west wheel file::
 
   # macOS, Linux
   python3 setup.py bdist_wheel
 
   # Windows
@@ -118,25 +133,14 @@
 To install the wheel::
 
   pip3 install -U dist/west-x.y.z-py3-none-any.whl
 
 You can ``pip3 uninstall west`` to remove this wheel before re-installing the
 version from PyPI, etc.
 
-Editable Install
-~~~~~~~~~~~~~~~~
-
-To run west "live" from the current source code tree, run this command from the
-top level directory in the west repository::
-
-  pip3 install -e .
-
-This is useful if you are actively working on west and don't want to re-package
-and install a wheel each time you run it.
-
 Installing Wheel
 ~~~~~~~~~~~~~~~~
 
 On macOS and Windows, you can install wheel with::
 
   pip3 install wheel
```

### Comparing `west-1.0.0a1/README.rst` & `west-1.1.0a1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 single file, called the *west manifest file*, or *manifest* for short.
 By default the manifest file is named ``west.yml``.
 You use ``west init`` to set up this directory, then ``west update`` to fetch
 and/or update the repositories named in the manifest.
 
 By default, west uses `upstream Zephyr's manifest file
 <https://github.com/zephyrproject-rtos/zephyr/blob/main/west.yml>`_, but west
-doesn't care if the manifest repository is a Zephyr tree or not.
+doesn't care if the manifest repository is zephyr or not. You can and are
+encouraged to make your own manifest repositories to meet your needs.
 
-For more details, see `Multiple Repository Management
-<https://docs.zephyrproject.org/latest/guides/west/repo-tool.html>`_ in the
-west documentation.
+For more details, see the `West guide
+<https://docs.zephyrproject.org/latest/guides/west/index.html>`_ in the Zephyr
+documentation.
 
 Example usage using the upstream manifest file::
 
   mkdir zephyrproject && cd zephyrproject
   west init
   west update
 
@@ -78,19 +79,33 @@
   tox
 
 See the tox configuration file, tox.ini, for more details.
 
 Hacking on West
 ---------------
 
+This section contains notes for getting started developing west itself.
+
+Editable Install
+~~~~~~~~~~~~~~~~
+
+To run west "live" from the current source code tree, run this command from the
+top level directory in the west repository::
+
+  pip3 install -e .
+
+This is useful if you are actively working on west and don't want to re-package
+and install a wheel each time you run it.
+
 Installing from Source
 ~~~~~~~~~~~~~~~~~~~~~~
 
-The `wheel`_ package is required to install west from source. See "Installing
-Wheel" below if you don't have ``wheel`` installed.
+You can create and install a wheel package to install west as well.
+The `wheel`_ Python package is required to do this. See "Installing Wheel"
+below if you need to do this.
 
 To build the west wheel file::
 
   # macOS, Linux
   python3 setup.py bdist_wheel
 
   # Windows
@@ -102,25 +117,14 @@
 To install the wheel::
 
   pip3 install -U dist/west-x.y.z-py3-none-any.whl
 
 You can ``pip3 uninstall west`` to remove this wheel before re-installing the
 version from PyPI, etc.
 
-Editable Install
-~~~~~~~~~~~~~~~~
-
-To run west "live" from the current source code tree, run this command from the
-top level directory in the west repository::
-
-  pip3 install -e .
-
-This is useful if you are actively working on west and don't want to re-package
-and install a wheel each time you run it.
-
 Installing Wheel
 ~~~~~~~~~~~~~~~~
 
 On macOS and Windows, you can install wheel with::
 
   pip3 install wheel
```

### Comparing `west-1.0.0a1/setup.py` & `west-1.1.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/src/west/app/config.py` & `west-1.1.0a1/src/west/app/config.py`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/src/west/app/main.py` & `west-1.1.0a1/src/west/app/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,34 +14,153 @@
 import argparse
 from collections import OrderedDict
 import colorama
 from io import StringIO
 import logging
 import os
 from pathlib import Path, PurePath
+import platform
 import shutil
+import signal
 import sys
 from subprocess import CalledProcessError
 import tempfile
 import textwrap
 import traceback
+from typing import NamedTuple, Optional
+from typing import List as ListType
 
 from west import log
 import west.configuration
 from west.commands import WestCommand, extension_commands, \
     CommandError, ExtensionCommandError, Verbosity
-from west.app.project import List, ManifestCommand, Diff, Status, \
+from west.app.project import List, ManifestCommand, Compare, Diff, Status, \
     SelfUpdate, ForAll, Init, Update, Topdir
 from west.app.config import Config
 from west.manifest import Manifest, MalformedConfig, MalformedManifest, \
     ManifestVersionError, ManifestImportFailed, _ManifestImportDepth, \
     ManifestProject, MANIFEST_REV_BRANCH
 from west.util import quote_sh_list, west_topdir, WestNotFound
 from west.version import __version__
 
+class EarlyArgs(NamedTuple):
+    # Data type for storing "early" argument parsing results.
+    #
+    # We do some manual parsing of the command-line arguments before
+    # delegating the hard parts to argparse. This extra work figures
+    # out the command name, verbosity level, etc.
+    #
+    # This is necessary for:
+    #
+    # - nicer error-handling in situations where the command is an
+    #   extension but we're not in a workspace
+    #
+    # - setting up log levels from the verbosity level
+
+    # Expected arguments:
+    help: bool                  # True if -h was given
+    version: bool               # True if -V was given
+    zephyr_base: Optional[str]  # -z argument value
+    verbosity: int              # 0 if not given, otherwise counts
+    command_name: Optional[str]
+
+    # Other arguments are appended here.
+    unexpected_arguments: ListType[str]
+
+def parse_early_args(argv: ListType[str]) -> EarlyArgs:
+    # Hand-rolled argument parser for early arguments.
+
+    help = False
+    version = False
+    zephyr_base = None
+    verbosity = 0
+    command_name = None
+    unexpected_arguments = []
+
+    expecting_zephyr_base = False
+
+    def consume_more_args(rest):
+        # Handle the 'Vv' portion of 'west -hVv'.
+
+        nonlocal help, version, zephyr_base, verbosity, command_name
+        nonlocal unexpected_arguments
+        nonlocal expecting_zephyr_base
+
+        if not rest:
+            return
+
+        if rest.startswith('h'):
+            help = True
+            consume_more_args(rest[1:])
+        elif rest.startswith('V'):
+            version = True
+            consume_more_args(rest[1:])
+        elif rest.startswith('v'):
+            verbosity += 1
+            consume_more_args(rest[1:])
+        elif rest.startswith('z'):
+            if not rest[1:]:
+                expecting_zephyr_base = True
+            elif rest[1] == '=':
+                zephyr_base = rest[2:]
+            else:
+                zephyr_base = rest[1:]
+        else:
+            unexpected_arguments.append(rest)
+
+    for arg in argv:
+        if expecting_zephyr_base:
+            zephyr_base = arg
+        elif arg.startswith('-h'):
+            help = True
+            consume_more_args(arg[2:])
+        elif arg.startswith('-V'):
+            version = True
+            consume_more_args(arg[2:])
+        elif arg == '--version':
+            version = True
+        elif arg.startswith('-v'):
+            verbosity += 1
+            consume_more_args(arg[2:])
+        elif arg == '--verbose':
+            verbosity += 1
+        elif arg.startswith('-z'):
+            if arg == '-z':
+                expecting_zephyr_base = True
+            elif arg.startswith('-z='):
+                zephyr_base = arg[3:]
+            else:
+                zephyr_base = arg[2:]
+        elif arg.startswith('-'):
+            unexpected_arguments.append(arg)
+        else:
+            command_name = arg
+            break
+
+    return EarlyArgs(help, version, zephyr_base, verbosity,
+                     command_name, unexpected_arguments)
+
+class LogFormatter(logging.Formatter):
+
+    def __init__(self):
+        super().__init__(fmt='%(name)s: %(levelname)s: %(message)s')
+
+class LogHandler(logging.Handler):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.setFormatter(LogFormatter())
+
+    def emit(self, record):
+        formatted = self.format(record)
+        if record.levelno >= logging.WARNING:
+            print(formatted, file=sys.stderr)
+        else:
+            print(formatted)
+
 class WestApp:
     # The west 'application' object.
     #
     # There's enough state to keep track of when building the final
     # WestCommand we want to run that it's convenient to have an
     # object to stash it all in.
     #
@@ -79,14 +198,28 @@
         #   to access from the Help object's parser attribute,
         #   which comes from subparser_gen.
         self.builtins['help'].app = self
 
     def run(self, argv):
         # Run the command-line application with argument list 'argv'.
 
+        early_args = parse_early_args(argv)
+
+        # Silence validation errors from pykwalify, which are logged at
+        # logging.ERROR level. We want to handle those ourselves as
+        # needed.
+        logging.getLogger('pykwalify').setLevel(logging.CRITICAL)
+
+        # Use verbosity to determine west API log levels
+        self.setup_west_logging(early_args.verbosity)
+
+        # Makes ANSI color escapes work on Windows, and strips them when
+        # stdout/stderr isn't a terminal
+        colorama.init()
+
         # See if we're in a workspace. It's fine if we're not.
         # Note that this falls back on searching from ZEPHYR_BASE
         # if the current directory isn't inside a west workspace.
         try:
             self.topdir = west_topdir()
         except WestNotFound:
             pass
@@ -104,15 +237,15 @@
         self.load_extension_specs()
 
         # Set up initial argument parsers. This requires knowing
         # self.extensions, so it can't happen before now.
         self.setup_parsers()
 
         # OK, we are all set. Run the command.
-        self.run_command(argv)
+        self.run_command(argv, early_args)
 
     def load_manifest(self):
         # Try to parse the manifest. We'll save it if that works, so
         # it doesn't have to be re-parsed.
 
         if not self.topdir:
             return
@@ -181,57 +314,41 @@
         def isinst(*args):
             return any(isinstance(self.mle, t) for t in args)
 
         if args.command not in no_manifest_ok:
             if isinst(MalformedManifest, MalformedConfig):
                 self.queued_io.append(
                     lambda cmd:
-                    cmd.die('\n  '.join(["can't load west manifest"] +
-                                        list(self.mle.args))))
+                    cmd.die("can't load west manifest: " +
+                            "\n".join(list(self.mle.args))))
             elif isinst(_ManifestImportDepth):
                 self.queued_io.append(
                     lambda cmd:
                     cmd.die(
                         'recursion depth exceeded during manifest resolution; '
                         'your manifest likely contains an import loop. '
                         'Run "west -v manifest --resolve" to debug.'))
             elif isinst(ManifestImportFailed):
                 if args.command == 'update':
                     return      # that's fine
 
-                p, imp = self.mle.project, self.mle.imp
-                ctxt = f'  Failed importing "{imp}"'
-                if not isinstance(p, ManifestProject):
-                    # Try to be more helpful by explaining exactly
-                    # what west.manifest needs to happen before we can
-                    # resolve the missing import.
-                    rev = p.revision
-
-                    ctxt += f' from revision "{rev}"\n'
-                    ctxt += '  Hint: for this to work:\n'
-                    ctxt += f'          - {p.name} must be cloned\n'
-                    ctxt += (f'          - its {MANIFEST_REV_BRANCH} ref '
-                             'must point to a commit with the import data\n')
-                    ctxt += '        To fix, run:\n'
-                    ctxt += '          west update'
-
-                self.queued_io.append(
-                    lambda cmd:
-                    cmd.die(f'failed manifest import in {p.name_and_path}\n' +
-                            ctxt))
+                self.queued_io.append(lambda cmd: cmd.die(mie_msg(self.mle)))
             elif isinst(FileNotFoundError):
                 # This should ordinarily only happen when the top
                 # level manifest is not found.
                 self.queued_io.append(
                     lambda cmd:
-                    cmd.die(f"file not found: {self.mle.filename}"))
+                    cmd.die(f"manifest file not found: {self.mle.filename}\n"
+                            "Please check manifest.file and manifest.path in "
+                            f"{self.topdir + '/' or ''}.west/config"))
             elif isinst(PermissionError):
                 self.queued_io.append(
                     lambda cmd:
-                    cmd.die(f"permission denied: {self.mle.filename}"))
+                    cmd.die("permission denied when loading manifest file: "
+                            f"{self.mle.filename}"))
             else:
                 self.queued_io.append(
                     lambda cmd:
                     cmd.die('internal error:',
                             f'unhandled manifest load exception: {self.mle}'))
 
     def load_extension_specs(self):
@@ -329,14 +446,16 @@
             prog='west', description='The Zephyr RTOS meta-tool.',
             epilog='''Run "west help <command>" for help on each <command>.''',
             add_help=False, west_app=self, allow_abbrev=False)
 
         # Remember to update zephyr's west-completion.bash if you add or
         # remove flags. This is currently the only place where shell
         # completion is available.
+        #
+        # If you update these, also update parse_early_args().
 
         parser.add_argument('-h', '--help', action=WestHelpAction, nargs=0,
                             help='get help for west or a command')
 
         parser.add_argument('-z', '--zephyr-base', default=None,
                             help='''Override the Zephyr base directory. The
                             default is the manifest project with path
@@ -351,19 +470,20 @@
                             help='print the program version and exit')
 
         subparser_gen = parser.add_subparsers(metavar='<command>',
                                               dest='command')
 
         return parser, subparser_gen
 
-    def run_command(self, argv):
+    def run_command(self, argv, early_args):
         # Parse command line arguments and run the WestCommand.
         # If we're running an extension, instantiate it from its
         # spec and re-parse arguments before running.
 
+        self.handle_early_arg_errors(early_args)
         args, unknown = self.west_parser.parse_known_args(args=argv)
 
         # Set up logging verbosity before running the command, for
         # backwards compatibility. Remove this when we can part ways
         # with the log module.
         log.set_verbosity(args.verbose)
 
@@ -380,15 +500,46 @@
             # Both run_builtin() and run_extension() set self.cmd so
             # we can use it in the exception handling blocks below.
             if args.command in self.builtins:
                 self.run_builtin(args, unknown)
             else:
                 self.run_extension(args.command, argv)
         except KeyboardInterrupt:
-            sys.exit(0)
+            # Catching this avoids dumping stack.
+            #
+            # Here we replicate CPython's behavior in exit_sigint() in
+            # Modules/main.c (as of
+            # 2f62a5da949cd368a9498e6a03e700f4629fa97f), but in pure
+            # Python since it's not clear how or if we can call that
+            # directly from here.
+            #
+            # For more discussion on this behavior, see:
+            #
+            # https://bugs.python.org/issue1054041
+            if platform.system() == 'Windows':
+                # The hex number is a standard value (STATUS_CONTROL_C_EXIT):
+                # https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-erref/596a1078-e883-4972-9bbc-49e60bebca55
+                #
+                # Subtracting 2**32 seems to be the convention for
+                # making it fit in an int32_t.
+                CONTROL_C_EXIT_CODE = 0xC000013A - 2**32
+                sys.exit(CONTROL_C_EXIT_CODE)
+            else:
+                # On Unix, just reinstate the default SIGINT handler
+                # and send the signal again, overriding the CPython
+                # KeyboardInterrupt stack dump.
+                #
+                # In addition to exiting with the correct "dying due
+                # to SIGINT" status code (usually 130), this signals
+                # to the calling environment that we were interrupted,
+                # so that e.g. "while true; do west ... ; done" will
+                # exit out of the entire while loop and not just
+                # the west command.
+                signal.signal(signal.SIGINT, signal.SIG_DFL)
+                os.kill(os.getpid(), signal.SIGINT)
         except BrokenPipeError:
             sys.exit(0)
         except CalledProcessError as cpe:
             self.cmd.err(f'command exited with status {cpe.returncode}: '
                          f'{quote_sh_list(cpe.cmd)}', fatal=True)
             if self.cmd.verbosity >= Verbosity.DBG_EXTREME:
                 self.cmd.banner('Traceback (enabled by -vvv):')
@@ -406,14 +557,50 @@
             # try to fix a previous update that left 'manifest-rev'
             # branches pointing at revisions with invalid manifest
             # data in projects that get imported.
             self.cmd.die('\n  '.join(str(arg) for arg in mm.args))
         except WestNotFound as wnf:
             self.cmd.die(str(wnf))
 
+    def handle_early_arg_errors(self, early_args):
+        # If early_args indicates we should error out, handle it
+        # gracefully. This provides more user-friendly output than
+        # argparse can do on its own.
+
+        if (early_args.command_name and
+            (early_args.command_name not in self.builtins and
+             (not self.extensions or
+              early_args.command_name not in self.extensions))):
+            self.handle_unknown_command(early_args.command_name)
+
+    def handle_unknown_command(self, command_name):
+        if self.topdir:
+            extra_help = (f'workspace {self.topdir} does not define '
+                          'this extension command -- try "west help"')
+        else:
+            extra_help = 'do you need to run this inside a workspace?'
+        self.print_usage_and_exit(f'west: unknown command "{command_name}"; '
+                                  f'{extra_help}')
+
+    def print_usage_and_exit(self, message):
+        self.west_parser.print_usage(file=sys.stderr)
+        sys.exit(message)
+
+    def setup_west_logging(self, verbosity):
+        logger = logging.getLogger('west.manifest')
+
+        if verbosity >= 2:
+            logger.setLevel(logging.DEBUG)
+        elif verbosity == 1:
+            logger.setLevel(logging.INFO)
+        else:
+            logger.setLevel(logging.WARNING)
+
+        logger.addHandler(LogHandler())
+
     def run_builtin(self, args, unknown):
         self.queued_io.append(
             lambda cmd: cmd.dbg('args namespace:', args,
                                 level=Verbosity.DBG_EXTREME))
         self.cmd = self.builtins.get(args.command,
                                      self.builtins['help'])
         adjust_command_verbosity(self.cmd, args)
@@ -820,64 +1007,97 @@
         optional['help'] = kwargs.get('help')
         self.west_optionals.append(optional)
 
         # Let argparse handle the actual argument.
         super().add_argument(*args, **kwargs)
 
     def error(self, message):
-        if (self.west_app and
-                self.west_app.mle and
-                isinstance(self.west_app.mle,
-                           ManifestVersionError) and
-                self.west_app.cmd):
-            self.west_app.cmd.die(mve_msg(self.west_app.mle))
+        if self.west_app and self.west_app.mle:
+            # If we have a known WestApp instance and the manifest
+            # failed to load, then try to specialize the generic error
+            # message we're getting from argparse to handle west-specific
+            # errors better.
+
+            app = self.west_app
+            mle = self.west_app.mle
+            if app.cmd:
+                cmd = app.cmd
+            else:
+                # No app.cmd probably means that the user is
+                # running an extension command that they expected
+                # to work, but we don't know about because the
+                # import failed and thus we have no manifest to
+                # load extensions from.
+                #
+                # Just use the help command as a stand-in instead.
+                # We have to manually patch up its config
+                # attribute in order to do this outside of
+                # do_run().
+                cmd = app.builtins['help']
+                cmd.config = west.configuration.Configuration(
+                    topdir=app.topdir)
+            if isinstance(mle, ManifestVersionError):
+                cmd.die(mve_msg(mle))
+            elif isinstance(mle, ManifestImportFailed):
+                cmd.die(mie_msg(mle))
         super().error(message=message)
 
 def mve_msg(mve, suggest_upgrade=True):
+    # Helper for getting a message for a ManifestVersionError.
     return '\n  '.join(
         [f'west v{mve.version} or later is required by the manifest',
          f'West version: v{__version__}'] +
         ([f'Manifest file: {mve.file}'] if mve.file else []) +
         (['Please upgrade west and retry.'] if suggest_upgrade else []))
 
+def mie_msg(mie):
+    # Helper for getting a message for a ManifestImportError.
+
+    p, imp = mie.project, mie.imp
+    ret = (f'failed manifest import in {p.name_and_path}:\n'
+           f'  Failed importing "{imp}"')
+    if not isinstance(p, ManifestProject):
+        # Try to be more helpful by explaining exactly
+        # what west.manifest needs to happen before we can
+        # resolve the missing import.
+        ret += (f' from revision "{p.revision}"\n'
+                f'  Hint: {p.name} must be cloned and its '
+                f'{MANIFEST_REV_BRANCH} ref must point to a '
+                'commit with the import data\n'
+                '  To fix, run "west update"')
+
+    return ret
+
 def adjust_command_verbosity(command, args):
     command.verbosity = min(command.verbosity + args.verbose,
                             Verbosity.DBG_EXTREME)
 
 def dump_traceback():
     # Save the current exception to a file and return its path.
     fd, name = tempfile.mkstemp(prefix='west-exc-', suffix='.txt')
     os.close(fd)        # traceback has no use for the fd
     with open(name, 'w') as f:
         traceback.print_exc(file=f)
     return name
 
 def main(argv=None):
-    # Silence validation errors from pykwalify, which are logged at
-    # logging.ERROR level. We want to handle those ourselves as
-    # needed.
-    logging.getLogger('pykwalify').setLevel(logging.CRITICAL)
-
-    # Makes ANSI color escapes work on Windows, and strips them when
-    # stdout/stderr isn't a terminal
-    colorama.init()
-
     # Create the WestApp instance and let it run.
     app = WestApp()
     app.run(argv or sys.argv[1:])
 
 # If you add a command here, make sure to think about how it should be
 # handled in case of ManifestVersionError or other reason the manifest
 # might fail to load (import error, configuration file error, etc.)
 BUILTIN_COMMAND_GROUPS = {
     'built-in commands for managing git repositories': [
         Init,
         Update,
         List,
         ManifestCommand,
+        Compare,
         Diff,
         Status,
         ForAll,
     ],
 
     'other built-in commands': [
         Help,
```

### Comparing `west-1.0.0a1/src/west/app/project.py` & `west-1.1.0a1/src/west/app/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 from time import perf_counter
 from urllib.parse import urlparse
 
 from west.configuration import Configuration
 from west import util
 from west.commands import WestCommand, CommandError, Verbosity
 from west.manifest import ImportFlag, Manifest, \
-    ManifestProject, _manifest_content_at, ManifestImportFailed, \
-    _ManifestImportDepth, ManifestVersionError, MalformedManifest
+    ManifestProject, _manifest_content_at, ManifestImportFailed
 from west.manifest import is_group as is_project_group
 from west.manifest import MANIFEST_REV_BRANCH as MANIFEST_REV
 from west.manifest import QUAL_MANIFEST_REV_BRANCH as QUAL_MANIFEST_REV
 from west.manifest import QUAL_REFS_WEST as QUAL_REFS
 
 #
 # Project-related or multi-repo commands, like "init", "update",
@@ -94,33 +93,52 @@
             s = 's:' if len(failed) > 1 else ''
             projects = ', '.join(f'{p.name}' for p in failed)
             self.err(f'{self.name} failed for project{s} {projects}')
         else:
             self.err(f'{self.name} failed for multiple projects; see above')
         raise CommandError(1)
 
-    def _setup_logging(self, args):
-        logger = logging.getLogger('west.manifest')
-
-        if self.verbosity >= Verbosity.INF:
-            level = logging.DEBUG
-        else:
-            level = logging.INFO
-
-        logger.setLevel(level)
-        logger.addHandler(ProjectCommandLogHandler(self))
-
     def _die_unknown(self, unknown):
         # Scream and die about unknown projects.
 
         s = 's' if len(unknown) > 1 else ''
         names = ' '.join(unknown)
         self.die(f'unknown project name{s}/path{s}: {names}\n'
                  '  Hint: use "west list" to list all projects.')
 
+    def _has_nonempty_status(self, project):
+        # Check if the project has any status output to print. We
+        # manually use Popen in order to try to exit as quickly as
+        # possible if 'git status' prints anything.
+
+        popen = subprocess.Popen(['git', 'status', '--porcelain'],
+                                 stdout=subprocess.PIPE,
+                                 stderr=subprocess.PIPE,
+                                 cwd=project.abspath)
+
+        def has_output():
+            # 'git status --porcelain' prints nothing if there
+            # are no notable changes, so any output at all
+            # means we should run 'git status' on the project.
+            stdout, stderr = None, None
+            try:
+                stdout, stderr = popen.communicate(timeout=0.1)
+            except subprocess.TimeoutExpired:
+                pass
+            return stdout or stderr
+
+        while True:
+            if has_output():
+                popen.kill()
+                return True
+            if popen.poll() is not None:
+                break
+
+        return has_output()
+
 class Init(_ProjectCommand):
 
     def __init__(self):
         super().__init__(
             'init',
             'create a west workspace',
             f'''\
@@ -196,16 +214,14 @@
             self.die_already(self.topdir, msg)
 
         if args.local and (args.manifest_url or args.manifest_rev):
             self.die('-l cannot be combined with -m or --mr')
 
         self.die_if_no_git()
 
-        self._setup_logging(args)
-
         if args.local:
             topdir = self.local(args)
         else:
             topdir = self.bootstrap(args)
 
         self.banner(f'Initialized. Now run "west update" inside {topdir}.')
 
@@ -408,16 +424,14 @@
             self.die_if_no_git()
 
             return "cloned" if project.is_cloned() else "not-cloned"
 
         def delay(func, project):
             return DelayFormat(partial(func, project))
 
-        self._setup_logging(args)
-
         for project in self._projects(args.projects):
             # Skip inactive projects unless the user said
             # --all or named some projects explicitly.
             if not (args.all or args.projects or
                     self.manifest.is_active(project)):
                 self.dbg(f'{project.name}: skipping inactive project')
                 continue
@@ -527,55 +541,213 @@
         group = parser.add_argument_group('options for --resolve and --freeze')
         group.add_argument('-o', '--out',
                            help='output file, default is standard output')
 
         return parser
 
     def do_run(self, args, user_args):
-        self._setup_logging(args)
-
-        # Since the user is explicitly managing the manifest, we are
-        # deliberately loading it again instead of using self.manifest
-        # to emit debug logs if enabled, which are turned off when the
-        # manifest is initially parsed in main.py.
-        #
-        # The code in main.py is usually responsible for handling any
-        # errors and printing useful messages. We re-do error checking
-        # for manifest-related errors that it won't handle.
-        try:
-            manifest = Manifest.from_topdir(topdir=self.topdir)
-        except _ManifestImportDepth:
-            self.die("cannot resolve manifest -- is there a loop?")
-        except ManifestImportFailed as mif:
-            self.die(f"manifest import failed\n  Project: {mif.project}\n  "
-                     f"File: {mif.filename}")
-        except (MalformedManifest, ManifestVersionError) as e:
-            self.die('\n  '.join(str(arg) for arg in e.args))
+        manifest = self.manifest
         dump_kwargs = {'default_flow_style': False,
                        'sort_keys': False}
 
         if args.validate:
             pass              # nothing more to do
         elif args.resolve:
+            self._die_if_manifest_project_filter('resolve')
             self._dump(args, manifest.as_yaml(**dump_kwargs))
         elif args.freeze:
+            self._die_if_manifest_project_filter('freeze')
             self._dump(args, manifest.as_frozen_yaml(**dump_kwargs))
         elif args.path:
             self.inf(manifest.path)
         else:
             # Can't happen.
             raise RuntimeError(f'internal error: unhandled args {args}')
 
+    def _die_if_manifest_project_filter(self, action):
+        if self.config.get('manifest.project-filter') is not None:
+            self.die(f'"west manifest --{action}" is not (yet) supported '
+                     'when the manifest.project-filter option is set. '
+                     'Please clear the project-filter configuration '
+                     'option and re-run this command, or contact the '
+                     'west developers if you have a use case for resolving '
+                     'the manifest while projects are made inactive by the '
+                     'project filter.')
+
     def _dump(self, args, to_dump):
         if args.out:
             with open(args.out, 'w') as f:
                 f.write(to_dump)
         else:
             sys.stdout.write(to_dump)
 
+class Compare(_ProjectCommand):
+    def __init__(self):
+        super().__init__(
+            'compare',
+            "compare project status against the manifest",
+            textwrap.dedent('''\
+            Compare each project's working tree state against the results
+            of the most recent successful "west update" command.
+
+            This command prints output for a project if (and only if)
+            at least one of the following is true:
+
+            1. its checked out commit (HEAD) is different than the commit
+               checked out by the most recent successful "west update"
+               (which the manifest-rev branch will point to)
+            2. its working tree is not clean (i.e. there are local uncommitted
+               changes)
+            3. it has a local checked out branch (unless the configuration
+               option compare.ignore-branches is true or --ignore-branches
+               is given on the command line, either of which disable this)
+
+            The command also prints output for the manifest repository if it
+            has nonempty status.
+
+            The output is meant to be human-readable, and may change. It is
+            not a stable interface to write scripts against. This command
+            requires git 2.22 or later.''')
+        )
+
+    def do_add_parser(self, parser_adder):
+        parser = self._parser(parser_adder,
+                              epilog=ACTIVE_CLONED_PROJECTS_HELP)
+        parser.add_argument('projects', metavar='PROJECT', nargs='*',
+                            help='''projects (by name or path) to operate on;
+                            defaults to active cloned projects''')
+        parser.add_argument('-a', '--all', action='store_true',
+                            help='include output for inactive projects')
+        parser.add_argument('--exit-code', action='store_true',
+                            help='''exit with status code 1 if status output
+                            was printed for any project''')
+        parser.add_argument('--ignore-branches',
+                            default=None, action='store_true',
+                            help='''skip output for projects with checked out
+                            branches and clean working trees if the branch is
+                            at the same commit as the last "west update"''')
+        parser.add_argument('--no-ignore-branches', dest='ignore_branches',
+                            action='store_false',
+                            help='''overrides a previous --ignore-branches
+                            or any compare.ignore-branches configuration
+                            option''')
+        return parser
+
+    def do_run(self, args, ignored):
+        self.die_if_no_git()
+        if self.git_version_info < (2, 22):
+            # This is for git branch --show-current.
+            self.die('git version 2.22 or later is required')
+
+        if args.ignore_branches is not None:
+            self.ignore_branches = args.ignore_branches
+        else:
+            self.ignore_branches = \
+                self.config.getboolean('compare.ignore-branches', False)
+
+        failed = []
+        printed_output = False
+        for project in self._cloned_projects(args, only_active=not args.all):
+            if isinstance(project, ManifestProject):
+                # West doesn't track the relationship between the manifest
+                # repository and any remote, but users are still interested
+                # in printing output for comparisons that makes sense.
+                if self._has_nonempty_status(project):
+                    try:
+                        self.compare(project)
+                        printed_output = True
+                    except subprocess.CalledProcessError:
+                        failed.append(project)
+                continue
+
+            # 'git status' output for all projects is noisy when there
+            # are lots of projects.
+            #
+            # We avoid this problem in 2 steps:
+            #
+            #   1. Check if we need to print any output for the
+            #      project.
+            #
+            #   2. If so, run 'git status' on the project. Otherwise,
+            #      skip output for the project entirely.
+            #
+            # In verbose mode, we always print output.
+
+            def has_checked_out_branch(project):
+                if self.ignore_branches:
+                    return False
+
+                return bool(project.git('branch --show-current',
+                                        capture_stdout=True,
+                                        capture_stderr=True).stdout.strip())
+
+            try:
+                if not (self.verbosity >= Verbosity.DBG or
+                        has_checked_out_branch(project) or
+                        (project.sha(QUAL_MANIFEST_REV) !=
+                         project.sha('HEAD')) or
+                        self._has_nonempty_status(project)):
+                    continue
+
+                self.compare(project)
+                printed_output = True
+            except subprocess.CalledProcessError:
+                failed.append(project)
+        self._handle_failed(args, failed)
+
+        if args.exit_code and printed_output:
+            raise CommandError(1)
+
+    def compare(self, project):
+        self.banner(f'{project.name_and_path}:')
+        self.print_rev_info(project)
+        self.print_status(project)
+
+    def print_rev_info(self, project):
+        # For non-manifest repositories, print HEAD's and
+        # manifest-rev's SHAs and commit titles, but only if they are
+        # different.
+        #
+        # We force git not to print in color so west's colored
+        # banner() separators stand out more in the output.
+        if isinstance(project, ManifestProject):
+            return
+
+        def rev_info(rev):
+            title = project.git(
+                ['log', '-1', '--color=never', '--pretty=%h%d %s',
+                 '--decorate-refs-exclude=refs/heads/manifest-rev',
+                 rev],
+                capture_stdout=True,
+                capture_stderr=True).stdout.decode().rstrip()
+            # "HEAD" is special; '--decorate-refs-exclude=HEAD' doesn't work.
+            # Fortunately it's always first.
+            return (
+                title.replace('(HEAD) ', '').replace('(HEAD, ', '(')
+                .replace('(HEAD -> ', '(')
+            )
+
+        head_info = rev_info('HEAD')
+        # If manifest-rev is missing, we already failed earlier.
+        manifest_rev_info = rev_info('manifest-rev')
+        if head_info != manifest_rev_info:
+            self.small_banner(f'manifest-rev: {manifest_rev_info}')
+            self.inf(f'            HEAD: {head_info}')
+
+    def print_status(self, project):
+        # `git status` shows `manifest-rev` "sometimes", see #643.
+        if self.color_ui:
+            color = '-c status.color=always'
+        else:
+            color = ''
+        cp = project.git(f'{color} status', capture_stdout=True,
+                         capture_stderr=True)
+        self.small_banner('status:')
+        self.inf(textwrap.indent(cp.stdout.decode().rstrip(), ' ' * 4))
+
 class Diff(_ProjectCommand):
     def __init__(self):
         super().__init__(
             'diff',
             '"git diff" for one or more projects',
             'Runs "git diff" on each of the specified projects.')
 
@@ -587,15 +759,14 @@
                             defaults to active cloned projects''')
         parser.add_argument('-a', '--all', action='store_true',
                             help='include output for inactive projects')
         return parser
 
     def do_run(self, args, ignored):
         self.die_if_no_git()
-        self._setup_logging(args)
 
         failed = []
         no_diff = 0
         # We may need to force git to use colors if the user wants them,
         # which it won't do ordinarily since stdout is not a terminal.
         color = ['--color=always'] if self.color_ui else []
         for project in self._cloned_projects(args, only_active=not args.all):
@@ -633,15 +804,14 @@
                             defaults to active cloned projects''')
         parser.add_argument('-a', '--all', action='store_true',
                             help='include output for inactive projects')
         return parser
 
     def do_run(self, args, user_args):
         self.die_if_no_git()
-        self._setup_logging(args)
 
         failed = []
         for project in self._cloned_projects(args, only_active=not args.all):
             # 'git status' output for all projects is noisy when there
             # are lots of projects.
             #
             # We avoid this problem in 2 steps:
@@ -652,71 +822,23 @@
             #   2. If so, run 'git status' on the project. Otherwise,
             #      skip output for the project entirely.
             #
             # In verbose mode, we always print output.
 
             try:
                 if not (self.verbosity >= Verbosity.DBG or
-                        self.should_print_for(project)):
+                        self._has_nonempty_status(project)):
                     continue
 
                 self.banner(f'status of {project.name_and_path}:')
                 project.git('status', extra_args=user_args)
             except subprocess.CalledProcessError:
                 failed.append(project)
         self._handle_failed(args, failed)
 
-    def should_print_for(self, project):
-        # do_run() helper; check if the project has any status output
-        # to print. We manually use Popen in order to try to exit as
-        # quickly as possible if 'git status' prints anything.
-
-        # This technique fails when tested on Python 3.6, which west
-        # still supports at time of writing. This seems likely to be
-        # due to https://bugs.python.org/issue35182.
-        #
-        # Users of old python versions will have to deal with the
-        # verbose output.
-        if sys.version_info < (3, 7):
-            return True
-
-        popen = subprocess.Popen(['git', 'status', '--porcelain'],
-                                 stdout=subprocess.PIPE,
-                                 stderr=subprocess.PIPE,
-                                 cwd=project.abspath)
-
-        def has_output():
-            # 'git status --porcelain' prints nothing if there
-            # are no notable changes, so any output at all
-            # means we should run 'git status' on the project.
-            stdout, stderr = None, None
-            try:
-                stdout, stderr = popen.communicate(timeout=0.1)
-            except subprocess.TimeoutExpired:
-                pass
-            except ValueError:
-                # In case this isn't issue35182, handle the exception
-                # anyway.
-                self.wrn(
-                    f'{project.name}: internal error; got ValueError '
-                    'from Popen.communicate() when checking status. '
-                    'Ignoring it, but please report this to the west '
-                    'developers.')
-                return True
-            return stdout or stderr
-
-        while True:
-            if has_output():
-                popen.kill()
-                return True
-            if popen.poll() is not None:
-                break
-
-        return has_output()
-
 class Update(_ProjectCommand):
 
     def __init__(self):
         super().__init__(
             'update',
             'update projects described in west manifest',
             textwrap.dedent('''\
@@ -809,15 +931,14 @@
                             help='''projects (by name or path) to operate on;
                             defaults to all active projects''')
 
         return parser
 
     def do_run(self, args, _):
         self.die_if_no_git()
-        self._setup_logging(args)
         self.init_state(args)
 
         # We can't blindly call self._projects() here: manifests with
         # imports are limited to plain 'west update', and cannot use
         # 'west update PROJECT [...]'.
         if not self.args.projects:
             self.update_all()
@@ -1452,24 +1573,31 @@
     def do_add_parser(self, parser_adder):
         parser = self._parser(parser_adder,
                               epilog=ACTIVE_CLONED_PROJECTS_HELP)
         parser.add_argument('-c', dest='subcommand', metavar='COMMAND',
                             required=True)
         parser.add_argument('-a', '--all', action='store_true',
                             help='include inactive projects'),
+        parser.add_argument('-g', '--group', dest='groups',
+                            default=[], action='append',
+                            help='''only run COMMAND if a project is
+                            in this group; if given more than once,
+                            the command will be run if the project is
+                            in any of the groups''')
         parser.add_argument('projects', metavar='PROJECT', nargs='*',
                             help='''projects (by name or path) to operate on;
                             defaults to active cloned projects''')
         return parser
 
     def do_run(self, args, user_args):
-        self._setup_logging(args)
-
         failed = []
+        group_set = set(args.groups)
         for project in self._cloned_projects(args, only_active=not args.all):
+            if group_set and not group_set.intersection(set(project.groups)):
+                continue
             self.banner(
                 f'running "{args.subcommand}" in {project.name_and_path}:')
             rc = subprocess.Popen(args.subcommand, shell=True,
                                   cwd=project.abspath).wait()
             if rc:
                 failed.append(project)
         self._handle_failed(args, failed)
```

### Comparing `west-1.0.0a1/src/west/commands.py` & `west-1.1.0a1/src/west/commands.py`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/src/west/configuration.py` & `west-1.1.0a1/src/west/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,28 +141,36 @@
 
 class Configuration:
     '''Represents the available configuration options and their values.
 
     Allows getting, setting, and deleting configuration options
     in the system, global, and local files.
 
-    Sets take effect immediately and are not protected against
-    concurrent gets. The caller is responsible for any necessary
+    Setting values affects files immediately and is not protected against
+    concurrent reads. The caller is responsible for any necessary
     mutual exclusion.
+
+    WEST_CONFIG_* environment variables take effect when and only when
+    a Configuration object is created. This can be used to point
+    different objects at different files.
+
+    If no topdir argument is passed to the constructor and WEST_CONFIG_LOCAL
+    is not defined then the object does not point to any local file.
+
     '''
 
     def __init__(self, topdir: Optional[PathType] = None):
         '''Load the system, global, and workspace configurations and
         make them available for the user.
 
         :param topdir: workspace location; may be None
         '''
 
         local_path = _location(ConfigFile.LOCAL, topdir=topdir,
-                               search_for_local=False) or None
+                               find_local=False) or None
 
         self._system_path = Path(_location(ConfigFile.SYSTEM))
         self._global_path = Path(_location(ConfigFile.GLOBAL))
         self._local_path = Path(local_path) if local_path is not None else None
 
         self._system = _InternalCF.from_path(self._system_path)
         self._global = _InternalCF.from_path(self._global_path)
@@ -543,15 +551,15 @@
         if stop:
             break
 
     if not found:
         raise KeyError(f'{section}.{key}')
 
 def _location(cfg: ConfigFile, topdir: Optional[PathType] = None,
-              search_for_local: bool = True) -> str:
+              find_local: bool = True) -> str:
     # Making this a function that gets called each time you ask for a
     # configuration file makes it respect updated environment
     # variables (such as XDG_CONFIG_HOME, PROGRAMDATA) if they're set
     # during the program lifetime.
     #
     # Its existence is also relied on in the test cases, to ensure
     # that the WEST_CONFIG_xyz variables are respected and we're not about
@@ -606,15 +614,15 @@
     elif cfg == ConfigFile.LOCAL:
         if 'WEST_CONFIG_LOCAL' in env:
             return env['WEST_CONFIG_LOCAL']
 
         if topdir:
             return os.fspath(Path(topdir) / '.west' / 'config')
 
-        if search_for_local:
+        if find_local:
             # Might raise WestNotFound!
             return os.fspath(Path(west_dir()) / 'config')
         else:
             return ''
     else:
         raise ValueError(f'invalid configuration file {cfg}')
```

### Comparing `west-1.0.0a1/src/west/log.py` & `west-1.1.0a1/src/west/log.py`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/src/west/manifest-schema.yml` & `west-1.1.0a1/src/west/manifest-schema.yml`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/src/west/manifest.py` & `west-1.1.0a1/src/west/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 
 '''
 Parser and abstract data types for west manifests.
 '''
 
+from collections import deque
 import enum
 import errno
 import logging
 import os
 from pathlib import PurePosixPath, Path
 import re
 import shlex
@@ -42,30 +43,34 @@
 QUAL_MANIFEST_REV_BRANCH = 'refs/heads/' + MANIFEST_REV_BRANCH
 
 #: Git ref space used by west for internal purposes.
 QUAL_REFS_WEST = 'refs/west/'
 
 #: The latest manifest schema version supported by this west program.
 #:
-#: This value changes when a new version of west includes new manifest
-#: file features not supported by earlier versions of west.
-SCHEMA_VERSION = '0.13'
+#: This value will change whenever a new version of west includes new
+#: manifest file features not supported by earlier versions of west.
+#: (Its value changed to 1.0 following the release of west versions
+#: v1.0.x, so that users can say "I want schema version 1" instead of
+#: having to keep using '0.13', which was the previous version this
+#: changed.)
+SCHEMA_VERSION = '1.0'
 # MAINTAINERS:
 #
 # - Make sure to update _VALID_SCHEMA_VERS if you change this.
 #
-# - When changing this, make sure that it has the exact same value as
-#   west.version.__version__ when the next release is cut.
+# - When changing this, make sure that it matches the major.minor
+#   version of west itself. E.g. if you add a new manifest feature for
+#   west 1.6, then SCHEMA_VERSION above should be 1.6, and west's
+#   release version numbers should be 1.6.x.
 
 #
 # Internal helpers
 #
 
-# Type aliases
-
 # The value of a west-commands as passed around during manifest
 # resolution. It can become a list due to resolving imports, even
 # though it's just a str in each individual file right now.
 WestCommandsType = Union[str, List[str]]
 
 # Type for the importer callback passed to the manifest constructor.
 # (ImportedContentType is just an alias for what it gives back.)
@@ -80,14 +85,89 @@
 
 # A list of group names to enable and disable, like ['+foo', '-bar'].
 GroupFilterType = List[str]
 
 # A list of group names belonging to a project, like ['foo', 'bar']
 GroupsType = List[str]
 
+class PFR(enum.Enum):
+    # "Project filter result": internal type for expressing whether a
+    # project has been explicitly made active or inactive via
+    # manifest.project-filter.
+
+    ACTIVE = 1
+    INACTIVE = 2
+    NONE = 3
+
+# Type for an individual element of a project filter.
+class ProjectFilterElt(NamedTuple):
+    # The regular expression to match against project names
+    # when applying the filter. This must match the entire project
+    # name in order for this filter to apply.
+    pattern: re.Pattern
+
+    # If True, projects whose names match 'pattern' are explicitly
+    # made active. If False, projects whose names match the regular
+    # expression are made inactive.
+    make_active: bool
+
+# The internal representation for a 'manifest.project-filter'
+# configuration option's value.
+#
+# If an individual list element matches, it makes the project active
+# or inactive accordingly. The "activate/inactivate result" from the
+# last match in the list "wins". If there are no matches, the
+# project's active/inactive status is not changed by the filter.
+#
+# For example, "-hal_.*,+hal_my_vendor' would make all projects
+# whose names start with 'hal_' inactive, except a project named exactly
+# 'hal_my_vendor'. We would represent that like this:
+#
+#   [ProjectFilterElt(re.compile('hal_.*'), False),
+#    ProjectFilterElt(re.compile('hal_my_vendor'), True)]
+#
+# The regular expression must match the entire project name.
+ProjectFilterType = List[ProjectFilterElt]
+
+def _update_project_filter(project_filter: ProjectFilterType,
+                           option_value: Optional[str]) -> None:
+    # Validate a 'manifest.project-filter' configuration option's
+    # value. The 'option_value' argument is the raw configuration
+    # option. If 'option_value' is invalid, error out. Otherwise,
+    # destructively modify 'project_filter' to reflect the option's
+    # value.
+
+    if option_value is None:
+        return
+
+    def _err(message):
+        raise MalformedConfig(
+            f'invalid "manifest.project-filter" option value '
+            f'"{option_value}": {message}')
+
+    for elt in option_value.split(','):
+        elt = elt.strip()
+        if not elt:
+            continue
+        elif not elt.startswith(('-', '+')):
+            _err(f'element "{elt}" does not start with "+" or "-"')
+        if len(elt) == 1:
+            _err('a bare "+" or "-" contains no regular expression')
+
+        make_active = elt.startswith('+')
+        regexp = elt[1:]
+
+        try:
+            pattern = re.compile(regexp)
+        except re.error as e:
+            _err(f'invalid regular expression "{regexp}": {str(e)}')
+
+        project_filter.append(ProjectFilterElt(pattern=pattern,
+                                               make_active=make_active))
+
 # The parsed contents of a manifest YAML file as returned by _load(),
 # after sanitychecking with validate().
 ManifestDataType = Union[str, Dict]
 
 # Logging
 
 _logger = logging.getLogger(__name__)
@@ -111,15 +191,15 @@
 _DEFAULT_REV = 'master'
 _WEST_YML = 'west.yml'
 _SCHEMA_PATH = os.path.join(os.path.dirname(__file__), "manifest-schema.yml")
 _SCHEMA_VER = parse_version(SCHEMA_VERSION)
 _EARLIEST_VER_STR = '0.6.99'  # we introduced the version feature after 0.6
 _VALID_SCHEMA_VERS = [
     _EARLIEST_VER_STR,
-    '0.7', '0.8', '0.9', '0.10', '0.12',
+    '0.7', '0.8', '0.9', '0.10', '0.12', '0.13',
     SCHEMA_VERSION
 ]
 
 def _is_yml(path: PathType) -> bool:
     return Path(path).suffix in ['.yml', '.yaml']
 
 def _load(data: str) -> Any:
@@ -260,35 +340,38 @@
 
     if blocked:
         return allowed
     else:
         return allowed or no_allowlists
 
 class _import_ctx(NamedTuple):
-    # Holds state that changes as we recurse down the manifest import tree.
+    # Holds shared state that we want to pass around as we
+    # resolve imports.
 
     # The current map from already-defined project names to Projects.
     #
     # This is shared, mutable state between Manifest() constructor
     # calls that happen during resolution. We mutate this directly
     # when handling 'manifest: projects:' lists. Manifests which are
     # imported earlier get higher precedence: if a 'projects:' list
     # contains a name which is already present here, we ignore that
     # element.
     projects: Dict[str, 'Project']
 
-    # The current shared group filter. This is mutable state in the
-    # same way 'projects' is. Manifests which are imported earlier get
-    # higher precedence here too.
-    #
-    # This is done by prepending (NOT appending) any 'manifest:
-    # group-filter:' lists we encounter during import resolution onto
-    # this list. Since group-filter lists have "last entry wins"
-    # semantics, earlier manifests take precedence.
-    group_filter: GroupFilterType
+    # The project filters we should apply while resolving imports. We
+    # try to load this only once from the 'manifest.project-filter'
+    # configuration option.
+    project_filter: ProjectFilterType
+
+    # Deque of group filters from every manifest we import.
+    # Manifests that are imported *earlier* appear *later*
+    # in the queue. That means that iterating over the queue
+    # is the same thing as iterating over group filters in
+    # the import tree in precedence order.
+    group_filter_q: deque
 
     # The list of west command names provided by the manifest
     # repository itself. This is mutable state in the same way
     # 'projects' is. Manifests which are imported earlier get
     # higher precedence here as usual.
     manifest_west_commands: List[str]
 
@@ -348,16 +431,24 @@
         # These type annotated versions silence mypy warnings.
         fn1: Callable[['Project'], bool] = imap_filter1
         fn2: Callable[['Project'], bool] = imap_filter2
         return lambda project: (fn1(project) and fn2(project))
     else:
         return imap_filter1 or imap_filter2
 
+# It's an error if a group name matches this pattern.
 _RESERVED_GROUP_RE = re.compile(r'(^[+-]|[\s,:])')
+
+# _INVALID_PROJECT_NAME_RE: pattern for project names that
+#                           are errors
+# _RESERVED_PROJECT_NAME_RE: pattern for names that cause warnings by
+#                            default for now, but will be errors later
+#                            (west 2.0 or later)
 _INVALID_PROJECT_NAME_RE = re.compile(r'([/\\])')
+_RESERVED_PROJECT_NAME_RE = re.compile(r'[\s,]')
 
 def _update_disabled_groups(disabled_groups: Set[str],
                             group_filter: GroupFilterType):
     # Update a set of disabled groups in place based on
     # 'group_filter'.
 
     for item in group_filter:
@@ -555,20 +646,22 @@
 
     def __init__(self, project: Optional['Project'], imp: Any):
         super().__init__()
         self.project = project
         self.imp = imp
 
     def __str__(self):
-        if self.project is not None:
-            return (f'ManifestImportFailed: project {self.project} '
-                    f'value {self.imp}')
-        else:
-            return (f'ManifestImportFailed: manifest repository '
-                    f'value {self.imp}')
+        if self.project is None:
+            # This happens when imports fail in the manifest repository
+            return (f'cannot import {self.imp}; is it present '
+                    'in your manifest repository?')
+        else:
+            return (f'project {self.project.name_and_path}: '
+                    f'cannot import contents of {self.imp}; '
+                    'do you need to run "west update"?')
 
 
 class ManifestVersionError(Exception):
     '''The manifest required a version of west more recent than the
     current version.
     '''
 
@@ -1231,15 +1324,16 @@
             - ``topdir``: the workspace top level directory as a string
                with symlinks resolved, or None
 
             - ``projects``: sequence of `Project` instances
 
             - ``has_imports``: bool, True if the manifest contains
               an "import:" attribute in "self:" or "projects:" that were
-              not ignored due to *import_flags*; False otherwise
+              not ignored due to *import_flags* or manifest.project-filter;
+              False otherwise
 
             - ``group_filter``: a group filter value equivalent to
               the resolved manifest's "group-filter:", along with any
               values from imported manifests. This value may be simpler
               than the actual input data.
 
         You must give exactly one of the *topdir* and *source_data* kwargs:
@@ -1333,26 +1427,32 @@
                 topdir_abspath = Path(topdir).resolve()
             if TYPE_CHECKING:
                 assert topdir_abspath is not None
             self.topdir = os.fspath(topdir_abspath)
         else:
             topdir_abspath = None
         self.has_imports: bool = False
+        # The final, effective group filter, with simplifications
+        # applied so that e.g. ['-foo', '+foo', '-bar'] becomes
+        # ['-bar'], with filters imported from other manifests applied.
         self.group_filter: GroupFilterType = []
 
         # Initialize private state, some of which is also overwritten
         # later as needed.
 
-        # This backs group_filter.
-        self._disabled_groups: Set[str] = set()
         # This backs the projects() property.
         self._projects: List[Project] = []
+        # The final set of groups which are explicitly disabled in
+        # this manifest data, after resolving imports. This is used
+        # as an optimization in is_active().
+        self._disabled_groups: Set[str] = set()
         # The "raw" (unparsed) manifest.group-filter configuration
         # option in the local configuration file. See
-        # _config_group_filter().
+        # _config_group_filter(); only initialized if self._top_level
+        # is True and if we're loading from a file in a workspace.
         self._raw_config_group_filter: Optional[str] = None
         # A helper attribute we use for schema version v0.9 compatibility.
         self._top_level_group_filter: GroupFilterType = []
         # The manifest.path configuration option in the local
         # configuration file, as a Path.
         self._config_path: Optional[Path] = None
         # These back the relevant properties.
@@ -1553,31 +1653,62 @@
         '''
         return self._projects
 
     def is_active(self, project: Project,
                   extra_filter: Optional[Iterable[str]] = None) -> bool:
         '''Is a project active?
 
-        Projects with empty 'project.groups' lists are always active.
+        If the manifest.project-filter configuration option is set,
+        the return value determined by the option's value:
 
-        Otherwise, if any group in 'project.groups' is enabled by this
-        manifest's 'group-filter:' list (and the
-        'manifest.group-filter' local configuration option, if we have
-        a workspace), returns True.
+        - The elements of the manifest.project-filter value are checked
+          against the project's name. If the regular expression in the
+          element matches the project's name, then the project is active
+          or inactive depending on if the element begins with + or -
+          respectively.
+
+        - If multiple elements have regular expressions matching the
+          project's name, the last element which has a match determines
+          the result.
+
+        - This function returns True or False if the project is active or
+          inactive according to these rules.
+
+        The manifest.project-filter value that was set at the time
+        this Manifest object was constructed is used.
+
+        Otherwise, the return value depends on whether the project has
+        any groups, and if so, whether they are enabled:
+
+        - Projects with empty 'project.groups' lists are always active,
+          and this function returns True for such projects.
+
+        - If 'project.groups' is not empty, and any group in it is
+          enabled by this manifest's 'group-filter:' list (and the
+          'manifest.group-filter' local configuration option, if we
+          have a workspace), this returns True.
 
-        Otherwise, i.e. if all of the project's groups are disabled,
-        this returns False.
+        - Otherwise, i.e. if all of the project's groups are disabled,
+          this returns False.
 
         "Inactive" projects should generally be considered absent from
-        the workspace for purposes like updating it, listing projects,
-        etc.
+        the workspace for purposes like updating, listing, resolving
+        imports, etc.
 
         :param project: project to check
         :param extra_filter: an optional additional group filter
         '''
+
+        if not isinstance(project, ManifestProject):
+            pfr = self._pfr(project)
+            if pfr == PFR.ACTIVE:
+                return True
+            elif pfr == PFR.INACTIVE:
+                return False
+
         if not project.groups:
             # Projects without any groups are always active, so just
             # exit early. Note that this happens to treat the
             # ManifestProject as though it's always active. This is
             # important for keeping it in the 'west list' output for
             # now.
             return True
@@ -1597,14 +1728,29 @@
                                                             list(extra_filter))
                 _update_disabled_groups(disabled_groups, extra_filter)
         else:
             disabled_groups = self._disabled_groups
 
         return any(group not in disabled_groups for group in project.groups)
 
+    def _pfr(self, project: Project) -> PFR:
+        # Internal helper for checking if a project has been
+        # made explicitly active or inactive.
+
+        name = project.name
+        ret = PFR.NONE
+        for elt in self._ctx.project_filter:
+            if not elt.pattern.fullmatch(name):
+                continue
+            if elt.make_active:
+                ret = PFR.ACTIVE
+            else:
+                ret = PFR.INACTIVE
+        return ret
+
     @property
     def path(self) -> Optional[str]:  # for compatibility
         '''Deprecated. Use abspath instead.'''
         return self.abspath
 
     @property
     def posixpath(self):
@@ -1694,14 +1840,15 @@
         if not _flags_ok(import_flags):
             raise ValueError(f'bad import_flags {import_flags:x}')
 
         current_abspath = None
         current_relpath = None
         current_data = source_data
         current_repo_abspath = None
+        project_filter: ProjectFilterType = []
 
         if topdir_abspath:
             config = config or Configuration(topdir=topdir_abspath)
 
             def get_option(option, default=None):
                 # Gets a ConfigFile.LOCAL option from 'config'.
                 return config.get(option, default=default,
@@ -1719,26 +1866,37 @@
                 _logger.warning('"manifest.path" should not be absolute: %s',
                                 manifest_path_option)
 
             manifest_file = get_option('manifest.file', _WEST_YML)
 
             current_relpath = manifest_path / manifest_file
             current_abspath = topdir_abspath / current_relpath
-            current_data = current_abspath.read_text(encoding='utf-8')
+            try:
+                current_data = current_abspath.read_text(encoding='utf-8')
+            except FileNotFoundError:
+                raise MalformedConfig(
+                    f'file not found: manifest file {current_abspath} '
+                    '(from configuration options '
+                    f'manifest.path="{manifest_path_option}", '
+                    f'manifest.file="{manifest_file}")')
+
             current_repo_abspath = topdir_abspath / manifest_path
 
             self.abspath = os.fspath(current_abspath)
             self.relative_path = os.fspath(current_relpath)
             self.repo_path = os.fspath(manifest_path)
             self.repo_abspath = os.fspath(current_repo_abspath)
             self._raw_config_group_filter = get_option('manifest.group-filter')
             self._config_path = manifest_path
+            _update_project_filter(project_filter,
+                                   config.get('manifest.project-filter'))
 
         return _import_ctx(projects={},
-                           group_filter=[],
+                           project_filter=project_filter,
+                           group_filter_q=deque(),
                            manifest_west_commands=[],
                            imap_filter=None,
                            path_prefix=Path('.'),
                            current_abspath=current_abspath,
                            current_relpath=current_relpath,
                            current_data=current_data,
                            current_repo_abspath=current_repo_abspath,
@@ -1788,15 +1946,14 @@
                      manifest_data.get('remotes', [])}
         defaults = self._load_defaults(manifest_data.get('defaults', {}),
                                        url_bases)
         self._load_projects(manifest_data, url_bases, defaults)
 
         # The manifest is resolved; perform post-resolution validation.
         self._check_paths_are_unique()
-        self._check_names()
 
         # Set up top-level state which relies on the resolved and
         # validated manifest.
         if self._top_level:
             # Create the ManifestProject instance.
             mp = ManifestProject(
                 path=self._config_path if self.topdir else self.yaml_path,
@@ -1807,15 +1964,15 @@
             # that rely on the ManifestProject existing.
             self._projects = list(self._ctx.projects.values())
             self._projects.insert(MANIFEST_PROJECT_INDEX, mp)
             self._projects_by_name: Dict[str, Project] = {'manifest': mp}
             self._projects_by_name.update(self._ctx.projects)
             self._projects_by_rpath: Dict[Path, Project] = {}  # resolved paths
             if self.topdir:
-                for i, p in enumerate(self.projects):
+                for p in self.projects:
                     if TYPE_CHECKING:
                         # The typing module can't tell that self.topdir
                         # being truthy guarantees p.abspath is a str, not None.
                         assert p.abspath
 
                     self._projects_by_rpath[Path(p.abspath).resolve()] = p
 
@@ -1829,28 +1986,28 @@
             # For schema version 0.9, we only want to warn once, at the
             # top level, if the distinction actually matters.
             self.group_filter = self._final_group_filter(schema_version)
 
         _logger.debug(f'loaded {loading_what}')
 
     def _load_group_filter(self, manifest_data: Dict[str, Any]) -> None:
-        # Update self._ctx.group_filter from manifest_data.
+        # Update self._ctx.group_filter_q from manifest_data.
 
         if 'group-filter' not in manifest_data:
             _logger.debug('group-filter: unset')
             return
 
         raw_filter: List[RawGroupType] = manifest_data['group-filter']
         if not raw_filter:
             self._malformed('"manifest: group-filter:" may not be empty')
 
         group_filter = self._validated_group_filter('manifest', raw_filter)
         _logger.debug('group-filter: %s', group_filter)
 
-        self._ctx.group_filter[:0] = group_filter
+        self._ctx.group_filter_q.appendleft(group_filter)
 
         if self._top_level:
             self._top_level_group_filter = group_filter
 
     def _validated_group_filter(
             self, source: Optional[str], raw_filter: List[RawGroupType]
     ) -> GroupFilterType:
@@ -2278,16 +2435,21 @@
 
     def _import_from_project(self, project: Project, imp: Any):
         # Recursively resolve a manifest import from 'project'.
         #
         # - project: Project instance to import from
         # - imp: the parsed value of project's import key (string, list, etc.)
 
-        self._assert_imports_ok()
+        pfr = self._pfr(project)
+        if pfr == PFR.INACTIVE:
+            _logger.debug(f'project {project.name} is inactive due to '
+                          'manifest.project-filter; ignoring its "import:"')
+            return
 
+        self._assert_imports_ok()
         self.has_imports = True
 
         imptype = type(imp)
         if imptype == bool:
             # We should not have been called unless the import was truthy.
             assert imp
             self._import_path_from_project(project, _WEST_YML)
@@ -2423,14 +2585,17 @@
                           name_allowlist,
                           path_allowlist,
                           name_blocklist,
                           path_blocklist,
                           copy.pop('path-prefix', ''))
 
         # Check that the value is OK.
+        #
+        # If you modify the error handling here, be sure to
+        # update test_import_map_error_handling() as needed.
         if copy:
             # We popped out all of the valid keys already.
             self._malformed(f'{src}: invalid import contents: {copy}')
         elif not _is_imap_list(ret.name_allowlist):
             self._malformed(f'{src}: bad import name-allowlist '
                             f'{ret.name_allowlist}')
         elif not _is_imap_list(ret.path_allowlist):
@@ -2450,68 +2615,91 @@
         return ret
 
     def _add_project(self, project: Project) -> bool:
         # Add the project to our map if we don't already know about it.
         # Return the result.
 
         if project.name not in self._ctx.projects:
+            self._check_project_name(project)
             self._ctx.projects[project.name] = project
             _logger.debug('added project %s path %s revision %s%s%s',
                           project.name, project.path, project.revision,
                           (f' from {self.abspath}' if self.abspath else ''),
                           (f' groups {project.groups}' if project.groups
                            else ''))
             return True
         else:
             return False
 
+    def _check_project_name(self, project):
+        name = project.name
+        if _INVALID_PROJECT_NAME_RE.search(name):
+            self._malformed(f'Invalid project name: {name}')
+        if _RESERVED_PROJECT_NAME_RE.search(name):
+            if self._ctx.current_abspath:
+                context = f' (defined in {self._ctx.current_abspath})'
+            elif self._ctx.current_repo_abspath:
+                context = f' (loaded from {self._ctx.current_repo_abspath})'
+            if self._ctx.project_filter:
+                raise MalformedConfig(
+                    f'project "{name}"{context} contains comma (",") or '
+                    'whitespace; this is incompatible with use of the '
+                    'manifest.project-filter option. '
+                    '(These characters will be forbidden entirely in a '
+                    'future version of west.)')
+            else:
+                _logger.warning(
+                    f'project "{name}"{context} contains comma (",") or '
+                    'whitespace; this will be forbidden in a future version '
+                    'of west')
+
     def _check_paths_are_unique(self) -> None:
         ppaths: Dict[Path, Project] = {}
         for name, project in self._ctx.projects.items():
             pp = Path(project.path)
             if self._top_level and pp == self._config_path:
                 self._malformed(f'project {name} path "{project.path}" '
                                 'is taken by the manifest repository')
             other = ppaths.get(pp)
             if other:
                 self._malformed(f'project {name} path "{project.path}" '
                                 f'is taken by project {other.name}')
             ppaths[pp] = project
 
-    def _check_names(self) -> None:
-        for name, project in self._ctx.projects.items():
-            if _INVALID_PROJECT_NAME_RE.search(name):
-                self._malformed(f'Invalid project name: {name}')
-
     def _final_group_filter(self, schema_version: str):
         # Update self.group_filter based on the schema version.
 
         if schema_version == '0.9':
             # If the user requested v0.9.x group-filter semantics,
             # provide them, but emit a warning that can't be silenced
             # if group filters were used anywhere.
             #
             # Hopefully no users ever actually see this warning.
 
-            if self._ctx.group_filter:
+            if any(self._ctx.group_filter_q):
                 _logger.warning(
                     "providing deprecated group-filter semantics "
                     "due to explicit 'manifest: version: 0.9'; "
                     "for the new semantics, use "
                     "'manifest: version: \"0.10\"' or later")
 
                 # Set attribute for white-box testing the above warning.
                 self._legacy_group_filter_warned = True
 
             return self._top_level_group_filter
 
         else:
-            _update_disabled_groups(self._disabled_groups,
-                                    self._ctx.group_filter)
-            return [f'-{g}' for g in self._disabled_groups]
+            _logger.debug(
+                'group filters in precedence order (later is higher): %s',
+                self._ctx.group_filter_q)
+            for group_filter in self._ctx.group_filter_q:
+                _update_disabled_groups(self._disabled_groups, group_filter)
+            ret = [f'-{g}' for g in self._disabled_groups]
+            _logger.debug('final top level group-filter: %s', ret)
+            return ret
 
 class _PatchedConfiguration(Configuration):
     # Internal helper class that fakes out manifest.path and manifest.file
     # to point at another location. Used by Manifest.from_file().
 
     def __init__(self, patch_dict, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `west-1.0.0a1/src/west/util.py` & `west-1.1.0a1/src/west/util.py`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/src/west/version.py` & `west-1.1.0a1/src/west/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2019, Nordic Semiconductor ASA
 #
 # Don't put anything else in here!
 #
 # This is the Python 3 version of option 3 in:
 # https://packaging.python.org/guides/single-sourcing-package-version/#single-sourcing-the-version
 
-__version__ = '1.0.0a1'
+__version__ = '1.1.0a1'
 #
 # MAINTAINERS:
 #
 # Make sure to update west.manifest.SCHEMA_VERSION if there have been
 # manifest schema version changes since the last release.
 #
 # Note that this is the "logical" west manifest schema, and that the
```

### Comparing `west-1.0.0a1/src/west/west-commands-schema.yml` & `west-1.1.0a1/src/west/west-commands-schema.yml`

 * *Files identical despite different names*

### Comparing `west-1.0.0a1/src/west.egg-info/PKG-INFO` & `west-1.1.0a1/src/west.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: west
-Version: 1.0.0a1
+Version: 1.1.0a1
 Summary: Zephyr RTOS Project meta-tool
 Home-page: https://github.com/zephyrproject-rtos/west
 Author: Zephyr Project
 Author-email: devel@lists.zephyrproject.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -34,19 +34,20 @@
 single file, called the *west manifest file*, or *manifest* for short.
 By default the manifest file is named ``west.yml``.
 You use ``west init`` to set up this directory, then ``west update`` to fetch
 and/or update the repositories named in the manifest.
 
 By default, west uses `upstream Zephyr's manifest file
 <https://github.com/zephyrproject-rtos/zephyr/blob/main/west.yml>`_, but west
-doesn't care if the manifest repository is a Zephyr tree or not.
+doesn't care if the manifest repository is zephyr or not. You can and are
+encouraged to make your own manifest repositories to meet your needs.
 
-For more details, see `Multiple Repository Management
-<https://docs.zephyrproject.org/latest/guides/west/repo-tool.html>`_ in the
-west documentation.
+For more details, see the `West guide
+<https://docs.zephyrproject.org/latest/guides/west/index.html>`_ in the Zephyr
+documentation.
 
 Example usage using the upstream manifest file::
 
   mkdir zephyrproject && cd zephyrproject
   west init
   west update
 
@@ -94,19 +95,33 @@
   tox
 
 See the tox configuration file, tox.ini, for more details.
 
 Hacking on West
 ---------------
 
+This section contains notes for getting started developing west itself.
+
+Editable Install
+~~~~~~~~~~~~~~~~
+
+To run west "live" from the current source code tree, run this command from the
+top level directory in the west repository::
+
+  pip3 install -e .
+
+This is useful if you are actively working on west and don't want to re-package
+and install a wheel each time you run it.
+
 Installing from Source
 ~~~~~~~~~~~~~~~~~~~~~~
 
-The `wheel`_ package is required to install west from source. See "Installing
-Wheel" below if you don't have ``wheel`` installed.
+You can create and install a wheel package to install west as well.
+The `wheel`_ Python package is required to do this. See "Installing Wheel"
+below if you need to do this.
 
 To build the west wheel file::
 
   # macOS, Linux
   python3 setup.py bdist_wheel
 
   # Windows
@@ -118,25 +133,14 @@
 To install the wheel::
 
   pip3 install -U dist/west-x.y.z-py3-none-any.whl
 
 You can ``pip3 uninstall west`` to remove this wheel before re-installing the
 version from PyPI, etc.
 
-Editable Install
-~~~~~~~~~~~~~~~~
-
-To run west "live" from the current source code tree, run this command from the
-top level directory in the west repository::
-
-  pip3 install -e .
-
-This is useful if you are actively working on west and don't want to re-package
-and install a wheel each time you run it.
-
 Installing Wheel
 ~~~~~~~~~~~~~~~~
 
 On macOS and Windows, you can install wheel with::
 
   pip3 install wheel
```

### Comparing `west-1.0.0a1/src/west.egg-info/SOURCES.txt` & `west-1.1.0a1/src/west.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,8 +19,14 @@
 src/west.egg-info/entry_points.txt
 src/west.egg-info/not-zip-safe
 src/west.egg-info/requires.txt
 src/west.egg-info/top_level.txt
 src/west/app/__init__.py
 src/west/app/config.py
 src/west/app/main.py
-src/west/app/project.py
+src/west/app/project.py
+tests/test_commands.py
+tests/test_config.py
+tests/test_help.py
+tests/test_main.py
+tests/test_manifest.py
+tests/test_project.py
```

