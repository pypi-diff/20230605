# Comparing `tmp/mypackagelicenseprototype-1.7.4-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-1.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 4394 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     2538 b- defN 23-Jun-05 10:00 mypackagelicenseprototype/PackageContent.py
+Zip file size: 4675 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     2512 b- defN 23-Jun-05 10:05 mypackagelicenseprototype/PackageContent.py
 -rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-05 09:52 mypackagelicenseprototype/__init__.py
 -rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-05 10:03 mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 10:03 mypackagelicenseprototype-1.7.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 10:03 mypackagelicenseprototype-1.7.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:03 mypackagelicenseprototype-1.7.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jun-05 10:03 mypackagelicenseprototype-1.7.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      783 b- defN 23-Jun-05 10:03 mypackagelicenseprototype-1.7.4.dist-info/RECORD
-8 files, 5231 bytes uncompressed, 2986 bytes compressed:  42.9%
+-rw-rw-rw-  2.0 fat      125 b- defN 23-Jun-05 10:05 pyarmor_runtime_000000/__init__.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-05 10:05 mypackagelicenseprototype-1.7.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Jun-05 10:05 mypackagelicenseprototype-1.7.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:05 mypackagelicenseprototype-1.7.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-05 10:05 mypackagelicenseprototype-1.7.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      873 b- defN 23-Jun-05 10:05 mypackagelicenseprototype-1.7.5.dist-info/RECORD
+9 files, 5443 bytes uncompressed, 3123 bytes compressed:  42.6%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: mypackagelicenseprototype/__init__.py
 Comment: 
 
 Filename: mypackagelicenseprototype/pyarmor_runtime_000000/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.4.dist-info/LICENSE
+Filename: pyarmor_runtime_000000/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.4.dist-info/METADATA
+Filename: mypackagelicenseprototype-1.7.5.dist-info/LICENSE
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.4.dist-info/WHEEL
+Filename: mypackagelicenseprototype-1.7.5.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.4.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-1.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-1.7.4.dist-info/RECORD
+Filename: mypackagelicenseprototype-1.7.5.dist-info/top_level.txt
+Comment: 
+
+Filename: mypackagelicenseprototype-1.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mypackagelicenseprototype/PackageContent.py

```diff
@@ -1,3 +1,3 @@
 # Pyarmor 8.2.3 (trial), 000000, non-profits, 2023-06-05T11:42:47.211088
-from mypackagelicenseprototype.pyarmor_runtime_000000 import __pyarmor__
+from pyarmor_runtime_000000 import __pyarmor__
 __pyarmor__(__name__, __file__, b"PY000000\x00\x03\n\x00o\r\r\n\x80\x00\x01\x00\x08\x00\x00\x00\x04\x00\x00\x00@\x00\x00\x00\xea\x02\x00\x00\x12\t\x04\x00\xc1b\xb6\xd9\x9d\x1b\x14\x01p$j\xe1m\xf7ui\x00\x00\x00\x00\x00\x00\x00\x00\xe4!)\xf0b\x1c\x87\x0f|\x08J\x94rL\x1eT\xc3O\x93.-\x06\xaa\xbc{=\xb0d\xa0\xf6:{\xcd\x03\xf2\xb1\xf0\xdf\xd4\xc2\xce\t\xedZB\xf7<K#\x90n\xd6s5t\xc7\xc6\xd9XR9\xdf'\xf7\x10\xc6\xe9!\x98\xb53qNzT\x15Y&\xea\xbc-!T$\x17\x06gCS'\xabt\x8e\xac\x84\x0f\r3\xf3R\xdc\x0cJ\xd2\x05\xb5\x1f\xab=n\xda\x12\xfa4+\xbe\xb2\x9f\xd0\xa1zg\xcc\xde\x93\xda20>\xa0\xdc\x1f\x9c\x98\xba\xac\xb5\x92\xca\x9a:6\xdb)\x0bp\xa6E\xbb\xea\xc1\xaf\x89\x8f\xdck\x1b\x16\xda\xb4u\xb5d\xf8\xf6\x7fJ\xa0'\xee\x9f.\xd9+\x15\xf7P\xa1\xbf\xb1\xfd\x02\x15\xbc\x9cc\xd9\xdb\xf38\x93\\\xe1i\xe1\x0e\xd4\xed\xb0X\x98\x1c\x1f\xc0\x96.\xcf.q\xd7\x9aB\xbe,.\xd4\xac:\xc9c\x8dI\x126\xe5o\xa7\xf3\x00\xe7\xd9\x192\x9cR16\x12\x08\x0f\xee\x98\x88\xae7\x0bD\x81&\x96e\x0f\xebj\n.\xb2[F\x1e\x8f\xac\xd12w\x95\xa0c\x9b\x8b\x9fhf\xd1O\xae<\x94\x84\xc6mhQ\x8c\x98\xe4_\n>!k\xa0k\xeb\x07\xc7V\xb3\x9d k2k\x83\x87\xa7\x1d\x7f'0`%&~*\xf8\xee\xccOZUj\xed\xbf\xfcj\xb4p\xd5\xaf\xbe\xb8\xde\xf5\xa9yy\xca\xc1\t\xbd:r\xe8.\xcd*\x0b)|\x8f\x1d\xa9\xc8MB\x9e\xec\xdf\xfa\xc7xc\xd4\x02\xd5\xb9\xdb\t\x08\xf3\x99\xeb9i\xcca\xb1\xce\x85o{\xe6\xa6\xa0\xf7\xbd\xc1b\xea9\xcdI\x01w\xaaD\x0b\xa2\xad\x1e\xd8a\xb1\x88\xd8Gn\xb7q\xf8\x8c@\xd3@\x08)\xa3\x8d\x8b1\xddx\xa8\x04\xd2\x9f.z\xd1\xb8\xcd\xe3R\x0c\x071\xac\xcb\xb7D\xd7\t0\x87\xbd\xb19Y\x14\x8c\x90\xdd[\x8a\xa6\x03\x1eS$\x8f\x93\x99s'<\xb57\x8f\xf5\xa1sT\xeb\x1b\xf7\xb4\xd0\n\x87\xd9\x8c\x15\x9d\\Y\xe3\x9eu\n1<RI\xa4\xdcA\xd0\x99\x9d\x86%\x10\xd0\xc9\x046\xf4J\xa9\xe8b\x9d\x8eu\xed\x95\xe8\xc2\xa1\xb4\xd8Z7\x8f\xb7\xcdV\xcc>\xb4\r\xf0\xd2R^)\xc5D\x143H\xa0*=\xa31\xc2n\xa0\xfe\x0b\xef\x11\xcf\xf2\x86_\xc1\xdb\xd3\x902\x08n\xed\xc6\xe9\xdaW\xb2\xaeM\xf7\xb4s\x170\xc6\x8f%\xce\xd0\xaf\x05\xc0\xd0.~\x00Y19\xd4c\x0e\xbaQ\xf5\xae\xd0\x84K\xc1\xa8\xf2\xc1B\xb4\x83\xc7\nb\xc1\xf1F^'\xc0?\x04\x98\xce3]\xf5\xf6\xc7f\xfa\x81>?\x02\xb2\xec\xb6^\x94h\x99\x95=\xd1\xa5\xa3\x06\xfb\x00\x15\xd0\xdf\x03\xfa\xcb\xd7\xfaJ\x7ft~\x10\xb0|\xfdK8D\xddlzT\x83p\xcd?\xc1\xba7\x81\x9d\xdb\xbdc4\xbd\x1d\x0b\xf7\xf9\x08\x07\xd2@\xb3\x87,C\x02\xed\x01{-\xd0\x03\xa8\xd9^?\x15\xacH\x06\xbd\xe9\xb7W\xceS\xcf\x96\x9b\xc2\xa5\x98.\xc5\xeb\xca\x03{\x8e\x88`/\x8d\x98^\xa6\x8d\x80i\xac.\xd8\x0b")
```

## Comparing `mypackagelicenseprototype-1.7.4.dist-info/LICENSE` & `mypackagelicenseprototype-1.7.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mypackagelicenseprototype-1.7.4.dist-info/METADATA` & `mypackagelicenseprototype-1.7.5.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackagelicenseprototype
-Version: 1.7.4
+Version: 1.7.5
 Summary: Description of your package
 Home-page: https://github.com/da-roth/PackageLicensePrototype
 Author: Daniel Roth
 Author-email: daniel-roth@posteo.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

