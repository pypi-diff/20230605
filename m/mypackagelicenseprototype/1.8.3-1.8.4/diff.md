# Comparing `tmp/mypackagelicenseprototype-1.8.3-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-1.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 223772 bytes, number of entries: 8
+Zip file size: 223766 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     2523 b- defN 23-Jun-05 10:16 mypackagelicenseprototype/PackageContent.py
--rw-rw-rw-  2.0 fat      190 b- defN 23-Jun-05 10:18 mypackagelicenseprototype/__init__.py
+-rw-rw-rw-  2.0 fat      180 b- defN 23-Jun-05 10:40 mypackagelicenseprototype/__init__.py
 -rw-rw-rw-  2.0 fat   615936 b- defN 23-Jun-05 10:12 mypackagelicenseprototype/pyarmor_runtime.pyd
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 10:39 mypackagelicenseprototype-1.8.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 10:39 mypackagelicenseprototype-1.8.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:39 mypackagelicenseprototype-1.8.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 10:39 mypackagelicenseprototype-1.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      772 b- defN 23-Jun-05 10:39 mypackagelicenseprototype-1.8.3.dist-info/RECORD
-8 files, 621137 bytes uncompressed, 222394 bytes compressed:  64.2%
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      772 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/RECORD
+8 files, 621127 bytes uncompressed, 222388 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
 Filename: mypackagelicenseprototype/pyarmor_runtime.pyd
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.3.dist-info/LICENSE
+Filename: mypackagelicenseprototype-1.8.4.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.3.dist-info/METADATA
+Filename: mypackagelicenseprototype-1.8.4.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.3.dist-info/WHEEL
+Filename: mypackagelicenseprototype-1.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.3.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-1.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.3.dist-info/RECORD
+Filename: mypackagelicenseprototype-1.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mypackagelicenseprototype/__init__.py

```diff
@@ -1,6 +1,6 @@
 # Pyarmor 8.2.3 (trial), 000000, 2023-06-05T12:12:33.594183
-from mypackagelicenseprototype.pyarmor_runtime import __pyarmor__
+from mypackagelicenseprototype.pyarmor_runtime import *
 
 from mypackagelicenseprototype.PackageContent import *
```

## Comparing `mypackagelicenseprototype-1.8.3.dist-info/LICENSE` & `mypackagelicenseprototype-1.8.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-1.8.3.dist-info/METADATA` & `mypackagelicenseprototype-1.8.4.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 1.8.3
+Version: 1.8.4
 Summary: Description of your package
 Home-page: https://github.com/da-roth/PackageLicensePrototype
 Author: Daniel Roth
 Author-email: daniel-roth@posteo.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

