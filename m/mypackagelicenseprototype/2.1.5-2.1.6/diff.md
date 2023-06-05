# Comparing `tmp/mypackagelicenseprototype-2.1.5-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-2.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 224292 bytes, number of entries: 8
+Zip file size: 224281 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     2646 b- defN 23-Jun-05 15:29 parent/PackageContent.py
 -rw-rw-rw-  2.0 fat     1399 b- defN 23-Jun-05 15:29 parent/__init__.py
 -rw-rw-rw-  2.0 fat      103 b- defN 23-Jun-05 15:51 parent/pyarmor_runtime_000000/__init__.py
 -rw-rw-rw-  2.0 fat   616960 b- defN 23-Jun-05 15:29 parent/pyarmor_runtime_000000/pyarmor_runtime.pyd
--rw-rw-rw-  2.0 fat     1479 b- defN 23-Jun-05 16:19 mypackagelicenseprototype-2.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 16:19 mypackagelicenseprototype-2.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-05 16:19 mypackagelicenseprototype-2.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      730 b- defN 23-Jun-05 16:19 mypackagelicenseprototype-2.1.5.dist-info/RECORD
-8 files, 623416 bytes uncompressed, 222998 bytes compressed:  64.2%
+-rw-rw-rw-  2.0 fat     1447 b- defN 23-Jun-05 16:23 mypackagelicenseprototype-2.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 16:23 mypackagelicenseprototype-2.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-05 16:23 mypackagelicenseprototype-2.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      730 b- defN 23-Jun-05 16:23 mypackagelicenseprototype-2.1.6.dist-info/RECORD
+8 files, 623384 bytes uncompressed, 222987 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: parent/pyarmor_runtime_000000/__init__.py
 Comment: 
 
 Filename: parent/pyarmor_runtime_000000/pyarmor_runtime.pyd
 Comment: 
 
-Filename: mypackagelicenseprototype-2.1.5.dist-info/METADATA
+Filename: mypackagelicenseprototype-2.1.6.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-2.1.5.dist-info/WHEEL
+Filename: mypackagelicenseprototype-2.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-2.1.5.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-2.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mypackagelicenseprototype-2.1.5.dist-info/RECORD
+Filename: mypackagelicenseprototype-2.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mypackagelicenseprototype-2.1.5.dist-info/METADATA` & `mypackagelicenseprototype-2.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 2.1.5
+Version: 2.1.6
 Requires-Dist: asttokens (==2.2.1)
 Requires-Dist: backcall (==0.2.0)
 Requires-Dist: build (==0.10.0)
 Requires-Dist: chardet (==5.1.0)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: comm (==0.1.3)
 Requires-Dist: Cython (==0.29.35)
@@ -28,15 +28,14 @@
 Requires-Dist: pure-eval (==0.2.2)
 Requires-Dist: pyarmor (==8.2.3)
 Requires-Dist: pyarmor.cli.core (==3.2.3)
 Requires-Dist: Pygments (==2.15.1)
 Requires-Dist: PyObfuscator (==0.1.1)
 Requires-Dist: pyproject-hooks (==1.0.0)
 Requires-Dist: python-dateutil (==2.8.2)
-Requires-Dist: pywin32 (==306)
 Requires-Dist: pyzmq (==25.1.0)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: stack-data (==0.6.2)
 Requires-Dist: tomli (==2.0.1)
 Requires-Dist: tornado (==6.3.2)
 Requires-Dist: traitlets (==5.9.0)
 Requires-Dist: wcwidth (==0.2.6)
```

## Comparing `mypackagelicenseprototype-2.1.5.dist-info/RECORD` & `mypackagelicenseprototype-2.1.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 parent/PackageContent.py,sha256=GkkmUxGR-4zeJac3GJmxvbLO-_tZRZg43O5wC86yhVQ,2646
 parent/__init__.py,sha256=IpTWFNUS3RHiykD6RwvN-prZ6baB27URaPwB7TiRrDw,1399
 parent/pyarmor_runtime_000000/__init__.py,sha256=h2zqGLQnd7mBEsxAyhX5UAmzfUNJqaxmuT0v8Qg1UsE,103
 parent/pyarmor_runtime_000000/pyarmor_runtime.pyd,sha256=IpCSrnG_vYRRcoSy7XZ8pswDv6hCtmECzA-wxPZCNJg,616960
-mypackagelicenseprototype-2.1.5.dist-info/METADATA,sha256=_D4kVV_4T9I61Ttdps_j0AuwikEVzAsgQ8foQLc6PMQ,1479
-mypackagelicenseprototype-2.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mypackagelicenseprototype-2.1.5.dist-info/top_level.txt,sha256=tPoeaFWZPj-ZvQeGrOjywqPqpZuLErDQBKS1aWQFTZo,7
-mypackagelicenseprototype-2.1.5.dist-info/RECORD,,
+mypackagelicenseprototype-2.1.6.dist-info/METADATA,sha256=zwbCdK1GCyxmwipF3zQaXXgk4BTWTat_nN-LToRMhBY,1447
+mypackagelicenseprototype-2.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mypackagelicenseprototype-2.1.6.dist-info/top_level.txt,sha256=tPoeaFWZPj-ZvQeGrOjywqPqpZuLErDQBKS1aWQFTZo,7
+mypackagelicenseprototype-2.1.6.dist-info/RECORD,,
```

