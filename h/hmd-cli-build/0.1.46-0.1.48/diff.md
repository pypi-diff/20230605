# Comparing `tmp/hmd_cli_build-0.1.46-py3-none-any.whl.zip` & `tmp/hmd_cli_build-0.1.48-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5268 bytes, number of entries: 6
--rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-01 16:55 hmd_cli_build/__init__.py
--rw-rw-rw-  2.0 unx     8418 b- defN 23-Mar-01 16:55 hmd_cli_build/controller.py
--rw-rw-rw-  2.0 unx     4267 b- defN 23-Mar-01 16:56 hmd_cli_build-0.1.46.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Mar-01 16:56 hmd_cli_build-0.1.46.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       14 b- defN 23-Mar-01 16:56 hmd_cli_build-0.1.46.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      489 b- defN 23-Mar-01 16:56 hmd_cli_build-0.1.46.dist-info/RECORD
-6 files, 13280 bytes uncompressed, 4374 bytes compressed:  67.1%
+Zip file size: 5265 bytes, number of entries: 6
+-rw-rw-rw-  2.0 unx        0 b- defN 23-May-18 16:45 hmd_cli_build/__init__.py
+-rw-rw-rw-  2.0 unx     8418 b- defN 23-May-18 16:45 hmd_cli_build/controller.py
+-rw-rw-rw-  2.0 unx     4268 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       14 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      489 b- defN 23-May-18 16:45 hmd_cli_build-0.1.48.dist-info/RECORD
+6 files, 13281 bytes uncompressed, 4371 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: hmd_cli_build/__init__.py
 Comment: 
 
 Filename: hmd_cli_build/controller.py
 Comment: 
 
-Filename: hmd_cli_build-0.1.46.dist-info/METADATA
+Filename: hmd_cli_build-0.1.48.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_build-0.1.46.dist-info/WHEEL
+Filename: hmd_cli_build-0.1.48.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_build-0.1.46.dist-info/top_level.txt
+Filename: hmd_cli_build-0.1.48.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_build-0.1.46.dist-info/RECORD
+Filename: hmd_cli_build-0.1.48.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hmd_cli_build-0.1.46.dist-info/METADATA` & `hmd_cli_build-0.1.48.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-build
-Version: 0.1.46
+Version: 0.1.48
 Summary: Generic build tool.
 Home-page: UNKNOWN
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -28,19 +28,19 @@
 Requires-Dist: decorator (==5.1.1)
 Requires-Dist: ecdsa (==0.17.0)
 Requires-Dist: frozenlist (==1.3.0)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: greenlet (==1.1.2)
 Requires-Dist: gremlinpython (==3.5.2)
 Requires-Dist: hmd-cli-app (~=1.1.595)
-Requires-Dist: hmd-cli-tools (~=1.1.227)
-Requires-Dist: hmd-entity-storage (~=0.1.216)
-Requires-Dist: hmd-graphql-client (~=0.1.98)
-Requires-Dist: hmd-lib-auth (~=0.1.67)
-Requires-Dist: hmd-lib-librarian-client (~=0.1.49)
+Requires-Dist: hmd-cli-tools (~=1.1.228)
+Requires-Dist: hmd-entity-storage (~=0.1.224)
+Requires-Dist: hmd-graphql-client (~=0.1.105)
+Requires-Dist: hmd-lib-auth (~=0.1.75)
+Requires-Dist: hmd-lib-librarian-client (~=0.1.53)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.35)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
```

