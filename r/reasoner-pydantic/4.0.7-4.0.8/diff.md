# Comparing `tmp/reasoner-pydantic-4.0.7.tar.gz` & `tmp/reasoner-pydantic-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.7.tar", last modified: Fri May 26 19:32:42 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.8.tar", last modified: Sun Jun  4 23:50:13 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.7.tar` & `reasoner-pydantic-4.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/setup.py
```

### Comparing `reasoner-pydantic-4.0.7/PKG-INFO` & `reasoner-pydantic-4.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.7
+Version: 4.0.8
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.7/README.md` & `reasoner-pydantic-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/message.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/message.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/results.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,19 @@
                 self.score,
                 self.support_graphs,
                 self.scoring_method,
             )
         )
 
     def update(self, other):
-        for k in self.edge_bindings.keys():
-            eb = other.edge_bindings.get(k)
-            if eb:
-                self.edge_bindings[k].update(eb)
+        for k in other.edge_bindings:
+            if k in self.edge_bindings:
+                self.edge_bindings[k].update(other.edge_bindings[k])
+            else:
+                self.edge_bindings[k] = other.edge_bindings[k]
         if other.attributes:
             if self.attributes:
                 self.attributes.update(other.attributes)
             else:
                 self.attributes = other.attributes
         if other.support_graphs:
             if self.support_graphs:
```

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.8/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.7
+Version: 4.0.8
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.7/setup.py` & `reasoner-pydantic-4.0.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.7",
+    version="4.0.8",
     author="Kenneth Morton",
     author_email="kenny@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

