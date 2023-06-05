# Comparing `tmp/pulsestreamer-1.6.2-py2.py3-none-any.whl.zip` & `tmp/pulsestreamer-1.7.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 26360 bytes, number of entries: 16
--rw-r--r--  2.0 unx      579 b- defN 23-Mar-07 22:53 pulsestreamer/__init__.py
+Zip file size: 26359 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      579 b- defN 23-Jun-03 13:13 pulsestreamer/__init__.py
 -rw-r--r--  2.0 unx      628 b- defN 22-Nov-29 10:55 pulsestreamer/__main__.py
--rw-r--r--  2.0 unx      305 b- defN 22-Nov-29 10:55 pulsestreamer/enums.py
+-rw-r--r--  2.0 unx      305 b- defN 23-May-23 09:35 pulsestreamer/enums.py
 -rw-r--r--  2.0 unx     6232 b- defN 22-Nov-29 10:55 pulsestreamer/findPulseStreamers.py
--rw-r--r--  2.0 unx    26191 b- defN 23-Feb-15 11:07 pulsestreamer/sequence.py
--rw-r--r--  2.0 unx     1538 b- defN 22-Nov-29 10:55 pulsestreamer/version.py
+-rw-r--r--  2.0 unx    26191 b- defN 23-May-14 10:59 pulsestreamer/sequence.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-May-23 09:35 pulsestreamer/version.py
 -rw-r--r--  2.0 unx       46 b- defN 22-Nov-29 10:55 pulsestreamer/grpc/__init__.py
--rw-r--r--  2.0 unx    19090 b- defN 22-Dec-02 17:58 pulsestreamer/grpc/pulse_streamer_grpc.py
--rw-r--r--  2.0 unx     8985 b- defN 23-Mar-07 22:53 pulsestreamer/grpc/pulse_streamer_pb2.py
--rw-r--r--  2.0 unx    55237 b- defN 23-Mar-07 22:53 pulsestreamer/grpc/pulse_streamer_pb2_grpc.py
+-rw-r--r--  2.0 unx    19090 b- defN 22-Dec-01 10:54 pulsestreamer/grpc/pulse_streamer_grpc.py
+-rw-r--r--  2.0 unx     8985 b- defN 23-Jun-03 13:13 pulsestreamer/grpc/pulse_streamer_pb2.py
+-rw-r--r--  2.0 unx    55237 b- defN 23-Jun-03 13:13 pulsestreamer/grpc/pulse_streamer_pb2_grpc.py
 -rw-r--r--  2.0 unx      114 b- defN 22-Nov-29 10:55 pulsestreamer/jrpc/__init__.py
--rw-r--r--  2.0 unx    15806 b- defN 23-Feb-15 09:15 pulsestreamer/jrpc/pulse_streamer_jrpc.py
--rw-r--r--  2.0 unx     1091 b- defN 22-Nov-29 10:55 pulsestreamer-1.6.2.dist-info/LICENSE.txt
-?rw-r--r--  2.0 unx       99 b- defN 16-Jan-01 00:00 pulsestreamer-1.6.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1797 b- defN 16-Jan-01 00:00 pulsestreamer-1.6.2.dist-info/METADATA
-?rw-r--r--  2.0 unx     1387 b- defN 16-Jan-01 00:00 pulsestreamer-1.6.2.dist-info/RECORD
-16 files, 139125 bytes uncompressed, 24056 bytes compressed:  82.7%
+-rw-r--r--  2.0 unx    15806 b- defN 23-May-23 09:35 pulsestreamer/jrpc/pulse_streamer_jrpc.py
+-rw-r--r--  2.0 unx     1091 b- defN 22-Nov-29 10:55 pulsestreamer-1.7.0.dist-info/LICENSE.txt
+?rw-r--r--  2.0 unx       99 b- defN 16-Jan-01 00:00 pulsestreamer-1.7.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1797 b- defN 16-Jan-01 00:00 pulsestreamer-1.7.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     1387 b- defN 16-Jan-01 00:00 pulsestreamer-1.7.0.dist-info/RECORD
+16 files, 139125 bytes uncompressed, 24055 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: pulsestreamer/jrpc/__init__.py
 Comment: 
 
 Filename: pulsestreamer/jrpc/pulse_streamer_jrpc.py
 Comment: 
 
-Filename: pulsestreamer-1.6.2.dist-info/LICENSE.txt
+Filename: pulsestreamer-1.7.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pulsestreamer-1.6.2.dist-info/WHEEL
+Filename: pulsestreamer-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: pulsestreamer-1.6.2.dist-info/METADATA
+Filename: pulsestreamer-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: pulsestreamer-1.6.2.dist-info/RECORD
+Filename: pulsestreamer-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pulsestreamer/__init__.py

```diff
@@ -1,10 +1,10 @@
 """A client software for Swabian Instrument's Pulse Streamer 8/2"""
 
-__version__ = '1.6.2'
+__version__ = '1.7.0'
 
 from pulsestreamer.jrpc import PulseStreamer
 from pulsestreamer.enums import ClockSource, TriggerRearm, TriggerStart
 from pulsestreamer.sequence import Sequence, OutputState
 from pulsestreamer.findPulseStreamers import findPulseStreamers
 from pulsestreamer.version import _compare_version_number
```

## Comparing `pulsestreamer-1.6.2.dist-info/LICENSE.txt` & `pulsestreamer-1.7.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pulsestreamer-1.6.2.dist-info/METADATA` & `pulsestreamer-1.7.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsestreamer
-Version: 1.6.2
+Version: 1.7.0
 Summary: A client software for Swabian Instrument's Pulse Streamer 8/2
 Home-page: https://www.swabianinstruments.com/pulse-streamer-8-2/
 License: MIT
 Author: Swabian Instruments GmbH
 Author-email: support@swabianinstruments.com
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

## Comparing `pulsestreamer-1.6.2.dist-info/RECORD` & `pulsestreamer-1.7.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pulsestreamer/__init__.py,sha256=0VQ2LU_WLHPHBJ_kRuHieP5K83lDVuI5z4ik3Hy4CUs,579
+pulsestreamer/__init__.py,sha256=wtoAi9JvAmcmDfezmcVWVLhjMInhBETgJ6S3bAYbk6s,579
 pulsestreamer/__main__.py,sha256=cZnoxQekIUOpzfa7j7qLebd-CldXOmr-vPneAVRXp7A,628
 pulsestreamer/enums.py,sha256=jbggOeF8MS_xDTvC9YxwZObat1hUqxws-CbpURa55AE,305
 pulsestreamer/findPulseStreamers.py,sha256=2zS_J5zqBNVXN42tiemWA0EL2xjXcYA9GAXFV6Cbm7I,6232
 pulsestreamer/sequence.py,sha256=TnAAoBQuSh4_kAfREENXyE2d-U_F2AzV0nMiGAuyLbg,26191
 pulsestreamer/version.py,sha256=7p1zDUkXyhWThrTEZ2QGMICin3YJhhnhfY6K6x7dQLc,1538
 pulsestreamer/grpc/__init__.py,sha256=6nZJITzcQNdYCoJ2mq7j_MvkSAgHqbE-EMcHmM2Famg,46
 pulsestreamer/grpc/pulse_streamer_grpc.py,sha256=FF1VP_1JzFONLt2eO-gTRL8QTxJh29VBZn3ZuuKFsUs,19090
 pulsestreamer/grpc/pulse_streamer_pb2.py,sha256=lM9kkSnK4QwFbXOXuVQBzbm5gayJYGAX-CeYFG1mpbg,8985
 pulsestreamer/grpc/pulse_streamer_pb2_grpc.py,sha256=PWdbtM2toc4-ikt3-EFha_IlEPpXvGdA2M3D8gIkWLg,55237
 pulsestreamer/jrpc/__init__.py,sha256=YzDCRkbF2k3ryrddlJB8F7ltfzgS3x85OmzQhb3l2C0,114
 pulsestreamer/jrpc/pulse_streamer_jrpc.py,sha256=ITpErGishsTWtl7jKpHZGysHxceYcDRqP5owGZrWP60,15806
-pulsestreamer-1.6.2.dist-info/LICENSE.txt,sha256=xxmkbLwlkbYV2W27IP0RNNf5d3OTGC1wdR6v60q5v2A,1091
-pulsestreamer-1.6.2.dist-info/WHEEL,sha256=kdeDBNPvBI0w3meLKPoGgAnEr54n1jzrZWUoaLmGzVY,99
-pulsestreamer-1.6.2.dist-info/METADATA,sha256=VG9IVxWtpmORlGWxfMxhV3p8epmI3SJPCXczD2i65Nk,1797
-pulsestreamer-1.6.2.dist-info/RECORD,,
+pulsestreamer-1.7.0.dist-info/LICENSE.txt,sha256=xxmkbLwlkbYV2W27IP0RNNf5d3OTGC1wdR6v60q5v2A,1091
+pulsestreamer-1.7.0.dist-info/WHEEL,sha256=kdeDBNPvBI0w3meLKPoGgAnEr54n1jzrZWUoaLmGzVY,99
+pulsestreamer-1.7.0.dist-info/METADATA,sha256=RwuzdOXS10Quke4u8vIwZOhJCtGWU1adCD3P6Y-PT6I,1797
+pulsestreamer-1.7.0.dist-info/RECORD,,
```

