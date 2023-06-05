# Comparing `tmp/streamlit_d3_network_component-0.0.2-py3-none-any.whl.zip` & `tmp/streamlit_d3_network_component-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12827 bytes, number of entries: 41
+Zip file size: 12864 bytes, number of entries: 41
 -rw-r--r--  2.0 unx     3494 b- defN 23-Jun-05 10:00 streamlit-network-d3/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/asset-manifest.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/favicon.ico
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/index.html
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/logo192.png
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/logo512.png
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/manifest.json
@@ -31,13 +31,13 @@
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/static/media/fa-regular-400.db78b935.ttf
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/static/media/fa-regular-400.f89ea91e.woff
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/static/media/fa-solid-900.1ab236ed.ttf
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/static/media/fa-solid-900.a0369ea5.eot
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/static/media/fa-solid-900.b15db15f.woff2
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/static/media/fa-solid-900.bea989e8.woff
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 10:00 streamlit-network-d3/frontend/build/static/media/fa-solid-900.ec763292.svg
--rw-r--r--  2.0 unx     3494 b- defN 23-Jun-05 09:43 streamlit_d3_network_component/__init__.py
--rw-r--r--  2.0 unx      440 b- defN 23-Jun-05 10:01 streamlit_d3_network_component-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 10:01 streamlit_d3_network_component-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 10:01 streamlit_d3_network_component-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4857 b- defN 23-Jun-05 10:01 streamlit_d3_network_component-0.0.2.dist-info/RECORD
-41 files, 12408 bytes uncompressed, 4321 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx     3493 b- defN 23-Jun-05 10:06 streamlit_d3_network_component/__init__.py
+-rw-r--r--  2.0 unx      440 b- defN 23-Jun-05 10:06 streamlit_d3_network_component-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 10:06 streamlit_d3_network_component-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 10:06 streamlit_d3_network_component-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4857 b- defN 23-Jun-05 10:06 streamlit_d3_network_component-0.0.3.dist-info/RECORD
+41 files, 12407 bytes uncompressed, 4358 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -105,20 +105,20 @@
 
 Filename: streamlit-network-d3/frontend/build/static/media/fa-solid-900.ec763292.svg
 Comment: 
 
 Filename: streamlit_d3_network_component/__init__.py
 Comment: 
 
-Filename: streamlit_d3_network_component-0.0.2.dist-info/METADATA
+Filename: streamlit_d3_network_component-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_d3_network_component-0.0.2.dist-info/WHEEL
+Filename: streamlit_d3_network_component-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_d3_network_component-0.0.2.dist-info/top_level.txt
+Filename: streamlit_d3_network_component-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_d3_network_component-0.0.2.dist-info/RECORD
+Filename: streamlit_d3_network_component-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_d3_network_component/__init__.py

```diff
@@ -4,15 +4,15 @@
 import streamlit.components.v1 as components
 import json
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

## Comparing `streamlit_d3_network_component-0.0.2.dist-info/RECORD` & `streamlit_d3_network_component-0.0.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -30,12 +30,12 @@
 streamlit-network-d3/frontend/build/static/media/fa-regular-400.db78b935.ttf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 streamlit-network-d3/frontend/build/static/media/fa-regular-400.f89ea91e.woff,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 streamlit-network-d3/frontend/build/static/media/fa-solid-900.1ab236ed.ttf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 streamlit-network-d3/frontend/build/static/media/fa-solid-900.a0369ea5.eot,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 streamlit-network-d3/frontend/build/static/media/fa-solid-900.b15db15f.woff2,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 streamlit-network-d3/frontend/build/static/media/fa-solid-900.bea989e8.woff,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 streamlit-network-d3/frontend/build/static/media/fa-solid-900.ec763292.svg,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-streamlit_d3_network_component/__init__.py,sha256=PoITwkD1cVz-g0ZEJEV78FhQetFuoTM4lPQNgyODMlI,3494
-streamlit_d3_network_component-0.0.2.dist-info/METADATA,sha256=tI42ahTb5rKvGrxwL-qUNgkPGehc_7LslVDNtUUnrmU,440
-streamlit_d3_network_component-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-streamlit_d3_network_component-0.0.2.dist-info/top_level.txt,sha256=fXL1LxH750Jd19O3qBejvmhFJgBAxPIoGcqiGBmWnVQ,31
-streamlit_d3_network_component-0.0.2.dist-info/RECORD,,
+streamlit_d3_network_component/__init__.py,sha256=yJMe0aVqp7uto5IJL35pz35EWldBh887bv08IeEzu58,3493
+streamlit_d3_network_component-0.0.3.dist-info/METADATA,sha256=KTJ2cKTgFci6CGsuYX-sLn4mMUykJqv_GqcYnLNJ7ss,440
+streamlit_d3_network_component-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+streamlit_d3_network_component-0.0.3.dist-info/top_level.txt,sha256=fXL1LxH750Jd19O3qBejvmhFJgBAxPIoGcqiGBmWnVQ,31
+streamlit_d3_network_component-0.0.3.dist-info/RECORD,,
```

