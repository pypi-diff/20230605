# Comparing `tmp/docleaf-0.1.0a2-cp310-cp310-manylinux_2_34_x86_64.whl.zip` & `tmp/docleaf-0.2.0a0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2294374 bytes, number of entries: 10
--rw-r--r--  4.6 unx     1184 b- defN 23-Jun-05 14:11 docleaf-0.1.0a2.dist-info/METADATA
--rw-r--r--  4.6 unx      110 b- defN 23-Jun-05 14:11 docleaf-0.1.0a2.dist-info/WHEEL
--rw-r--r--  4.6 unx     3502 b- defN 23-Jun-05 14:11 docleaf-0.1.0a2.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     2870 b- defN 23-Jun-05 14:11 docleaf/domains.py
--rw-r--r--  4.6 unx       93 b- defN 23-Jun-05 14:11 docleaf/errors.py
--rw-r--r--  4.6 unx     3673 b- defN 23-Jun-05 14:11 docleaf/copied.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-05 14:11 docleaf/__init__.py
--rw-r--r--  4.6 unx    12300 b- defN 23-Jun-05 14:11 docleaf/doxygen.py
--rwxr-xr-x  4.6 unx  8278568 b- defN 23-Jun-05 14:11 docleaf/backend.cpython-310-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      797 b- defN 23-Jun-05 14:11 docleaf-0.1.0a2.dist-info/RECORD
-10 files, 8303097 bytes uncompressed, 2293026 bytes compressed:  72.4%
+Zip file size: 2315489 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     1184 b- defN 23-Jun-05 15:47 docleaf-0.2.0a0.dist-info/METADATA
+-rw-r--r--  4.6 unx      123 b- defN 23-Jun-05 15:47 docleaf-0.2.0a0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3502 b- defN 23-Jun-05 15:47 docleaf-0.2.0a0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx       93 b- defN 23-Jun-05 15:47 docleaf/errors.py
+-rw-r--r--  4.6 unx     2870 b- defN 23-Jun-05 15:47 docleaf/domains.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-05 15:47 docleaf/__init__.py
+-rw-r--r--  4.6 unx     3673 b- defN 23-Jun-05 15:47 docleaf/copied.py
+-rw-r--r--  4.6 unx    12300 b- defN 23-Jun-05 15:47 docleaf/doxygen.py
+-rwxr-xr-x  4.6 unx  7641316 b- defN 23-Jun-05 15:47 docleaf/backend.cpython-310-i386-linux-gnu.so
+-rw-r--r--  4.6 unx      795 b- defN 23-Jun-05 15:47 docleaf-0.2.0a0.dist-info/RECORD
+10 files, 7665856 bytes uncompressed, 2314145 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: docleaf-0.1.0a2.dist-info/METADATA
+Filename: docleaf-0.2.0a0.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.1.0a2.dist-info/WHEEL
+Filename: docleaf-0.2.0a0.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.1.0a2.dist-info/license_files/LICENSE.md
-Comment: 
-
-Filename: docleaf/domains.py
+Filename: docleaf-0.2.0a0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: docleaf/errors.py
 Comment: 
 
-Filename: docleaf/copied.py
+Filename: docleaf/domains.py
 Comment: 
 
 Filename: docleaf/__init__.py
 Comment: 
 
+Filename: docleaf/copied.py
+Comment: 
+
 Filename: docleaf/doxygen.py
 Comment: 
 
-Filename: docleaf/backend.cpython-310-x86_64-linux-gnu.so
+Filename: docleaf/backend.cpython-310-i386-linux-gnu.so
 Comment: 
 
-Filename: docleaf-0.1.0a2.dist-info/RECORD
+Filename: docleaf-0.2.0a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `docleaf-0.1.0a2.dist-info/METADATA` & `docleaf-0.2.0a0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.1.0a2
+Version: 0.2.0a0
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,<6,!=5.0.0
 License-File: LICENSE.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
 Author: Michael Jones
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/docleaf-labs/docleaf
```

## Comparing `docleaf-0.1.0a2.dist-info/license_files/LICENSE.md` & `docleaf-0.2.0a0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `docleaf-0.1.0a2.dist-info/RECORD` & `docleaf-0.2.0a0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-docleaf-0.1.0a2.dist-info/METADATA,sha256=b3bXn6YXAGyaQ3_XM0QcUw33hneiaFjeqSVxJ4TckGo,1184
-docleaf-0.1.0a2.dist-info/WHEEL,sha256=L98fCWQzY8AHUKCt5LhJCDWVrTp_lzcRP08bVdZXElw,110
-docleaf-0.1.0a2.dist-info/license_files/LICENSE.md,sha256=20NXnKx0h0eVlML_pg1pYvMUOGbuZsAwACSzigFYQx0,3502
-docleaf/domains.py,sha256=-egzFCmmYmKldtA_Cs3vBy3leme2SSHFBKkGRgXUzNE,2870
+docleaf-0.2.0a0.dist-info/METADATA,sha256=LqyZXG7sCuzuhmiyM42ULd7W69aoB-5J-rfFeE0gm0Q,1184
+docleaf-0.2.0a0.dist-info/WHEEL,sha256=bzJxnlccrvEHc_LpfrfYCkrVsEdrH5EmG069RcyLKIU,123
+docleaf-0.2.0a0.dist-info/license_files/LICENSE.md,sha256=20NXnKx0h0eVlML_pg1pYvMUOGbuZsAwACSzigFYQx0,3502
 docleaf/errors.py,sha256=FjwCrBWj0_XRF_63IkYnz8_24FpTHlKE3bek1Iajp9Y,93
-docleaf/copied.py,sha256=xZKyniORIB8IQol2pUuwGjVPqOrihfU1SLV-Fo6lwhw,3673
+docleaf/domains.py,sha256=-egzFCmmYmKldtA_Cs3vBy3leme2SSHFBKkGRgXUzNE,2870
 docleaf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+docleaf/copied.py,sha256=xZKyniORIB8IQol2pUuwGjVPqOrihfU1SLV-Fo6lwhw,3673
 docleaf/doxygen.py,sha256=mi4RPRTeVOGICNpHOF-33ui2rfoB6AvVCl7YulCeK1w,12300
-docleaf/backend.cpython-310-x86_64-linux-gnu.so,sha256=BJnHaStgh0HJzjPwpkn0JMetodaYO5XH5xGvrnoHi_E,8278568
-docleaf-0.1.0a2.dist-info/RECORD,,
+docleaf/backend.cpython-310-i386-linux-gnu.so,sha256=7lGcsJ0iy942eZuui47KcxeXrEVCVWTCwTlc9DQZFbo,7641316
+docleaf-0.2.0a0.dist-info/RECORD,,
```

