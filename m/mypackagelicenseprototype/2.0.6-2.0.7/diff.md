# Comparing `tmp/mypackagelicenseprototype-2.0.6-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-2.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 3536 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      140 b- defN 23-Jun-05 11:33 mypackagelicenseprototype/PackageContent.py
+Zip file size: 5410 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-05 12:11 mypackagelicenseprototype/PackageContent.py
+-rw-rw-rw-  2.0 fat      140 b- defN 23-Jun-05 11:33 mypackagelicenseprototype/PackageContentOld.py
 -rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-05 12:06 mypackagelicenseprototype/__init__.py
+-rw-rw-rw-  2.0 fat      103 b- defN 23-Jun-05 12:11 mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
 -rw-rw-rw-  2.0 fat      124 b- defN 23-Jun-05 12:06 mypackagelicenseprototype/submodule/SubmoduleContent.py
 -rw-rw-rw-  2.0 fat       33 b- defN 23-Jun-05 12:06 mypackagelicenseprototype/submodule/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      879 b- defN 23-Jun-05 12:07 mypackagelicenseprototype-2.0.6.dist-info/RECORD
-9 files, 3297 bytes uncompressed, 1968 bytes compressed:  40.3%
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 12:13 mypackagelicenseprototype-2.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-05 12:13 mypackagelicenseprototype-2.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 12:13 mypackagelicenseprototype-2.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 12:13 mypackagelicenseprototype-2.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1098 b- defN 23-Jun-05 12:13 mypackagelicenseprototype-2.0.7.dist-info/RECORD
+11 files, 6139 bytes uncompressed, 3478 bytes compressed:  43.3%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: mypackagelicenseprototype/PackageContent.py
 Comment: 
 
+Filename: mypackagelicenseprototype/PackageContentOld.py
+Comment: 
+
 Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
+Filename: mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
+Comment: 
+
 Filename: mypackagelicenseprototype/submodule/SubmoduleContent.py
 Comment: 
 
 Filename: mypackagelicenseprototype/submodule/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.6.dist-info/LICENSE
+Filename: mypackagelicenseprototype-2.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.6.dist-info/METADATA
+Filename: mypackagelicenseprototype-2.0.7.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.6.dist-info/WHEEL
+Filename: mypackagelicenseprototype-2.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.6.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-2.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mypackagelicenseprototype-2.0.6.dist-info/RECORD
+Filename: mypackagelicenseprototype-2.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mypackagelicenseprototype/PackageContent.py

```diff
@@ -1,7 +1,3 @@
-import numpy as np
-
-def add_numbers_2(a, b):
-    """
-    Adds two numbers and returns the result.
-    """
-    return a + 2 *np.sqrt(2)
+# Pyarmor 8.2.3 (trial), 000000, non-profits, 2023-06-05T14:11:29.792462
+from pyarmor_runtime_000000 import __pyarmor__
+__pyarmor__(__name__, __file__, b'PY000000\x00\x03\n\x00o\r\r\n\x80\x00\x01\x00\x08\x00\x00\x00\x04\x00\x00\x00@\x00\x00\x00\xea\x02\x00\x00\x12\t\x04\x00\x84\xfba4\x02\xb3VY\xf9\xfdh-\x83\xd5\x14f\x00\x00\x00\x00\x00\x00\x00\x00e\xa2\xfe\x9a\x1d\xcbK\xa40\x96\xc9P\xabh\x83\x0cS\xdfu[\xff\x8f\x1f+#U\xb1,:\x11%s \xe6}\xa5\xab{\x80\xae\xf9\xa8I\xa0\x8c\x11"u\x9a,\xe0:Rt\x1a#\xc0I\x01\xc8\x9cu\x8a#[4\x92Re|u\xc4\x80{\xeb\xd5\xc8\xd1t\xb4#G\xd6%\xb4\x7f\xd7\xa4\x88\x93\x87\x05\xc0\xf2\x16!\x18\x142)\xb2\x1a\xb4\\\x94\xc5|\xf5i\xfc\x87\x1c\xedz\x8e\x1cN\x01N^\xb8uL\x1ae\x80\x82\xe2\xd3A)(\xa85$*\x94\x08l\xcc\xce\x06\x88\xc4\xf15\xb9A\xac\xd8\xad\x05b\x12\xb0\x8f\x17Y\x08\xda\x13|\xf1}2\x8a\x16"\xb7.\x8d\xf1\x89\xdb\xd97\x1e\xce>\x96\xe1\xc1\xd8fY\xaf\x1f\xc5\x97\x12GI\xe1\xe6\xb4\xb9Hz\xe8\np?Y\x9d\\4Q\xcd\x805\x86\xda(\x13o\x10\xa8\xfe_\xeck\t\x17(\xe5\x80\x01Z\xecH\x03\x1d\xe1\xe2\xc8\x87\xddN\x9f\xc7\x16S6\x0e\xeef\x1d\xf5\x12@\xb6\xc9\\\x06#\xf1\x853\x08\xdb\xb9(\xd8\x18t\xfb\x11\xa7\x03\x08\x9e\x8a\xc4\xba\xbep\x1cc\xca\x13\x8dD/\x1f\xb9\xd4h}\xf7\x18%\xf4\xb7p+\xdfR\xe5X\xa9\xaa\xd4/\xcb\x0c\xf5\xb7\x1f\x1c\xe8,\x0f\\\xda\xef<r\xd2\xf3\xa6,/o\x95\x12\xa5i\\\x9c\xab\x9d8a\x128\xc7aN\x98\xf8tL\x08G\x15$\xe0\x14\xean\x11L\xa9\xee\xbd\xa0\x15\x00\\\x07\x92\xb19\xdf{2\x81F\x97&m\xf1\xbb\xe5h\xb0G\xf0\xef)\x900U\xea\x98J\\0\x85e*\xec\xe5Y\x10\xe5\xc1\x98<5\xaf\x93\x19|v:\xef\xd1`\xb6\xf0l\xad\x973t\x13\t\xebI\xb1e3\xbf{\xd8u\n>\xe8H\x8a\x9d[\xee\x86a\xa7\x13>!\x1f6\xd2\xfft#\xde;\x9e\xdd\xe5\x89E\\\xc3\xcfK\xa9\x15\x05de:-\xf8e\xaf\x0f\xb6\xc8?eU\x1f\xdaB\x8c\xe5\xe8\xf7\x87\xdf\x1a\x1d=\xf2\x9b\xb7\xc8\xcf\xc1\\\x7fM\x82\xc7\xd5\xcef\xdaB\x80\xaej\x93\x1c\x88\nfO^\xc6\x86\x9f;_\x1b\xfd\xa8\xb2j\x01\xa8\xe1\x16\x0cr\\\xbf\xed\x07\n5\xb3\xb7\x8b)\tX4\xeaD\xcf:\xc2\xebTM\xdc,\xbe\x8a\xd5\xbb:K\xf9\xa6\xf4\x9e\xf6\x06h*\xc2\xe2\xf1E\xdc\x0b\x15G\x08g\xd3\xae.\xcb\xe5I\xc6\n\xc7\xb88pG\x0f\xf2\x0f#\xef\xb7\x04\r\x04?3\xde[g\xa3\x05^\xab\xad>\xe7x*#\xf7\xda\x05\xa6=k\x9c\xe2\xc3\x8f@\x17s\xa5O\xf9\xf3\xc9+\xab\xbc\xbc}x\x11\xcf\xad\xbe\xb9\x13<\x81;\xfe\x9e\x81\x821\x9b\xab\xfb\x86\x11\x0c\xcc\xa0\x8e\x0co\x85\xca\xe3\xc6~k\xeb\xac\xfe6\x90\t\x16\x81\x19W\xa7+C\xf3\xfc\xc1\x8c\xa5\xb3\x9f\xc5\x9f\xc9\x9fm\xcd\x84\xc8Q\x14J}\x92I\xd4\xe8\x930\x8a\xb4\xe3\xf2\xb5\xdcJ\x9c\xc0\xda\xf5\x92\xcbp\x0b\\}U\xc9\x18^KA\xc6\x1cS\x97\xe3%\x0b\xdc\xd5\xa0\xd5#gv\x87\x92\xf6.')
```

## Comparing `mypackagelicenseprototype-2.0.6.dist-info/LICENSE` & `mypackagelicenseprototype-2.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-2.0.6.dist-info/METADATA` & `mypackagelicenseprototype-2.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 2.0.6
+Version: 2.0.7
 Summary: Description of your package
 Author-email: Daniel Roth <daniel-roth@posteo.org>
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `mypackagelicenseprototype-2.0.6.dist-info/RECORD` & `mypackagelicenseprototype-2.0.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-mypackagelicenseprototype/PackageContent.py,sha256=r1QR71SzTg8UPbwveQJ80Sfj1uu-iFmEt9-azQPyw5o,140
+mypackagelicenseprototype/PackageContent.py,sha256=3-cUIN1SNYLIGJpPsdCwq7TvVKDmAfqoL4fhRu8emvs,2520
+mypackagelicenseprototype/PackageContentOld.py,sha256=r1QR71SzTg8UPbwveQJ80Sfj1uu-iFmEt9-azQPyw5o,140
 mypackagelicenseprototype/__init__.py,sha256=p-MTtFmMR8liEgb9nTGc3uKplgcHi82XjOC_NBxZMrY,31
+mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py,sha256=e4cbXB0RJFUcI-O6CteGhRGokuQ2C_wadQKHPvlqF6c,103
 mypackagelicenseprototype/submodule/SubmoduleContent.py,sha256=zjPPT9BTowqyb_p-SYwcLY8GadFjuh8oPfXX80r_pcM,124
 mypackagelicenseprototype/submodule/__init__.py,sha256=R6BGM-6RIVOU45qPMZaENalYgeF9SD1R68NOmOAJ4Cw,33
-mypackagelicenseprototype-2.0.6.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
-mypackagelicenseprototype-2.0.6.dist-info/METADATA,sha256=s2td0dVYonWRd-cXwf8XsakBCzIoqVc7MCZgXgmmOco,887
-mypackagelicenseprototype-2.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mypackagelicenseprototype-2.0.6.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
-mypackagelicenseprototype-2.0.6.dist-info/RECORD,,
+mypackagelicenseprototype-2.0.7.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
+mypackagelicenseprototype-2.0.7.dist-info/METADATA,sha256=PErFUG4maLkLUS_zXjN5NOaCdTXw2krdxae7wA1Ht2I,887
+mypackagelicenseprototype-2.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mypackagelicenseprototype-2.0.7.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
+mypackagelicenseprototype-2.0.7.dist-info/RECORD,,
```

