# Comparing `tmp/mypackagelicenseprototype-1.7.7-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-1.7.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4763 bytes, number of entries: 9
+Zip file size: 4761 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     2523 b- defN 23-Jun-05 10:16 mypackagelicenseprototype/PackageContent.py
--rw-rw-rw-  2.0 fat      190 b- defN 23-Jun-05 10:13 mypackagelicenseprototype/__init__.py
+-rw-rw-rw-  2.0 fat      190 b- defN 23-Jun-05 10:18 mypackagelicenseprototype/__init__.py
 -rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-05 10:03 mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
 -rw-rw-rw-  2.0 fat      125 b- defN 23-Jun-05 10:05 pyarmor_runtime_000000/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 10:17 mypackagelicenseprototype-1.7.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 10:17 mypackagelicenseprototype-1.7.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:17 mypackagelicenseprototype-1.7.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 10:17 mypackagelicenseprototype-1.7.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      874 b- defN 23-Jun-05 10:17 mypackagelicenseprototype-1.7.7.dist-info/RECORD
-9 files, 5564 bytes uncompressed, 3211 bytes compressed:  42.3%
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 10:18 mypackagelicenseprototype-1.7.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 10:18 mypackagelicenseprototype-1.7.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:18 mypackagelicenseprototype-1.7.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 10:18 mypackagelicenseprototype-1.7.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      874 b- defN 23-Jun-05 10:18 mypackagelicenseprototype-1.7.8.dist-info/RECORD
+9 files, 5564 bytes uncompressed, 3209 bytes compressed:  42.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
 Comment: 
 
 Filename: pyarmor_runtime_000000/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.7.dist-info/LICENSE
+Filename: mypackagelicenseprototype-1.7.8.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.7.dist-info/METADATA
+Filename: mypackagelicenseprototype-1.7.8.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.7.dist-info/WHEEL
+Filename: mypackagelicenseprototype-1.7.8.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.7.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-1.7.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.7.dist-info/RECORD
+Filename: mypackagelicenseprototype-1.7.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mypackagelicenseprototype/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-from mypackagelicenseprototype.PackageContent import *
-
 # Pyarmor 8.2.3 (trial), 000000, 2023-06-05T12:12:33.594183
 from mypackagelicenseprototype.pyarmor_runtime import __pyarmor__
 
+from mypackagelicenseprototype.PackageContent import *
+
```

## Comparing `mypackagelicenseprototype-1.7.7.dist-info/LICENSE` & `mypackagelicenseprototype-1.7.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-1.7.7.dist-info/RECORD` & `mypackagelicenseprototype-1.7.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mypackagelicenseprototype/PackageContent.py,sha256=-uaKwLXEdB3Bvw2SfZzyvY_3DQNglZIWSDqtW5rm4jI,2523
-mypackagelicenseprototype/__init__.py,sha256=UGSTqmWc7uTbfcvFlnew0iyRvIhEYa5yNZJ7s-1BMjc,190
+mypackagelicenseprototype/__init__.py,sha256=rnkxZUXw-F2VnuwxvqLxAy9TYfkbsnhVI6-Lj0pz_VY,190
 mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py,sha256=9EBGxP0TXkbULvC_Wz_TQNMArucBpuK3JYh6toBaWwc,136
 pyarmor_runtime_000000/__init__.py,sha256=8CfltoBYj3lSnaVdqo0A-q9Btn55faiRWcIgfBopQOo,125
-mypackagelicenseprototype-1.7.7.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
-mypackagelicenseprototype-1.7.7.dist-info/METADATA,sha256=3pVE1ivIWJXBsxli0nmkbixyTlvmGd7YDSZv_3mZFhs,513
-mypackagelicenseprototype-1.7.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mypackagelicenseprototype-1.7.7.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
-mypackagelicenseprototype-1.7.7.dist-info/RECORD,,
+mypackagelicenseprototype-1.7.8.dist-info/LICENSE,sha256=MFjy2DRESBKfGwSsA2dSPSYX9psqdp3IvVGe7AEEhkM,1085
+mypackagelicenseprototype-1.7.8.dist-info/METADATA,sha256=frw1_AYKlcJLY9xGdKtEPE9MMcFVnd7LqJ8_5R6HGBg,513
+mypackagelicenseprototype-1.7.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mypackagelicenseprototype-1.7.8.dist-info/top_level.txt,sha256=_Q0yM1hCg8ClYW5tjn-WmYvLZGCGs4TaESHpRbB0tEQ,26
+mypackagelicenseprototype-1.7.8.dist-info/RECORD,,
```

