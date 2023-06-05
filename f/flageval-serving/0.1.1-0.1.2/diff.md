# Comparing `tmp/flageval_serving-0.1.1.tar.gz` & `tmp/flageval_serving-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flageval_serving-0.1.1.tar", max compression
+gzip compressed data, was "flageval_serving-0.1.2.tar", max compression
```

## Comparing `flageval_serving-0.1.1.tar` & `flageval_serving-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1289 2023-05-29 08:11:29.020506 flageval_serving-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.1/flageval/serving/__init__.py
--rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.1/flageval/serving/app.py
--rw-r--r--   0        0        0     3902 2023-05-29 07:09:29.693749 flageval_serving-0.1.1/flageval/serving/cli.py
--rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.1/flageval/serving/extensions.py
--rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.1/flageval/serving/finder.py
--rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.1/flageval/serving/flagenv.py
--rw-r--r--   0        0        0     4224 2023-05-30 07:00:42.215950 flageval_serving-0.1.1/flageval/serving/flageval.py
--rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.1/flageval/serving/guniconf.py
--rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.1/flageval/serving/service/__init__.py
--rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.1/flageval/serving/service/base.py
--rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.1/flageval/serving/service/demo_service.py
--rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.1/flageval/serving/service/guniconf.py
--rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.1/flageval/serving/service/nlp.py
--rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.1/flageval/serving/service/settings.py
--rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.1/flageval/serving/service/views.py
--rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.1/flageval/serving/signals.py
--rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.1/flageval/serving/util.py
--rw-r--r--   0        0        0      567 2023-05-30 07:01:04.642331 flageval_serving-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 flageval_serving-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1289 2023-05-29 08:11:29.020506 flageval_serving-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.2/flageval/serving/__init__.py
+-rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.2/flageval/serving/app.py
+-rw-r--r--   0        0        0     3903 2023-06-05 00:31:36.366312 flageval_serving-0.1.2/flageval/serving/cli.py
+-rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.2/flageval/serving/extensions.py
+-rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.2/flageval/serving/finder.py
+-rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.2/flageval/serving/flagenv.py
+-rw-r--r--   0        0        0     4224 2023-05-30 07:00:42.215950 flageval_serving-0.1.2/flageval/serving/flageval.py
+-rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.2/flageval/serving/guniconf.py
+-rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.2/flageval/serving/service/__init__.py
+-rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.2/flageval/serving/service/base.py
+-rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.2/flageval/serving/service/demo_service.py
+-rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.2/flageval/serving/service/guniconf.py
+-rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.2/flageval/serving/service/nlp.py
+-rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.2/flageval/serving/service/settings.py
+-rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.2/flageval/serving/service/views.py
+-rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.2/flageval/serving/signals.py
+-rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.2/flageval/serving/util.py
+-rw-r--r--   0        0        0      567 2023-06-05 00:32:38.531019 flageval_serving-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 flageval_serving-0.1.2/PKG-INFO
```

### Comparing `flageval_serving-0.1.1/README.md` & `flageval_serving-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/app.py` & `flageval_serving-0.1.2/flageval/serving/app.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/cli.py` & `flageval_serving-0.1.2/flageval/serving/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     sys.argv.append("--config=python:flageval.serving.service.guniconf")
     from gunicorn.app.wsgiapp import WSGIApplication
 
     WSGIApplication("%(prog)s OPTIONS").run()
 
 
 @cli.command()
-@click.option("--host", default="http://120.92.108.238:8080/", help="FlagEval host.")
+@click.option("--host", default="https://flageval.baai.ac.cn/", help="FlagEval host.")
 @click.option("--token", required=True, help="Token to upload model.")
 @click.option("--followlinks", default=False, help="Follow links.")
 @click.argument("model_path", required=True)
 def upload(host, token, followlinks, model_path):
     "Upload model for evaluating."
     from .flageval import FlagEvalUploader
```

### Comparing `flageval_serving-0.1.1/flageval/serving/finder.py` & `flageval_serving-0.1.2/flageval/serving/finder.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/flagenv.py` & `flageval_serving-0.1.2/flageval/serving/flagenv.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/flageval.py` & `flageval_serving-0.1.2/flageval/serving/flageval.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/guniconf.py` & `flageval_serving-0.1.2/flageval/serving/guniconf.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/service/base.py` & `flageval_serving-0.1.2/flageval/serving/service/base.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/service/demo_service.py` & `flageval_serving-0.1.2/flageval/serving/service/demo_service.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/service/nlp.py` & `flageval_serving-0.1.2/flageval/serving/service/nlp.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/signals.py` & `flageval_serving-0.1.2/flageval/serving/signals.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/flageval/serving/util.py` & `flageval_serving-0.1.2/flageval/serving/util.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.1/pyproject.toml` & `flageval_serving-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flageval-serving"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["FlagEval <flageval@baai.ac.cn>"]
 readme = "README.md"
 packages = [{ include = "flageval" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `flageval_serving-0.1.1/PKG-INFO` & `flageval_serving-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flageval-serving
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: FlagEval
 Author-email: flageval@baai.ac.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

