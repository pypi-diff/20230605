# Comparing `tmp/mypackagelicenseprototype-1.8.4-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 223766 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     2523 b- defN 23-Jun-05 10:16 mypackagelicenseprototype/PackageContent.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-Jun-05 10:40 mypackagelicenseprototype/__init__.py
--rw-rw-rw-  2.0 fat   615936 b- defN 23-Jun-05 10:12 mypackagelicenseprototype/pyarmor_runtime.pyd
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      772 b- defN 23-Jun-05 10:40 mypackagelicenseprototype-1.8.4.dist-info/RECORD
-8 files, 621127 bytes uncompressed, 222388 bytes compressed:  64.2%
+Zip file size: 2747 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      140 b- defN 23-Jun-05 09:04 mypackagelicenseprototype/PackageContent.py
+-rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-05 10:59 mypackagelicenseprototype/__init__.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 11:05 mypackagelicenseprototype-2.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      444 b- defN 23-Jun-05 11:05 mypackagelicenseprototype-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 11:05 mypackagelicenseprototype-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 11:05 mypackagelicenseprototype-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      666 b- defN 23-Jun-05 11:05 mypackagelicenseprototype-2.0.0.dist-info/RECORD
+7 files, 2484 bytes uncompressed, 1535 bytes compressed:  38.2%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: mypackagelicenseprototype/PackageContent.py
 Comment: 
 
 Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype/pyarmor_runtime.pyd
+Filename: mypackagelicenseprototype-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.4.dist-info/LICENSE
+Filename: mypackagelicenseprototype-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.4.dist-info/METADATA
+Filename: mypackagelicenseprototype-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.4.dist-info/WHEEL
+Filename: mypackagelicenseprototype-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mypackagelicenseprototype-1.8.4.dist-info/top_level.txt
-Comment: 
-
-Filename: mypackagelicenseprototype-1.8.4.dist-info/RECORD
+Filename: mypackagelicenseprototype-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mypackagelicenseprototype/PackageContent.py

```diff
@@ -1,3 +1,7 @@
-# Pyarmor 8.2.3 (trial), 000000, non-profits, 2023-06-05T12:12:33.599497
-#from mypackagelicenseprototype.pyarmor_runtime import __pyarmor__
-__pyarmor__(__name__, __file__, b'PY000000\x00\x03\t\x00a\r\r\n\x80\x00\x01\x00\x08\x00\x00\x00\x04\x00\x00\x00@\x00\x00\x00\xed\x02\x00\x00\x12\t\x04\x00\xde\xa23p\xe5a\xe6~\x908\x97H\xdbi\x97-\x00\x00\x00\x00\x00\x00\x00\x00\xfd\x9a\xa0l\xf12vx0`\xff\xfc\x81q\xb6\xe9\xa58\xca,-I7\xa3\xb2\xa4"#2\t\x19\n\x1d\xe3%\xb2-\xdf\xc4$\x139\x9d\xd4\xf4\x9a4S\x07hY\xc9&g\xaa\xe1\x17\xa1a\xc9 N\xf5\xd0\xfdD-7\n\xa6c\x16vUj\xfbr\'^\xcdqg\x12n\x7f\x10\xf7;Te\x90-\xbcO\xde\xbc\np\x1e\xac\xb6i#x\x86\x99\xca\x02\x83\xd2h\x84\x9f\xf7\xfc\xfbC\x9c\xeb\xc4\xfb\x0c\xe9\x9a\xcb\x97\xba})\x9015N@l\xd3\xf9q\x11\x02\xe0\xb8\xf4\xdd\xb9\x17\x1f<\x10\xda\xa9\x85\nE=$\x9c\xeed\xde\xe9\xf9\xa6\x17lr\x19\xd9)=l\xea\xb2\xc2\x04c\x7f\xe1\x94\xc0RN\xd8\x185\x81#\x97#"\xf7M\xfd\xd2\xff\x0cLh\xa7\xdd\xdd\x88/\x01\xd9\x1e\xa6\xcbi\xffx\xcf\x9aq\xd7\xfa\xb5\xdfl\x89\xe5O\x14a\xd0\xdb\xd1\x11\x1d\xf9n\x98V\x00|\xc3};\x93\x1d\xce\xa4\xf5>|\tZ\xaa\xb5Q\x1b\xf5g\x0f\x8b1F0\xc6-\xeeE*\xb3\xd1\x05q\xc2\x80or\x83\xda\x805]\xc4\xf5\x82\xc2z\xee\xe5\xb7\x00\xc5\x9f|T|\x89A\x82\x10\x10h\xf6\x7f\xd7\xb1\xd2\x88\xd5jUN\x83O\x84H\xd2\xbc\x8e;\x83"\x8eE\xc7\xbf\x8c\x9ag\x11<U\x0b\x92\x03\x95Hh\xedIlM\xe9\xfd\xd3I\xd5\xfba\x91x\xff\xb9J\xe8\n\x13y\xc3K\x9d%qA,c\x1c1\xeeV\xd0\xe1)\xe1fE\x82e\xb2\xc7\x13\xb1\x10\r4\xe1\xc1\xef\xca\xf4\xbb\xa2D\xc9|\x93\xa8>\xe2?\x94\xa0\xe4\xc2\xe6\x1d<\x00Nx1\xb2e\'\x05g]\x81Y\xc7\xec\xbe\x05\xee\x17\x81\xc1\xceq\x89=\x8f,\x86\xb6q\x9f\xa1:[\xc3_\xef\xfeF\x0f&\xcc\x1f\xc6\x88\x17\x15c\x8d\xfe_\xa9\xb4\xe2)N\xe3\xb6\xb9\xedH\xd5\xd5\xa1\x94\xedo\x93OZr&\xaf\xe1\x9d89\xc9\xa3\xf8|}Ooe\x15\xbe)\xfb\x9b\xedP\xd8\xb3\xe2%\xb8.\xa8\xb8R\x9d\xbb\xd3\x0fI\xc1\xd4EY-?u%\x80+\x8cS\x8e\xd9\xf0\x84~?M\xa7\xa2\xde<\xd8,\xb1e\x98h\xa0,A\xd4H\x1d\x8b\xcb\r/\xb7\xe8\xdf\xf1\x01[\x9a\x93\x96\x89\x91\x1b\xf1\xf9\xa3\xb8\xb2\x9c\\\xad@j\x16~\xb8\xfbc\x9f\xda\xc6\x89\xe2\x81\x1c\xbd\xd5G\xe7\xab\xc4C\xf6\xf6\xd8\x9cG\xa1\xcc\x1a\xfe:\x97u\xb1H\xce\xbd\xea\x82\x06\x10\x8d5\xda\xdc\x97\x9d nO\x08W\xdf\x8c\x11|\xde\x81\xad+0\x8c\xc7\xcd\xf2\x14\xcb\x1c\xbay\x0b\xba\xaa#o \x04\xab\xa4\xb5\xb8\xb1wy7\xf7zX\xe1\x1d|\xab\x84\x19\xc5l\x12}\xe6\x97o\xd7f\xc3\xbf\xe1\xe5\xea\xddS0\x84xU\x0f\xe3\xc7\x81\x1cv$\xc0\xb4\x14\x81\xc0\rAL]\xecqH\xbf\xec\xa5\xcd1\xa9\xf6\xc2\x97\xe6v\xb5\x19)\x94\x1e\xc1y%\xafi\xa2\xa2\xde\xe6\xddb\x93B\x84\xddUiB\xf9\xf5\x02s\x1d\xbf\x87\xaaoV3Y\x00\x907D|')
+import numpy as np
+
+def add_numbers_2(a, b):
+    """
+    Adds two numbers and returns the result.
+    """
+    return a + 2 *np.sqrt(2)
```

## mypackagelicenseprototype/__init__.py

```diff
@@ -1,6 +1 @@
-# Pyarmor 8.2.3 (trial), 000000, 2023-06-05T12:12:33.594183
-from mypackagelicenseprototype.pyarmor_runtime import *
-
-from mypackagelicenseprototype.PackageContent import *
-
-
+from .PackageContent import *
```

## Comparing `mypackagelicenseprototype-1.8.4.dist-info/LICENSE` & `mypackagelicenseprototype-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

