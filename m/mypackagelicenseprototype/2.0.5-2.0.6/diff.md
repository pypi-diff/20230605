# Comparing `tmp/mypackagelicenseprototype-2.0.5-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-2.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 2954 bytes, number of entries: 7
+Zip file size: 3536 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      140 b- defN 23-Jun-05 11:33 mypackagelicenseprototype/PackageContent.py
--rw-rw-rw-  2.0 fat       32 b- defN 23-Jun-05 11:57 mypackagelicenseprototype/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      666 b- defN 23-Jun-05 12:00 mypackagelicenseprototype-2.0.5.dist-info/RECORD
-7 files, 2928 bytes uncompressed, 1742 bytes compressed:  40.5%
+-rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-05 12:06 mypackagelicenseprototype/__init__.py
+-rw-rw-rw-  2.0 fat      124 b- defN 23-Jun-05 12:06 mypackagelicenseprototype/submodule/SubmoduleContent.py
+-rw-rw-rw-  2.0 fat       33 b- defN 23-Jun-05 12:06 mypackagelicenseprototype/submodule/__init__.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      879 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/RECORD
+9 files, 3297 bytes uncompressed, 1968 bytes compressed:  40.3%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: mypackagelicenseprototype/PackageContent.py
 Comment: 
 
 Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.5.dist-info/LICENSE
+Filename: mypackagelicenseprototype/submodule/SubmoduleContent.py
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.5.dist-info/METADATA
+Filename: mypackagelicenseprototype/submodule/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.5.dist-info/WHEEL
+Filename: mypackagelicenseprototype-2.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.5.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-2.0.6.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.5.dist-info/RECORD
+Filename: mypackagelicenseprototype-2.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: mypackagelicenseprototype-2.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: mypackagelicenseprototype-2.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mypackagelicenseprototype/__init__.py

```diff
@@ -1 +1 @@
-#from .PackageContent import *
+from .PackageContent import *
```

## Comparing `mypackagelicenseprototype-2.0.5.dist-info/LICENSE` & `mypackagelicenseprototype-2.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-2.0.5.dist-info/METADATA` & `mypackagelicenseprototype-2.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 2.0.5
+Version: 2.0.6
 Summary: Description of your package
 Author-email: Daniel Roth <daniel-roth@posteo.org>
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `mypackagelicenseprototype-2.0.5.dist-info/RECORD` & `mypackagelicenseprototype-2.0.6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 mypackagelicenseprototype/PackageContent.py,sha256=r1QR71SzTg8UPbwveQJ80Sfj1uu-iFmEt9-azQPyw5o,140
-mypackagelicenseprototype/__init__.py,sha256=iMqIIT_lt8TxKCsngt4Bigb-dynZrumEHaAWhul3cQA,32
-mypackagelicenseprototype-2.0.5.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
-mypackagelicenseprototype-2.0.5.dist-info/METADATA,sha256=bESI5VfKeUasA0AsmU8wz708n7dJ7CQPsWmatg8ZWzw,887
-mypackagelicenseprototype-2.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mypackagelicenseprototype-2.0.5.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
-mypackagelicenseprototype-2.0.5.dist-info/RECORD,,
+mypackagelicenseprototype/__init__.py,sha256=p-MTtFmMR8liEgb9nTGc3uKplgcHi82XjOC_NBxZMrY,31
+mypackagelicenseprototype/submodule/SubmoduleContent.py,sha256=zjPPT9BTowqyb_p-SYwcLY8GadFjuh8oPfXX80r_pcM,124
+mypackagelicenseprototype/submodule/__init__.py,sha256=R6BGM-6RIVOU45qPMZaENalYgeF9SD1R68NOmOAJ4Cw,33
+mypackagelicenseprototype-2.0.6.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
+mypackagelicenseprototype-2.0.6.dist-info/METADATA,sha256=s2td0dVYonWRd-cXwf8XsakBCzIoqVc7MCZgXgmmOco,887
+mypackagelicenseprototype-2.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mypackagelicenseprototype-2.0.6.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
+mypackagelicenseprototype-2.0.6.dist-info/RECORD,,
```

