# Comparing `tmp/FuncsForSPO-5.0.9.tar.gz` & `tmp/FuncsForSPO-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.0.9.tar", last modified: Fri Jun  2 21:42:53 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.1.0.tar", last modified: Mon Jun  5 14:59:31 2023, max compression
```

## Comparing `FuncsForSPO-5.0.9.tar` & `FuncsForSPO-5.1.0.tar`

### file list

```diff
@@ -1,66 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:53.236912 FuncsForSPO-5.0.9/
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.116380 FuncsForSPO-5.0.9/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.465901 FuncsForSPO-5.0.9/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.9/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.9/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.506791 FuncsForSPO-5.0.9/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.9/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.567129 FuncsForSPO-5.0.9/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.9/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.594154 FuncsForSPO-5.0.9/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.9/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.606627 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.650757 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     3908 2023-06-02 21:36:43.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3545 2023-06-02 20:31:43.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.683789 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.778184 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.788654 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.827205 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.845239 FuncsForSPO-5.0.9/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.864147 FuncsForSPO-5.0.9/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.9/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.970548 FuncsForSPO-5.0.9/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.9/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:53.014730 FuncsForSPO-5.0.9/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.9/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:53.047530 FuncsForSPO-5.0.9/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.9/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.9/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:53.067925 FuncsForSPO-5.0.9/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.9/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.9/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:53.081226 FuncsForSPO-5.0.9/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.9/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:42:52.377943 FuncsForSPO-5.0.9/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-02 21:42:50.000000 FuncsForSPO-5.0.9/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1520 2023-06-02 21:42:51.000000 FuncsForSPO-5.0.9/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 21:42:50.000000 FuncsForSPO-5.0.9/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-02 21:42:50.000000 FuncsForSPO-5.0.9/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      377 2023-06-02 21:42:50.000000 FuncsForSPO-5.0.9/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.9/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-02 21:42:53.231510 FuncsForSPO-5.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 21:42:53.236912 FuncsForSPO-5.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2297 2023-06-02 21:42:43.000000 FuncsForSPO-5.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.647494 FuncsForSPO-5.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.177224 FuncsForSPO-5.1.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.240824 FuncsForSPO-5.1.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.252688 FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.265527 FuncsForSPO-5.1.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.273525 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.277919 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.296923 FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.307039 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.355087 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     4228 2023-06-05 14:50:30.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3545 2023-06-05 13:10:09.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.410098 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.437160 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.447579 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.466444 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.481379 FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.494336 FuncsForSPO-5.1.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.509811 FuncsForSPO-5.1.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.521510 FuncsForSPO-5.1.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.1.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.537369 FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.550124 FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.559868 FuncsForSPO-5.1.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.228479 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1646 2023-06-05 14:59:31.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      432 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-05 14:59:31.640836 FuncsForSPO-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 14:59:31.648515 FuncsForSPO-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2421 2023-06-05 14:59:21.000000 FuncsForSPO-5.1.0/setup.py
```

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.1.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,33 +49,39 @@
             espera_elemento(self.WDW, (By.CSS_SELECTOR, 'input[type="file"]'), in_dom=True)
             self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.PDF_PATH)
             espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'div[class*="flex justify-between"]>button'))
 
 
             while True:
                 try:
-                    espera_input_limpa_e_envia_send_keys(self.WDW30, 'Coloque no inicio da sua resposta: "IA" e me responda em português. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]'))
+                    espera_input_limpa_e_envia_send_keys(self.WDW30, 'é de suma importância que você coloque no inicio da sua resposta: "IA" e me responda em português. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]'))
                     espera_elemento_disponivel_e_clica(self.WDW30, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]~button'))
                     break
                 except ElementClickInterceptedException:
                     try:
                         self.DRIVER.execute_script("arguments[0].remove();", self.DRIVER.find_element(By.CSS_SELECTOR, '#__NEXT_DATA__~ins'))
                     except Exception:
                         pass
-
-            while True:
+            
+            tentativas = 30
+            text = ''
+            while tentativas > 0:
                 faz_log('Aguardando resposta...')
                 text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, '#__next main>div~div>div~div>div>div>div>div~div'))
-                if 'IA' in text:
+                if 'IA' in text or 'sorry' in text.lower():
                     break
                 else:
+                    tentativas -= 1
                     sleep(2)
                     continue
             self.DRIVER.get('https://pdf.ai/documents')
             espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'a[href="/auth/account"]~button'))
+            sleep(2)
             self.DRIVER.quit()
+            if tentativas == 0:
+                raise ErroPDFAIException('Muitas tentativas, tente uma nova solicitação')
             return text
         except Exception as e:
             faz_log(repr(e), 'c*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
             self.DRIVER.quit()
             raise ErroPDFAIException
```

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files 9% similar despite different names*

```diff
@@ -1673,78 +1673,24 @@
         if (format_exit == '') or (format_exit is None) or (isinstance(format_exit, bool)):
             return data
         data_ = data.strftime(format_exit)
         return data_
 
 
 def remove_pontos_e_barras(string):
-    """Função remove esses elementos da string
-    
-    '.'
-    
-    '/'
-    
-    ','
-    
-    '-'
-    
-    '_'
-    
-    '='
-    
-    '|'
-    
-    '#'
-    
-    '`'
-    
-    '~'
-    
-    "'"
-    
-    '"'
-    
-    'string'.strip()
-    #### Função já converte o argumento para str()
+    """Remove caracteres especiais da string.
 
     Args:
-        string (str): str com os caracteres
+        string (str): String com os caracteres especiais.
 
     Returns:
-        str: Retorna string sem nenhum desses caracteres
+        str: String sem os caracteres especiais.
     """
-    string = str(string)
-    string = string.replace('.','')
-    string = string.replace('/', '')
-    string = string.replace(',', '')
-    string = string.replace('-', '')
-    string = string.replace('_', '')
-    string = string.replace('=', '')
-    string = string.replace('|', '')
-    string = string.replace('`', '')
-    string = string.replace('~', '')
-    string = string.replace("'", '')
-    string = string.replace('"', '')
-    string = string.replace('#', '')
-    string = string.replace(';', '')
-    string = string.replace(':', '')
-    string = string.replace('@', '')
-    string = string.replace('!', '')
-    string = string.replace('(', '')
-    string = string.replace(')', '')
-    string = string.replace('$', '')
-    string = string.replace('%', '')
-    string = string.replace('+', '')
-    string = string.replace('&', '')
-    string = string.replace('^', '')
-    string = string.replace('*', '')
-    string = string.replace('{', '')
-    string = string.replace('}', '')
-    string = string.replace('[', '')
-    string = string.replace(']', '')
+    special_chars = r'[./,_=\|`~\'"#;:@!()\$%+&^\*\{\}\[\]\\]'
+    string = re.sub(special_chars, '', str(string))
     string = string.strip()
     return string
 
 
 def remove_duplicados_na_lista(iteravel:list|tuple, convert_str:bool=False):
     """Remove duplicados de uma lista
```

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.1.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.1.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.9
+Version: 5.1.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.9/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.1.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 FuncsForSPO.egg-info/top_level.txt
 FuncsForSPO/femails/__init__.py
 FuncsForSPO/femails/femails.py
 FuncsForSPO/fexceptions/__init__.py
 FuncsForSPO/fexceptions/exceptions.py
 FuncsForSPO/fftp/__init__.py
 FuncsForSPO/fftp/fftp.py
+FuncsForSPO/flanguage/__init__.py
+FuncsForSPO/flanguage/translator/__init__.py
+FuncsForSPO/flanguage/translator/translator.py
 FuncsForSPO/fopenpyxl/__init__.py
 FuncsForSPO/fopenpyxl/openpyxl_funcs.py
 FuncsForSPO/fpdf/__init__.py
 FuncsForSPO/fpdf/fanalyser/__init__.py
 FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
 FuncsForSPO/fpdf/fanalyser/base.py
 FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
```

### Comparing `FuncsForSPO-5.0.9/LICENSE` & `FuncsForSPO-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/PKG-INFO` & `FuncsForSPO-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.9
+Version: 5.1.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.9/README.md` & `FuncsForSPO-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.9/setup.py` & `FuncsForSPO-5.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.0.9'
+version = '5.1.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -17,14 +17,16 @@
         keywords='Funções Para Melhorar Desenvolvimento de Robôs com Selenium',
         description=u'Funções Para Melhorar Desenvolvimento de Robôs com Selenium',
         
         packages= [
             os.path.join('FuncsForSPO', 'femails'),
             os.path.join('FuncsForSPO', 'fexceptions'),
             os.path.join('FuncsForSPO', 'fftp'),
+            os.path.join('FuncsForSPO', 'flanguage'),
+            os.path.join('FuncsForSPO', 'flanguage', 'translator'),
             os.path.join('FuncsForSPO', 'fpdf'),
             os.path.join('FuncsForSPO', 'fpdf', 'focr'),
             os.path.join('FuncsForSPO', 'fpdf', 'focr'),
             os.path.join('FuncsForSPO', 'fpdf', 'fcompress'),
             os.path.join('FuncsForSPO', 'fpdf', 'fimgpdf'),
             os.path.join('FuncsForSPO', 'fpdf', 'fanalyser'),
             os.path.join('FuncsForSPO', 'fpdf', 'fhtml_to_pdf'),
```

