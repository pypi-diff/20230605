# Comparing `tmp/cirq-1.2.0.dev20230602213529-py3-none-any.whl.zip` & `tmp/cirq-1.2.0.dev20230605100941-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7975 bytes, number of entries: 5
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-02 21:35 cirq-1.2.0.dev20230602213529.dist-info/LICENSE
--rw-r--r--  2.0 unx     7781 b- defN 23-Jun-02 21:35 cirq-1.2.0.dev20230602213529.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 21:35 cirq-1.2.0.dev20230602213529.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 21:35 cirq-1.2.0.dev20230602213529.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      461 b- defN 23-Jun-02 21:35 cirq-1.2.0.dev20230602213529.dist-info/RECORD
-5 files, 19692 bytes uncompressed, 7105 bytes compressed:  63.9%
+Zip file size: 7974 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-05 10:09 cirq-1.2.0.dev20230605100941.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7781 b- defN 23-Jun-05 10:09 cirq-1.2.0.dev20230605100941.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 10:09 cirq-1.2.0.dev20230605100941.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-05 10:09 cirq-1.2.0.dev20230605100941.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      461 b- defN 23-Jun-05 10:09 cirq-1.2.0.dev20230605100941.dist-info/RECORD
+5 files, 19692 bytes uncompressed, 7104 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: cirq-1.2.0.dev20230602213529.dist-info/LICENSE
+Filename: cirq-1.2.0.dev20230605100941.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.2.0.dev20230602213529.dist-info/METADATA
+Filename: cirq-1.2.0.dev20230605100941.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.2.0.dev20230602213529.dist-info/WHEEL
+Filename: cirq-1.2.0.dev20230605100941.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.2.0.dev20230602213529.dist-info/top_level.txt
+Filename: cirq-1.2.0.dev20230605100941.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.2.0.dev20230602213529.dist-info/RECORD
+Filename: cirq-1.2.0.dev20230605100941.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.2.0.dev20230602213529.dist-info/LICENSE` & `cirq-1.2.0.dev20230605100941.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.2.0.dev20230602213529.dist-info/METADATA` & `cirq-1.2.0.dev20230605100941.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.2.0.dev20230602213529
+Version: 1.2.0.dev20230605100941
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
-Requires-Dist: cirq-aqt (==1.2.0.dev20230602213529)
-Requires-Dist: cirq-core (==1.2.0.dev20230602213529)
-Requires-Dist: cirq-google (==1.2.0.dev20230602213529)
-Requires-Dist: cirq-ionq (==1.2.0.dev20230602213529)
-Requires-Dist: cirq-pasqal (==1.2.0.dev20230602213529)
-Requires-Dist: cirq-rigetti (==1.2.0.dev20230602213529)
-Requires-Dist: cirq-web (==1.2.0.dev20230602213529)
+Requires-Dist: cirq-aqt (==1.2.0.dev20230605100941)
+Requires-Dist: cirq-core (==1.2.0.dev20230605100941)
+Requires-Dist: cirq-google (==1.2.0.dev20230605100941)
+Requires-Dist: cirq-ionq (==1.2.0.dev20230605100941)
+Requires-Dist: cirq-pasqal (==1.2.0.dev20230605100941)
+Requires-Dist: cirq-rigetti (==1.2.0.dev20230605100941)
+Requires-Dist: cirq-web (==1.2.0.dev20230605100941)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
 Requires-Dist: pytest ; extra == 'dev_env'
```

