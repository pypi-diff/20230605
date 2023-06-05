# Comparing `tmp/autil-0.2.3.tar.gz` & `tmp/autil-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autil-0.2.3.tar", last modified: Fri May 19 17:33:58 2023, max compression
+gzip compressed data, was "autil-0.2.4.tar", max compression
```

## Comparing `autil-0.2.3.tar` & `autil-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      510 2022-04-25 12:36:00.308470 autil-0.2.3/autil/__init__.py
--rw-r--r--   0        0        0     1932 2023-05-19 17:17:27.828887 autil-0.2.3/autil/alt_plot.py
--rwxr-xr-x   0        0        0      937 2020-10-09 14:28:44.901723 autil-0.2.3/autil/country2continent.py
--rw-r--r--   0        0        0      782 2023-05-19 17:02:24.835613 autil-0.2.3/autil/io.py
--rw-r--r--   0        0        0     1124 2020-12-09 14:28:02.713989 autil-0.2.3/autil/io_download.py
--rw-r--r--   0        0        0      437 2022-07-07 18:34:54.917037 autil-0.2.3/autil/io_parquet.py
--rw-r--r--   0        0        0      336 2021-06-28 21:09:47.281261 autil-0.2.3/autil/ipy_addpath.py
--rwxr-xr-x   0        0        0     3798 2021-09-15 11:20:18.932676 autil-0.2.3/autil/ipy_displays.py
--rw-r--r--   0        0        0     1588 2020-11-28 09:51:40.919240 autil-0.2.3/autil/ipy_print.py
--rw-r--r--   0        0        0     1398 2022-01-21 13:51:44.810518 autil-0.2.3/autil/lm_lighten.py
--rw-r--r--   0        0        0     2164 2023-03-27 06:11:48.922951 autil-0.2.3/autil/mpl_plot.py
--rw-r--r--   0        0        0     6277 2022-07-03 21:43:07.837620 autil-0.2.3/autil/mpl_set.py
--rwxr-xr-x   0        0        0      971 2022-04-25 12:19:09.214814 autil-0.2.3/autil/owari.py
--rwxr-xr-x   0        0        0      393 2020-10-09 14:28:56.506532 autil-0.2.3/autil/pd_clean.py
--rw-r--r--   0        0        0      448 2022-12-12 06:25:01.443831 autil-0.2.3/autil/pd_perform.py
--rw-r--r--   0        0        0      988 2022-04-25 12:05:26.060654 autil-0.2.3/autil/pd_table.py
--rw-r--r--   0        0        0      203 2021-10-06 16:58:32.312882 autil-0.2.3/autil/print.py
--rw-r--r--   0        0        0     3372 2022-08-01 16:03:49.044363 autil-0.2.3/autil/scrape.py
--rw-r--r--   0        0        0     5194 2022-08-06 18:39:17.423544 autil-0.2.3/autil/scrape_proxy.py
--rw-r--r--   0        0        0     1102 2022-04-25 12:30:51.577437 autil-0.2.3/autil/sendmail.py
--rw-r--r--   0        0        0     4527 2022-04-25 12:10:11.910350 autil-0.2.3/autil/sk_metrics.py
--rw-r--r--   0        0        0     1791 2021-08-19 08:33:57.016179 autil-0.2.3/autil/sqlite.py
--rw-r--r--   0        0        0     3391 2019-11-17 12:31:48.420195 autil-0.2.3/autil/stat_summary.py
--rw-r--r--   0        0        0     3118 2022-12-09 08:05:51.189792 autil-0.2.3/autil/tex_table.py
--rw-r--r--   0        0        0      659 2022-04-25 12:31:44.528913 autil-0.2.3/autil/tr.py
--rw-r--r--   0        0        0     1452 2020-10-09 14:14:04.379726 autil-0.2.3/autil/z2h.py
--rw-r--r--   0        0        0      745 2023-05-19 17:18:45.482262 autil-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1132 2023-05-19 17:33:58.695172 autil-0.2.3/setup.py
--rw-r--r--   0        0        0     1098 2023-05-19 17:33:58.695445 autil-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      510 2022-04-25 12:36:00.308470 autil-0.2.4/autil/__init__.py
+-rw-r--r--   0        0        0     1932 2023-05-19 17:17:27.828887 autil-0.2.4/autil/alt_plot.py
+-rwxr-xr-x   0        0        0      937 2020-10-09 14:28:44.901723 autil-0.2.4/autil/country2continent.py
+-rw-r--r--   0        0        0      782 2023-05-19 17:02:24.835613 autil-0.2.4/autil/io.py
+-rw-r--r--   0        0        0     1124 2020-12-09 14:28:02.713989 autil-0.2.4/autil/io_download.py
+-rw-r--r--   0        0        0      437 2022-07-07 18:34:54.917037 autil-0.2.4/autil/io_parquet.py
+-rw-r--r--   0        0        0      336 2021-06-28 21:09:47.281261 autil-0.2.4/autil/ipy_addpath.py
+-rwxr-xr-x   0        0        0     3798 2021-09-15 11:20:18.932676 autil-0.2.4/autil/ipy_displays.py
+-rw-r--r--   0        0        0     1588 2020-11-28 09:51:40.919240 autil-0.2.4/autil/ipy_print.py
+-rw-r--r--   0        0        0     1398 2022-01-21 13:51:44.810518 autil-0.2.4/autil/lm_lighten.py
+-rw-r--r--   0        0        0     2164 2023-03-27 06:11:48.922951 autil-0.2.4/autil/mpl_plot.py
+-rw-r--r--   0        0        0     6277 2022-07-03 21:43:07.837620 autil-0.2.4/autil/mpl_set.py
+-rwxr-xr-x   0        0        0      971 2022-04-25 12:19:09.214814 autil-0.2.4/autil/owari.py
+-rwxr-xr-x   0        0        0      393 2020-10-09 14:28:56.506532 autil-0.2.4/autil/pd_clean.py
+-rw-r--r--   0        0        0      448 2022-12-12 06:25:01.443831 autil-0.2.4/autil/pd_perform.py
+-rw-r--r--   0        0        0      988 2022-04-25 12:05:26.060654 autil-0.2.4/autil/pd_table.py
+-rw-r--r--   0        0        0      203 2021-10-06 16:58:32.312882 autil-0.2.4/autil/print.py
+-rw-r--r--   0        0        0     3372 2022-08-01 16:03:49.044363 autil-0.2.4/autil/scrape.py
+-rw-r--r--   0        0        0     5194 2022-08-06 18:39:17.423544 autil-0.2.4/autil/scrape_proxy.py
+-rw-r--r--   0        0        0     1102 2022-04-25 12:30:51.577437 autil-0.2.4/autil/sendmail.py
+-rw-r--r--   0        0        0     4527 2022-04-25 12:10:11.910349 autil-0.2.4/autil/sk_metrics.py
+-rw-r--r--   0        0        0     1791 2021-08-19 08:33:57.016179 autil-0.2.4/autil/sqlite.py
+-rw-r--r--   0        0        0     3391 2019-11-17 12:31:48.420195 autil-0.2.4/autil/stat_summary.py
+-rw-r--r--   0        0        0     3118 2022-12-09 08:05:51.189792 autil-0.2.4/autil/tex_table.py
+-rw-r--r--   0        0        0      659 2022-04-25 12:31:44.528913 autil-0.2.4/autil/tr.py
+-rw-r--r--   0        0        0     1452 2020-10-09 14:14:04.379726 autil-0.2.4/autil/z2h.py
+-rw-r--r--   0        0        0      779 2023-06-05 20:11:38.382178 autil-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 autil-0.2.4/PKG-INFO
```

### Comparing `autil-0.2.3/autil/alt_plot.py` & `autil-0.2.4/autil/alt_plot.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/country2continent.py` & `autil-0.2.4/autil/country2continent.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/io.py` & `autil-0.2.4/autil/io.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/io_download.py` & `autil-0.2.4/autil/io_download.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/ipy_displays.py` & `autil-0.2.4/autil/ipy_displays.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/ipy_print.py` & `autil-0.2.4/autil/ipy_print.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/lm_lighten.py` & `autil-0.2.4/autil/lm_lighten.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/mpl_plot.py` & `autil-0.2.4/autil/mpl_plot.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/mpl_set.py` & `autil-0.2.4/autil/mpl_set.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/owari.py` & `autil-0.2.4/autil/owari.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/pd_table.py` & `autil-0.2.4/autil/pd_table.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/scrape.py` & `autil-0.2.4/autil/scrape.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/scrape_proxy.py` & `autil-0.2.4/autil/scrape_proxy.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/sendmail.py` & `autil-0.2.4/autil/sendmail.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/sk_metrics.py` & `autil-0.2.4/autil/sk_metrics.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/sqlite.py` & `autil-0.2.4/autil/sqlite.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/stat_summary.py` & `autil-0.2.4/autil/stat_summary.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/tex_table.py` & `autil-0.2.4/autil/tex_table.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/tr.py` & `autil-0.2.4/autil/tr.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/autil/z2h.py` & `autil-0.2.4/autil/z2h.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.3/pyproject.toml` & `autil-0.2.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 authors = ["alalalalaki <harlan.zhu@gmail.com>"]
 description = "Some Python snippets for a researcher's daily use"
 name = "autil"
-version = "0.2.3"
+version = "0.2.4"
 
 [tool.poetry.dependencies]
 adjustText = "^0.7.3"
 altair = "^4.1"
 country_converter = "^0.7.3"
 cycler = "^0.10"
 deepl = "^1.6.0"
 linearmodels = "^4.24"
 matplotlib = "^3.4"
+matplotlib-label-lines = "^0.5.1"
 numpy = "^1.21"
 pandas = "^1.3"
 pyarrow = "^5.0.0"
 pycountry_convert = "^0.7.2"
 python = "^3.8"
 requests = "^2.26"
 requests_html = "^0.10"
```

