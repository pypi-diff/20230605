# Comparing `tmp/FuncsForSPO-5.1.0.tar.gz` & `tmp/FuncsForSPO-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.1.0.tar", last modified: Mon Jun  5 14:59:31 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.1.1.tar", last modified: Mon Jun  5 16:02:00 2023, max compression
```

## Comparing `FuncsForSPO-5.1.0.tar` & `FuncsForSPO-5.1.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.647494 FuncsForSPO-5.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.177224 FuncsForSPO-5.1.0/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.240824 FuncsForSPO-5.1.0/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.0/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.0/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.252688 FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.265527 FuncsForSPO-5.1.0/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.0/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.273525 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.277919 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.0/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.296923 FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.307039 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.355087 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     4228 2023-06-05 14:50:30.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3545 2023-06-05 13:10:09.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.410098 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.437160 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.447579 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.466444 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.481379 FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.494336 FuncsForSPO-5.1.0/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.0/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.509811 FuncsForSPO-5.1.0/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.0/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.521510 FuncsForSPO-5.1.0/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.1.0/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.537369 FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.550124 FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.559868 FuncsForSPO-5.1.0/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.0/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:59:31.228479 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1646 2023-06-05 14:59:31.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      432 2023-06-05 14:59:30.000000 FuncsForSPO-5.1.0/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.0/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-05 14:59:31.640836 FuncsForSPO-5.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 14:59:31.648515 FuncsForSPO-5.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2421 2023-06-05 14:59:21.000000 FuncsForSPO-5.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:02:00.291216 FuncsForSPO-5.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.517506 FuncsForSPO-5.1.1/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.830084 FuncsForSPO-5.1.1/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.1/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.1/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.873133 FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.906080 FuncsForSPO-5.1.1/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.1/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.986463 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.024988 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.064706 FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.090091 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.204043 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     4247 2023-06-05 16:01:34.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3545 2023-06-05 13:10:09.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.266928 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.340003 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.368130 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.434177 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.526001 FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.567269 FuncsForSPO-5.1.1/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.1/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.632407 FuncsForSPO-5.1.1/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.1/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.713592 FuncsForSPO-5.1.1/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.1.1/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.758067 FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.787678 FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:59.824372 FuncsForSPO-5.1.1/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.1/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:01:58.780470 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1646 2023-06-05 16:01:58.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      432 2023-06-05 16:01:57.000000 FuncsForSPO-5.1.1/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-05 16:02:00.202861 FuncsForSPO-5.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:02:00.296825 FuncsForSPO-5.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2421 2023-06-05 16:01:41.000000 FuncsForSPO-5.1.1/setup.py
```

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.1.1/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-5.1.1/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,20 +58,20 @@
                     break
                 except ElementClickInterceptedException:
                     try:
                         self.DRIVER.execute_script("arguments[0].remove();", self.DRIVER.find_element(By.CSS_SELECTOR, '#__NEXT_DATA__~ins'))
                     except Exception:
                         pass
             
-            tentativas = 30
+            tentativas = 10
             text = ''
             while tentativas > 0:
                 faz_log('Aguardando resposta...')
                 text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, '#__next main>div~div>div~div>div>div>div>div~div'))
-                if 'IA' in text or 'sorry' in text.lower():
+                if 'IA' in text or 'sorry' in text.lower() or tentativas == 1:
                     break
                 else:
                     tentativas -= 1
                     sleep(2)
                     continue
             self.DRIVER.get('https://pdf.ai/documents')
             espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'a[href="/auth/account"]~button'))
```

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.1.1/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.1.1/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.1.1/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.0
+Version: 5.1.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.0/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.1.1/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/LICENSE` & `FuncsForSPO-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/PKG-INFO` & `FuncsForSPO-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.0
+Version: 5.1.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.0/README.md` & `FuncsForSPO-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.0/setup.py` & `FuncsForSPO-5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.1.0'
+version = '5.1.1'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

