# Comparing `tmp/s3ball-0.1.0.tar.gz` & `tmp/s3ball-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3ball-0.1.0.tar", last modified: Fri Jun  2 09:09:21 2023, max compression
+gzip compressed data, was "s3ball-0.1.1.tar", last modified: Mon Jun  5 12:43:55 2023, max compression
```

## Comparing `s3ball-0.1.0.tar` & `s3ball-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:09:21.296087 s3ball-0.1.0/
--rw-r--r--   0 snglth    (1000) users      (100)      285 2023-06-01 16:04:05.000000 s3ball-0.1.0/.envrc
--rw-r--r--   0 snglth    (1000) users      (100)      125 2023-06-01 16:11:42.000000 s3ball-0.1.0/.flake8
--rw-r--r--   0 snglth    (1000) users      (100)       46 2023-06-01 16:02:58.000000 s3ball-0.1.0/.gitignore
--rw-r--r--   0 snglth    (1000) users      (100)      598 2023-06-01 16:10:49.000000 s3ball-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 snglth    (1000) users      (100)    11357 2023-06-01 16:18:50.000000 s3ball-0.1.0/LICENSE
--rw-r--r--   0 snglth    (1000) users      (100)      742 2023-06-02 09:09:21.296087 s3ball-0.1.0/PKG-INFO
--rw-r--r--   0 snglth    (1000) users      (100)      189 2023-06-02 09:07:47.000000 s3ball-0.1.0/README.rst
--rw-r--r--   0 snglth    (1000) users      (100)      948 2023-06-02 09:09:14.000000 s3ball-0.1.0/pyproject.toml
--rw-r--r--   0 snglth    (1000) users      (100)      403 2023-06-01 14:23:41.000000 s3ball-0.1.0/requirements.txt
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:09:21.294087 s3ball-0.1.0/s3ball/
--rw-r--r--   0 snglth    (1000) users      (100)       18 2023-06-01 14:21:50.000000 s3ball-0.1.0/s3ball/__init__.py
--rw-r--r--   0 snglth    (1000) users      (100)      287 2023-06-01 16:11:01.000000 s3ball-0.1.0/s3ball/cli.py
--rw-r--r--   0 snglth    (1000) users      (100)     1441 2023-06-01 16:39:48.000000 s3ball-0.1.0/s3ball/download.py
--rw-r--r--   0 snglth    (1000) users      (100)      552 2023-06-01 16:11:01.000000 s3ball-0.1.0/s3ball/options.py
--rw-r--r--   0 snglth    (1000) users      (100)     1012 2023-06-01 16:11:16.000000 s3ball-0.1.0/s3ball/upload.py
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:09:21.296087 s3ball-0.1.0/s3ball.egg-info/
--rw-r--r--   0 snglth    (1000) users      (100)      742 2023-06-02 09:09:21.000000 s3ball-0.1.0/s3ball.egg-info/PKG-INFO
--rw-r--r--   0 snglth    (1000) users      (100)      379 2023-06-02 09:09:21.000000 s3ball-0.1.0/s3ball.egg-info/SOURCES.txt
--rw-r--r--   0 snglth    (1000) users      (100)        1 2023-06-02 09:09:21.000000 s3ball-0.1.0/s3ball.egg-info/dependency_links.txt
--rw-r--r--   0 snglth    (1000) users      (100)       43 2023-06-02 09:09:21.000000 s3ball-0.1.0/s3ball.egg-info/entry_points.txt
--rw-r--r--   0 snglth    (1000) users      (100)       21 2023-06-02 09:09:21.000000 s3ball-0.1.0/s3ball.egg-info/requires.txt
--rw-r--r--   0 snglth    (1000) users      (100)       12 2023-06-02 09:09:21.000000 s3ball-0.1.0/s3ball.egg-info/top_level.txt
--rw-r--r--   0 snglth    (1000) users      (100)       38 2023-06-02 09:09:21.296087 s3ball-0.1.0/setup.cfg
--rw-r--r--   0 snglth    (1000) users      (100)       92 2023-06-01 14:22:24.000000 s3ball-0.1.0/shell.nix
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:43:55.138086 s3ball-0.1.1/
+-rw-r--r--   0 snglth    (1000) users      (100)      285 2023-06-01 16:04:05.000000 s3ball-0.1.1/.envrc
+-rw-r--r--   0 snglth    (1000) users      (100)      125 2023-06-01 16:11:42.000000 s3ball-0.1.1/.flake8
+-rw-r--r--   0 snglth    (1000) users      (100)       46 2023-06-01 16:02:58.000000 s3ball-0.1.1/.gitignore
+-rw-r--r--   0 snglth    (1000) users      (100)      598 2023-06-01 16:10:49.000000 s3ball-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 snglth    (1000) users      (100)    11357 2023-06-01 16:18:50.000000 s3ball-0.1.1/LICENSE
+-rw-r--r--   0 snglth    (1000) users      (100)      742 2023-06-05 12:43:55.138086 s3ball-0.1.1/PKG-INFO
+-rw-r--r--   0 snglth    (1000) users      (100)      189 2023-06-02 09:07:47.000000 s3ball-0.1.1/README.rst
+-rw-r--r--   0 snglth    (1000) users      (100)      948 2023-06-02 09:09:14.000000 s3ball-0.1.1/pyproject.toml
+-rw-r--r--   0 snglth    (1000) users      (100)      403 2023-06-01 14:23:41.000000 s3ball-0.1.1/requirements.txt
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:43:55.138086 s3ball-0.1.1/s3ball/
+-rw-r--r--   0 snglth    (1000) users      (100)       18 2023-06-05 12:43:17.000000 s3ball-0.1.1/s3ball/__init__.py
+-rw-r--r--   0 snglth    (1000) users      (100)      287 2023-06-01 16:11:01.000000 s3ball-0.1.1/s3ball/cli.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1382 2023-06-05 12:42:13.000000 s3ball-0.1.1/s3ball/download.py
+-rw-r--r--   0 snglth    (1000) users      (100)      552 2023-06-01 16:11:01.000000 s3ball-0.1.1/s3ball/options.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1012 2023-06-01 16:11:16.000000 s3ball-0.1.1/s3ball/upload.py
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:43:55.138086 s3ball-0.1.1/s3ball.egg-info/
+-rw-r--r--   0 snglth    (1000) users      (100)      742 2023-06-05 12:43:55.000000 s3ball-0.1.1/s3ball.egg-info/PKG-INFO
+-rw-r--r--   0 snglth    (1000) users      (100)      379 2023-06-05 12:43:55.000000 s3ball-0.1.1/s3ball.egg-info/SOURCES.txt
+-rw-r--r--   0 snglth    (1000) users      (100)        1 2023-06-05 12:43:55.000000 s3ball-0.1.1/s3ball.egg-info/dependency_links.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       43 2023-06-05 12:43:55.000000 s3ball-0.1.1/s3ball.egg-info/entry_points.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       21 2023-06-05 12:43:55.000000 s3ball-0.1.1/s3ball.egg-info/requires.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       12 2023-06-05 12:43:55.000000 s3ball-0.1.1/s3ball.egg-info/top_level.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       38 2023-06-05 12:43:55.138086 s3ball-0.1.1/setup.cfg
+-rw-r--r--   0 snglth    (1000) users      (100)       92 2023-06-01 14:22:24.000000 s3ball-0.1.1/shell.nix
```

### Comparing `s3ball-0.1.0/.pre-commit-config.yaml` & `s3ball-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `s3ball-0.1.0/LICENSE` & `s3ball-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s3ball-0.1.0/PKG-INFO` & `s3ball-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3ball
-Version: 0.1.0
+Version: 0.1.1
 Summary: S3 to tarball and vice versa
 Author-email: Illia Shestakov <i.shestakov@abstract-technology.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Abstract-Tech/s3ball
 Project-URL: Bug Tracker, https://github.com/Abstract-Tech/s3ball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `s3ball-0.1.0/pyproject.toml` & `s3ball-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3ball-0.1.0/s3ball/download.py` & `s3ball-0.1.1/s3ball/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-import io
 import sys
 import tarfile
 
 import click
 from minio import Minio
 
 from s3ball.options import (
     access_key_option,
     endpoint_option,
     protocol_option,
     secret_key_option,
 )
 
 
-def _chunked_tar_write(tar, name, stream) -> None:
-    for chunk in stream:
-        tarinfo = tarfile.TarInfo(name=name)
-        tarinfo.size = len(chunk)
-
-        tar.addfile(tarinfo, fileobj=io.BytesIO(chunk))
-
-
 @endpoint_option
 @access_key_option
 @secret_key_option
 @protocol_option
 @click.argument("bucket", nargs=1)
 @click.command(name="download")
 def download(
@@ -42,13 +33,17 @@
         exit(1)
 
     objects = s3_client.list_objects(bucket, recursive=True)
     with tarfile.open(mode="w|", fileobj=sys.stdout.buffer) as tar:
         for obj in objects:
             if not obj.is_dir:
                 obj_key = obj.object_name
+                obj_size = obj.size
+                obj_stream = s3_client.get_object(bucket, obj_key)
+                obj_stream.decode_content = False
                 try:
-                    obj_stream = s3_client.get_object(bucket, obj_key)
-                    _chunked_tar_write(tar, obj_key, obj_stream.stream())
+                    tarinfo = tarfile.TarInfo(name=obj_key)
+                    tarinfo.size = obj_size
+                    tar.addfile(tarinfo, obj_stream)
                 finally:
                     obj_stream.close()
                     obj_stream.release_conn()
```

### Comparing `s3ball-0.1.0/s3ball/options.py` & `s3ball-0.1.1/s3ball/options.py`

 * *Files identical despite different names*

### Comparing `s3ball-0.1.0/s3ball/upload.py` & `s3ball-0.1.1/s3ball/upload.py`

 * *Files identical despite different names*

### Comparing `s3ball-0.1.0/s3ball.egg-info/PKG-INFO` & `s3ball-0.1.1/s3ball.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3ball
-Version: 0.1.0
+Version: 0.1.1
 Summary: S3 to tarball and vice versa
 Author-email: Illia Shestakov <i.shestakov@abstract-technology.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Abstract-Tech/s3ball
 Project-URL: Bug Tracker, https://github.com/Abstract-Tech/s3ball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

