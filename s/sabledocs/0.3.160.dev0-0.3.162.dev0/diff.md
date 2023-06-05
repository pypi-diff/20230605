# Comparing `tmp/sabledocs-0.3.160.dev0.tar.gz` & `tmp/sabledocs-0.3.162.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.3.160.dev0.tar", last modified: Mon Jun  5 20:16:25 2023, max compression
+gzip compressed data, was "sabledocs-0.3.162.dev0.tar", last modified: Mon Jun  5 20:18:05 2023, max compression
```

## Comparing `sabledocs-0.3.160.dev0.tar` & `sabledocs-0.3.162.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:25.071799 sabledocs-0.3.160.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-05 20:16:25.071799 sabledocs-0.3.160.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-06-05 20:16:25.071799 sabledocs-0.3.160.dev0/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:25.063798 sabledocs-0.3.160.dev0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:25.067798 sabledocs-0.3.160.dev0/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13732 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:25.063798 sabledocs-0.3.160.dev0/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:25.071799 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:25.071799 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-06-05 20:16:00.000000 sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:16:25.067798 sabledocs-0.3.160.dev0/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-05 20:16:25.000000 sabledocs-0.3.160.dev0/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-05 20:16:25.000000 sabledocs-0.3.160.dev0/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-05 20:16:25.000000 sabledocs-0.3.160.dev0/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-05 20:16:25.000000 sabledocs-0.3.160.dev0/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-05 20:16:25.000000 sabledocs-0.3.160.dev0/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-05 20:16:25.000000 sabledocs-0.3.160.dev0/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:18:05.401253 sabledocs-0.3.162.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-05 20:18:05.401253 sabledocs-0.3.162.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-06-05 20:18:05.401253 sabledocs-0.3.162.dev0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:18:05.397253 sabledocs-0.3.162.dev0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:18:05.401253 sabledocs-0.3.162.dev0/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13681 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:18:05.397253 sabledocs-0.3.162.dev0/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:18:05.401253 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:18:05.401253 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-06-05 20:17:52.000000 sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:18:05.401253 sabledocs-0.3.162.dev0/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-05 20:18:05.000000 sabledocs-0.3.162.dev0/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-05 20:18:05.000000 sabledocs-0.3.162.dev0/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-05 20:18:05.000000 sabledocs-0.3.162.dev0/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-05 20:18:05.000000 sabledocs-0.3.162.dev0/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-05 20:18:05.000000 sabledocs-0.3.162.dev0/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-05 20:18:05.000000 sabledocs-0.3.162.dev0/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.3.160.dev0/LICENSE` & `sabledocs-0.3.162.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/PKG-INFO` & `sabledocs-0.3.162.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.3.160.dev0
+Version: 0.3.162.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.3.160.dev0/README.md` & `sabledocs-0.3.162.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/pyproject.toml` & `sabledocs-0.3.162.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/__main__.py` & `sabledocs-0.3.162.dev0/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/lunr_search.py` & `sabledocs-0.3.162.dev0/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.3.162.dev0/src/sabledocs/proto_descriptor_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,16 +151,14 @@
     m.repository_url = build_source_code_url(
         ctx.config.repository_url,
         ctx.config.repository_type,
         ctx.config.repository_branch,
         m.source_file_path,
         m.line_number)
 
-    print(f"Full name of message: {m.full_name}")
-
     m.is_map_entry = message.options.map_entry
     for i, mf in enumerate(message.field):
         m.fields.append(parse_field(mf, ctx.ExtendPath(COMMENT_MESSAGE_FIELD_INDEX, i)))
 
     m.fields.sort(key=lambda mf: mf.number)
 
     parse_messages(message.nested_type, ctx.ExtendPath(COMMENT_MESSAGE_MESSAGE_INDEX), m, f"{message.name}.")
```

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/proto_model.py` & `sabledocs-0.3.162.dev0/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/sable_config.py` & `sabledocs-0.3.162.dev0/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/base.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/index.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/message.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/package.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/search.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/service.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.3.162.dev0/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.3.162.dev0/src/sabledocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.3.160.dev0
+Version: 0.3.162.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.3.160.dev0/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.3.162.dev0/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

