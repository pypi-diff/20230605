# Comparing `tmp/absfuyu-1.6.0.tar.gz` & `tmp/absfuyu-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\tmpp39rjox7\absfuyu-1.6.0.tar", last modified: Sat Jun 11 13:30:29 2022, max compression
+gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-011s6zg4\absfuyu-2.0.0.tar", last modified: Mon Jun  5 17:18:25 2023, max compression
```

## Comparing `absfuyu-1.6.0.tar` & `absfuyu-2.0.0.tar`

### file list

```diff
@@ -1,79 +1,109 @@
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:29.000000 absfuyu-1.6.0/
--rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-1.6.0/LICENSE
--rw-rw-rw-   0        0        0      189 2022-02-16 17:39:44.000000 absfuyu-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3718 2022-06-11 13:30:29.000000 absfuyu-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-1.6.0/README.md
--rw-rw-rw-   0        0        0     1015 2022-03-15 09:00:24.000000 absfuyu-1.6.0/extra_requirements.txt
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/images/
--rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-1.6.0/images/repository-image-crop.png
--rw-rw-rw-   0        0        0      171 2022-02-16 17:39:44.000000 absfuyu-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-1.6.0/requirements.txt
--rw-rw-rw-   0        0        0     1360 2022-06-11 13:30:29.000000 absfuyu-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1002 2022-02-16 17:39:44.000000 absfuyu-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu/
--rw-rw-rw-   0        0        0     1105 2022-03-07 17:47:18.000000 absfuyu-1.6.0/src/absfuyu/__init__.py
--rw-rw-rw-   0        0        0     8189 2022-03-07 17:18:33.000000 absfuyu-1.6.0/src/absfuyu/__main__.py
--rw-rw-rw-   0        0        0     7379 2022-02-18 12:51:43.000000 absfuyu-1.6.0/src/absfuyu/calculation.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu/code_red/
--rw-rw-rw-   0        0        0     5580 2022-02-17 09:30:21.000000 absfuyu-1.6.0/src/absfuyu/code_red/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu/config/
--rw-rw-rw-   0        0        0     4182 2022-02-27 13:18:36.000000 absfuyu-1.6.0/src/absfuyu/config/__init__.py
--rw-rw-rw-   0        0        0      791 2022-06-11 13:30:12.000000 absfuyu-1.6.0/src/absfuyu/config/config.json
--rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-1.6.0/src/absfuyu/config/template.json
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu/contrib/
--rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-1.6.0/src/absfuyu/contrib/__init__.py
--rw-rw-rw-   0        0        0     7899 2022-02-19 16:47:12.000000 absfuyu-1.6.0/src/absfuyu/contrib/basic_lunar_calendar.py
--rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-1.6.0/src/absfuyu/contrib/color_extract.py
--rw-rw-rw-   0        0        0     3580 2022-03-07 17:30:55.000000 absfuyu-1.6.0/src/absfuyu/core.py
--rw-rw-rw-   0        0        0     3028 2022-02-16 17:39:44.000000 absfuyu-1.6.0/src/absfuyu/data.py
--rw-rw-rw-   0        0        0     2113 2022-02-25 06:31:13.000000 absfuyu-1.6.0/src/absfuyu/dicts.py
--rw-rw-rw-   0        0        0      950 2022-03-07 16:45:18.000000 absfuyu-1.6.0/src/absfuyu/everything.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu/extensions/
--rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-1.6.0/src/absfuyu/extensions/__init__.py
--rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-1.6.0/src/absfuyu/extensions/beautiful.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:29.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/
--rw-rw-rw-   0        0        0    12666 2022-03-11 16:00:09.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/WGS.py
--rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/__init__.py
--rw-rw-rw-   0        0        0      456 2022-02-14 17:36:30.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/_make_dat.py
--rw-rw-rw-   0        0        0      395 2022-02-18 04:12:55.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/load_data.py
--rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/password_hash.py
--rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/pkglib.py
--rw-rw-rw-   0        0        0    23305 2022-01-29 15:58:34.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/prime.dat
--rw-rw-rw-   0        0        0    14546 2022-06-11 13:29:04.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/primo_cal.py
--rw-rw-rw-   0        0        0     7203 2022-03-01 10:50:50.000000 absfuyu-1.6.0/src/absfuyu/extensions/dev/sudoku.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:29.000000 absfuyu-1.6.0/src/absfuyu/extensions/extra/
--rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-1.6.0/src/absfuyu/extensions/extra/__init__.py
--rw-rw-rw-   0        0        0     5231 2022-03-16 06:58:59.000000 absfuyu-1.6.0/src/absfuyu/extensions/extra/data_analysis.py
--rw-rw-rw-   0        0        0     1590 2022-02-14 17:36:30.000000 absfuyu-1.6.0/src/absfuyu/fibonacci.py
--rw-rw-rw-   0        0        0     5759 2022-03-04 00:37:37.000000 absfuyu-1.6.0/src/absfuyu/fun.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:29.000000 absfuyu-1.6.0/src/absfuyu/game/
--rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-1.6.0/src/absfuyu/game/__init__.py
--rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-1.6.0/src/absfuyu/game/tictactoe.py
--rw-rw-rw-   0        0        0     5343 2022-02-16 17:39:44.000000 absfuyu-1.6.0/src/absfuyu/generator.py
--rw-rw-rw-   0        0        0     2236 2022-03-07 16:39:19.000000 absfuyu-1.6.0/src/absfuyu/help.py
--rw-rw-rw-   0        0        0     2203 2022-02-16 17:39:09.000000 absfuyu-1.6.0/src/absfuyu/lists.py
--rw-rw-rw-   0        0        0    10786 2022-02-16 17:39:44.000000 absfuyu-1.6.0/src/absfuyu/obfuscator.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:29.000000 absfuyu-1.6.0/src/absfuyu/pkg_data/
--rw-rw-rw-   0        0        0      930 2022-02-14 17:36:30.000000 absfuyu-1.6.0/src/absfuyu/pkg_data/__init__.py
--rw-rw-rw-   0        0        0        0 2022-01-29 17:00:32.000000 absfuyu-1.6.0/src/absfuyu/pkg_data/dummy.dat
--rw-rw-rw-   0        0        0       31 2022-02-03 13:01:43.000000 absfuyu-1.6.0/src/absfuyu/pkg_data/punishment_windows.dat
--rw-rw-rw-   0        0        0      704 2022-02-16 17:39:09.000000 absfuyu-1.6.0/src/absfuyu/pry.py
--rw-rw-rw-   0        0        0     3070 2022-02-16 17:39:09.000000 absfuyu-1.6.0/src/absfuyu/sort.py
--rw-rw-rw-   0        0        0     3428 2022-03-16 06:39:33.000000 absfuyu-1.6.0/src/absfuyu/stats.py
--rw-rw-rw-   0        0        0     6993 2022-02-18 13:03:05.000000 absfuyu-1.6.0/src/absfuyu/strings.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:29.000000 absfuyu-1.6.0/src/absfuyu/tools/
--rw-rw-rw-   0        0        0      116 2022-03-07 17:02:01.000000 absfuyu-1.6.0/src/absfuyu/tools/__init__.py
--rw-rw-rw-   0        0        0     9264 2022-03-07 17:43:52.000000 absfuyu-1.6.0/src/absfuyu/tools/keygen.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:29.000000 absfuyu-1.6.0/src/absfuyu/tools/short_link/
--rw-rw-rw-   0        0        0      150 2022-03-07 17:01:51.000000 absfuyu-1.6.0/src/absfuyu/tools/short_link/__init__.py
--rw-rw-rw-   0        0        0     5069 2022-03-07 17:01:43.000000 absfuyu-1.6.0/src/absfuyu/tools/short_link/rebrandly.py
--rw-rw-rw-   0        0        0     4698 2022-03-01 10:58:55.000000 absfuyu-1.6.0/src/absfuyu/util.py
--rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-1.6.0/src/absfuyu/version.py
-drwxrwxrwx   0        0        0        0 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu.egg-info/
--rw-rw-rw-   0        0        0     3718 2022-06-11 13:30:27.000000 absfuyu-1.6.0/src/absfuyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-11 13:30:27.000000 absfuyu-1.6.0/src/absfuyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1039 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-06-11 13:30:28.000000 absfuyu-1.6.0/src/absfuyu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/
+-rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3836 2023-06-05 17:18:25.000000 absfuyu-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1161 2023-05-24 23:25:15.000000 absfuyu-2.0.0/extra_requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:24.000000 absfuyu-2.0.0/images/
+-rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.0.0/images/repository-image-crop.png
+-rw-rw-rw-   0        0        0      193 2023-06-05 17:18:06.000000 absfuyu-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0     1360 2023-06-05 17:18:25.000000 absfuyu-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/
+-rw-rw-rw-   0        0        0     1004 2023-06-05 10:10:40.000000 absfuyu-2.0.0/src/absfuyu/__init__.py
+-rw-rw-rw-   0        0        0     6530 2023-06-05 10:08:56.000000 absfuyu-2.0.0/src/absfuyu/__main__.py
+-rw-rw-rw-   0        0        0     2566 2023-06-04 16:54:26.000000 absfuyu-2.0.0/src/absfuyu/calculation.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/code_red/
+-rw-rw-rw-   0        0        0     5580 2022-02-17 09:30:21.000000 absfuyu-2.0.0/src/absfuyu/code_red/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/collections/
+-rw-rw-rw-   0        0        0     1264 2023-05-25 00:03:43.000000 absfuyu-2.0.0/src/absfuyu/collections/__init__.py
+-rw-rw-rw-   0        0        0    14620 2023-05-24 23:35:16.000000 absfuyu-2.0.0/src/absfuyu/collections/content.py
+-rw-rw-rw-   0        0        0    20344 2023-06-05 09:59:00.000000 absfuyu-2.0.0/src/absfuyu/collections/data_extension.py
+-rw-rw-rw-   0        0        0     6742 2023-06-05 14:26:41.000000 absfuyu-2.0.0/src/absfuyu/collections/generator.py
+-rw-rw-rw-   0        0        0     5822 2023-05-24 23:57:55.000000 absfuyu-2.0.0/src/absfuyu/collections/human.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/config/
+-rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/config/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-05 17:18:13.000000 absfuyu-2.0.0/src/absfuyu/config/config.json
+-rw-rw-rw-   0        0        0     1555 2023-05-24 23:30:58.000000 absfuyu-2.0.0/src/absfuyu/config/config2.py
+-rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.0.0/src/absfuyu/config/template.json
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/contrib/
+-rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.0.0/src/absfuyu/contrib/__init__.py
+-rw-rw-rw-   0        0        0     8190 2023-05-25 00:27:41.000000 absfuyu-2.0.0/src/absfuyu/contrib/basic_lunar_calendar.py
+-rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.0.0/src/absfuyu/contrib/color_extract.py
+-rw-rw-rw-   0        0        0     3313 2023-06-05 09:42:30.000000 absfuyu-2.0.0/src/absfuyu/core.py
+-rw-rw-rw-   0        0        0      832 2023-06-05 10:09:19.000000 absfuyu-2.0.0/src/absfuyu/everything.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/
+-rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.0.0/src/absfuyu/extensions/__init__.py
+-rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.0.0/src/absfuyu/extensions/beautiful.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/
+-rw-rw-rw-   0        0        0    11971 2023-06-05 17:02:34.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/WGS.py
+-rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/__init__.py
+-rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/horoscope.py
+-rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/password_hash.py
+-rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/pkglib.py
+-rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/primo_cal.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/
+-rw-rw-rw-   0        0        0      150 2022-03-07 17:01:51.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/__init__.py
+-rw-rw-rw-   0        0        0     5069 2022-03-07 17:01:43.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/rebrandly.py
+-rw-rw-rw-   0        0        0     2775 2023-06-04 19:15:00.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/tarot.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/extra/
+-rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.0.0/src/absfuyu/extensions/extra/__init__.py
+-rw-rw-rw-   0        0        0     6812 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/extensions/extra/data_analysis.py
+-rw-rw-rw-   0        0        0     6001 2023-06-04 17:07:41.000000 absfuyu-2.0.0/src/absfuyu/fun.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/game/
+-rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.0.0/src/absfuyu/game/__init__.py
+-rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/game/sudoku.py
+-rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.0.0/src/absfuyu/game/tictactoe.py
+-rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/game/wordle.py
+-rw-rw-rw-   0        0        0     3612 2023-05-25 00:07:58.000000 absfuyu-2.0.0/src/absfuyu/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/
+-rw-rw-rw-   0        0        0     3043 2023-06-04 18:25:52.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/__init__.py
+-rw-rw-rw-   0        0        0   247094 2023-05-27 07:47:21.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/chemistry.json
+-rw-rw-rw-   0        0        0        0 2022-01-29 17:00:32.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/dummy.dat
+-rw-rw-rw-   0        0        0       31 2022-02-03 13:01:43.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/punishment_windows.dat
+-rw-rw-rw-   0        0        0    86614 2023-06-04 18:47:18.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/tarot.json
+-rw-rw-rw-   0        0        0     5882 2023-05-27 10:46:34.000000 absfuyu-2.0.0/src/absfuyu/sort.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/tools/
+-rw-rw-rw-   0        0        0      136 2023-05-26 15:55:24.000000 absfuyu-2.0.0/src/absfuyu/tools/__init__.py
+-rw-rw-rw-   0        0        0     5853 2023-06-05 17:07:39.000000 absfuyu-2.0.0/src/absfuyu/tools/converter.py
+-rw-rw-rw-   0        0        0     9264 2023-02-16 09:21:06.000000 absfuyu-2.0.0/src/absfuyu/tools/keygen.py
+-rw-rw-rw-   0        0        0     8482 2023-06-05 09:33:57.000000 absfuyu-2.0.0/src/absfuyu/tools/obfuscator.py
+-rw-rw-rw-   0        0        0     3008 2023-06-05 10:41:12.000000 absfuyu-2.0.0/src/absfuyu/tools/stats.py
+-rw-rw-rw-   0        0        0     1180 2023-05-27 10:43:07.000000 absfuyu-2.0.0/src/absfuyu/tools/web.py
+-rw-rw-rw-   0        0        0    12499 2023-06-05 10:13:07.000000 absfuyu-2.0.0/src/absfuyu/unused.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/util/
+-rw-rw-rw-   0        0        0     2358 2023-06-05 15:57:31.000000 absfuyu-2.0.0/src/absfuyu/util/__init__.py
+-rw-rw-rw-   0        0        0     2769 2023-05-27 10:21:24.000000 absfuyu-2.0.0/src/absfuyu/util/api.py
+-rw-rw-rw-   0        0        0     2366 2023-05-27 10:30:03.000000 absfuyu-2.0.0/src/absfuyu/util/json_method.py
+-rw-rw-rw-   0        0        0     5605 2023-05-27 10:34:09.000000 absfuyu-2.0.0/src/absfuyu/util/path.py
+-rw-rw-rw-   0        0        0     3829 2023-05-27 10:38:41.000000 absfuyu-2.0.0/src/absfuyu/util/performance.py
+-rw-rw-rw-   0        0        0     2499 2023-05-27 19:37:56.000000 absfuyu-2.0.0/src/absfuyu/util/zipped.py
+-rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.0.0/src/absfuyu/version.py
+-rw-rw-rw-   0        0        0     9951 2023-06-05 14:44:21.000000 absfuyu-2.0.0/src/absfuyu/version2.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu.egg-info/
+-rw-rw-rw-   0        0        0     3836 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2591 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1266 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/tests/
+-rw-rw-rw-   0        0        0      805 2023-05-25 06:54:29.000000 absfuyu-2.0.0/tests/test_DictKai.py
+-rw-rw-rw-   0        0        0     2941 2023-05-26 16:32:44.000000 absfuyu-2.0.0/tests/test_Generator.py
+-rw-rw-rw-   0        0        0     3206 2023-06-05 06:47:06.000000 absfuyu-2.0.0/tests/test_IntNumber.py
+-rw-rw-rw-   0        0        0     2068 2023-05-25 04:14:43.000000 absfuyu-2.0.0/tests/test_ListKai.py
+-rw-rw-rw-   0        0        0     3246 2023-06-05 09:58:53.000000 absfuyu-2.0.0/tests/test_Text.py
+-rw-rw-rw-   0        0        0      632 2023-05-27 19:12:16.000000 absfuyu-2.0.0/tests/test_api.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.0.0/tests/test_beautiful.py
+-rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.0.0/tests/test_config.py
+-rw-rw-rw-   0        0        0      769 2023-05-27 10:06:18.000000 absfuyu-2.0.0/tests/test_converter.py
+-rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.0.0/tests/test_everything.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.0.0/tests/test_extensions.py
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.0.0/tests/test_fun.py
+-rw-rw-rw-   0        0        0      425 2023-05-27 19:15:29.000000 absfuyu-2.0.0/tests/test_json_method.py
+-rw-rw-rw-   0        0        0      706 2023-06-05 09:45:00.000000 absfuyu-2.0.0/tests/test_obfuscator.py
+-rw-rw-rw-   0        0        0      649 2023-05-27 18:57:56.000000 absfuyu-2.0.0/tests/test_path.py
+-rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.0.0/tests/test_pkg_data.py
+-rw-rw-rw-   0        0        0     1133 2023-06-05 15:55:36.000000 absfuyu-2.0.0/tests/test_util.py
```

### Comparing `absfuyu-1.6.0/LICENSE` & `absfuyu-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/PKG-INFO` & `absfuyu-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 1.6.0
+Version: 2.0.0
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -18,40 +18,44 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: rich
 Provides-Extra: beautiful
-Provides-Extra: dev
+Provides-Extra: cli
 Provides-Extra: click
 Provides-Extra: extra
-Provides-Extra: cli
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
 Provides-Extra: pipx
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: fixers
 Provides-Extra: autoimport
+Provides-Extra: fixers
 Provides-Extra: black
-Provides-Extra: test
 Provides-Extra: pytest
+Provides-Extra: test
 Provides-Extra: tox
+Provides-Extra: sphinx
+Provides-Extra: sphinx_rtd_theme
+Provides-Extra: python-dateutil
+Provides-Extra: unidecode
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 	<h1 align="center">
 		<img src="https://github.com/AbsoluteWinter/AbsoluteWinter.github.io/blob/main/absfuyu/images/repository-image-crop.png?raw=true" alt="absfuyu"/>
 	</h1>
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 1.6.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.0.0 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown Provides-Extra: rich Provides-Extra:
-beautiful Provides-Extra: dev Provides-Extra: click Provides-Extra: extra
-Provides-Extra: cli Provides-Extra: colorama Provides-Extra: build Provides-
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+rich Provides-Extra: beautiful Provides-Extra: cli Provides-Extra: click
+Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: test
-Provides-Extra: pytest Provides-Extra: tox Provides-Extra: all License-File:
-LICENSE
+autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
+Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
+sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
+Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
 $ pip install -U absfuyu ``` ## **USAGE:** ```python import absfuyu
 absfuyu.help() ``` ## **DOCUMENTATION:** > [here](https://
 absolutewinter.github.io/absfuyu/) ## **LICENSE:** ``` MIT License Copyright
```

### Comparing `absfuyu-1.6.0/README.md` & `absfuyu-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/extra_requirements.txt` & `absfuyu-2.0.0/extra_requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # sortedcontainers:         future
 # alive-progress:           future
 # opencv-python:            extract-color
 # scikit-learn:             extract-color
 # numpy 1.12.5; pandas 1.3.5; matplotlib 3.5.1
 
 
-rich:                       beautiful
+rich:                       beautiful, dev
 click>=8.0.0:               cli, dev, extra
 colorama>=0.4:              cli, dev, extra
 build:                      dev
 twine>=3.7.1:               dev
 virtualenv>=20.13.0:        dev
 setuptools>=51.0.0:         dev
 wheel:                      dev
@@ -24,8 +24,12 @@
 pandas:                     extra
 matplotlib:                 extra
 scipy:                      extra
 LunarCalendar>=0.0.9:       extra
 autoimport:                 fixers
 black>=22.1.0:              fixers
 pytest>=6.2.5:              test, dev
-tox>=3.24.5:                test
+tox>=3.24.5:                test
+sphinx:                     dev
+sphinx_rtd_theme:           dev
+python-dateutil:            extra
+unidecode:                  extra, dev
```

### Comparing `absfuyu-1.6.0/images/repository-image-crop.png` & `absfuyu-2.0.0/images/repository-image-crop.png`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/setup.cfg` & `absfuyu-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/setup.py` & `absfuyu-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,12 +26,12 @@
             extra_deps['all'] = set(vv for v in extra_deps.values() for vv in v)
 
     return extra_deps
 
 setuptools.setup(
     name="absfuyu",
     extras_require=get_extra_requires("extra_requirements.txt"),
-    package_data={"": ["dev/*.dat","pkg_data/*","config/*"]},
+    package_data={"": ["extensions/dev/*","pkg_data/*","config/*"]},
     exclude_package_data={
         "": ["tempCodeRunnerFile.py"],
     },
 )
```

### Comparing `absfuyu-1.6.0/src/absfuyu/__init__.py` & `absfuyu-2.0.0/src/absfuyu/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 """
 ABSFUYU
--------
+---
 A small collection of code
 
 LINKS
------
+---
 - Home page: https://pypi.org/project/absfuyu/
 - Documentation: https://absolutewinter.github.io/absfuyu/
 
 USAGE
------
+---
 `import absfuyu`
-
-`absfuyu.help()`
 """
 
 
+# Module level
+###########################################################################
 __title__ = "absfuyu"
 __author__ = "AbsoluteWinter"
 __license__ = "MIT License"
 __all__ = [
     # default
-    "calculation", "data", "generator",
-    "strings", "util", "lists",
+    "calculation", "util",
     # extra
-    "fibonacci", "obfuscator", "sort", "fun",
-    "stats", "pkg_data", "extra", "dicts",
+    "sort", "fun",
+    "pkg_data",
     "game", "tools", "extensions",
     # config
     "config",
     # Other
-    # "help", "pry", "version",
-    # "everything",
+    "version",
+    "everything",
 ]
 
+
+# Library
+###########################################################################
 # default function
-from .help import *
-from .pry import *
 from .version import __version__
 from .version import check_for_update
 
 
 # default module
 from . import calculation as cal
-from . import data
-from . import generator as gen
-from . import lists
-from . import strings
 from . import util
 
 
 # config
 # from . import config as __config
 # __config.welcome()
```

### Comparing `absfuyu-1.6.0/src/absfuyu/__main__.py` & `absfuyu-2.0.0/src/absfuyu/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ABSFUYU
 -------
 COMMAND LINE INTERFACE
 """
 
 
 # Library
-##############################################################
+###########################################################################
 from random import choice as __randc
 from subprocess import run as __run
 
 CLI_MODE = False
 try:
     import click as __click
     import colorama as __colorama
@@ -32,32 +32,31 @@
     reset_cfg as __reset,
     welcome as __welcome,
     toggle_setting as __togg,
 )
 
 from . import core as __core
 from . import version as __v
-from .generator import randStrGen as __randStr
 
 
 
 
 # Color stuff
-##############################################################
+###########################################################################
 if CLI_MODE:
     if __colorama is not None:
         __colorama.init(autoreset=True)
         __COLOR = __core.Color
     else:
         __COLOR = {"green":"", "blue":"", "red":"", "yellow":"", "reset":""}
 
 
 
 # Main group
-##############################################################
+###########################################################################
 @__click.command()
 def welcome():
     """Welcome message"""
     import os as __os
     try:
         user = __os.getlogin()
     except:
@@ -106,30 +105,15 @@
 def version():
     """Check current version"""
     __click.echo(f"{__COLOR['green']}absfuyu: {__v.__version__}")
 
 
 
 # Do group
-##############################################################
-@__click.command(name="gen-pass")
-@__click.argument("size", type=int, default=8)
-@__click.option(
-    "--password_type", "-p",
-    type=__click.Choice(["default","full"], case_sensitive=False),
-    default="full", show_default=True,
-    help="default: [a-zA-Z0-9] | full: [a-zA-Z0-9] + special char")
-def gen_password(size, password_type):
-    """Generate password of choice"""
-    __click.echo(__randStr(
-        size=size,
-        char=password_type,
-        string_type_if_1=True))
-
-
+###########################################################################
 @__click.command()
 @__click.option(
     "--force_update/--no-force-update", "-F/-f", "force_update",
     type=bool, default=True,
     show_default=True,
     help="Update the package")
 def update(force_update: bool):
@@ -222,73 +206,34 @@
 def advice():
     """Give some recommendation when bored"""
     from .fun import im_bored
     __click.echo(f"{__COLOR['green']}{im_bored()}")
     pass
 
 
-@__click.command(name="slink")
-@__click.argument("destination",type=str)
-@__click.option(
-    "--slash-tag", "-s", "slash_tag",
-    type=str, default=None,
-    help="Custom shortlink name")
-@__click.option(
-    "--title", "-t", "title",
-    type=str, default=None,
-    help="Title of link")
-@__click.option(
-    "--domain", "-d", "domain",
-    type=str, default=None,
-    help="Domain (if any) [Default: Rebrand.ly]")
-@__click.option(
-    "--api", "-a", "api",
-    type=str, default=None,
-    help="User's API key")
-@__click.option(
-    "--workspace", "-w", "workspace",
-    type=str, default=None,
-    help="User's Workspace ID")
-@__click.option(
-    "--trace/--no-trace", "-T/-N", "no_trace",
-    type=bool, default=True,
-    show_default=True,
-    help="Reset API every run")
-def shortlink(
-        destination, slash_tag,
-        title, domain, api, workspace,
-        no_trace,
-    ):
-    """Short link with Rebrandly's API"""
-    from .tools import short_link
-    short_link.short_link(
-        destination=destination, slash_tag=slash_tag,
-        title=title, domain=domain, api=api, workspace=workspace,
-        no_trace=no_trace,
-    )
-    pass
+
 
 
 
 @__click.group(name="do")
 def do_group():
     """Perform functinalities"""
     pass
-do_group.add_command(gen_password)
+
 do_group.add_command(reset)
 do_group.add_command(update)
 do_group.add_command(game)
 do_group.add_command(install)
 do_group.add_command(advice)
-do_group.add_command(shortlink)
+
 
 
 
 # Main group init
-##############################################################
+###########################################################################
 @__click.group()
 def main():
     """
     absfuyu's command line interface
     
     Usage:
         python -m absfuyu --help
@@ -298,10 +243,12 @@
 main.add_command(welcome)
 main.add_command(greet)
 main.add_command(toggle)
 main.add_command(version)
 main.add_command(do_group)
 
 
+# Run
+###########################################################################
 if __name__ == "__main__":
     if CLI_MODE:
         main()
```

### Comparing `absfuyu-1.6.0/src/absfuyu/code_red/__init__.py` & `absfuyu-2.0.0/src/absfuyu/code_red/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/config/__init__.py` & `absfuyu-2.0.0/src/absfuyu/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import Any as __Any
 
 
 
 # Define
 ##############################################################
 __here = __os.path.abspath(__os.path.dirname(__file__))
+CONFIG_LOC = __os.path.join(__here, "config.json")
 __config_name = "config"
 __config_template = """\
 {
     "setting": {
         "temp": {
             "default": null,
             "help": null,
```

### Comparing `absfuyu-1.6.0/src/absfuyu/config/config.json` & `absfuyu-2.0.0/src/absfuyu/config/template.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "{'minor': 1, 'patch': 4}"}*

```diff
@@ -19,13 +19,13 @@
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
         "major": 1,
-        "minor": 6,
-        "patch": 0,
+        "minor": 1,
+        "patch": 4,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-1.6.0/src/absfuyu/contrib/basic_lunar_calendar.py` & `absfuyu-2.0.0/src/absfuyu/contrib/basic_lunar_calendar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-'''
+"""
 Basic Lunar calendar
-'''
+"""
+
+
 # Source:
 # Astronomical algorithms from the book "Astronomical Algorithms" by Jean Meeus, 1998
 # https://www.informatik.uni-leipzig.de/~duc/amlich/AL.py
 
+
+# Library
+##############################################################
 import math as __math
 
 def __jdFromDate(dd, mm, yy):
     """
     Compute the (integral) Julian day number of day dd/mm/yyyy
     
     i.e., the number of days between 1/1/4713 BC (Julian calendar) and dd/mm/yyyy.
@@ -215,8 +220,16 @@
         if (leapM < 0):
             leapM += 12
         if (lunarLeap != 0 and lunarM != leapM):
             return [0, 0, 0]
         elif (lunarLeap != 0 or off >= leapOff):
             off += 1
     monthStart = __getNewMoonDay(k + off, tZ)
-    return __jdToDate(monthStart + lunarD - 1)
+    return __jdToDate(monthStart + lunarD - 1)
+
+
+# Run
+##############################################################
+if __name__ == "__main__":
+    from datetime import datetime
+    now = datetime.now()
+    print(S2L(now.day, now.month, now.year))
```

### Comparing `absfuyu-1.6.0/src/absfuyu/contrib/color_extract.py` & `absfuyu-2.0.0/src/absfuyu/contrib/color_extract.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/core.py` & `absfuyu-2.0.0/src/absfuyu/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """
-Core Module
------------
-
+Absfuyu: Core
+---
 Contain type hint and other stuff
+
+Version: 2.0.0
+Date updated: 05/06/2023 (dd/mm/yyyy)
 """
 
 # Module Package
-##############################################################
+###########################################################################
 ModulePackage = [
     "all",
     "cli",
     "beautiful", "extra", "tools",
     "test", "dev", "fixers",
 ]
 ModuleList = [
-    "calculation", "data", "fibonacci", "generator",
-    "obfuscator", "sort", "strings", "util", "fun",
-    "lists", "stats", "help", "pkg_data","config",
-    "extensions", "dicts", "game", "tools", "version",
+    "calculation",
+    "sort", "util", "fun",
+    "pkg_data", "config",
+    "extensions", "game", "tools", "version"
 ]
 
 
 # Library
-##############################################################
+###########################################################################
+import os
+from pathlib import Path
 from typing import (
     Dict as __Dict,
-    # Iterable as __Iterable,
-    List as __List,
-    Optional as __Optional,
-    # Sequence as __Sequence,
-    Tuple as __Tuple,
     TypeVar as __TypeVar,
     Union as __Union,
 )
 
 from sys import version_info as __py_ver # Get python version
 if __py_ver[0] == 3:
     # Python 3.7.x
@@ -62,15 +61,15 @@
 except ImportError:
     __colorama = None
 
 
 
 
 # Color - colorama
-##############################################################
+###########################################################################
 if __colorama is not None:
     # __colorama.init(autoreset=True)
     Color: __Dict[str, str] = {
         "green": __colorama.Fore.LIGHTGREEN_EX,
         "GREEN": __colorama.Fore.GREEN,
         "blue": __colorama.Fore.LIGHTCYAN_EX,
         "BLUE": __colorama.Fore.CYAN,
@@ -91,41 +90,31 @@
         "yellow": "",
         "YELLOW": "",
         "reset": ""
     }
 
 
 # Type hints
-##############################################################
+###########################################################################
 Number = __TypeVar("Number", int, float)
 NumberC = __TypeVar("NumberC", int, float, complex)
 
 # Random string generator
 CharacterOption = __Literal[
     "default", "alphabet", "full", "uppercase",
     "lowercase", "digit", "special", "all"
 ]
 
-# Obfuscator
-EncodeOption = __Literal["b64","full"]
-CodecOption = __Literal["rot_13"]
-TxtFormat = __Literal["txt","py","bat"]
-
-Path = str
-
-# Matrix stuff
-MatrixOption = __Literal["all","row","col"]
-
-# Sudoku
-Sudoku = __List[__List[int]]
-SudokuStr = str
-Position = __Optional[__Tuple[int, int]]
-SudokuStrStyle = __Literal["zero", "dot"]
-
 # Other
 MonthLong = __Literal["january", "february", "march", "april", "may", "june", "july", "august" , "september", "october", "november", "december"]
 MonthShort = __Literal["jan", "feb", "mar", "apr", "may", "jun", "jul", "aug" , "sep", "oct", "nov", "dec"]
 Month = __Union[MonthShort, MonthLong]
 
 #
 Opt3 = __Union[__Literal[True], __Literal[False], None]
-AlignPosition = __Literal["left", "right", "center"]
+AlignPosition = __Literal["left", "right", "center"]
+
+
+# Path
+CORE_PATH = Path(os.path.abspath(os.path.dirname(__file__)))
+CONFIG_PATH = CORE_PATH.joinpath("config", "config.json")
+DATA_PATH = CORE_PATH.joinpath("pkg_data")
```

### Comparing `absfuyu-1.6.0/src/absfuyu/everything.py` & `absfuyu-2.0.0/src/absfuyu/everything.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-ABSFUYU: EVERYTHING
--------------------
+Absfuyu: Everything [W.I.P]
+---
 Everything has to offer in this package
+
+Version: 1.0.1
+Last update: 19/04/2023 (mm/dd/yyyy)
 """
 
-# Normal
+
+# Library
+###########################################################################
 from absfuyu.calculation import *
-from absfuyu.data import *
-from absfuyu.fibonacci import *
-from absfuyu.help import *
-from absfuyu.pry import *
+from absfuyu.core import *
+from absfuyu.config import *
 from absfuyu.fun import *
-from absfuyu.generator import *
-from absfuyu.obfuscator import *
+from absfuyu.pkg_data import *
+from absfuyu.logger import *
 from absfuyu.sort import *
-from absfuyu.strings import *
-from absfuyu.util import *
+from absfuyu.unused import *
 from absfuyu.version import *
-from absfuyu.lists import *
-from absfuyu.stats import *
-from absfuyu.dicts import *
+
+from absfuyu.collections import *
+from absfuyu.contrib import *
+from absfuyu.extensions import *
 from absfuyu.game import *
-from absfuyu.config import *
-from absfuyu.pkg_data import *
 from absfuyu.tools import *
+from absfuyu.util import *
 
-# Extra
-try: from absfuyu.extensions.extra import *
-except: pass
-try: from absfuyu.extensions.beautiful import *
-except: pass
-try: from absfuyu.extensions.dev import *
-except: pass
 
 # Is loaded
+###########################################################################
 __IS_EVERYTHING = True
```

### Comparing `absfuyu-1.6.0/src/absfuyu/extensions/beautiful.py` & `absfuyu-2.0.0/src/absfuyu/extensions/beautiful.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/extensions/dev/__init__.py` & `absfuyu-2.0.0/src/absfuyu/extensions/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/extensions/dev/password_hash.py` & `absfuyu-2.0.0/src/absfuyu/extensions/dev/password_hash.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/extensions/dev/pkglib.py` & `absfuyu-2.0.0/src/absfuyu/extensions/dev/pkglib.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/extensions/extra/__init__.py` & `absfuyu-2.0.0/src/absfuyu/extensions/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/extensions/extra/data_analysis.py` & `absfuyu-2.0.0/src/absfuyu/extensions/extra/data_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -214,8 +214,66 @@
             fs.append(temp)
         else:
             error_count += 1
             if error_count > max_error:
                 break
     
     # Output
-    return fs
+    return fs
+
+
+def divide_dataframe(df: __pd.DataFrame, by: str) -> list:
+    """
+    Divide df into a list of df
+    """
+    divided = [y for _, y in df.groupby(by)]
+    # divided[0] # this is the first separated df
+    # divided[len(divided)-1] # this is the last separated df
+    return divided
+
+
+def delta_date(df: __pd.DataFrame, date_field: str, col_name: str="delta_date"):
+    """
+    Calculate date interval between row
+    """
+    dated = df[date_field].to_list()
+    cal = []
+    for i in range(len(dated)):
+        if i==0:
+            cal.append(dated[i]-dated[i])
+        else:
+            cal.append(dated[i]-dated[i-1])
+    df[col_name] = [x.days for x in cal]
+    return df
+
+
+def get_unique(df: __pd.DataFrame, col:str):
+    """
+    Return a list of unique values in a column
+    """
+    return list(df[col].unique())
+
+
+def modify_date(df: __pd.DataFrame, date_col: str):
+    """
+    Add date, week, and year column for date_col
+    """
+    df["Date"] = __pd.to_datetime(df[date_col])
+    df["Week"] = df["Date"].dt.isocalendar().week
+    df["Year"] = df["Date"].dt.isocalendar().year
+    return df
+
+
+def equalize_df(data: dict, fillna = __np.nan):
+    """
+    Make all list in dict have equal length to make pd.DataFrame
+    """
+    max_len = 0
+    for _, v in data.items():
+        if len(v) >= max_len:
+            max_len = len(v)
+    for _, v in data.items():
+        if len(v) < max_len:
+            missings = max_len-len(v)
+            for _ in range(missings):
+                v.append(fillna)
+    return data
```

### Comparing `absfuyu-1.6.0/src/absfuyu/fun.py` & `absfuyu-2.0.0/src/absfuyu/fun.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-Fun Module
-------------------
+Absfuyu: Fun
+---
 Some fun or weird stuff
 
-Contain:
+Version: 1.0.0
+Date updated: 25/05/2023 (dd/mm/yyyy)
+
+Feature:
 - zodiac_sign
 - happy_new_year
 - im_bored
 """
 
 
 # Module level
-##############################################################
+###########################################################################
 __all__ = [
     "happy_new_year", "zodiac_sign", "im_bored"
 ]
 
 
-
-
-
 # Library
-##############################################################
-from datetime import date as __date
+###########################################################################
+from datetime import date
+import subprocess
+import sys
 
+from absfuyu.logger import logger
+from absfuyu.util.api import APIRequest
 
 
 # Function
-##############################################################
+###########################################################################
 def zodiac_sign(
         day: int,
         month: int,
         zodiac13: bool = False,
-        debug: bool = False
     ):
     """
     Calculate zodiac sign
 
     Include 13 zodiacs mode
     """
 
@@ -153,43 +155,38 @@
             ]), # 18/12-20/1
             "Capricorn": any([
                 month == 1 and day >= 21,
                 month == 2 and day <= 16
             ]), # 21/1-16/2
         }
 
-    if debug:
-        print(zodiac)
+    logger.debug(zodiac)
     
     for k, v in zodiac.items():
         if v is True:
             return k
 
-def im_bored():
-    from absfuyu import version as v
-    api = "https://www.boredapi.com/api/activity"
-    return v.__load_data_from_json_api(api)["activity"]
+def im_bored() -> str:
+    """Get random activity from `boredapi` website"""
+    api = APIRequest("https://www.boredapi.com/api/activity")
+    return api.fetch_data_only().json()["activity"]
 
 
 def force_shutdown():
     """Force the computer to shutdown"""
-    
-    import subprocess
-    import sys
-    
-    # get operating system
+    # Get operating system
     os_name = sys.platform
 
-    # shutdown
+    # Shutdown
     shutdown = {
         # Windows
         "win32": "shutdown -f -s -t 0".split(),
         "cygwin": "shutdown -f -s -t 0".split(),
         # Mac OS
-        "darwin": ['osascript', '-e', 'tell app "System Events" to shut down'],
+        "darwin": ["osascript", "-e", 'tell app "System Events" to shut down'],
         # Linux
         "linux": "shutdown -h now".split(),
     }
 
     if os_name in shutdown:
         return subprocess.run(shutdown[os_name])
     else:
@@ -199,15 +196,22 @@
 # For new year only
 def happy_new_year(forced: bool = False):
     """Only occurs on 01/01 every year"""
 
     if forced:
         return force_shutdown()
 
-    m = __date.today().month
-    d = __date.today().day
+    today = date.today()
+    m = today.month
+    d = today.day
 
     if m==1 and d==1:
         print("Happy New Year! You should take rest now.")
         return force_shutdown()
     else:
-        raise SystemExit("The time has not come yet")
+        raise SystemExit("The time has not come yet")
+
+
+# Run
+###########################################################################
+if __name__ == "__main__":
+    logger.setLevel(10)
```

### Comparing `absfuyu-1.6.0/src/absfuyu/game/__init__.py` & `absfuyu-2.0.0/src/absfuyu/game/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/game/tictactoe.py` & `absfuyu-2.0.0/src/absfuyu/game/tictactoe.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/help.py` & `absfuyu-2.0.0/src/absfuyu/extensions/dev/tarot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,99 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
-Help Module
------------
+Absfuyu: Tarot
+---
+Tarot stuff
 
-Contain help pages
+Version: 1.0.0
+Date updated: 05/06/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
-##############################################################
+###########################################################################
 __all__ = [
-    "help",
+    "Tarot"
 ]
 
 
-
-
 # Library
-##############################################################
-from . import core as __core
-from . import sort as __s
-from .version import __version__ as v
-
-
-
-
-
-
-# Function
-##############################################################
-
-current_func = ["help","srcMe"]
-
-def __printAlphabet(lst: list):
-    """
-    Print item in list in alphabet order with line break
-    """
-    
-    data = __s.alphabetAppear(lst)
-    incre = data[1]
-    for i in range(len(lst)):
-        if i in incre:
-            print("")
-        if i == len(lst)-1:
-            print(lst[i], end = " ")
-        else:
-            print(lst[i], end = "; ")
-    
-    return None
-
-def help(page: int = 1):
-    """
-    absfuyu builtin help page
-    """
-    
-    if page == 1:
-        print(f"""
-            absfuyu version: {v}
-            
-            USAGE:
-            import absfuyu
-            absfuyu.help()
-            help(absfuyu)
-            """)
-        
-        print("\tUse code below to use all the functions: \n")
-        module_list = __core.ModuleList
-        for x in __s.selection_sort(module_list):
-            print(f"\tfrom absfuyu import {x}")
-        
-        print("""
-            Or, you can go overboard with:
-            from absfuyu import everything as ab
-            
-            page 1 of 2
-            """)
-    
-    elif page == 2:
-        print("List of function that can use in main module:")
-        __printAlphabet(current_func)
-        print("\n")
-        print("page 2 of 2")
-        
-    else:
-        return None
-
-
-
-################################
-    # to documenting
-    """
-    Summary
-    -------
-    
-    Summary line.
-
-    Extended description of function.
-
-    Parameters
-    ----------
-    arg1 : int
-        Description of arg1
-    
-    arg2 : str
-        Description of arg2
-
-    Returns
-    -------
-    int
-        Description of return value
-
-    """
-################################
+###########################################################################
+import random
+from typing import Dict, List
+
+from absfuyu.core import DATA_PATH
+from absfuyu.logger import logger
+from absfuyu.util.api import APIRequest
+
+
+# Class
+###########################################################################
+class TarotCard:
+    """Tarot card"""
+    def __init__(
+            self,
+            name: str,
+            rank: int,
+            suit: str,
+            meanings: Dict[str, List[str]],
+            keywords: List[str],
+            fortune_telling: List[str]
+        ) -> None:
+        self.name = name.title()
+        self.rank = rank
+        self.suit = suit
+        self.meanings = meanings
+        self.keywords = keywords
+        self.fortune_telling = fortune_telling
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}({self.name})"
+    def __repr__(self) -> str:
+        return self.__str__()
+
+
+class Tarot:
+    """Tarot data"""
+    def __init__(self) -> None:
+        self.data = APIRequest(
+            "https://raw.githubusercontent.com/dariusk/corpora/master/data/divination/tarot_interpretations.json",
+            encoding="utf-8"
+        )
+        self.data_location = DATA_PATH.joinpath("tarot.json")
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}()"
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def _load(self, update: bool = False) -> List[TarotCard]:
+        """
+        Load tarot json data from API
+
+        update: refresh the cache
+        """
+        json_data = self.data.fetch_data(
+            update=update,
+            json_cache=self.data_location
+        )
+        tarot_data = json_data["tarot_interpretations"]
+        logger.debug(f"{len(tarot_data)} tarot cards loaded")
+        # return tarot_data
+        return [
+            TarotCard(
+                name=x["name"],
+                rank=x["rank"],
+                suit=x["suit"],
+                meanings=x["meanings"],
+                keywords=x["keywords"],
+                fortune_telling=x["fortune_telling"]
+            ) for x in tarot_data
+        ]
+    
+    def random_card(self):
+        """Pick a random tarot card"""
+        return random.choice(self._load())
+
+# Run
+###########################################################################
+if __name__ == "__main__":
+    logger.setLevel(10)
+    from rich import print
+    test = Tarot()
+    print(test.random_card())
```

### Comparing `absfuyu-1.6.0/src/absfuyu/tools/keygen.py` & `absfuyu-2.0.0/src/absfuyu/tools/keygen.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/tools/short_link/rebrandly.py` & `absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/rebrandly.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu/version.py` & `absfuyu-2.0.0/src/absfuyu/version.py`

 * *Files identical despite different names*

### Comparing `absfuyu-1.6.0/src/absfuyu.egg-info/PKG-INFO` & `absfuyu-2.0.0/src/absfuyu.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 1.6.0
+Version: 2.0.0
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -18,40 +18,44 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: rich
 Provides-Extra: beautiful
-Provides-Extra: dev
+Provides-Extra: cli
 Provides-Extra: click
 Provides-Extra: extra
-Provides-Extra: cli
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
 Provides-Extra: pipx
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: fixers
 Provides-Extra: autoimport
+Provides-Extra: fixers
 Provides-Extra: black
-Provides-Extra: test
 Provides-Extra: pytest
+Provides-Extra: test
 Provides-Extra: tox
+Provides-Extra: sphinx
+Provides-Extra: sphinx_rtd_theme
+Provides-Extra: python-dateutil
+Provides-Extra: unidecode
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 	<h1 align="center">
 		<img src="https://github.com/AbsoluteWinter/AbsoluteWinter.github.io/blob/main/absfuyu/images/repository-image-crop.png?raw=true" alt="absfuyu"/>
 	</h1>
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 1.6.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.0.0 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown Provides-Extra: rich Provides-Extra:
-beautiful Provides-Extra: dev Provides-Extra: click Provides-Extra: extra
-Provides-Extra: cli Provides-Extra: colorama Provides-Extra: build Provides-
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+rich Provides-Extra: beautiful Provides-Extra: cli Provides-Extra: click
+Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: test
-Provides-Extra: pytest Provides-Extra: tox Provides-Extra: all License-File:
-LICENSE
+autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
+Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
+sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
+Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
 $ pip install -U absfuyu ``` ## **USAGE:** ```python import absfuyu
 absfuyu.help() ``` ## **DOCUMENTATION:** > [here](https://
 absolutewinter.github.io/absfuyu/) ## **LICENSE:** ``` MIT License Copyright
```

### Comparing `absfuyu-1.6.0/src/absfuyu.egg-info/requires.txt` & `absfuyu-2.0.0/src/absfuyu.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,33 +2,37 @@
 [:python_version == "3.7"]
 typing_extensions>=3.7.4
 
 [LunarCalendar]
 LunarCalendar>=0.0.9
 
 [all]
-wheel
+scipy
 tox>=3.24.5
-LunarCalendar>=0.0.9
-setuptools>=51.0.0
-pandas
-colorama>=0.4
-twine>=3.7.1
 pytest>=6.2.5
+unidecode
+twine>=3.7.1
+wheel
 pipx
-virtualenv>=20.13.0
-black>=22.1.0
 matplotlib
 autoimport
-scipy
+pandas
+sphinx_rtd_theme
+sphinx
 click>=8.0.0
 build
+black>=22.1.0
+LunarCalendar>=0.0.9
+colorama>=0.4
+python-dateutil
+setuptools>=51.0.0
 numpy
-rich
+virtualenv>=20.13.0
 requests
+rich
 
 [autoimport]
 autoimport
 
 [beautiful]
 rich
 
@@ -45,37 +49,43 @@
 [click]
 click>=8.0.0
 
 [colorama]
 colorama>=0.4
 
 [dev]
-pipx
-wheel
-click>=8.0.0
-build
-colorama>=0.4
-virtualenv>=20.13.0
 setuptools>=51.0.0
 twine>=3.7.1
+sphinx_rtd_theme
+click>=8.0.0
+pipx
+build
 pytest>=6.2.5
+sphinx
+virtualenv>=20.13.0
+unidecode
+colorama>=0.4
+wheel
+rich
 
 [extra]
 scipy
-click>=8.0.0
-pandas
 numpy
-colorama>=0.4
+click>=8.0.0
 matplotlib
+pandas
 LunarCalendar>=0.0.9
+unidecode
+colorama>=0.4
 requests
+python-dateutil
 
 [fixers]
-black>=22.1.0
 autoimport
+black>=22.1.0
 
 [matplotlib]
 matplotlib
 
 [numpy]
 numpy
 
@@ -84,37 +94,49 @@
 
 [pipx]
 pipx
 
 [pytest]
 pytest>=6.2.5
 
+[python-dateutil]
+python-dateutil
+
 [requests]
 requests
 
 [rich]
 rich
 
 [scipy]
 scipy
 
 [setuptools]
 setuptools>=51.0.0
 
+[sphinx]
+sphinx
+
+[sphinx_rtd_theme]
+sphinx_rtd_theme
+
 [test]
-tox>=3.24.5
 pytest>=6.2.5
+tox>=3.24.5
 
 [tools]
 requests
 
 [tox]
 tox>=3.24.5
 
 [twine]
 twine>=3.7.1
 
+[unidecode]
+unidecode
+
 [virtualenv]
 virtualenv>=20.13.0
 
 [wheel]
 wheel
```

