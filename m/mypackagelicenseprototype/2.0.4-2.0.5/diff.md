# Comparing `tmp/mypackagelicenseprototype-2.0.4-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-2.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2955 bytes, number of entries: 7
+Zip file size: 2954 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      140 b- defN 23-Jun-05 11:33 mypackagelicenseprototype/PackageContent.py
--rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-05 11:34 mypackagelicenseprototype/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      666 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/RECORD
-7 files, 2927 bytes uncompressed, 1743 bytes compressed:  40.5%
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Jun-05 11:57 mypackagelicenseprototype/__init__.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      666 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/RECORD
+7 files, 2928 bytes uncompressed, 1742 bytes compressed:  40.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mypackagelicenseprototype/PackageContent.py
 Comment: 
 
 Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.4.dist-info/LICENSE
+Filename: mypackagelicenseprototype-2.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.4.dist-info/METADATA
+Filename: mypackagelicenseprototype-2.0.5.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.4.dist-info/WHEEL
+Filename: mypackagelicenseprototype-2.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.4.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-2.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.4.dist-info/RECORD
+Filename: mypackagelicenseprototype-2.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mypackagelicenseprototype/__init__.py

```diff
@@ -1 +1 @@
-from .PackageContent import *
+#from .PackageContent import *
```

## Comparing `mypackagelicenseprototype-2.0.4.dist-info/LICENSE` & `mypackagelicenseprototype-2.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-2.0.4.dist-info/METADATA` & `mypackagelicenseprototype-2.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 2.0.4
+Version: 2.0.5
 Summary: Description of your package
 Author-email: Daniel Roth <daniel-roth@posteo.org>
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

