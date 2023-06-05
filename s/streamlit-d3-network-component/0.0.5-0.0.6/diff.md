# Comparing `tmp/streamlit-d3-network-component-0.0.5.tar.gz` & `tmp/streamlit-d3-network-component-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-d3-network-component-0.0.5.tar", last modified: Mon Jun  5 10:12:37 2023, max compression
+gzip compressed data, was "streamlit-d3-network-component-0.0.6.tar", last modified: Mon Jun  5 10:16:50 2023, max compression
```

## Comparing `streamlit-d3-network-component-0.0.5.tar` & `streamlit-d3-network-component-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.958351 streamlit-d3-network-component-0.0.5/
--rw-r--r--   0 andras     (501) staff       (20)       65 2023-06-05 10:12:17.000000 streamlit-d3-network-component-0.0.5/MANIFEST.in
--rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 10:12:37.958121 streamlit-d3-network-component-0.0.5/PKG-INFO
--rw-r--r--   0 andras     (501) staff       (20)       38 2023-06-05 10:12:37.958408 streamlit-d3-network-component-0.0.5/setup.cfg
--rw-r--r--   0 andras     (501) staff       (20)      798 2023-06-05 10:12:26.000000 streamlit-d3-network-component-0.0.5/setup.py
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.762452 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/
--rw-r--r--   0 andras     (501) staff       (20)     3492 2023-06-05 10:09:51.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/__init__.py
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.760207 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.860376 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/
--rw-r--r--   0 andras     (501) staff       (20)     1307 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/asset-manifest.json
--rw-rw-r--   0 andras     (501) staff       (20)     3150 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/favicon.ico
--rw-r--r--   0 andras     (501) staff       (20)     2302 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/index.html
--rw-rw-r--   0 andras     (501) staff       (20)     5347 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/logo192.png
--rw-rw-r--   0 andras     (501) staff       (20)     9664 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/logo512.png
--rw-rw-r--   0 andras     (501) staff       (20)      492 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/manifest.json
--rw-r--r--   0 andras     (501) staff       (20)     2486 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/precache-manifest.9a6cee5862e83e747d32a923936a576d.js
--rw-rw-r--   0 andras     (501) staff       (20)       67 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/robots.txt
--rw-r--r--   0 andras     (501) staff       (20)     1181 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/service-worker.js
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.761163 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.868725 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/
--rw-r--r--   0 andras     (501) staff       (20)    58890 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css
--rw-r--r--   0 andras     (501) staff       (20)    89084 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map
--rw-r--r--   0 andras     (501) staff       (20)     1007 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css
--rw-r--r--   0 andras     (501) staff       (20)     1899 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.923276 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/
--rw-r--r--   0 andras     (501) staff       (20)  1022852 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js
--rw-r--r--   0 andras     (501) staff       (20)     5927 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.LICENSE.txt
--rw-r--r--   0 andras     (501) staff       (20)  4266749 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.map
--rw-r--r--   0 andras     (501) staff       (20)     5506 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js
--rw-r--r--   0 andras     (501) staff       (20)    21943 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map
--rw-r--r--   0 andras     (501) staff       (20)     1575 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js
--rw-r--r--   0 andras     (501) staff       (20)     8288 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.957236 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/
--rw-r--r--   0 andras     (501) staff       (20)   715890 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg
--rw-r--r--   0 andras     (501) staff       (20)   132728 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf
--rw-r--r--   0 andras     (501) staff       (20)    76612 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2
--rw-r--r--   0 andras     (501) staff       (20)   133034 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot
--rw-r--r--   0 andras     (501) staff       (20)    89824 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff
--rw-r--r--   0 andras     (501) staff       (20)    34390 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot
--rw-r--r--   0 andras     (501) staff       (20)   144322 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg
--rw-r--r--   0 andras     (501) staff       (20)    13584 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2
--rw-r--r--   0 andras     (501) staff       (20)    34092 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf
--rw-r--r--   0 andras     (501) staff       (20)    16800 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff
--rw-r--r--   0 andras     (501) staff       (20)   202616 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf
--rw-r--r--   0 andras     (501) staff       (20)   202902 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot
--rw-r--r--   0 andras     (501) staff       (20)    79444 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2
--rw-r--r--   0 andras     (501) staff       (20)   103300 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff
--rw-r--r--   0 andras     (501) staff       (20)   897426 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:12:37.764828 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component.egg-info/
--rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 10:12:37.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component.egg-info/PKG-INFO
--rw-r--r--   0 andras     (501) staff       (20)     3107 2023-06-05 10:12:37.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component.egg-info/SOURCES.txt
--rw-r--r--   0 andras     (501) staff       (20)        1 2023-06-05 10:12:37.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component.egg-info/dependency_links.txt
--rw-r--r--   0 andras     (501) staff       (20)       16 2023-06-05 10:12:37.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component.egg-info/requires.txt
--rw-r--r--   0 andras     (501) staff       (20)       31 2023-06-05 10:12:37.000000 streamlit-d3-network-component-0.0.5/streamlit_d3_network_component.egg-info/top_level.txt
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.149409 streamlit-d3-network-component-0.0.6/
+-rw-r--r--   0 andras     (501) staff       (20)       65 2023-06-05 10:12:17.000000 streamlit-d3-network-component-0.0.6/MANIFEST.in
+-rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 10:16:50.148939 streamlit-d3-network-component-0.0.6/PKG-INFO
+-rw-r--r--   0 andras     (501) staff       (20)       38 2023-06-05 10:16:50.149488 streamlit-d3-network-component-0.0.6/setup.cfg
+-rw-r--r--   0 andras     (501) staff       (20)      798 2023-06-05 10:16:43.000000 streamlit-d3-network-component-0.0.6/setup.py
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.107575 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/
+-rw-r--r--   0 andras     (501) staff       (20)     3496 2023-06-05 10:16:43.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/__init__.py
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.103947 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.126454 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/
+-rw-r--r--   0 andras     (501) staff       (20)     1307 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/asset-manifest.json
+-rw-rw-r--   0 andras     (501) staff       (20)     3150 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/favicon.ico
+-rw-r--r--   0 andras     (501) staff       (20)     2302 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/index.html
+-rw-rw-r--   0 andras     (501) staff       (20)     5347 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/logo192.png
+-rw-rw-r--   0 andras     (501) staff       (20)     9664 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/logo512.png
+-rw-rw-r--   0 andras     (501) staff       (20)      492 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/manifest.json
+-rw-r--r--   0 andras     (501) staff       (20)     2486 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/precache-manifest.9a6cee5862e83e747d32a923936a576d.js
+-rw-rw-r--   0 andras     (501) staff       (20)       67 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/robots.txt
+-rw-r--r--   0 andras     (501) staff       (20)     1181 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/service-worker.js
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.104961 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.128718 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/
+-rw-r--r--   0 andras     (501) staff       (20)    58890 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css
+-rw-r--r--   0 andras     (501) staff       (20)    89084 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map
+-rw-r--r--   0 andras     (501) staff       (20)     1007 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css
+-rw-r--r--   0 andras     (501) staff       (20)     1899 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.136523 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/
+-rw-r--r--   0 andras     (501) staff       (20)  1022852 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js
+-rw-r--r--   0 andras     (501) staff       (20)     5927 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.LICENSE.txt
+-rw-r--r--   0 andras     (501) staff       (20)  4266749 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.map
+-rw-r--r--   0 andras     (501) staff       (20)     5506 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js
+-rw-r--r--   0 andras     (501) staff       (20)    21943 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map
+-rw-r--r--   0 andras     (501) staff       (20)     1575 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js
+-rw-r--r--   0 andras     (501) staff       (20)     8288 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.147637 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/
+-rw-r--r--   0 andras     (501) staff       (20)   715890 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg
+-rw-r--r--   0 andras     (501) staff       (20)   132728 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf
+-rw-r--r--   0 andras     (501) staff       (20)    76612 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2
+-rw-r--r--   0 andras     (501) staff       (20)   133034 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot
+-rw-r--r--   0 andras     (501) staff       (20)    89824 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff
+-rw-r--r--   0 andras     (501) staff       (20)    34390 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot
+-rw-r--r--   0 andras     (501) staff       (20)   144322 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg
+-rw-r--r--   0 andras     (501) staff       (20)    13584 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2
+-rw-r--r--   0 andras     (501) staff       (20)    34092 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf
+-rw-r--r--   0 andras     (501) staff       (20)    16800 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff
+-rw-r--r--   0 andras     (501) staff       (20)   202616 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf
+-rw-r--r--   0 andras     (501) staff       (20)   202902 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot
+-rw-r--r--   0 andras     (501) staff       (20)    79444 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2
+-rw-r--r--   0 andras     (501) staff       (20)   103300 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff
+-rw-r--r--   0 andras     (501) staff       (20)   897426 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:16:50.110526 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component.egg-info/
+-rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 10:16:50.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component.egg-info/PKG-INFO
+-rw-r--r--   0 andras     (501) staff       (20)     3107 2023-06-05 10:16:50.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component.egg-info/SOURCES.txt
+-rw-r--r--   0 andras     (501) staff       (20)        1 2023-06-05 10:16:50.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component.egg-info/dependency_links.txt
+-rw-r--r--   0 andras     (501) staff       (20)       16 2023-06-05 10:16:50.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component.egg-info/requires.txt
+-rw-r--r--   0 andras     (501) staff       (20)       31 2023-06-05 10:16:50.000000 streamlit-d3-network-component-0.0.6/streamlit_d3_network_component.egg-info/top_level.txt
```

### Comparing `streamlit-d3-network-component-0.0.5/setup.py` & `streamlit-d3-network-component-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-d3-network-component",
-    version="0.0.5",
+    version="0.0.6",
     author="Andras Gyacsok",
     author_email="andras.gyacsok@boehringer-ingelheim.com",
     description="This package is a Streamlit custom component to represent network diagram using D3.js",
     long_description="This package is the custom Streamlit component to visualise network graphs using D3.js",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/__init__.py` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from pathlib import Path
 
 import streamlit.components.v1 as components
 import json
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
@@ -70,14 +69,15 @@
     return component_value
 
 
 # Add some test code to play with the component while it's in development.
 # During development, we can run this just as we would any other Streamlit
 # app: `$ streamlit run my_component/__init__.py`
 if not _RELEASE:
+    from pathlib import Path
     import streamlit as st
 
     st.set_page_config(layout="wide")
     st.subheader("Pathway")
 
     with open(Path(__file__).parent.joinpath('frontend/src/data/data.json'), 'r') as f:
         data_df = json.load(f)
```

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/asset-manifest.json` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/favicon.ico` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/index.html` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/logo192.png` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/logo192.png`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/logo512.png` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/logo512.png`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/precache-manifest.9a6cee5862e83e747d32a923936a576d.js` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/precache-manifest.9a6cee5862e83e747d32a923936a576d.js`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/service-worker.js` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.LICENSE.txt` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.map` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.5/streamlit_d3_network_component.egg-info/SOURCES.txt` & `streamlit-d3-network-component-0.0.6/streamlit_d3_network_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

