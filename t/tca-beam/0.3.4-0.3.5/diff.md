# Comparing `tmp/tca_beam-0.3.4.tar.gz` & `tmp/tca_beam-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tca_beam-0.3.4.tar", max compression
+gzip compressed data, was "tca_beam-0.3.5.tar", max compression
```

## Comparing `tca_beam-0.3.4.tar` & `tca_beam-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      134 2023-06-04 22:52:29.592758 tca_beam-0.3.4/README.md
--rw-r--r--   0        0        0      420 2023-06-05 13:51:57.621551 tca_beam-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.3.4/tca_beam/__init__.py
--rw-r--r--   0        0        0     6363 2023-06-05 13:51:30.716704 tca_beam-0.3.4/tca_beam/tca_beam.py
--rw-r--r--   0        0        0      526 2023-06-05 10:09:21.285125 tca_beam-0.3.4/tca_beam/templates/AllPreviews.swift
--rw-r--r--   0        0        0       86 2023-06-04 16:14:37.894614 tca_beam-0.3.4/tca_beam/templates/OneFile.swift
--rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.3.4/tca_beam/templates/TwoFile_ReducerPart.swift
--rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.3.4/tca_beam/templates/TwoFile_ViewPart.swift
--rw-r--r--   0        0        0      633 2023-06-05 09:48:58.421080 tca_beam-0.3.4/tca_beam/templates/View.swift
--rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.3.4/tca_beam/templates/ViewFeature.swift
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 tca_beam-0.3.4/setup.py
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 tca_beam-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.3.5/README.md
+-rw-r--r--   0        0        0      419 2023-06-05 16:56:48.721051 tca_beam-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.3.5/tca_beam/__init__.py
+-rw-r--r--   0        0        0     6467 2023-06-05 14:40:07.483250 tca_beam-0.3.5/tca_beam/tca_beam.py
+-rw-r--r--   0        0        0      526 2023-06-05 10:09:21.285125 tca_beam-0.3.5/tca_beam/templates/AllPreviews.swift
+-rw-r--r--   0        0        0       86 2023-06-04 16:14:37.894614 tca_beam-0.3.5/tca_beam/templates/OneFile.swift
+-rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.3.5/tca_beam/templates/TwoFile_ReducerPart.swift
+-rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.3.5/tca_beam/templates/TwoFile_ViewPart.swift
+-rw-r--r--   0        0        0      633 2023-06-05 09:48:58.421080 tca_beam-0.3.5/tca_beam/templates/View.swift
+-rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.3.5/tca_beam/templates/ViewFeature.swift
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.3.5/setup.py
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 tca_beam-0.3.5/PKG-INFO
```

### Comparing `tca_beam-0.3.4/tca_beam/tca_beam.py` & `tca_beam-0.3.5/tca_beam/tca_beam.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,18 @@
         echo(start.get_help(click.get_current_context()))
         sys.exit(1)
 
     p("")
     p("tca-beam is preparing two-by-fours...")
     p("")
 
+    # if dry_run:
+    #     p("In DRY-RUN mode. No files or folders will be created.")
+    #     p("")
+
     script_dir = os.path.abspath(os.path.dirname(__file__))
 
     templates_path = make_abs_path('templates')
     file_loader = FileSystemLoader(templates_path)
     env = Environment(loader=file_loader)
 
     run(env, script_dir, two_files, sub_dirs, preview_all, force_overwrite, dry_run, feature_names)
```

### Comparing `tca_beam-0.3.4/tca_beam/templates/AllPreviews.swift` & `tca_beam-0.3.5/tca_beam/templates/AllPreviews.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.3.4/tca_beam/templates/View.swift` & `tca_beam-0.3.5/tca_beam/templates/View.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.3.4/setup.py` & `tca_beam-0.3.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['click>=8.1.3,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tca-beam = tca_beam.tca_beam:start']}
 
 setup_kwargs = {
     'name': 'tca-beam',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Feature stub generation for The Composable Architecture',
-    'long_description': 'This is a proof-of-concept implementation of [Scaffold for The Composable Architecture](../README.md) in Python.\n\nWork in progress!\n\n\n',
+    'long_description': 'TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.\n\nhttps://github.com/alexhunsley/tca-beam\n\n',
     'author': 'Alex Hunsley',
     'author_email': 'alex.hunsley@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.4,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `tca_beam-0.3.4/PKG-INFO` & `tca_beam-0.3.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: tca-beam
-Version: 0.3.4
+Version: 0.3.5
 Summary: Feature stub generation for The Composable Architecture
 Author: Alex Hunsley
 Author-email: alex.hunsley@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.4,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Description-Content-Type: text/markdown
 
-This is a proof-of-concept implementation of [Scaffold for The Composable Architecture](../README.md) in Python.
-
-Work in progress!
+TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.
 
+https://github.com/alexhunsley/tca-beam
```

