# Comparing `tmp/mlplatformutils-0.8.4.tar.gz` & `tmp/mlplatformutils-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.4.tar", last modified: Mon Jun  5 06:21:57 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.5.tar", last modified: Mon Jun  5 20:05:49 2023, max compression
```

## Comparing `mlplatformutils-0.8.4.tar` & `mlplatformutils-0.8.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 06:21:57.054082 mlplatformutils-0.8.4/
--rw-rw-rw-   0        0        0     3055 2023-06-05 06:21:57.055073 mlplatformutils-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.4/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-05 06:21:57.062077 mlplatformutils-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-05 06:21:51.000000 mlplatformutils-0.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 06:21:56.797362 mlplatformutils-0.8.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 06:21:56.834596 mlplatformutils-0.8.4/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.4/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 06:21:57.049074 mlplatformutils-0.8.4/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3611 2023-06-05 06:21:00.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7274 2023-06-05 06:20:40.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-05 06:21:34.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 06:21:56.939141 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.324216 mlplatformutils-0.8.5/
+-rw-rw-rw-   0        0        0     3055 2023-06-05 20:05:49.325218 mlplatformutils-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.5/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-05 20:05:49.329218 mlplatformutils-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-05 20:05:40.000000 mlplatformutils-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.051883 mlplatformutils-0.8.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.095536 mlplatformutils-0.8.5/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.5/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.321214 mlplatformutils-0.8.5/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8410 2023-06-05 20:03:42.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3611 2023-06-05 06:21:00.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7274 2023-06-05 06:20:40.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-05 20:05:32.000000 mlplatformutils-0.8.5/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:05:49.157546 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 20:05:48.000000 mlplatformutils-0.8.5/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8.4/PKG-INFO` & `mlplatformutils-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.4
+Version: 0.8.5
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.8.4/setup.py` & `mlplatformutils-0.8.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.4',
+    version='0.8.5',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.8.4/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.5/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.4/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.5/src/mlplatformutils/core/lineagegraph.py`

 * *Files 11% similar despite different names*

```diff
@@ -154,8 +154,31 @@
             callback = self.client.submitAsync(query)
             for result in callback.result():
                 print(result)
             self.print_status_attributes(callback.result())
             return result
         except Exception as e:
             traceback.print_exc()
-            raise ValueError("Failed to QUERY Cosmos Gremlin graph!")
+            raise ValueError("Failed to QUERY Cosmos Gremlin graph!")
+        
+    def update_lineage_graph(self,run_id,pipeline_step_name,properties):
+        try:
+            query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+pipeline_step_name+"').values('id')"
+            documentId = self.query_graph(query)[0]
+            self.update_vertex(documentId,properties)
+            return
+        except Exception as e:
+            traceback.print_exc()
+            raise ValueError("Failed to Update lineage graph!")
+        
+    def connect_lineage_graph(self,run_id,source_pipeline_step_name,dest_pipeline_step_name):
+        try:
+            src_query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+source_pipeline_step_name+"').values('id')"
+            source_doc_id = self.query_graph(src_query)[0]
+            dest_query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+dest_pipeline_step_name+"').values('id')"
+            dest_doc_id = self.query_graph(dest_query)[0]
+            self.insert_edges(source_doc_id, dest_doc_id,"DependendsOn", None)
+            return
+        except Exception as e:
+            traceback.print_exc()
+            raise ValueError("Failed to connect lineage graph!")
+
```

### Comparing `mlplatformutils-0.8.4/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.8.5/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.4/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.5/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.4/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.5/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.4/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.8.5/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.4
+Version: 0.8.5
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.8.4/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.5/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

