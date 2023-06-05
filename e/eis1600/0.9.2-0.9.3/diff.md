# Comparing `tmp/eis1600-0.9.2.tar.gz` & `tmp/eis1600-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.9.2.tar", last modified: Wed May 24 13:59:54 2023, max compression
+gzip compressed data, was "eis1600-0.9.3.tar", last modified: Mon Jun  5 10:52:14 2023, max compression
```

## Comparing `eis1600-0.9.2.tar` & `eis1600-0.9.3.tar`

### file list

```diff
@@ -1,86 +1,84 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.338217 eis1600-0.9.2/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.2/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-24 13:59:54.338217 eis1600-0.9.2/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7640 2023-05-11 10:42:54.000000 eis1600-0.9.2/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.322217 eis1600-0.9.2/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.2/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.322217 eis1600-0.9.2/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.2/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.2/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-05-22 08:30:44.000000 eis1600-0.9.2/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.2/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.326217 eis1600-0.9.2/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.9.2/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4127 2023-05-24 09:18:31.000000 eis1600-0.9.2/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.2/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.326217 eis1600-0.9.2/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.2/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.2/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1317 2023-05-24 08:44:37.000000 eis1600-0.9.2/eis1600/gazetteers/data/regions.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      482 2023-03-23 10:19:45.000000 eis1600-0.9.2/eis1600/gazetteers/data/regions_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.2/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   273895 2023-05-24 08:44:37.000000 eis1600-0.9.2/eis1600/gazetteers/data/toponyms.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.330217 eis1600-0.9.2/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      976 2023-05-17 14:58:12.000000 eis1600-0.9.2/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.2/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.2/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.2/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.330217 eis1600-0.9.2/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.2/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.2/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.9.2/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.9.2/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.2/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3891 2023-05-17 14:58:12.000000 eis1600-0.9.2/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.2/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11237 2023-05-24 09:28:18.000000 eis1600-0.9.2/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.2/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1676 2023-05-24 09:32:10.000000 eis1600-0.9.2/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.334217 eis1600-0.9.2/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.2/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.2/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.9.2/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.9.2/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.9.2/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.9.2/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.9.2/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.334217 eis1600-0.9.2/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-05-12 10:15:49.000000 eis1600-0.9.2/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8466 2023-05-24 09:28:18.000000 eis1600-0.9.2/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.2/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2786 2023-05-12 09:46:15.000000 eis1600-0.9.2/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9184 2023-05-22 10:36:45.000000 eis1600-0.9.2/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.9.2/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7716 2023-05-24 09:05:11.000000 eis1600-0.9.2/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.334217 eis1600-0.9.2/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.2/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.9.2/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3690 2023-05-12 09:46:15.000000 eis1600-0.9.2/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.9.2/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.334217 eis1600-0.9.2/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.2/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1543 2023-05-17 14:41:04.000000 eis1600-0.9.2/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10345 2023-05-17 14:23:21.000000 eis1600-0.9.2/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.2/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.338217 eis1600-0.9.2/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.2/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.9.2/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-05-17 15:14:22.000000 eis1600-0.9.2/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.338217 eis1600-0.9.2/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.2/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.2/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.2/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.338217 eis1600-0.9.2/eis1600/toponyms/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.2/eis1600/toponyms/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1488 2023-05-17 15:02:34.000000 eis1600-0.9.2/eis1600/toponyms/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1777 2023-05-17 15:35:46.000000 eis1600-0.9.2/eis1600/toponyms/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      777 2023-05-22 08:46:53.000000 eis1600-0.9.2/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-24 13:59:54.322217 eis1600-0.9.2/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-24 13:59:54.000000 eis1600-0.9.2/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2122 2023-05-24 13:59:54.000000 eis1600-0.9.2/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-05-24 13:59:54.000000 eis1600-0.9.2/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      800 2023-05-24 13:59:54.000000 eis1600-0.9.2/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-05-24 13:59:54.000000 eis1600-0.9.2/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-05-24 13:59:54.000000 eis1600-0.9.2/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-05-24 13:59:54.338217 eis1600-0.9.2/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2372 2023-05-24 13:59:37.000000 eis1600-0.9.2/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.530443 eis1600-0.9.3/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.3/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-06-05 10:52:14.530443 eis1600-0.9.3/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7640 2023-05-11 10:42:54.000000 eis1600-0.9.3/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.510443 eis1600-0.9.3/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.3/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.514443 eis1600-0.9.3/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.3/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.3/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5860 2023-05-26 10:12:33.000000 eis1600-0.9.3/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.3/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.514443 eis1600-0.9.3/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.3/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3444 2023-06-05 10:10:23.000000 eis1600-0.9.3/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.3/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.518443 eis1600-0.9.3/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.3/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.3/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.3/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264263 2023-06-05 09:15:15.000000 eis1600-0.9.3/eis1600/gazetteers/data/toponyms_gazetteer.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.518443 eis1600-0.9.3/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.3/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.3/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.3/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.3/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.522443 eis1600-0.9.3/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.3/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.3/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.3/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.3/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.3/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3805 2023-05-26 10:16:32.000000 eis1600-0.9.3/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.3/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11237 2023-05-24 09:28:18.000000 eis1600-0.9.3/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.3/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1682 2023-05-26 10:17:00.000000 eis1600-0.9.3/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.522443 eis1600-0.9.3/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.3/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.3/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.3/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.3/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.9.3/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.3/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.3/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.522443 eis1600-0.9.3/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.3/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8429 2023-05-26 10:49:19.000000 eis1600-0.9.3/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.3/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.3/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9125 2023-05-25 14:09:24.000000 eis1600-0.9.3/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.3/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8483 2023-05-26 10:07:04.000000 eis1600-0.9.3/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.3/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.9.3/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3511 2023-05-26 10:27:39.000000 eis1600-0.9.3/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.9.3/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.3/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.3/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10339 2023-05-26 10:07:04.000000 eis1600-0.9.3/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.3/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.3/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4705 2023-05-26 10:08:19.000000 eis1600-0.9.3/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4613 2023-05-26 14:04:30.000000 eis1600-0.9.3/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.3/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.3/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.3/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/toponyms/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.3/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1494 2023-05-26 10:26:52.000000 eis1600-0.9.3/eis1600/toponyms/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1777 2023-05-17 15:35:46.000000 eis1600-0.9.3/eis1600/toponyms/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      856 2023-05-26 12:57:33.000000 eis1600-0.9.3/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.514443 eis1600-0.9.3/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2050 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      800 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-06-05 10:52:14.530443 eis1600-0.9.3/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2372 2023-06-05 10:52:09.000000 eis1600-0.9.3/setup.py
```

### Comparing `eis1600-0.9.2/LICENSE` & `eis1600-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/PKG-INFO` & `eis1600-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.2
+Version: 0.9.3
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.2/README.md` & `eis1600-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/dates/Date.py` & `eis1600-0.9.3/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/dates/date_patterns.py` & `eis1600-0.9.3/eis1600/dates/date_patterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import re
+from re import compile
 
 from openiti.helper.ara import denormalize
 
 from eis1600.helper.ar_normalization import normalize_dict
 from eis1600.helper.markdown_patterns import WORD
 
 ONES = {
@@ -66,18 +66,18 @@
        r'(?:\s(?P<weekday>' + AR_WEEKDAY + r'))?' + \
        r'(?:\s(:?ال)?(?P<day_ones>' + AR_ONES_DAY + r'))?(?:\s(:?و)?(:?ال)?(?P<day_ten>' + AR_TEN_DAY + r'))?' + \
        r'(?:\s(?:(?:من\s)?(?:شهر\s)?)?(?:ال)?(?P<month>' + AR_MONTHS + r')(?:\s(?:من|ف[يى])(?:\sشهور)?)?)?' + \
        r'\s(?P<sana>سن[ةه]|عام)(?:\s(?P<ones>' + AR_ONES + r'))?' + \
        r'(?:\s[و]?(?P<ten>' + AR_TEN + r'))?' + \
        r'(?:\s[و]?(?P<hundred>' + AR_HUNDRED + r'))?(?=(?:' + WORD + r'|[\s\.,]|$))'
 
-DATE_PATTERN = re.compile(DATE)
-MONTH_PATTERN = re.compile(AR_MONTHS)
+DATE_PATTERN = compile(DATE)
+MONTH_PATTERN = compile(AR_MONTHS)
 
 DATE_CATEGORIES = {
         'ولد': 'B', 'مولد': 'B', 'مات': 'D', 'موت': 'D', 'توفي': 'D', 'وفاة': 'D', 'حج': 'P',
         'سمع': 'K', 'قرا': 'K', 'استقر': 'O', 'اجاز': 'K', 'انفصل': 'O', 'لقي': 'M'
 }
 DATE_CATEGORIES_NOR = normalize_dict(DATE_CATEGORIES)
 
 AR_DATE_CATEGORIES = '|'.join([denormalize(key) for key in DATE_CATEGORIES.keys()])
-DATE_CATEGORY_PATTERN = re.compile(r'\s[وف]?(?P<date_category>' + AR_DATE_CATEGORIES + r')')
+DATE_CATEGORY_PATTERN = compile(r'\s[وف]?(?P<date_category>' + AR_DATE_CATEGORIES + r')')
```

### Comparing `eis1600-0.9.2/eis1600/dates/methods.py` & `eis1600-0.9.3/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/gazetteers/Onomastics.py` & `eis1600-0.9.3/eis1600/gazetteers/Onomastics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import re
-
-from importlib_resources import files
 from typing import List, Pattern
-import pandas as pd
+from importlib_resources import files
+from re import compile
+from pandas import concat, read_csv
+
 from eis1600.helper.Singleton import Singleton
 from openiti.helper.ara import denormalize
 
 path = files('eis1600.gazetteers.data').joinpath('onomastic_gazetteer.csv')
 
 
 @Singleton
@@ -33,15 +33,15 @@
     __nsb = None
     __swm = None
     __tot = None
     __ngrams = None
     __ngrams_regex = None
 
     def __init__(self) -> None:
-        oa_df = pd.read_csv(path)
+        oa_df = read_csv(path)
         oa_df['NGRAM'] = oa_df['NGRAM'].astype('uint8')
         oa_df['CATEGORY'] = oa_df['CATEGORY'].astype('category')
 
         Onomastics.__end = oa_df.loc[oa_df['CATEGORY'] == 'END', 'VALUE'].to_list()
         Onomastics.__exp = oa_df.loc[oa_df['CATEGORY'] == 'EXP', 'VALUE'].to_list()
         Onomastics.__ism = oa_df.loc[oa_df['CATEGORY'] == 'ISM', 'VALUE'].to_list()
         Onomastics.__ism = oa_df.loc[oa_df['CATEGORY'] == 'KUN', 'VALUE'].to_list()
@@ -61,22 +61,22 @@
             new_row = row
             new_row['VALUE'] = row['VALUE'].replace('أبو', 'أبي')
             return new_row
 
         abu_rows = oa_df.loc[oa_df['VALUE'].str.contains('أبو')]
         spelling_variations_1 = abu_rows.apply(rplc_to_aba, axis=1)
         spelling_variations_2 = abu_rows.apply(rplc_to_abi, axis=1)
-        df_abu_variations = pd.concat([oa_df.loc[oa_df['CATEGORY'] != 'END'], spelling_variations_1,
+        df_abu_variations = concat([oa_df.loc[oa_df['CATEGORY'] != 'END'], spelling_variations_1,
                                        spelling_variations_2])
 
         # Sort from longest to shortest ngrams - longest need to come first in regex otherwise only the shorter one
         # will be matched
         Onomastics.__ngrams = df_abu_variations.sort_values(by=['NGRAM'], ascending=False)
         ngrams = Onomastics.__ngrams['VALUE'].to_list()
-        Onomastics.__ngrams_regex = re.compile('(^| )(' + denormalize('|'.join(ngrams)) + ')')
+        Onomastics.__ngrams_regex = compile('(^| )(' + denormalize('|'.join(ngrams)) + ')')
 
     @staticmethod
     def exp() -> List[str]:
         return Onomastics.__exp
 
     @staticmethod
     def end() -> List[str]:
```

### Comparing `eis1600-0.9.2/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-0.9.3/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-0.9.3/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/gazetteers/data/toponyms.csv` & `eis1600-0.9.3/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,25 @@
 ABASKUN_540E370N_S,Ābaskūn,آبسكون,آبسكون,NW_IRAN_515E356N_R,towns,Point,"(54.04327, 37.02772)"
 ABBADAN_482E303N_S,ʿAbbādān,عبادان,عبادان,IRAQ_459E319N_R,towns,Point,"(48.27394, 30.33563)"
 ABBASIYYA_317E305N_S,al-ʿAbbāsiyyaŧ,العباسية,العباسية,MISR_305E292N_R,towns,Point,"(31.70644, 30.53647)"
 ABDAS_473E314N_S,ʿAbdās,عبداس,عبداس,IRAQ_459E319N_R,towns,Point,"(47.33731, 31.46283)"
 ABDIN_493E312N_S,ʿAbdīn,عبدين,عبدين,SW_IRAN_540E294N_R,waystations,Point,"(49.31456, 31.22889)"
 ABHAR_492E361N_S,Abhar,أبهر,أبهر,NW_IRAN_515E356N_R,towns,Point,"(49.23473, 36.15722)"
 ABIWARD_595E372N_S,Abīward,أبيورد,أبيورد,NE_IRAN_606E351N_R,towns,Point,"(59.59733, 37.27)"
-ABKHAN_483E408N_R,al-Abḫān,الأبخان,الأبخان، لايجان، ليزان، ليزان، ليران,,regions,Point,"(48.38086, 40.88004)"
 ABKHAN_483E408N_S,al-Abḫān,الأبخان,الأبخان، لايجان، ليزان، ليزان، ليران,QABQ_457E413N_R,towns,Point,"(48.38086, 40.88004)"
 ABNASH_039W396N_S,Abnaš,أبنش,أبنش,ANDALUS_040E398N_R,towns,Point,"(-3.91003, 39.63212)"
 ABSHAYA_317E264N_S,Abšāyaŧ,أبشاية,أبشاية,MISR_305E292N_R,villages,Point,"(31.7988, 26.47449)"
 ABSHIN_635E352N_S,Abšīn,أبشين,أبشين,NE_IRAN_606E351N_R,towns,Point,"(63.528, 35.24882)"
 ABSHUR_574E326N_S,Āb Šūr,آب شور,آب شور,SE_IRAN_656E286N_R,waystations,Point,"(57.40729, 32.65943)"
 ABTIA_500E336N_S,Abtiʿaŧ,أبتعة,أبتعة,NW_IRAN_515E356N_R,waystations,Point,"(50.05422, 33.62812)"
 ABUKHASIB_479E304N_S,Abū al-Ḫaṣīb,أبو الخصيب,أبو الخصيب,IRAQ_459E319N_R,towns,Point,"(47.99265, 30.43759)"
 ABUQSHA_619E410N_O,Abūqšaŧ,أبوقشة,أبوقشة,MAWARANNAHR_656E401N_R,sites,Point,"(61.95529, 41.0484)"
 ABWAB_340E174N_S,al-Abwāb,الأبواب,الأبواب,MISR_305E292N_R,villages,Point,"(34.09472, 17.49927)"
 ABWA_390E232N_S,al-Abwāʾ,الأبواء,الأبواء,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.09484, 23.22814)"
 ABYAD_424E318N_S,al-Abyaḍ,الأبيض,الأبيض,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(42.45438, 31.86163)"
-ABYAYN_449E131N_R,Abyāyn,أبياين,أبياين,,regions,Point,"(44.96348, 13.14229)"
 ABYAYN_449E131N_S,Abyāyn,أبياين,أبياين,SW_ARABIA_456E158N_R,capitals,Point,"(44.96348, 13.14229)"
 ABZAR_529E282N_S,Abzar,أبزر,أبزر,SW_IRAN_540E294N_R,villages,Point,"(52.94703, 28.28084)"
 ADAN_450E127N_S,ʿAdan,عدن,عدن,SW_ARABIA_456E158N_R,towns,Point,"(45.03942, 12.79365)"
 ADHANA_353E369N_S,Aḏanaŧ,أذنة,أذنة,SHAM_363E335N_R,waystations,Point,"(35.34272, 36.96023)"
 ADHARBAYJAN_479E382N_R,Aḏarbayǧān,أذربيجان,أذربيجان,QABQ_457E413N_R,regions,Point,"(47.95801, 38.24076)"
 ADHNUN_352E333N_S,ʿAḏnūn,عذنون,عذنون,SHAM_363E335N_R,towns,Point,"(35.2662, 33.39418)"
 ADHRAMA_417E369N_S,Aḏramaŧ,أذرمة,أذرمة,JAZIRA_420E364N_R,towns,Point,"(41.72002, 36.99109)"
@@ -40,41 +38,37 @@
 AFRIDHIN_517E354N_S,Afrīḏīn,أفريذين,أفريذين,NW_IRAN_515E356N_R,villages,Point,"(51.77466, 35.42345)"
 AHAR_471E384N_S,Ahar,أهر,أهر,QABQ_457E413N_R,towns,Point,"(47.14386, 38.45223)"
 AHNAS_309E291N_S,Ahnās,أهناس,أهناس,MISR_305E292N_R,towns,Point,"(30.95992, 29.13124)"
 AHQAF_508E193N_R,al-Aḥqāf,الأحقاف,الأحقاف,SE_ARABIA_556E220N_R,regions,Point,"(50.8587, 19.38865)"
 AHSA_495E253N_S,al-Aḥsāʾ,الأحساء,الأحساء,SE_ARABIA_556E220N_R,capitals,Point,"(49.54137, 25.34929)"
 AHWAR_465E136N_R,Aḥwar,أحور,أحور,SW_ARABIA_456E158N_R,regions,Point,"(46.54442, 13.67538)"
 AHWAR_466E135N_S,Aḥwar,أحور,أحور,SW_ARABIA_456E158N_R,towns,Point,"(46.61972, 13.56967)"
-AHWAZ_486E313N_R,al-Ahwāz,الأهواز,الأهواز، سوق الأهواز,,regions,Point,"(48.69059, 31.32986)"
 AHWAZ_486E313N_S,al-Ahwāz,الأهواز,الأهواز، سوق الأهواز,SW_IRAN_540E294N_R,metropoles,Point,"(48.69059, 31.32986)"
 AJARUD_323E300N_S,ʿAǧarūd,عجرود,عجرود,MISR_305E292N_R,waystations,Point,"(32.38039, 30.05828)"
 AJDABIYYA_202E304N_S,Aǧdābiyyaŧ,أجدابية,أجدابية,BARQA_221E314N_R,towns,Point,"(20.20218, 30.46697)"
 AJFUR_429E274N_S,al-Aǧfur,الأجفر,الأجفر,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(42.97781, 27.44255)"
 AJGH_569E375N_S,Aǧġ,أجغ,أجغ,NW_IRAN_515E356N_R,villages,Point,"(56.95205, 37.51437)"
 AJWALI_374E298N_S,al-Aǧwalī,الأجولي,الأجولي,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(37.4317, 29.87858)"
 AKHDAMIYYA_422E322N_S,al-Aḫdamiyyaŧ,الأخدمية,الأخدمية,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(42.23928, 32.28927)"
 AKHILLA_451E132N_R,Aḫillaŧ,أخلة,أخلة,SW_ARABIA_456E158N_R,regions,Point,"(45.17945, 13.2032)"
 AKHLAT_425E387N_S,Aḫlāṭ,أخلاط,أخلاط، خلاط,QABQ_457E413N_R,towns,Point,"(42.51044, 38.76551)"
-AKHLAT_425E387N_S,Aḫlāṭ,أخلاط,أخلاط، خلاط,QABQ_457E413N_R,towns,Point,"(42.51044, 38.76551)"
 AKHMIM_317E265N_S,Aḫmīm,أخميم,أخميم,MISR_305E292N_R,towns,Point,"(31.72957, 26.56301)"
 AKHSHIKATH_713E409N_S,Aḫšīkaṯ,أخشيكث,أخشيكث,MAWARANNAHR_656E401N_R,capitals,Point,"(71.36392, 40.91733)"
 AKHSISAK_652E378N_S,Aḫsīsak,أخسيسك,أخسيسك,MAWARANNAHR_656E401N_R,capitals,Point,"(65.26937, 37.888)"
 AKHUR_557E391N_S,Āḫur,آخر,آخر,NW_IRAN_515E356N_R,capitals,Point,"(55.71277, 39.19825)"
 AKHYAS_130E381N_S,Aḫyās,أخياس,أخياس,SIQILIYYA_145E375N_R,towns,Point,"(13.09201, 38.13882)"
 AKKA_350E329N_S,ʿAkkaŧ,عكة,عكة,SHAM_363E335N_R,towns,Point,"(35.07559, 32.92878)"
-AKKA_350E329N_S,ʿAkkaŧ,عكة,عكة,SHAM_363E335N_R,towns,Point,"(35.07559, 32.92878)"
 ALHAM_522E365N_S,Alham,ألهم,ألهم,NW_IRAN_515E356N_R,towns,Point,"(52.23414, 36.56405)"
 ALHAN_440E148N_R,Alhān,ألهان,ألهان,SW_ARABIA_456E158N_R,regions,Point,"(44.07982, 14.80399)"
 ALLAQI_328E230N_S,ʿAllaqī,علقي,علقي,MISR_305E292N_R,towns,Point,"(32.87404, 23.01969)"
 ALTH_440E340N_S,ʿAlṯ ,علث ,علث ،  العلث,IRAQ_459E319N_R,towns,Point,"(44.08916, 34.02656)"
 ALUS_424E339N_S,Ālūs,آلوس,آلوس، آلوسا,JAZIRA_420E364N_R,towns,Point,"(42.41353, 33.98559)"
 AMASHIYYA_439E165N_S,al-Aʿmašiyyaŧ,الأعمشية,الأعمشية,SW_ARABIA_456E158N_R,waystations,Point,"(43.95032, 16.56721)"
 AMAWAS_349E318N_S,ʿAmawās,عمواس,عمواس,SHAM_363E335N_R,villages,Point,"(34.97656, 31.84394)"
 AMID_402E379N_S,Āmid,آمد,آمد,JAZIRA_420E364N_R,capitals,Point,"(40.21323, 37.9151)"
-AMID_402E379N_S,Āmid,آمد,آمد,JAZIRA_420E364N_R,capitals,Point,"(40.21323, 37.9151)"
 AMLIL_029W352N_S,Amlīl,أمليل,أمليل,MAGHRIB_045E323N_R,towns,Point,"(-2.96861, 35.29761)"
 AMMAN_359E319N_S,ʿAmmān,عمان,عمان,SHAM_363E335N_R,towns,Point,"(35.91903, 31.93113)"
 AMQ_364E363N_S,ʿAmq,عمق,عمق,SHAM_363E335N_R,waystations,Point,"(36.47102, 36.38345)"
 AMUL_524E364N_S,Āmul,آمل,آمل,NW_IRAN_515E356N_R,capitals,Point,"(52.40859, 36.42256)"
 AMUL_635E390N_S,Āmul,آمل,آمل,NE_IRAN_606E351N_R,towns,Point,"(63.51255, 39.06795)"
 AMZAH_642E399N_S,Amzah,أمزه,أمزه,MAWARANNAHR_656E401N_R,waystations,Point,"(64.25722, 39.90472)"
 ANAFA_357E343N_S,Anafaŧ,أنفة,أنفة,SHAM_363E335N_R,towns,Point,"(35.73678, 34.35634)"
@@ -127,19 +121,17 @@
 ARJUMAN_526E311N_R,Arǧumān,أرجمان,أرجمان,SW_IRAN_540E294N_R,regions,Point,"(52.62743, 31.1799)"
 ARJUNA_040W379N_S,Arǧūnaŧ,أرجونة,أرجونة,ANDALUS_040E398N_R,towns,Point,"(-4.053, 37.9204)"
 ARJ_392E238N_O,al-ʿArǧ,العرج,العرج,CENTRAL_ARABIA_416E227N_R,sites,Point,"(39.20944, 23.85851)"
 ARKU_072E360N_S,Arkū,أركو,أركو، ركوة,IFRIQIYYA_78E349N_R,towns,Point,"(7.20287, 36.05429)"
 ARMABIL_663E262N_S,Armābīl,أرمابيل,أرمابيل، أرمائيل,SE_IRAN_656E286N_R,villages,Point,"(66.38343, 26.23769)"
 ARMANT_325E256N_S,Armant,أرمنت,أرمنت,MISR_305E292N_R,towns,Point,"(32.51795, 25.64017)"
 ARMINIYYA_441E394N_R,Arminiyyaŧ,أرمنية,أرمنية,QABQ_457E413N_R,regions,Point,"(44.11256, 39.47331)"
-ARMINIYYA_441E394N_R,Arminiyyaŧ,أرمنية,أرمنية,QABQ_457E413N_R,regions,Point,"(44.11256, 39.47331)"
 ARQA_360E345N_S,ʿArqaŧ,عرقة,عرقة,SHAM_363E335N_R,towns,Point,"(36.073, 34.52991)"
 ARQA_379E383N_S,ʿArqaŧ,عرقة,عرقة,JAZIRA_420E364N_R,waystations,Point,"(37.96251, 38.36373)"
 ARRAJAN_502E306N_S,Arrāǧān,أراجان,أراجان,SW_IRAN_540E294N_R,capitals,Point,"(50.29766, 30.6103)"
-ARRAJAN_502E306N_S,Arrāǧān,أراجان,أراجان,SW_IRAN_540E294N_R,capitals,Point,"(50.29766, 30.6103)"
 ARRAN_471E406N_R,Arrān,أران,أران,QABQ_457E413N_R,regions,Point,"(47.14761, 40.60291)"
 ARSUBANIKATH_696E399N_S,Arsubānīkaṯ,أرسبانيكث,أرسبانيكث، سبانيكث,MAWARANNAHR_656E401N_R,towns,Point,"(69.60096, 39.93024)"
 ARSUF_348E321N_S,Arsūf,أرسوف,أرسوف,SHAM_363E335N_R,towns,Point,"(34.80739, 32.19588)"
 ARTHA_422E557N_R,al-Arṯā,الأرثا,الأرثا، الأرثانية,QABQ_457E413N_R,regions,Point,"(42.25518, 55.73456)"
 ARZAN_416E379N_S,Arzan,أرزن,أرزن,JAZIRA_420E364N_R,villages,Point,"(41.65964, 37.9789)"
 ASADABADH_481E348N_S,Asadābāḏ,أسداباذ,أسداباذ,NW_IRAN_515E356N_R,towns,Point,"(48.15134, 34.80031)"
 ASADABADH_564E363N_S,Asadābāḏ,أسداباذ,أسداباذ,NE_IRAN_606E351N_R,towns,Point,"(56.45362, 36.32897)"
@@ -149,45 +141,38 @@
 ASBARA_707E401N_S,Asbaraŧ,أسبرة,أسبرة,MAWARANNAHR_656E401N_R,villages,Point,"(70.70139, 40.13989)"
 ASBARA_735E427N_S,Asbaraŧ,أسبرة,أسبرة,MAWARANNAHR_656E401N_R,villages,Point,"(73.56945, 42.77192)"
 ASBIDHDASHT_511E321N_S,Asbīḏ Dašt,أسبيذ دشت,أسبيذ دشت,NW_IRAN_515E356N_R,waystations,Point,"(51.18532, 32.13467)"
 ASFABJAY_670E305N_S,Asfabǧāy,أسفبجاي,أسفبجاي، سفنجاوي,SE_IRAN_656E286N_R,towns,Point,"(67.02922, 30.58971)"
 ASFAQA_622E262N_S,Aṣfaqaŧ,أصفقة,أصفقة,SE_IRAN_656E286N_R,towns,Point,"(62.20454, 26.24757)"
 ASFAQUS_108E347N_S,Asfāqus,أسفاقس,أسفاقس,IFRIQIYYA_78E349N_R,towns,Point,"(10.8019, 34.77411)"
 ASFARAYIN_574E369N_S,Asfarāyin,أسفراين,أسفراين,NE_IRAN_606E351N_R,towns,Point,"(57.43023, 36.98777)"
-ASFARAYIN_574E369N_S,Asfarāyin,أسفراين,أسفراين,NE_IRAN_606E351N_R,towns,Point,"(57.43023, 36.98777)"
-ASFUZAR_621E332N_R,al-Asfuzār,الأسفزار,الأسفزار,,regions,Point,"(62.12974, 33.24402)"
 ASFUZAR_621E332N_S,al-Asfuzār,الأسفزار,الأسفزار,NE_IRAN_606E351N_R,capitals,Point,"(62.12974, 33.24402)"
 ASHAM_412E198N_R,ʿAšam,عشم,عشم,CENTRAL_ARABIA_416E227N_R,regions,Point,"(41.23862, 19.80364)"
 ASHIR_031E357N_S,ʿAšīr,عشير,عشير,MAGHRIB_045E323N_R,towns,Point,"(3.16032, 35.70178)"
 ASHRASHAL_022E365N_S,Ašrašāl,أشرشال,أشرشال,MAGHRIB_045E323N_R,towns,Point,"(2.25421, 36.541)"
-ASKARMUKRAM_488E316N_R,ʿAskar Mukram,عسكر مكرم,عسكر مكرم,,regions,Point,"(48.8982, 31.66531)"
 ASKARMUKRAM_488E316N_S,ʿAskar Mukram,عسكر مكرم,عسكر مكرم,SW_IRAN_540E294N_R,capitals,Point,"(48.8982, 31.66531)"
 ASLAN_011W354N_S,Āslān,آسلان,آسلان، واسلان,MAGHRIB_045E323N_R,towns,Point,"(-1.16486, 35.45814)"
 ASNA_325E253N_S,Asnā,أسنا,أسنا,MISR_305E292N_R,towns,Point,"(32.55162, 25.32189)"
 ASQALAN_345E316N_S,ʿAsqalān,عسقلان,عسقلان,SHAM_363E335N_R,towns,Point,"(34.55455, 31.66572)"
 ASRAB_637E358N_S,al-Asrāb,الأسراب,الأسراب,NE_IRAN_606E351N_R,waystations,Point,"(63.76323, 35.81599)"
 ASTARABADH_544E367N_S,Astārabāḏ,أستارباذ,أستارباذ,NW_IRAN_515E356N_R,towns,Point,"(54.47005, 36.7886)"
-ASTARABADH_544E367N_S,Astārabāḏ,أستارباذ,أستارباذ,NW_IRAN_515E356N_R,towns,Point,"(54.47005, 36.7886)"
 ASTARABYAN_628E342N_S,Astarabyān,أستربيان,أستربيان,NE_IRAN_606E351N_R,towns,Point,"(62.80223, 34.2484)"
 ASYUT_311E271N_S,Asyūṭ,أسيوط,أسيوط,MISR_305E292N_R,towns,Point,"(31.18485, 27.17922)"
 ATASHKAHAN_567E336N_S,Ataškahān,أتشكهان,أتشكهان,SE_IRAN_656E286N_R,villages,Point,"(56.78965, 33.67155)"
 ATBASH_758E411N_S,Aṭbāš,أطباش,أطباش، طباش,MAWARANNAHR_656E401N_R,villages,Point,"(75.81567, 41.16025)"
 ATFIH_312E294N_S,Aṭfīḥ,أطفيح,أطفيح,MISR_305E292N_R,towns,Point,"(31.29974, 29.43347)"
 ATFU_328E250N_R,Atfū,أتفو,أتفو,,regions,Point,"(32.87999, 25.01203)"
 ATHAFIT_439E161N_S,Aṯāfit,أثافت,أثافت,SW_ARABIA_456E158N_R,waystations,Point,"(43.97249, 16.11174)"
 ATHARIB_368E361N_S,al-Aṯārib,الأثارب,الأثارب,SHAM_363E335N_R,waystations,Point,"(36.83533, 36.13792)"
 ATMIN_366E353N_S,al-Aṭmīn,الأطمين,الأطمين، اللطمين,SHAM_363E335N_R,villages,Point,"(36.62191, 35.31245)"
 ATRABINUSH_125E379N_S,Aṭrābinuš,أطرابنش,أطرابنش,SIQILIYYA_145E375N_R,towns,Point,"(12.50893, 37.98824)"
 ATRABIYYA_317E307N_R,Aṭrabiyyaŧ,أطربية,أطربية,MISR_305E292N_R,regions,Point,"(31.74628, 30.70963)"
 ATRABULUS_131E328N_S,Aṭrābulus,أطرابلس,أطرابلس، طرابلس,BARQA_221E314N_R,towns,Point,"(13.19209, 32.87801)"
 ATRABULUS_358E344N_S,Aṭrābulus,أطرابلس,أطرابلس، طرابلس,SHAM_363E335N_R,towns,Point,"(35.85194, 34.44044)"
-ATRABULUS_358E344N_S,Aṭrābulus,أطرابلس,أطرابلس، طرابلس,SHAM_363E335N_R,towns,Point,"(35.85194, 34.44044)"
-ATRIB_311E304N_R,Atrīb,أتريب,أتريب,,regions,Point,"(31.17223, 30.45947)"
 ATRIB_311E304N_S,Atrīb,أتريب,أتريب,MISR_305E292N_R,towns,Point,"(31.17223, 30.45947)"
-ATTAR_423E171N_R,ʿAṭṭār,عطار,عطار,,regions,Point,"(42.39306, 17.18513)"
 ATTAR_423E171N_S,ʿAṭṭār,عطار,عطار,SW_ARABIA_456E158N_R,capitals,Point,"(42.39306, 17.18513)"
 AWAL_717E404N_S,Awāl,أوال,أوال,MAWARANNAHR_656E401N_R,towns,Point,"(71.74749, 40.4358)"
 AWAMIL_400E349N_S,al-ʿAwāmil,العوامل,العوامل,JAZIRA_420E364N_R,waystations,Point,"(40.09518, 34.93204)"
 AWARIK_579E293N_S,Awārik,أوارك,أوارك,SW_IRAN_540E294N_R,towns,Point,"(57.95411, 29.32947)"
 AWA_505E346N_S,Āwaŧ,آوة,آوة,NW_IRAN_515E356N_R,towns,Point,"(50.54227, 34.68541)"
 AWBA_631E344N_S,Awbaŧ,أوبة,أوبة، أوفة,NE_IRAN_606E351N_R,towns,Point,"(63.16814, 34.4094)"
 AWDHANA_102E365N_S,Awḏanaŧ,أوذنة,أوذنة,IFRIQIYYA_78E349N_R,towns,Point,"(10.28004, 36.59668)"
@@ -197,15 +182,14 @@
 AWNID_359E270N_S,al-ʿAwnīd,العونيد,العونيد,CENTRAL_ARABIA_416E227N_R,towns,Point,"(35.99173, 27.00533)"
 AWNID_369E316N_S,al-ʿAwnīd,العونيد,العونيد,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(36.92899, 31.64055)"
 AWRAHA_795E264N_S,Awrahaŧ,أورهة,أورهة,SE_IRAN_656E286N_R,towns,Point,"(79.59619, 26.46686)"
 AWSAJA_440E259N_S,al-ʿAwsaǧaŧ,العوسجة,العوسجة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(44.07861, 25.98495)"
 AWSIYA_312E311N_R,al-Awsiyaŧ,الأوسية,الأوسية,MISR_305E292N_R,regions,Point,"(31.25278, 31.19181)"
 AWTAS_406E217N_S,Awṭās,أوطاس,أوطاس,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(40.68003, 21.733)"
 AYDHAB_362E224N_S,ʿAyḏab,عيذب,عيذب,MISR_305E292N_R,towns,Point,"(36.24428, 22.48899)"
-AYDHAB_362E224N_S,ʿAyḏab,عيذب,عيذب,MISR_305E292N_R,towns,Point,"(36.24428, 22.48899)"
 AYLAN_076W314N_S,Aylān,أيلان,أيلان، أغمات أيلا، أغمات ويلا,MAGHRIB_045E323N_R,towns,Point,"(-7.6971, 31.49952)"
 AYLA_349E295N_S,Aylaŧ,أيلة,أيلة، ويلة,SHAM_363E335N_R,towns,Point,"(34.94527, 29.57226)"
 AYNJARR_359E337N_S,ʿAyn al-Ǧarr,عين الجر,عين الجر,SHAM_363E335N_R,waystations,Point,"(35.90422, 33.7273)"
 AYNMUGHATTA_138E373N_S,ʿAyn al-Muġaṭṭāʾ,عين المغطاء,عين المغطاء,SIQILIYYA_145E375N_R,towns,Point,"(13.86212, 37.35487)"
 AYNRUMIYYA_389E363N_S,ʿAyn al-Rūmiyyaŧ,عين الرومية,عين الرومية,JAZIRA_420E364N_R,waystations,Point,"(38.91206, 36.34984)"
 AYNSHAMS_313E301N_S,ʿAyn Šams,عين شمس,عين شمس,MISR_305E292N_R,towns,Point,"(31.3077, 30.12919)"
 AYNTAMR_435E326N_S,ʿAyn al-Tamr,عين التمر,عين التمر,IRAQ_459E319N_R,towns,Point,"(43.52574, 32.62337)"
@@ -217,15 +201,14 @@
 AZDUD_346E317N_S,Azdūd,أزدود,أزدود، يزدود,SHAM_363E335N_R,waystations,Point,"(34.66817, 31.79837)"
 AZILA_059W355N_S,Azīlaŧ,أزيلة,أزيلة,MAGHRIB_045E323N_R,towns,Point,"(-5.97486, 35.58306)"
 AZKAS_521E315N_S,Azkās,أزكاس,أزكاس,SW_IRAN_540E294N_R,waystations,Point,"(52.17709, 31.51558)"
 AZRAQ_368E318N_S,al-Azraq,الأزرق,الأزرق,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(36.87768, 31.84612)"
 BAASHIQA_433E364N_S,Bāʿašīqā,باعشيقا,باعشيقا,JAZIRA_420E364N_R,villages,Point,"(43.36699, 36.41022)"
 BAAYNATHA_424E366N_S,Bāʿaynāṯā,باعيناثا,باعيناثا,JAZIRA_420E364N_R,towns,Point,"(42.43701, 36.6609)"
 BABABWAB_483E420N_S,Bāb al-Abwāb,باب الأبواب,باب الأبواب,QABQ_457E413N_R,towns,Point,"(48.30854, 42.04308)"
-BABABWAB_483E420N_S,Bāb al-Abwāb,باب الأبواب,باب الأبواب,QABQ_457E413N_R,towns,Point,"(48.30854, 42.04308)"
 BABHADID_670E382N_O,Bāb al-Ḥadīd,باب الحديد,باب الحديد,MAWARANNAHR_656E401N_R,sites,Point,"(67.03158, 38.22114)"
 BABIJ_307E308N_S,Babīǧ,ببيج,ببيج,MISR_305E292N_R,towns,Point,"(30.75642, 30.87466)"
 BABIL_444E325N_S,Bābil,بابل,بابل,IRAQ_459E319N_R,towns,Point,"(44.42281, 32.57211)"
 BABNA_624E349N_S,Babnaŧ,ببنة,ببنة,NE_IRAN_606E351N_R,towns,Point,"(62.4787, 34.94152)"
 BAB_711E408N_S,Bāb,باب,باب,MAWARANNAHR_656E401N_R,towns,Point,"(71.16439, 40.88072)"
 BADAH_499E312N_S,Badah,بده,بده,SW_IRAN_540E294N_R,waystations,Point,"(49.96262, 31.29164)"
 BADAQUN_305E308N_R,al-Badaqūn,البدقون,البدقون,MISR_305E292N_R,regions,Point,"(30.52845, 30.89835)"
@@ -241,19 +224,17 @@
 BADIS_066E347N_S,Bādis,بادس,بادس,IFRIQIYYA_78E349N_R,towns,Point,"(6.65773, 34.76281)"
 BADI_394E156N_S,Bāḍiʿ,باضع,باضع,MISR_305E292N_R,towns,Point,"(39.48117, 15.63308)"
 BADLIS_421E383N_S,Badlīs,بدليس,بدليس، بدليس,JAZIRA_420E364N_R,towns,Point,"(42.13266, 38.3955)"
 BADR_388E237N_S,Badr,بدر,بدر,CENTRAL_ARABIA_416E227N_R,towns,Point,"(38.80098, 23.72676)"
 BADR_447E138N_R,Badr,بدر,بدر,SW_ARABIA_456E158N_R,regions,Point,"(44.72906, 13.87387)"
 BADURAYA_442E333N_S,Bādūrayā,بادوريا,بادوريا,IRAQ_459E319N_R,towns,Point,"(44.21572, 33.37712)"
 BAGHAY_071E355N_S,Bāġāy,باغاي,باغاي,IFRIQIYYA_78E349N_R,towns,Point,"(7.12454, 35.50598)"
-BAGHDAD_443E333N_S,Baġdād,بغداد,بغداد,IRAQ_459E319N_R,metropoles,Point,"(44.35693, 33.35932)"
+BAGHDAD_443E333N_S,Baġdād,بغداد,بغداد، بغداذ، بغذاذ,IRAQ_459E319N_R,metropoles,Point,"(44.35693, 33.35932)"
 BAGHIRQAN_612E414N_S,Baġirqān,بغرقان,بغرقان,MAWARANNAHR_656E401N_R,villages,Point,"(61.27533, 41.43986)"
-BAGHLAN_687E362N_R,Baġlān,بغلان,بغلان,,regions,Point,"(68.77093, 36.2356)"
 BAGHLAN_687E362N_S,Baġlān,بغلان,بغلان,NE_IRAN_606E351N_R,towns,Point,"(68.77093, 36.2356)"
-BAGHNIN_650E327N_R,Baġnīn,بغنين,بغنين,,regions,Point,"(65.00452, 32.71541)"
 BAGHNIN_650E327N_S,Baġnīn,بغنين,بغنين,SE_IRAN_656E286N_R,towns,Point,"(65.00452, 32.71541)"
 BAGHRAS_362E364N_S,Baġrās,بغراس,بغراس,SHAM_363E335N_R,villages,Point,"(36.22768, 36.41518)"
 BAGHRAWAND_431E400N_R,Baġrawand,بغروند,بغروند,QABQ_457E413N_R,regions,Point,"(43.16621, 40.00234)"
 BAGHSHUR_625E356N_S,Baġšūr,بغشور,بغشور,NE_IRAN_606E351N_R,towns,Point,"(62.54722, 35.60846)"
 BAHAR_563E298N_S,Bahār,بهار,بهار,SW_IRAN_540E294N_R,towns,Point,"(56.35225, 29.8855)"
 BAHAWADH_559E318N_S,Bahāwaḏ,بهاوذ,بهاوذ,SW_IRAN_540E294N_R,towns,Point,"(55.96459, 31.83238)"
 BAHIRABADH_624E368N_S,Baḥīrābāḏ,بحيراباذ,بحيراباذ,NE_IRAN_606E351N_R,waystations,Point,"(62.46952, 36.88847)"
@@ -268,48 +249,43 @@
 BAHRRUM_017E372N_W,Baḥr al-Rūm,بحر الروم,بحر الروم,,waters,Point,"(1.71713, 37.28888)"
 BAHRRUM_302E322N_W,Baḥr al-Rūm,بحر الروم,بحر الروم,,waters,Point,"(30.28697, 32.20303)"
 BAJANAK_408E486N_R,al-Baǧānāk,البجاناك,البجاناك، البجاناكية,QABQ_457E413N_R,regions,Point,"(40.8946, 48.61696)"
 BAJANAK_499E492N_R,al-Baǧānāk,البجاناك,البجاناك، البجاناكية,QABQ_457E413N_R,regions,Point,"(49.92897, 49.24133)"
 BAJARWAN_389E361N_S,Bāǧarwān,باجروان,باجروان,JAZIRA_420E364N_R,towns,Point,"(38.98556, 36.13571)"
 BAJARWAN_481E392N_R,Bāǧarwān,باجروان,باجروان، موقان، موغكان,,regions,Point,"(48.12475, 39.2256)"
 BAJAYA_050E367N_S,Baǧāyaŧ,بجاية,بجاية,IFRIQIYYA_78E349N_R,towns,Point,"(5.04769, 36.70199)"
-BAJA_078W380N_R,Bāǧaŧ,باجة,باجة,,regions,Point,"(-7.80444, 38.00689)"
 BAJA_078W380N_S,Bāǧaŧ,باجة,باجة,ANDALUS_040E398N_R,towns,Point,"(-7.80444, 38.00689)"
 BAJA_092E366N_S,Bāǧaŧ,باجة,باجة,IFRIQIYYA_78E349N_R,towns,Point,"(9.20563, 36.67738)"
 BAJISRA_446E337N_S,Bāǧisrá,باجسرى,باجسرى,IRAQ_459E319N_R,towns,Point,"(44.63801, 33.73126)"
-BAJJANA_024W369N_R,Baǧǧānaŧ,بجانة,بجانة,,regions,Point,"(-2.41826, 36.95657)"
 BAJJANA_024W369N_S,Baǧǧānaŧ,بجانة,بجانة,ANDALUS_040E398N_R,towns,Point,"(-2.41826, 36.95657)"
 BAKHARZ_603E350N_R,Bāḫarz,باخرز,باخرز,NE_IRAN_606E351N_R,regions,Point,"(60.33692, 35.01995)"
 BAKHTA_561E291N_S,Bāḫtaŧ,باختة,باختة، ناجت,SW_IRAN_540E294N_R,towns,Point,"(56.16823, 29.12939)"
 BAKRABADH_658E315N_S,Bakrābāḏ,بكراباذ,بكراباذ، بكراواذ,SE_IRAN_656E286N_R,towns,Point,"(65.86183, 31.59434)"
 BAKUH_498E403N_S,Bākūh,باكوه,باكوه,QABQ_457E413N_R,towns,Point,"(49.86422, 40.379)"
 BAKUSAYA_464E329N_S,Bākusāyā,باكسايا,باكسايا,IRAQ_459E319N_R,towns,Point,"(46.46935, 32.94441)"
 BALABAKK_361E340N_S,Baʿlabakk,بعلبك,بعلبك,SHAM_363E335N_R,towns,Point,"(36.19213, 34.01251)"
 BALADDAWAR_651E322N_R,Balad Dāwar,بلد داور,بلد داور، بلا داور، زمين داور,SE_IRAN_656E286N_R,regions,Point,"(65.17678, 32.23313)"
 BALADGHUMAR_047W351N_S,Balad Ġumār,بلد غمار,بلد غمار,MAGHRIB_045E323N_R,towns,Point,"(-4.70461, 35.19603)"
 BALADNUBA_316E197N_R,Balad al-Nūbaŧ,بلد النوبة,بلد النوبة,MISR_305E292N_R,regions,Point,"(31.60503, 19.72554)"
 BALAD_427E364N_S,Balad,بلد,بلد,JAZIRA_420E364N_R,towns,Point,"(42.758, 36.47417)"
 BALANJAR_464E432N_S,Balanǧar,بلنجر,بلنجر,QABQ_457E413N_R,towns,Point,"(46.42082, 43.28166)"
-BALANSIYYA_004W394N_R,Balansiyyaŧ,بلنسية,بلنسية,,regions,Point,"(-0.41486, 39.43516)"
 BALANSIYYA_004W394N_S,Balansiyyaŧ,بلنسية,بلنسية,ANDALUS_040E398N_R,towns,Point,"(-0.41486, 39.43516)"
 BALARM_133E381N_S,Balarm,بلرم,بلرم,SIQILIYYA_145E375N_R,capitals,Point,"(13.34479, 38.10757)"
 BALASABUR_511E303N_R,Balā Sābūr,بلا سابور,بلا سابور,SW_IRAN_540E294N_R,regions,Point,"(51.1775, 30.39947)"
 BALAYAN_694E411N_S,Bālāyān,بالايان,بالايان,MAWARANNAHR_656E401N_R,towns,Point,"(69.45575, 41.11173)"
 BALHIB_304E312N_S,Balhīb,بلهيب,بلهيب,MISR_305E292N_R,towns,Point,"(30.46299, 31.28513)"
 BALISH_676E296N_R,Bāliš,بالش,بالش، بالس، والش، والشتان,SE_IRAN_656E286N_R,regions,Point,"(67.65738, 29.64265)"
 BALIS_380E360N_S,Bālis,بالس,بالس,SHAM_363E335N_R,towns,Point,"(38.09005, 36.02806)"
 BALJA_130E376N_S,Balǧaŧ,بلجة,بلجة,SIQILIYYA_145E375N_R,towns,Point,"(13.02806, 37.67797)"
 BALKHAB_478E393N_S,Balḫāb,بلخاب,بلخاب، تلخاب,QABQ_457E413N_R,villages,Point,"(47.82733, 39.34245)"
 BALKHAN_660E375N_S,Balḫān,بلخان,بلخان,MAWARANNAHR_656E401N_R,waystations,Point,"(66.00329, 37.51897)"
-BALKH_668E367N_R,Balḫ,بلخ,بلخ,,regions,Point,"(66.88305, 36.78497)"
 BALKH_668E367N_S,Balḫ,بلخ,بلخ,NE_IRAN_606E351N_R,capitals,Point,"(66.88305, 36.78497)"
 BALQA_359E320N_R,al-Balqāʾ,البلقاء,البلقاء,SHAM_363E335N_R,regions,Point,"(35.96379, 32.08487)"
 BALUR_520E358N_S,Balūr,بلور,بلور، بلور,NW_IRAN_515E356N_R,waystations,Point,"(52.0667, 35.81911)"
 BAMAQARA_393E377N_S,Bāmaqarā,بامقرا,بامقرا، بامقدة,JAZIRA_420E364N_R,waystations,Point,"(39.3345, 37.75537)"
-BAMIYAN_678E348N_R,al-Bāmiyān,الباميان,الباميان,,regions,Point,"(67.80206, 34.84737)"
 BAMIYAN_678E348N_S,al-Bāmiyān,الباميان,الباميان,NE_IRAN_606E351N_R,capitals,Point,"(67.80206, 34.84737)"
 BAMM_583E291N_S,Bamm,بم,بم,SW_IRAN_540E294N_R,capitals,Point,"(58.34327, 29.10304)"
 BANAKATH_688E407N_S,Banākaṯ,بناكث,بناكث,MAWARANNAHR_656E401N_R,towns,Point,"(68.80969, 40.71867)"
 BANATJARM_427E192N_O,Banāt Ǧarm,بنات جرم,بنات جرم، بنات حرم، بنات حرب,CENTRAL_ARABIA_416E227N_R,sites,Point,"(42.7829, 19.20706)"
 BANDANIJAN_454E337N_S,Bandanīǧān,بندنيجان,بندنيجان، بندنيجين,IRAQ_459E319N_R,towns,Point,"(45.48927, 33.71797)"
 BAND_620E260N_S,Band,بند,بند، بيذ,SE_IRAN_656E286N_R,towns,Point,"(62.05375, 26.0929)"
 BANHAASAL_311E304N_S,Banhā al-ʿAsal,بنها العسل,بنها العسل,MISR_305E292N_R,towns,Point,"(31.16142, 30.43641)"
@@ -342,15 +318,14 @@
 BARJAH_708E426N_S,Bārǧāḥ,بارجاح,بارجاح، بارجاخ، بارجاج,MAWARANNAHR_656E401N_R,waystations,Point,"(70.80406, 42.62635)"
 BARJAMT_116E330N_S,Bārǧamt,بارجمت,بارجمت، أبار دخت,BARQA_221E314N_R,waystations,Point,"(11.63847, 33.05675)"
 BARKARI_437E389N_S,Barkarī,بركري,بركري، بركوي,QABQ_457E413N_R,towns,Point,"(43.75682, 38.98412)"
 BARKUSH_695E415N_S,Barkūš,بركوش,بركوش,MAWARANNAHR_656E401N_R,towns,Point,"(69.53615, 41.5108)"
 BARM_526E311N_R,Barm,برم,برم,SW_IRAN_540E294N_R,regions,Point,"(52.62743, 31.1799)"
 BARNIQ_200E321N_S,Barnīq,برنيق,برنيق,BARQA_221E314N_R,towns,Point,"(20.08482, 32.11419)"
 BARQAID_420E369N_S,Barqaʿīd,برقعيد,برقعيد,JAZIRA_420E364N_R,towns,Point,"(42.07551, 36.95274)"
-BARQA_208E323N_R,Barqaŧ,برقة,برقة,,regions,Point,"(20.84475, 32.37576)"
 BARQA_208E323N_S,Barqaŧ,برقة,برقة,BARQA_221E314N_R,capitals,Point,"(20.84475, 32.37576)"
 BARSIQ_302E310N_S,Barsīq,برسيق,برسيق,MISR_305E292N_R,towns,Point,"(30.29934, 31.08146)"
 BARTANNA_128E377N_S,Barṭannaŧ,برطنة,برطنة,SIQILIYYA_145E375N_R,towns,Point,"(12.88988, 37.7083)"
 BARTINIQ_131E380N_S,Barṭinīq,برطنيق,برطنيق,SIQILIYYA_145E375N_R,towns,Point,"(13.11223, 38.03112)"
 BARWAN_485E375N_S,Barwān,بروان,بروان,NW_IRAN_515E356N_R,towns,Point,"(48.55981, 37.57057)"
 BARWAN_692E351N_S,Barwān,بروان,بروان، فروان,NE_IRAN_606E351N_R,towns,Point,"(69.25887, 35.17084)"
 BARZAND_478E389N_S,Barzand,برزند,برزند,QABQ_457E413N_R,towns,Point,"(47.85286, 38.96621)"
@@ -364,15 +339,14 @@
 BASIYAN_487E306N_S,Bāsiyān,باسيان,باسيان,SW_IRAN_540E294N_R,towns,Point,"(48.77033, 30.65916)"
 BASMAD_708E291N_S,Basmad,بسمد,بسمد,SE_IRAN_656E286N_R,towns,Point,"(70.8735, 29.12094)"
 BASRA_058W348N_S,Baṣraŧ,بصرة,بصرة,MAGHRIB_045E323N_R,towns,Point,"(-5.88806, 34.82887)"
 BASRA_477E304N_S,al-Baṣraŧ,البصرة,البصرة,IRAQ_459E319N_R,capitals,Point,"(47.71735, 30.40147)"
 BASTA_314E305N_R,Basṭaŧ,بسطة,بسطة,MISR_305E292N_R,regions,Point,"(31.49925, 30.56736)"
 BAS_578E270N_S,Bās,باس,باس,SW_IRAN_540E294N_R,towns,Point,"(57.81535, 27.01075)"
 BATAIH_452E319N_R,al-Baṭāʾiḥ,البطائح,البطائح، البطيحة,IRAQ_459E319N_R,regions,Point,"(45.29796, 31.98716)"
-BATALYUS_069W388N_R,Baṭalyūs,بطليوس,بطليوس، بطليوث,,regions,Point,"(-6.99606, 38.835)"
 BATALYUS_069W388N_S,Baṭalyūs,بطليوس,بطليوس، بطليوث,ANDALUS_040E398N_R,towns,Point,"(-6.99606, 38.835)"
 BATARLIYYA_141E378N_S,Baṭarliyyaŧ,بطرلية,بطرلية,SIQILIYYA_145E375N_R,towns,Point,"(14.13046, 37.81415)"
 BATARNWA_149E375N_S,Baṭarnwaŧ,بطرنوة,بطرنوة، بطرنو,SIQILIYYA_145E375N_R,towns,Point,"(14.91436, 37.57624)"
 BATHANIYYA_361E327N_S,al-Baṯaniyyaŧ,البثنية,البثنية,SHAM_363E335N_R,towns,Point,"(36.15837, 32.72189)"
 BATHA_006E357N_S,al-Baṭḥaŧ,البطحة,البطحة,MAGHRIB_045E323N_R,towns,Point,"(0.60289, 35.78297)"
 BATHRUN_356E342N_S,Baṯrūn,بثرون,بثرون,SHAM_363E335N_R,towns,Point,"(35.67059, 34.25903)"
 BATNMARR_397E216N_S,Baṭn Marr,بطن مر,بطن مر,CENTRAL_ARABIA_416E227N_R,villages,Point,"(39.73935, 21.64499)"
@@ -396,15 +370,14 @@
 BAYRUT_355E339N_S,Bayrūt,بيروت,بيروت,SHAM_363E335N_R,towns,Point,"(35.5091, 33.90162)"
 BAYRUT_479E320N_S,Bayrūt,بيروت,بيروت,SW_IRAN_540E294N_R,towns,Point,"(47.90375, 32.06082)"
 BAYSAN_354E325N_S,Baysān,بيسان,بيسان,SHAM_363E335N_R,towns,Point,"(35.49256, 32.5)"
 BAYSH_425E173N_S,Bayš,بيش,بيش,SW_ARABIA_456E158N_R,towns,Point,"(42.53617, 17.37689)"
 BAYTJIBRIL_348E316N_S,Bayt Ǧibrīl,بيت جبريل,بيت جبريل، بيت جبرين,SHAM_363E335N_R,towns,Point,"(34.88059, 31.60564)"
 BAYTLAHM_351E317N_S,Bayt Laḥm,بيت لحم,بيت لحم,SHAM_363E335N_R,villages,Point,"(35.18792, 31.70926)"
 BAYTMAQDIS_352E317N_S,Bayt al-Maqdis,بيت المقدس,بيت المقدس، القدس، إيليا,SHAM_363E335N_R,towns,Point,"(35.20345, 31.77768)"
-BAYTMAQDIS_352E317N_S,Bayt al-Maqdis,بيت المقدس,بيت المقدس، القدس، إيليا,SHAM_363E335N_R,towns,Point,"(35.20345, 31.77768)"
 BAYTRAM_356E318N_S,Bayt al-Rām,بيت الرام,بيت الرام، بيت رامة، بيت الراس,SHAM_363E335N_R,villages,Point,"(35.60287, 31.80167)"
 BAYYASA_034W379N_S,Bayyāsaŧ,بياسة,بياسة,ANDALUS_040E398N_R,towns,Point,"(-3.45773, 37.9998)"
 BAYYAS_362E367N_S,Bayyās,بياس,بياس,SHAM_363E335N_R,towns,Point,"(36.23856, 36.75139)"
 BAZDA_654E390N_S,Bazdaŧ,بزدة,بزدة,MAWARANNAHR_656E401N_R,towns,Point,"(65.44949, 39.03468)"
 BAZIR_498E316N_S,Bāzīr,بازير,بازير، بازنك,SW_IRAN_540E294N_R,towns,Point,"(49.89265, 31.6409)"
 BAZRANJ_511E299N_R,Bazranǧ,بزرنج,بزرنج,SW_IRAN_540E294N_R,regions,Point,"(51.11281, 29.92934)"
 BIH_613E262N_S,Bih,به,به,,towns,Point,"(61.33378, 26.22927)"
@@ -419,15 +392,14 @@
 BIRA_398E356N_S,Bīrā,بيرا,بيرا,JAZIRA_420E364N_R,villages,Point,"(39.87384, 35.65809)"
 BIRBAR_575E321N_S,Biʾr Bar,بئر بر,بئر بر، جاه بر,SE_IRAN_656E286N_R,waystations,Point,"(57.50413, 32.1335)"
 BIRHUMAYD_681E403N_S,Biʾr Ḥumayd,بئر حميد,بئر حميد,MAWARANNAHR_656E401N_R,waystations,Point,"(68.19849, 40.3886)"
 BIRHUSAYN_679E402N_S,Biʾr al-Ḥusayn,بئر الحسين,بئر الحسين,MAWARANNAHR_656E401N_R,waystations,Point,"(67.99605, 40.23516)"
 BIRSAID_652E392N_S,Biʾr al-Saʿīd,بئر السعيد,بئر السعيد,MAWARANNAHR_656E401N_R,waystations,Point,"(65.29357, 39.2921)"
 BISHA_426E199N_S,Bīšaŧ,بيشة,بيشة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(42.62594, 19.93935)"
 BISHA_426E200N_R,Bīšaŧ,بيشة,بيشة,CENTRAL_ARABIA_416E227N_R,regions,Point,"(42.69682, 20.04402)"
-BISHLANK_648E326N_R,Bišlank,بشلنك,بشلنك,,regions,Point,"(64.81783, 32.6817)"
 BISHLANK_648E326N_S,Bišlank,بشلنك,بشلنك,SE_IRAN_656E286N_R,towns,Point,"(64.81783, 32.6817)"
 BISHSHARA_088E338N_S,Biššará,بشرى,بشرى، بشري,IFRIQIYYA_78E349N_R,towns,Point,"(8.81609, 33.8038)"
 BISKAND_583E360N_S,Bīskand,بيسكند,بيسكند، بيشكند,NE_IRAN_606E351N_R,villages,Point,"(58.39294, 36.08371)"
 BISKARA_057E348N_S,Biskaraŧ,بسكرة,بسكرة,IFRIQIYYA_78E349N_R,towns,Point,"(5.72622, 34.84755)"
 BISKATH_694E408N_S,Biskaṯ,بسكث,بسكث,MAWARANNAHR_656E401N_R,towns,Point,"(69.42766, 40.89646)"
 BISTAMA_307E306N_S,Bistāmaŧ,بستامة,بستامة,MISR_305E292N_R,towns,Point,"(30.78887, 30.62076)"
 BISTAM_550E364N_S,Bisṭām,بسطام,بسطام,NW_IRAN_515E356N_R,towns,Point,"(55.07205, 36.45952)"
@@ -448,15 +420,14 @@
 BUHAYRAMARYUT_299E311N_W,Buḥayraŧ Maryūṭ,بحيرة مريوط,بحيرة مريوط,MISR_305E292N_R,waters,Point,"(29.91455, 31.12142)"
 BUHAYRAMUNTINA_354E313N_W,Buḥayraŧ al-Muntinaŧ,بحيرة المنتنة,بحيرة المنتنة، بحيرة المقلوبة، بحيرة الميتة، بحيرة الصغر,SHAM_363E335N_R,waters,Point,"(35.46173, 31.3845)"
 BUHAYRAQADAS_355E330N_W,Buḥayraŧ Qadas,بحيرة قدس,بحيرة قدس,SHAM_363E335N_R,waters,Point,"(35.59845, 33.06755)"
 BUHAYRATABARIYYA_355E328N_W,Buḥayraŧ Ṭabariyyaŧ,بحيرة طبرية,بحيرة طبرية,SHAM_363E335N_R,waters,Point,"(35.57727, 32.80982)"
 BUHAYRATINNIS_319E312N_W,Buḥayraŧ Tinnīs,بحيرة تنيس,بحيرة تنيس,MISR_305E292N_R,waters,Point,"(31.99133, 31.25935)"
 BUHAYRAURMIYYA_453E377N_W,Buḥayraŧ Urmiyyaŧ,بحيرة أرمية,بحيرة أرمية,QABQ_457E413N_R,waters,Point,"(45.35353, 37.70285)"
 BUHAYRAZARAH_612E314N_W,Buḥayraŧ Zarah,بحيرة زره,بحيرة زره، بحيرة الصنط,SE_IRAN_656E286N_R,waters,Point,"(61.23634, 31.47449)"
-BUKHARA_644E398N_R,Buḫāraŧ,بخارة,بخارة,,regions,Point,"(64.46489, 39.85224)"
 BUKHARA_644E398N_S,Buḫāraŧ,بخارة,بخارة,MAWARANNAHR_656E401N_R,capitals,Point,"(64.46489, 39.85224)"
 BULGHAR_484E541N_R,Bulġār,بلغار,بلغار,QABQ_457E413N_R,regions,Point,"(48.40369, 54.1546)"
 BULGHAR_492E548N_S,Bulġār,بلغار,بلغار,QABQ_457E413N_R,towns,Point,"(49.25044, 54.86714)"
 BULUNYAS_359E351N_S,Bulunyās,بلنياس,بلنياس,SHAM_363E335N_R,towns,Point,"(35.97212, 35.18256)"
 BULYANA_319E262N_S,Bulyanā,بلينا,بلينا,MISR_305E292N_R,towns,Point,"(31.9959, 26.21922)"
 BUMINA_297E309N_S,Būmīnaŧ,بومينة,بومينة، بومينى,MISR_305E292N_R,waystations,Point,"(29.71572, 30.93264)"
 BUMJIKATH_688E397N_S,Būmǧikaṯ,بومجكث,بومجكث، بنجكث، بمجكث,MAWARANNAHR_656E401N_R,capitals,Point,"(68.83442, 39.74616)"
@@ -468,27 +439,23 @@
 BURJ_496E333N_S,al-Burǧ,البرج,البرج,NW_IRAN_515E356N_R,towns,Point,"(49.64019, 33.39951)"
 BURKHUWAR_516E327N_R,Burḫuwār,برخوار,برخوار,NW_IRAN_515E356N_R,regions,Point,"(51.67468, 32.78618)"
 BURNAMADH_681E399N_S,Būrnamaḏ,بورنمذ,بورنمذ، فورنمذ,MAWARANNAHR_656E401N_R,towns,Point,"(68.12909, 39.95059)"
 BURQAD_138E379N_S,Būrqād,بورقاد,بورقاد,SIQILIYYA_145E375N_R,towns,Point,"(13.87795, 37.97731)"
 BURTAS_466E526N_R,Burṭās,برطاس,برطاس,QABQ_457E413N_R,regions,Point,"(46.64374, 52.68645)"
 BURUJIRD_488E339N_S,Burūǧird,بروجرد,بروجرد,NW_IRAN_515E356N_R,capitals,Point,"(48.8094, 33.90164)"
 BURULLUS_309E315N_S,Burullus,برلس,برلس، برلس,MISR_305E292N_R,towns,Point,"(30.99606, 31.58612)"
-BUSANJ_614E343N_R,Būsanǧ,بوسنج,بوسنج، فشنج، بوشنك,,regions,Point,"(61.47787, 34.35023)"
-BUSANJ_614E343N_S,Būsanǧ,بوسنج,بوسنج، فشنج، بوشنك,NE_IRAN_606E351N_R,capitals,Point,"(61.47787, 34.35023)"
 BUSANJ_614E343N_S,Būsanǧ,بوسنج,بوسنج، فشنج، بوشنك,NE_IRAN_606E351N_R,capitals,Point,"(61.47787, 34.35023)"
 BUSFURJAN_456E395N_R,Busfurǧān,بسفرجان,بسفرجان,QABQ_457E413N_R,regions,Point,"(45.61619, 39.54632)"
-BUSHTAFRUSH_592E361N_R,Buštafrūš,بشتفروش,بشتفروش، بستنفروش,,regions,Point,"(59.24061, 36.17813)"
 BUSHTAFRUSH_592E361N_S,Buštafrūš,بشتفروش,بشتفروش، بستنفروش,NE_IRAN_606E351N_R,villages,Point,"(59.24061, 36.17813)"
 BUSHTBADHAM_554E330N_S,Bušt Bāḏām,بشت باذام,بشت باذام,SE_IRAN_656E286N_R,waystations,Point,"(55.41827, 33.02224)"
 BUSHT_582E352N_R,Bušt,بشت,بشت,NE_IRAN_606E351N_R,regions,Point,"(58.27285, 35.2614)"
 BUSIR_311E292N_S,Būṣīr,بوصير,بوصير، بوصير الفيوم، أبوصير، بوصير قوريدس، بوصير الأشمونين,MISR_305E292N_R,towns,Point,"(31.10677, 29.27633)"
 BUSRA_364E325N_S,Buṣrá,بصرى,بصرى,SHAM_363E335N_R,towns,Point,"(36.43071, 32.51503)"
 BUSTADARAN_568E341N_S,Bustadārān,بستداران,بستداران,SE_IRAN_656E286N_R,waystations,Point,"(56.87872, 34.16617)"
 BUSTA_497E351N_S,Būstaŧ,بوستة,بوستة,NW_IRAN_515E356N_R,towns,Point,"(49.74164, 35.13286)"
-BUST_643E313N_R,Bust,بست,بست,,regions,Point,"(64.39078, 31.39108)"
 BUST_643E313N_S,Bust,بست,بست,SE_IRAN_656E286N_R,capitals,Point,"(64.39078, 31.39108)"
 BUTHIRA_142E371N_S,Buṯīraŧ,بثيرة,بثيرة,SIQILIYYA_145E375N_R,towns,Point,"(14.21096, 37.185)"
 BUTIJ_312E271N_S,Būtīǧ,بوتيج,بوتيج,MISR_305E292N_R,towns,Point,"(31.22681, 27.10901)"
 BUTLAMIYYA_383E355N_S,al-Buṭlāmiyyaŧ,البطلامية,البطلامية، الخربة,SHAM_363E335N_R,waystations,Point,"(38.31435, 35.52404)"
 BUTTAM_684E389N_S,al-Buttam,البتم,البتم,MAWARANNAHR_656E401N_R,towns,Point,"(68.49336, 38.95345)"
 BUWAHRIZ_446E337N_S,Buwahriz,بوهرز,بوهرز,IRAQ_459E319N_R,towns,Point,"(44.64201, 33.70578)"
 BUWAYB_315E301N_S,Buwayb,بويب,بويب,MISR_305E292N_R,waystations,Point,"(31.57979, 30.16955)"
@@ -506,20 +473,16 @@
 DAKHILA_287E255N_R,al-Dāḫilaŧ,الداخلة,الداخلة,MISR_305E292N_R,regions,Point,"(28.73902, 25.54178)"
 DAKHWID_512E303N_S,Daḫwīd,دخويد,دخويد، درخيذ,SW_IRAN_540E294N_R,villages,Point,"(51.2582, 30.30738)"
 DALAS_311E292N_S,Dalāṣ,دلاص,دلاص، دلاص,MISR_305E292N_R,towns,Point,"(31.16142, 29.21524)"
 DALIYA_407E347N_S,al-Dāliyaŧ,الدالية,الدالية,JAZIRA_420E364N_R,towns,Point,"(40.74111, 34.71355)"
 DAMANHUR_304E310N_S,Damanhūr,دمنهور,دمنهور,MISR_305E292N_R,towns,Point,"(30.45872, 31.03855)"
 DAMANNASH_154E381N_S,Damannaš,دمنش,دمنش,SIQILIYYA_145E375N_R,towns,Point,"(15.40177, 38.15878)"
 DAMGHAN_543E361N_S,al-Damġān,الدمغان,الدمغان,NW_IRAN_515E356N_R,capitals,Point,"(54.37503, 36.13093)"
-DAMGHAN_543E361N_S,al-Damġān,الدمغان,الدمغان,NW_IRAN_515E356N_R,capitals,Point,"(54.37503, 36.13093)"
-DAMGHAN_543E361N_S,al-Damġān,الدمغان,الدمغان,NW_IRAN_515E356N_R,capitals,Point,"(54.37503, 36.13093)"
 DAMIRA_313E311N_S,Damīraŧ,دميرة,دميرة، دميرة,MISR_305E292N_R,towns,Point,"(31.3504, 31.1414)"
-DAMSIS_312E308N_R,Damsīs,دمسيس,دمسيس,,regions,Point,"(31.22403, 30.82041)"
 DAMSIS_312E308N_S,Damsīs,دمسيس,دمسيس,MISR_305E292N_R,towns,Point,"(31.22403, 30.82041)"
-DAMTH_447E141N_R,Damṯ,دمث,دمث,,regions,Point,"(44.74355, 14.16433)"
 DAMTH_447E141N_S,Damṯ,دمث,دمث,SW_ARABIA_456E158N_R,towns,Point,"(44.74355, 14.16433)"
 DANDANAQAN_616E372N_S,Dandānaqān,دندانقان,دندانقان,NE_IRAN_606E351N_R,towns,Point,"(61.65152, 37.27393)"
 DANDARA_326E261N_R,Dandaraŧ,دندرة,دندرة,,regions,Point,"(32.64544, 26.15778)"
 DANJI_516E329N_S,Dānǧī,دانجي,دانجي,SE_IRAN_656E286N_R,waystations,Point,"(51.67468, 32.90827)"
 DANKAN_423E175N_R,Ḍankān,ضنكان,ضنكان,SW_ARABIA_456E158N_R,regions,Point,"(42.35312, 17.52221)"
 DANK_563E235N_S,Ḍank,ضنك,ضنك,SE_ARABIA_556E220N_R,towns,Point,"(56.30591, 23.53023)"
 DANSHAL_305E309N_S,Danšāl,دنشال,دنشال,MISR_305E292N_R,villages,Point,"(30.51137, 30.95938)"
@@ -554,15 +517,14 @@
 DASKARA_449E339N_S,Daskaraŧ,دسكرة,دسكرة، دسكرة الملك,IRAQ_459E319N_R,towns,Point,"(44.9231, 33.94151)"
 DASKARDAN_566E342N_S,Daskardān,دسكردان,دسكردان، دسكروان,SE_IRAN_656E286N_R,waystations,Point,"(56.60995, 34.25952)"
 DASTAJIRDA_666E368N_S,Dastaǧirdaŧ,دستجردة,دستجردة,NE_IRAN_606E351N_R,villages,Point,"(66.6411, 36.8334)"
 DATHINA_419E232N_S,al-Daṯīnaŧ,الدثينة,الدثينة، دفينة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.92466, 23.22544)"
 DATHINA_458E138N_R,Daṯīnaŧ,دثينة,دثينة,SW_ARABIA_456E158N_R,regions,Point,"(45.89739, 13.81354)"
 DAWMAJANDAL_398E297N_S,Dawmaŧ al-Ǧandal,دومة الجندل,دومة الجندل,CENTRAL_ARABIA_416E227N_R,villages,Point,"(39.87767, 29.75959)"
 DAWQA_409E195N_S,Dawqaŧ,دوقة,دوقة,CENTRAL_ARABIA_416E227N_R,villages,Point,"(40.96521, 19.5605)"
-DAWRAQ_489E308N_R,al-Dawraq,الدورق,الدورق، السراق,,regions,Point,"(48.92625, 30.81069)"
 DAWRAQ_489E308N_S,al-Dawraq,الدورق,الدورق، السراق,SW_IRAN_540E294N_R,capitals,Point,"(48.92625, 30.81069)"
 DAWSAR_384E359N_S,Dawsar,دوسر,دوسر,SHAM_363E335N_R,waystations,Point,"(38.49243, 35.92575)"
 DAYBUL_676E244N_S,al-Daybul,الديبل,الديبل,SE_IRAN_656E286N_R,towns,Point,"(67.69101, 24.43756)"
 DAYLAMAN_505E366N_R,Daylamān,ديلمان,ديلمان، الديلم,NW_IRAN_515E356N_R,regions,Point,"(50.52548, 36.69592)"
 DAYRAQUL_449E329N_S,Dayr al-ʿĀqūl,دير العاقول,دير العاقول,IRAQ_459E319N_R,towns,Point,"(44.9846, 32.91181)"
 DAYRA_493E307N_S,Dayraŧ,ديرة,ديرة,SW_IRAN_540E294N_R,waystations,Point,"(49.32901, 30.78178)"
 DAYRBAZAMA_447E336N_S,Dayr Bāzamaŧ ,دير بازمة ,دير بازمة ،  دير تيرمة,IRAQ_459E319N_R,waystations,Point,"(44.70196, 33.60709)"
@@ -571,15 +533,14 @@
 DAYRUT_304E312N_S,Dayrūṭ,ديروط,ديروط,MISR_305E292N_R,towns,Point,"(30.44535, 31.25059)"
 DAYR_316E265N_R,al-Dayr,الدير,الدير، دير بو شنودة,MISR_305E292N_R,regions,Point,"(31.60625, 26.5449)"
 DAYYAY_307E310N_S,Dayyāy,دياي,دياي,MISR_305E292N_R,towns,Point,"(30.70519, 31.01916)"
 DAZIQI_411E343N_S,Dāziqī,دازقي,دازقي,JAZIRA_420E364N_R,waystations,Point,"(41.1598, 34.33397)"
 DHATHUMAM_293E308N_S,Ḏāt al-Ḥumām,ذات الحمام,ذات الحمام، ذات الحمام,BARQA_221E314N_R,towns,Point,"(29.30208, 30.86496)"
 DHATIRQ_404E216N_S,Ḏāt ʿIrq,ذات عرق,ذات عرق,CENTRAL_ARABIA_416E227N_R,villages,Point,"(40.42853, 21.62677)"
 DHATSAHIL_310E302N_S,Ḏāt al-Sāḥil,ذات الساحل,ذات الساحل,MISR_305E292N_R,waystations,Point,"(31.01228, 30.22134)"
-DHIMAR_443E145N_R,Ḏimār,ذمار,ذمار,,regions,Point,"(44.3972, 14.56364)"
 DHIMAR_443E145N_S,Ḏimār,ذمار,ذمار,SW_ARABIA_456E158N_R,towns,Point,"(44.3972, 14.56364)"
 DHUBHAN_441E132N_R,Ḏubḥān,ذبحان,ذبحان,SW_ARABIA_456E158N_R,regions,Point,"(44.10309, 13.23247)"
 DHUHULAYFA_395E244N_S,Ḏū al-Ḥulayfaŧ,ذو الحليفة,ذو الحليفة,CENTRAL_ARABIA_416E227N_R,villages,Point,"(39.56501, 24.40558)"
 DHUJURRA_446E154N_R,Ḏū Ǧurraŧ,ذو جرة,ذو جرة,SW_ARABIA_456E158N_R,regions,Point,"(44.64961, 15.40346)"
 DHUKHUSHUB_392E247N_S,Ḏū Ḫušub,ذو خشب,ذو خشب,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.29172, 24.72896)"
 DIHBARIST_561E277N_S,Dih Bārist,ده بارست,ده بارست، ده رويست,SW_IRAN_540E294N_R,villages,Point,"(56.13806, 27.7741)"
 DIHISTAN_556E390N_R,Dihistān,دهستان,دهستان,NW_IRAN_515E356N_R,regions,Point,"(55.63466, 39.09457)"
@@ -660,15 +621,14 @@
 FISHA_304E311N_S,Fīšaŧ,فيشة,فيشة,MISR_305E292N_R,villages,Point,"(30.49999, 31.13129)"
 FUDAYN_405E354N_S,al-Fudayn,الفدين,الفدين,JAZIRA_420E364N_R,towns,Point,"(40.59626, 35.4148)"
 FUHAYMA_421E342N_S,al-Fuḥaymaŧ,الفحيمة,الفحيمة,JAZIRA_420E364N_R,villages,Point,"(42.18317, 34.23688)"
 FURAT_383E358N_W,al-Furāt,الفرات,الفرات,SHAM_363E335N_R,waters,Point,"(38.38504, 35.81449)"
 FURDA_407E346N_S,al-Furḍaŧ,الفرضة,الفرضة,JAZIRA_420E364N_R,villages,Point,"(40.78158, 34.679)"
 FURJ_551E283N_S,Furǧ,فرج,فرج,SW_IRAN_540E294N_R,towns,Point,"(55.16805, 28.31921)"
 FUSTAT_312E300N_S,Fusṭāṭ,فسطاط,فسطاط,MISR_305E292N_R,metropoles,Point,"(31.24964, 30.04325)"
-FUSTAT_312E300N_S,Fusṭāṭ,فسطاط,فسطاط,MISR_305E292N_R,metropoles,Point,"(31.24964, 30.04325)"
 FUSTUJAN_540E288N_S,al-Fustuǧān,الفستجان,الفستجان، الفستكان، البستجان,SW_IRAN_540E294N_R,towns,Point,"(54.07735, 28.88371)"
 FUTUQ_412E214N_S,al-Futuq,الفتق,الفتق,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.28101, 21.44752)"
 FUWA_305E312N_S,Fuwaŧ,فوة,فوة,MISR_305E292N_R,towns,Point,"(30.50654, 31.2237)"
 GHADAMIS_094E301N_S,Ġadāmis,غدامس,غدامس,BARQA_221E314N_R,towns,Point,"(9.47597, 30.12935)"
 GHAFIQ_050W386N_S,Ġāfiq,غافق,غافق,ANDALUS_040E398N_R,towns,Point,"(-5.01064, 38.68214)"
 GHALAFIQA_430E144N_S,Ġalāfiqaŧ,غلافقة,غلافقة,SW_ARABIA_456E158N_R,towns,Point,"(43.03243, 14.44273)"
 GHAMRA_408E218N_S,al-Ġamraŧ,الغمرة,الغمرة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(40.84007, 21.89675)"
@@ -676,15 +636,14 @@
 GHARANDAL_351E300N_S,Ġarandal,غرندل,غرندل، عرندل,SHAM_363E335N_R,towns,Point,"(35.17023, 30.03245)"
 GHARDAMAN_603E418N_S,Ġardamān,غردمان,غردمان,MAWARANNAHR_656E401N_R,towns,Point,"(60.37258, 41.88381)"
 GHARJSHAR_644E348N_R,Ġarǧ al-Šār,غرج الشار,غرج الشار، جرجستان,NE_IRAN_606E351N_R,regions,Point,"(64.44388, 34.88273)"
 GHARNATA_035W372N_S,Ġarnāṭaŧ,غرناطة,غرناطة,ANDALUS_040E398N_R,towns,Point,"(-3.5998, 37.20621)"
 GHARWA_498E315N_S,Ġarwaŧ,غروة,غروة، عروة,SW_IRAN_540E294N_R,towns,Point,"(49.89724, 31.54027)"
 GHAWR_354E318N_R,al-Ġawr,الغور,الغور,SHAM_363E335N_R,regions,Point,"(35.48149, 31.86882)"
 GHAYFA_315E303N_S,Ġayfā,غيفا,غيفا,MISR_305E292N_R,towns,Point,"(31.51348, 30.38241)"
-GHAZNA_684E335N_R,Ġaznaŧ,غزنة,غزنة، غزنين,,regions,Point,"(68.40733, 33.56409)"
 GHAZNA_684E335N_S,Ġaznaŧ,غزنة,غزنة، غزنين,NE_IRAN_606E351N_R,capitals,Point,"(68.40733, 33.56409)"
 GHAZZA_344E314N_S,Ġazzaŧ,غزة,غزة,SHAM_363E335N_R,towns,Point,"(34.45664, 31.49664)"
 GHUBAYRA_569E297N_S,Ġubayrāʾ,غبيراء,غبيراء,SW_IRAN_540E294N_R,towns,Point,"(56.97972, 29.72844)"
 GHUDAR_442E158N_R,al-Ġudar,الغدر,الغدر,SW_ARABIA_456E158N_R,regions,Point,"(44.26507, 15.88071)"
 GHUNDIJAN_512E292N_S,al-Ġundiǧān,الغندجان,الغندجان,SW_IRAN_540E294N_R,towns,Point,"(51.26065, 29.22327)"
 GHURAYZ_394E353N_S,al-Ġurayz ,الغريز ,الغريز ، العرير,JAZIRA_420E364N_R,waystations,Point,"(39.46613, 35.32264)"
 GHURRABA_373E313N_S,al-Ġurrabaŧ,الغربة,الغربة,CENTRAL_ARABIA_416E227N_R,towns,Point,"(37.34142, 31.36925)"
@@ -711,58 +670,53 @@
 HAJR_467E246N_S,al-Ḥaǧr,الحجر,الحجر,CENTRAL_ARABIA_416E227N_R,capitals,Point,"(46.73212, 24.64352)"
 HAJUR_435E160N_R,Ḥaǧūr,حجور,حجور,SW_ARABIA_456E158N_R,regions,Point,"(43.51706, 16.00544)"
 HAKAM_429E163N_R,Ḥakam,حكم,حكم,SW_ARABIA_456E158N_R,regions,Point,"(42.94727, 16.37831)"
 HALAB_371E361N_S,Ḥalab,حلب,حلب,SHAM_363E335N_R,capitals,Point,"(37.17518, 36.19828)"
 HALAWARD_687E378N_S,Halāward,هلاورد,هلاورد,MAWARANNAHR_656E401N_R,towns,Point,"(68.78102, 37.83441)"
 HALIMAN_222E327N_S,Ḥalīmān,حليمان,حليمان، جب حليمان,BARQA_221E314N_R,waystations,Point,"(22.203, 32.77902)"
 HALI_413E186N_S,Ḥalī,حلي,حلي,CENTRAL_ARABIA_416E227N_R,towns,Point,"(41.39305, 18.62751)"
-HAMADHAN_485E347N_R,Hamaḏān,همذان,همذان,,regions,Point,"(48.57908, 34.77554)"
 HAMADHAN_485E347N_S,Hamaḏān,همذان,همذان,NW_IRAN_515E356N_R,metropoles,Point,"(48.57908, 34.77554)"
 HAMAD_506E247N_S,Ḥamaḍ,حمض,حمض,SE_ARABIA_556E220N_R,waystations,Point,"(50.65214, 24.74231)"
 HAMA_367E351N_S,Ḥamāŧ,حماة,حماة,SHAM_363E335N_R,towns,Point,"(36.76872, 35.12587)"
 HAMDAN_441E155N_R,Hamdān,همدان,همدان,SW_ARABIA_456E158N_R,regions,Point,"(44.12811, 15.57151)"
 HAMMAMIBNUMAR_443E323N_S,Ḥammām Ibn ʿUmar,حمام إبن عمر,حمام إبن عمر,IRAQ_459E319N_R,towns,Point,"(44.34773, 32.39084)"
 HAMMA_081E340N_S,al-Ḥammaŧ,الحمة,الحمة,IFRIQIYYA_78E349N_R,towns,Point,"(8.19472, 34.0563)"
 HANIYYARUM_288E308N_S,Ḥaniyyaŧ al-Rūm,حنية الروم,حنية الروم، قصور الروم,BARQA_221E314N_R,waystations,Point,"(28.8519, 30.80549)"
 HAQL_350E292N_S,al-Ḥaql,الحقل,الحقل,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(35.03845, 29.27449)"
 HAQL_442E142N_R,al-Ḥaql,الحقل,الحقل,SW_ARABIA_456E158N_R,regions,Point,"(44.23214, 14.25242)"
 HARAZ_437E150N_R,Ḥarāz,حراز,حراز,SW_ARABIA_456E158N_R,regions,Point,"(43.71898, 15.06484)"
 HARA_544E301N_S,Harāŧ,هراة,هراة,SW_IRAN_540E294N_R,towns,Point,"(54.41315, 30.11392)"
-HARA_621E343N_R,Harāŧ,هراة,هراة,,regions,Point,"(62.15235, 34.33419)"
 HARA_621E343N_S,Harāŧ,هراة,هراة,NE_IRAN_606E351N_R,capitals,Point,"(62.15235, 34.33419)"
 HARBA_441E339N_S,Ḥarbá,حربى,حربى,IRAQ_459E319N_R,towns,Point,"(44.18508, 33.95808)"
 HARRAN_390E368N_S,Ḥarrān,حران,حران,JAZIRA_420E364N_R,towns,Point,"(39.08906, 36.88438)"
 HARUNIYYA_450E339N_S,al-Hārūniyya,الهاروني,الهاروني، طرستان,IRAQ_459E319N_R,towns,Point,"(45.01502, 33.97686)"
 HARURI_623E312N_S,Ḥarūrī,حروري,حروري,SE_IRAN_656E286N_R,villages,Point,"(62.39332, 31.2857)"
 HASANIYYA_427E371N_S,al-Ḥasaniyyaŧ,الحسنية,الحسنية,JAZIRA_420E364N_R,towns,Point,"(42.72248, 37.11078)"
 HASHIMJIRD_670E376N_S,Hāšimǧird,هاشمجرد,هاشمجرد,MAWARANNAHR_656E401N_R,towns,Point,"(67.07594, 37.69255)"
 HASHIYYA_398E314N_S,al-Ḥašiyyaŧ,الحشية,الحشية,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.82192, 31.43199)"
 HAWDHAJIB_554E335N_S,Ḥawḍ al-Ḥāǧib,حوض الحاجب,حوض الحاجب,SE_IRAN_656E286N_R,waystations,Point,"(55.43921, 33.57348)"
 HAWD_587E319N_S,al-Ḥawḍ,الحوض,الحوض,SE_IRAN_656E286N_R,waystations,Point,"(58.78635, 31.90091)"
 HAWFGHARBI_304E307N_R,al-Ḥawf al-Ġarbī,الحوف الغربي,الحوف الغربي,MISR_305E292N_R,regions,Point,"(30.43738, 30.75268)"
 HAWFSHARQI_315E305N_R,al-Ḥawf al-Šarqī,الحوف الشرقي,الحوف الشرقي,MISR_305E292N_R,regions,Point,"(31.57495, 30.59137)"
-HAWMAZUTT_497E310N_R,Ḥawmaŧ al-Zuṭṭ,حومة الزط,حومة الزط، الزط,,regions,Point,"(49.71372, 31.05807)"
 HAWMAZUTT_497E310N_S,Ḥawmaŧ al-Zuṭṭ,حومة الزط,حومة الزط، الزط,SW_IRAN_540E294N_R,capitals,Point,"(49.71372, 31.05807)"
 HAWRAN_367E326N_S,al-Ḥawrān,الحوران,الحوران,SHAM_363E335N_R,towns,Point,"(36.73153, 32.65059)"
-HAWRAN_367E326N_S,al-Ḥawrān,الحوران,الحوران,SHAM_363E335N_R,towns,Point,"(36.73153, 32.65059)"
 HAWRA_373E250N_S,al-Ḥawrāʾ,الحوراء,الحوراء,CENTRAL_ARABIA_416E227N_R,towns,Point,"(37.33759, 25.0302)"
 HAWZAN_435E150N_R,Hawzān,هوزان,هوزان,SW_ARABIA_456E158N_R,regions,Point,"(43.50125, 15.0801)"
 HAWZAN_629E359N_S,Ḥawzān,حوزان,حوزان,NE_IRAN_606E351N_R,waystations,Point,"(62.96749, 35.96191)"
 HAYRAN_430E159N_R,Ḥayrān,حيران,حيران,SW_ARABIA_456E158N_R,regions,Point,"(43.03594, 15.96703)"
 HAYS_434E139N_S,Ḥays,حيس,حيس,SW_ARABIA_456E158N_R,towns,Point,"(43.48282, 13.9314)"
 HAYYABDALLAH_244E318N_S,Ḥayy ʿAbd Allãh,حي عبد الله,حي عبد الله,BARQA_221E314N_R,waystations,Point,"(24.49433, 31.87271)"
 HAZARASB_610E412N_S,Hazārāsb,هزاراسب,هزاراسب,MAWARANNAHR_656E401N_R,towns,Point,"(61.09517, 41.2861)"
 HAZAR_524E299N_S,Hazār,هزار,هزار، أزار سابور,SW_IRAN_540E294N_R,towns,Point,"(52.49428, 29.94029)"
 HIJAZ_390E235N_R,al-Ḥiǧāz,الحجاز,الحجاز,CENTRAL_ARABIA_416E227N_R,regions,Point,"(39.02138, 23.51137)"
 HIJRSALIH_379E268N_S,Ḥiǧr Ṣāliḥ,حجر صالح,حجر صالح، الحجر,CENTRAL_ARABIA_416E227N_R,towns,Point,"(37.93999, 26.86125)"
 HIMS_367E347N_S,Ḥimṣ,حمص,حمص,SHAM_363E335N_R,capitals,Point,"(36.72425, 34.73793)"
 HINDUJAN_513E293N_S,Hindūǧān,هندوجان,هندوجان، هنديجان,SW_IRAN_540E294N_R,villages,Point,"(51.30074, 29.39151)"
 HINDUWAN_497E302N_S,Hinduwān,هندوان,هندوان، هنديجان,SW_IRAN_540E294N_R,towns,Point,"(49.70675, 30.25118)"
 HIRA_443E320N_S,al-Ḥīraŧ,الحيرة,الحيرة,IRAQ_459E319N_R,towns,Point,"(44.37232, 32.01734)"
-HIRDA_427E152N_R,al-Ḥirdaŧ,الحردة,الحردة,,regions,Point,"(42.73173, 15.22479)"
 HIRDA_427E152N_S,al-Ḥirdaŧ,الحردة,الحردة,SW_ARABIA_456E158N_R,towns,Point,"(42.73173, 15.22479)"
 HISNBADRA_514E333N_S,Ḥiṣn Badraŧ,حصن بدرة,حصن بدرة,SE_IRAN_656E286N_R,waystations,Point,"(51.46355, 33.39951)"
 HISNBARZUYA_362E356N_S,Ḥiṣn Barzūyaŧ,حصن برزوية,حصن برزوية,SHAM_363E335N_R,waystations,Point,"(36.27118, 35.67547)"
 HISNBULKUNA_042W378N_S,Ḥiṣn Bulkūnaŧ,حصن بلكونة,حصن بلكونة,ANDALUS_040E398N_R,towns,Point,"(-4.22025, 37.87073)"
 HISNIBNUMARA_549E265N_S,Ḥiṣn Ibn ʿUmāraŧ,حصن إبن عمارة,حصن إبن عمارة، قلعة إبن عمارة,SW_IRAN_540E294N_R,waystations,Point,"(54.90122, 26.57451)"
 HISNKAYFA_414E377N_S,Ḥiṣn Kayfā,حصن كيفا,حصن كيفا,JAZIRA_420E364N_R,towns,Point,"(41.42113, 37.70021)"
 HISNMAHDI_483E305N_S,Ḥiṣn Mahdī,حصن مهدي,حصن مهدي,SW_IRAN_540E294N_R,towns,Point,"(48.33301, 30.52571)"
@@ -792,23 +746,20 @@
 IKHNA_306E314N_R,Iḫnā,إخنا,إخنا,MISR_305E292N_R,regions,Point,"(30.65681, 31.46786)"
 IKHNA_307E315N_S,Iḫnā,إخنا,إخنا، أجنا,MISR_305E292N_R,towns,Point,"(30.79, 31.51979)"
 ILAQ_702E407N_R,Īlāq,إيلاق,إيلاق,MAWARANNAHR_656E401N_R,regions,Point,"(70.2074, 40.78508)"
 IMMARA_431E253N_S,Immaraŧ,إمرة,إمرة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.1471, 25.37319)"
 IQLID_526E309N_S,Iqlīd,إقليد,إقليد,SW_IRAN_540E294N_R,villages,Point,"(52.67168, 30.91897)"
 IRD_467E248N_R,al-ʿIrḍ,العرض,العرض,CENTRAL_ARABIA_416E227N_R,regions,Point,"(46.72918, 24.881)"
 ISBAHANAT_540E291N_S,al-Iṣbahānāt,الإصبهانات,الإصبهانات، إصطهبانان,SW_IRAN_540E294N_R,towns,Point,"(54.04351, 29.10684)"
-ISBAHAN_516E326N_R,Iṣbahān,إصبهان,إصبهان، إصفهان,,regions,Point,"(51.65, 32.66855)"
-ISBAHAN_516E326N_S,Iṣbahān,إصبهان,إصبهان، إصفهان، اليهودية,NW_IRAN_515E356N_R,capitals,Point,"(51.65, 32.66855)"
+ISBAHAN_516E326N_S,Iṣbahān,إصبهان,إصبهان، إصفهان، اليهودية، أصبهان,NW_IRAN_515E356N_R,capitals,Point,"(51.65, 32.66855)"
 ISBIDH_599E299N_S,Isbīḏ,إسبيذ,إسبيذ، إسفيد، سبيذ، سفيد، سبيج، سنيج,SE_IRAN_656E286N_R,towns,Point,"(59.96927, 29.91949)"
-ISBIJAB_697E422N_R,Isbīǧāb,إسبيجاب,إسبيجاب,,regions,Point,"(69.75409, 42.23062)"
 ISBIJAB_697E422N_S,Isbīǧāb,إسبيجاب,إسبيجاب,MAWARANNAHR_656E401N_R,capitals,Point,"(69.75409, 42.23062)"
-ISHBILIYYA_059W374N_R,Išbīliyyaŧ,إشبيلية,إشبيلية,,regions,Point,"(-5.96199, 37.4079)"
 ISHBILIYYA_059W374N_S,Išbīliyyaŧ,إشبيلية,إشبيلية,ANDALUS_040E398N_R,towns,Point,"(-5.96199, 37.4079)"
 ISHTIKHAN_668E399N_S,Ištīḫān,إشتيخان,إشتيخان,MAWARANNAHR_656E401N_R,towns,Point,"(66.87902, 39.94544)"
-ISKANDARIYYA_299E311N_S,al-Iskandariyyaŧ,الإسكندرية,الإسكندرية,MISR_305E292N_R,capitals,Point,"(29.90981, 31.1949)"
+ISKANDARIYYA_299E311N_S,al-Iskandariyyaŧ,الإسكندرية,الإسكندرية، اسكندرية,MISR_305E292N_R,capitals,Point,"(29.90981, 31.1949)"
 ISKANDARUNA_361E365N_S,Iskandarūnaŧ,إسكندرونة,إسكندرونة، إسكندريية,SHAM_363E335N_R,towns,Point,"(36.19234, 36.57473)"
 ISKIFAGHAN_663E385N_S,Iskīfaġan,إسكيفغن,إسكيفغن,MAWARANNAHR_656E401N_R,towns,Point,"(66.30707, 38.53462)"
 ISTAKHR_529E299N_S,Iṣṭaḫr,إصطخر,إصطخر,SW_IRAN_540E294N_R,capitals,Point,"(52.92548, 29.97008)"
 ISTIJA_051W375N_S,Istiǧaŧ,إستجة,إستجة,ANDALUS_040E398N_R,towns,Point,"(-5.10865, 37.53493)"
 ITIL_480E462N_S,Itil,إتل,إتل، أتل,QABQ_457E413N_R,capitals,Point,"(48.0869, 46.2788)"
 ITNA_429E148N_S,ʿIṭnaŧ,عطنة,عطنة,SW_ARABIA_456E158N_R,towns,Point,"(42.94507, 14.82308)"
 IYJ_542E289N_S,Iyǧ,إيج,إيج، إيك,SW_IRAN_540E294N_R,towns,Point,"(54.24655, 28.98623)"
@@ -857,15 +808,14 @@
 JAMILA_056E362N_S,Ǧamīlā,جميلا,جميلا,IFRIQIYYA_78E349N_R,towns,Point,"(5.60237, 36.24063)"
 JAMM_523E278N_S,Ǧamm,جم,جم,SW_IRAN_540E294N_R,villages,Point,"(52.39133, 27.8168)"
 JAMUKAT_696E422N_S,Ǧamūkat,جموكت,جموكت,MAWARANNAHR_656E401N_R,towns,Point,"(69.62235, 42.26934)"
 JAM_414E316N_S,al-Ǧamʿ,الجمع,الجمع,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.46573, 31.67372)"
 JAM_605E353N_R,Ǧām,جام,جام,NE_IRAN_606E351N_R,regions,Point,"(60.57003, 35.33837)"
 JANADIL_302E196N_O,al-Ǧanādil,الجنادل,الجنادل,MISR_305E292N_R,sites,Point,"(30.25325, 19.63029)"
 JANADIL_329E240N_O,al-Ǧanādil,الجنادل,الجنادل,MISR_305E292N_R,sites,Point,"(32.92462, 24.01605)"
-JANAD_441E136N_R,al-Ǧanad,الجند,الجند,,regions,Point,"(44.17508, 13.69225)"
 JANAD_441E136N_S,al-Ǧanad,الجند,الجند,SW_ARABIA_456E158N_R,towns,Point,"(44.17508, 13.69225)"
 JANNABA_505E296N_S,Ǧannābaŧ,جنابة,جنابة,SW_IRAN_540E294N_R,towns,Point,"(50.53898, 29.60089)"
 JANZARUDH_569E306N_S,Ǧanzarūḏ,جنزروذ,جنزروذ، جاترود,SW_IRAN_540E294N_R,towns,Point,"(56.92513, 30.67077)"
 JANZA_463E408N_S,Ǧanzaŧ,جنزة,جنزة، جنجة,QABQ_457E413N_R,towns,Point,"(46.38603, 40.81356)"
 JARABULUS_380E368N_S,Ǧarabuluṣ,جربلص,جربلص,SHAM_363E335N_R,towns,Point,"(38.00577, 36.81562)"
 JARAS_141E378N_S,Ǧārās,جاراس,جاراس,SIQILIYYA_145E375N_R,towns,Point,"(14.1894, 37.85376)"
 JARAWAABUAYSH_022W350N_S,Ǧarāwaŧ Abū al-ʿAyš,جراوة أبو العيش,جراوة أبو العيش,MAGHRIB_045E323N_R,towns,Point,"(-2.28691, 35.09519)"
@@ -886,15 +836,14 @@
 JASIM_360E329N_S,Ǧāsim,جاسم,جاسم,SHAM_363E335N_R,waystations,Point,"(36.04321, 32.98099)"
 JAWFHAMDAN_448E155N_R,Ǧawf Hamdān,جوف همدان,جوف همدان,SW_ARABIA_456E158N_R,regions,Point,"(44.81642, 15.59445)"
 JAWFMURAD_454E151N_R,Ǧawf Murād,جوف مراد,جوف مراد,SW_ARABIA_456E158N_R,regions,Point,"(45.44152, 15.10298)"
 JAWLAN_357E330N_S,al-Ǧawlān,الجولان,الجولان,SHAM_363E335N_R,towns,Point,"(35.79833, 33.09084)"
 JAYHAN_355E367N_W,al-Ǧayḥān,الجيحان,الجيحان,SHAM_363E335N_R,waters,Point,"(35.58877, 36.79276)"
 JAYIMAND_598E350N_S,Ǧāyimand,جايمند,جايمند,NE_IRAN_606E351N_R,towns,Point,"(59.84669, 35.04974)"
 JAYYAN_038W377N_S,Ǧayyān,جيان,جيان,ANDALUS_040E398N_R,towns,Point,"(-3.80302, 37.78977)"
-JAYZAN_498E308N_R,al-Ǧāyzan,الجايزن,الجايزن,,regions,Point,"(49.83759, 30.88498)"
 JAYZAN_498E308N_S,al-Ǧāyzan,الجايزن,الجايزن,SW_IRAN_540E294N_R,towns,Point,"(49.83759, 30.88498)"
 JAZAN_425E168N_S,Ǧāzān,جازان,جازان,SW_ARABIA_456E158N_R,towns,Point,"(42.55043, 16.89564)"
 JAZAN_427E169N_R,Ǧāzān,جازان,جازان,SW_ARABIA_456E158N_R,regions,Point,"(42.72032, 16.99054)"
 JAZIRAABUSHARIK_109E370N_S,Ǧazīraŧ Abū Šarīk,جزيرة أبو شريك,جزيرة أبو شريك,IFRIQIYYA_78E349N_R,towns,Point,"(10.99773, 37.03058)"
 JAZIRABANUZAGHANNAYA_030E367N_S,Ǧazīraŧ Banū Zaġannāyaŧ,جزيرة بنو زغناية,جزيرة بنو زغناية,MAGHRIB_045E323N_R,towns,Point,"(3.09046, 36.70793)"
 JAZIRAIBNUMAR_421E372N_R,Ǧazīraŧ Ibn ʿUmar,جزيرة إبن عمر,جزيرة إبن عمر,,regions,Point,"(42.19943, 37.28521)"
 JAZIRAJABALTARIQ_053W361N_S,Ǧazīraŧ Ǧabal Ṭāriq,جزيرة جبل طارق,جزيرة جبل طارق,ANDALUS_040E398N_R,towns,Point,"(-5.33071, 36.16752)"
@@ -934,40 +883,37 @@
 JUBAYL_356E341N_S,Ǧubayl,جبيل,جبيل,SHAM_363E335N_R,towns,Point,"(35.65206, 34.12764)"
 JUBBAMIRA_313E301N_O,Ǧubb ʿAmīraŧ,جب عميرة,جب عميرة,MISR_305E292N_R,sites,Point,"(31.38569, 30.1607)"
 JUBBAWSAJ_273E310N_S,Ǧubb al-ʿAwsaǧ,جب العوسج,جب العوسج,BARQA_221E314N_R,waystations,Point,"(27.30318, 31.04479)"
 JUBBA_401E318N_S,al-Ǧubbaŧ,الجبة,الجبة، المحنة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(40.18305, 31.84948)"
 JUBBHAMMAD_632E385N_S,Ǧubb Ḥammād,جب حماد,جب حماد,NE_IRAN_606E351N_R,waystations,Point,"(63.20339, 38.58258)"
 JUBBMAYDAN_233E321N_S,Ǧubb al-Maydān,جب الميدان,جب الميدان، جب الميدعان,BARQA_221E314N_R,waystations,Point,"(23.31692, 32.18179)"
 JUBBYUSUF_355E329N_S,Ǧubb Yūsuf,جب يوسف,جب يوسف,SHAM_363E335N_R,villages,Point,"(35.52565, 32.92434)"
-JUBLAN_436E142N_R,Ǧublān,جبلان,جبلان,,regions,Point,"(43.67157, 14.2788)"
 JUBLAN_436E142N_S,Ǧublān,جبلان,جبلان,SW_ARABIA_456E158N_R,towns,Point,"(43.67157, 14.2788)"
 JUDAD_410E217N_S,al-Ǧudad,الجدد,الجدد,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.07197, 21.733)"
 JUDDA_391E214N_S,Ǧuddaŧ,جدة,جدة,CENTRAL_ARABIA_416E227N_R,towns,Point,"(39.1779, 21.46201)"
 JUHFA_391E226N_S,al-Ǧuḥfaŧ,الجحفة,الجحفة,CENTRAL_ARABIA_416E227N_R,towns,Point,"(39.12422, 22.60833)"
 JULLAB_389E374N_S,Ǧullāb,جلاب,جلاب,JAZIRA_420E364N_R,waystations,Point,"(38.91048, 37.41051)"
 JULLAFAR_559E257N_S,Ǧullafār,جلفار,جلفار,SE_ARABIA_556E220N_R,towns,Point,"(55.98855, 25.75227)"
 JULSHUB_724E428N_S,Ǧūl Šūb,جول شوب,جول شوب,MAWARANNAHR_656E401N_R,waystations,Point,"(72.4972, 42.89268)"
 JUL_747E428N_S,Ǧūl,جول,جول,MAWARANNAHR_656E401N_R,waystations,Point,"(74.79378, 42.84796)"
 JUNAYNA_371E279N_S,al-Ǧunaynaŧ,الجنينة,الجنينة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(37.19786, 27.92136)"
 JUNBADHMALLAGHAN_508E302N_S,Ǧunbaḏ Mallaġān,جنبذ ملغان,جنبذ ملغان، جنبذ ملجان,SW_IRAN_540E294N_R,towns,Point,"(50.84951, 30.29389)"
-JUNDAYSABUR_485E322N_R,Ǧundaysābūr,جنديسابور,جنديسابور,,regions,Point,"(48.53919, 32.29866)"
 JUNDAYSABUR_485E322N_S,Ǧundaysābūr,جنديسابور,جنديسابور,SW_IRAN_540E294N_R,capitals,Point,"(48.53919, 32.29866)"
 JUNIYYA_356E339N_S,Ǧuniyyaŧ,جنية,جنية,SHAM_363E335N_R,towns,Point,"(35.61897, 33.98398)"
 JURAB_489E342N_S,Ǧūrāb,جوراب,جوراب,NW_IRAN_515E356N_R,waystations,Point,"(48.90536, 34.21059)"
 JURASH_358E322N_S,Ǧuraš,جرش,جرش,SHAM_363E335N_R,towns,Point,"(35.8804, 32.27309)"
 JURASH_424E187N_R,Ǧuraš,جرش,جرش,CENTRAL_ARABIA_416E227N_R,regions,Point,"(42.44873, 18.77618)"
 JURASH_426E186N_S,Ǧuraš,جرش,جرش,CENTRAL_ARABIA_416E227N_R,towns,Point,"(42.69682, 18.63711)"
 JURASIYYAT_308E303N_S,al-Ǧurasiyyāt,الجرسيات,الجرسيات,MISR_305E292N_R,villages,Point,"(30.89161, 30.34164)"
 JURJANIYYASUGHRA_593E422N_S,Ǧurǧāniyyaŧ al-Ṣuġrá,جرجانية الصغرى,جرجانية الصغرى,MAWARANNAHR_656E401N_R,towns,Point,"(59.31292, 42.28887)"
 JURJANIYYA_592E424N_S,al-Ǧurǧāniyyaŧ,الجرجانية,الجرجانية,MAWARANNAHR_656E401N_R,capitals,Point,"(59.21993, 42.45632)"
 JURJAN_549E373N_R,Ǧurǧān,جرجان,جرجان,NW_IRAN_515E356N_R,regions,Point,"(54.99028, 37.33269)"
 JURJAN_552E371N_R,Ǧurǧān,جرجان,جرجان,,regions,Point,"(55.206, 37.19091)"
 JURJIR_321E309N_S,Ǧurǧīr,جرجير,جرجير,MISR_305E292N_R,towns,Point,"(32.19454, 30.91373)"
 JURZAN_432E425N_R,Ǧurzān,جرزان,جرزان,QABQ_457E413N_R,regions,Point,"(43.20001, 42.55502)"
-JURZUWAN_658E358N_R,al-Ǧurzuwān,الجرزوان,الجرزوان,,regions,Point,"(65.87895, 35.88517)"
 JURZUWAN_658E358N_S,al-Ǧurzuwān,الجرزوان,الجرزوان,NE_IRAN_606E351N_R,towns,Point,"(65.87895, 35.88517)"
 JUR_525E288N_S,Ǧūr,جور,جور، بيروزاباذ,SW_IRAN_540E294N_R,towns,Point,"(52.58324, 28.84797)"
 JUSADA_427E195N_S,Ǧusadāʾ,جسداء,جسداء,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(42.71961, 19.51994)"
 JUSIYA_365E344N_S,Ǧūsiyaŧ,جوسية,جوسية,SHAM_363E335N_R,towns,Point,"(36.56409, 34.44699)"
 JUWAYMABUAHMAD_539E281N_S,Ǧuwaym Abū Aḥmad,جويم أبو أحمد,جويم أبو أحمد,SW_IRAN_540E294N_R,villages,Point,"(53.94661, 28.14336)"
 JUWAYM_522E298N_S,Ǧuwaym,جويم,جويم,SW_IRAN_540E294N_R,villages,Point,"(52.29587, 29.87379)"
 JUWAYN_566E368N_R,Ǧuwayn,جوين,جوين، كويان,NE_IRAN_606E351N_R,regions,Point,"(56.69972, 36.86045)"
@@ -994,29 +940,26 @@
 KALIF_663E373N_S,Kālif,كالف,كالف,MAWARANNAHR_656E401N_R,towns,Point,"(66.31581, 37.37958)"
 KALLAR_519E307N_S,Kallār,كلار,كلار,SW_IRAN_540E294N_R,villages,Point,"(51.92199, 30.72449)"
 KALWADHAR_531E298N_S,Kalwaḏār,كلوذار,كلوذار، قلوذر، قرية الحمام,SW_IRAN_540E294N_R,waystations,Point,"(53.16886, 29.88067)"
 KALWADHA_444E333N_S,Kalwāḏá,كلواذى,كلواذى,IRAQ_459E319N_R,towns,Point,"(44.43153, 33.30144)"
 KALWAN_646E261N_R,Kalwān,كلوان,كلوان، كلوان,SE_IRAN_656E286N_R,regions,Point,"(64.6656, 26.16004)"
 KAMAKH_390E395N_S,Kamaḫ,كمخ,كمخ، كماخ,JAZIRA_420E364N_R,waystations,Point,"(39.02492, 39.58627)"
 KAMFAYRUZ_519E305N_R,Kām Fayrūz,كام فيروز,كام فيروز,SW_IRAN_540E294N_R,regions,Point,"(51.90116, 30.50943)"
-KAMIN_531E301N_R,Kamīn,كمين,كمين,,regions,Point,"(53.16106, 30.17019)"
 KAMIN_531E301N_S,Kamīn,كمين,كمين,SW_IRAN_540E294N_R,villages,Point,"(53.16106, 30.17019)"
 KANAISHADID_279E309N_S,Kanāʾis al-Ḥadīd,كنائس الحديد,كنائس الحديد، كنائس الحرير,BARQA_221E314N_R,waystations,Point,"(27.94768, 30.91449)"
 KANBAYA_725E223N_S,Kanbāyaŧ,كنباية,كنباية,SE_IRAN_656E286N_R,towns,Point,"(72.56065, 22.35228)"
 KANDAK_667E383N_S,Kandak,كندك,كندك,MAWARANNAHR_656E401N_R,villages,Point,"(66.78829, 38.37384)"
 KANDARAM_646E353N_S,Kandaram,كندرم,كندرم,NE_IRAN_606E351N_R,towns,Point,"(64.60334, 35.33988)"
 KAND_705E402N_S,Kand,كند,كند,MAWARANNAHR_656E401N_R,towns,Point,"(70.51735, 40.29225)"
 KANISA_349E327N_S,al-Kanīsaŧ,الكنيسة,الكنيسة,SHAM_363E335N_R,villages,Point,"(34.95381, 32.7475)"
 KANJABADH_639E357N_S,Kanǧābāḏ,كنجاباذ,كنجاباذ,NE_IRAN_606E351N_R,waystations,Point,"(63.98233, 35.78873)"
 KANJRUSTAQ_624E350N_R,Kanǧ Rustāq,كنج رستاق,كنج رستاق,NE_IRAN_606E351N_R,regions,Point,"(62.46952, 35.0772)"
 KARAH_613E344N_S,Karah,كره,كره,NE_IRAN_606E351N_R,towns,Point,"(61.32587, 34.42834)"
-KARAJ_495E338N_R,al-Karaǧ,الكرج,الكرج، كرج أبو دلف,,regions,Point,"(49.54697, 33.88116)"
 KARAJ_495E338N_S,al-Karaǧ,الكرج,الكرج، كرج أبو دلف,NW_IRAN_515E356N_R,capitals,Point,"(49.54697, 33.88116)"
 KARAK_356E311N_S,Karak,كرك,كرك,SHAM_363E335N_R,villages,Point,"(35.69038, 31.17824)"
-KARAK_356E311N_S,Karak,كرك,كرك,SHAM_363E335N_R,villages,Point,"(35.69038, 31.17824)"
 KARA_531E307N_S,Karaŧ,كرة,كرة,SW_IRAN_540E294N_R,towns,Point,"(53.12982, 30.73791)"
 KARBALA_440E326N_S,Karbalāʾ,كربلاء,كربلاء,IRAQ_459E319N_R,towns,Point,"(44.03706, 32.61792)"
 KARBANK_689E373N_S,Kārbank,كاربنك,كاربنك,MAWARANNAHR_656E401N_R,towns,Point,"(68.92955, 37.32188)"
 KARB_542E282N_S,Karb,كرب,كرب,SW_IRAN_540E294N_R,waystations,Point,"(54.21531, 28.26649)"
 KARDARANKHAS_606E413N_S,Kardarānḫās,كردرانخاس,كردرانخاس، كردرانخواش,MAWARANNAHR_656E401N_R,towns,Point,"(60.68254, 41.38937)"
 KARDAR_597E428N_S,Kardar,كردر,كردر، كردر، كردر,MAWARANNAHR_656E401N_R,towns,Point,"(59.79383, 42.80533)"
 KARDIZ_691E336N_S,Kardīz,كرديز,كرديز,SE_IRAN_656E286N_R,waystations,Point,"(69.15407, 33.62249)"
@@ -1027,15 +970,14 @@
 KARKH_443E333N_S,al-Karḫ,الكرخ,الكرخ,IRAQ_459E319N_R,quarters,Point,"(44.35293, 33.31703)"
 KARKUYAH_617E312N_S,Karkūyah,كركويه,كركويه,SE_IRAN_656E286N_R,towns,Point,"(61.74272, 31.26104)"
 KARKUYA_040W388N_S,Karkūyaŧ,كركوية,كركوية,ANDALUS_040E398N_R,towns,Point,"(-4.06918, 38.81784)"
 KARMIINIYYA_654E401N_S,Karmiīniyyaŧ,كرمينية,كرمينية,MAWARANNAHR_656E401N_R,towns,Point,"(65.40937, 40.14581)"
 KARUKH_625E344N_S,Karūḫ,كروخ,كروخ,NE_IRAN_606E351N_R,towns,Point,"(62.54651, 34.47814)"
 KARU_516E317N_S,Karū,كرو,كرو,SW_IRAN_540E294N_R,waystations,Point,"(51.69552, 31.79256)"
 KARWAN_517E324N_R,Karwān,كروان,كروان,NW_IRAN_515E356N_R,regions,Point,"(51.72677, 32.40272)"
-KARWAN_718E414N_R,Karwān,كروان,كروان,,regions,Point,"(71.83079, 41.48396)"
 KARWAN_718E414N_S,Karwān,كروان,كروان,MAWARANNAHR_656E401N_R,capitals,Point,"(71.83079, 41.48396)"
 KARYAN_537E280N_S,Kāryān,كاريان,كاريان,SW_IRAN_540E294N_R,waystations,Point,"(53.70323, 28.05935)"
 KARYUN_301E311N_S,al-Karyūn,الكريون,الكريون، كريون,MISR_305E292N_R,towns,Point,"(30.13142, 31.14286)"
 KARZIN_531E284N_S,Kārzin,كارزن,كارزن,SW_IRAN_540E294N_R,villages,Point,"(53.11293, 28.40599)"
 KASAN_716E412N_S,Kāsān,كاسان,كاسان,MAWARANNAHR_656E401N_R,towns,Point,"(71.64288, 41.24406)"
 KASBA_655E389N_S,Kasbaŧ,كسبة,كسبة,MAWARANNAHR_656E401N_R,towns,Point,"(65.5409, 38.9315)"
 KASHAN_645E358N_S,Kasḥān,كسحان,كسحان,NE_IRAN_606E351N_R,waystations,Point,"(64.54957, 35.88354)"
@@ -1108,15 +1050,14 @@
 KHAWST_588E327N_S,Ḫawst,خوست,خوست,SE_IRAN_656E286N_R,villages,Point,"(58.87551, 32.77833)"
 KHAYAR_539E292N_S,Ḫayār,خيار,خيار، خير، خيرة,SW_IRAN_540E294N_R,villages,Point,"(53.93868, 29.25944)"
 KHAYBAR_392E257N_S,Ḫaybar,خيبر,خيبر,CENTRAL_ARABIA_416E227N_R,towns,Point,"(39.26821, 25.78667)"
 KHAYLAM_709E411N_S,Ḫaylām,خيلام,خيلام، خيرلم,MAWARANNAHR_656E401N_R,capitals,Point,"(70.99972, 41.13472)"
 KHAYM_395E223N_S,al-Ḫaym,الخيم,الخيم، خيم أم معبد، قديد,CENTRAL_ARABIA_416E227N_R,villages,Point,"(39.56795, 22.38571)"
 KHAYSAR_625E342N_S,Ḫaysār,خيسار,خيسار,NE_IRAN_606E351N_R,towns,Point,"(62.58466, 34.27292)"
 KHAYSAR_673E324N_S,Ḫāysār,خايسار,خايسار، خابشان، خابسار,SE_IRAN_656E286N_R,villages,Point,"(67.33448, 32.4844)"
-KHAYWAN_440E162N_R,Ḫaywān,خيوان,خيوان,,regions,Point,"(44.06424, 16.29079)"
 KHAYWAN_440E162N_S,Ḫaywān,خيوان,خيوان,SW_ARABIA_456E158N_R,towns,Point,"(44.06424, 16.29079)"
 KHAZANA_546E323N_S,Ḫazānaŧ,خزانة,خزانة، خرانة,SE_IRAN_656E286N_R,villages,Point,"(54.65669, 32.32168)"
 KHAZAR_475E474N_R,al-Ḫazar,الخزر,الخزر,QABQ_457E413N_R,regions,Point,"(47.55892, 47.42616)"
 KHIRBAQAWM_261E313N_S,Ḫirbaŧ al-Qawm,خربة القوم,خربة القوم,BARQA_221E314N_R,waystations,Point,"(26.11423, 31.35376)"
 KHIWAH_603E413N_S,Ḫīwah,خيوه,خيوه,MAWARANNAHR_656E401N_R,towns,Point,"(60.33577, 41.38465)"
 KHIZANA_425E339N_S,al-Ḫizānaŧ,الخزانة,الخزانة,JAZIRA_420E364N_R,waystations,Point,"(42.50069, 33.9843)"
 KHUDIMANKAN_655E401N_S,Ḫudīmankān,خديمنكان,خديمنكان,MAWARANNAHR_656E401N_R,towns,Point,"(65.58856, 40.12063)"
@@ -1134,30 +1075,28 @@
 KHUNDAB_492E344N_S,Ḫundāb,خنداب,خنداب,NW_IRAN_515E356N_R,waystations,Point,"(49.27004, 34.41215)"
 KHURMUQ_513E286N_R,Ḫurmuq,خرمق,خرمق,SW_IRAN_540E294N_R,regions,Point,"(51.39095, 28.66191)"
 KHURRAMA_533E295N_S,Ḫurrāmaŧ,خرامة,خرامة,SW_IRAN_540E294N_R,towns,Point,"(53.33817, 29.54292)"
 KHURRA_519E292N_S,Ḫurraŧ,خرة,خرة,SW_IRAN_540E294N_R,towns,Point,"(51.9773, 29.22327)"
 KHUR_584E329N_S,Ḫūr,خور,خور,SE_IRAN_656E286N_R,towns,Point,"(58.45153, 32.93881)"
 KHUSHAF_376E360N_S,Ḫušāf,خشاف,خشاف,SHAM_363E335N_R,towns,Point,"(37.69991, 36.0863)"
 KHUSHNABADH_552E287N_S,Ḫušnābāḏ,خشناباذ,خشناباذ، حسناباذ,SW_IRAN_540E294N_R,waystations,Point,"(55.24354, 28.71262)"
-KHUSHUNUBA_079W370N_R,Ḫušunubaŧ,خشنبة,خشنبة، أخشنبة,,regions,Point,"(-7.90515, 37.06463)"
 KHUSHUNUBA_079W370N_S,Ḫušunubaŧ,خشنبة,خشنبة، أخشنبة,ANDALUS_040E398N_R,towns,Point,"(-7.90515, 37.06463)"
 KHUSIKAN_524E305N_S,Ḫūsikān,خوسكان,خوسكان,SW_IRAN_540E294N_R,waystations,Point,"(52.48426, 30.5027)"
 KHUSRAWJIRD_574E361N_S,Ḫusrawǧird,خسروجرد,خسروجرد,NE_IRAN_606E351N_R,towns,Point,"(57.47851, 36.18956)"
 KHUTTAL_697E379N_R,al-Ḫuttal,الختل,الختل,MAWARANNAHR_656E401N_R,regions,Point,"(69.75285, 37.94076)"
 KHUWAKAND_710E405N_S,Ḫuwākand,خواكند,خواكند,MAWARANNAHR_656E401N_R,towns,Point,"(71.05784, 40.55623)"
 KHUWARIZM_599E416N_R,Ḫuwārizm,خوارزم,خوارزم,MAWARANNAHR_656E401N_R,regions,Point,"(59.97545, 41.65733)"
 KHUWAR_524E352N_S,al-Ḫuwār,الخوار,الخوار,NW_IRAN_515E356N_R,towns,Point,"(52.40859, 35.26209)"
 KHUWI_449E385N_S,Ḫuwī,خوي,خوي، خوي، خويت,QABQ_457E413N_R,towns,Point,"(44.99055, 38.5865)"
 KHUZAYMIYYA_431E279N_S,al-Ḫuzaymiyyaŧ,الخزيمية,الخزيمية,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.13666, 27.91046)"
 KIJ_630E260N_S,Kīǧ,كيج,كيج، كيز,SE_IRAN_656E286N_R,towns,Point,"(63.09359, 26.02584)"
 KILABA_360E275N_S,Kilābaŧ,كلابة,كلابة، كلاية,CENTRAL_ARABIA_416E227N_R,villages,Point,"(36.07695, 27.50168)"
 KINDAWASAKUN_486E153N_R,Kindaŧ wa Sakūn,كندة و سكون,كندة و سكون,SW_ARABIA_456E158N_R,regions,Point,"(48.67779, 15.30551)"
 KIRAND_523E284N_S,Kīrand,كيرند,كيرند,SW_IRAN_540E294N_R,waystations,Point,"(52.36569, 28.41977)"
 KISHSH_623E301N_S,Kišš,كش,كش، كس,SE_IRAN_656E286N_R,towns,Point,"(62.37889, 30.15265)"
-KISHSH_668E390N_R,Kišš,كش,كش، كش,,regions,Point,"(66.84071, 39.03102)"
 KISHSH_668E390N_S,Kišš,كش,كش، كش,MAWARANNAHR_656E401N_R,capitals,Point,"(66.84071, 39.03102)"
 KIT_590E420N_S,Kīt,كيت,كيت، جيت,MAWARANNAHR_656E401N_R,towns,Point,"(59.02814, 42.09511)"
 KIZKANAN_665E290N_S,Kīzkānān,كيزكانان,كيزكانان,SE_IRAN_656E286N_R,towns,Point,"(66.57332, 29.0222)"
 KUBAL_762E432N_S,Kubāl,كبال,كبال,MAWARANNAHR_656E401N_R,villages,Point,"(76.21861, 43.21825)"
 KUBAN_328E231N_S,Kubān,كبان,كبان، قبان,MISR_305E292N_R,waystations,Point,"(32.8863, 23.12192)"
 KUDAYY_418E205N_S,Kudayy,كدي,كدي,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.8722, 20.55409)"
 KUFA_443E320N_S,al-Kūfaŧ,الكوفة,الكوفة,IRAQ_459E319N_R,capitals,Point,"(44.39355, 32.03808)"
@@ -1200,36 +1139,32 @@
 LAHJ_448E130N_S,Laḥǧ,لحج,لحج، لهج,SW_ARABIA_456E158N_R,towns,Point,"(44.86953, 13.06747)"
 LAHUN_309E292N_S,al-Lāhūn,اللاهون,اللاهون,MISR_305E292N_R,towns,Point,"(30.99122, 29.24901)"
 LAJJUN_352E326N_S,al-Laǧǧūn,اللجون,اللجون,SHAM_363E335N_R,towns,Point,"(35.27017, 32.60823)"
 LANTINI_150E372N_S,Lantīnī,لنتيني,لنتيني,SIQILIYYA_145E375N_R,towns,Point,"(15.02478, 37.29252)"
 LARIDA_006E416N_S,Lāridaŧ,لاردة,لاردة,ANDALUS_040E398N_R,waystations,Point,"(0.64889, 41.60948)"
 LASHTAR_482E338N_S,Lāštar,لاشتر,لاشتر,NW_IRAN_515E356N_R,villages,Point,"(48.25553, 33.8675)"
 LAWAKAND_690E379N_S,Lāwakand,لاوكند,لاوكند,MAWARANNAHR_656E401N_R,towns,Point,"(69.04582, 37.95639)"
-LIBIRA_036W372N_R,Libīraŧ,لبيرة,لبيرة، إلبيرة,,regions,Point,"(-3.66814, 37.22734)"
 LIBIRA_036W372N_S,Libīraŧ,لبيرة,لبيرة، إلبيرة,ANDALUS_040E398N_R,towns,Point,"(-3.66814, 37.22734)"
 LISHBUNA_091W387N_S,Lišbūnaŧ,لشبونة,لشبونة,ANDALUS_040E398N_R,towns,Point,"(-9.14514, 38.76878)"
 LITH_403E201N_S,al-Līṯ,الليث,الليث,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(40.33707, 20.18053)"
 LIYUN_055W426N_S,Liyūn,ليون,ليون,ANDALUS_040E398N_R,towns,Point,"(-5.56634, 42.6185)"
 LUDD_348E319N_S,Ludd,لد,لد,SHAM_363E335N_R,villages,Point,"(34.88482, 31.95598)"
 LURBUS_088E361N_S,Lurbus,لربس,لربس، الأربس,IFRIQIYYA_78E349N_R,towns,Point,"(8.83937, 36.10562)"
 LURDAJAN_507E315N_S,Lūrdaǧān,لوردجان,لوردجان، اللورجان,SW_IRAN_540E294N_R,towns,Point,"(50.73914, 31.53831)"
 LURQA_017W376N_S,Lurqaŧ,لرقة,لرقة,ANDALUS_040E398N_R,towns,Point,"(-1.73128, 37.6532)"
-LURQA_017W376N_S,Lurqaŧ,لرقة,لرقة,ANDALUS_040E398N_R,towns,Point,"(-1.73128, 37.6532)"
 LUR_483E325N_R,al-Lūr,اللور,اللور,SW_IRAN_540E294N_R,regions,Point,"(48.30291, 32.53782)"
 MAAB_357E312N_S,Maʾāb,مآب,مآب، مؤاب,SHAM_363E335N_R,towns,Point,"(35.73272, 31.2579)"
 MAADINTIBR_333E226N_O,Maʿādin al-Tibr,معادن التبر,معادن التبر,MISR_305E292N_R,sites,Point,"(33.35835, 22.61001)"
 MAADINZUMURRUDH_338E250N_O,Maʿādin al-Zumurruḏ,معادن الزمرذ,معادن الزمرذ,MISR_305E292N_R,sites,Point,"(33.89324, 25.07556)"
 MAAFIR_445E132N_R,al-Maʿāfir,المعافر,المعافر,SW_ARABIA_456E158N_R,regions,Point,"(44.52977, 13.22221)"
 MAAN_357E301N_S,Maʿān,معان,معان، معان,SHAM_363E335N_R,towns,Point,"(35.72442, 30.19664)"
 MAARRANUMAN_366E356N_S,Maʿarraŧ al-Nuʿmān,معرة النعمان,معرة النعمان,SHAM_363E335N_R,towns,Point,"(36.69124, 35.64344)"
-MAARRANUMAN_366E356N_S,Maʿarraŧ al-Nuʿmān,معرة النعمان,معرة النعمان,SHAM_363E335N_R,towns,Point,"(36.69124, 35.64344)"
 MAARRAQINNASRIN_366E360N_S,Maʿarraŧ Qinnasrīn,معرة قنسرين,معرة قنسرين,SHAM_363E335N_R,towns,Point,"(36.69667, 36.01376)"
 MABARBADHAKHSHAN_699E375N_O,Maʿbar Baḏaḫšān,معبر بذخشان,معبر بذخشان,MAWARANNAHR_656E401N_R,sites,Point,"(69.90205, 37.5917)"
 MADAIN_445E330N_S,al-Madāʾīn,المدائين,المدائين,IRAQ_459E319N_R,towns,Point,"(44.59672, 33.09075)"
-MADAIN_445E330N_S,al-Madāʾīn,المدائين,المدائين,IRAQ_459E319N_R,towns,Point,"(44.59672, 33.09075)"
 MADALLIN_059W389N_S,Madallīn,مدلين,مدلين,ANDALUS_040E398N_R,towns,Point,"(-5.94131, 38.93229)"
 MADAN_091W386N_S,al-Maʿdan,المعدن,المعدن,ANDALUS_040E398N_R,towns,Point,"(-9.19189, 38.64984)"
 MADHARWISTAN_460E344N_S,Māḏarwistān,ماذروستان,ماذروستان,NW_IRAN_515E356N_R,waystations,Point,"(46.04283, 34.43477)"
 MADHAR_473E314N_S,al-Maḏār,المذار,المذار,IRAQ_459E319N_R,towns,Point,"(47.37621, 31.48197)"
 MADHAR_678E353N_S,Maḏar,مذر,مذر,NE_IRAN_606E351N_R,towns,Point,"(67.85287, 35.38044)"
 MADHAWAN_542E287N_S,al-Māḏawan,الماذون,الماذون,SW_IRAN_540E294N_R,towns,Point,"(54.29861, 28.72175)"
 MADHMINIYYA_593E426N_S,Maḏmīniyyaŧ,مذمينية,مذمينية، مدكمينية !,MAWARANNAHR_656E401N_R,towns,Point,"(59.30953, 42.67871)"
@@ -1250,15 +1185,14 @@
 MAHALLAMAHRUM_309E307N_S,Maḥallaŧ al-Maḥrūm,محلة المحروم,محلة المحروم,MISR_305E292N_R,towns,Point,"(30.92349, 30.79572)"
 MAHALLANUQAYDA_307E307N_S,Maḥallaŧ Nuqaydaŧ,محلة نقيدة,محلة نقيدة,MISR_305E292N_R,villages,Point,"(30.70804, 30.78411)"
 MAHALLAQAYYASIN_668E374N_S,Maḥallaŧ al-Qayyāsīn,محلة القياسين,محلة القياسين,MAWARANNAHR_656E401N_R,waystations,Point,"(66.8817, 37.44577)"
 MAHALLASURAD_308E309N_S,Maḥallaŧ Ṣurad,محلة صرد,محلة صرد,MISR_305E292N_R,villages,Point,"(30.8512, 30.96963)"
 MAHAN_573E301N_S,Māhān,ماهان,ماهان,SW_IRAN_540E294N_R,towns,Point,"(57.31039, 30.11166)"
 MAHDIABADH_624E371N_S,Mahdīābāḏ,مهدياباذ,مهدياباذ,NE_IRAN_606E351N_R,waystations,Point,"(62.41583, 37.12201)"
 MAHDIYYA_110E354N_S,Mahdiyyaŧ,مهدية,مهدية,IFRIQIYYA_78E349N_R,towns,Point,"(11.05807, 35.49133)"
-MAHDIYYA_110E354N_S,Mahdiyyaŧ,مهدية,مهدية,IFRIQIYYA_78E349N_R,towns,Point,"(11.05807, 35.49133)"
 MAHJAM_430E152N_S,al-Mahǧam,المهجم,المهجم,SW_ARABIA_456E158N_R,towns,Point,"(43.07237, 15.22352)"
 MAHJARA_435E176N_S,al-Mahǧaraŧ,المهجرة,المهجرة,CENTRAL_ARABIA_416E227N_R,villages,Point,"(43.54039, 17.60657)"
 MAHLABIYYA_427E362N_S,al-Maḥlabiyyaŧ,المحلبية,المحلبية,JAZIRA_420E364N_R,villages,Point,"(42.7655, 36.25676)"
 MAHRA_502E151N_R,Mahraŧ,مهرة,مهرة,SW_ARABIA_456E158N_R,regions,Point,"(50.21937, 15.14685)"
 MAHRUBAN_502E300N_S,Mahrūbān,مهروبان,مهروبان,SW_IRAN_540E294N_R,towns,Point,"(50.21436, 30.06436)"
 MAHUZAZDUD_346E318N_S,Māḥūz Azdūd,ماحوز أزدود,ماحوز أزدود,SHAM_363E335N_R,towns,Point,"(34.63712, 31.81276)"
 MAHUZYUBNA_346E318N_S,Māḥūz Yubnā,ماحوز يبنا,ماحوز يبنا,SHAM_363E335N_R,towns,Point,"(34.66888, 31.87811)"
@@ -1272,30 +1206,26 @@
 MAKHNAQ_446E128N_S,al-Maḫnaq,المخنق,المخنق,SW_ARABIA_456E158N_R,villages,Point,"(44.60835, 12.8341)"
 MAKKA_398E213N_S,Makkaŧ,مكة,مكة,CENTRAL_ARABIA_416E227N_R,metropoles,Point,"(39.83612, 21.39132)"
 MAKNAABUMANSUR_091E368N_R,Maknaŧ Abū Manṣūr,مكنة أبو منصور,مكنة أبو منصور,IFRIQIYYA_78E349N_R,regions,Point,"(9.11248, 36.81309)"
 MALAL_394E242N_S,Malal,ملل,ملل,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.45628, 24.29047)"
 MALAQUN_039W391N_S,Malaqūn,ملقون,ملقون,ANDALUS_040E398N_R,towns,Point,"(-3.91362, 39.1739)"
 MALATHAYA_429E368N_S,Maʿlaṯāyaŧ,معلثاية,معلثاية,JAZIRA_420E364N_R,towns,Point,"(42.9635, 36.81597)"
 MALATIN_383E383N_S,Malaṭīn,ملطين,ملطين، ملطية,JAZIRA_420E364N_R,towns,Point,"(38.35767, 38.35806)"
-MALATIN_383E383N_S,Malaṭīn,ملطين,ملطين، ملطية,JAZIRA_420E364N_R,towns,Point,"(38.35767, 38.35806)"
 MALAYAKIRD_602E354N_S,Mālāyakird,مالايكرد,مالايكرد,NE_IRAN_606E351N_R,waystations,Point,"(60.29878, 35.4167)"
 MALAZKIRD_425E391N_S,Malāzkird,ملازكرد,ملازكرد، ملازجرد، منازجرد,QABQ_457E413N_R,towns,Point,"(42.55713, 39.1437)"
-MALAZKIRD_425E391N_S,Malāzkird,ملازكرد,ملازكرد، ملازجرد، منازجرد,QABQ_457E413N_R,towns,Point,"(42.55713, 39.1437)"
 MALIDAS_303E312N_R,al-Malīdās,المليداس,المليداس، المليدس,MISR_305E292N_R,regions,Point,"(30.37989, 31.24231)"
 MALIJ_310E305N_S,Malīǧ,مليج,مليج,MISR_305E292N_R,towns,Point,"(31.01342, 30.58083)"
 MALIN_602E349N_S,Mālin,مالن,مالن، كواخرز,NE_IRAN_606E351N_R,towns,Point,"(60.26487, 34.93776)"
 MALIN_621E341N_S,Mālin,مالن,مالن، السفلقات، ملين، مالان,NE_IRAN_606E351N_R,towns,Point,"(62.19614, 34.18473)"
 MALIN_650E368N_S,Mālin,مالن,مالن,NE_IRAN_606E351N_R,towns,Point,"(65.07649, 36.81403)"
-MALIQA_044W367N_R,Māliqaŧ,مالقة,مالقة,,regions,Point,"(-4.43066, 36.74791)"
 MALIQA_044W367N_S,Māliqaŧ,مالقة,مالقة,ANDALUS_040E398N_R,towns,Point,"(-4.43066, 36.74791)"
 MALLAHA_593E355N_S,al-Mallāḥaŧ,الملاحة,الملاحة,NE_IRAN_606E351N_R,waystations,Point,"(59.36352, 35.53664)"
 MAMATIR_527E365N_S,Māmaṭīr,مامطير,مامطير,NW_IRAN_515E356N_R,towns,Point,"(52.74659, 36.51713)"
 MANADHIR_485E313N_R,Manāḏir,مناذر,مناذر,SW_IRAN_540E294N_R,regions,Point,"(48.53345, 31.39058)"
 MANBIJ_379E365N_S,Manbiǧ,منبج,منبج,JAZIRA_420E364N_R,towns,Point,"(37.98957, 36.54651)"
-MANDAB_434E126N_R,al-Mandab,المندب,المندب,,regions,Point,"(43.4995, 12.6926)"
 MANDAB_434E126N_S,al-Mandab,المندب,المندب,SW_ARABIA_456E158N_R,towns,Point,"(43.4995, 12.6926)"
 MANDAM_488E310N_S,Mandam,مندم,مندم، بندم,SW_IRAN_540E294N_R,waystations,Point,"(48.881, 31.02269)"
 MANF_312E298N_S,Manf,منف,منف، العزيزية,MISR_305E292N_R,towns,Point,"(31.25648, 29.85447)"
 MANHAB_422E272N_R,al-Manhab,المنهب,المنهب,CENTRAL_ARABIA_416E227N_R,sites,Point,"(42.21215, 27.2743)"
 MANJABARA_682E258N_S,Manǧābārá,منجابارى,منجابارى,SE_IRAN_656E286N_R,towns,Point,"(68.25338, 25.84265)"
 MANSAF_320E301N_S,al-Manṣaf,المنصف,المنصف,MISR_305E292N_R,villages,Point,"(32.05366, 30.18702)"
 MANSURA_688E258N_S,al-Manṣūraŧ,المنصورة,المنصورة,SE_IRAN_656E286N_R,capitals,Point,"(68.87697, 25.8651)"
@@ -1310,15 +1240,14 @@
 MARABADH_630E343N_S,Mārābāḏ,ماراباذ,ماراباذ,NE_IRAN_606E351N_R,towns,Point,"(63.00426, 34.3371)"
 MARAGHA_462E373N_S,Marāġaŧ,مراغة,مراغة,QABQ_457E413N_R,towns,Point,"(46.24758, 37.34276)"
 MARAND_458E384N_S,Marand,مرند,مرند,QABQ_457E413N_R,towns,Point,"(45.80321, 38.46017)"
 MARAQIYYA_359E350N_S,Marāqiyyaŧ,مراقية,مراقية,SHAM_363E335N_R,villages,Point,"(35.91774, 35.04801)"
 MARASH_369E375N_S,Marʿaš,مرعش,مرعش,JAZIRA_420E364N_R,waystations,Point,"(36.92987, 37.58314)"
 MARDIN_407E373N_S,Mārdīn,ماردين,ماردين,JAZIRA_420E364N_R,towns,Point,"(40.71117, 37.30186)"
 MARGHINAN_717E405N_S,Marġīnan,مرغينن,مرغينن,MAWARANNAHR_656E401N_R,towns,Point,"(71.76105, 40.50359)"
-MARIB_454E155N_R,Maʾrib,مأرب,مأرب,,regions,Point,"(45.439, 15.55742)"
 MARIB_454E155N_S,Maʾrib,مأرب,مأرب,SW_ARABIA_456E158N_R,capitals,Point,"(45.439, 15.55742)"
 MARIDA_063W388N_S,Māridaŧ,ماردة,ماردة,ANDALUS_040E398N_R,towns,Point,"(-6.32886, 38.89521)"
 MARIS_309E203N_R,Marīs,مريس,مريس,MISR_305E292N_R,regions,Point,"(30.93987, 20.35618)"
 MARIYYA_025W368N_S,al-Mariyyaŧ,المرية,المرية,ANDALUS_040E398N_R,towns,Point,"(-2.50099, 36.86202)"
 MARJJUHAYNA_432E361N_S,Marǧ Ǧuhaynaŧ,مرج جهينة,مرج جهينة، مر جهينة,JAZIRA_420E364N_R,towns,Point,"(43.26652, 36.14235)"
 MARJRAHIT_365E336N_O,Marǧ Rāhiṭ,مرج راهط,مرج راهط,SHAM_363E335N_R,sites,Point,"(36.50981, 33.60226)"
 MARJSHAYKH_248E316N_S,Marǧ al-Šayḫ,مرج الشيخ,مرج الشيخ,BARQA_221E314N_R,waystations,Point,"(24.83486, 31.67644)"
@@ -1327,18 +1256,15 @@
 MARJ_462E343N_S,al-Marǧ,المرج,المرج، مرج القلعة,NW_IRAN_515E356N_R,waystations,Point,"(46.22379, 34.30577)"
 MARMAJANNA_084E354N_S,Marmāǧannaŧ,مرماجنة,مرماجنة، ماجنة,IFRIQIYYA_78E349N_R,villages,Point,"(8.40114, 35.48917)"
 MARMAL_443E155N_R,Marmal,مرمل,مرمل,SW_ARABIA_456E158N_R,regions,Point,"(44.36603, 15.56063)"
 MARSADAJJAJ_035E367N_S,Marsá al-Daǧǧāǧ,مرسى الدجاج,مرسى الدجاج,MAGHRIB_045E323N_R,towns,Point,"(3.58797, 36.73169)"
 MARSAKHARAZ_084E368N_S,Marsá al-Ḫaraz,مرسى الخرز,مرسى الخرز,IFRIQIYYA_78E349N_R,towns,Point,"(8.42231, 36.8546)"
 MARTUSH_039W377N_S,Mārtūš,مارتوش,مارتوش,ANDALUS_040E398N_R,towns,Point,"(-3.98826, 37.74285)"
 MARWA_385E257N_S,al-Marwaŧ,المروة,المروة، ذو المروة,CENTRAL_ARABIA_416E227N_R,towns,Point,"(38.58647, 25.71785)"
-MARWRUDH_633E355N_R,Marw al-Rūḏ,مرو الروذ,مرو الروذ,,regions,Point,"(63.3667, 35.5925)"
-MARWRUDH_633E355N_S,Marw al-Rūḏ,مرو الروذ,مرو الروذ,NE_IRAN_606E351N_R,capitals,Point,"(63.3667, 35.5925)"
 MARWRUDH_633E355N_S,Marw al-Rūḏ,مرو الروذ,مرو الروذ,NE_IRAN_606E351N_R,capitals,Point,"(63.3667, 35.5925)"
-MARW_621E376N_R,Marw,مرو,مرو، مرو الشاهجان,,regions,Point,"(62.10386, 37.67193)"
 MARW_621E376N_S,Marw,مرو,مرو، مرو الشاهجان,NE_IRAN_606E351N_R,capitals,Point,"(62.10386, 37.67193)"
 MARZAQAN_567E279N_S,Marzaqān,مرزقان,مرزقان,SW_IRAN_540E294N_R,villages,Point,"(56.75347, 27.96611)"
 MASABADHAN_469E335N_R,Māsabaḏān,ماسبذان,ماسبذان,NW_IRAN_515E356N_R,regions,Point,"(46.92023, 33.58473)"
 MASANI_439E155N_R,al-Maṣāniʿ,المصانع,المصانع,SW_ARABIA_456E158N_R,regions,Point,"(43.96174, 15.5805)"
 MASDAQAN_498E350N_S,Maṣdaqān,مصدقان,مصدقان,NW_IRAN_515E356N_R,waystations,Point,"(49.85406, 35.06107)"
 MASHA_694E395N_R,Masḥā,مسحا,مسحا,MAWARANNAHR_656E401N_R,regions,Point,"(69.45848, 39.51566)"
 MASHKA_639E274N_S,Mašká,مشكى,مشكى، مشكي,SE_IRAN_656E286N_R,towns,Point,"(63.94609, 27.46467)"
@@ -1395,15 +1321,14 @@
 MISKYANA_077E356N_S,al-Miskyānaŧ,المسكيانة,المسكيانة,IFRIQIYYA_78E349N_R,towns,Point,"(7.73214, 35.6162)"
 MISLAH_407E224N_S,al-Mislaḥ,المسلح,المسلح,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(40.79626, 22.44276)"
 MISSISA_356E369N_S,al-Miṣṣīṣaŧ,المصيصة,المصيصة,SHAM_363E335N_R,waystations,Point,"(35.66897, 36.94067)"
 MIYANKAL_642E393N_S,Miyān Kāl,ميان كال,ميان كال,MAWARANNAHR_656E401N_R,waystations,Point,"(64.26931, 39.34189)"
 MUBARAK_398E355N_S,al-Mubārak,المبارك,المبارك,JAZIRA_420E364N_R,villages,Point,"(39.8395, 35.58832)"
 MUDHAYKHIRA_439E137N_S,al-Muḏayḫiraŧ,المذيخرة,المذيخرة,SW_ARABIA_456E158N_R,towns,Point,"(43.97403, 13.78649)"
 MUGHAN_039W399N_S,Muġān,مغان,مغان,ANDALUS_040E398N_R,villages,Point,"(-3.9424, 39.97062)"
-MUGHAN_485E393N_R,Mūġān,موغان,موغان، موغكان، موقان,,regions,Point,"(48.50179, 39.33548)"
 MUGHAN_485E393N_S,Mūġān,موغان,موغان، موغكان، موقان,QABQ_457E413N_R,capitals,Point,"(48.50179, 39.33548)"
 MUGHITHAMAWAN_414E250N_S,Muġīṯaŧ al-Māwān,مغيثة الماوان,مغيثة الماوان، المغيثة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.4016, 25.00091)"
 MUGHITHA_440E311N_S,al-Muġīṯaŧ,المغيثة,المغيثة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(44.00938, 31.10097)"
 MUHALLABI_561E334N_S,al-Muhallabī,المهلبي,المهلبي,SE_IRAN_656E286N_R,waystations,Point,"(56.18509, 33.40323)"
 MUHDATHA_371E315N_S,al-Muḥdaṯaŧ,المحدثة,المحدثة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(37.15494, 31.51278)"
 MUHDATHA_374E277N_S,al-Muḥdaṯaŧ,المحدثة,المحدثة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(37.46327, 27.73026)"
 MUKHA_432E133N_S,Muḫā,مخا,مخا,SW_ARABIA_456E158N_R,towns,Point,"(43.26069, 13.32902)"
@@ -1514,33 +1439,29 @@
 NAJIRAM_511E284N_R,Naǧīram,نجيرم,نجيرم,SW_IRAN_540E294N_R,regions,Point,"(51.12283, 28.49687)"
 NAJRAN_442E175N_S,Naǧrān,نجران,نجران,CENTRAL_ARABIA_416E227N_R,towns,Point,"(44.2995, 17.58603)"
 NAMAHAND_519E357N_S,Nāmahand,نامهند,نامهند,NW_IRAN_515E356N_R,waystations,Point,"(51.9273, 35.72749)"
 NAMALATA_046W341N_S,Namālataŧ,نمالتة,نمالتة,MAGHRIB_045E323N_R,towns,Point,"(-4.6284, 34.13739)"
 NAMIYA_543E367N_S,Nāmiyaŧ,نامية,نامية,NW_IRAN_515E356N_R,towns,Point,"(54.32519, 36.77488)"
 NARMASIR_586E289N_S,Narmāsīr,نرماسير,نرماسير,SW_IRAN_540E294N_R,capitals,Point,"(58.64795, 28.98436)"
 NASAFAN_448E140N_R,Nasafān,نسفان,نسفان,SW_ARABIA_456E158N_R,regions,Point,"(44.8432, 14.02916)"
-NASAF_658E388N_R,Nasaf,نسف,نسف,,regions,Point,"(65.8104, 38.86245)"
 NASAF_658E388N_S,Nasaf,نسف,نسف,MAWARANNAHR_656E401N_R,capitals,Point,"(65.8104, 38.86245)"
 NASA_582E378N_S,Nasāʾ,نساء,نساء,NE_IRAN_606E351N_R,towns,Point,"(58.21787, 37.85763)"
-NASA_582E378N_S,Nasāʾ,نساء,نساء,NE_IRAN_606E351N_R,towns,Point,"(58.21787, 37.85763)"
 NASA_711E404N_R,Nasāʾ,نساء,نساء، نسيا,,regions,Point,"(71.10821, 40.41184)"
 NASHAWA_453E393N_S,al-Našawá,النشوى,النشوى,QABQ_457E413N_R,towns,Point,"(45.3766, 39.34739)"
 NASHK_580E297N_S,Našk,نشك,نشك,SW_IRAN_540E294N_R,towns,Point,"(58.03255, 29.70224)"
 NASIBIN_412E370N_S,Naṣībīn,نصيبين,نصيبين,JAZIRA_420E364N_R,towns,Point,"(41.22167, 37.05514)"
 NASTARAWA_307E314N_S,Nastarāwaŧ,نستراوة,نستراوة، نستراو,MISR_305E292N_R,towns,Point,"(30.70804, 31.48776)"
 NATIL_519E364N_S,Nātil,ناتل,ناتل,NW_IRAN_515E356N_R,towns,Point,"(51.91951, 36.47768)"
 NATWAYA_313E306N_R,Naṭwayaŧ,نطوية,نطوية، نطو الرمان,MISR_305E292N_R,regions,Point,"(31.37316, 30.69837)"
 NAWASA_312E309N_R,Nawasā,نوسا,نوسا,MISR_305E292N_R,regions,Point,"(31.28494, 30.97866)"
 NAWA_360E328N_S,Nawá,نوى,نوى,SHAM_363E335N_R,towns,Point,"(36.02865, 32.88099)"
 NAWIKATH_758E430N_S,Nawīkaṯ,نويكث,نويكث,MAWARANNAHR_656E401N_R,towns,Point,"(75.87766, 43.067)"
 NAWKAD_662E388N_S,Nawkād,نوكاد,نوكاد، نوقاد قريش,MAWARANNAHR_656E401N_R,towns,Point,"(66.29094, 38.84309)"
 NAWUSA_426E338N_S,al-Nāwusaŧ,الناوسة,الناوسة,IRAQ_459E319N_R,waystations,Point,"(42.61179, 33.82317)"
-NAYRIZ_542E292N_R,Nayrīz,نيريز,نيريز,,regions,Point,"(54.27518, 29.21368)"
 NAYRIZ_542E292N_S,Nayrīz,نيريز,نيريز,SW_IRAN_540E294N_R,capitals,Point,"(54.27518, 29.21368)"
-NAYSABUR_587E361N_R,Naysābūr,نيسابور,نيسابور,,regions,Point,"(58.79841, 36.12138)"
 NAYSABUR_587E361N_S,Naysābūr,نيسابور,نيسابور,NE_IRAN_606E351N_R,metropoles,Point,"(58.79841, 36.12138)"
 NAZWA_575E228N_S,Nazwaŧ,نزوة,نزوة,SE_ARABIA_556E220N_R,towns,Point,"(57.52541, 22.86309)"
 NIBAJ_444E263N_S,al-Nibāǧ,النباج,النباج,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(44.45181, 26.35812)"
 NIHAWAND_483E342N_S,Nihāwand,نهاوند,نهاوند، ماه البصرة,NW_IRAN_515E356N_R,capitals,Point,"(48.39263, 34.21512)"
 NIHIYYA_415E343N_S,al-Nihiyyaŧ,النهية,النهية,JAZIRA_420E364N_R,towns,Point,"(41.5567, 34.39307)"
 NIHYA_373E344N_S,Nihyā,نهيا,نهيا,SHAM_363E335N_R,waystations,Point,"(37.38213, 34.45245)"
 NIH_600E315N_S,Nih,نه,نه، نيه,SE_IRAN_656E286N_R,towns,Point,"(60.05406, 31.5777)"
@@ -1595,36 +1516,32 @@
 QALUNIYAAWFI_384E403N_S,Qalūniyaŧ al-ʿAwfī,قلونية العوفي,قلونية العوفي,RUM_335E392N_R,waystations,Point,"(38.49484, 40.32189)"
 QAMARTI_404E348N_S,al-Qamarṭī,القمرطي,القمرطي، القمرطي,JAZIRA_420E364N_R,waystations,Point,"(40.45161, 34.81073)"
 QAMUDA_091E351N_R,Qamūdaŧ,قمودة,قمودة,IFRIQIYYA_78E349N_R,regions,Point,"(9.13153, 35.15407)"
 QAMUHUL_717E236N_S,Qāmuhul,قامهل,قامهل,SE_IRAN_656E286N_R,towns,Point,"(71.72209, 23.61826)"
 QANAWNA_411E191N_S,Qanawnaŧ,قنونة,قنونة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.15761, 19.12337)"
 QANBALI_665E254N_S,Qanbalī,قنبلي,قنبلي، قنبلى,SE_IRAN_656E286N_R,towns,Point,"(66.57989, 25.49111)"
 QANDABIL_674E286N_S,Qandābīl,قندابيل,قندابيل,SE_IRAN_656E286N_R,towns,Point,"(67.48191, 28.62665)"
-QANDAHAR_656E316N_R,Qandahār,قندهار,قندهار,,regions,Point,"(65.69197, 31.64414)"
 QANDAHAR_656E316N_S,Qandahār,قندهار,قندهار,SE_IRAN_656E286N_R,towns,Point,"(65.69197, 31.64414)"
-QANNAWJ_800E271N_R,Qannawǧ,قنوج,قنوج,,regions,Point,"(80.03921, 27.11654)"
 QANNAWJ_800E271N_S,Qannawǧ,قنوج,قنوج,SE_IRAN_656E286N_R,capitals,Point,"(80.03921, 27.11654)"
 QANTARANUMAN_476E344N_S,Qanṭaraŧ al-Nuʿmān,قنطرة النعمان,قنطرة النعمان,NW_IRAN_515E356N_R,waystations,Point,"(47.65232, 34.46868)"
 QANTARASIF_068W396N_S,Qanṭaraŧ al-Sīf,قنطرة السيف,قنطرة السيف,ANDALUS_040E398N_R,towns,Point,"(-6.8414, 39.69061)"
 QANTARA_323E308N_S,al-Qanṭaraŧ,القنطرة,القنطرة,MISR_305E292N_R,villages,Point,"(32.32461, 30.85902)"
 QANT_004W383N_S,Qānt,قانت,قانت,ANDALUS_040E398N_R,towns,Point,"(-0.47061, 38.34618)"
 QANUWAN_506E332N_S,Qanūwān,قنووان,قنووان,NW_IRAN_515E356N_R,waystations,Point,"(50.65469, 33.23683)"
 QARAJUN_644E395N_S,Qārāǧūn,قاراجون,قاراجون,MAWARANNAHR_656E401N_R,villages,Point,"(64.42927, 39.56944)"
 QARA_368E341N_S,Qāraŧ,قارة,قارة,SHAM_363E335N_R,waystations,Point,"(36.84868, 34.16598)"
 QARA_438E308N_S,Qarʿāʾ,قرعاء,قرعاء,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.81303, 30.87576)"
 QARA_468E274N_S,al-Qarʿaŧ,القرعة,القرعة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(46.88787, 27.45084)"
 QARINASH_131E381N_S,Qarīnaš,قرينش,قرينش,SIQILIYYA_145E375N_R,towns,Point,"(13.18997, 38.15105)"
 QARINAYN_624E365N_S,al-Qarīnayn,القرينين,القرينين,NE_IRAN_606E351N_R,villages,Point,"(62.44974, 36.5754)"
 QARMASIN_470E343N_S,Qarmāsīn,قرماسين,قرماسين، قرميسين,NW_IRAN_515E356N_R,towns,Point,"(47.09845, 34.32388)"
-QARMASIN_470E343N_S,Qarmāsīn,قرماسين,قرماسين، قرميسين,NW_IRAN_515E356N_R,towns,Point,"(47.09845, 34.32388)"
 QARMUNA_056W374N_S,Qarmūnaŧ,قرمونة,قرمونة,ANDALUS_040E398N_R,towns,Point,"(-5.64097, 37.42933)"
 QARNIN_622E315N_S,Qarnīn,قرنين,قرنين,SE_IRAN_656E286N_R,towns,Point,"(62.23227, 31.51377)"
 QARN_402E214N_S,Qarn,قرن,قرن، قرن المنازل,CENTRAL_ARABIA_416E227N_R,towns,Point,"(40.21296, 21.46576)"
 QARQISIYYA_404E351N_S,Qarqīsiyyaŧ,قرقيسية,قرقيسية,JAZIRA_420E364N_R,towns,Point,"(40.43747, 35.1462)"
-QARQISIYYA_404E351N_S,Qarqīsiyyaŧ,قرقيسية,قرقيسية,JAZIRA_420E364N_R,towns,Point,"(40.43747, 35.1462)"
 QARTAJANNA_009W376N_S,Qarṭāǧannaŧ,قرطاجنة,قرطاجنة,ANDALUS_040E398N_R,villages,Point,"(-0.98315, 37.6005)"
 QARTAJANNA_102E368N_S,Qarṭāǧannaŧ,قرطاجنة,قرطاجنة,IFRIQIYYA_78E349N_R,towns,Point,"(10.26628, 36.87916)"
 QARTASA_304E310N_S,Qarṭasā,قرطسا,قرطسا,MISR_305E292N_R,villages,Point,"(30.44108, 31.05659)"
 QARUN_357E335N_S,al-Qarʿūn,القرعون,القرعون,SHAM_363E335N_R,waystations,Point,"(35.71229, 33.57083)"
 QARYAASAD_538E315N_S,Qaryaŧ al-Asad,قرية الأسد,قرية الأسد,SW_IRAN_540E294N_R,waystations,Point,"(53.84828, 31.55774)"
 QARYAAS_539E296N_S,Qaryaŧ al-Ās,قرية الآس,قرية الآس,SW_IRAN_540E294N_R,waystations,Point,"(53.92036, 29.69008)"
 QARYABARATIKIN_599E431N_S,Qaryaŧ Barātikīn,قرية براتكين,قرية براتكين، قرية فراتكين، قرية قراتجين,MAWARANNAHR_656E401N_R,towns,Point,"(59.95269, 43.19354)"
@@ -1639,15 +1556,14 @@
 QARYASALM_592E312N_S,Qaryaŧ Salm,قرية سلم,قرية سلم,SE_IRAN_656E286N_R,waystations,Point,"(59.28094, 31.25781)"
 QARYATAN_372E342N_S,al-Qaryatān,القريتان,القريتان,SHAM_363E335N_R,waystations,Point,"(37.24976, 34.2251)"
 QARYATAYN_164E311N_O,al-Qaryatayn,القريتين,القريتين,BARQA_221E314N_R,sites,Point,"(16.44486, 31.18315)"
 QARYATAYN_439E260N_S,al-Qaryatayn,القريتين,القريتين,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.92995, 26.08634)"
 QARYAUYUN_355E333N_S,Qaryaŧ al-ʿUyūn,قرية العيون,قرية العيون,SHAM_363E335N_R,waystations,Point,"(35.56778, 33.36423)"
 QASABA_397E350N_S,al-Qaṣabaŧ,القصبة,القصبة,JAZIRA_420E364N_R,waystations,Point,"(39.76511, 35.05726)"
 QASARASH_063W394N_S,Qaṣarāš,قصراش,قصراش,ANDALUS_040E398N_R,towns,Point,"(-6.3954, 39.46953)"
-QASHAN_515E339N_R,Qāšān,قاشان,قاشان,,regions,Point,"(51.50468, 33.96762)"
 QASHAN_515E339N_S,Qāšān,قاشان,قاشان,NW_IRAN_515E356N_R,capitals,Point,"(51.50468, 33.96762)"
 QASRAHNAF_632E357N_S,Qaṣr Aḥnaf,قصر أحنف,قصر أحنف,NE_IRAN_606E351N_R,towns,Point,"(63.21212, 35.76147)"
 QASRAIN_524E308N_S,Qaṣr Aʿīn,قصر أعين,قصر أعين، قصر آيين، الرون,SW_IRAN_540E294N_R,towns,Point,"(52.44521, 30.82066)"
 QASRATISH_181E305N_S,Qaṣr al-ʿAṭiš,قصر العطش,قصر العطش,BARQA_221E314N_R,waystations,Point,"(18.19751, 30.54115)"
 QASRBANUWARDAS_084W383N_S,Qaṣr Banū Wardās,قصر بنو ورداس,قصر بنو ورداس,ANDALUS_040E398N_R,towns,Point,"(-8.48333, 38.36698)"
 QASRIBADI_172E309N_S,Qaṣr al-ʿIbādī,قصر العبادي,قصر العبادي، قبر العبادي,BARQA_221E314N_R,waystations,Point,"(17.29329, 30.94914)"
 QASRIBNHUBAYRA_443E327N_S,Qaṣr Ibn Hubayraŧ,قصر إبن هبيرة,قصر إبن هبيرة,IRAQ_459E319N_R,towns,Point,"(44.34902, 32.70401)"
@@ -1677,28 +1593,26 @@
 QAZWIN_500E362N_S,Qazwīn,قزوين,قزوين,NW_IRAN_515E356N_R,towns,Point,"(50.0011, 36.27854)"
 QA_436E297N_S,al-Qāʾ,القاء,القاء,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.61126, 29.78571)"
 QA_653E363N_S,al-Qāʾ,القاء,القاء,NE_IRAN_606E351N_R,waystations,Point,"(65.32516, 36.3564)"
 QIFT_328E259N_R,Qifṭ,قفط,قفط، قفط,,regions,Point,"(32.80433, 25.99671)"
 QINA_327E261N_R,Qinā,قنا,قنا,,regions,Point,"(32.73283, 26.17068)"
 QINNASRIN_370E359N_S,Qinnasrīn,قنسرين,قنسرين,SHAM_363E335N_R,capitals,Point,"(37.02701, 35.99617)"
 QIR_530E284N_S,Qīr,قير,قير، كير,SW_IRAN_540E294N_R,towns,Point,"(53.03724, 28.44621)"
-QUBADHIYAN_681E372N_R,Qubāḏiyān,قباذيان,قباذيان، قواذيان,,regions,Point,"(68.12506, 37.2898)"
 QUBADHIYAN_681E372N_S,Qubāḏiyān,قباذيان,قباذيان، قواذيان,MAWARANNAHR_656E401N_R,capitals,Point,"(68.12506, 37.2898)"
 QUBA_395E244N_S,Qubā,قبا,قبا,CENTRAL_ARABIA_416E227N_R,villages,Point,"(39.58264, 24.44572)"
 QUBA_416E227N_S,Qubāʾ,قباء,قباء,CENTRAL_ARABIA_416E227N_R,villages,Point,"(41.65725, 22.78726)"
 QUBA_721E405N_S,Qubā,قبا,قبا,MAWARANNAHR_656E401N_R,towns,Point,"(72.18143, 40.5566)"
 QUDAM_436E158N_R,Qudam,قدم,قدم، قدم,SW_ARABIA_456E158N_R,regions,Point,"(43.68913, 15.81462)"
 QUFAA_435E137N_R,Qufāʿaŧ,قفاعة,قفاعة,SW_ARABIA_456E158N_R,regions,Point,"(43.58641, 13.78649)"
 QUHISTAN_594E337N_R,Qūhistān,قوهستان,قوهستان,NE_IRAN_606E351N_R,regions,Point,"(59.44592, 33.77051)"
 QULAYBUMMAL_308E308N_S,Qulayb al-`Ummāl,قليب العمال,قليب العمال,MISR_305E292N_R,villages,Point,"(30.82245, 30.86818)"
 QULUFI_395E321N_S,al-Qulūfī,القلوفي,القلوفي، العلوي,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.59203, 32.14778)"
 QULZUM_325E300N_S,al-Qulzum,القلزم,القلزم,MISR_305E292N_R,towns,Point,"(32.55684, 30.02822)"
 QUMISA_518E320N_S,Qūmisaŧ,قومسة,قومسة,SW_IRAN_540E294N_R,waystations,Point,"(51.86732, 32.00251)"
 QUMIS_541E361N_R,Qūmis,قومس,قومس,NW_IRAN_515E356N_R,regions,Point,"(54.13205, 36.11206)"
-QUMM_509E346N_R,Qumm,قم,قم,,regions,Point,"(50.90695, 34.63354)"
 QUMM_509E346N_S,Qumm,قم,قم,NW_IRAN_515E356N_R,capitals,Point,"(50.90695, 34.63354)"
 QURAKIR_377E313N_S,Qurākir,قراكر,قراكر، قراقر,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(37.75187, 31.32585)"
 QURAYN_395E214N_S,Qurayn,قرين,قرين,CENTRAL_ARABIA_416E227N_R,villages,Point,"(39.57789, 21.41489)"
 QURAY_417E315N_S,al-Qurāy,القراي,القراي,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.7933, 31.51068)"
 QURA_495E269N_S,al-Qurá,القرى,القرى,SE_ARABIA_556E220N_R,waystations,Point,"(49.50023, 26.90449)"
 QURBAYT_316E307N_R,Qurbayt,قربيت,قربيت,MISR_305E292N_R,regions,Point,"(31.62447, 30.73556)"
 QURH_379E265N_S,Qurḥ,قرح,قرح,CENTRAL_ARABIA_416E227N_R,capitals,Point,"(37.99288, 26.55412)"
@@ -1733,16 +1647,14 @@
 RAKAN_527E297N_S,Rakān,ركان,ركان,SW_IRAN_540E294N_R,villages,Point,"(52.74824, 29.7751)"
 RAKB_438E133N_R,Rakb,ركب,ركب,SW_ARABIA_456E158N_R,regions,Point,"(43.83575, 13.3854)"
 RAKUNIN_527E326N_S,Rakūnīn,ركونين,ركونين,SE_IRAN_656E286N_R,waystations,Point,"(52.72262, 32.66383)"
 RAMADA_276E310N_S,Ramādaŧ,رمادة,رمادة,BARQA_221E314N_R,towns,Point,"(27.61485, 31.02336)"
 RAMAN_486E342N_S,Rāman,رامن,رامن,NW_IRAN_515E356N_R,towns,Point,"(48.65585, 34.25819)"
 RAMASHAHRISTAN_612E303N_S,Rāmašahristān,رامشهرستان,رامشهرستان,SE_IRAN_656E286N_R,towns,Point,"(61.2099, 30.32501)"
 RAMA_434E257N_S,Rāmaŧ,رامة,رامة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.4292, 25.77608)"
-RAMHURMUZ_496E312N_R,Rām Hurmuz,رام هرمز,رام هرمز، رامهرمز,,regions,Point,"(49.60131, 31.28576)"
-RAMHURMUZ_496E312N_S,Rām Hurmuz,رام هرمز,رام هرمز، رامهرمز,SW_IRAN_540E294N_R,capitals,Point,"(49.60131, 31.28576)"
 RAMHURMUZ_496E312N_S,Rām Hurmuz,رام هرمز,رام هرمز، رامهرمز,SW_IRAN_540E294N_R,capitals,Point,"(49.60131, 31.28576)"
 RAMLA_348E319N_S,al-Ramlaŧ,الرملة,الرملة,SHAM_363E335N_R,capitals,Point,"(34.86436, 31.92484)"
 RAML_631E401N_S,al-Raml,الرمل,الرمل,MAWARANNAHR_656E401N_R,waystations,Point,"(63.16025, 40.13581)"
 RAMTA_154E381N_S,Ramṭaŧ,رمطة,رمطة، رمطة,SIQILIYYA_145E375N_R,towns,Point,"(15.44048, 38.18022)"
 RANYA_421E203N_S,Ranyaŧ,رنية,رنية,CENTRAL_ARABIA_416E227N_R,villages,Point,"(42.1041, 20.30924)"
 RAQIM_359E318N_S,al-Raqīm,الرقيم,الرقيم، الرقم,SHAM_363E335N_R,villages,Point,"(35.96419, 31.89279)"
 RAQQA_390E359N_S,al-Raqqaŧ,الرقة,الرقة,JAZIRA_420E364N_R,capitals,Point,"(39.05128, 35.9493)"
@@ -1756,15 +1668,14 @@
 RASK_612E267N_S,Rāsk,راسك,راسك,SE_IRAN_656E286N_R,towns,Point,"(61.22272, 26.70943)"
 RASMA_588E324N_S,Raʾs al-Māʾ,رأس الماء,رأس الماء,SE_IRAN_656E286N_R,waystations,Point,"(58.87027, 32.4344)"
 RASSIKR_528E297N_S,Raʾs al-Sikr,رأس السكر,رأس السكر,SW_IRAN_540E294N_R,waystations,Point,"(52.87257, 29.7751)"
 RASTAN_367E349N_S,Rastān,رستان,رستان,SHAM_363E335N_R,towns,Point,"(36.75337, 34.9335)"
 RAWARA_386E320N_S,al-Rawārá,الروارى,الروارى، الدوارى,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(38.64087, 32.03911)"
 RAWHA_392E241N_S,Rawḥāʾ,روحاء,روحاء,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.2976, 24.11893)"
 RAYDA_440E158N_S,al-Raydaŧ,الريدة,الريدة,SW_ARABIA_456E158N_R,villages,Point,"(44.0447, 15.83194)"
-RAYDA_440E158N_S,al-Raydaŧ,الريدة,الريدة,SW_ARABIA_456E158N_R,villages,Point,"(44.0447, 15.83194)"
 RAYKAN_526E285N_S,Rāykān,رايكان,رايكان، خان أزادمرد,SW_IRAN_540E294N_R,waystations,Point,"(52.67152, 28.52097)"
 RAYYA_044W369N_R,Rayyaŧ,رية,رية، ريه,ANDALUS_040E398N_R,regions,Point,"(-4.40368, 36.98351)"
 RAYY_515E356N_S,al-Rayy,الري,الري,NW_IRAN_515E356N_R,capitals,Point,"(51.50831, 35.62754)"
 RIBATABDALLAH_639E313N_S,Ribāṭ ʿAbd Allãh,رباط عبد الله,رباط عبد الله,SE_IRAN_656E286N_R,waystations,Point,"(63.92927, 31.3733)"
 RIBATABSHUTURAN_559E332N_S,Ribāṭ Āb Šuturān,رباط آب شتران,رباط آب شتران، خان أشتران,SE_IRAN_656E286N_R,waystations,Point,"(55.93385, 33.24359)"
 RIBATABUSAHL_574E401N_S,Ribāṭ Abū Sahl,رباط أبو سهل,رباط أبو سهل,NW_IRAN_515E356N_R,waystations,Point,"(57.45149, 40.18649)"
 RIBATAFRAWA_562E389N_S,Ribāṭ Afrāwaŧ,رباط أفراوة,رباط أفراوة,NE_IRAN_606E351N_R,waystations,Point,"(56.26856, 38.92182)"
@@ -1809,15 +1720,14 @@
 RIMA_432E143N_R,Rimāʿ,رماع,رماع,SW_ARABIA_456E158N_R,regions,Point,"(43.25806, 14.35515)"
 RIQAN_587E286N_S,Rīqān,ريقان,ريقان، ريكان,SW_IRAN_540E294N_R,towns,Point,"(58.73846, 28.65133)"
 RISHAHR_502E303N_S,Rīšahr,ريشهر,ريشهر,SW_IRAN_540E294N_R,villages,Point,"(50.22217, 30.34108)"
 RISHTAN_715E400N_S,Rištān,رشتان,رشتان,MAWARANNAHR_656E401N_R,towns,Point,"(71.55377, 40.02761)"
 RIWAND_583E361N_S,Rīwand,ريوند,ريوند,NE_IRAN_606E351N_R,towns,Point,"(58.36115, 36.18583)"
 RUAYN_445E144N_R,Ruʿayn,رعين,رعين,SW_ARABIA_456E158N_R,regions,Point,"(44.59298, 14.42424)"
 RUBANJ_544E285N_R,Rūbanǧ,روبنج,روبنج,SW_IRAN_540E294N_R,regions,Point,"(54.40794, 28.5161)"
-RUDHAN_560E303N_R,al-Rūḏān,الروذان,الروذان,,regions,Point,"(56.02186, 30.39947)"
 RUDHAN_560E303N_S,al-Rūḏān,الروذان,الروذان,SW_IRAN_540E294N_R,towns,Point,"(56.02186, 30.39947)"
 RUDHA_497E351N_S,Rūḏaŧ,روذة,روذة,NW_IRAN_515E356N_R,villages,Point,"(49.791, 35.10371)"
 RUDHBAR_577E278N_R,Ruḏbār,رذبار,رذبار، رذبال,SW_IRAN_540E294N_R,regions,Point,"(57.73088, 27.82747)"
 RUDHRAWAR_483E346N_S,Ruḏrāwar,رذراور,رذراور,NW_IRAN_515E356N_R,towns,Point,"(48.39263, 34.62225)"
 RUHABA_442E154N_R,Ruḥābaŧ,رحابة,رحابة,SW_ARABIA_456E158N_R,regions,Point,"(44.25892, 15.45562)"
 RUHAYMA_439E318N_S,al-Ruhaymaŧ,الرهيمة,الرهيمة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.95117, 31.85995)"
 RUHA_388E371N_S,al-Ruhā,الرها,الرها,JAZIRA_420E364N_R,towns,Point,"(38.82122, 37.1497)"
@@ -1829,15 +1739,14 @@
 RUSAFA_463E317N_S,al-Ruṣāfaŧ,الرصافة,الرصافة,IRAQ_459E319N_R,waystations,Point,"(46.3645, 31.78987)"
 RUSTAJIRD_502E317N_S,Rustaǧird,رستجرد,رستجرد، الدز,SW_IRAN_540E294N_R,waystations,Point,"(50.29984, 31.71801)"
 RUSTAKUHAN_664E265N_S,Rustākuhan,رستاكهن,رستاكهن,SE_IRAN_656E286N_R,towns,Point,"(66.40105, 26.57497)"
 RUSTAQBIK_699E371N_S,Rustāq Bīk,رستاق بيك,رستاق بيك,MAWARANNAHR_656E401N_R,towns,Point,"(69.91617, 37.11046)"
 RUSTAQ_551E284N_S,Rustāq,رستاق,رستاق,SW_IRAN_540E294N_R,towns,Point,"(55.10037, 28.4795)"
 RUWAYDASHT_527E324N_S,Ruwaydašt,رويدشت,رويدشت,NW_IRAN_515E356N_R,towns,Point,"(52.7166, 32.43743)"
 RUWAYTHA_392E240N_S,Ruwayṯaŧ,رويثة,رويثة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.23589, 24.01966)"
-RUYAN_517E363N_R,al-Rūyān,الرويان,الرويان,,regions,Point,"(51.7108, 36.36237)"
 RUYAN_517E363N_S,al-Rūyān,الرويان,الرويان,NW_IRAN_515E356N_R,towns,Point,"(51.7108, 36.36237)"
 RUZKAN_519E318N_S,Rūzkān,روزكان,روزكان,SW_IRAN_540E294N_R,waystations,Point,"(51.96103, 31.80584)"
 SABASTIYA_351E322N_S,Sabasṭiyaŧ,سبسطية,سبسطية,SHAM_363E335N_R,villages,Point,"(35.15237, 32.27085)"
 SABAT_687E399N_S,Ṣābāṭ,صاباط,صاباط,MAWARANNAHR_656E401N_R,towns,Point,"(68.7622, 39.99901)"
 SABA_453E154N_R,Sabāʾ,سباء,سباء,SW_ARABIA_456E158N_R,regions,Point,"(45.33616, 15.40854)"
 SABIBA_091E354N_S,Sabībaŧ,سبيبة,سبيبة,IFRIQIYYA_78E349N_R,towns,Point,"(9.16117, 35.41674)"
 SABKHAMANHUSHA_186E297N_R,Sabḫaŧ Manhūšā,سبخة منهوشا,سبخة منهوشا,BARQA_221E314N_R,regions,Point,"(18.63423, 29.78891)"
@@ -1852,15 +1761,14 @@
 SADAD_369E343N_S,Ṣadad,صدد,صدد,SHAM_363E335N_R,waystations,Point,"(36.9334, 34.31043)"
 SADA_437E169N_S,Ṣaʿdaŧ,صعدة,صعدة,SW_ARABIA_456E158N_R,towns,Point,"(43.76442, 16.9453)"
 SADUSAN_678E264N_S,Sadūsān,سدوسان,سدوسان، سدوستان,SE_IRAN_656E286N_R,towns,Point,"(67.85929, 26.41721)"
 SAFIYYA_306E310N_S,al-Ṣāfiyyaŧ,الصافية,الصافية,MISR_305E292N_R,villages,Point,"(30.6995, 31.04306)"
 SAFRA_389E240N_S,al-Ṣafrāʾ,الصفراء,الصفراء,CENTRAL_ARABIA_416E227N_R,villages,Point,"(38.95085, 24.03308)"
 SAFR_416E208N_S,Ṣafr,صفر,صفر,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.68929, 20.85351)"
 SAGHAND_552E325N_S,Sāġand,ساغند,ساغند,SE_IRAN_656E286N_R,waystations,Point,"(55.21675, 32.52933)"
-SAGHANIYAN_678E382N_R,al-Ṣaġāniyān,الصغانيان,الصغانيان,,regions,Point,"(67.89454, 38.26337)"
 SAGHANIYAN_678E382N_S,al-Ṣaġāniyān,الصغانيان,الصغانيان,MAWARANNAHR_656E401N_R,capitals,Point,"(67.89454, 38.26337)"
 SAGHAN_680E330N_S,Saġān,سغان,سغان,SE_IRAN_656E286N_R,villages,Point,"(68.03075, 33.0881)"
 SAGHB_364E271N_S,Saġb,سغب,سغب,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(36.47366, 27.19891)"
 SAHIH_543E297N_S,Ṣahīh,صهيه,صهيه، صاهك,SW_IRAN_540E294N_R,towns,Point,"(54.30902, 29.77106)"
 SAHIH_601E361N_S,Ṣāhih,صاهه,صاهه,NE_IRAN_606E351N_R,villages,Point,"(60.18929, 36.10597)"
 SAHIK_504E299N_S,Ṣāḥik,صاحك,صاحك,SW_IRAN_540E294N_R,waystations,Point,"(50.4613, 29.96408)"
 SAHIK_508E307N_S,Ṣāhik,صاهك,صاهك,SW_IRAN_540E294N_R,villages,Point,"(50.80266, 30.74015)"
@@ -1902,15 +1810,14 @@
 SANKAN_594E350N_S,Sankān,سنكان,سنكان، سنجان,NE_IRAN_606E351N_R,towns,Point,"(59.41155, 35.05003)"
 SANKARDAH_675E385N_S,Sankardah,سنكرده,سنكرده,MAWARANNAHR_656E401N_R,towns,Point,"(67.57933, 38.50044)"
 SANTA_334E194N_S,al-Sanṭaŧ,السنطة,السنطة,MISR_305E292N_R,villages,Point,"(33.43051, 19.40078)"
 SAN_318E309N_R,Ṣān,صان,صان,MISR_305E292N_R,regions,Point,"(31.87265, 30.9789)"
 SARAFANDA_352E334N_S,Ṣarafandaŧ,صرفندة,صرفندة,SHAM_363E335N_R,towns,Point,"(35.28606, 33.45495)"
 SARAKHS_611E365N_S,Saraḫs,سرخس,سرخس,NE_IRAN_606E351N_R,towns,Point,"(61.18671, 36.51694)"
 SARANDIB_808E076N_R,Sarandīb,سرنديب,سرنديب,SE_IRAN_656E286N_R,regions,Point,"(80.81976, 7.60759)"
-SARAQUSA_009W416N_R,Saraqūsaŧ,سرقوسة,سرقوسة، سرقوسطة,,regions,Point,"(-0.9292, 41.63368)"
 SARAQUSA_009W416N_S,Saraqūsaŧ,سرقوسة,سرقوسة، سرقوسطة,ANDALUS_040E398N_R,towns,Point,"(-0.9292, 41.63368)"
 SARAQUSA_152E370N_S,Saraqūsaŧ,سرقوسة,سرقوسة,SIQILIYYA_145E375N_R,towns,Point,"(15.29356, 37.0911)"
 SARAT_475E379N_S,al-Sarāt,السرات,السرات,QABQ_457E413N_R,villages,Point,"(47.57698, 37.91236)"
 SARAYSHAHR_597E281N_S,Sarāy Šahr,سراي شهر,سراي شهر,SE_IRAN_656E286N_R,towns,Point,"(59.73164, 28.17735)"
 SARDAN_504E309N_R,Sardān,سردان,سردان,SW_IRAN_540E294N_R,regions,Point,"(50.42781, 30.9971)"
 SARDUS_311E301N_S,Sardūs,سردوس,سردوس,MISR_305E292N_R,towns,Point,"(31.18645, 30.16277)"
 SARIGH_752E428N_S,Sāriġ,سارغ,سارغ,MAWARANNAHR_656E401N_R,waystations,Point,"(75.26356, 42.80107)"
@@ -1942,22 +1849,20 @@
 SA_307E309N_S,Ṣāʾ,صاء,صاء,MISR_305E292N_R,villages,Point,"(30.73849, 30.95914)"
 SHABABAK_550E301N_S,Šābābak,شابابك,شابابك، شاباوك، شهرباباك,SW_IRAN_540E294N_R,towns,Point,"(55.05872, 30.13418)"
 SHABARAN_487E412N_S,Šābarān,شابران,شابران,QABQ_457E413N_R,towns,Point,"(48.76916, 41.2707)"
 SHABAS_307E310N_R,Šabās,شباس,شباس,MISR_305E292N_R,regions,Point,"(30.72312, 31.08986)"
 SHABRUWA_312E301N_S,Šabruwā,شبروا,شبروا، شبرو,MISR_305E292N_R,towns,Point,"(31.24225, 30.11048)"
 SHABURQAN_657E366N_S,Šabūrqān,شبورقان,شبورقان، أشبورقان,NE_IRAN_606E351N_R,towns,Point,"(65.78352, 36.65136)"
 SHABUR_307E308N_S,Šābūr,شابور,شابور,MISR_305E292N_R,villages,Point,"(30.73365, 30.80318)"
-SHADHUNA_059W364N_R,Šaḏūnaŧ,شذونة,شذونة، شدونة,,regions,Point,"(-5.91433, 36.4664)"
 SHADHUNA_059W364N_S,Šaḏūnaŧ,شذونة,شذونة، شدونة,ANDALUS_040E398N_R,towns,Point,"(-5.91433, 36.4664)"
 SHAHHAJIYYA_429E362N_S,al-Šaḥḥāǧiyyaŧ,الشحاجية,الشحاجية,JAZIRA_420E364N_R,waystations,Point,"(42.9665, 36.27006)"
 SHAHI_443E322N_S,Šāhī,شاهي,شاهي، ساهي,IRAQ_459E319N_R,waystations,Point,"(44.36844, 32.24535)"
 SHAHRASTAN_515E298N_S,Šahrastān,شهرستان,شهرستان، سابور,SW_IRAN_540E294N_R,capitals,Point,"(51.51624, 29.83157)"
 SHAHRASTAN_552E371N_S,Šahrastān,شهرستان,شهرستان، جرجان,NW_IRAN_515E356N_R,metropoles,Point,"(55.206, 37.19091)"
 SHAHRAZUR_460E352N_R,Šahrazūr,شهرزور,شهرزور,NW_IRAN_515E356N_R,towns,Point,"(46.01676, 35.25767)"
-SHAKKI_472E413N_R,Šakkī,شكي,شكي,,regions,Point,"(47.20469, 41.34856)"
 SHAKKI_472E413N_S,Šakkī,شكي,شكي,QABQ_457E413N_R,towns,Point,"(47.20469, 41.34856)"
 SHALANBA_520E356N_S,Šalanbaŧ,شلنبة,شلنبة,NW_IRAN_515E356N_R,towns,Point,"(52.04723, 35.68449)"
 SHALJI_716E425N_S,Šalǧī,شلجي,شلجي,MAWARANNAHR_656E401N_R,towns,Point,"(71.66129, 42.59356)"
 SHALUS_514E366N_S,Šālūs,شالوس,شالوس، سالوس,NW_IRAN_515E356N_R,towns,Point,"(51.45535, 36.60408)"
 SHAMAKHIYYA_486E406N_S,al-Šamāḫiyyaŧ,الشماخية,الشماخية,QABQ_457E413N_R,villages,Point,"(48.68505, 40.67871)"
 SHAMAT_560E297N_S,al-Šāmāt,الشامات,الشامات,SW_IRAN_540E294N_R,towns,Point,"(56.01438, 29.76249)"
 SHAMKUR_460E409N_S,Šamkūr,شمكور,شمكور,QABQ_457E413N_R,towns,Point,"(46.06157, 40.99521)"
@@ -1985,43 +1890,40 @@
 SHIBAM_439E155N_S,Šibām,شبام,شبام,SW_ARABIA_456E158N_R,villages,Point,"(43.90335, 15.51632)"
 SHIBAM_485E159N_S,Šibām,شبام,شبام,SW_ARABIA_456E158N_R,towns,Point,"(48.57208, 15.92483)"
 SHIHMAR_528E361N_S,Šihmār,شهمار,شهمار، سهمار,NW_IRAN_515E356N_R,towns,Point,"(52.86652, 36.16111)"
 SHIHR_495E147N_S,al-Šiḥr,الشحر,الشحر,SW_ARABIA_456E158N_R,towns,Point,"(49.5998, 14.76671)"
 SHIMSHAT_398E386N_S,Šimšāṭ,شمشاط,شمشاط,JAZIRA_420E364N_R,waystations,Point,"(39.83119, 38.61412)"
 SHIRAK_305E309N_R,al-Širāk,الشراك,الشراك,MISR_305E292N_R,regions,Point,"(30.57342, 30.99062)"
 SHIRAZ_525E296N_S,Šīrāz,شيراز,شيراز,SW_IRAN_540E294N_R,metropoles,Point,"(52.52867, 29.61884)"
-SHIRWAN_487E411N_R,Širwān,شروان,شروان، شروان,,regions,Point,"(48.75339, 41.11585)"
 SHIRWAN_487E411N_S,Širwān,شروان,شروان، شروان,QABQ_457E413N_R,towns,Point,"(48.75339, 41.11585)"
 SHUBAYKA_415E224N_S,al-Šubaykaŧ,الشبيكة,الشبيكة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(41.51032, 22.44819)"
 SHUMAN_688E385N_S,Šūmān,شومان,شومان,MAWARANNAHR_656E401N_R,towns,Point,"(68.82268, 38.58166)"
 SHUQUQ_434E290N_S,al-Šuqūq,الشقوق,الشقوق,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.41491, 29.08495)"
 SHURAB_487E312N_S,Šūrāb,شوراب,شوراب,SW_IRAN_540E294N_R,towns,Point,"(48.79726, 31.20731)"
 SHURAKHAN_609E415N_S,Šurāḫān,شراخان,شراخان,MAWARANNAHR_656E401N_R,waystations,Point,"(60.94019, 41.50228)"
 SHURIRUDH_577E312N_S,Šūrirūḏ,شورروذ,شورروذ، شور دوازدة,SE_IRAN_656E286N_R,waystations,Point,"(57.78936, 31.27116)"
 SHURMIN_635E347N_S,Šūrmīn,شورمين,شورمين,NE_IRAN_606E351N_R,towns,Point,"(63.51568, 34.72729)"
 SHURUKH_633E400N_S,Šurūḫ,شروخ,شروخ,MAWARANNAHR_656E401N_R,waystations,Point,"(63.3995, 40.05505)"
 SIB_448E329N_S,al-Sīb,السيب,السيب,IRAQ_459E319N_R,towns,Point,"(44.8461, 32.97916)"
 SIDRA_662E368N_S,al-Sidraŧ,السدرة,السدرة,NE_IRAN_606E351N_R,waystations,Point,"(66.21231, 36.8377)"
 SIFFIN_384E358N_O,Ṣiffīn,صفين,صفين,JAZIRA_420E364N_R,sites,Point,"(38.4104, 35.8566)"
 SIFUMARA_547E267N_R,Sīf ʿUmāraŧ,سيف عمارة,سيف عمارة,SW_IRAN_540E294N_R,regions,Point,"(54.75943, 26.77937)"
-SIJILMASA_042W312N_R,Siǧilmāsaŧ,سجلماسة,سجلماسة,,regions,Point,"(-4.23723, 31.27819)"
 SIJILMASA_042W312N_S,Siǧilmāsaŧ,سجلماسة,سجلماسة,MAGHRIB_045E323N_R,capitals,Point,"(-4.23723, 31.27819)"
 SIKKAHAMMAM_267E311N_S,Sikkaŧ al-Ḥammām,سكة الحمام,سكة الحمام,BARQA_221E314N_R,waystations,Point,"(26.77604, 31.19426)"
 SIKR_467E321N_S,al-Sikr,السكر,السكر,IRAQ_459E319N_R,towns,Point,"(46.77226, 32.19607)"
 SIMAKAN_531E286N_S,al-Ṣīmakān,الصيمكان,الصيمكان,SW_IRAN_540E294N_R,towns,Point,"(53.13182, 28.69941)"
 SIMINJAN_680E362N_S,Siminǧān,سمنجان,سمنجان,NE_IRAN_606E351N_R,towns,Point,"(68.09011, 36.22585)"
 SIMNAN_534E354N_S,Simnān,سمنان,سمنان,NW_IRAN_515E356N_R,towns,Point,"(53.40856, 35.49513)"
 SINIZ_502E299N_S,Sīnīz,سينيز,سينيز، شينيز,SW_IRAN_540E294N_R,towns,Point,"(50.27838, 29.92283)"
 SINJAR_418E363N_S,Sinǧār,سنجار,سنجار,JAZIRA_420E364N_R,towns,Point,"(41.89101, 36.32446)"
 SINJ_616E374N_S,Sinǧ,سنج,سنج، سنك,NE_IRAN_606E351N_R,towns,Point,"(61.68119, 37.4648)"
 SINNNUHAS_416E393N_S,Sinn Nuḥās,سن نحاس,سن نحاس، باجنيس,QABQ_457E413N_R,waystations,Point,"(41.69403, 39.39009)"
 SINN_434E352N_S,al-Sinn,السن,السن,IRAQ_459E319N_R,towns,Point,"(43.46591, 35.26076)"
 SIRAF_523E276N_S,Sīrāf,سيراف,سيراف,SW_IRAN_540E294N_R,capitals,Point,"(52.34306, 27.69666)"
 SIRAWAN_468E335N_S,al-Sīrawān,السيروان,السيروان، الشيراوان,NW_IRAN_515E356N_R,towns,Point,"(46.86539, 33.52303)"
-SIRJAN_557E294N_R,al-Sīrǧān,السيرجان,السيرجان,,regions,Point,"(55.74854, 29.46102)"
 SIRJAN_557E294N_S,al-Sīrǧān,السيرجان,السيرجان,SW_IRAN_540E294N_R,metropoles,Point,"(55.74854, 29.46102)"
 SIRRAYN_407E198N_S,al-Sirrayn,السرين,السرين,CENTRAL_ARABIA_416E227N_R,towns,Point,"(40.76268, 19.83698)"
 SIRR_568E230N_S,al-Sirr,السر,السر,SE_ARABIA_556E220N_R,towns,Point,"(56.82897, 23.0552)"
 SISAR_469E353N_S,Sīsar,سيسر,سيسر,NW_IRAN_515E356N_R,towns,Point,"(46.98439, 35.31623)"
 SIWI_678E295N_S,Sīwī,سيوي,سيوي، سيوة,SE_IRAN_656E286N_R,capitals,Point,"(67.85288, 29.53796)"
 SIYAHKUH_522E345N_O,Siyāh Kūh,سياه كوه,سياه كوه,SE_IRAN_656E286N_R,sites,Point,"(52.27735, 34.57768)"
 SUBANIKATH_688E423N_S,Subānīkaṯ,سبانيكث,سبانيكث,MAWARANNAHR_656E401N_R,towns,Point,"(68.89105, 42.36818)"
@@ -2056,17 +1958,14 @@
 SURDUD_430E151N_R,Surdud,سردد,سردد، سردد,SW_ARABIA_456E158N_R,regions,Point,"(43.03638, 15.18964)"
 SURT_166E310N_S,Surt,سرت,سرت,BARQA_221E314N_R,towns,Point,"(16.60839, 31.09917)"
 SURU_562E271N_S,Sūrū,سورو,سورو,SW_IRAN_540E294N_R,towns,Point,"(56.21348, 27.19067)"
 SUR_352E332N_S,Ṣūr,صور,صور,SHAM_363E335N_R,towns,Point,"(35.20796, 33.26921)"
 SUSANQIN_500E350N_S,Sūsanqīn,سوسنقين,سوسنقين، سوسنقين، سونقين,NW_IRAN_515E356N_R,waystations,Point,"(50.02954, 35.0274)"
 SUSAQAN_617E376N_S,al-Sūsaqān,السوسقان,السوسقان، السوسقان,NE_IRAN_606E351N_R,towns,Point,"(61.73152, 37.68151)"
 SUSA_106E358N_S,Sūsaŧ,سوسة,سوسة,IFRIQIYYA_78E349N_R,towns,Point,"(10.6156, 35.81044)"
-SUSA_106E358N_S,Sūsaŧ,سوسة,سوسة,IFRIQIYYA_78E349N_R,towns,Point,"(10.6156, 35.81044)"
-SUS_482E322N_R,Sūs,سوس,سوس,,regions,Point,"(48.26047, 32.20166)"
-SUS_482E322N_S,Sūs,سوس,سوس,SW_IRAN_540E294N_R,capitals,Point,"(48.26047, 32.20166)"
 SUS_482E322N_S,Sūs,سوس,سوس,SW_IRAN_540E294N_R,capitals,Point,"(48.26047, 32.20166)"
 SUTURKATH_688E408N_S,Sutūrkaṯ,ستوركث,ستوركث، أشتوركث,MAWARANNAHR_656E401N_R,towns,Point,"(68.87652, 40.88768)"
 SUWAKIN_373E191N_S,Suwākin,سواكن,سواكن,MISR_305E292N_R,villages,Point,"(37.33032, 19.11304)"
 SUWARIQIYYA_403E232N_S,al-Suwāriqiyyaŧ,السوارقية,السوارقية,CENTRAL_ARABIA_416E227N_R,towns,Point,"(40.35548, 23.28483)"
 SUWAR_499E544N_S,Suwār,سوار,سوار,QABQ_457E413N_R,towns,Point,"(49.96347, 54.45304)"
 SUWAYDA_365E326N_S,Suwaydāʾ,سويداء,سويداء,SHAM_363E335N_R,villages,Point,"(36.55945, 32.69627)"
 SUWAYDA_390E250N_S,al-Suwaydāʾ,السويداء,السويداء، السويدية,CENTRAL_ARABIA_416E227N_R,villages,Point,"(39.03019, 25.04884)"
@@ -2088,23 +1987,21 @@
 TABISTAN_538E289N_S,Ṭabistān,طبستان,طبستان، طمستان، طمارستان,SW_IRAN_540E294N_R,towns,Point,"(53.81699, 28.94971)"
 TABRISH_500E347N_R,Ṭabrīš,طبريش,طبريش,NW_IRAN_515E356N_R,regions,Point,"(50.09809, 34.71922)"
 TABRIZ_463E380N_S,Tabrīz,تبريز,تبريز,QABQ_457E413N_R,towns,Point,"(46.33121, 38.06387)"
 TABUK_365E283N_S,Tabūk,تبوك,تبوك,CENTRAL_ARABIA_416E227N_R,towns,Point,"(36.5062, 28.37114)"
 TADMUR_382E345N_S,Tadmur,تدمر,تدمر,SHAM_363E335N_R,towns,Point,"(38.28754, 34.54735)"
 TAHA_306E282N_S,Ṭaḥā,طحا,طحا,MISR_305E292N_R,towns,Point,"(30.69125, 28.27313)"
 TAHIRIYYA_625E398N_S,al-Ṭāhiriyyaŧ,الطاهرية,الطاهرية,MAWARANNAHR_656E401N_R,villages,Point,"(62.52055, 39.80992)"
-TAHIRT_013E353N_R,Tāhirt,تاهرت,تاهرت,,regions,Point,"(1.36504, 35.36971)"
 TAHIRT_013E353N_S,Tāhirt,تاهرت,تاهرت,MAGHRIB_045E323N_R,capitals,Point,"(1.36504, 35.36971)"
 TAHUDHA_058E347N_S,Tahūḏā,تهوذا,تهوذا,IFRIQIYYA_78E349N_R,towns,Point,"(5.82783, 34.79932)"
 TAHUNA_283E308N_S,al-Ṭaḥūnaŧ,الطحونة,الطحونة,BARQA_221E314N_R,waystations,Point,"(28.30167, 30.84844)"
 TAIF_404E212N_S,al-Ṭāʾif,الطائف,الطائف,CENTRAL_ARABIA_416E227N_R,towns,Point,"(40.40566, 21.21629)"
 TAJANNA_013E363N_S,Taǧannaŧ,تجنة,تجنة,MAGHRIB_045E323N_R,towns,Point,"(1.35022, 36.34557)"
 TAKRIT_436E345N_S,Takrīt,تكريت,تكريت,IRAQ_459E319N_R,towns,Point,"(43.69617, 34.59215)"
 TALABIRA_048W399N_S,Ṭalābiraŧ,طلابرة,طلابرة,ANDALUS_040E398N_R,towns,Point,"(-4.82541, 39.97062)"
-TALAQAN_508E361N_R,Ṭalaqān,طلقان,طلقان,,regions,Point,"(50.84322, 36.18658)"
 TALAQAN_508E361N_S,Ṭalaqān,طلقان,طلقان,NW_IRAN_515E356N_R,towns,Point,"(50.84322, 36.18658)"
 TALAQAN_642E357N_S,Ṭalaqān,طلقان,طلقان,NE_IRAN_606E351N_R,towns,Point,"(64.24579, 35.72328)"
 TALAQAN_696E367N_S,Ṭālaqān,طالقان,طالقان,NE_IRAN_606E351N_R,towns,Point,"(69.62314, 36.76021)"
 TALASTANA_614E370N_S,Talastānaŧ,تلستانة,تلستانة,NE_IRAN_606E351N_R,waystations,Point,"(61.47492, 37.03409)"
 TALLABDA_387E366N_S,Tall ʿAbdā,تل عبدا,تل عبدا,JAZIRA_420E364N_R,waystations,Point,"(38.72906, 36.69218)"
 TALLAFAR_424E363N_S,Tall Aʿfar,تل أعفر,تل أعفر,JAZIRA_420E364N_R,towns,Point,"(42.49401, 36.36312)"
 TALLFAFAN_417E377N_S,Tall Fāfān,تل فافان,تل فافان، عين تل فافان,JAZIRA_420E364N_R,towns,Point,"(41.78238, 37.72559)"
@@ -2149,15 +2046,14 @@
 THAJR_378E288N_S,Ṯaǧr,ثجر,ثجر,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(37.89149, 28.87521)"
 THALABIYYA_431E282N_S,al-Ṯaʿlabiyyaŧ,الثعلبية,الثعلبية,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.16528, 28.29472)"
 THAMANIN_426E373N_S,Ṯamānīn,ثمانين,ثمانين,JAZIRA_420E364N_R,towns,Point,"(42.64158, 37.31295)"
 THANIYYA_463E240N_R,al-Ṯaniyyaŧ,الثنية,الثنية,CENTRAL_ARABIA_416E227N_R,regions,Point,"(46.32366, 24.02771)"
 THATWA-RADA_447E144N_R,Ṯāt wa-Radāʿ,ثات ورداع,ثات ورداع,SW_ARABIA_456E158N_R,regions,Point,"(44.76857, 14.4846)"
 THIRMA_137E379N_S,Ṯirmaŧ,ثرمة,ثرمة,SIQILIYYA_145E375N_R,towns,Point,"(13.70463, 37.97037)"
 THUJJA_431E181N_S,al-Ṯuǧǧaŧ,الثجة,الثجة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.19302, 18.1711)"
-THUJJA_441E139N_R,al-Ṯuǧǧaŧ,الثجة,الثجة,,regions,Point,"(44.17683, 13.97911)"
 THUJJA_441E139N_S,al-Ṯuǧǧaŧ,الثجة,الثجة,SW_ARABIA_456E158N_R,capitals,Point,"(44.17683, 13.97911)"
 THURABDIN_408E374N_S,Ṯūr ʿAbdīn,ثور عبدين,ثور عبدين,JAZIRA_420E364N_R,towns,Point,"(40.86321, 37.40165)"
 TIB_473E322N_S,al-Ṭīb,الطيب,الطيب,IRAQ_459E319N_R,towns,Point,"(47.30428, 32.22674)"
 TIDA_308E312N_R,Tīdaŧ,تيدة,تيدة,MISR_305E292N_R,regions,Point,"(30.827, 31.23866)"
 TIFLIS_448E420N_S,Tiflīs,تفليس,تفليس,QABQ_457E413N_R,towns,Point,"(44.83734, 42.0841)"
 TIHAMA_425E175N_R,Tihāmaŧ,تهامة,تهامة,CENTRAL_ARABIA_416E227N_R,regions,Point,"(42.51067, 17.58374)"
 TIHBANUISRAIL_338E291N_R,Tīh Banū Isrāʾil,تيه بنو إسرائل,تيه بنو إسرائل,MISR_305E292N_R,regions,Point,"(33.80128, 29.16755)"
@@ -2172,15 +2068,14 @@
 TIZA_040W342N_S,Tīzā,تيزا,تيزا، تازة,MAGHRIB_045E323N_R,towns,Point,"(-4.02927, 34.22102)"
 TIZIN_367E362N_S,Tīzīn,تيزين,تيزين، توزين,SHAM_363E335N_R,towns,Point,"(36.70483, 36.23776)"
 TIZ_606E253N_S,al-Tīz,التيز,التيز,SE_IRAN_656E286N_R,towns,Point,"(60.63196, 25.38207)"
 TUAM_557E241N_S,Tuʾām,تؤام,تؤام,SE_ARABIA_556E220N_R,towns,Point,"(55.77403, 24.19401)"
 TUBNA_053E353N_S,Ṭubnaŧ,طبنة,طبنة,IFRIQIYYA_78E349N_R,towns,Point,"(5.35573, 35.32395)"
 TUDMIR_013W379N_R,Tudmīr,تدمير,تدمير,ANDALUS_040E398N_R,regions,Point,"(-1.34462, 37.95834)"
 TUKHARISTAN_686E360N_R,Ṭuḫāristān,طخارستان,طخارستان,NE_IRAN_606E351N_R,regions,Point,"(68.67012, 36.03586)"
-TULAYTILA_040W398N_R,Ṭulayṭilaŧ,طليطلة,طليطلة,,regions,Point,"(-4.0521, 39.88926)"
 TULAYTILA_040W398N_S,Ṭulayṭilaŧ,طليطلة,طليطلة,ANDALUS_040E398N_R,towns,Point,"(-4.0521, 39.88926)"
 TUMAYY_315E309N_R,Ṭumayy,طمي,طمي,MISR_305E292N_R,regions,Point,"(31.51063, 30.94376)"
 TUNANIR_408E363N_S,Tunānīr,تنانير,تنانير، تنينير,JAZIRA_420E364N_R,towns,Point,"(40.87703, 36.38969)"
 TUNA_320E311N_S,Tūnaŧ,تونة,تونة,MISR_305E292N_R,towns,Point,"(32.0824, 31.16442)"
 TUNIS_101E367N_S,Tūnis,تونس,تونس,IFRIQIYYA_78E349N_R,towns,Point,"(10.17736, 36.77071)"
 TUNKATH_702E410N_S,Tūnkaṯ,تونكث,تونكث,MAWARANNAHR_656E401N_R,capitals,Point,"(70.22483, 41.01789)"
 TUN_581E339N_S,Tūn,تون,تون,NE_IRAN_606E351N_R,towns,Point,"(58.11679, 33.92591)"
@@ -2190,19 +2085,16 @@
 TURMUGHAN_708E407N_S,Turmuġān,ترمغان,ترمغان، طرمقان,MAWARANNAHR_656E401N_R,villages,Point,"(70.89318, 40.78105)"
 TURSINA_339E283N_O,Ṭūr Sīnāʾ,طور سيناء,طور سيناء,MISR_305E292N_R,sites,Point,"(33.95454, 28.35876)"
 TURTHITH_584E351N_S,Ṭurṯīṯ,طرثيث,طرثيث، ترشيز، طريثيث,NE_IRAN_606E351N_R,capitals,Point,"(58.4113, 35.13557)"
 TURTUSHA_006E407N_S,Ṭurṭūšaŧ,طرطوشة,طرطوشة,ANDALUS_040E398N_R,towns,Point,"(0.60933, 40.79221)"
 TUSHTAN_578E294N_S,Tūštān,توشتان,توشتان,SW_IRAN_540E294N_R,towns,Point,"(57.80931, 29.4241)"
 TUSHUMMUS_059W350N_S,Tušummus,تشمس,تشمس,MAGHRIB_045E323N_R,towns,Point,"(-5.95157, 35.07007)"
 TUSHUMMUS_059W350N_W,Tušummus,تشمس,تشمس,MAGHRIB_045E323N_R,waters,Point,"(-5.95157, 35.07007)"
-TUSTAR_488E320N_R,Tustar,تستر,تستر، ششتر,,regions,Point,"(48.85461, 32.0511)"
 TUSTAR_488E320N_S,Tustar,تستر,تستر، ششتر,SW_IRAN_540E294N_R,capitals,Point,"(48.85461, 32.0511)"
-TUS_594E364N_R,Ṭūs,طوس,طوس، طابران,,regions,Point,"(59.49915, 36.42208)"
 TUS_594E364N_S,Ṭūs,طوس,طوس، طابران,NE_IRAN_606E351N_R,capitals,Point,"(59.49915, 36.42208)"
-TUTILA_016W420N_R,Tuṭīlaŧ,تطيلة,تطيلة,,regions,Point,"(-1.62697, 42.04634)"
 TUTILA_016W420N_S,Tuṭīlaŧ,تطيلة,تطيلة,ANDALUS_040E398N_R,towns,Point,"(-1.62697, 42.04634)"
 TUWWA_309E306N_R,Ṭuwwaŧ,طوة,طوة,,regions,Point,"(30.93316, 30.68075)"
 TUZ_422E267N_S,Tūz,توز,توز,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(42.29198, 26.71435)"
 UBAYR_367E307N_S,Ubayr,أبير,أبير، وبير,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(36.70106, 30.73317)"
 UBBA_087E358N_S,Ubbaŧ,أبة,أبة,IFRIQIYYA_78E349N_R,villages,Point,"(8.72082, 35.80744)"
 UBULLA_478E304N_S,al-Ubullaŧ,الأبلة,الأبلة,IRAQ_459E319N_R,towns,Point,"(47.83555, 30.49692)"
 UDHAYB_441E314N_S,al-Uḏayb,الأذيب,الأذيب,CENTRAL_ARABIA_416E227N_R,villages,Point,"(44.13666, 31.49049)"
@@ -2225,15 +2117,14 @@
 URF_442E150N_S,al-ʿUrf,العرف,العرف,SW_ARABIA_456E158N_R,towns,Point,"(44.27297, 15.09101)"
 URMIYA_450E375N_S,Urmīyaŧ,أرميية,أرميية,QABQ_457E413N_R,towns,Point,"(45.07411, 37.52011)"
 URSH_428E169N_S,al-ʿUrš,العرش,العرش,SW_ARABIA_456E158N_R,waystations,Point,"(42.82787, 16.96745)"
 URUNT_364E359N_W,al-Urunṭ,الأرنط,الأرنط، الأرند,SHAM_363E335N_R,waters,Point,"(36.42208, 35.99287)"
 USAYLA_407E250N_S,al-ʿUsaylaŧ,العسيلة,العسيلة,CENTRAL_ARABIA_416E227N_R,villages,Point,"(40.79626, 25.04085)"
 USFAN_394E218N_S,ʿUsfān,عسفان,عسفان,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(39.46144, 21.88079)"
 USHMUNAYN_307E278N_S,al-Ušmūnayn,الأشمونين,الأشمونين,MISR_305E292N_R,towns,Point,"(30.75576, 27.85616)"
-USHMUNAYN_307E278N_S,al-Ušmūnayn,الأشمونين,الأشمونين,MISR_305E292N_R,towns,Point,"(30.75576, 27.85616)"
 USHNUH_451E370N_S,Ušnuh,أشنه,أشنه,QABQ_457E413N_R,towns,Point,"(45.12379, 37.02695)"
 USHRUSANA_687E395N_R,Ušrūsanaŧ,أشروسنة,أشروسنة,MAWARANNAHR_656E401N_R,regions,Point,"(68.72187, 39.56749)"
 USHTIQAN_720E406N_S,Uštīqān,أشتيقان,أشتيقان,MAWARANNAHR_656E401N_R,towns,Point,"(72.05745, 40.67718)"
 USHTURMAGHAK_613E368N_S,Ušturmaġāk,أشترمغاك,أشترمغاك,NE_IRAN_606E351N_R,villages,Point,"(61.32517, 36.8048)"
 USH_728E405N_S,Ūš,أوش,أوش,MAWARANNAHR_656E401N_R,towns,Point,"(72.85752, 40.53599)"
 USWAN_329E241N_S,Uswān,أسوان,أسوان,MISR_305E292N_R,capitals,Point,"(32.98286, 24.10701)"
 UWAL_505E261N_R,Uwāl,أوال,أوال,SE_ARABIA_556E220N_R,regions,Point,"(50.56693, 26.11827)"
@@ -2243,15 +2134,14 @@
 WADIALLAQI_341E221N_W,Wādī ʿAllaqī,وادي علقي,وادي علقي,MISR_305E292N_R,waters,Point,"(34.10934, 22.13452)"
 WADIAQIQ_402E241N_W,Wādī al-ʿAqīq,وادي العقيق,وادي العقيق,CENTRAL_ARABIA_416E227N_R,waters,Point,"(40.29083, 24.11089)"
 WADIA_438E160N_R,Wādiʿaŧ,وادعة,وادعة,SW_ARABIA_456E158N_R,regions,Point,"(43.80678, 16.03244)"
 WADIDARA_074W309N_W,Wādī Darʿaŧ,وادي درعة,وادي درعة,MAGHRIB_045E323N_R,waters,Point,"(-7.42487, 30.93544)"
 WADIDARA_080W291N_W,Wādī Darʿaŧ,وادي درعة,وادي درعة,MAGHRIB_045E323N_R,waters,Point,"(-8.07804, 29.19903)"
 WADIFUR_390E230N_W,Wādī Furʿ,وادي فرع,وادي فرع,CENTRAL_ARABIA_416E227N_R,waters,Point,"(39.0919, 23.06872)"
 WADIHAYRAN_430E160N_W,Wādī Ḥayrān,وادي حيران,وادي حيران,SW_ARABIA_456E158N_R,waters,Point,"(43.06403, 16.05227)"
-WADIHIJARA_031W406N_R,Wādī al-Ḥijāraŧ,وادي الحجارة,وادي الحجارة,,regions,Point,"(-3.15111, 40.6491)"
 WADIHIJARA_031W406N_S,Wādī al-Ḥijāraŧ,وادي الحجارة,وادي الحجارة,ANDALUS_040E398N_R,towns,Point,"(-3.15111, 40.6491)"
 WADIINAWAN_043W342N_W,Wādī Īnāwan,وادي إيناون,وادي إيناون,MAGHRIB_045E323N_R,waters,Point,"(-4.39975, 34.24946)"
 WADIKHARID_444E159N_W,Wādī al-Ḫārid,وادي الخارد,وادي الخارد,SW_ARABIA_456E158N_R,waters,Point,"(44.43363, 15.95585)"
 WADIKHULAB_430E167N_W,Wādī Ḫulab,وادي خلب,وادي خلب,SW_ARABIA_456E158N_R,waters,Point,"(43.0017, 16.70128)"
 WADIMAKHIL_226E322N_W,Wādī Maḫīl,وادي مخيل,وادي مخيل,BARQA_221E314N_R,waters,Point,"(22.62048, 32.2648)"
 WADIMALAL_440E154N_R,Wāḍiʿ al-Maʿlal,واضع المعلل,واضع المعلل,SW_ARABIA_456E158N_R,regions,Point,"(44.0447, 15.45244)"
 WADIMALIH_031E361N_W,Wādī al-Māliḥ,وادي المالح,وادي المالح,MAGHRIB_045E323N_R,waters,Point,"(3.18573, 36.1099)"
@@ -2293,21 +2183,19 @@
 WARDHANA_643E401N_S,Warḏānaŧ,ورذانة,ورذانة، أورذانة,MAWARANNAHR_656E401N_R,towns,Point,"(64.30515, 40.15432)"
 WARIKA_076W314N_S,Warīkaŧ,وريكة,وريكة، أغمات وريكة,MAGHRIB_045E323N_R,towns,Point,"(-7.6357, 31.44535)"
 WARRADA_335E310N_S,al-Warrādaŧ,الورادة,الورادة,MISR_305E292N_R,towns,Point,"(33.54242, 31.06734)"
 WARTHAN_476E395N_S,Warṯān,ورثان,ورثان,QABQ_457E413N_R,towns,Point,"(47.64257, 39.56659)"
 WARWALIJ_688E367N_S,Warwālīǧ,ورواليج,ورواليج، ولواليز,NE_IRAN_606E351N_R,towns,Point,"(68.89729, 36.78174)"
 WARZAQAN_466E385N_S,Warzaqān,ورزقان,ورزقان,QABQ_457E413N_R,towns,Point,"(46.66017, 38.56125)"
 WASHJIRD_692E384N_S,Wašǧird,وشجرد,وشجرد، دستجرد، دستكرد,MAWARANNAHR_656E401N_R,capitals,Point,"(69.21115, 38.46704)"
-WASHQA_003W421N_R,Wašqaŧ,وشقة,وشقة,,regions,Point,"(-0.35371, 42.16109)"
 WASHQA_003W421N_S,Wašqaŧ,وشقة,وشقة,ANDALUS_040E398N_R,towns,Point,"(-0.35371, 42.16109)"
 WASIJ_681E426N_S,Wasīǧ,وسيج,وسيج,MAWARANNAHR_656E401N_R,towns,Point,"(68.12972, 42.63098)"
 WASIM_311E301N_S,Wasīm,وسيم,وسيم,MISR_305E292N_R,towns,Point,"(31.10905, 30.12144)"
 WASIT_463E321N_S,Wāsiṭ,واسط,واسط,IRAQ_459E319N_R,capitals,Point,"(46.32308, 32.19497)"
 WASTAN_431E383N_S,Wasṭān,وسطان,وسطان,QABQ_457E413N_R,towns,Point,"(43.13392, 38.34421)"
-WAYHIND_722E339N_R,Wayhind,ويهند,ويهند,,regions,Point,"(72.24681, 33.90757)"
 WAYHIND_722E339N_S,Wayhind,ويهند,ويهند,SE_IRAN_656E286N_R,capitals,Point,"(72.24681, 33.90757)"
 WAYKHAN_601E420N_S,Wāyḫān,وايخان,وايخان,MAWARANNAHR_656E401N_R,towns,Point,"(60.19436, 42.0552)"
 WAZARMAND_597E418N_S,Wazārmand,وزارمند,وزارمند، أوزارمند,MAWARANNAHR_656E401N_R,towns,Point,"(59.74298, 41.86361)"
 WAZKARD_672E394N_S,Wazkard,وزكرد,وزكرد، وزكردة,MAWARANNAHR_656E401N_R,villages,Point,"(67.29033, 39.42539)"
 WINKARD_684E405N_S,Wīnkard,وينكرد,وينكرد,MAWARANNAHR_656E401N_R,villages,Point,"(68.43871, 40.57316)"
 WUJAYN_757E232N_S,Wuǧayn,وجين,وجين,SE_IRAN_656E286N_R,towns,Point,"(75.78308, 23.20809)"
 YABAMBAM_428E188N_S,Yabambam,يبمبم,يبمبم، يبنبم,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(42.82847, 18.87682)"
@@ -2320,15 +2208,14 @@
 YAHUDIYYA_648E359N_S,al-Yahūdiyyaŧ,اليهودية,اليهودية، جكوذان,NE_IRAN_606E351N_R,waystations,Point,"(64.83857, 35.9347)"
 YAJ_151E376N_S,al-Yāǧ,الياج,الياج,SIQILIYYA_145E375N_R,towns,Point,"(15.1673, 37.62947)"
 YALAMLAM_400E208N_S,Yalamlam,يلملم,يلملم,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(40.08231, 20.84741)"
 YAMAMA_467E240N_R,al-Yamāmaŧ,اليمامة,اليمامة,CENTRAL_ARABIA_416E227N_R,regions,Point,"(46.73506, 24.08674)"
 YAM_446E159N_R,Yām,يام,يام,SW_ARABIA_456E158N_R,regions,Point,"(44.67244, 15.92968)"
 YANBU_381E241N_S,Yanbuʿ,ينبع,ينبع,CENTRAL_ARABIA_416E227N_R,towns,Point,"(38.12512, 24.1082)"
 YAZDAKHAWAST_544E283N_S,Yazdaḫawāst,يزدخواست,يزدخواست,SW_IRAN_540E294N_R,towns,Point,"(54.43137, 28.33754)"
-YAZD_543E319N_R,Yazd,يزد,يزد، كثة,,regions,Point,"(54.34286, 31.90975)"
 YAZD_543E319N_S,Yazd,يزد,يزد، كثة,SW_IRAN_540E294N_R,towns,Point,"(54.34286, 31.90975)"
 YUBNA_347E318N_S,Yubnā,يبنا,يبنا,SHAM_363E335N_R,villages,Point,"(34.73521, 31.87092)"
 YUNABIDH_586E342N_S,Yunābīḏ,ينابيذ,ينابيذ، جنابذ,NE_IRAN_606E351N_R,towns,Point,"(58.63618, 34.24652)"
 ZABADANI_360E337N_S,Zabadānī,زبداني,زبداني,SHAM_363E335N_R,villages,Point,"(36.08756, 33.73115)"
 ZABID_433E142N_S,Zabīd,زبيد,زبيد,SW_ARABIA_456E158N_R,capitals,Point,"(43.32654, 14.20796)"
 ZABKABIR_438E363N_W,Zāb al-Kabīr,زاب الكبير,زاب الكبير، زاب الأعلى,JAZIRA_420E364N_R,waters,Point,"(43.87398, 36.3752)"
 ZABSAGHIR_441E356N_W,Zāb al-Ṣaġīr,زاب الصغير,زاب الصغير، زاب الأسفل,JAZIRA_420E364N_R,waters,Point,"(44.10965, 35.64182)"
@@ -2357,7 +2244,26 @@
 ZIFTAJAWAD_312E307N_S,Ziftā Ǧawād,زفتا جواد,زفتا جواد,MISR_305E292N_R,towns,Point,"(31.21094, 30.70718)"
 ZIRADABADH_553E366N_S,Ziradābāḏ,زرداباذ,زرداباذ، زرداباذ,NW_IRAN_515E356N_R,waystations,Point,"(55.30802, 36.65798)"
 ZIYADABADHZIYADAWADH_532E298N_S,ZiyādābāḏZiyādāwāḏ,زياداباذزياداواذ,زياداباذزياداواذ,,waystations,Point,"(53.22441, 29.83708)"
 ZUBALA_435E294N_S,Zubālaŧ,زبالة,زبالة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.5639, 29.40521)"
 ZUBAYDIYYA_468E342N_S,al-Zubaydiyyaŧ,الزبيدية,الزبيدية,NW_IRAN_515E356N_R,waystations,Point,"(46.85168, 34.23099)"
 ZUBAYDIYYA_469E344N_S,al-Zubaydiyyaŧ,الزبيدية,الزبيدية,NW_IRAN_515E356N_R,waystations,Point,"(46.93427, 34.43457)"
 ZUZAN_598E343N_S,Zūzan,زوزن,زوزن,NE_IRAN_606E351N_R,towns,Point,"(59.86207, 34.3105)"
+ANDALUS_040E398N_R,al-Andalus,الأندلس,الأندلس,,regions,Point,"(-4.0521, 39.88926)"
+BARQA_221E314N_R,Barqaŧ,برقة,برقة,,regions,Point,"(22.1, 31.4)"
+CENTRAL_ARABIA_416E227N_R,al-Ḥijāz+,الجزيرة,الجزيرة، أقور,,regions,Point,"(41.65725, 22.78726)"
+IFRIQIYYA_78E349N_R,Ifriqiyyā,إفريقية,إفريقية,,regions,Point,"(7.8, 34.9)"
+IRAQ_459E319N_R,al-ʿIrāq,العراق,العراق,,regions,Point,"(45.96, 31.9)"
+JAZIRA_420E364N_R,al-Jazīraŧ,جزيرة,جزيرة، جزيرة العرب,,regions,Point,"(42.05, 36.41)"
+MAGHRIB_045E323N_R,al-Maġrib,المغرب,المغرب,,regions,Point,"(-4.52149, 32.30201)"
+MAWARANNAHR_656E401N_R,Mā warāʾ al-nahr,ما وراء النهر,ما وراء النهر,,regions,Point,"(65.61472, 40.1917)"
+MISR_305E292N_R,Miṣr,مصر,مصر، الديار المصرية,,regions,Point,"(30.52, 29.23)"
+NE_IRAN_606E351N_R,Ḫurāsān,خراسان,خراسان,,regions,Point,"(60.61524, 35.17917)"
+NW_IRAN_515E356N_R,al-Jibāl+,الجبال,الجبال، الجبل,,regions,Point,"(51.50831, 35.62754)"
+QABQ_457E413N_R,al-Riḥāb,الرحاب,الرحاب,,regions,Point,"(45.79, 41.33)"
+RUM_335E392N_R,al-Rūm,الروم,الروم، بلد الروم,,regions,Point,"(33.57, 39.21)"
+SE_ARABIA_556E220N_R,ʿUmān+,,,,regions,Point,"(55.67, 22.01)"
+SE_IRAN_656E286N_R,Sījīstān+,سجستان,سجستان، سيستان,,regions,Point,"(65.61472, 28.62665)"
+SHAM_363E335N_R,al-Šām,الشام,الشام، شام,,regions,Point,"(36.30199, 33.51843)"
+SIQILIYYA_145E375N_R,Ṣiqiliyyaŧ,,,,regions,Point,"(14.5, 37.57)"
+SW_ARABIA_456E158N_R,al-Yaman,اليمن,اليمن,,regions,Point,"(45.68, 15.82)"
+SW_IRAN_540E294N_R,Fārs+,فارس,فارس,,regions,Point,"(54.00, 29.43)"
```

### Comparing `eis1600-0.9.2/eis1600/helper/EntityTags.py` & `eis1600-0.9.3/eis1600/helper/EntityTags.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from importlib_resources import files
 from typing import List
-import pandas as pd
+from pandas import read_csv, DataFrame
+
 from eis1600.helper.Singleton import Singleton
 
 entities_path = files('eis1600.helper.data').joinpath('entity_tags.csv')
 
 
 @Singleton
 class EntityTags:
     __entity_tags_df = None
     __tag_list = None
     __nasab_tag_list = None
 
     def __init__(self) -> None:
-        entity_tags_df = pd.read_csv(entities_path)
+        entity_tags_df = read_csv(entities_path)
         EntityTags.__entity_tags_df = entity_tags_df
         EntityTags.__tag_list = entity_tags_df.loc[entity_tags_df['CATEGORY'].notna(), 'TAG'].to_list()
         EntityTags.__nasab_tag_list = entity_tags_df.loc[entity_tags_df['CATEGORY'] == 'ONOMASTIC', 'TAG'].to_list()
 
     @staticmethod
-    def get_entity_tags_df() -> pd.DataFrame:
+    def get_entity_tags_df() -> DataFrame:
         return EntityTags.__entity_tags_df
 
     @staticmethod
     def get_entity_tags() -> List[str]:
         return EntityTags.__tag_list
 
     @staticmethod
```

### Comparing `eis1600-0.9.2/eis1600/helper/Singleton.py` & `eis1600-0.9.3/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/helper/ar_normalization.py` & `eis1600-0.9.3/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.9.3/eis1600/helper/fix_miu_annotation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import re
+from re import compile
 from glob import glob
 from p_tqdm import p_uimap
 from eis1600.processing.preprocessing import get_yml_and_miu_df
 from eis1600.processing.postprocessing import write_updated_miu_to_file
 
 
-sheikhuna = re.compile('[و]?شيخنا')
+sheikhuna = compile('[و]?شيخنا')
 
 
 def untag_sheikhuna(row):
     if row['TOKENS'] and sheikhuna.match(row['TOKENS']) and row['TAGS_LISTS'] and [tag for tag in row['TAGS_LISTS']
                                                                                    if tag.startswith('P1')]:
         if len(row['TAGS_LISTS']) > 1:
             row['TAGS_LISTS'].pop()
```

### Comparing `eis1600-0.9.2/eis1600/helper/markdown_methods.py` & `eis1600-0.9.3/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/helper/markdown_patterns.py` & `eis1600-0.9.3/eis1600/helper/markdown_patterns.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import re
+from re import compile
 
 from eis1600.helper.EntityTags import EntityTags
 
 AR_LETTERS_CHARSET = frozenset(
         u'\u0621\u0622\u0623\u0624\u0625\u0626\u0627'
         u'\u0628\u0629\u062a\u062b\u062c\u062d\u062e'
         u'\u062f\u0630\u0631\u0632\u0633\u0634\u0635'
@@ -13,70 +13,70 @@
 AR_CHR = r'[' + u''.join(AR_LETTERS_CHARSET) + ']'
 AR_STR = AR_CHR + '+'
 AR_STR_AND_TAGS = r'[' + u''.join(AR_LETTERS_CHARSET) + 'a-zA-ZÜ0-9]+'
 WORD = r'(?:\s' + AR_STR + ')'
 
 # EIS1600 mARkdown
 UID = r'_ء_(#)?=(?P<UID>\d{12})= '
-UID_PATTERN = re.compile(UID)
+UID_PATTERN = compile(UID)
 MIU_UID = r'_ء_#=(?P<UID>\d{12})= '
-MIU_UID_PATTERN = re.compile(MIU_UID)
-HEADER_END_PATTERN = re.compile(r'(#META#Header#End#)\n')
+MIU_UID_PATTERN = compile(MIU_UID)
+HEADER_END_PATTERN = compile(r'(#META#Header#End#)\n')
 MIU_HEADER = r'#MIU#Header#'
-MIU_HEADER_PATTERN = re.compile(MIU_HEADER)
-HEADING_PATTERN = re.compile(UID + r'(?P<level>[|]+) (?P<heading>.*)\n')
-EMPTY_PARAGRAPH_PATTERN = re.compile(UID + r'::UNDEFINED:: ~')
-EMPTY_FIRST_PARAGRAPH_PATTERN = re.compile(r'_ء_#=\d{12}=')
+MIU_HEADER_PATTERN = compile(MIU_HEADER)
+HEADING_PATTERN = compile(UID + r'(?P<level>[|]+) (?P<heading>.*)\n')
+EMPTY_PARAGRAPH_PATTERN = compile(UID + r'::UNDEFINED:: ~')
+EMPTY_FIRST_PARAGRAPH_PATTERN = compile(r'_ء_#=\d{12}=')
 PAGE_TAG = r' ?(?P<page_tag>PageV\d{2}P\d{3,})'
-PAGE_TAG_PATTERN = re.compile(PAGE_TAG)
+PAGE_TAG_PATTERN = compile(PAGE_TAG)
 ONLY_PAGE_TAG = UID + r'::UNDEFINED:: ~\n' + PAGE_TAG
-ONLY_PAGE_TAG_PATTERN = re.compile(ONLY_PAGE_TAG)
-PAGE_TAG_IN_BETWEEN_PATTERN = re.compile(
+ONLY_PAGE_TAG_PATTERN = compile(ONLY_PAGE_TAG)
+PAGE_TAG_IN_BETWEEN_PATTERN = compile(
         AR_STR + r' ?' + r'\n\n' + ONLY_PAGE_TAG + r'\n\n' + r'_ء_=\d{12}= ::[A-Z]+:: ~\n' + AR_STR
 )
 
 # MIU_TAG_PATTERN is used to split text - indices depend on the number of capturing groups so be careful when
 # changing them
-MIU_TAG_PATTERN = re.compile(r'(' + MIU_UID + r'(?P<category>[^\n]+))')
-CATEGORY_PATTERN = re.compile(r'[$|@]+(?:[A-Z]+[|])?')
+MIU_TAG_PATTERN = compile(r'(' + MIU_UID + r'(?P<category>[^\n]+))')
+CATEGORY_PATTERN = compile(r'[$|@]+(?:[A-Z]+[|])?')
 SECTION_TAG = r'_ء_=\d{12}= ::[A-Z]+:: ~'
-SECTION_PATTERN = re.compile(SECTION_TAG)
-SECTION_SPLITTER_PATTERN = re.compile(r'\n\n(' + SECTION_TAG + ')\n(?:_ء_)?')
-TAG_PATTERN = re.compile(r'Ü?(?:[a-zA-Z0-9_%~]+(?:\.[a-zA-Z0-9_%~]+)?)|' + PAGE_TAG + '|(?:::)')
+SECTION_PATTERN = compile(SECTION_TAG)
+SECTION_SPLITTER_PATTERN = compile(r'\n\n(' + SECTION_TAG + ')\n(?:_ء_)?')
+TAG_PATTERN = compile(r'Ü?(?:[a-zA-Z0-9_%~]+(?:\.[a-zA-Z0-9_%~]+)?)|' + PAGE_TAG + '|(?:::)')
 NOR_DIGIT_NOR_AR_STR = r'[^\d\n' + u''.join(AR_LETTERS_CHARSET) + ']+?'
 TAG_AND_TEXT_SAME_LINE = r'([$@]+' + NOR_DIGIT_NOR_AR_STR + r'\d*' + NOR_DIGIT_NOR_AR_STR + r') ?((?:[(\[] ?)?' + AR_STR + r')'
-UID_TAG_AND_TEXT_SAME_LINE_PATTERN = re.compile(
+UID_TAG_AND_TEXT_SAME_LINE_PATTERN = compile(
         r'(_ء_#=\d{12}= )' + TAG_AND_TEXT_SAME_LINE)
-MIU_TAG_AND_TEXT_PATTERN = re.compile(r'(' + MIU_UID + r'[$@]+?(?: \d+)?)\n((?:\( ?)?' + AR_STR + r')')
+MIU_TAG_AND_TEXT_PATTERN = compile(r'(' + MIU_UID + r'[$@]+?(?: \d+)?)\n((?:\( ?)?' + AR_STR + r')')
 
 # MIU entity tags
 entity_tags = '|'.join(EntityTags.instance().get_entity_tags())
-ENTITY_TAGS_PATTERN = re.compile(r'Ü?(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})(?:[A-Z0-9]+)?')
-YEAR_PATTERN = re.compile(r'Ü?Y\d{1,2}(?P<cat>[A-Z])(?P<written>\d{4})(?P<i>I)?Y(?P<real>\d{4})?')
-AGE_PATTERN = re.compile(r'Ü?A\d(?P<cat>[A-Z])(?P<written>\d{2,3})(?P<i>I)?A(?P<real>\d{2,3})?')
+ENTITY_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})(?:[A-Z0-9]+)?')
+YEAR_PATTERN = compile(r'Ü?Y\d{1,2}(?P<cat>[A-Z])(?P<written>\d{4})(?P<i>I)?Y(?P<real>\d{4})?')
+AGE_PATTERN = compile(r'Ü?A\d(?P<cat>[A-Z])(?P<written>\d{2,3})(?P<i>I)?A(?P<real>\d{2,3})?')
 nasab_tags = '|'.join(EntityTags.instance().get_nasab_tags())
-NASAB_TAGS_PATTERN = re.compile(r'Ü?(?P<entity>' + nasab_tags + r')(?P<length>\d{1,2})')
+NASAB_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + nasab_tags + r')(?P<length>\d{1,2})')
 
 # EIS1600 light mARkdown
-HEADING_OR_BIO_PATTERN = re.compile(r'# [|$]+')
-MIU_LIGHT_OR_EIS1600_PATTERN = re.compile(r'#|_ء_#')
+HEADING_OR_BIO_PATTERN = compile(r'# [|$]+')
+MIU_LIGHT_OR_EIS1600_PATTERN = compile(r'#|_ء_#')
 
 # Fix mARkdown files
-SPACES_CROWD_PATTERN = re.compile(r' +')
-NEWLINES_CROWD_PATTERN = re.compile(r'\n{3,}')
-SPACES_AFTER_NEWLINES_PATTERN = re.compile(r'\n +')
-POETRY_PATTERN = re.compile(
+SPACES_CROWD_PATTERN = compile(r' +')
+NEWLINES_CROWD_PATTERN = compile(r'\n{3,}')
+SPACES_AFTER_NEWLINES_PATTERN = compile(r'\n +')
+POETRY_PATTERN = compile(
         r'# (' + AR_STR_AND_TAGS + '(?: ' + AR_STR_AND_TAGS + ')* %~% ' + AR_STR_AND_TAGS + '(?: ' +
         AR_STR_AND_TAGS +
         r')*) ?'
 )
-BELONGS_TO_PREV_PARAGRAPH_PATTERN = re.compile(r'\n(.{1,10})\n')
-PAGE_TAG_ON_NEWLINE_PATTERN = re.compile(r'\n' + PAGE_TAG)
-PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN = re.compile(
+BELONGS_TO_PREV_PARAGRAPH_PATTERN = compile(r'\n(.{1,10})\n')
+PAGE_TAG_ON_NEWLINE_PATTERN = compile(r'\n' + PAGE_TAG)
+PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN = compile(
         '(' + AR_STR + ' ?)' + r'\n\n' + PAGE_TAG + r'\n\n' + '(' + AR_STR +
         ')'
 )
-NORMALIZE_BIO_CHR_MD_PATTERN = re.compile('# ([$@]((BIO|CHR)_[A-Z]+[$@])| RAW)')
-BIO_CHR_TO_NEWLINE_PATTERN = re.compile(TAG_AND_TEXT_SAME_LINE)
+NORMALIZE_BIO_CHR_MD_PATTERN = compile('# ([$@]((BIO|CHR)_[A-Z]+[$@])| RAW)')
+BIO_CHR_TO_NEWLINE_PATTERN = compile(TAG_AND_TEXT_SAME_LINE)
 
 # Fixed poetry old file path pattern
-FIXED_POETRY_OLD_PATH_PATTERN = re.compile(r'/Users/romanov/_OpenITI/_main_corpus/\w+/data/')
+FIXED_POETRY_OLD_PATH_PATTERN = compile(r'/Users/romanov/_OpenITI/_main_corpus/\w+/data/')
```

### Comparing `eis1600-0.9.2/eis1600/helper/miu_random_revisions.py` & `eis1600-0.9.3/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/helper/repo.py` & `eis1600-0.9.3/eis1600/helper/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/helper/yml_to_json.py` & `eis1600-0.9.3/eis1600/helper/yml_to_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import sys
+from sys import argv
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from pathlib import Path
 import jsonpickle
 from p_tqdm import p_uimap
 
 from eis1600.processing.preprocessing import get_yml
 from eis1600.helper.repo import MC_REPO, TRAINING_DATA_REPO
 
 
 def main():
     arg_parser = ArgumentParser(
-            prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+            prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to generate JSON from MIU YAMLHeaders.'''
     )
     arg_parser.add_argument('-D', '--debug', action='store_true')
     args = arg_parser.parse_args()
 
     debug = args.debug
     with open(TRAINING_DATA_REPO + 'gold_standard.txt', 'r', encoding='utf-8') as fh:
```

### Comparing `eis1600-0.9.2/eis1600/markdown/UIDs.py` & `eis1600-0.9.3/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.9.3/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from functools import partial
 
 from tqdm import tqdm
 from p_tqdm import p_uimap
 from pathlib import Path
 
-import sys
-import os
+from sys import argv, exit
+from os.path import isfile, splitext
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 from glob import glob
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, read_files_from_readme, write_to_readme, \
     update_texts_fixed_poetry_readme
 from eis1600.markdown.methods import convert_to_EIS1600TMP
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
-        if input_arg and os.path.isfile(input_arg):
-            filepath, fileext = os.path.splitext(input_arg)
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
             if fileext not in ['.mARkdown', '.inProgess', '.completed']:
                 parser.error('You need to input a mARkdown file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 def main():
     arg_parser = ArgumentParser(
-            prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+            prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to convert mARkdown file(s) to EIS1600TMP file(s).
 -----
 Give a single mARkdown file as input
 or 
 Give an input AND an output directory for batch processing.
 
 Run without input arg to batch process all mARkdown files in the EIS1600 directory which have not been processed yet.
@@ -79,15 +79,15 @@
         print(f'Convert mARkdown files from {input_dir}, save resulting EIS1600TMP files to {output_dir}')
 
         infiles = glob(input_dir + '*.mARkdown')
         if not infiles:
             print(
                     'The input directory does not contain any mARkdown files to process'
             )
-            sys.exit()
+            exit()
 
         # Check if output directory exists else create that directory
         Path(output_dir).mkdir(exist_ok=True, parents=True)
 
         if verbose:
             for infile in tqdm(infiles):
                 try:
@@ -110,15 +110,15 @@
         infiles = get_files_from_eis1600_dir(
                 input_dir, files_list, ['mARkdown', 'inProcress', 'completed'], 'EIS1600*'
         )
         if not infiles:
             print(
                     'There are no more mARkdown files to process'
             )
-            sys.exit()
+            exit()
 
         if verbose:
             for infile in tqdm(infiles):
                 try:
                     convert_to_EIS1600TMP(infile, None, verbose)
                 except Exception as e:
                     print(infile, e)
```

### Comparing `eis1600-0.9.2/eis1600/markdown/insert_uids.py` & `eis1600-0.9.3/eis1600/markdown/insert_uids.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from tqdm import tqdm
 from p_tqdm import p_uimap
 from pathlib import Path
 
-import sys
-import os
+from sys import argv, exit
+from os.path import isfile, splitext
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 from glob import glob
 from multiprocessing import Pool
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, write_to_readme, read_files_from_readme
 from eis1600.markdown.methods import insert_uids
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
-        if input_arg and os.path.isfile(input_arg):
-            filepath, fileext = os.path.splitext(input_arg)
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
             if fileext != '.EIS1600TMP':
                 parser.error('You need to input an EIS1600TMP file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 def main():
     arg_parser = ArgumentParser(
-            prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+            prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to insert UIDs in EIS1600TMP file(s) and thereby converting them to final EIS1600 
             file(s).
 -----
 Give a single EIS1600TMP file as input
 or 
 Give an input AND an output directory for batch processing.
 
@@ -77,15 +77,15 @@
         print(f'Insert UIDs into {input_dir}, save resulting EIS1600 files to {output_dir}')
 
         infiles = glob(input_dir + '/*.EIS1600TMP')
         if not infiles:
             print(
                     'The input directory does not contain any EIS1600TMP files to process'
                     )
-            sys.exit()
+            exit()
 
         # Check if output directory exists else create that directory
         Path(output_dir).mkdir(exist_ok=True, parents=True)
 
         params = [(infile, output_dir, verbose) for infile in infiles]
 
         with Pool() as p:
@@ -100,15 +100,15 @@
         print(f'Insert UIDs into files from the EIS1600 repo (only if there is not an EIS1600 file yet)')
         files_list = read_files_from_readme(input_dir, '# Texts converted into `.EIS1600TMP`\n')
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'EIS1600TMP', 'EIS1600')
         if not infiles:
             print(
                     'There are no more EIS1600TMP files to process'
                     )
-            sys.exit()
+            exit()
 
         # Insert UIDs in the selected files, runs in parallel
         if verbose:
             for infile in tqdm(infiles):
                 try:
                     insert_uids(infile, None, verbose)
                 except Exception as e:
```

### Comparing `eis1600-0.9.2/eis1600/markdown/methods.py` & `eis1600-0.9.3/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/markdown/update_uids.py` & `eis1600-0.9.3/eis1600/markdown/update_uids.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import sys
-import os
+from sys import argv, exit
+from os.path import isfile, splitext
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 
 from p_tqdm import p_uimap
 from tqdm import tqdm
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, write_to_readme, read_files_from_readme
 from eis1600.markdown.methods import update_uids
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
-        if input_arg and os.path.isfile(input_arg):
-            filepath, fileext = os.path.splitext(input_arg)
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
             if fileext != '.EIS1600':
                 parser.error('You need to input an EIS1600 file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 def main():
     arg_parser = ArgumentParser(
-            prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+            prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to insert UIDs in updated EIS1600 file(s).
 -----
 Give a single EIS1600 file as input
 or 
 Run without input arg to batch process all EIS1600 files in the EIS1600 directory which have not been processed yet.
 '''
     )
@@ -67,15 +67,15 @@
                 input_dir, '# Texts converted into `.EIS1600`\n', False
         )
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'EIS1600')
         if not infiles:
             print(
                     'There are no more files to update'
             )
-            sys.exit()
+            exit()
 
         if verbose:
             for infile in tqdm(infiles):
                 try:
                     update_uids(infile, verbose)
                 except Exception as e:
                     print(infile, e)
```

### Comparing `eis1600-0.9.2/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.9.3/eis1600/markdown/update_uids_old_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from os.path import split, splitext
-
-from eis1600.markdown.UIDs import UIDs
 from typing import Optional
-
-import sys
-import os
+from sys import argv, exit
+from os.path import isfile, split, splitext
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 from multiprocessing import Pool
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, write_to_readme, read_files_from_readme
 from eis1600.helper.markdown_patterns import BIO_CHR_TO_NEWLINE_PATTERN, HEADER_END_PATTERN, HEADING_OR_BIO_PATTERN, \
     MIU_LIGHT_OR_EIS1600_PATTERN, NEWLINES_CROWD_PATTERN, UID_PATTERN
+from eis1600.markdown.UIDs import UIDs
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
-        if input_arg and os.path.isfile(input_arg):
-            filepath, fileext = os.path.splitext(input_arg)
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
             if fileext != '.EIS1600':
                 parser.error('You need to input an EIS1600 file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
@@ -88,15 +85,15 @@
 
     with open(outfile, 'w', encoding='utf8') as outfile_h:
         outfile_h.write(final)
 
 
 def main():
     arg_parser = ArgumentParser(
-            prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+            prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to insert UIDs in updated EIS1600 file(s).
 -----
 Give a single EIS1600 file as input
 or 
 Use -e <EIS1600_repo> to batch process all EIS1600 files in the EIS1600 directory which have not been processed yet.
 '''
     )
@@ -130,22 +127,22 @@
             input_dir, '# Texts which need to be updated (old process)\n', False
             )
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'EIS1600')
         if not infiles:
             print(
                     'There are no more files to update'
             )
-            sys.exit()
+            exit()
 
         params = [(infile, verbose) for infile in infiles]
 
         with Pool() as p:
             p.starmap_async(xx_update_uids, params).get()
 
         write_to_readme(input_dir, infiles, '# Texts updated with missing UIDs\n')
     else:
         print(
                 'Pass in a <uri.EIS1600> file to process a single file or use the -e option for batch processing'
         )
-        sys.exit()
+        exit()
 
     print('Done')
```

### Comparing `eis1600-0.9.2/eis1600/miu/HeadingTracker.py` & `eis1600-0.9.3/eis1600/miu/HeadingTracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
-import copy
-import json
+from copy import deepcopy
 
 from typing import Dict, Optional
 
 
 class HeadingTracker:
     """A class to keep track of the super elements of a MIU.
 
@@ -38,15 +37,15 @@
     def get_curr_state(self) -> HeadingTracker:
         """Get current state of the tacker as deepcopy.
 
         Returns a deepcopy of the current state.
         :return HeadingTracker: Deepcopy of the current state of the tracker.
         """
 
-        return copy.deepcopy(self)
+        return deepcopy(self)
 
     def get_yamlfied(self) -> str:
         """Stringifies HeadingTracker in YAML format, only includes levels which are set.
 
         :return str: returns the HeadingTracker in YAML format as a string.
         """
```

### Comparing `eis1600-0.9.2/eis1600/miu/YAMLHandler.py` & `eis1600-0.9.3/eis1600/miu/YAMLHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
                 val_list = raw_val_list.strip('()').split('), (')
                 values = []
                 for v in val_list:
                     t = v.split(', ')
                     values.append((YAMLHandler.__parse_yml_val(t[0]), YAMLHandler.__parse_yml_val(t[1])))
             elif raw_val_list.startswith('[') or raw_val_list.startswith('{'):
                 # Nested lists
-                print(f'val: {val}')
                 values = literal_eval(val)
             else:
                 # List of other values
                 val_list = raw_val_list.split(', ')
                 values = [YAMLHandler.__parse_yml_val(v) for v in val_list]
             return values
         else:
```

### Comparing `eis1600-0.9.2/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.9.3/eis1600/miu/disassemble_into_miu_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-from functools import partial
-
-import sys
-import os
+from sys import argv, exit
+from os.path import isfile, splitext
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
+from functools import partial
 
 from p_tqdm import p_uimap
 from tqdm import tqdm
 
 from eis1600.helper.repo import get_path_to_other_repo, read_files_from_autoreport, get_files_from_eis1600_dir, \
-    write_to_readme
+    write_to_readme, TEXT_REPO
 from eis1600.miu.methods import disassemble_text
-from eis1600.helper.repo import TEXT_REPO
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
-        if input_arg and os.path.isfile(input_arg):
-            filepath, fileext = os.path.splitext(input_arg)
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
             if fileext != '.EIS1600':
                 parser.error('You need to input an EIS1600 file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 def main():
     arg_parser = ArgumentParser(
-            prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+            prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to disassemble EIS1600 file(s) into MIU file(s).
 -----
 Give a single EIS1600 file as input
 or 
 Run without input arg to batch process all double-checked EIS1600 files from the AUTOREPORT.
 '''
     )
@@ -59,15 +57,15 @@
 
         print(f'Disassemble double-checked EIS1600 files from the AUTOREPORT')
         files_list = read_files_from_autoreport(input_dir)
 
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'EIS1600')
         if not infiles:
             print('There are no EIS1600 files to process')
-            sys.exit()
+            exit()
 
         if verbose:
             for infile in tqdm(infiles):
                 try:
                     disassemble_text(infile, out_path, verbose)
                 except Exception as e:
                     print(infile, e)
```

### Comparing `eis1600-0.9.2/eis1600/miu/methods.py` & `eis1600-0.9.3/eis1600/miu/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from glob import glob
-from logging import Logger
 from os.path import splitext, split, exists
 from typing import List, Optional
 from pathlib import Path
 
-from eis1600.onomastics.methods import nasab_annotate_miu
-
 from eis1600.dates.methods import date_annotate_miu_text
-from eis1600.miu.HeadingTracker import HeadingTracker
-from eis1600.processing.preprocessing import get_yml_and_miu_df
-from eis1600.processing.postprocessing import write_updated_miu_to_file
-from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text
-from eis1600.miu.yml_handling import create_yml_header, extract_yml_header_and_text
 from eis1600.helper.markdown_patterns import CATEGORY_PATTERN, HEADER_END_PATTERN, HEADING_PATTERN, MIU_TAG_PATTERN, \
     MIU_UID_PATTERN, PAGE_TAG_PATTERN
+from eis1600.miu.HeadingTracker import HeadingTracker
+from eis1600.miu.yml_handling import create_yml_header, extract_yml_header_and_text
+from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text
+from eis1600.onomastics.methods import nasab_annotate_miu
+from eis1600.processing.postprocessing import write_updated_miu_to_file
+from eis1600.processing.preprocessing import get_yml_and_miu_df
 
 
 def disassemble_text(infile: str, out_path: str, verbose: Optional[bool] = None) -> None:
     """Disassemble text into MIU files.
 
     Retrieve MIU files by disassembling the text based on the EIS1600 mARkdown.
     :param str infile: Path to the file which is to be disassembled.
@@ -151,15 +149,15 @@
 
     for i, miu_id in enumerate(ids):
         mius.extend(glob(file_path + 'MIUs/' + uri + '.' + miu_id + '.EIS1600'))
 
     return mius
 
 
-def annotate_miu_file(path: str, logger: Logger = None, tsv_path=None, output_path=None, force_annotation=False):
+def annotate_miu_file(path: str, tsv_path=None, output_path=None, force_annotation=False):
     if output_path is None:
         output_path = path
     if tsv_path is None:
         tsv_path = path.replace('.EIS1600', '.tsv')
 
     # if the file is already annotated, do nothing
     if exists(tsv_path) and not force_annotation:
@@ -176,15 +174,15 @@
         df['NER_TAGS'] = camel2md_as_list(df['NER_LABELS'].tolist())
 
         # 4. annotate dates
         df['DATE_TAGS'] = date_annotate_miu_text(df[['TOKENS']], yml_handler)
 
         # 5. annotate onomastic information
         # TODO Needs to be run after the NASAB END tag was inserted
-        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, path, logger)
+        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, path)
 
         # TODO 6. disambiguation of toponyms (same toponym, different places) --> replace ambigious toponyms flag
         # TODO 7. toponym categorization
         # TODO 8. assign roles for persons
         # TODO 9. get frequencies of unidentified entities (toponyms, nisbas)
 
         # 6. save csv file
```

### Comparing `eis1600-0.9.2/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.9.3/eis1600/miu/reassemble_from_miu_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import sys
-import os
+from sys import argv, exit
+from os.path import isfile, splitext
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 from multiprocessing import Pool
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, get_path_to_other_repo, read_files_from_readme
 from eis1600.miu.methods import reassemble_text
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
-        if input_arg and os.path.isfile(input_arg):
-            filepath, fileext = os.path.splitext(input_arg)
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
             if fileext != '.IDs':
                 parser.error('You need to input an IDs file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 def main():
     arg_parser = ArgumentParser(
-        prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+        prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
         description='''Script to reassemble EIS1600 file(s) from MIU file(s).
 -----
 Give a single IDs file as input
 or 
 Use -e <EIS1600_repo> to batch process all files in the EIS1600 directory.
 '''
         )
@@ -55,20 +55,20 @@
         out_path = get_path_to_other_repo(input_dir, 'TEXT')
 
         print(f'Reassemble EIS1600 files from the EIS1600 repo')
         files_list = read_files_from_readme(input_dir, '# Texts disassembled into MIU files\n')
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'IDs')
         if not infiles:
             print('There are no IDs files to process')
-            sys.exit()
+            exit()
 
         params = [(infile, out_path, verbose) for infile in infiles]
 
         with Pool() as p:
             p.starmap_async(reassemble_text, params).get()
     else:
         print(
                 'Pass in a <uri.IDs> file to process a single file or use the -e option for batch processing'
         )
-        sys.exit()
+        exit()
 
     print('Done')
```

### Comparing `eis1600-0.9.2/eis1600/miu/yml_handling.py` & `eis1600-0.9.3/eis1600/miu/yml_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 from itertools import combinations
+from os import makedirs
+from os.path import dirname, split, splitext
 from typing import Dict, List, Optional, Set, TextIO, Tuple, Union
 
 from eis1600.gazetteers.Toponyms import Toponyms
-from eis1600.helper.markdown_methods import get_yrs_tag_value
 from eis1600.helper.EntityTags import EntityTags
+from eis1600.helper.logging import setup_logger
+from eis1600.helper.markdown_methods import get_yrs_tag_value
+from eis1600.helper.markdown_patterns import ENTITY_TAGS_PATTERN, MIU_HEADER_PATTERN, NEWLINES_CROWD_PATTERN
+from eis1600.helper.repo import GAZETTEERS_REPO
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.miu.YAMLHandler import YAMLHandler
-from eis1600.helper.markdown_patterns import ENTITY_TAGS_PATTERN, MIU_HEADER_PATTERN, NEWLINES_CROWD_PATTERN
+
+
+__log_filename_nasab = GAZETTEERS_REPO + 'logs/nasab_known.log'
+makedirs(dirname(__log_filename_nasab), exist_ok=True)
+LOGGER_NASAB_KNOWN = setup_logger('nasab_known', __log_filename_nasab)
+LOGGER_TOPONYMS_UNKNOWN = setup_logger('toponyms_unknown', GAZETTEERS_REPO + 'logs/toponyms_unknown.log')
 
 
 def create_yml_header(category: str, headings: Optional[HeadingTracker] = None) -> str:
     """Creates a YAML header for the current MIU file and returns it as yamlfied string.
 
     :param str category: Category of the entry.
     :param Type[HeadingsTracker] headings: HeadingTracker with the super elements of the current MIU, optional.
@@ -26,16 +36,15 @@
 
 def extract_yml_header_and_text(miu_file_object: TextIO, is_header: Optional[bool] = False) -> (str, str):
     """ Returns the YAML header and the text as a tuple from MIU file object.
 
     Splits the MIU file into a tuple of YAML header and text.
     :param TextIO miu_file_object: File object of the MIU file from which to extract YAML header and text.
     :param bool is_header: Indicates if the current MIU is the YAML header of the whole work and if so skips
-    removing
-    blank lines, defaults to False.
+    removing blank lines, defaults to False.
     :return (str, str): Tuple of the extracted YAML header and text.
     """
     text = ''
     miu_yml_header = ''
     for line in iter(miu_file_object):
         if MIU_HEADER_PATTERN.match(line):
             # Omit the #MIU#Header# line as it is only needed inside the MIU.EIS1600 file, but not in YMLDATA.yml
@@ -87,20 +96,24 @@
             entities_dict[cat][tag] = [entity]
         elif isinstance(entity, list):
             entities_dict[cat] = entity
         else:
             entities_dict[cat] = [entity]
 
 
-def add_annotated_entities_to_yml(text_with_tags: str, yml_handler: YAMLHandler, filename: str) -> None:
+def add_annotated_entities_to_yml(
+        text_with_tags: str,
+        yml_handler: YAMLHandler,
+        file_path: str,
+) -> None:
     """Populates YAMLHeader with annotated entities.
 
     :param str text_with_tags: Text with inserted tags of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
-    :param str filename: Filename of the current MIU (used in error msg).
+    :param str file_path: Filename of the current MIU (used in error msg).
     """
     # We do not need to differentiate between automated and manual tags
     text_with_tags = text_with_tags.replace('Ü', '')
     tg = Toponyms.instance()
     entity_tags_df = EntityTags.instance().get_entity_tags_df()
     entities_dict = {}
     nas_dict = {}
@@ -116,31 +129,37 @@
 
         cat = entity_tags_df.loc[entity_tags_df['TAG'].str.fullmatch(tag), 'CATEGORY'].iloc[0]
         if cat == 'DATE' or cat == 'AGE':
             try:
                 val, e_cat = get_yrs_tag_value(m.group(0))
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val, 'cat': e_cat})
             except ValueError:
-                print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {filename}')
+                print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {file_path}')
                 return
         elif cat == 'TOPONYM':
             place, uri, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
-            if len(list_of_uris) > 1:
-                yml_handler.set_ambigious_toponyms()
-            toponyms_set.update(list_of_uris)
-            provinces_set.update(list_of_provinces)
             add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uri})
+            if len(list_of_uris) == 0:
+                path, uri = split(file_path)
+                uri, ext = splitext(uri)
+                LOGGER_TOPONYMS_UNKNOWN.info(f'{uri},{entity}')
+            else:
+                toponyms_set.update(list_of_uris)
+                provinces_set.update(list_of_provinces)
+                if len(list_of_uris) > 1:
+                    yml_handler.set_ambigious_toponyms()
         elif cat == 'ONOMASTIC':
             if tag.startswith('SHR') and entity.startswith('ب'):
                 entity = entity[1:]
                 add_to_entities_dict(entities_dict, cat, entity, tag)
             elif tag.startswith('NAS'):
                 nas_dict['nas_' + str(nas_counter)] = entity
                 nas_counter += 1
             add_to_entities_dict(entities_dict, cat, entity, tag)
+            LOGGER_NASAB_KNOWN.info(f'{tag},{entity}')
         else:
             add_to_entities_dict(entities_dict, cat, entity, tag)
 
         m = ENTITY_TAGS_PATTERN.search(text_with_tags, m.end())
 
     if nas_dict != {}:
         if 'onomastics' in entities_dict.keys():
```

### Comparing `eis1600-0.9.2/eis1600/nlp/cameltools.py` & `eis1600-0.9.3/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.9.3/eis1600/nlp/ner_annotate_mius.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-import sys
-import os
+from sys import argv, exit
+from os.path import isfile, splitext
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 from functools import partial
 from pathlib import Path
 
-from eis1600.helper.logging import setup_logger
 from p_tqdm import p_uimap
 from tqdm import tqdm
 
-from eis1600.helper.repo import get_files_from_eis1600_dir, read_files_from_readme
+from eis1600.helper.repo import get_files_from_eis1600_dir, read_files_from_readme, MIU_REPO
 from eis1600.miu.methods import annotate_miu_file, get_mius
-from eis1600.helper.repo import MIU_REPO
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
-        if input_arg and os.path.isfile(input_arg):
-            filepath, fileext = os.path.splitext(input_arg)
+        if input_arg and isfile(input_arg):
+            filepath, fileext = splitext(input_arg)
             if fileext != '.IDs' and fileext != '.EIS1600':
                 parser.error('You need to input an IDs file or a single MIU file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 def main():
     arg_parser = ArgumentParser(
-        prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+        prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
         description='''Script to NER annotate MIU file(s).
 -----
 Give an IDs file or a single MIU file as input
 otherwise 
 all files in the MIU directory are batch processed.
 '''
         )
@@ -46,15 +44,15 @@
     args = arg_parser.parse_args()
 
     verbose = args.verbose
     force = args.force
 
     if args.input:
         infile = './' + args.input
-        filepath, fileext = os.path.splitext(infile)
+        filepath, fileext = splitext(infile)
         if fileext == '.IDs':
             mius = get_mius(infile)[1:]  # First element is path to the OPENITI HEADER
             print(f'NER annotate MIUs of {infile}')
             if args.parallel:
                 res = []
                 res += p_uimap(partial(annotate_miu_file), mius)
             else:
@@ -68,33 +66,32 @@
             annotate_miu_file(infile, force_annotation=force)
     else:
         input_dir = MIU_REPO
 
         if not Path(input_dir).exists():
             print('Your working directory seems to be wrong, make sure it is set to the parent dir of '
                   '`EIS1600_MIUs/`.')
-            sys.exit()
+            exit()
 
         print(f'NER annotate MIU files')
         files_list = read_files_from_readme(input_dir, '# Texts disassembled into MIU files\n')
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'IDs')
         if not infiles:
             print('There are no IDs files to process')
-            sys.exit()
+            exit()
 
-        logger_nasab = setup_logger('nasab_unknown', 'logs/nasab_unknown.log')
         for infile in infiles:
             if verbose:
                 print(f'NER annotate MIUs of {infile}')
 
             mius = get_mius(infile)[1:]  # First element is path to the OPENITI HEADER
             if args.parallel:
                 res = []
-                res += p_uimap(partial(annotate_miu_file, logger_nasab), mius)
+                res += p_uimap(partial(annotate_miu_file), mius)
             else:
                 for miu in tqdm(mius):
                     try:
-                        annotate_miu_file(miu, logger_nasab)
+                        annotate_miu_file(miu)
                     except Exception as e:
                         print(miu, e)
 
     print('Done')
```

### Comparing `eis1600-0.9.2/eis1600/nlp/utils.py` & `eis1600-0.9.3/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/onomastics/annotation.py` & `eis1600-0.9.3/eis1600/onomastics/annotation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from glob import glob
 from pathlib import Path
 
 import sys
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from functools import partial
 
-from eis1600.helper.logging import setup_logger
 from p_tqdm import p_uimap
 
-from eis1600.onomastics.methods import nasab_annotation
 from eis1600.helper.repo import TRAINING_DATA_REPO
+from eis1600.onomastics.methods import nasab_annotation
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
@@ -29,17 +28,16 @@
             files_txt = fh.read().splitlines()
 
         infiles = [TRAINING_DATA_REPO + 'gold_standard/' + file for file in files_txt if Path(
                 TRAINING_DATA_REPO + 'gold_standard/' + file).exists()]
     else:
         infiles = glob(TRAINING_DATA_REPO + 'training_data_nasab_ML2/*.EIS1600')
 
-    logger_nasab = setup_logger('nasab_unknown', TRAINING_DATA_REPO + 'logs/nasab_unknown.log')
     if debug:
         for file in infiles:
             print(file)
-            nasab_annotation(file, logger_nasab, test)
+            nasab_annotation(file, test)
     else:
         res = []
-        res += p_uimap(partial(nasab_annotation, logger_nasab=logger_nasab, test=test), infiles)
+        res += p_uimap(partial(nasab_annotation, test=test), infiles)
 
     print('Done')
```

### Comparing `eis1600-0.9.2/eis1600/onomastics/methods.py` & `eis1600-0.9.3/eis1600/onomastics/methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-from logging import Logger
+from os import makedirs
+from os.path import dirname
 from pathlib import Path
 from typing import Optional
-
-import pandas as pd
 from numpy import nan
 from pandas import Series
+from pandas import DataFrame, notna
 
 from eis1600.gazetteers.Onomastics import Onomastics
 from eis1600.gazetteers.Toponyms import Toponyms
+from eis1600.helper.logging import setup_logger
+from eis1600.helper.repo import GAZETTEERS_REPO
 from eis1600.miu.YAMLHandler import YAMLHandler
 from eis1600.onomastics.re_pattern import ABI, ABU, BN_BNT, CRF_PATTERN, IBN_IBNA, SHR_PATTERN, SPELLING, UMM
-from eis1600.processing.postprocessing import reconstruct_miu_text_with_tags, write_updated_miu_to_file
+from eis1600.processing.postprocessing import write_updated_miu_to_file
 from eis1600.processing.preprocessing import get_tokens_and_tags, get_yml_and_miu_df
 
+__log_filename = GAZETTEERS_REPO + 'logs/nasab_unknown.log'
+makedirs(dirname(__log_filename), exist_ok=True)
+LOGGER_NASAB_UNKNOWN = setup_logger('nasab_unknown', __log_filename)
+
 
 def get_nas(text: str) -> str:
     """Add the list of forefathers to the YAMLHeader and return nasab part with tagged NAS and manipulated so it is
     ignored for further onomastic analysis (all elements which refere to ancestors are filtered here).
 
     :param str text: nasab str.
     :return str: nasab str with tagged and manipulated nas elements.
@@ -66,18 +72,17 @@
                           text_mnpld[end + 1 + last_ancestor:].replace('_', ' ')
 
         return text_w_tags
 
     return text_mnpld
 
 
-def tag_nasab(text: str, logger_nasab: Logger) -> str:
+def tag_nasab(text: str) -> str:
     """Annotate the nasab part of the MIU.
 
-    :param logger_nasab:
     :param str text: nasab part of the MIU as one single string with tagged and filtered NAS elements (NAS is
     connected with '_' and therefore does not match with the gazetteer).
     :return str: the nasab part pf the MIU which contains also the tags in front of the recognized elements,
     '_' are removed.
     """
     og = Onomastics.instance()
     tg = Toponyms.instance()
@@ -113,35 +118,35 @@
         else:
             text_mnpld = text_mnpld[:pos] + tag + text_mnpld[pos:]
 
         end += len(tag)
 
         m = og.get_ngrams_regex().search(text_mnpld, end)
 
-    if logger_nasab:
-        # Log unidentified tokens as uni- and bi-grams
-        filtered = text_mnpld
-        m = og.get_ngrams_regex().search(filtered)
-        while m:
-            filtered = filtered[:m.start()] + m.group(1) + m.group(2).replace(' ', '_') + filtered[m.end():]
-            m = og.get_ngrams_regex().search(filtered, m.end())
-        tokens = [token for token in filtered.split() if not token.startswith('Ü')]
-        unknown_uni = [t for t in tokens if not ('_' in t or t in og.total() + tg.total())]
-        prev = None
-        unknown_bi = []
-        for t in tokens:
-            if not prev and not ('_' in t or t in og.total() + tg.total() + ['بن', 'بنت']):
+    # Log unidentified tokens as uni- and bi-grams
+    filtered = text_mnpld
+    m = og.get_ngrams_regex().search(filtered)
+    while m:
+        filtered = filtered[:m.start()] + m.group(1) + m.group(2).replace(' ', '_') + filtered[m.end():]
+        m = og.get_ngrams_regex().search(filtered, m.end())
+    tokens = [token for token in filtered.split() if not token.startswith('Ü')]
+    unknown_uni = [t for t in tokens if not ('_' in t or t in og.total() + tg.total())]
+    prev = None
+    unknown_bi = []
+    for t in tokens:
+        if not prev and not ('_' in t or t in og.total() + tg.total() + ['بن', 'بنت']):
+            prev = t
+        else:
+            if not ('_' in t or t in og.total() + tg.total() + ['بن', 'بنت']):
+                unknown_bi.append(prev + ' ' + t)
                 prev = t
             else:
-                if not ('_' in t or t in og.total() + tg.total() + ['بن', 'بنت']):
-                    unknown_bi.append(prev + ' ' + t)
-                    prev = t
-                else:
-                    prev = None
-        logger_nasab.info('\n'.join(unknown_uni + unknown_bi))
+                prev = None
+    if unknown_uni or unknown_bi:
+        LOGGER_NASAB_UNKNOWN.info('\n'.join(unknown_uni + unknown_bi))
 
     return text_mnpld.replace('_', ' ')
 
 
 def tag_spelling(text: str) -> str:
     """Tags spelling information which is stated in the nasab part of the MIU text.
 
@@ -158,23 +163,23 @@
 
         m = SPELLING.search(text_updated, m.end() + len(tag))
 
     return text_updated
 
 
 def nasab_annotate_miu(
-        df: pd.DataFrame, yml_handler: YAMLHandler, file: str, logger_nasab: Optional[Logger],
+        df: DataFrame, yml_handler: YAMLHandler,
+        file: str,
         test: Optional[bool] = False
 ) -> Series:
     """Onomastic analysis of the nasab part of the MIU.
 
     :param DataFrame df: DataFrame of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :param Path file: the MIU which was opened.
-    :param Logger logger_nasab: logs unrecognized uni- and bi-grams to a log file, optional.
     :param bool test: run on test data set, optional.
     :return Series: a series of the same length as the df containing the nasab tags corresponding to the tokens.
     """
     if not yml_handler.is_bio():
         return Series([nan] * len(df))
 
     s_notna = df['TAGS_LISTS'].loc[df['TAGS_LISTS'].notna()].apply(lambda tag_list: ','.join(tag_list))
@@ -201,49 +206,49 @@
     tagged_spelling = tag_spelling(text)
     ar_tokens, tags = get_tokens_and_tags(tagged_spelling)
     df.loc[nasab_idx, 'NASAB_TAGS'] = tags
 
     count = 0
     spl_idcs = []
     for row in df.loc[nasab_idx].itertuples():
-        if pd.notna(row[4]):
+        if notna(row[4]):
             count = int(row[4][-1])
         if count > 0:
             count -= 1
             spl_idcs.append(row[0])
 
     nasab_idx = df.loc[nasab_idx.difference(spl_idcs)].index
     text = ' '.join(df['TOKENS'].loc[nasab_idx])
 
     text_w_mnpld_nas = get_nas(text)
-    tagged_onomastics = tag_nasab(text_w_mnpld_nas, logger_nasab)
+    tagged_onomastics = tag_nasab(text_w_mnpld_nas)
     ar_tokens, tags = get_tokens_and_tags(tagged_onomastics)
     df.loc[nasab_idx, 'NASAB_TAGS'] = tags
 
     if idx != len(df):
         # TODO make NASAB stay on same line
         df.loc[idx - 1, 'NASAB_END'] = 'NASAB'
 
     return df['NASAB_TAGS'].to_list()
 
 
-def nasab_annotation(file: str, logger_nasab: Logger, test: bool):
+def nasab_annotation(file: str, test: bool):
     """Only used for onomastic_annotation cmdline script."""
     with open(file, 'r', encoding='utf-8') as miu_file_object:
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
     if test:
         # Only used if run on training_data batch because this information is missing there
         if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
             df['NASAB_TAGS'] = Series([nan] * len(df))
         else:
             yml_handler.set_category('$')
-            df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab, test)
+            df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, test)
     else:
         # Run on new data batch
-        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab, test)
+        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, test)
     yml_handler.unset_reviewed()
 
     if test:
         output_path = str(file).replace('gold_standard', 'gold_standard_nasab')
     else:
         output_path = str(file)
```

### Comparing `eis1600-0.9.2/eis1600/onomastics/re_pattern.py` & `eis1600-0.9.3/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/processing/postprocessing.py` & `eis1600-0.9.3/eis1600/processing/postprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,112 @@
 from typing import Iterator, List, TextIO, Tuple, Union
 
-import pandas as pd
+from os import path
+from pandas import DataFrame, notna
 from camel_tools.utils.charsets import UNICODE_PUNCT_CHARSET
 
 from eis1600.helper.markdown_patterns import ENTITY_TAGS_PATTERN
 from eis1600.miu.YAMLHandler import YAMLHandler
 from eis1600.miu.yml_handling import add_annotated_entities_to_yml
 
 
 def get_text_with_annotation_only(
-        text_and_tags: Union[Iterator[Tuple[Union[str, None], str, Union[List[str], None]]], pd.DataFrame]
+        text_and_tags: Union[Iterator[Tuple[Union[str, None], str, Union[List[str], None]]], DataFrame]
 ) -> str:
     """Returns the MIU text only with annotation tags, not page tags and section tags.
 
     Returns the MIU text only with annotation tags contained in the list of tags. Tags are inserted BEFORE the token.
     Section headers and other tags - like page tags - are ignored.
     :param Iterator[Tuple[Union[str, None], str, Union[List[str], None]]] text_and_tags: zip object containing three
     sparse columns: sections, tokens, lists of tags.
     :return str: The MIU text with annotation only.
     """
-    if type(text_and_tags) is pd.DataFrame:
+    if type(text_and_tags) is DataFrame:
         text_and_tags_iter = text_and_tags.itertuples(index=False)
     else:
         text_and_tags_iter = text_and_tags.__iter__()
     next(text_and_tags_iter)
     text_with_annotation_only = ''
     for section, token, tags in text_and_tags_iter:
         if isinstance(tags, list):
             entity_tags = [tag for tag in tags if ENTITY_TAGS_PATTERN.fullmatch(tag)]
             text_with_annotation_only += ' ' + ' '.join(entity_tags)
-        if pd.notna(token):
+        if notna(token):
             text_with_annotation_only += ' ' + token
 
     return text_with_annotation_only
 
 
 def reconstruct_miu_text_with_tags(
-        text_and_tags: Union[Iterator[Tuple[Union[str, None], str, Union[List[str], None]]], pd.DataFrame]
+        text_and_tags: Union[Iterator[Tuple[Union[str, None], str, Union[List[str], None]]], DataFrame]
 ) -> str:
     """Reconstruct the MIU text from a zip object containing three columns: sections, tokens, lists of tags.
 
     Reconstructs the MIU text with the tags contained in the list of tags. Tags are inserted BEFORE the token.
     Section headers are inserted after an empty line ('\n\n'), followed by the text on the next line.
     :param Iterator[Tuple[Union[str, None], str, Union[List[str], None]]] text_and_tags: zip object containing three
     sparse columns: sections, tokens, lists of tags.
     :return str: The reconstructed MIU text containing all the tags.
     """
-    if type(text_and_tags) is pd.DataFrame:
+    if type(text_and_tags) is DataFrame:
         text_and_tags_iter = text_and_tags.itertuples(index=False)
     else:
         text_and_tags_iter = text_and_tags.__iter__()
     heading, _, _ = next(text_and_tags_iter)
     reconstructed_text = heading
     # TODO NASAB tag after token
     for section, token, tags in text_and_tags_iter:
-        if pd.notna(section):
+        if notna(section):
             reconstructed_text += '\n\n' + section + '\n_ء_'
         if isinstance(tags, list):
             reconstructed_text += ' ' + ' '.join(tags)
-        if pd.notna(token):
+        if notna(token):
             if token in UNICODE_PUNCT_CHARSET:
                 reconstructed_text += token
             else:
                 reconstructed_text += ' ' + token
 
     reconstructed_text += '\n\n'
     reconstructed_text = reconstructed_text.replace(' NEWLINE ', '\n_ء_ ')
     reconstructed_text = reconstructed_text.replace('HEMISTICH', '%~%')
     return reconstructed_text
 
 
 def merge_tagslists(lst1, lst2):
     if isinstance(lst1, list):
-        if pd.notna(lst2):
+        if notna(lst2):
             lst1.append(lst2)
     else:
-        if pd.notna(lst2):
+        if notna(lst2):
             lst1 = [lst2]
     return lst1
 
 
-def write_updated_miu_to_file(miu_file_object: TextIO, yml_handler: YAMLHandler, df: pd.DataFrame) -> None:
+def write_updated_miu_to_file(
+        miu_file_object: TextIO,
+        yml_handler: YAMLHandler,
+        df: DataFrame,
+) -> None:
     """Write MIU file with annotations and populated YAML header.
 
     :param TextIO miu_file_object: Path to the MIU file to write
     :param YAMLHandler yml_handler: The YAMLHandler of the MIU.
-    :param pd.DataFrame df: df containing the columns ['SECTIONS', 'TOKENS', 'TAGS_LISTS'] and optional 'ÜTAGS_LISTS'.
+    :param DataFrame df: df containing the columns ['SECTIONS', 'TOKENS', 'TAGS_LISTS'] and optional 'ÜTAGS_LISTS'.
     :return None:
     """
     if not yml_handler.is_reviewed():
         columns_of_automated_tags = ['NER_TAGS', 'DATE_TAGS', 'NASAB_TAGS']
         df['ÜTAGS'] = df['TAGS_LISTS']
         for col in columns_of_automated_tags:
             if col in df.columns:
                 df['ÜTAGS'] = df.apply(lambda x: merge_tagslists(x['ÜTAGS'], x[col]), axis=1)
         df_subset = df[['SECTIONS', 'TOKENS', 'ÜTAGS']]
     else:
         df_subset = df[['SECTIONS', 'TOKENS', 'TAGS_LISTS']]
 
     text_with_tags = get_text_with_annotation_only(df_subset)
-    add_annotated_entities_to_yml(text_with_tags, yml_handler, miu_file_object.name)
+    add_annotated_entities_to_yml(text_with_tags, yml_handler, path.realpath(miu_file_object.name))
     updated_text = reconstruct_miu_text_with_tags(df_subset)
 
     miu_file_object.seek(0)
     miu_file_object.write(str(yml_handler) + updated_text)
     miu_file_object.truncate()
```

### Comparing `eis1600-0.9.2/eis1600/processing/preprocessing.py` & `eis1600-0.9.3/eis1600/processing/preprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from eis1600.miu.YAMLHandler import YAMLHandler
 
 from eis1600.miu.yml_handling import extract_yml_header_and_text
 from typing import Iterator, List, TextIO, Tuple, Union
 
-import pandas as pd
+from pandas import DataFrame, options
 
 from camel_tools.tokenizers.word import simple_word_tokenize
 from eis1600.helper.markdown_patterns import MIU_TAG_PATTERN, SECTION_PATTERN, SECTION_SPLITTER_PATTERN, TAG_PATTERN
 
 
-pd.options.mode.chained_assignment = None
+options.mode.chained_assignment = None
 
 
 def get_tokens_and_tags(tagged_text: str) -> Tuple[List[Union[str, None]], List[Union[str, None]]]:
     """Splits the annotated text into two lists of the same length, one containing the tokens, the other one the tags
 
     :param str tagged_text: the annotated text as a single str.
     :return List[str], List[str]: two lists, first contains the arabic tokens, the other one the tags.
@@ -84,25 +84,25 @@
                 tags.append(tag)
 
         paragraph = next(text_iter, None)
 
     return zip(sections, ar_tokens, tags)
 
 
-def get_yml_and_miu_df(miu_file_object: TextIO) -> Tuple[YAMLHandler, pd.DataFrame]:
+def get_yml_and_miu_df(miu_file_object: TextIO) -> Tuple[YAMLHandler, DataFrame]:
     """Returns YAMLHandler instance and MIU as a DataFrame containing the columns 'SECTIONS', 'TOKENS', 'TAGS_LISTS'.
 
     :param TextIO miu_file_object: File object of the MIU file.
     :return Tuple[YAMLHandler, DataFrame]: YAMLHandler and DataFrame containing the columns 'SECTIONS', 'TOKENS',
     'TAGS_LISTS'.
     """
     yml_str, text = extract_yml_header_and_text(miu_file_object, False)
     yml_handler = YAMLHandler().from_yml_str(yml_str)
     zipped = tokenize_miu_text(text)
-    df = pd.DataFrame(zipped, columns=['SECTIONS', 'TOKENS', 'TAGS_LISTS'])
+    df = DataFrame(zipped, columns=['SECTIONS', 'TOKENS', 'TAGS_LISTS'])
 
     df.mask(df == '', inplace=True)
 
     return yml_handler, df
 
 
 def get_yml(path: str) -> Tuple[str, YAMLHandler]:
```

### Comparing `eis1600-0.9.2/eis1600/stats/methods.py` & `eis1600-0.9.3/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/stats/miu_stats.py` & `eis1600-0.9.3/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/toponyms/annotation.py` & `eis1600-0.9.3/eis1600/toponyms/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Annotate hajja -> Mekka
 # Annotate jāwara -> Medina
 # Tag category of toponyms
 from glob import glob
 from pathlib import Path
 
-import sys
+from sys import argv
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from functools import partial
 
 from p_tqdm import p_uimap
 
 from eis1600.helper.repo import TRAINING_DATA_REPO
 from eis1600.toponyms.methods import toponym_category_annotation
 
 
 def main():
     arg_parser = ArgumentParser(
-            prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
+            prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
     arg_parser.add_argument('-D', '--debug', action='store_true')
     arg_parser.add_argument('-T', '--test', action='store_true')
 
     args = arg_parser.parse_args()
     debug = args.debug
```

### Comparing `eis1600-0.9.2/eis1600/toponyms/methods.py` & `eis1600-0.9.3/eis1600/toponyms/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/eis1600/toponyms/toponym_categories.py` & `eis1600-0.9.3/eis1600/toponyms/toponym_categories.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import re
+from re import compile
 
 from openiti.helper.ara import denormalize
 
 from eis1600.helper.ar_normalization import normalize_dict
 
 
 TOPONYM_CATEGORIES = {
         'ولد': 'B', 'مولد': 'B',
         'مات': 'D', 'موت': 'D', 'توفي': 'D', 'وفاة': 'D',
         'حج': 'P',
-        'سمع': 'K', 'قرا': 'K', 'اجاز': 'K',
-        'استقر': 'O', 'انفصل': 'O', 'ولي': 'O', 'قاضي': 'O',
+        'سمع': 'K', 'روى': 'K', 'روا': 'K', 'قرا': 'K', 'اجاز': 'K',
+        'استقر': 'O', 'انفصل': 'O', 'ولي': 'O', 'قاضي': 'O', 'أعمال': 'O',
         'لقي': 'M',
-        'سكن': 'L', 'نزل': 'L', 'نريل': 'L', 'من اهل': 'L', 'استوطن': 'L'
+        'سكن': 'L', 'نزل': 'L', 'نزيل': 'L', 'من اهل': 'L', 'استوطن': 'L', 'كان من': 'L'
 }
 TOPONYM_CATEGORIES_NOR = normalize_dict(TOPONYM_CATEGORIES)
 
 AR_TOPONYM_CATEGORIES = '|'.join([denormalize(key) for key in TOPONYM_CATEGORIES.keys()])
-TOPONYM_CATEGORY_PATTERN = re.compile(r'\s[وف]?(?P<topo_category>' + AR_TOPONYM_CATEGORIES + r')')
+TOPONYM_CATEGORY_PATTERN = compile(r'\s[وف]?(?P<topo_category>' + AR_TOPONYM_CATEGORIES + r')')
```

### Comparing `eis1600-0.9.2/eis1600.egg-info/PKG-INFO` & `eis1600-0.9.3/eis1600.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.2
+Version: 0.9.3
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.2/eis1600.egg-info/SOURCES.txt` & `eis1600-0.9.3/eis1600.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 eis1600/dates/date_patterns.py
 eis1600/dates/methods.py
 eis1600/gazetteers/Onomastics.py
 eis1600/gazetteers/Toponyms.py
 eis1600/gazetteers/__init__.py
 eis1600/gazetteers/data/__init__.py
 eis1600/gazetteers/data/onomastic_gazetteer.csv
-eis1600/gazetteers/data/regions.csv
-eis1600/gazetteers/data/regions_gazetteer.csv
 eis1600/gazetteers/data/spelling_gazetteer.csv
-eis1600/gazetteers/data/toponyms.csv
+eis1600/gazetteers/data/toponyms_gazetteer.csv
 eis1600/helper/EntityTags.py
 eis1600/helper/Singleton.py
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
 eis1600/helper/fix_miu_annotation.py
 eis1600/helper/logging.py
 eis1600/helper/markdown_methods.py
```

### Comparing `eis1600-0.9.2/eis1600.egg-info/entry_points.txt` & `eis1600-0.9.3/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.2/setup.py` & `eis1600-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.9.2',
+      version='0.9.3',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```

