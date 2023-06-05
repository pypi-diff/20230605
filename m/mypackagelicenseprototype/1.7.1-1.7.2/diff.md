# Comparing `tmp/mypackagelicenseprototype-1.7.1-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-1.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,10 @@
-Zip file size: 2201 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 09:50 mypackagelicenseprototype-1.7.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 09:50 mypackagelicenseprototype-1.7.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 09:50 mypackagelicenseprototype-1.7.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-05 09:50 mypackagelicenseprototype-1.7.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      474 b- defN 23-Jun-05 09:50 mypackagelicenseprototype-1.7.1.dist-info/RECORD
-5 files, 2165 bytes uncompressed, 1301 bytes compressed:  39.9%
+Zip file size: 4349 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     2512 b- defN 23-Jun-05 09:42 mypackagelicenseprototype/PackageContent.py
+-rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-05 09:52 mypackagelicenseprototype/__init__.py
+-rw-rw-rw-  2.0 fat      103 b- defN 23-Jun-05 09:42 mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 09:52 mypackagelicenseprototype-1.7.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 09:52 mypackagelicenseprototype-1.7.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 09:52 mypackagelicenseprototype-1.7.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 09:52 mypackagelicenseprototype-1.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      783 b- defN 23-Jun-05 09:52 mypackagelicenseprototype-1.7.2.dist-info/RECORD
+8 files, 5172 bytes uncompressed, 2941 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -1,16 +1,25 @@
-Filename: mypackagelicenseprototype-1.7.1.dist-info/LICENSE
+Filename: mypackagelicenseprototype/PackageContent.py
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.1.dist-info/METADATA
+Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.1.dist-info/WHEEL
+Filename: mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.1.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-1.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.1.dist-info/RECORD
+Filename: mypackagelicenseprototype-1.7.2.dist-info/METADATA
+Comment: 
+
+Filename: mypackagelicenseprototype-1.7.2.dist-info/WHEEL
+Comment: 
+
+Filename: mypackagelicenseprototype-1.7.2.dist-info/top_level.txt
+Comment: 
+
+Filename: mypackagelicenseprototype-1.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mypackagelicenseprototype-1.7.1.dist-info/LICENSE` & `mypackagelicenseprototype-1.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-1.7.1.dist-info/METADATA` & `mypackagelicenseprototype-1.7.2.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 1.7.1
+Version: 1.7.2
 Summary: Description of your package
 Home-page: https://github.com/da-roth/PackageLicensePrototype
 Author: Daniel Roth
 Author-email: daniel-roth@posteo.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

