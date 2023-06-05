# Comparing `tmp/flageval_serving-0.1.2.tar.gz` & `tmp/flageval_serving-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flageval_serving-0.1.2.tar", max compression
+gzip compressed data, was "flageval_serving-0.1.3.tar", max compression
```

## Comparing `flageval_serving-0.1.2.tar` & `flageval_serving-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1289 2023-05-29 08:11:29.020506 flageval_serving-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.2/flageval/serving/__init__.py
--rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.2/flageval/serving/app.py
--rw-r--r--   0        0        0     3903 2023-06-05 00:31:36.366312 flageval_serving-0.1.2/flageval/serving/cli.py
--rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.2/flageval/serving/extensions.py
--rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.2/flageval/serving/finder.py
--rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.2/flageval/serving/flagenv.py
--rw-r--r--   0        0        0     4224 2023-05-30 07:00:42.215950 flageval_serving-0.1.2/flageval/serving/flageval.py
--rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.2/flageval/serving/guniconf.py
--rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.2/flageval/serving/service/__init__.py
--rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.2/flageval/serving/service/base.py
--rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.2/flageval/serving/service/demo_service.py
--rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.2/flageval/serving/service/guniconf.py
--rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.2/flageval/serving/service/nlp.py
--rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.2/flageval/serving/service/settings.py
--rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.2/flageval/serving/service/views.py
--rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.2/flageval/serving/signals.py
--rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.2/flageval/serving/util.py
--rw-r--r--   0        0        0      567 2023-06-05 00:32:38.531019 flageval_serving-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 flageval_serving-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1289 2023-05-29 08:11:29.020506 flageval_serving-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.3/flageval/serving/__init__.py
+-rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.3/flageval/serving/app.py
+-rw-r--r--   0        0        0     3903 2023-06-05 00:31:36.366312 flageval_serving-0.1.3/flageval/serving/cli.py
+-rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.3/flageval/serving/extensions.py
+-rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.3/flageval/serving/finder.py
+-rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.3/flageval/serving/flagenv.py
+-rw-r--r--   0        0        0     4710 2023-06-05 06:43:26.434926 flageval_serving-0.1.3/flageval/serving/flageval.py
+-rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.3/flageval/serving/guniconf.py
+-rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.3/flageval/serving/service/__init__.py
+-rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.3/flageval/serving/service/base.py
+-rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.3/flageval/serving/service/demo_service.py
+-rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.3/flageval/serving/service/guniconf.py
+-rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.3/flageval/serving/service/nlp.py
+-rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.3/flageval/serving/service/settings.py
+-rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.3/flageval/serving/service/views.py
+-rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.3/flageval/serving/signals.py
+-rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.3/flageval/serving/util.py
+-rw-r--r--   0        0        0      567 2023-06-05 06:46:25.845592 flageval_serving-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 flageval_serving-0.1.3/PKG-INFO
```

### Comparing `flageval_serving-0.1.2/README.md` & `flageval_serving-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/app.py` & `flageval_serving-0.1.3/flageval/serving/app.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/cli.py` & `flageval_serving-0.1.3/flageval/serving/cli.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/finder.py` & `flageval_serving-0.1.3/flageval/serving/finder.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/flagenv.py` & `flageval_serving-0.1.3/flageval/serving/flagenv.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/flageval.py` & `flageval_serving-0.1.3/flageval/serving/flageval.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,17 +43,23 @@
     def upload(self):
         local_files = self._list_local_files()
         remote_files = self._list_remote_files()
         if len(remote_files) == 0:
             self._create_remote_files(local_files)
             remote_files = self._list_remote_files()
 
-        for item in tqdm.tqdm(remote_files):
-            if not item.ks3_ready:
-                self._do_upload(item)
+        total_kb = sum(x.size_kb for x in remote_files)
+        progbar = tqdm.tqdm(total=total_kb, unit="KB")
+
+        for item in remote_files:
+            if item.ks3_ready:
+                progbar.update(item.size_kb)
+                continue
+            self._do_upload(item, progbar)
+        progbar.close()
 
     def _list_local_files(self) -> List[File]:
         results: List[File] = []
         for root, dirs, files in os.walk(
                 self.path, followlinks=self.options.get('followlinks', False),
         ):
             for name in files:
@@ -99,26 +105,30 @@
                 for item in local_files
             ]
         })
         if resp.status_code >= 400:
             raise FlagEvalError(resp.status_code, resp.text)
         return resp.json()
 
-    def _do_upload(self, item: File):
+    def _do_upload(self, item: File, progbar: tqdm.tqdm):
         url = f'{self.host}{self.CHUNKS_PATH.format(item.id_)}'
+        innerbar = tqdm.tqdm(total=item.size_kb, unit='KB', desc=item.filename)
+
         with open(item.path,'rb') as f:
-            for i, chunk in tqdm.tqdm(enumerate(item.chunks), desc=item.filename):
+            for i, chunk in enumerate(item.chunks):
                 buf = io.BytesIO()
                 if i + 1 < len(item.chunks):
                     content = f.read(chunk.size_kb * 1024)
                 else:
                     content = f.read()
                 buf.write(content)
                 buf.seek(0)
                 if chunk.ks3_ready:
+                    progbar.update(chunk.size_kb)
+                    innerbar.update(chunk.size_kb)
                     continue
 
                 files = {'file': buf}
                 values = {
                     'chunk_num': chunk.num,
                     'token': self.token,
                 }
@@ -129,7 +139,11 @@
                     },
                 )
                 if resp.status_code >= 400:
                     raise FlagEvalError(resp.status_code, resp.text)
                 r = resp.json()
                 if r['status'] != 200:
                     raise FlagEvalError(r)
+
+                progbar.update(chunk.size_kb)
+                innerbar.update(chunk.size_kb)
+        innerbar.close()
```

### Comparing `flageval_serving-0.1.2/flageval/serving/guniconf.py` & `flageval_serving-0.1.3/flageval/serving/guniconf.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/service/base.py` & `flageval_serving-0.1.3/flageval/serving/service/base.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/service/demo_service.py` & `flageval_serving-0.1.3/flageval/serving/service/demo_service.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/service/nlp.py` & `flageval_serving-0.1.3/flageval/serving/service/nlp.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/signals.py` & `flageval_serving-0.1.3/flageval/serving/signals.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/flageval/serving/util.py` & `flageval_serving-0.1.3/flageval/serving/util.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.2/pyproject.toml` & `flageval_serving-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flageval-serving"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["FlagEval <flageval@baai.ac.cn>"]
 readme = "README.md"
 packages = [{ include = "flageval" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `flageval_serving-0.1.2/PKG-INFO` & `flageval_serving-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flageval-serving
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: FlagEval
 Author-email: flageval@baai.ac.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

