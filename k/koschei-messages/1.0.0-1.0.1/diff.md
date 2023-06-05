# Comparing `tmp/koschei-messages-1.0.0.tar.gz` & `tmp/koschei-messages-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koschei-messages-1.0.0.tar", max compression
+gzip compressed data, was "koschei-messages-1.0.1.tar", max compression
```

## Comparing `koschei-messages-1.0.0.tar` & `koschei-messages-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0        0        0        0 2023-06-03 05:53:25.239104 koschei-messages-1.0.0/LICENSES/
--rw-r--r--   0        0        0      335 2023-06-03 06:42:24.832011 koschei-messages-1.0.0/README.md
--rw-r--r--   0        0        0      196 2023-06-03 06:25:14.942660 koschei-messages-1.0.0/koschei_messages/__init__.py
--rw-r--r--   0        0        0      694 2023-06-03 06:26:06.663828 koschei-messages-1.0.0/koschei_messages/base.py
--rw-r--r--   0        0        0     2012 2023-06-03 06:26:06.664827 koschei-messages-1.0.0/koschei_messages/collection.py
--rw-r--r--   0        0        0     2736 2023-06-03 06:26:06.664827 koschei-messages-1.0.0/koschei_messages/package.py
--rw-r--r--   0        0        0     2166 2023-06-03 06:34:35.139471 koschei-messages-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1444 2023-06-03 07:00:04.470800 koschei-messages-1.0.0/setup.py
--rw-r--r--   0        0        0     1493 2023-06-03 07:00:04.471061 koschei-messages-1.0.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-06-03 05:53:25.239104 koschei-messages-1.0.1/LICENSES/
+-rw-r--r--   0        0        0      335 2023-06-03 06:42:24.832011 koschei-messages-1.0.1/README.md
+-rw-r--r--   0        0        0      196 2023-06-03 06:25:14.942660 koschei-messages-1.0.1/koschei_messages/__init__.py
+-rw-r--r--   0        0        0      694 2023-06-03 06:26:06.663828 koschei-messages-1.0.1/koschei_messages/base.py
+-rw-r--r--   0        0        0     2012 2023-06-03 06:26:06.664827 koschei-messages-1.0.1/koschei_messages/collection.py
+-rw-r--r--   0        0        0     2736 2023-06-03 06:26:06.664827 koschei-messages-1.0.1/koschei_messages/package.py
+-rw-r--r--   0        0        0     2166 2023-06-05 07:44:52.095758 koschei-messages-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1419 2023-06-05 07:46:09.579719 koschei-messages-1.0.1/setup.py
+-rw-r--r--   0        0        0     1455 2023-06-05 07:46:09.580103 koschei-messages-1.0.1/PKG-INFO
```

### Comparing `koschei-messages-1.0.0/koschei_messages/base.py` & `koschei-messages-1.0.1/koschei_messages/base.py`

 * *Files identical despite different names*

### Comparing `koschei-messages-1.0.0/koschei_messages/collection.py` & `koschei-messages-1.0.1/koschei_messages/collection.py`

 * *Files identical despite different names*

### Comparing `koschei-messages-1.0.0/koschei_messages/package.py` & `koschei-messages-1.0.1/koschei_messages/package.py`

 * *Files identical despite different names*

### Comparing `koschei-messages-1.0.0/pyproject.toml` & `koschei-messages-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Contributors to the Fedora Project
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 [tool.poetry]
 name = "koschei-messages"
-version = "1.0.0"
+version = "1.0.1"
 description = "A schema package for messages sent by Koschei"
 authors = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 license = "GPLv2-or-later"
 readme = "README.md"
 homepage = "https://github.com/fedora-infra/koschei-messages"
 repository = "https://github.com/fedora-infra/koschei-messages"
 keywords = ["fedora-messaging"]
@@ -25,22 +25,22 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fedora-messaging = "^3.3.0"
 coverage = {extras = ["toml"], version = "^7.2.7"}
-reuse = "^1.1.2"
 
 [tool.poetry.dev-dependencies]
 poetry = "^1.2.0b2"
 black = ">=22.6.0"
 pytest = "^7.1.2"
 pytest-cov = ">=3.0.0"
 ruff = ">=0.0.253"
+reuse = "^1.1.2"
 
 [tool.poetry.plugins."fedora.messages"]
 "koschei.package.state.change" = "koschei_messages.package:PackageStateChange"
 "koschei.collection.state.change" = "koschei_messages.collection:CollectionStateChange"
 
 [tool.black]
 line-length = 100
```

### Comparing `koschei-messages-1.0.0/setup.py` & `koschei-messages-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 packages = \
 ['koschei_messages']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['coverage[toml]>=7.2.7,<8.0.0',
- 'fedora-messaging>=3.3.0,<4.0.0',
- 'reuse>=1.1.2,<2.0.0']
+['coverage[toml]>=7.2.7,<8.0.0', 'fedora-messaging>=3.3.0,<4.0.0']
 
 entry_points = \
 {'fedora.messages': ['koschei.collection.state.change = '
                      'koschei_messages.collection:CollectionStateChange',
                      'koschei.package.state.change = '
                      'koschei_messages.package:PackageStateChange']}
 
 setup_kwargs = {
     'name': 'koschei-messages',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'A schema package for messages sent by Koschei',
     'long_description': '<!--\nSPDX-FileCopyrightText: 2023 Contributors to the Fedora Project\n\nSPDX-License-Identifier: GPL-2.0-or-later\n-->\n\n# Koschei messages\n\nA schema package for [Koschei](http://github.com/fedora-infra/koschei).\n\nSee the [detailed documentation](https://fedora-messaging.readthedocs.io/en/stable/messages.html) on packaging your schemas.\n',
     'author': 'Fedora Infrastructure Team',
     'author_email': 'infrastructure@lists.fedoraproject.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fedora-infra/koschei-messages',
```

### Comparing `koschei-messages-1.0.0/PKG-INFO` & `koschei-messages-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koschei-messages
-Version: 1.0.0
+Version: 1.0.1
 Summary: A schema package for messages sent by Koschei
 Home-page: https://github.com/fedora-infra/koschei-messages
 License: GPLv2-or-later
 Keywords: fedora-messaging
 Author: Fedora Infrastructure Team
 Author-email: infrastructure@lists.fedoraproject.org
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: coverage[toml] (>=7.2.7,<8.0.0)
 Requires-Dist: fedora-messaging (>=3.3.0,<4.0.0)
-Requires-Dist: reuse (>=1.1.2,<2.0.0)
 Project-URL: Repository, https://github.com/fedora-infra/koschei-messages
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2023 Contributors to the Fedora Project
 
 SPDX-License-Identifier: GPL-2.0-or-later
```

