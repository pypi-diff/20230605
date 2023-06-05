# Comparing `tmp/hmd_cli_python-0.2.74-py3-none-any.whl.zip` & `tmp/hmd_cli_python-0.2.75-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6063 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-01 18:24 hmd_cli_python/__init__.py
--rw-rw-rw-  2.0 unx     3624 b- defN 23-Mar-01 18:24 hmd_cli_python/controller.py
--rw-rw-rw-  2.0 unx     9749 b- defN 23-Mar-01 18:24 hmd_cli_python/hmd_cli_python.py
--rw-rw-rw-  2.0 unx     2496 b- defN 23-Mar-01 18:25 hmd_cli_python-0.2.74.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Mar-01 18:25 hmd_cli_python-0.2.74.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 23-Mar-01 18:25 hmd_cli_python-0.2.74.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      584 b- defN 23-Mar-01 18:25 hmd_cli_python-0.2.74.dist-info/RECORD
-7 files, 16560 bytes uncompressed, 5017 bytes compressed:  69.7%
+Zip file size: 6082 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-May-18 15:53 hmd_cli_python/__init__.py
+-rw-rw-rw-  2.0 unx     3624 b- defN 23-May-18 15:53 hmd_cli_python/controller.py
+-rw-rw-rw-  2.0 unx     9749 b- defN 23-May-18 15:53 hmd_cli_python/hmd_cli_python.py
+-rw-rw-rw-  2.0 unx     2534 b- defN 23-May-18 15:54 hmd_cli_python-0.2.75.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-18 15:54 hmd_cli_python-0.2.75.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 23-May-18 15:54 hmd_cli_python-0.2.75.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      584 b- defN 23-May-18 15:54 hmd_cli_python-0.2.75.dist-info/RECORD
+7 files, 16598 bytes uncompressed, 5036 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_python/controller.py
 Comment: 
 
 Filename: hmd_cli_python/hmd_cli_python.py
 Comment: 
 
-Filename: hmd_cli_python-0.2.74.dist-info/METADATA
+Filename: hmd_cli_python-0.2.75.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_python-0.2.74.dist-info/WHEEL
+Filename: hmd_cli_python-0.2.75.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_python-0.2.74.dist-info/top_level.txt
+Filename: hmd_cli_python-0.2.75.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_python-0.2.74.dist-info/RECORD
+Filename: hmd_cli_python-0.2.75.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hmd_cli_python-0.2.74.dist-info/METADATA` & `hmd_cli_python-0.2.75.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-python
-Version: 0.2.74
+Version: 0.2.75
 Summary: Implementation for python cli command
 Home-page: UNKNOWN
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: attrs (==21.4.0)
@@ -13,32 +13,33 @@
 Requires-Dist: boto3 (==1.21.7)
 Requires-Dist: botocore (==1.24.9)
 Requires-Dist: cachetools (==5.2.0)
 Requires-Dist: cement (==3.0.6)
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: cffi (==1.15.0)
 Requires-Dist: charset-normalizer (==2.0.12)
-Requires-Dist: colorama (==0.4.4)
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: coverage[toml] (==6.3.2)
 Requires-Dist: cryptography (==39.0.1)
 Requires-Dist: docutils (==0.18.1)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: hmd-cli-app (~=1.1.595)
-Requires-Dist: hmd-cli-tools (~=1.1.227)
+Requires-Dist: hmd-cli-tools (~=1.1.228)
 Requires-Dist: idna (==3.3)
 Requires-Dist: importlib-metadata (==4.11.2)
 Requires-Dist: iniconfig (==1.1.1)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: jeepney (==0.8.0)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: keyring (==23.5.0)
 Requires-Dist: kubernetes (==24.2.0)
+Requires-Dist: markdown-it-py (==2.2.0)
 Requires-Dist: markupsafe (==2.1.0)
+Requires-Dist: mdurl (==0.1.2)
 Requires-Dist: oauthlib (==3.2.2)
 Requires-Dist: packaging (==21.3)
 Requires-Dist: pfzy (==0.3.4)
 Requires-Dist: pkginfo (==1.8.2)
 Requires-Dist: pluggy (==1.0.0)
 Requires-Dist: prompt-toolkit (==3.0.38)
 Requires-Dist: py (==1.11.0)
@@ -49,28 +50,28 @@
 Requires-Dist: pyopenssl (==23.0.0)
 Requires-Dist: pyparsing (==3.0.7)
 Requires-Dist: pytest (==7.0.1)
 Requires-Dist: pytest-cov (==3.0.0)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: python-dotenv (==0.19.2)
 Requires-Dist: pyyaml (==6.0)
-Requires-Dist: readme-renderer (==32.0)
+Requires-Dist: readme-renderer (==37.3)
 Requires-Dist: requests (==2.28.2)
 Requires-Dist: requests-oauthlib (==1.3.1)
 Requires-Dist: requests-toolbelt (==0.9.1)
 Requires-Dist: rfc3986 (==2.0.0)
+Requires-Dist: rich (==13.3.5)
 Requires-Dist: rsa (==4.8)
 Requires-Dist: s3transfer (==0.5.2)
 Requires-Dist: secretstorage (==3.3.3)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: tomli (==2.0.1)
-Requires-Dist: tqdm (==4.63.0)
-Requires-Dist: twine (==3.8.0)
+Requires-Dist: twine (==4.0.2)
 Requires-Dist: urllib3 (==1.26.8)
 Requires-Dist: wcwidth (==0.2.6)
 Requires-Dist: webencodings (==0.5.1)
 Requires-Dist: websocket-client (==1.3.3)
 Requires-Dist: wheel (==0.38.0)
-Requires-Dist: zipp (==3.7.0)
+Requires-Dist: zipp (==3.15.0)
 
 UNKNOWN
```

## Comparing `hmd_cli_python-0.2.74.dist-info/RECORD` & `hmd_cli_python-0.2.75.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 hmd_cli_python/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hmd_cli_python/controller.py,sha256=VHaY1zMnTssbznWWkOWsq2PTZpovd4krDgwH_l3HJGI,3624
 hmd_cli_python/hmd_cli_python.py,sha256=AmgT4OBX2qAnEAJ-Zgz7NQbV0bB0oZp646l7mgUTxw0,9749
-hmd_cli_python-0.2.74.dist-info/METADATA,sha256=7X4utCWueIK6rPXO4SoP174ZOIv2f4YzFSu5L4T6GPs,2496
-hmd_cli_python-0.2.74.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_cli_python-0.2.74.dist-info/top_level.txt,sha256=i2ZCGVJeOkzYWeWmczts0Y8Yv2QsTWcueX0_qWGbs7M,15
-hmd_cli_python-0.2.74.dist-info/RECORD,,
+hmd_cli_python-0.2.75.dist-info/METADATA,sha256=Dobhrp_2dWzPjAAV7aBzyw3xANMlflOkWSuZNOkjELY,2534
+hmd_cli_python-0.2.75.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_cli_python-0.2.75.dist-info/top_level.txt,sha256=i2ZCGVJeOkzYWeWmczts0Y8Yv2QsTWcueX0_qWGbs7M,15
+hmd_cli_python-0.2.75.dist-info/RECORD,,
```

