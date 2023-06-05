# Comparing `tmp/mypackagelicenseprototype-2.0.3-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3010 bytes, number of entries: 7
+Zip file size: 2955 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      140 b- defN 23-Jun-05 11:33 mypackagelicenseprototype/PackageContent.py
 -rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-05 11:34 mypackagelicenseprototype/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 11:49 mypackagelicenseprototype-2.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1017 b- defN 23-Jun-05 11:49 mypackagelicenseprototype-2.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 11:49 mypackagelicenseprototype-2.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 11:49 mypackagelicenseprototype-2.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      667 b- defN 23-Jun-05 11:49 mypackagelicenseprototype-2.0.3.dist-info/RECORD
-7 files, 3058 bytes uncompressed, 1798 bytes compressed:  41.2%
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      666 b- defN 23-Jun-05 11:52 mypackagelicenseprototype-2.0.4.dist-info/RECORD
+7 files, 2927 bytes uncompressed, 1743 bytes compressed:  40.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mypackagelicenseprototype/PackageContent.py
 Comment: 
 
 Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.3.dist-info/LICENSE
+Filename: mypackagelicenseprototype-2.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.3.dist-info/METADATA
+Filename: mypackagelicenseprototype-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.3.dist-info/WHEEL
+Filename: mypackagelicenseprototype-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.3.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.3.dist-info/RECORD
+Filename: mypackagelicenseprototype-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mypackagelicenseprototype-2.0.3.dist-info/LICENSE` & `mypackagelicenseprototype-2.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-2.0.3.dist-info/METADATA` & `mypackagelicenseprototype-2.0.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 2.0.3
+Version: 2.0.4
 Summary: Description of your package
-Home-page: https://github.com/da-roth/PackageLicensePrototype
-Author: Daniel Roth
 Author-email: Daniel Roth <daniel-roth@posteo.org>
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
 
 # PackageLicensePrototype
 
 # Activate virtual environment
 .venv\Scripts\activate.bat
```

## Comparing `mypackagelicenseprototype-2.0.3.dist-info/RECORD` & `mypackagelicenseprototype-2.0.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 mypackagelicenseprototype/PackageContent.py,sha256=r1QR71SzTg8UPbwveQJ80Sfj1uu-iFmEt9-azQPyw5o,140
 mypackagelicenseprototype/__init__.py,sha256=p-MTtFmMR8liEgb9nTGc3uKplgcHi82XjOC_NBxZMrY,31
-mypackagelicenseprototype-2.0.3.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
-mypackagelicenseprototype-2.0.3.dist-info/METADATA,sha256=0-sRus6Boxy_jgvG9DgT6_LKLbUkyYMguZxEHx6YmJY,1017
-mypackagelicenseprototype-2.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mypackagelicenseprototype-2.0.3.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
-mypackagelicenseprototype-2.0.3.dist-info/RECORD,,
+mypackagelicenseprototype-2.0.4.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
+mypackagelicenseprototype-2.0.4.dist-info/METADATA,sha256=aJCVruQ6kbJQ4vbck6VEgwSRlJPJ27iWoeWMPX1PUCs,887
+mypackagelicenseprototype-2.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mypackagelicenseprototype-2.0.4.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
+mypackagelicenseprototype-2.0.4.dist-info/RECORD,,
```

