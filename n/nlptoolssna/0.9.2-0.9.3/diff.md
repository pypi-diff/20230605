# Comparing `tmp/nlptoolssna-0.9.2.tar.gz` & `tmp/nlptoolssna-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.9.2.tar", last modified: Tue May 30 18:28:10 2023, max compression
+gzip compressed data, was "dist\nlptoolssna-0.9.3.tar", last modified: Mon Jun  5 20:16:14 2023, max compression
```

## Comparing `nlptoolssna-0.9.2.tar` & `nlptoolssna-0.9.3.tar`

### file list

```diff
@@ -1,105 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.965044 nlptoolssna-0.9.2/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-30 18:28:10.965044 nlptoolssna-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.831739 nlptoolssna-0.9.2/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.9.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.789202 nlptoolssna-0.9.2/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.791206 nlptoolssna-0.9.2/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.833741 nlptoolssna-0.9.2/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.2/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.842015 nlptoolssna-0.9.2/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.2/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.9.2/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.2/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.2/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.9.2/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.852905 nlptoolssna-0.9.2/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.855723 nlptoolssna-0.9.2/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.2/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.863067 nlptoolssna-0.9.2/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.865123 nlptoolssna-0.9.2/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.9.2/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.9.2/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.866069 nlptoolssna-0.9.2/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.9.2/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.9.2/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.874245 nlptoolssna-0.9.2/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.9.2/docs/source/api/utils/implication.rst
--rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.9.2/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.9.2/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.9.2/docs/source/api/utils/text_transliteration.rst
--rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.9.2/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.9.2/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.9.2/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.9.2/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.9.2/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.9.2/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.880272 nlptoolssna-0.9.2/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.883254 nlptoolssna-0.9.2/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.9.2/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     9187 2023-05-17 17:03:21.000000 nlptoolssna-0.9.2/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.9.2/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.885341 nlptoolssna-0.9.2/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.9.2/nlptools/arabiner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.894867 nlptoolssna-0.9.2/nlptools/arabiner/bin/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-05-29 19:50:55.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/eval.py
--rw-rw-rw-   0        0        0     2472 2023-05-30 17:36:00.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/infer.py
--rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/process.py
--rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/train.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.899868 nlptoolssna-0.9.2/nlptools/arabiner/data/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/data/__init__.py
--rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.9.2/nlptools/arabiner/data/datasets.py
--rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/data/transforms.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.906524 nlptoolssna-0.9.2/nlptools/arabiner/nn/
--rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/BaseModel.py
--rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/BertNestedTagger.py
--rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/BertSeqTagger.py
--rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.913750 nlptoolssna-0.9.2/nlptools/arabiner/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/__init__.py
--rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/data.py
--rw-rw-rw-   0        0        0     3720 2023-05-17 17:35:38.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/helpers.py
--rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/metrics.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.915749 nlptoolssna-0.9.2/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.9.2/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.925396 nlptoolssna-0.9.2/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.9.2/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.9.2/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.9.2/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.9.2/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.9.2/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.930740 nlptoolssna-0.9.2/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.9.2/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    17930 2023-05-20 20:02:01.000000 nlptoolssna-0.9.2/nlptools/salma/views.py
--rw-rw-rw-   0        0        0     7719 2023-05-20 20:02:29.000000 nlptoolssna-0.9.2/nlptools/salma/wsd.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.947367 nlptoolssna-0.9.2/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.9.2/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0     4706 2023-05-29 19:21:39.000000 nlptoolssna-0.9.2/nlptools/utils/corpus.py
--rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.9.2/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0    10160 2023-05-22 14:31:38.000000 nlptoolssna-0.9.2/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     6144 2023-05-22 14:15:55.000000 nlptoolssna-0.9.2/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.9.2/nlptools/utils/text_transliteration.py
--rw-rw-rw-   0        0        0     1201 2023-05-29 19:17:26.000000 nlptoolssna-0.9.2/nlptools/utils/tokenizer.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.9.2/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.959528 nlptoolssna-0.9.2/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      144 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-30 18:28:10.966854 nlptoolssna-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     2095 2023-05-17 07:09:09.000000 nlptoolssna-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.963911 nlptoolssna-0.9.2/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:14.102490 nlptoolssna-0.9.3/
+-rw-rw-rw-   0        0        0      159 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3539 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       89 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1069 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0      262 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2282 2023-06-05 20:16:14.103496 nlptoolssna-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.360428 nlptoolssna-0.9.3/docs/
+-rw-rw-rw-   0        0        0      656 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:11.940341 nlptoolssna-0.9.3/docs/build/
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:11.954339 nlptoolssna-0.9.3/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.366428 nlptoolssna-0.9.3/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.434476 nlptoolssna-0.9.3/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2020-07-08 15:50:51.000000 nlptoolssna-0.9.3/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2020-07-08 15:50:51.000000 nlptoolssna-0.9.3/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2020-07-08 15:50:51.000000 nlptoolssna-0.9.3/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      756 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.636485 nlptoolssna-0.9.3/docs/source/
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.648485 nlptoolssna-0.9.3/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.664484 nlptoolssna-0.9.3/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.668483 nlptoolssna-0.9.3/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      131 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      219 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.673485 nlptoolssna-0.9.3/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      139 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      215 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:12.948485 nlptoolssna-0.9.3/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/utils/implication.rst
+-rw-rw-rw-   0        0        0       98 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       95 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      135 2023-06-05 18:40:07.000000 nlptoolssna-0.9.3/docs/source/api/utils/sentence_tokenizer.rst
+-rw-rw-rw-   0        0        0      137 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api/utils/text_transliteration.rst
+-rw-rw-rw-   0        0        0      282 2023-06-05 18:39:56.000000 nlptoolssna-0.9.3/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      168 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/api.rst
+-rw-rw-rw-   0        0        0       31 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     5972 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/conf.py
+-rw-rw-rw-   0        0        0      288 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1126 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       30 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.034489 nlptoolssna-0.9.3/nlptools/
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.192485 nlptoolssna-0.9.3/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     9187 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      128 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.198487 nlptoolssna-0.9.3/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.274500 nlptoolssna-0.9.3/nlptools/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     2504 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/bin/eval.py
+-rw-rw-rw-   0        0        0     1831 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/bin/infer.py
+-rw-rw-rw-   0        0        0     4558 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/bin/process.py
+-rw-rw-rw-   0        0        0     6169 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/bin/train.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.295505 nlptoolssna-0.9.3/nlptools/arabiner/data/
+-rw-rw-rw-   0        0        0        0 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/data/__init__.py
+-rw-rw-rw-   0        0        0     4922 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/data/datasets.py
+-rw-rw-rw-   0        0        0     4761 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/data/transforms.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.392484 nlptoolssna-0.9.3/nlptools/arabiner/nn/
+-rw-rw-rw-   0        0        0      586 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/nn/BaseModel.py
+-rw-rw-rw-   0        0        0     1189 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/nn/BertNestedTagger.py
+-rw-rw-rw-   0        0        0      487 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/nn/BertSeqTagger.py
+-rw-rw-rw-   0        0        0      153 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.453486 nlptoolssna-0.9.3/nlptools/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4041 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3599 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0     2665 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/arabiner/utils/metrics.py
+-rw-rw-rw-   0        0        0      439 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.527485 nlptoolssna-0.9.3/nlptools/morphology/
+-rw-rw-rw-   0        0        0      364 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2724 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     6197 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       45 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      583 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       19 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.548485 nlptoolssna-0.9.3/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    17512 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/salma/views.py
+-rw-rw-rw-   0        0        0     7512 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/salma/wsd.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.674483 nlptoolssna-0.9.3/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    27267 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0     9909 2023-06-05 13:32:11.000000 nlptoolssna-0.9.3/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     5997 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0     2165 2023-06-05 18:51:38.000000 nlptoolssna-0.9.3/nlptools/utils/sentence_tokenizer.py
+-rw-rw-rw-   0        0        0     8605 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/utils/text_transliteration.py
+-rw-rw-rw-   0        0        0       31 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:13.993503 nlptoolssna-0.9.3/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     2282 2023-06-05 20:16:10.000000 nlptoolssna-0.9.3/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-06-05 20:16:11.000000 nlptoolssna-0.9.3/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 20:16:10.000000 nlptoolssna-0.9.3/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-05 20:16:10.000000 nlptoolssna-0.9.3/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-04 17:28:10.000000 nlptoolssna-0.9.3/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      144 2023-06-05 20:16:10.000000 nlptoolssna-0.9.3/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 20:16:10.000000 nlptoolssna-0.9.3/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-06-05 20:16:14.226485 nlptoolssna-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     2026 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:16:14.098499 nlptoolssna-0.9.3/tests/
+-rw-rw-rw-   0        0        0       38 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 17:46:49.000000 nlptoolssna-0.9.3/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.9.2/CONTRIBUTING.rst` & `nlptoolssna-0.9.3/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/eng-aomar/nlptools/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-nlptools could always use more documentation, whether as part of the
-official nlptools docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/eng-aomar/nlptools/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `nlptools` for local development.
-
-1. Fork the `nlptools` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/nlptools.git
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv nlptools
-    $ cd nlptools/
-    $ python setup.py develop
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-    $ flake8 nlptools tests
-    $ python setup.py test or pytest
-    $ tox
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-6. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://travis-ci.com/eng-aomar/nlptools/pull_requests
-   and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-
-    $ python -m unittest tests.test_nlptools
-
-Deploying
----------
-
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-
-Travis will then deploy to PyPI if tests pass.
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/eng-aomar/nlptools/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+nlptools could always use more documentation, whether as part of the
+official nlptools docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/eng-aomar/nlptools/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `nlptools` for local development.
+
+1. Fork the `nlptools` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/nlptools.git
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv nlptools
+    $ cd nlptools/
+    $ python setup.py develop
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+    $ flake8 nlptools tests
+    $ python setup.py test or pytest
+    $ tox
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+6. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
+   https://travis-ci.com/eng-aomar/nlptools/pull_requests
+   and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+
+    $ python -m unittest tests.test_nlptools
+
+Deploying
+---------
+
+A reminder for the maintainers on how to deploy.
+Make sure all your changes are committed (including an entry in HISTORY.rst).
+Then run::
+
+$ bump2version patch # possible: major / minor / patch
+$ git push
+$ git push --tags
+
+Travis will then deploy to PyPI if tests pass.
```

### Comparing `nlptoolssna-0.9.2/PKG-INFO` & `nlptoolssna-0.9.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: nlptoolssna
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
+Description: ========
+        nlptools
+        ========
+        
+        
+        .. image:: https://img.shields.io/pypi/v/nlptools.svg
+                :target: https://pypi.python.org/pypi/nlptools
+        
+        .. image:: https://img.shields.io/travis/eng-aomar/nlptools.svg
+                :target: https://travis-ci.com/eng-aomar/nlptools
+        
+        .. image:: https://readthedocs.org/projects/nlptools/badge/?version=latest
+                :target: https://nlptools.readthedocs.io/en/latest/?version=latest
+                :alt: Documentation Status
+        
+        
+        
+        
+        Python Boilerplate contains all the boilerplate you need to create a Python package.
+        
+        
+        * Free software: MIT license
+        * Documentation: https://nlptools.readthedocs.io.
+        
+        
+        Features
+        --------
+        
+        * TODO
+        
+        Credits
+        -------
+        
+        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+        
+        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
+        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+        
+        
+        =======
+        History
+        =======
+        
+        0.1.0 (2023-04-15)
+        ------------------
+        
+        * First release on PyPI.
+        
 Keywords: nlptools
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-========
-nlptools
-========
-
-
-.. image:: https://img.shields.io/pypi/v/nlptools.svg
-        :target: https://pypi.python.org/pypi/nlptools
-
-.. image:: https://img.shields.io/travis/eng-aomar/nlptools.svg
-        :target: https://travis-ci.com/eng-aomar/nlptools
-
-.. image:: https://readthedocs.org/projects/nlptools/badge/?version=latest
-        :target: https://nlptools.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-
-
-Python Boilerplate contains all the boilerplate you need to create a Python package.
-
-
-* Free software: MIT license
-* Documentation: https://nlptools.readthedocs.io.
-
-
-Features
---------
-
-* TODO
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-
-=======
-History
-=======
-
-0.1.0 (2023-04-15)
-------------------
-
-* First release on PyPI.
```

### Comparing `nlptoolssna-0.9.2/README.rst` & `nlptoolssna-0.9.3/README.rst`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-========
-nlptools
-========
-
-
-.. image:: https://img.shields.io/pypi/v/nlptools.svg
-        :target: https://pypi.python.org/pypi/nlptools
-
-.. image:: https://img.shields.io/travis/eng-aomar/nlptools.svg
-        :target: https://travis-ci.com/eng-aomar/nlptools
-
-.. image:: https://readthedocs.org/projects/nlptools/badge/?version=latest
-        :target: https://nlptools.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-
-
-Python Boilerplate contains all the boilerplate you need to create a Python package.
-
-
-* Free software: MIT license
-* Documentation: https://nlptools.readthedocs.io.
-
-
-Features
---------
-
-* TODO
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+========
+nlptools
+========
+
+
+.. image:: https://img.shields.io/pypi/v/nlptools.svg
+        :target: https://pypi.python.org/pypi/nlptools
+
+.. image:: https://img.shields.io/travis/eng-aomar/nlptools.svg
+        :target: https://travis-ci.com/eng-aomar/nlptools
+
+.. image:: https://readthedocs.org/projects/nlptools/badge/?version=latest
+        :target: https://nlptools.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+
+
+Python Boilerplate contains all the boilerplate you need to create a Python package.
+
+
+* Free software: MIT license
+* Documentation: https://nlptools.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `nlptoolssna-0.9.2/docs/Makefile` & `nlptoolssna-0.9.3/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SOURCEDIR     = source
-SPHINXOPTS    =
-SPHINXBUILD   = sphinx-build -c $(SOURCEDIR) -c $(SOURCEDIR)/config
-SPHINXPROJ    = nlptools
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-    @$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-    @$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line.
+SOURCEDIR     = source
+SPHINXOPTS    =
+SPHINXBUILD   = sphinx-build -c $(SOURCEDIR) -c $(SOURCEDIR)/config
+SPHINXPROJ    = nlptools
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+    @$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+    @$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `nlptoolssna-0.9.2/docs/build/html/_images/download.png` & `nlptoolssna-0.9.3/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.2/docs/build/html/_static/download.png` & `nlptoolssna-0.9.3/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.2/docs/make.bat` & `nlptoolssna-0.9.3/docs/make.bat`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=source
-set BUILDDIR=build
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
-	exit /b 1
-)
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=source
+set BUILDDIR=build
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.http://sphinx-doc.org/
+	exit /b 1
+)
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+
+:end
+popd
```

### Comparing `nlptoolssna-0.9.2/docs/source/_static/download.png` & `nlptoolssna-0.9.3/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.2/docs/source/installation.rst` & `nlptoolssna-0.9.3/docs/source/installation.rst`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-.. highlight:: shell
-
-============
-Installation
-============
-
-
-Stable release
---------------
-
-To install nlptools, run this command in your terminal:
-
-.. code-block:: console
-
-    $ pip install nlptools
-
-This is the preferred method to install nlptools, as it will always install the most recent stable release.
-
-If you don't have `pip`_ installed, this `Python installation guide`_ can guide
-you through the process.
-
-.. _pip: https://pip.pypa.io
-.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
-
-
-From sources
-------------
-
-The sources for nlptools can be downloaded from the `Github repo`_.
-
-You can either clone the public repository:
-
-.. code-block:: console
-
-    $ git clone git://github.com/eng-aomar/nlptools
-
-Or download the `tarball`_:
-
-.. code-block:: console
-
-    $ curl -OJL https://github.com/eng-aomar/nlptools/tarball/master
-
-Once you have a copy of the source, you can install it with:
-
-.. code-block:: console
-
-    $ python setup.py install
-
-
-.. _Github repo: https://github.com/eng-aomar/nlptools
-.. _tarball: https://github.com/eng-aomar/nlptools/tarball/master
+.. highlight:: shell
+
+============
+Installation
+============
+
+
+Stable release
+--------------
+
+To install nlptools, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install nlptools
+
+This is the preferred method to install nlptools, as it will always install the most recent stable release.
+
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for nlptools can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: console
+
+    $ git clone git://github.com/eng-aomar/nlptools
+
+Or download the `tarball`_:
+
+.. code-block:: console
+
+    $ curl -OJL https://github.com/eng-aomar/nlptools/tarball/master
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: console
+
+    $ python setup.py install
+
+
+.. _Github repo: https://github.com/eng-aomar/nlptools
+.. _tarball: https://github.com/eng-aomar/nlptools/tarball/master
```

### Comparing `nlptoolssna-0.9.2/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.9.3/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/bin/eval.py` & `nlptoolssna-0.9.3/nlptools/arabiner/bin/eval.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,87 @@
-import os
-import logging
-from collections import namedtuple
-from nlptools.arabiner.utils.helpers import load_checkpoint, make_output_dirs, logging_config
-from nlptools.arabiner.utils.data import get_dataloaders, parse_conll_files
-from nlptools.arabiner.utils.metrics import compute_single_label_metrics, compute_nested_metrics
-from nlptools.DataDownload import downloader
-logger = logging.getLogger(__name__)
-
-
-def evaluate_dataset(output_path,data_paths ,batch_size=32):
-    """
-    Run the model to evaluate text data and save the predictions.
-
-    Args:
-        output_path (str): Path to save the results.
-        model_path (str): Model path.
-        data_paths (list[str]): List of paths to text or sequence files to tag.
-        batch_size (int, optional): Batch size. Default is 32.
-    """
-    # Create directory to save predictions
-    make_output_dirs(output_path, overwrite=True)
-    logging_config(log_file=os.path.join(output_path, "eval.log"))
-    filename = 'Wj27012000.tar'
-    path =downloader.get_appdatadir()
-    model_path = os.path.join(path, filename)
-    # Load tagger
-    tagger, tag_vocab, train_config = load_checkpoint(model_path)
-
-    # Convert text to a tagger dataset and index the tokens in args.text
-    datasets, vocab = parse_conll_files(data_paths)
-
-    vocabs = namedtuple("Vocab", ["tags", "tokens"])
-    vocab = vocabs(tokens=vocab.tokens, tags=tag_vocab)
-
-    # From the datasets generate the dataloaders
-    dataloaders = get_dataloaders(
-        datasets, vocab,
-        train_config.data_config,
-        batch_size=batch_size,
-        shuffle=[False] * len(datasets)
-    )
-
-    # Evaluate the model on each dataloader
-    for dataloader, input_file in zip(dataloaders,data_paths):
-        filename = os.path.basename(input_file)
-        predictions_file = os.path.join(output_path, f"predictions_{filename}")
-        _, segments, _, _ = tagger.eval(dataloader)
-        tagger.segments_to_file(segments, predictions_file)
-
-        if "Nested" in train_config.trainer_config["fn"]:
-            compute_nested_metrics(segments, vocab.tags[1:])
-        else:
-            compute_single_label_metrics(segments)
-
+import os
+import logging
+import argparse
+from collections import namedtuple
+from nlptools.arabiner.utils.helpers import load_checkpoint, make_output_dirs, logging_config
+from nlptools.arabiner.utils.data import get_dataloaders, parse_conll_files
+from nlptools.arabiner.utils.metrics import compute_single_label_metrics, compute_nested_metrics
+
+logger = logging.getLogger(__name__)
+
+
+def parse_args():
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+
+    parser.add_argument(
+        "--output_path",
+        type=str,
+        required=True,
+        help="Path to save results",
+    )
+
+    parser.add_argument(
+        "--model_path",
+        type=str,
+        required=True,
+        help="Model path",
+    )
+
+    parser.add_argument(
+        "--data_paths",
+        nargs="+",
+        type=str,
+        required=True,
+        help="Text or sequence to tag, this is in same format as training data with 'O' tag for all tokens",
+    )
+
+    parser.add_argument(
+        "--batch_size",
+        type=int,
+        default=32,
+        help="Batch size",
+    )
+
+    args = parser.parse_args()
+
+    return args
+
+
+def main(args):
+    # Create directory to save predictions
+    make_output_dirs(args.output_path, overwrite=True)
+    logging_config(log_file=os.path.join(args.output_path, "eval.log"))
+
+    # Load tagger
+    tagger, tag_vocab, train_config = load_checkpoint(args.model_path)
+
+    # Convert text to a tagger dataset and index the tokens in args.text
+    datasets, vocab = parse_conll_files(args.data_paths)
+
+    vocabs = namedtuple("Vocab", ["tags", "tokens"])
+    vocab = vocabs(tokens=vocab.tokens, tags=tag_vocab)
+
+    # From the datasets generate the dataloaders
+    dataloaders = get_dataloaders(
+        datasets, vocab,
+        train_config.data_config,
+        batch_size=args.batch_size,
+        shuffle=[False] * len(datasets)
+    )
+
+    # Evaluate the model on each dataloader
+    for dataloader, input_file in zip(dataloaders, args.data_paths):
+        filename = os.path.basename(input_file)
+        predictions_file = os.path.join(args.output_path, f"predictions_{filename}")
+        _, segments, _, _ = tagger.eval(dataloader)
+        tagger.segments_to_file(segments, predictions_file)
+
+        if "Nested" in train_config.trainer_config["fn"]:
+            compute_nested_metrics(segments, vocab.tags[1:])
+        else:
+            compute_single_label_metrics(segments)
+
+
+if __name__ == "__main__":
+    main(parse_args())
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/bin/process.py` & `nlptoolssna-0.9.3/nlptools/arabiner/bin/process.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-import os
-import argparse
-import csv
-import logging
-import numpy as np
-from nlptools.arabiner.utils.helpers import logging_config
-from nlptools.arabiner.utils.data import conll_to_segments
-
-logger = logging.getLogger(__name__)
-
-
-def to_conll_format(input_files, output_path, multi_label=False):
-    """
-    Parse data files and convert them into CoNLL format
-    :param input_files: List[str] - list of filenames
-    :param output_path: str - output path
-    :param multi_label: boolean - True to process data with mutli-class/multi-label
-    :return:
-    """
-    for input_file in input_files:
-        tokens = list()
-        prev_sent_id = None
-
-        with open(input_file, "r") as fh:
-            r = csv.reader(fh, delimiter="\t", quotechar=" ")
-            next(r)
-
-            for row in r:
-                sent_id, token, labels = row[1], row[3], row[4].split()
-                valid_labels = sum([1 for l in labels if "-" in l or l == "O"]) == len(labels)
-
-                if not valid_labels:
-                    logging.warning("Invalid labels found %s", str(row))
-                    continue
-                if not labels:
-                    logging.warning("Token %s has no label", str(row))
-                    continue
-                if not token:
-                    logging.warning("Token %s is missing", str(row))
-                    continue
-                if len(token.split()) > 1:
-                    logging.warning("Token %s has multiple tokens", str(row))
-                    continue
-
-                if prev_sent_id is not None and sent_id != prev_sent_id:
-                    tokens.append([])
-
-                if multi_label:
-                    tokens.append([token] + labels)
-                else:
-                    tokens.append([token, labels[0]])
-
-                prev_sent_id = sent_id
-
-        num_segments = sum([1 for token in tokens if not token])
-        logging.info("Found %d segments and %d tokens in %s", num_segments + 1, len(tokens) - num_segments, input_file)
-
-        filename = os.path.basename(input_file)
-        output_file = os.path.join(output_path, filename)
-
-        with open(output_file, "w") as fh:
-            fh.write("\n".join(" ".join(token) for token in tokens))
-            logging.info("Output file %s", output_file)
-
-
-def train_dev_test_split(input_files, output_path, train_ratio, dev_ratio):
-    segments = list()
-    filenames = ["train.txt", "val.txt", "test.txt"]
-
-    for input_file in input_files:
-        segments += conll_to_segments(input_file)
-
-    n = len(segments)
-    np.random.shuffle(segments)
-    datasets = np.split(segments, [int(train_ratio*n), int((train_ratio+dev_ratio)*n)])
-
-    # write data to files
-    for i in range(len(datasets)):
-        filename = os.path.join(output_path, filenames[i])
-
-        with open(filename, "w") as fh:
-            text = "\n\n".join(["\n".join([f"{token.text} {' '.join(token.gold_tag)}" for token in segment]) for segment in datasets[i]])
-            fh.write(text)
-            logging.info("Output file %s", filename)
-
-
-def main(args):
-    if args.task == "to_conll_format":
-        to_conll_format(args.input_files, args.output_path, multi_label=args.multi_label)
-    if args.task == "train_dev_test_split":
-        train_dev_test_split(args.input_files, args.output_path, args.train_ratio, args.dev_ratio)
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    parser.add_argument(
-        "--input_files",
-        type=str,
-        nargs="+",
-        required=True,
-        help="List of input files",
-    )
-
-    parser.add_argument(
-        "--output_path",
-        type=str,
-        required=True,
-        help="Output path",
-    )
-
-    parser.add_argument(
-        "--train_ratio",
-        type=float,
-        required=False,
-        help="Training data ratio (percent of segments). Required with the task train_dev_test_split. "
-             "Files must in ConLL format",
-    )
-
-    parser.add_argument(
-        "--dev_ratio",
-        type=float,
-        required=False,
-        help="Dev/val data ratio (percent of segments). Required with the task train_dev_test_split. "
-             "Files must in ConLL format",
-    )
-
-    parser.add_argument(
-        "--task", required=True, choices=["to_conll_format", "train_dev_test_split"]
-    )
-
-    parser.add_argument(
-        "--multi_label", action='store_true'
-    )
-
-    args = parser.parse_args()
-    logging_config(os.path.join(args.output_path, "process.log"))
-    main(args)
+import os
+import argparse
+import csv
+import logging
+import numpy as np
+from nlptools.arabiner.utils.helpers import logging_config
+from nlptools.arabiner.utils.data import conll_to_segments
+
+logger = logging.getLogger(__name__)
+
+
+def to_conll_format(input_files, output_path, multi_label=False):
+    """
+    Parse data files and convert them into CoNLL format
+    :param input_files: List[str] - list of filenames
+    :param output_path: str - output path
+    :param multi_label: boolean - True to process data with mutli-class/multi-label
+    :return:
+    """
+    for input_file in input_files:
+        tokens = list()
+        prev_sent_id = None
+
+        with open(input_file, "r") as fh:
+            r = csv.reader(fh, delimiter="\t", quotechar=" ")
+            next(r)
+
+            for row in r:
+                sent_id, token, labels = row[1], row[3], row[4].split()
+                valid_labels = sum([1 for l in labels if "-" in l or l == "O"]) == len(labels)
+
+                if not valid_labels:
+                    logging.warning("Invalid labels found %s", str(row))
+                    continue
+                if not labels:
+                    logging.warning("Token %s has no label", str(row))
+                    continue
+                if not token:
+                    logging.warning("Token %s is missing", str(row))
+                    continue
+                if len(token.split()) > 1:
+                    logging.warning("Token %s has multiple tokens", str(row))
+                    continue
+
+                if prev_sent_id is not None and sent_id != prev_sent_id:
+                    tokens.append([])
+
+                if multi_label:
+                    tokens.append([token] + labels)
+                else:
+                    tokens.append([token, labels[0]])
+
+                prev_sent_id = sent_id
+
+        num_segments = sum([1 for token in tokens if not token])
+        logging.info("Found %d segments and %d tokens in %s", num_segments + 1, len(tokens) - num_segments, input_file)
+
+        filename = os.path.basename(input_file)
+        output_file = os.path.join(output_path, filename)
+
+        with open(output_file, "w") as fh:
+            fh.write("\n".join(" ".join(token) for token in tokens))
+            logging.info("Output file %s", output_file)
+
+
+def train_dev_test_split(input_files, output_path, train_ratio, dev_ratio):
+    segments = list()
+    filenames = ["train.txt", "val.txt", "test.txt"]
+
+    for input_file in input_files:
+        segments += conll_to_segments(input_file)
+
+    n = len(segments)
+    np.random.shuffle(segments)
+    datasets = np.split(segments, [int(train_ratio*n), int((train_ratio+dev_ratio)*n)])
+
+    # write data to files
+    for i in range(len(datasets)):
+        filename = os.path.join(output_path, filenames[i])
+
+        with open(filename, "w") as fh:
+            text = "\n\n".join(["\n".join([f"{token.text} {' '.join(token.gold_tag)}" for token in segment]) for segment in datasets[i]])
+            fh.write(text)
+            logging.info("Output file %s", filename)
+
+
+def main(args):
+    if args.task == "to_conll_format":
+        to_conll_format(args.input_files, args.output_path, multi_label=args.multi_label)
+    if args.task == "train_dev_test_split":
+        train_dev_test_split(args.input_files, args.output_path, args.train_ratio, args.dev_ratio)
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+
+    parser.add_argument(
+        "--input_files",
+        type=str,
+        nargs="+",
+        required=True,
+        help="List of input files",
+    )
+
+    parser.add_argument(
+        "--output_path",
+        type=str,
+        required=True,
+        help="Output path",
+    )
+
+    parser.add_argument(
+        "--train_ratio",
+        type=float,
+        required=False,
+        help="Training data ratio (percent of segments). Required with the task train_dev_test_split. "
+             "Files must in ConLL format",
+    )
+
+    parser.add_argument(
+        "--dev_ratio",
+        type=float,
+        required=False,
+        help="Dev/val data ratio (percent of segments). Required with the task train_dev_test_split. "
+             "Files must in ConLL format",
+    )
+
+    parser.add_argument(
+        "--task", required=True, choices=["to_conll_format", "train_dev_test_split"]
+    )
+
+    parser.add_argument(
+        "--multi_label", action='store_true'
+    )
+
+    args = parser.parse_args()
+    logging_config(os.path.join(args.output_path, "process.log"))
+    main(args)
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/bin/train.py` & `nlptoolssna-0.9.3/nlptools/arabiner/bin/train.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import os
-import logging
-import json
-import argparse
-import torch.utils.tensorboard
-from torchvision import *
-import pickle
-from nlptools.arabiner.utils.data import get_dataloaders, parse_conll_files
-from nlptools.arabiner.utils.helpers import logging_config, load_object, make_output_dirs, set_seed
-
-logger = logging.getLogger(__name__)
-
-
-def parse_args():
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    parser.add_argument(
-        "--output_path",
-        type=str,
-        required=True,
-        help="Output path",
-    )
-
-    parser.add_argument(
-        "--train_path",
-        type=str,
-        required=True,
-        help="Path to training data",
-    )
-
-    parser.add_argument(
-        "--val_path",
-        type=str,
-        required=True,
-        help="Path to training data",
-    )
-
-    parser.add_argument(
-        "--test_path",
-        type=str,
-        required=True,
-        help="Path to training data",
-    )
-
-    parser.add_argument(
-        "--bert_model",
-        type=str,
-        default="aubmindlab/bert-base-arabertv2",
-        help="BERT model",
-    )
-
-    parser.add_argument(
-        "--gpus",
-        type=int,
-        nargs="+",
-        default=[0],
-        help="GPU IDs to train on",
-    )
-
-    parser.add_argument(
-        "--log_interval",
-        type=int,
-        default=10,
-        help="Log results every that many timesteps",
-    )
-
-    parser.add_argument(
-        "--batch_size",
-        type=int,
-        default=32,
-        help="Batch size",
-    )
-
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=0,
-        help="Dataloader number of workers",
-    )
-
-    parser.add_argument(
-        "--data_config",
-        type=json.loads,
-        default='{"fn": "arabiner.data.datasets.DefaultDataset", "kwargs": {"max_seq_len": 512}}',
-        help="Dataset configurations",
-    )
-
-    parser.add_argument(
-        "--trainer_config",
-        type=json.loads,
-        default='{"fn": "arabiner.trainers.BertTrainer", "kwargs": {"max_epochs": 50}}',
-        help="Trainer configurations",
-    )
-
-    parser.add_argument(
-        "--network_config",
-        type=json.loads,
-        default='{"fn": "arabiner.nn.BertSeqTagger", "kwargs": '
-                '{"dropout": 0.1, "bert_model": "aubmindlab/bert-base-arabertv2"}}',
-        help="Network configurations",
-    )
-
-    parser.add_argument(
-        "--optimizer",
-        type=json.loads,
-        default='{"fn": "torch.optim.AdamW", "kwargs": {"lr": 0.0001}}',
-        help="Optimizer configurations",
-    )
-
-    parser.add_argument(
-        "--lr_scheduler",
-        type=json.loads,
-        default='{"fn": "torch.optim.lr_scheduler.ExponentialLR", "kwargs": {"gamma": 1}}',
-        help="Learning rate scheduler configurations",
-    )
-
-    parser.add_argument(
-        "--loss",
-        type=json.loads,
-        default='{"fn": "torch.nn.CrossEntropyLoss", "kwargs": {}}',
-        help="Loss function configurations",
-    )
-
-    parser.add_argument(
-        "--overwrite",
-        action="store_true",
-        help="Overwrite output directory",
-    )
-
-    parser.add_argument(
-        "--seed",
-        type=int,
-        default=1,
-        help="Seed for random initialization",
-    )
-
-    args = parser.parse_args()
-
-    return args
-
-
-def main(args):
-    make_output_dirs(
-        args.output_path,
-        subdirs=("tensorboard", "checkpoints"),
-        overwrite=args.overwrite,
-    )
-
-    # Set the seed for randomization
-    set_seed(args.seed)
-
-    logging_config(os.path.join(args.output_path, "train.log"))
-    summary_writer = torch.utils.tensorboard.SummaryWriter(
-        os.path.join(args.output_path, "tensorboard")
-    )
-    os.environ["CUDA_VISIBLE_DEVICES"] = ",".join([str(gpu) for gpu in args.gpus])
-
-    # Get the datasets and vocab for tags and tokens
-    datasets, vocab = parse_conll_files((args.train_path, args.val_path, args.test_path))
-
-    if "Nested" in args.network_config["fn"]:
-        args.network_config["kwargs"]["num_labels"] = [len(v) for v in vocab.tags[1:]]
-    else:
-        args.network_config["kwargs"]["num_labels"] = len(vocab.tags[0])
-
-    # Save tag vocab to desk
-    with open(os.path.join(args.output_path, "tag_vocab.pkl"), "wb") as fh:
-        pickle.dump(vocab.tags, fh)
-
-    # Write config to file
-    args_file = os.path.join(args.output_path, "args.json")
-    with open(args_file, "w") as fh:
-        logger.info("Writing config to %s", args_file)
-        json.dump(args.__dict__, fh, indent=4)
-
-    # From the datasets generate the dataloaders
-    args.data_config["kwargs"]["bert_model"] = args.network_config["kwargs"]["bert_model"]
-    train_dataloader, val_dataloader, test_dataloader = get_dataloaders(
-        datasets, vocab, args.data_config, args.batch_size, args.num_workers
-    )
-
-    model = load_object(args.network_config["fn"], args.network_config["kwargs"])
-    model = torch.nn.DataParallel(model, device_ids=range(len(args.gpus)))
-
-    if torch.cuda.is_available():
-        model = model.cuda()
-
-    args.optimizer["kwargs"]["params"] = model.parameters()
-    optimizer = load_object(args.optimizer["fn"], args.optimizer["kwargs"])
-
-    args.lr_scheduler["kwargs"]["optimizer"] = optimizer
-    if "num_training_steps" in args.lr_scheduler["kwargs"]:
-        args.lr_scheduler["kwargs"]["num_training_steps"] = args.max_epochs * len(
-            train_dataloader
-        )
-
-    scheduler = load_object(args.lr_scheduler["fn"], args.lr_scheduler["kwargs"])
-    loss = load_object(args.loss["fn"], args.loss["kwargs"])
-
-    args.trainer_config["kwargs"].update({
-        "model": model,
-        "optimizer": optimizer,
-        "scheduler": scheduler,
-        "loss": loss,
-        "train_dataloader": train_dataloader,
-        "val_dataloader": val_dataloader,
-        "test_dataloader": test_dataloader,
-        "log_interval": args.log_interval,
-        "summary_writer": summary_writer,
-        "output_path": args.output_path
-    })
-
-    trainer = load_object(args.trainer_config["fn"], args.trainer_config["kwargs"])
-    trainer.train()
-    return
-
-
-if __name__ == "__main__":
-    main(parse_args())
+import os
+import logging
+import json
+import argparse
+import torch.utils.tensorboard
+from torchvision import *
+import pickle
+from nlptools.arabiner.utils.data import get_dataloaders, parse_conll_files
+from nlptools.arabiner.utils.helpers import logging_config, load_object, make_output_dirs, set_seed
+
+logger = logging.getLogger(__name__)
+
+
+def parse_args():
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+
+    parser.add_argument(
+        "--output_path",
+        type=str,
+        required=True,
+        help="Output path",
+    )
+
+    parser.add_argument(
+        "--train_path",
+        type=str,
+        required=True,
+        help="Path to training data",
+    )
+
+    parser.add_argument(
+        "--val_path",
+        type=str,
+        required=True,
+        help="Path to training data",
+    )
+
+    parser.add_argument(
+        "--test_path",
+        type=str,
+        required=True,
+        help="Path to training data",
+    )
+
+    parser.add_argument(
+        "--bert_model",
+        type=str,
+        default="aubmindlab/bert-base-arabertv2",
+        help="BERT model",
+    )
+
+    parser.add_argument(
+        "--gpus",
+        type=int,
+        nargs="+",
+        default=[0],
+        help="GPU IDs to train on",
+    )
+
+    parser.add_argument(
+        "--log_interval",
+        type=int,
+        default=10,
+        help="Log results every that many timesteps",
+    )
+
+    parser.add_argument(
+        "--batch_size",
+        type=int,
+        default=32,
+        help="Batch size",
+    )
+
+    parser.add_argument(
+        "--num_workers",
+        type=int,
+        default=0,
+        help="Dataloader number of workers",
+    )
+
+    parser.add_argument(
+        "--data_config",
+        type=json.loads,
+        default='{"fn": "arabiner.data.datasets.DefaultDataset", "kwargs": {"max_seq_len": 512}}',
+        help="Dataset configurations",
+    )
+
+    parser.add_argument(
+        "--trainer_config",
+        type=json.loads,
+        default='{"fn": "arabiner.trainers.BertTrainer", "kwargs": {"max_epochs": 50}}',
+        help="Trainer configurations",
+    )
+
+    parser.add_argument(
+        "--network_config",
+        type=json.loads,
+        default='{"fn": "arabiner.nn.BertSeqTagger", "kwargs": '
+                '{"dropout": 0.1, "bert_model": "aubmindlab/bert-base-arabertv2"}}',
+        help="Network configurations",
+    )
+
+    parser.add_argument(
+        "--optimizer",
+        type=json.loads,
+        default='{"fn": "torch.optim.AdamW", "kwargs": {"lr": 0.0001}}',
+        help="Optimizer configurations",
+    )
+
+    parser.add_argument(
+        "--lr_scheduler",
+        type=json.loads,
+        default='{"fn": "torch.optim.lr_scheduler.ExponentialLR", "kwargs": {"gamma": 1}}',
+        help="Learning rate scheduler configurations",
+    )
+
+    parser.add_argument(
+        "--loss",
+        type=json.loads,
+        default='{"fn": "torch.nn.CrossEntropyLoss", "kwargs": {}}',
+        help="Loss function configurations",
+    )
+
+    parser.add_argument(
+        "--overwrite",
+        action="store_true",
+        help="Overwrite output directory",
+    )
+
+    parser.add_argument(
+        "--seed",
+        type=int,
+        default=1,
+        help="Seed for random initialization",
+    )
+
+    args = parser.parse_args()
+
+    return args
+
+
+def main(args):
+    make_output_dirs(
+        args.output_path,
+        subdirs=("tensorboard", "checkpoints"),
+        overwrite=args.overwrite,
+    )
+
+    # Set the seed for randomization
+    set_seed(args.seed)
+
+    logging_config(os.path.join(args.output_path, "train.log"))
+    summary_writer = torch.utils.tensorboard.SummaryWriter(
+        os.path.join(args.output_path, "tensorboard")
+    )
+    os.environ["CUDA_VISIBLE_DEVICES"] = ",".join([str(gpu) for gpu in args.gpus])
+
+    # Get the datasets and vocab for tags and tokens
+    datasets, vocab = parse_conll_files((args.train_path, args.val_path, args.test_path))
+
+    if "Nested" in args.network_config["fn"]:
+        args.network_config["kwargs"]["num_labels"] = [len(v) for v in vocab.tags[1:]]
+    else:
+        args.network_config["kwargs"]["num_labels"] = len(vocab.tags[0])
+
+    # Save tag vocab to desk
+    with open(os.path.join(args.output_path, "tag_vocab.pkl"), "wb") as fh:
+        pickle.dump(vocab.tags, fh)
+
+    # Write config to file
+    args_file = os.path.join(args.output_path, "args.json")
+    with open(args_file, "w") as fh:
+        logger.info("Writing config to %s", args_file)
+        json.dump(args.__dict__, fh, indent=4)
+
+    # From the datasets generate the dataloaders
+    args.data_config["kwargs"]["bert_model"] = args.network_config["kwargs"]["bert_model"]
+    train_dataloader, val_dataloader, test_dataloader = get_dataloaders(
+        datasets, vocab, args.data_config, args.batch_size, args.num_workers
+    )
+
+    model = load_object(args.network_config["fn"], args.network_config["kwargs"])
+    model = torch.nn.DataParallel(model, device_ids=range(len(args.gpus)))
+
+    if torch.cuda.is_available():
+        model = model.cuda()
+
+    args.optimizer["kwargs"]["params"] = model.parameters()
+    optimizer = load_object(args.optimizer["fn"], args.optimizer["kwargs"])
+
+    args.lr_scheduler["kwargs"]["optimizer"] = optimizer
+    if "num_training_steps" in args.lr_scheduler["kwargs"]:
+        args.lr_scheduler["kwargs"]["num_training_steps"] = args.max_epochs * len(
+            train_dataloader
+        )
+
+    scheduler = load_object(args.lr_scheduler["fn"], args.lr_scheduler["kwargs"])
+    loss = load_object(args.loss["fn"], args.loss["kwargs"])
+
+    args.trainer_config["kwargs"].update({
+        "model": model,
+        "optimizer": optimizer,
+        "scheduler": scheduler,
+        "loss": loss,
+        "train_dataloader": train_dataloader,
+        "val_dataloader": val_dataloader,
+        "test_dataloader": test_dataloader,
+        "log_interval": args.log_interval,
+        "summary_writer": summary_writer,
+        "output_path": args.output_path
+    })
+
+    trainer = load_object(args.trainer_config["fn"], args.trainer_config["kwargs"])
+    trainer.train()
+    return
+
+
+if __name__ == "__main__":
+    main(parse_args())
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/data/datasets.py` & `nlptoolssna-0.9.3/nlptools/arabiner/data/datasets.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import logging
-import torch
-from torch.utils.data import Dataset
-from torch.nn.utils.rnn import pad_sequence
-from nlptools.arabiner.data.transforms import (
-    BertSeqTransform,
-    NestedTagsTransform
-)
-
-logger = logging.getLogger(__name__)
-
-
-class Token:
-    def __init__(self, text=None, pred_tag=None, gold_tag=None):
-        """
-        Token object to hold token attributes
-        :param text: str
-        :param pred_tag: str
-        :param gold_tag: str
-        """
-        self.text = text
-        self.gold_tag = gold_tag
-        self.pred_tag = pred_tag
-        self.subwords = None
-
-    @property
-    def subwords(self):
-        return self._subwords
-
-    @subwords.setter
-    def subwords(self, value):
-        self._subwords = value
-
-    def __str__(self):
-        """
-        Token text representation
-        :return: str
-        """
-        gold_tags = "|".join(self.gold_tag)
-        pred_tags = "|".join([pred_tag["tag"] for pred_tag in self.pred_tag])
-
-        if self.gold_tag:
-            r = f"{self.text}\t{gold_tags}\t{pred_tags}"
-        else:
-            r = f"{self.text}\t{pred_tags}"
-
-        return r
-
-
-class DefaultDataset(Dataset):
-    def __init__(
-        self,
-        examples=None,
-        vocab=None,
-        bert_model="aubmindlab/bert-base-arabertv2",
-        max_seq_len=512,
-    ):
-        """
-        The dataset that used to transform the segments into training data
-        :param examples: list[[tuple]] - [[(token, tag), (token, tag), ...], [(token, tag), ...]]
-                         You can get generate examples from -- arabiner.data.dataset.parse_conll_files
-        :param vocab: vocab object containing indexed tags and tokens
-        :param bert_model: str - BERT model
-        :param: int - maximum sequence length
-        """
-        self.transform = BertSeqTransform(bert_model, vocab, max_seq_len=max_seq_len)
-        self.examples = examples
-        self.vocab = vocab
-
-    def __len__(self):
-        return len(self.examples)
-
-    def __getitem__(self, item):
-        subwords, tags, tokens, valid_len = self.transform(self.examples[item])
-        return subwords, tags, tokens, valid_len
-
-    def collate_fn(self, batch):
-        """
-        Collate function that is called when the batch is called by the trainer
-        :param batch: Dataloader batch
-        :return: Same output as the __getitem__ function
-        """
-        subwords, tags, tokens, valid_len = zip(*batch)
-
-        # Pad sequences in this batch
-        # subwords and tokens are padded with zeros
-        # tags are padding with the index of the O tag
-        subwords = pad_sequence(subwords, batch_first=True, padding_value=0)
-        tags = pad_sequence(
-            tags, batch_first=True, padding_value=self.vocab.tags[0].get_stoi()["O"]
-        )
-        return subwords, tags, tokens, valid_len
-
-
-class NestedTagsDataset(Dataset):
-    def __init__(
-        self,
-        examples=None,
-        vocab=None,
-        bert_model="aubmindlab/bert-base-arabertv2",
-        max_seq_len=512,
-    ):
-        """
-        The dataset that used to transform the segments into training data
-        :param examples: list[[tuple]] - [[(token, tag), (token, tag), ...], [(token, tag), ...]]
-                         You can get generate examples from -- arabiner.data.dataset.parse_conll_files
-        :param vocab: vocab object containing indexed tags and tokens
-        :param bert_model: str - BERT model
-        :param: int - maximum sequence length
-        """
-        self.transform = NestedTagsTransform(
-            bert_model, vocab, max_seq_len=max_seq_len
-        )
-        self.examples = examples
-        self.vocab = vocab
-
-    def __len__(self):
-        return len(self.examples)
-
-    def __getitem__(self, item):
-        subwords, tags, tokens, masks, valid_len = self.transform(self.examples[item])
-        return subwords, tags, tokens, masks, valid_len
-
-    def collate_fn(self, batch):
-        """
-        Collate function that is called when the batch is called by the trainer
-        :param batch: Dataloader batch
-        :return: Same output as the __getitem__ function
-        """
-        subwords, tags, tokens, masks, valid_len = zip(*batch)
-
-        # Pad sequences in this batch
-        # subwords and tokens are padded with zeros
-        # tags are padding with the index of the O tag
-        subwords = pad_sequence(subwords, batch_first=True, padding_value=0)
-
-        masks = [torch.nn.ConstantPad1d((0, subwords.shape[-1] - tag.shape[-1]), 0)(mask)
-                 for tag, mask in zip(tags, masks)]
-        masks = torch.cat(masks)
-
-        # Pad the tags, do the padding for each tag type
-        tags = [torch.nn.ConstantPad1d((0, subwords.shape[-1] - tag.shape[-1]), vocab.get_stoi()["<pad>"])(tag)
-                for tag, vocab in zip(tags, self.vocab.tags[1:])]
-        tags = torch.cat(tags)
-
-        return subwords, tags, tokens, masks, valid_len
+import logging
+import torch
+from torch.utils.data import Dataset
+from torch.nn.utils.rnn import pad_sequence
+from nlptools.arabiner.data.transforms import (
+    BertSeqTransform,
+    NestedTagsTransform
+)
+
+logger = logging.getLogger(__name__)
+
+
+class Token:
+    def __init__(self, text=None, pred_tag=None, gold_tag=None):
+        """
+        Token object to hold token attributes
+        :param text: str
+        :param pred_tag: str
+        :param gold_tag: str
+        """
+        self.text = text
+        self.gold_tag = gold_tag
+        self.pred_tag = pred_tag
+        self.subwords = None
+
+    @property
+    def subwords(self):
+        return self._subwords
+
+    @subwords.setter
+    def subwords(self, value):
+        self._subwords = value
+
+    def __str__(self):
+        """
+        Token text representation
+        :return: str
+        """
+        gold_tags = "|".join(self.gold_tag)
+        pred_tags = "|".join([pred_tag["tag"] for pred_tag in self.pred_tag])
+
+        if self.gold_tag:
+            r = f"{self.text}\t{gold_tags}\t{pred_tags}"
+        else:
+            r = f"{self.text}\t{pred_tags}"
+
+        return r
+
+
+class DefaultDataset(Dataset):
+    def __init__(
+        self,
+        examples=None,
+        vocab=None,
+        bert_model="aubmindlab/bert-base-arabertv2",
+        max_seq_len=512,
+    ):
+        """
+        The dataset that used to transform the segments into training data
+        :param examples: list[[tuple]] - [[(token, tag), (token, tag), ...], [(token, tag), ...]]
+                         You can get generate examples from -- arabiner.data.dataset.parse_conll_files
+        :param vocab: vocab object containing indexed tags and tokens
+        :param bert_model: str - BERT model
+        :param: int - maximum sequence length
+        """
+        self.transform = BertSeqTransform(bert_model, vocab, max_seq_len=max_seq_len)
+        self.examples = examples
+        self.vocab = vocab
+
+    def __len__(self):
+        return len(self.examples)
+
+    def __getitem__(self, item):
+        subwords, tags, tokens, valid_len = self.transform(self.examples[item])
+        return subwords, tags, tokens, valid_len
+
+    def collate_fn(self, batch):
+        """
+        Collate function that is called when the batch is called by the trainer
+        :param batch: Dataloader batch
+        :return: Same output as the __getitem__ function
+        """
+        subwords, tags, tokens, valid_len = zip(*batch)
+
+        # Pad sequences in this batch
+        # subwords and tokens are padded with zeros
+        # tags are padding with the index of the O tag
+        subwords = pad_sequence(subwords, batch_first=True, padding_value=0)
+        tags = pad_sequence(
+            tags, batch_first=True, padding_value=self.vocab.tags[0].get_stoi()["O"]
+        )
+        return subwords, tags, tokens, valid_len
+
+
+class NestedTagsDataset(Dataset):
+    def __init__(
+        self,
+        examples=None,
+        vocab=None,
+        bert_model="aubmindlab/bert-base-arabertv2",
+        max_seq_len=512,
+    ):
+        """
+        The dataset that used to transform the segments into training data
+        :param examples: list[[tuple]] - [[(token, tag), (token, tag), ...], [(token, tag), ...]]
+                         You can get generate examples from -- arabiner.data.dataset.parse_conll_files
+        :param vocab: vocab object containing indexed tags and tokens
+        :param bert_model: str - BERT model
+        :param: int - maximum sequence length
+        """
+        self.transform = NestedTagsTransform(
+            bert_model, vocab, max_seq_len=max_seq_len
+        )
+        self.examples = examples
+        self.vocab = vocab
+
+    def __len__(self):
+        return len(self.examples)
+
+    def __getitem__(self, item):
+        subwords, tags, tokens, masks, valid_len = self.transform(self.examples[item])
+        return subwords, tags, tokens, masks, valid_len
+
+    def collate_fn(self, batch):
+        """
+        Collate function that is called when the batch is called by the trainer
+        :param batch: Dataloader batch
+        :return: Same output as the __getitem__ function
+        """
+        subwords, tags, tokens, masks, valid_len = zip(*batch)
+
+        # Pad sequences in this batch
+        # subwords and tokens are padded with zeros
+        # tags are padding with the index of the O tag
+        subwords = pad_sequence(subwords, batch_first=True, padding_value=0)
+
+        masks = [torch.nn.ConstantPad1d((0, subwords.shape[-1] - tag.shape[-1]), 0)(mask)
+                 for tag, mask in zip(tags, masks)]
+        masks = torch.cat(masks)
+
+        # Pad the tags, do the padding for each tag type
+        tags = [torch.nn.ConstantPad1d((0, subwords.shape[-1] - tag.shape[-1]), vocab.get_stoi()["<pad>"])(tag)
+                for tag, vocab in zip(tags, self.vocab.tags[1:])]
+        tags = torch.cat(tags)
+
+        return subwords, tags, tokens, masks, valid_len
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/data/transforms.py` & `nlptoolssna-0.9.3/nlptools/arabiner/data/transforms.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-import torch
-from transformers import BertTokenizer
-from functools import partial
-import re
-import itertools
-from nlptools.arabiner.data import datasets
-class BertSeqTransform:
-    def __init__(self, bert_model, vocab, max_seq_len=512):
-        self.tokenizer = BertTokenizer.from_pretrained(bert_model)
-        self.encoder = partial(
-            self.tokenizer.encode,
-            max_length=max_seq_len,
-            truncation=True,
-        )
-        self.max_seq_len = max_seq_len
-        self.vocab = vocab
-
-    def __call__(self, segment):
-        subwords, tags, tokens = list(), list(), list()
-        unk_token = datasets.Token(text="UNK")
-
-        for token in segment:
-            token_subwords = self.encoder(token.text)[1:-1]
-            subwords += token_subwords
-            tags += [self.vocab.tags[0].get_stoi()[token.gold_tag[0]]] + [self.vocab.tags[0].get_stoi()["O"]] * (len(token_subwords) - 1)
-            tokens += [token] + [unk_token] * (len(token_subwords) - 1)
-
-        # Truncate to max_seq_len
-        if len(subwords) > self.max_seq_len - 2:
-            text = " ".join([t.text for t in tokens if t.text != "UNK"])
-          
-            subwords = subwords[:self.max_seq_len - 2]
-            tags = tags[:self.max_seq_len - 2]
-            tokens = tokens[:self.max_seq_len - 2]
-
-        subwords.insert(0, self.tokenizer.cls_token_id)
-        subwords.append(self.tokenizer.sep_token_id)
-
-        tags.insert(0, self.vocab.tags[0].get_stoi()["O"])
-        tags.append(self.vocab.tags[0].get_stoi()["O"])
-
-        tokens.insert(0, unk_token)
-        tokens.append(unk_token)
-
-        return torch.LongTensor(subwords), torch.LongTensor(tags), tokens, len(tokens)
-
-
-class NestedTagsTransform:
-    def __init__(self, bert_model, vocab, max_seq_len=512):
-        self.tokenizer = BertTokenizer.from_pretrained(bert_model)
-        self.encoder = partial(
-            self.tokenizer.encode,
-            max_length=max_seq_len,
-            truncation=True,
-        )
-        self.max_seq_len = max_seq_len
-        self.vocab = vocab
-
-    def __call__(self, segment):
-        tags, tokens, subwords = list(), list(), list()
-        unk_token = datasets.Token(text="UNK")
-
-        # Encode each token and get its subwords and IDs
-        for token in segment:
-            token.subwords = self.encoder(token.text)[1:-1]
-            subwords += token.subwords
-            tokens += [token] + [unk_token] * (len(token.subwords ) - 1)
-
-        # Construct the labels for each tag type
-        # The sequence will have a list of tags for each type
-        # The final tags for a sequence is a matrix NUM_TAG_TYPES x SEQ_LEN
-        # Example:
-        #   [
-        #       [O,     O,     B-PERS, I-PERS, O, O, O]
-        #       [B-ORG, I-ORG, O,      O,      O, O, O]
-        #       [O,     O,     O,      O,      O, O, B-GPE]
-        #   ]
-        for vocab in self.vocab.tags[1:]:
-            vocab_tags = "|".join([t for t in vocab.get_itos() if "-" in t])
-            r = re.compile(vocab_tags)
-
-            # This is really messy
-            # For a given token we find a matching tag_name, BUT we might find
-            # multiple matches (i.e. a token can be labeled B-ORG and I-ORG) in this
-            # case we get only the first tag as we do not have overlapping of same type
-            single_type_tags = [[(list(filter(r.match, token.gold_tag))
-                                or ["O"])[0]] + ["O"] * (len(token.subwords) - 1)
-                                for token in segment]
-            single_type_tags = list(itertools.chain(*single_type_tags))
-            tags.append([vocab.get_stoi()[tag] for tag in single_type_tags])
-
-        # Truncate to max_seq_len
-        if len(subwords) > self.max_seq_len - 2:
-            text = " ".join([t.text for t in tokens if t.text != "UNK"])
-          
-            subwords = subwords[:self.max_seq_len - 2]
-            tags = [t[:self.max_seq_len - 2] for t in tags]
-            tokens = tokens[:self.max_seq_len - 2]
-
-        # Add dummy token at the start end of sequence
-        tokens.insert(0, unk_token)
-        tokens.append(unk_token)
-
-        # Add CLS and SEP at start end of subwords
-        subwords.insert(0, self.tokenizer.cls_token_id)
-        subwords.append(self.tokenizer.sep_token_id)
-        subwords = torch.LongTensor(subwords)
-
-        # Add "O" tags for the first and last subwords
-        tags = torch.Tensor(tags)
-        tags = torch.column_stack((
-            torch.Tensor([vocab.get_stoi()["O"] for vocab in self.vocab.tags[1:]]),
-            tags,
-            torch.Tensor([vocab.get_stoi()["O"] for vocab in self.vocab.tags[1:]]),
-        )).unsqueeze(0)
-
-        mask = torch.ones_like(tags)
+import torch
+from transformers import BertTokenizer
+from functools import partial
+import re
+import itertools
+from nlptools.arabiner.data import datasets
+class BertSeqTransform:
+    def __init__(self, bert_model, vocab, max_seq_len=512):
+        self.tokenizer = BertTokenizer.from_pretrained(bert_model)
+        self.encoder = partial(
+            self.tokenizer.encode,
+            max_length=max_seq_len,
+            truncation=True,
+        )
+        self.max_seq_len = max_seq_len
+        self.vocab = vocab
+
+    def __call__(self, segment):
+        subwords, tags, tokens = list(), list(), list()
+        unk_token = datasets.Token(text="UNK")
+
+        for token in segment:
+            token_subwords = self.encoder(token.text)[1:-1]
+            subwords += token_subwords
+            tags += [self.vocab.tags[0].get_stoi()[token.gold_tag[0]]] + [self.vocab.tags[0].get_stoi()["O"]] * (len(token_subwords) - 1)
+            tokens += [token] + [unk_token] * (len(token_subwords) - 1)
+
+        # Truncate to max_seq_len
+        if len(subwords) > self.max_seq_len - 2:
+            text = " ".join([t.text for t in tokens if t.text != "UNK"])
+          
+            subwords = subwords[:self.max_seq_len - 2]
+            tags = tags[:self.max_seq_len - 2]
+            tokens = tokens[:self.max_seq_len - 2]
+
+        subwords.insert(0, self.tokenizer.cls_token_id)
+        subwords.append(self.tokenizer.sep_token_id)
+
+        tags.insert(0, self.vocab.tags[0].get_stoi()["O"])
+        tags.append(self.vocab.tags[0].get_stoi()["O"])
+
+        tokens.insert(0, unk_token)
+        tokens.append(unk_token)
+
+        return torch.LongTensor(subwords), torch.LongTensor(tags), tokens, len(tokens)
+
+
+class NestedTagsTransform:
+    def __init__(self, bert_model, vocab, max_seq_len=512):
+        self.tokenizer = BertTokenizer.from_pretrained(bert_model)
+        self.encoder = partial(
+            self.tokenizer.encode,
+            max_length=max_seq_len,
+            truncation=True,
+        )
+        self.max_seq_len = max_seq_len
+        self.vocab = vocab
+
+    def __call__(self, segment):
+        tags, tokens, subwords = list(), list(), list()
+        unk_token = datasets.Token(text="UNK")
+
+        # Encode each token and get its subwords and IDs
+        for token in segment:
+            token.subwords = self.encoder(token.text)[1:-1]
+            subwords += token.subwords
+            tokens += [token] + [unk_token] * (len(token.subwords ) - 1)
+
+        # Construct the labels for each tag type
+        # The sequence will have a list of tags for each type
+        # The final tags for a sequence is a matrix NUM_TAG_TYPES x SEQ_LEN
+        # Example:
+        #   [
+        #       [O,     O,     B-PERS, I-PERS, O, O, O]
+        #       [B-ORG, I-ORG, O,      O,      O, O, O]
+        #       [O,     O,     O,      O,      O, O, B-GPE]
+        #   ]
+        for vocab in self.vocab.tags[1:]:
+            vocab_tags = "|".join([t for t in vocab.get_itos() if "-" in t])
+            r = re.compile(vocab_tags)
+
+            # This is really messy
+            # For a given token we find a matching tag_name, BUT we might find
+            # multiple matches (i.e. a token can be labeled B-ORG and I-ORG) in this
+            # case we get only the first tag as we do not have overlapping of same type
+            single_type_tags = [[(list(filter(r.match, token.gold_tag))
+                                or ["O"])[0]] + ["O"] * (len(token.subwords) - 1)
+                                for token in segment]
+            single_type_tags = list(itertools.chain(*single_type_tags))
+            tags.append([vocab.get_stoi()[tag] for tag in single_type_tags])
+
+        # Truncate to max_seq_len
+        if len(subwords) > self.max_seq_len - 2:
+            text = " ".join([t.text for t in tokens if t.text != "UNK"])
+          
+            subwords = subwords[:self.max_seq_len - 2]
+            tags = [t[:self.max_seq_len - 2] for t in tags]
+            tokens = tokens[:self.max_seq_len - 2]
+
+        # Add dummy token at the start end of sequence
+        tokens.insert(0, unk_token)
+        tokens.append(unk_token)
+
+        # Add CLS and SEP at start end of subwords
+        subwords.insert(0, self.tokenizer.cls_token_id)
+        subwords.append(self.tokenizer.sep_token_id)
+        subwords = torch.LongTensor(subwords)
+
+        # Add "O" tags for the first and last subwords
+        tags = torch.Tensor(tags)
+        tags = torch.column_stack((
+            torch.Tensor([vocab.get_stoi()["O"] for vocab in self.vocab.tags[1:]]),
+            tags,
+            torch.Tensor([vocab.get_stoi()["O"] for vocab in self.vocab.tags[1:]]),
+        )).unsqueeze(0)
+
+        mask = torch.ones_like(tags)
         return subwords, tags, tokens, mask, len(tokens)
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/nn/BertNestedTagger.py` & `nlptoolssna-0.9.3/nlptools/arabiner/nn/BertNestedTagger.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import torch
-import torch.nn as nn
-from nlptools.arabiner.nn import BaseModel
-
-
-class BertNestedTagger(BaseModel):
-    def __init__(self, **kwargs):
-        super(BertNestedTagger, self).__init__(**kwargs)
-
-        self.max_num_labels = max(self.num_labels)
-        classifiers = [nn.Linear(768, num_labels) for num_labels in self.num_labels]
-        self.classifiers = torch.nn.Sequential(*classifiers)
-
-    def forward(self, x):
-        y = self.bert(x)
-        y = self.dropout(y["last_hidden_state"])
-        output = list()
-
-        for i, classifier in enumerate(self.classifiers):
-            logits = classifier(y)
-
-            # Pad logits to allow Multi-GPU/DataParallel training to work
-            # We will truncate the padded dimensions when we compute the loss in the trainer
-            logits = torch.nn.ConstantPad1d((0, self.max_num_labels - logits.shape[-1]), 0)(logits)
-            output.append(logits)
-
-        # Return tensor of the shape B x T x L x C
-        # B: batch size
-        # T: sequence length
-        # L: number of tag types
-        # C: number of classes per tag type
-        output = torch.stack(output).permute((1, 2, 0, 3))
-        return output
-
+import torch
+import torch.nn as nn
+from nlptools.arabiner.nn import BaseModel
+
+
+class BertNestedTagger(BaseModel):
+    def __init__(self, **kwargs):
+        super(BertNestedTagger, self).__init__(**kwargs)
+
+        self.max_num_labels = max(self.num_labels)
+        classifiers = [nn.Linear(768, num_labels) for num_labels in self.num_labels]
+        self.classifiers = torch.nn.Sequential(*classifiers)
+
+    def forward(self, x):
+        y = self.bert(x)
+        y = self.dropout(y["last_hidden_state"])
+        output = list()
+
+        for i, classifier in enumerate(self.classifiers):
+            logits = classifier(y)
+
+            # Pad logits to allow Multi-GPU/DataParallel training to work
+            # We will truncate the padded dimensions when we compute the loss in the trainer
+            logits = torch.nn.ConstantPad1d((0, self.max_num_labels - logits.shape[-1]), 0)(logits)
+            output.append(logits)
+
+        # Return tensor of the shape B x T x L x C
+        # B: batch size
+        # T: sequence length
+        # L: number of tag types
+        # C: number of classes per tag type
+        output = torch.stack(output).permute((1, 2, 0, 3))
+        return output
+
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/utils/data.py` & `nlptoolssna-0.9.3/nlptools/arabiner/utils/data.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-from torch.utils.data import DataLoader
-from torchtext.vocab import vocab
-from collections import Counter, namedtuple
-import logging
-import re
-import itertools
-from nlptools.arabiner.utils.helpers import load_object
-from nlptools.arabiner.data.datasets import Token
-
-logger = logging.getLogger(__name__)
-
-
-def conll_to_segments(filename):
-    """
-    Convert CoNLL files to segments. This return list of segments and each segment is
-    a list of tuples (token, tag)
-    :param filename: Path
-    :return: list[[tuple]] - [[(token, tag), (token, tag), ...], [(token, tag), ...]]
-    """
-    segments, segment = list(), list()
-
-    with open(filename, "r") as fh:
-        for token in fh.read().splitlines():
-            if not token.strip():
-                segments.append(segment)
-                segment = list()
-            else:
-                parts = token.split()
-                token = Token(text=parts[0], gold_tag=parts[1:])
-                segment.append(token)
-
-        segments.append(segment)
-
-    return segments
-
-
-def parse_conll_files(data_paths):
-    """
-    Parse CoNLL formatted files and return list of segments for each file and index
-    the vocabs and tags across all data_paths
-    :param data_paths: tuple(Path) - tuple of filenames
-    :return: tuple( [[(token, tag), ...], [(token, tag), ...]], -> segments for data_paths[i]
-                    [[(token, tag), ...], [(token, tag), ...]], -> segments for data_paths[i+1],
-                    ...
-                  )
-             List of segments for each dataset and each segment has list of (tokens, tags)
-    """
-    vocabs = namedtuple("Vocab", ["tags", "tokens"])
-    datasets, tags, tokens = list(), list(), list()
-
-    for data_path in data_paths:
-        dataset = conll_to_segments(data_path)
-        datasets.append(dataset)
-        tokens += [token.text for segment in dataset for token in segment]
-        tags += [token.gold_tag for segment in dataset for token in segment]
-
-    # Flatten list of tags
-    tags = list(itertools.chain(*tags))
-
-    # Generate vocabs for tags and tokens
-    tag_vocabs = tag_vocab_by_type(tags)
-    tag_vocabs.insert(0, vocab(Counter(tags)))
-    vocabs = vocabs(tokens=vocab(Counter(tokens), specials=["UNK"]), tags=tag_vocabs)
-    return tuple(datasets), vocabs
-
-
-def tag_vocab_by_type(tags):
-    vocabs = list()
-    c = Counter(tags)
-    tag_names = c.keys()
-    tag_types = sorted(list(set([tag.split("-", 1)[1] for tag in tag_names if "-" in tag])))
-
-    for tag_type in tag_types:
-        r = re.compile(".*-" + tag_type)
-        t = list(filter(r.match, tags)) + ["O"]
-        vocabs.append(vocab(Counter(t), specials=["<pad>"]))
-
-    return vocabs
-
-
-def text2segments(text):
-    """
-    Convert text to a datasets and index the tokens
-    """
-    dataset = [[Token(text=token, gold_tag=["O"]) for token in text.split()]]
-    tokens = [token.text for segment in dataset for token in segment]
-
-    # Generate vocabs for the tokens
-    segment_vocab = vocab(Counter(tokens), specials=["UNK"])
-    return dataset, segment_vocab
-
-
-def get_dataloaders(
-    datasets, vocab, data_config, batch_size=32, num_workers=0, shuffle=(True, False, False)
-):
-    """
-    From the datasets generate the dataloaders
-    :param datasets: list - list of the datasets, list of list of segments and tokens
-    :param batch_size: int
-    :param num_workers: int
-    :param shuffle: boolean - to shuffle the data or not
-    :return: List[torch.utils.data.DataLoader]
-    """
-    dataloaders = list()
-
-    for i, examples in enumerate(datasets):
-        data_config["kwargs"].update({"examples": examples, "vocab": vocab})
-        dataset = load_object(data_config["fn"], data_config["kwargs"])
-
-        dataloader = DataLoader(
-            dataset=dataset,
-            shuffle=shuffle[i],
-            batch_size=batch_size,
-            num_workers=num_workers,
-            collate_fn=dataset.collate_fn,
-        )
-
-        logger.info("%s batches found", len(dataloader))
-        dataloaders.append(dataloader)
-
-    return dataloaders
+from torch.utils.data import DataLoader
+from torchtext.vocab import vocab
+from collections import Counter, namedtuple
+import logging
+import re
+import itertools
+from nlptools.arabiner.utils.helpers import load_object
+from nlptools.arabiner.data.datasets import Token
+
+logger = logging.getLogger(__name__)
+
+
+def conll_to_segments(filename):
+    """
+    Convert CoNLL files to segments. This return list of segments and each segment is
+    a list of tuples (token, tag)
+    :param filename: Path
+    :return: list[[tuple]] - [[(token, tag), (token, tag), ...], [(token, tag), ...]]
+    """
+    segments, segment = list(), list()
+
+    with open(filename, "r") as fh:
+        for token in fh.read().splitlines():
+            if not token.strip():
+                segments.append(segment)
+                segment = list()
+            else:
+                parts = token.split()
+                token = Token(text=parts[0], gold_tag=parts[1:])
+                segment.append(token)
+
+        segments.append(segment)
+
+    return segments
+
+
+def parse_conll_files(data_paths):
+    """
+    Parse CoNLL formatted files and return list of segments for each file and index
+    the vocabs and tags across all data_paths
+    :param data_paths: tuple(Path) - tuple of filenames
+    :return: tuple( [[(token, tag), ...], [(token, tag), ...]], -> segments for data_paths[i]
+                    [[(token, tag), ...], [(token, tag), ...]], -> segments for data_paths[i+1],
+                    ...
+                  )
+             List of segments for each dataset and each segment has list of (tokens, tags)
+    """
+    vocabs = namedtuple("Vocab", ["tags", "tokens"])
+    datasets, tags, tokens = list(), list(), list()
+
+    for data_path in data_paths:
+        dataset = conll_to_segments(data_path)
+        datasets.append(dataset)
+        tokens += [token.text for segment in dataset for token in segment]
+        tags += [token.gold_tag for segment in dataset for token in segment]
+
+    # Flatten list of tags
+    tags = list(itertools.chain(*tags))
+
+    # Generate vocabs for tags and tokens
+    tag_vocabs = tag_vocab_by_type(tags)
+    tag_vocabs.insert(0, vocab(Counter(tags)))
+    vocabs = vocabs(tokens=vocab(Counter(tokens), specials=["UNK"]), tags=tag_vocabs)
+    return tuple(datasets), vocabs
+
+
+def tag_vocab_by_type(tags):
+    vocabs = list()
+    c = Counter(tags)
+    tag_names = c.keys()
+    tag_types = sorted(list(set([tag.split("-", 1)[1] for tag in tag_names if "-" in tag])))
+
+    for tag_type in tag_types:
+        r = re.compile(".*-" + tag_type)
+        t = list(filter(r.match, tags)) + ["O"]
+        vocabs.append(vocab(Counter(t), specials=["<pad>"]))
+
+    return vocabs
+
+
+def text2segments(text):
+    """
+    Convert text to a datasets and index the tokens
+    """
+    dataset = [[Token(text=token, gold_tag=["O"]) for token in text.split()]]
+    tokens = [token.text for segment in dataset for token in segment]
+
+    # Generate vocabs for the tokens
+    segment_vocab = vocab(Counter(tokens), specials=["UNK"])
+    return dataset, segment_vocab
+
+
+def get_dataloaders(
+    datasets, vocab, data_config, batch_size=32, num_workers=0, shuffle=(True, False, False)
+):
+    """
+    From the datasets generate the dataloaders
+    :param datasets: list - list of the datasets, list of list of segments and tokens
+    :param batch_size: int
+    :param num_workers: int
+    :param shuffle: boolean - to shuffle the data or not
+    :return: List[torch.utils.data.DataLoader]
+    """
+    dataloaders = list()
+
+    for i, examples in enumerate(datasets):
+        data_config["kwargs"].update({"examples": examples, "vocab": vocab})
+        dataset = load_object(data_config["fn"], data_config["kwargs"])
+
+        dataloader = DataLoader(
+            dataset=dataset,
+            shuffle=shuffle[i],
+            batch_size=batch_size,
+            num_workers=num_workers,
+            collate_fn=dataset.collate_fn,
+        )
+
+        logger.info("%s batches found", len(dataloader))
+        dataloaders.append(dataloader)
+
+    return dataloaders
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/utils/helpers.py` & `nlptoolssna-0.9.3/nlptools/arabiner/utils/helpers.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import os
-import sys
-import logging
-import importlib
-import shutil
-import torch
-import pickle
-import json
-import random
-import numpy as np
-from argparse import Namespace
-
-
-def logging_config(log_file=None):
-    """
-    Initialize custom logger
-    :param log_file: str - path to log file, full path
-    :return: None
-    """
-    handlers = [logging.StreamHandler(sys.stdout)]
-
-    if log_file:
-        handlers.append(logging.FileHandler(log_file, "w", "utf-8"))
-        print("Logging to {}".format(log_file))
-
-    logging.basicConfig(
-        level=logging.INFO,
-        handlers=handlers,
-        format="%(levelname)s\t%(name)s\t%(asctime)s\t%(message)s",
-        datefmt="%a, %d %b %Y %H:%M:%S",
-        force=True
-    )
-
-
-def load_object(name, kwargs):
-    """
-    Load objects dynamically given the object name and its arguments
-    :param name: str - object name, class name or function name
-    :param kwargs: dict - keyword arguments
-    :return: object
-    """
-    object_module, object_name = name.rsplit(".", 1)
-    object_module = importlib.import_module(object_module)
-    fn = getattr(object_module, object_name)(**kwargs)
-    return fn
-
-
-def make_output_dirs(path, subdirs=[], overwrite=True):
-    """
-    Create root directory and any other sub-directories
-    :param path: str - root directory
-    :param subdirs: List[str] - list of sub-directories
-    :param overwrite: boolean - to overwrite the directory or not
-    :return: None
-    """
-    if overwrite:
-        shutil.rmtree(path, ignore_errors=True)
-
-    os.makedirs(path)
-
-    for subdir in subdirs:
-        os.makedirs(os.path.join(path, subdir))
-
-
-def load_checkpoint(path):
-    """
-    Load model given the model path
-    :param model_path: str - path to model
-    :return: tagger - arabiner.trainers.BaseTrainer - the tagger model
-             vocab - torchtext.vocab.Vocab - indexed tags
-             train_config - argparse.Namespace - training configurations
-    """
-    _path = os.path.join(path, "tag_vocab.pkl")
-    print('2',_path)
-    with open(_path, "rb") as fh:
-        tag_vocab = pickle.load(fh)
-
-    # Load train configurations from checkpoint
-    train_config = Namespace()
-    args_path = os.path.join(path, "args.json")
-    print('3', args_path)
-    with open(args_path, "r") as fh:
-        train_config.__dict__ = json.load(fh)
-
-    # Initialize the loss function, not used for inference, but evaluation
-    loss = load_object(train_config.loss["fn"], train_config.loss["kwargs"])
-
-    # Load BERT tagger
-    model = load_object(train_config.network_config["fn"], train_config.network_config["kwargs"])
-    model = torch.nn.DataParallel(model)
-
-    if torch.cuda.is_available():
-        model = model.cuda()
-
-    # Update arguments for the tagger
-    # Attach the model, loss (used for evaluations cases)
-    train_config.trainer_config["kwargs"]["model"] = model
-    train_config.trainer_config["kwargs"]["loss"] = loss
-
-    tagger = load_object(train_config.trainer_config["fn"], train_config.trainer_config["kwargs"])
-    tagger.load(os.path.join(path, "checkpoints"))
-    return tagger, tag_vocab, train_config
-
-
-def set_seed(seed):
-    """
-    Set the seed for random intialization and set
-    CUDANN parameters to ensure determmihstic results across
-    multiple runs with the same seed
-
-    :param seed: int
-    """
-    np.random.seed(seed)
-    random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed(seed)
-    torch.cuda.manual_seed_all(seed)
-
-    torch.backends.cudnn.deterministic = True
-    torch.backends.cudnn.benchmark = False
-    torch.backends.cudnn.enabled = False
+import os
+import sys
+import logging
+import importlib
+import shutil
+import torch
+import pickle
+import json
+import random
+import numpy as np
+from argparse import Namespace
+
+
+def logging_config(log_file=None):
+    """
+    Initialize custom logger
+    :param log_file: str - path to log file, full path
+    :return: None
+    """
+    handlers = [logging.StreamHandler(sys.stdout)]
+
+    if log_file:
+        handlers.append(logging.FileHandler(log_file, "w", "utf-8"))
+        print("Logging to {}".format(log_file))
+
+    logging.basicConfig(
+        level=logging.INFO,
+        handlers=handlers,
+        format="%(levelname)s\t%(name)s\t%(asctime)s\t%(message)s",
+        datefmt="%a, %d %b %Y %H:%M:%S",
+        force=True
+    )
+
+
+def load_object(name, kwargs):
+    """
+    Load objects dynamically given the object name and its arguments
+    :param name: str - object name, class name or function name
+    :param kwargs: dict - keyword arguments
+    :return: object
+    """
+    object_module, object_name = name.rsplit(".", 1)
+    object_module = importlib.import_module(object_module)
+    fn = getattr(object_module, object_name)(**kwargs)
+    return fn
+
+
+def make_output_dirs(path, subdirs=[], overwrite=True):
+    """
+    Create root directory and any other sub-directories
+    :param path: str - root directory
+    :param subdirs: List[str] - list of sub-directories
+    :param overwrite: boolean - to overwrite the directory or not
+    :return: None
+    """
+    if overwrite:
+        shutil.rmtree(path, ignore_errors=True)
+
+    os.makedirs(path)
+
+    for subdir in subdirs:
+        os.makedirs(os.path.join(path, subdir))
+
+
+def load_checkpoint(path):
+    """
+    Load model given the model path
+    :param model_path: str - path to model
+    :return: tagger - arabiner.trainers.BaseTrainer - the tagger model
+             vocab - torchtext.vocab.Vocab - indexed tags
+             train_config - argparse.Namespace - training configurations
+    """
+    _path = os.path.join(path, "tag_vocab.pkl")
+    print('2',_path)
+    with open(_path, "rb") as fh:
+        tag_vocab = pickle.load(fh)
+
+    # Load train configurations from checkpoint
+    train_config = Namespace()
+    args_path = os.path.join(path, "args.json")
+    print('3', args_path)
+    with open(args_path, "r") as fh:
+        train_config.__dict__ = json.load(fh)
+
+    # Initialize the loss function, not used for inference, but evaluation
+    loss = load_object(train_config.loss["fn"], train_config.loss["kwargs"])
+
+    # Load BERT tagger
+    model = load_object(train_config.network_config["fn"], train_config.network_config["kwargs"])
+    model = torch.nn.DataParallel(model)
+
+    if torch.cuda.is_available():
+        model = model.cuda()
+
+    # Update arguments for the tagger
+    # Attach the model, loss (used for evaluations cases)
+    train_config.trainer_config["kwargs"]["model"] = model
+    train_config.trainer_config["kwargs"]["loss"] = loss
+
+    tagger = load_object(train_config.trainer_config["fn"], train_config.trainer_config["kwargs"])
+    tagger.load(os.path.join(path, "checkpoints"))
+    return tagger, tag_vocab, train_config
+
+
+def set_seed(seed):
+    """
+    Set the seed for random intialization and set
+    CUDANN parameters to ensure determmihstic results across
+    multiple runs with the same seed
+
+    :param seed: int
+    """
+    np.random.seed(seed)
+    random.seed(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed(seed)
+    torch.cuda.manual_seed_all(seed)
+
+    torch.backends.cudnn.deterministic = True
+    torch.backends.cudnn.benchmark = False
+    torch.backends.cudnn.enabled = False
```

### Comparing `nlptoolssna-0.9.2/nlptools/arabiner/utils/metrics.py` & `nlptoolssna-0.9.3/nlptools/arabiner/utils/metrics.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from seqeval.metrics import (
-    classification_report,
-    precision_score,
-    recall_score,
-    f1_score,
-    accuracy_score,
-)
-from seqeval.scheme import IOB2
-from types import SimpleNamespace
-import logging
-import re
-
-logger = logging.getLogger(__name__)
-
-
-def compute_nested_metrics(segments, vocabs):
-    """
-    Compute metrics for nested NER
-    :param segments: List[List[arabiner.data.dataset.Token]] - list of segments
-    :return: metrics - SimpleNamespace - F1/micro/macro/weights, recall, precision, accuracy
-    """
-    y, y_hat = list(), list()
-
-    # We duplicate the dataset N times, where N is the number of entity types
-    # For each copy, we create y and y_hat
-    # Example: first copy, will create pairs of ground truth and predicted labels for entity type GPE
-    #          another copy will create pairs for LOC, etc.
-    for i, vocab in enumerate(vocabs):
-        vocab_tags = [tag for tag in vocab.get_itos() if "-" in tag]
-        r = re.compile("|".join(vocab_tags))
-
-        y += [[(list(filter(r.match, token.gold_tag)) or ["O"])[0] for token in segment] for segment in segments]
-        y_hat += [[token.pred_tag[i]["tag"] for token in segment] for segment in segments]
-
-    logging.info("\n" + classification_report(y, y_hat, scheme=IOB2, digits=4))
-
-    metrics = {
-        "micro_f1": f1_score(y, y_hat, average="micro", scheme=IOB2),
-        "macro_f1": f1_score(y, y_hat, average="macro", scheme=IOB2),
-        "weights_f1": f1_score(y, y_hat, average="weighted", scheme=IOB2),
-        "precision": precision_score(y, y_hat, scheme=IOB2),
-        "recall": recall_score(y, y_hat, scheme=IOB2),
-        "accuracy": accuracy_score(y, y_hat),
-    }
-
-    return SimpleNamespace(**metrics)
-
-
-def compute_single_label_metrics(segments):
-    """
-    Compute metrics for flat NER
-    :param segments: List[List[arabiner.data.dataset.Token]] - list of segments
-    :return: metrics - SimpleNamespace - F1/micro/macro/weights, recall, precision, accuracy
-    """
-    y = [[token.gold_tag[0] for token in segment] for segment in segments]
-    y_hat = [[token.pred_tag[0]["tag"] for token in segment] for segment in segments]
-
-    logging.info("\n" + classification_report(y, y_hat, scheme=IOB2))
-
-    metrics = {
-        "micro_f1": f1_score(y, y_hat, average="micro", scheme=IOB2),
-        "macro_f1": f1_score(y, y_hat, average="macro", scheme=IOB2),
-        "weights_f1": f1_score(y, y_hat, average="weighted", scheme=IOB2),
-        "precision": precision_score(y, y_hat, scheme=IOB2),
-        "recall": recall_score(y, y_hat, scheme=IOB2),
-        "accuracy": accuracy_score(y, y_hat),
-    }
-
-    return SimpleNamespace(**metrics)
+from seqeval.metrics import (
+    classification_report,
+    precision_score,
+    recall_score,
+    f1_score,
+    accuracy_score,
+)
+from seqeval.scheme import IOB2
+from types import SimpleNamespace
+import logging
+import re
+
+logger = logging.getLogger(__name__)
+
+
+def compute_nested_metrics(segments, vocabs):
+    """
+    Compute metrics for nested NER
+    :param segments: List[List[arabiner.data.dataset.Token]] - list of segments
+    :return: metrics - SimpleNamespace - F1/micro/macro/weights, recall, precision, accuracy
+    """
+    y, y_hat = list(), list()
+
+    # We duplicate the dataset N times, where N is the number of entity types
+    # For each copy, we create y and y_hat
+    # Example: first copy, will create pairs of ground truth and predicted labels for entity type GPE
+    #          another copy will create pairs for LOC, etc.
+    for i, vocab in enumerate(vocabs):
+        vocab_tags = [tag for tag in vocab.get_itos() if "-" in tag]
+        r = re.compile("|".join(vocab_tags))
+
+        y += [[(list(filter(r.match, token.gold_tag)) or ["O"])[0] for token in segment] for segment in segments]
+        y_hat += [[token.pred_tag[i]["tag"] for token in segment] for segment in segments]
+
+    logging.info("\n" + classification_report(y, y_hat, scheme=IOB2, digits=4))
+
+    metrics = {
+        "micro_f1": f1_score(y, y_hat, average="micro", scheme=IOB2),
+        "macro_f1": f1_score(y, y_hat, average="macro", scheme=IOB2),
+        "weights_f1": f1_score(y, y_hat, average="weighted", scheme=IOB2),
+        "precision": precision_score(y, y_hat, scheme=IOB2),
+        "recall": recall_score(y, y_hat, scheme=IOB2),
+        "accuracy": accuracy_score(y, y_hat),
+    }
+
+    return SimpleNamespace(**metrics)
+
+
+def compute_single_label_metrics(segments):
+    """
+    Compute metrics for flat NER
+    :param segments: List[List[arabiner.data.dataset.Token]] - list of segments
+    :return: metrics - SimpleNamespace - F1/micro/macro/weights, recall, precision, accuracy
+    """
+    y = [[token.gold_tag[0] for token in segment] for segment in segments]
+    y_hat = [[token.pred_tag[0]["tag"] for token in segment] for segment in segments]
+
+    logging.info("\n" + classification_report(y, y_hat, scheme=IOB2))
+
+    metrics = {
+        "micro_f1": f1_score(y, y_hat, average="micro", scheme=IOB2),
+        "macro_f1": f1_score(y, y_hat, average="macro", scheme=IOB2),
+        "weights_f1": f1_score(y, y_hat, average="weighted", scheme=IOB2),
+        "precision": precision_score(y, y_hat, scheme=IOB2),
+        "recall": recall_score(y, y_hat, scheme=IOB2),
+        "accuracy": accuracy_score(y, y_hat),
+    }
+
+    return SimpleNamespace(**metrics)
```

### Comparing `nlptoolssna-0.9.2/nlptools/morphology/charsets.py` & `nlptoolssna-0.9.3/nlptools/morphology/charsets.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# -*- coding: utf-8 -*-
-# We acknoledge that this file  charsets.py is imported from Camel tools citation. url
-#
-
-import unicodedata
-
-from six import unichr
-
-
-UNICODE_PUNCT_CHARSET = frozenset(
-    [unichr(x) for x in range(65536) if unicodedata.category(
-        unichr(x))[0] == 'P'])
-UNICODE_SYMBOL_CHARSET = frozenset(
-    [unichr(x) for x in range(65536) if unicodedata.category(
-        unichr(x))[0] == 'S'])
-UNICODE_PUNCT_SYMBOL_CHARSET = UNICODE_PUNCT_CHARSET | UNICODE_SYMBOL_CHARSET
-
-UNICODE_LETTER_CHARSET = frozenset(
-    [unichr(x) for x in range(65536) if unicodedata.category(
-        unichr(x))[0] == 'L'])
-UNICODE_MARK_CHARSET = frozenset(
-    [unichr(x) for x in range(65536) if unicodedata.category(
-        unichr(x))[0] == 'M'])
-UNICODE_NUMBER_CHARSET = frozenset(
-    [unichr(x) for x in range(65536) if unicodedata.category(
-        unichr(x))[0] == 'N'])
-UNICODE_LETTER_MARK_NUMBER_CHARSET = (UNICODE_LETTER_CHARSET |
-                                      UNICODE_MARK_CHARSET |
-                                      UNICODE_NUMBER_CHARSET)
-
-AR_LETTERS_CHARSET = frozenset(u'\u0621\u0622\u0623\u0624\u0625\u0626\u0627'
-                               u'\u0628\u0629\u062a\u062b\u062c\u062d\u062e'
-                               u'\u062f\u0630\u0631\u0632\u0633\u0634\u0635'
-                               u'\u0636\u0637\u0638\u0639\u063a\u0640\u0641'
-                               u'\u0642\u0643\u0644\u0645\u0646\u0647\u0648'
-                               u'\u0649\u064a\u0671\u067e\u0686\u06a4\u06af')
-AR_DIAC_CHARSET = frozenset(u'\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652'
-                            u'\u0670\u0640')
-AR_CHARSET = AR_LETTERS_CHARSET | AR_DIAC_CHARSET
-
-BW_LETTERS_CHARSET = frozenset(u'$&\'*<>ADEGHJPSTVYZ_bdfghjklmnpqrstvwxyz{|}')
-BW_DIAC_CHARSET = frozenset(u'FKN`aiou~_')
-BW_CHARSET = BW_LETTERS_CHARSET | BW_DIAC_CHARSET
-
-SAFEBW_LETTERS_CHARSET = frozenset(u'ABCDEGHIJLMOPQSTVWYZ_bcdefghjklmnpqrstvwx'
-                                   u'yz')
-SAFEBW_DIAC_CHARSET = frozenset(u'FKNaeiou~_')
-SAFEBW_CHARSET = SAFEBW_LETTERS_CHARSET | SAFEBW_DIAC_CHARSET
-
-XMLBW_LETTERS_CHARSET = frozenset(u'$\'*ABDEGHIJOPSTWYZ_bdfghjklmnpqrstvwxyz{|'
-                                  u'}')
-XMLBW_DIAC_CHARSET = frozenset(u'FKN`aiou~_')
-XMLBW_CHARSET = XMLBW_LETTERS_CHARSET | XMLBW_DIAC_CHARSET
-
-HSB_LETTERS_CHARSET = frozenset(u'\'ADHST_bcdfghjklmnpqrstvwxyz'
-                                u'\u00c2\u00c4\u00e1\u00f0\u00fd\u0100\u0102'
-                                u'\u010e\u0127\u0161\u0175\u0177\u03b3\u03b8'
-                                u'\u03c2')
-HSB_DIAC_CHARSET = frozenset(u'.aiu~\u00c4\u00e1\u00e3\u0129\u0169_')
-HSB_CHARSET = HSB_LETTERS_CHARSET | HSB_DIAC_CHARSET
+# -*- coding: utf-8 -*-
+# We acknoledge that this file  charsets.py is imported from Camel tools citation. url
+#
+
+import unicodedata
+
+from six import unichr
+
+
+UNICODE_PUNCT_CHARSET = frozenset(
+    [unichr(x) for x in range(65536) if unicodedata.category(
+        unichr(x))[0] == 'P'])
+UNICODE_SYMBOL_CHARSET = frozenset(
+    [unichr(x) for x in range(65536) if unicodedata.category(
+        unichr(x))[0] == 'S'])
+UNICODE_PUNCT_SYMBOL_CHARSET = UNICODE_PUNCT_CHARSET | UNICODE_SYMBOL_CHARSET
+
+UNICODE_LETTER_CHARSET = frozenset(
+    [unichr(x) for x in range(65536) if unicodedata.category(
+        unichr(x))[0] == 'L'])
+UNICODE_MARK_CHARSET = frozenset(
+    [unichr(x) for x in range(65536) if unicodedata.category(
+        unichr(x))[0] == 'M'])
+UNICODE_NUMBER_CHARSET = frozenset(
+    [unichr(x) for x in range(65536) if unicodedata.category(
+        unichr(x))[0] == 'N'])
+UNICODE_LETTER_MARK_NUMBER_CHARSET = (UNICODE_LETTER_CHARSET |
+                                      UNICODE_MARK_CHARSET |
+                                      UNICODE_NUMBER_CHARSET)
+
+AR_LETTERS_CHARSET = frozenset(u'\u0621\u0622\u0623\u0624\u0625\u0626\u0627'
+                               u'\u0628\u0629\u062a\u062b\u062c\u062d\u062e'
+                               u'\u062f\u0630\u0631\u0632\u0633\u0634\u0635'
+                               u'\u0636\u0637\u0638\u0639\u063a\u0640\u0641'
+                               u'\u0642\u0643\u0644\u0645\u0646\u0647\u0648'
+                               u'\u0649\u064a\u0671\u067e\u0686\u06a4\u06af')
+AR_DIAC_CHARSET = frozenset(u'\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652'
+                            u'\u0670\u0640')
+AR_CHARSET = AR_LETTERS_CHARSET | AR_DIAC_CHARSET
+
+BW_LETTERS_CHARSET = frozenset(u'$&\'*<>ADEGHJPSTVYZ_bdfghjklmnpqrstvwxyz{|}')
+BW_DIAC_CHARSET = frozenset(u'FKN`aiou~_')
+BW_CHARSET = BW_LETTERS_CHARSET | BW_DIAC_CHARSET
+
+SAFEBW_LETTERS_CHARSET = frozenset(u'ABCDEGHIJLMOPQSTVWYZ_bcdefghjklmnpqrstvwx'
+                                   u'yz')
+SAFEBW_DIAC_CHARSET = frozenset(u'FKNaeiou~_')
+SAFEBW_CHARSET = SAFEBW_LETTERS_CHARSET | SAFEBW_DIAC_CHARSET
+
+XMLBW_LETTERS_CHARSET = frozenset(u'$\'*ABDEGHIJOPSTWYZ_bdfghjklmnpqrstvwxyz{|'
+                                  u'}')
+XMLBW_DIAC_CHARSET = frozenset(u'FKN`aiou~_')
+XMLBW_CHARSET = XMLBW_LETTERS_CHARSET | XMLBW_DIAC_CHARSET
+
+HSB_LETTERS_CHARSET = frozenset(u'\'ADHST_bcdfghjklmnpqrstvwxyz'
+                                u'\u00c2\u00c4\u00e1\u00f0\u00fd\u0100\u0102'
+                                u'\u010e\u0127\u0161\u0175\u0177\u03b3\u03b8'
+                                u'\u03c2')
+HSB_DIAC_CHARSET = frozenset(u'.aiu~\u00c4\u00e1\u00e3\u0129\u0169_')
+HSB_CHARSET = HSB_LETTERS_CHARSET | HSB_DIAC_CHARSET
```

### Comparing `nlptoolssna-0.9.2/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.9.3/nlptools/morphology/morph_analyzer.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-
-from nlptools.morphology import settings 
-import re
-from nlptools.morphology.tokenizers_words import simple_word_tokenize
-from nlptools.utils.parser import arStrip
-from nlptools.morphology.charsets import AR_CHARSET, AR_DIAC_CHARSET
-
-_IS_AR_RE = re.compile(u'^[' + re.escape(u''.join(AR_CHARSET)) + u']+$')
-def find_solution(token, language, task):
-    """
-    Given a token, this method finds the morphological solution lemma and/or pos based on a spesific language and task.
-          
-    Args:
-        token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
-        language (:obj:`str`): In the current version, `MSA` is only supported. 
-        task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
-
-    Returns:
-        list (:obj:`list`): A list of [token, lemma, pos], where:
-           token: the original input token
-           lemma: the lemma of the token 
-           pos: the part-of-speech of the token 
-    Note:
-        If no sloution is found for this token, an empty list is returned.
-    """
-    if token in settings.div_dic.keys():
-        soluation = settings.div_dic[token]
-        return  [token, soluation[0], soluation[1]]               
-    else:
-        return []
-
-def analyze(text, language ='MSA', task ='full'):
-   """
-    This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that,
-    if:
-        the task is lemmatizer, then the morphological soltuion is only the lemma.
-        the task is pos, then the morphological soltuion is only the pos.
-        the task is full, the the morphological soltuion is both the lemma and the pos.
-     
-    Args:
-        token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
-        language (:obj:`str`): In the current version, `MSA` is only supported. 
-        task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
-         
-    Returns:
-        list (:obj:`list`): A list of [token, lemma, pos], based on the spesified task, where:
-           token: the original input token
-           lemma: the lemma of the token 
-           pos: the part-of-speech of the token 
-
-    **Example:**
-
-     .. highlight:: python
-     .. code-block:: python
-     
-          from nlptools.morphology  import morph_analyzer
-     
-          Return the morpological solution for each token in this text
-          Exampel: task = full 
-          morph_analyzer.analyze('ذهب الولد الى المدرسة')
-           
-           [['ذهب', 'ذَهَبَ۪ 1', 'فعل'],
-           ['الولد', 'وَلَد 1', 'اسم'],
-           ['الى', 'إِلَى 1', 'كلمة وظيفية'],
-           ['المدرسة', 'مَدْرَسَة 1', 'اسم']]
-
-           Exampel: task = pos
-           morph_analyzer.analyze('ذهب الولد الى المدرسة',task='pos')
-           #the output
-           [['ذهب', 'فعل'], ['الولد', 'اسم'], ['الى', 'كلمة وظيفية'], ['المدرسة', 'اسم']]
-
-           Exampel: task = lemmatizer
-           morph_analyzer.analyze('طار العصور فوق الشجرة', task='lemmatizer')
-           [['طار', 'طارِ۪ 1'],
-            ['العصور', 'عَصْر 1'],
-            ['فوق', 'فَوْق 1'],
-            ['الشجرة', 'شَجَرَة 1']]
-     """
- 
-   #@check if the init does not load data correctly, call load_alma inside
-   output_list = []
-
-   tokens = simple_word_tokenize(text)
-
-   for token in tokens:
-         result_token =[]
-         token = arStrip(token , False , True , False , False , False , False) 
-         token = re.sub('[ٱ]','ﺍ',token)
-         solution=[token, token+"_0",""]
-
-         if token.isdigit():
-            solution[2] = "digit" #pos
-
-         elif not _is_ar(token):
-            solution[2] = "Foreign" #pos
-
-        #  elif re.match("^[a-zA-Z]*$", token): 
-        #     solution[2] = "Foreign" #pos
-
-         else:
-            result_token = find_solution(token,language, task)
-            
-            if result_token == []:
-               token_without_al = re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token))
-               if len(token_without_al) > 5  :
-                  result_token = find_solution(token_without_al, language, task)
-
-            if result_token == []:
-              # try with replace ﻩ with ﺓ
-               result_token = find_solution(re.sub(r'[ﻩ]$','ﺓ',token), language, task)
-               
-
-            if result_token == []:
-               # try with unify Alef
-               word_with_unify_alef = arStrip(token , False , False , False , False , True , False) # Unify Alef
-               result_token = find_solution(word_with_unify_alef, language, task)
-            
-            if result_token == []:
-               # try with remove diac
-               word_undiac = arStrip(token , True , False , True , True , False , False) # remove diacs, shaddah ,  digit
-               result_token = find_solution(word_undiac, language, task)
-
-            if result_token == []:
-               # try with remove diac and unify alef
-               word_undiac = arStrip(token , True , True , True , False, True , False) # diacs , smallDiacs , shaddah ,  alif
-               result_token = find_solution(word_undiac, language, task)
-
-         if result_token != []:
-               
-               output_list.append(result_token)
-         else:
-            # if no solution is found
-            output_list.append(solution)
-        
-   return filter_results(task, output_list)
-
-
-def filter_results(task, lst):
-    if task == 'lemmatizer':
-        return remove_items_by_index(lst, [2])
-    elif task == 'pos':
-        return remove_items_by_index(lst, [1])
-    else: 
-        return lst
-
-
-def remove_items_by_index(lst, index_list):
-    for inner_list in lst:
-        for index in sorted(index_list, reverse=True):
-            if len(inner_list) > index:
-                inner_list.pop(index)
-    return lst
-
-
-def _is_ar(word):
-    return _IS_AR_RE.match(word) is not None       
-        
-
-  
-  
-  
-    
-    
-    
-    
-    
+
+from nlptools.morphology import settings 
+import re
+from nlptools.morphology.tokenizers_words import simple_word_tokenize
+from nlptools.utils.parser import arStrip
+from nlptools.morphology.charsets import AR_CHARSET, AR_DIAC_CHARSET
+
+_IS_AR_RE = re.compile(u'^[' + re.escape(u''.join(AR_CHARSET)) + u']+$')
+def find_solution(token, language, task):
+    """
+    Given a token, this method finds the morphological solution lemma and/or pos based on a spesific language and task.
+          
+    Args:
+        token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
+        language (:obj:`str`): In the current version, `MSA` is only supported. 
+        task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
+
+    Returns:
+        list (:obj:`list`): A list of [token, lemma, pos], where:
+           token: the original input token
+           lemma: the lemma of the token 
+           pos: the part-of-speech of the token 
+    Note:
+        If no sloution is found for this token, an empty list is returned.
+    """
+    if token in settings.div_dic.keys():
+        soluation = settings.div_dic[token]
+        return  [token, soluation[0], soluation[1]]               
+    else:
+        return []
+
+def analyze(text, language ='MSA', task ='full'):
+   """
+    This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that,
+    if:
+        the task is lemmatizer, then the morphological soltuion is only the lemma.
+        the task is pos, then the morphological soltuion is only the pos.
+        the task is full, the the morphological soltuion is both the lemma and the pos.
+     
+    Args:
+        token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
+        language (:obj:`str`): In the current version, `MSA` is only supported. 
+        task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
+         
+    Returns:
+        list (:obj:`list`): A list of [token, lemma, pos], based on the spesified task, where:
+           token: the original input token
+           lemma: the lemma of the token 
+           pos: the part-of-speech of the token 
+
+    **Example:**
+
+     .. highlight:: python
+     .. code-block:: python
+     
+          from nlptools.morphology  import morph_analyzer
+     
+          Return the morpological solution for each token in this text
+          Exampel: task = full 
+          morph_analyzer.analyze('ذهب الولد الى المدرسة')
+           
+           [['ذهب', 'ذَهَبَ۪ 1', 'فعل'],
+           ['الولد', 'وَلَد 1', 'اسم'],
+           ['الى', 'إِلَى 1', 'كلمة وظيفية'],
+           ['المدرسة', 'مَدْرَسَة 1', 'اسم']]
+
+           Exampel: task = pos
+           morph_analyzer.analyze('ذهب الولد الى المدرسة',task='pos')
+           #the output
+           [['ذهب', 'فعل'], ['الولد', 'اسم'], ['الى', 'كلمة وظيفية'], ['المدرسة', 'اسم']]
+
+           Exampel: task = lemmatizer
+           morph_analyzer.analyze('طار العصور فوق الشجرة', task='lemmatizer')
+           [['طار', 'طارِ۪ 1'],
+            ['العصور', 'عَصْر 1'],
+            ['فوق', 'فَوْق 1'],
+            ['الشجرة', 'شَجَرَة 1']]
+     """
+ 
+   #@check if the init does not load data correctly, call load_alma inside
+   output_list = []
+
+   tokens = simple_word_tokenize(text)
+
+   for token in tokens:
+         result_token =[]
+         token = arStrip(token , False , True , False , False , False , False) 
+         token = re.sub('[ٱ]','ﺍ',token)
+         solution=[token, token+"_0",""]
+
+         if token.isdigit():
+            solution[2] = "digit" #pos
+
+         elif not _is_ar(token):
+            solution[2] = "Foreign" #pos
+
+        #  elif re.match("^[a-zA-Z]*$", token): 
+        #     solution[2] = "Foreign" #pos
+
+         else:
+            result_token = find_solution(token,language, task)
+            
+            if result_token == []:
+               token_without_al = re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token))
+               if len(token_without_al) > 5  :
+                  result_token = find_solution(token_without_al, language, task)
+
+            if result_token == []:
+              # try with replace ﻩ with ﺓ
+               result_token = find_solution(re.sub(r'[ﻩ]$','ﺓ',token), language, task)
+               
+
+            if result_token == []:
+               # try with unify Alef
+               word_with_unify_alef = arStrip(token , False , False , False , False , True , False) # Unify Alef
+               result_token = find_solution(word_with_unify_alef, language, task)
+            
+            if result_token == []:
+               # try with remove diac
+               word_undiac = arStrip(token , True , False , True , True , False , False) # remove diacs, shaddah ,  digit
+               result_token = find_solution(word_undiac, language, task)
+
+            if result_token == []:
+               # try with remove diac and unify alef
+               word_undiac = arStrip(token , True , True , True , False, True , False) # diacs , smallDiacs , shaddah ,  alif
+               result_token = find_solution(word_undiac, language, task)
+
+         if result_token != []:
+               
+               output_list.append(result_token)
+         else:
+            # if no solution is found
+            output_list.append(solution)
+        
+   return filter_results(task, output_list)
+
+
+def filter_results(task, lst):
+    if task == 'lemmatizer':
+        return remove_items_by_index(lst, [2])
+    elif task == 'pos':
+        return remove_items_by_index(lst, [1])
+    else: 
+        return lst
+
+
+def remove_items_by_index(lst, index_list):
+    for inner_list in lst:
+        for index in sorted(index_list, reverse=True):
+            if len(inner_list) > index:
+                inner_list.pop(index)
+    return lst
+
+
+def _is_ar(word):
+    return _IS_AR_RE.match(word) is not None       
+        
+
+  
+  
+  
+    
+    
+    
+    
+
```

### Comparing `nlptoolssna-0.9.2/nlptools/salma/views.py` & `nlptoolssna-0.9.3/nlptools/salma/views.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,419 +1,419 @@
-# ./bookstore_app/api/views.py
-import django
-django.setup()
-import requests
-import json
-from django.http import JsonResponse
-from rest_framework.decorators import api_view
-from salma import settings 
-# Comented by tymaa to Run service via GPU
-#from salma.word_sense_disambiguation import word_sense
-from salma.word_sense_disambiguation import normalizearabert
-from salma.word_sense_disambiguation import load_data_model
-from salma.word_sense_disambiguation import GlossPredictor
-from salma.parser import arStrip
-from salma.parser import removePunctuation
-from salma.parser import removeEnglish
-from salma.tokenizers_words import simple_word_tokenize
-from ALMA_multi_word_service.views import ALMA_multi_word
-import re
-import numpy as np
-from arabiner.bin import infer
-from api_clients_counter_month.ApikeyValidation import checkApikey
-from ApiTrackingService.InsertApiLog import insertLog
-import multiprocessing
-from functools import partial
-from lemmatizer_v2_DB.views import lemmatize_sentence
-from arabiner.views import NER
-
-# Added By Tymaa: 2023-02-05 to call GlossPredictor as a web service from GPU machine 
-#from urllib.request import Request, urlopen
-
-def delete_form_list(position, word_lemma):
-    tmp_word_lemma = [] 
-    output = []
-    for wordLemma in word_lemma:
-        if position == int(wordLemma[2]): # start 
-           word = wordLemma[0]
-           gloss = wordLemma[1]
-           position = int(wordLemma[3]) 
-           concept_count = int(wordLemma[4]) 
-           undiac_multi_word_lemma = wordLemma[5]
-           multi_word_lemma = wordLemma[6]
-           output.append([word, gloss, concept_count, undiac_multi_word_lemma, multi_word_lemma])# word
-        elif position < int(wordLemma[2]): 
-           tmp_word_lemma.append(wordLemma)
-    return tmp_word_lemma, output, position
-    #return output
-
-def find_two_word_lemma(input_sentence):
-    i = 0
-    output = []
-    length = len(input_sentence)
-    while i < length - 1:
-        two_grams = input_sentence[i] +" "+ input_sentence[i + 1] 
-      #   r = requests.get("https://ontology.birzeit.edu/sina/v2/api/ALMA_multi_wordDB/"+two_grams+"?apikey=samplekey", verify=False)
-      #   data = json.loads(r.text)
-        data = ALMA_multi_word(two_grams,2)
-        try :
-            # found two_grams
-            found_2Word_lemma = [two_grams,data[0]['glosses'], i, i + 1,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
-            output.append(found_2Word_lemma) 
-            i = i + 1    
-        except: # no record found on this multi_lema
-            i = i + 1 
-    return output
-
-
-def find_three_word_lemma(input_sentence):
-    i = 0
-    output = []
-    length = len(input_sentence)
-    while i < length - 2:
-        three_grams = input_sentence[i] +" "+ input_sentence[i + 1] + " "+ input_sentence[i + 2]
-        #r = requests.get("https://ontology.birzeit.edu/sina/v2/api/ALMA_multi_wordDB/"+three_grams+"?apikey=samplekey", verify=False)
-        #data = json.loads(r.text) 
-        data = ALMA_multi_word(three_grams,3)
-        try:
-           found_3Word_lemma = [three_grams, data[0]['glosses'], i, i + 2,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
-           output.append(found_3Word_lemma) 
-           i = i + 1    
-        except:  
-           i = i + 1 
-    return output
-
-def find_four_word_lemma(input_sentence):
-   i = 0
-   output = []
-   length = len(input_sentence)
-   while i < length - 3:
-      four_grams = input_sentence[i] +" "+ input_sentence[i + 1] + " "+ input_sentence[i + 2] + " "+ input_sentence[i + 3]
-      data = ALMA_multi_word(four_grams,4)
-      try:
-         found_4Word_lemma = [four_grams, data[0]['glosses'], i, i + 3,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
-         output.append(found_4Word_lemma) 
-         i = i + 1    
-      except:  
-         i = i + 1 
-   return output
-
-
-def find_five_word_lemma(input_sentence):
-   i = 0
-   output = []
-   length = len(input_sentence)
-   while i < length - 4:
-      five_grams = input_sentence[i] +" "+ input_sentence[i + 1] + " "+ input_sentence[i + 2] + " "+ input_sentence[i + 3] + " "+ input_sentence[i + 4]
-      data = ALMA_multi_word(five_grams,5)
-      try:
-         found_5Word_lemma = [five_grams, data[0]['glosses'], i, i + 4,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
-         output.append(found_5Word_lemma) 
-         i = i + 1    
-      except:  
-         i = i + 1 
-   return output
-
-def find_named_entities(string):
-   found_entities = []
-   entites = NER(string, "4")
-   tag_gloss = {
-      "PERS": "اسم شخص",
-      "ORG": "اسم مؤسسة",
-      #"NORP": "مجموعة من الناس", 
-      #"OCC": "منصب/مسمى وظيفي",
-      "LOC": "اسم منطقة جغرافية",
-      "FAC": "اسم لمَعلَم",
-      #"EVENT": "حدث",
-      "DATE": "فترة زمنية تدل على تاريخ",
-      "UNIT": "وحدة قياس",
-      "CURR": "عملة",
-      "GPE": "اسم بلد، له حدود إدارية/جيوسياسية",
-      "TIME": "فترة زمنية تدل على الوقت",
-      "CARDINAL": "عدد يدل على معدود",
-      "ORDINAL": "رقم، لا يدل على معدود",
-      "PERCENT": "نسبة مئوية",
-      "QUANTITY": "كمية",
-      "MONEY": "مبلغ مالي",
-      "LANGUAGE": "اسم للغة طبيعية",
-      "PRODUCT": "اسم منتج",
-      "LAW": "قانون"
-   }
-
-   for entity in entites:
-      gloss_ner = ""
-      if entity[1] in tag_gloss.keys():
-         gloss_ner = tag_gloss[entity[1]]  
-
-      if gloss_ner != "":
-         gloss = [{'concept_id': '', 'resource_id': '', 'resource_name': '', 'gloss': gloss_ner}]   
-         entity = [entity[0],gloss,int(entity[2]), int(entity[3]),1,arStrip(entity[0],True,True,True,False,True,False),entity[0]]   
-         found_entities.append(entity)
-   #print("list : ",found_entities)
-   return found_entities   
-
-
-def find_glosses_using_ALMA(word):
-   #r = requests.post('https://ontology.birzeit.edu/sina/v2/api/ALMADB/', json= {"sentence":word}, verify=False)
-   #data = json.loads(r.text)
-   data = lemmatize_sentence(word)
-   Diac_lemma = ""
-   pos = ""
-   Undiac_lemma = ""
-   glosses = []
-   #for values in data['resp']: ### Think about bugs in lemmatizer .ex: connection error...
-   Diac_lemma = data[0][1]
-   pos = data[0][2]
-   Undiac_lemma = arStrip(Diac_lemma, True, True, True, True, True, False) # Remove diacs , smallDiacs , shaddah ,  digit , alif , specialChars
-   glosses = data[0][4]
-   concept_count = data[0][3]
-   return word, Undiac_lemma, Diac_lemma, pos , concept_count, glosses
-   
-def disambiguate_glosses_using_SALMA(glosses, Diac_lemma, Undiac_lemma, word, sentence):
-   word = normalizearabert(word)
-   #print(" word After normalized : ", word)
-   glosses_dictionary = {}
-   if glosses != None:
-      for gloss in glosses:
-         # result = json.loads(gloss)
-         glosses_dictionary.update({gloss['concept_id'] : gloss['gloss']})
-      # Commented by Tymaa (2023-02-05) to call GlossPredictor as a web service from GPU machine 
-      print(" Before GlossPredictor on word = ", word)
-      concept_id, gloss = GlossPredictor(Diac_lemma, Undiac_lemma,word,sentence,glosses_dictionary)
-      print(" After GlossPredictor on word = ", word, " Concept_id : ", concept_id, " gloss : ", gloss)
-
-
-      # Added By Tymaa: 2023-02-05 to call GlossPredictor as a web service from GPU machine 
-      #data = {}
-      #data["Diac_lemma"] = Diac_lemma 
-      #data["Undiac_lemma"] = Undiac_lemma
-      #data["word"] = word
-      #data["sentence"] = sentence
-      #data["glosses_dictionary"] = glosses_dictionary
-      #print("Data : ", data)
-      #data = json.dumps(data).encode('utf8')
-      #req = Request(
-      #      url="http://185.19.228.221:8000/word_sense_disambiguation/",
-      #      data=data,
-      #      headers={'User-Agent': 'Mozilla/5.0', 'Content-Type': 'application/json'},
-      #      method='POST'
-      #)
-      #print("url decode : ", urlopen(req).read().decode())
-      #webpage = urlopen(req).read().decode()
-      #concept_id = json.loads(webpage)['concept_id']
-      #gloss = json.loads(webpage)['Gloss']
-
-      #url = "http://185.19.228.221:8000/word_sense_disambiguation/"
-      
-      #data = json.dumps(data).encode('utf8')
-      #print("encode data: " , data)
-      #response = requests.post(url, data=data, headers={'User-Agent': 'Mozilla/5.0', 'Content-Type': 'application/json'})
-      #print(response.status_code)
-      #if response.status_code == 200:
-      #    resp_text = json.loads(response.text)
-      #    concept_id = resp_text["concept_id"]
-      #    gloss = resp_text["Gloss"]  
-      #else:
-      #    concept_id = None
-      #    gloss = None
-      ##
-
-      my_json = {}    
-      my_json['Concept_id'] = concept_id
-      my_json['Gloss'] = gloss
-      my_json['word'] = word
-      my_json['Undiac_lemma'] = Undiac_lemma
-      my_json['Diac_lemma'] = Diac_lemma
-      return my_json
-   else:
-      #print(" word with gloss = None ", word)
-      my_json = {}    
-      my_json['word'] = word
-      my_json['Undiac_lemma'] = Undiac_lemma
-      my_json['Diac_lemma'] = Diac_lemma
-      return my_json
-
-
-
-
-def find_glosses(input_sentence, three_word_lemma, two_word_lemma, four_word_lemma, five_word_lemma, ner):
-      output_list = []
-      position = 0
-      while position < len(input_sentence):    
-         flag = "False"
-         output_from5word = delete_form_list(position, five_word_lemma)
-         five_word_lemma = output_from5word[0]
-         if output_from5word[1] != []: # output
-            position = output_from5word[2]  
-            flag = "True"
-            my_json = {}    
-            my_json['word'] = output_from5word[1][0][0]
-            my_json['concept_count'] = output_from5word[1][0][2]
-            my_json['glosses'] = output_from5word[1][0][1]
-            my_json['Diac_lemma'] = output_from5word[1][0][4]
-            my_json['Undiac_lemma'] = output_from5word[1][0][3]
-            output_list.append(my_json)
-            position = position + 1                
-
-
-
-         output_from4word = delete_form_list(position, four_word_lemma)
-         four_word_lemma = output_from4word[0]
-         if output_from4word[1] != []: # output
-            position = output_from4word[2]  
-            flag = "True"
-            my_json = {}    
-            my_json['word'] = output_from4word[1][0][0]
-            my_json['concept_count'] = output_from4word[1][0][2]
-            my_json['glosses'] = output_from4word[1][0][1]
-            my_json['Diac_lemma'] = output_from4word[1][0][4]
-            my_json['Undiac_lemma'] = output_from4word[1][0][3]
-            output_list.append(my_json)
-            position = position + 1                
-         
-         output_from3word = delete_form_list(position, three_word_lemma)
-         three_word_lemma = output_from3word[0]
-         if output_from3word[1] != []: # output
-            position = output_from3word[2]  
-            flag = "True"
-            my_json = {}    
-            my_json['word'] = output_from3word[1][0][0]
-            my_json['concept_count'] = output_from3word[1][0][2]
-            my_json['glosses'] = output_from3word[1][0][1]
-            my_json['Diac_lemma'] = output_from3word[1][0][4]
-            my_json['Undiac_lemma'] = output_from3word[1][0][3]
-            output_list.append(my_json)
-            position = position + 1                
-
-
-
-         output_from2Word = delete_form_list(position, two_word_lemma)
-         two_word_lemma = output_from2Word[0] 
-         if output_from2Word[1] != []:  
-            position = output_from2Word[2]
-            flag = "True"
-            my_json = {}    
-            word = output_from2Word[1][0][0]
-            my_json['word'] = word
-            my_json['concept_count'] = output_from2Word[1][0][2]
-            my_json['glosses'] = output_from2Word[1][0][1]
-            my_json['Diac_lemma'] = output_from2Word[1][0][4]
-            my_json['Undiac_lemma'] = output_from2Word[1][0][3] 
-            output_list.append(my_json)
-            position = position + 1                 
-               
-
-
-         output_from_ner = delete_form_list(position, ner)
-         ner = output_from_ner[0] 
-         if output_from_ner[1] != []:  
-            position = output_from_ner[2]
-            flag = "True"
-            my_json = {}    
-            word = output_from_ner[1][0][0]
-            my_json['word'] = word
-            my_json['concept_count'] = output_from_ner[1][0][2]
-            my_json['glosses'] = output_from_ner[1][0][1]
-            my_json['Diac_lemma'] = output_from_ner[1][0][4]
-            my_json['Undiac_lemma'] = output_from_ner[1][0][3] 
-            output_list.append(my_json)
-            position = position + 1                             
-         
-         if flag == "False": # Not found in ner or in multi_word_dictionary, ASK ALMA 
-            word = input_sentence[position]
-            word, Undiac_lemma, Diac_lemma, pos , concept_count, glosses = find_glosses_using_ALMA(word)   
-            my_json = {}    
-            my_json['word'] = word
-            my_json['concept_count'] = concept_count
-            my_json['glosses'] = glosses
-            my_json['Diac_lemma'] = Diac_lemma
-            my_json['Undiac_lemma'] = Undiac_lemma
-            output_list.append(my_json)
-            position = position + 1  
-      return output_list                    
-
-def disambiguate_glosses_main(word, sentence):
-   concept_count = word['concept_count']
-   if concept_count == 0:
-      print(" word : ", word['word'], " with concept count = 0", concept_count)
-      my_json = {}    
-      my_json['word'] = word['word']
-      my_json['Diac_lemma'] = word['Diac_lemma']
-      my_json['Undiac_lemma'] = word['Undiac_lemma']
-      return my_json
-   elif concept_count == 1:
-      print(" word : ", word['word'], " with concept count = 1", concept_count)
-      my_json = {}    
-      my_json['word'] = word['word']
-      #my_json['Gloss'] = word['glosses']
-      #glosses = json.loads(word['glosses'][0])
-      glosses = word['glosses'][0]
-      my_json['Gloss'] = glosses['gloss']
-      my_json['Concept_id'] = glosses['concept_id']
-      my_json['Diac_lemma'] = word['Diac_lemma']
-      my_json['Undiac_lemma'] = word['Undiac_lemma']
-      return my_json
-   else:   
-      print(" word : ", word['word'], " with concept count > 1", concept_count)
-      input_word = word['word']
-      concept_count = word['concept_count']
-      glosses = word['glosses']
-      Diac_lemma = word['Diac_lemma']
-      Undiac_lemma = word['Undiac_lemma']
-      return disambiguate_glosses_using_SALMA(glosses, Diac_lemma, Undiac_lemma, input_word, sentence)
-
-def WSD(sentence):
-   
-   input_sentence = simple_word_tokenize(sentence)
-   
-   five_word_lemma = find_five_word_lemma(input_sentence)
-   
-   four_word_lemma = find_four_word_lemma(input_sentence)
-   
-   three_word_lemma = find_three_word_lemma(input_sentence)
-   
-   two_word_lemma = find_two_word_lemma(input_sentence)
-   
-   ner = find_named_entities(" ".join(input_sentence))
-   #ner = []
-
-   output_list = find_glosses(input_sentence, three_word_lemma, two_word_lemma, four_word_lemma, five_word_lemma, ner)
-   
-   results = []
-   #with multiprocessing.Pool(processes=multiprocessing.cpu_count()) as pool:
-   #    results = pool.map(partial(disambiguate_glosses_main, sentence= sentence), output_list)
-   for word in output_list:
-      results.append(disambiguate_glosses_main(word, sentence))
-   #print("Number of processors: ", mp.cpu_count())   
-   #print("After multiProcessing : ", results)
-   return results
-
-@api_view(["POST"])
-def SALMA(request):
-      apikey = "" # defult apikey
-      if 'apikey' in request.GET: # check if user entered the apikey
-         apikey = request.GET['apikey'] # get apikey from URL request
-      else:
-         # if no apikey in URL return these message 
-         return JsonResponse({"statusText":"User is not authenticated","statusCode":-3} ) 
-      body_unicode = request.body.decode('utf-8')
-      body = json.dumps(json.JSONDecoder().decode(body_unicode))
-      d = json.loads(body)
-      sentence = d['sentence']
-      
-      if len(sentence) > 500:
-         content = {"statusText":"Input is too long","statusCode":-7}
-         return JsonResponse(content, safe=False, json_dumps_params={'ensure_ascii': False}) 
-      else: 
-         serviceName = request.path.split("/")[4] # get service_url from request to check if service_groups table contains this url
-         insertLog(request) # if apiKey is not null insert log in table api_tracking_logs
-         apikeyValidation = checkApikey(apikey , serviceName) # call checkApikey function to check apikey validation and limitation
-         if apikeyValidation == True: # if apikey valid, limitation not exceeded, and date has not expired
-            #try:
-               #print("Start with sentence : ", sentence)
-               results = WSD(sentence)
-               content = {"resp": results, "statusText":"OK","statusCode":0}
-               return JsonResponse(content, safe=False, json_dumps_params={'ensure_ascii': False})  
-            #except:
-            #   return JsonResponse({"statusText":"Error !!","statusCode":"-1"} )    # Note: check statusCode number ?-1         
-         else: # if apikey not valid return error message which came from checkApikey
+# ./bookstore_app/api/views.py
+import django
+django.setup()
+import requests
+import json
+from django.http import JsonResponse
+from rest_framework.decorators import api_view
+from salma import settings 
+# Comented by tymaa to Run service via GPU
+#from salma.word_sense_disambiguation import word_sense
+from salma.word_sense_disambiguation import normalizearabert
+from salma.word_sense_disambiguation import load_data_model
+from salma.word_sense_disambiguation import GlossPredictor
+from salma.parser import arStrip
+from salma.parser import removePunctuation
+from salma.parser import removeEnglish
+from salma.tokenizers_words import simple_word_tokenize
+from ALMA_multi_word_service.views import ALMA_multi_word
+import re
+import numpy as np
+from arabiner.bin import infer
+from api_clients_counter_month.ApikeyValidation import checkApikey
+from ApiTrackingService.InsertApiLog import insertLog
+import multiprocessing
+from functools import partial
+from lemmatizer_v2_DB.views import lemmatize_sentence
+from arabiner.views import NER
+
+# Added By Tymaa: 2023-02-05 to call GlossPredictor as a web service from GPU machine 
+#from urllib.request import Request, urlopen
+
+def delete_form_list(position, word_lemma):
+    tmp_word_lemma = [] 
+    output = []
+    for wordLemma in word_lemma:
+        if position == int(wordLemma[2]): # start 
+           word = wordLemma[0]
+           gloss = wordLemma[1]
+           position = int(wordLemma[3]) 
+           concept_count = int(wordLemma[4]) 
+           undiac_multi_word_lemma = wordLemma[5]
+           multi_word_lemma = wordLemma[6]
+           output.append([word, gloss, concept_count, undiac_multi_word_lemma, multi_word_lemma])# word
+        elif position < int(wordLemma[2]): 
+           tmp_word_lemma.append(wordLemma)
+    return tmp_word_lemma, output, position
+    #return output
+
+def find_two_word_lemma(input_sentence):
+    i = 0
+    output = []
+    length = len(input_sentence)
+    while i < length - 1:
+        two_grams = input_sentence[i] +" "+ input_sentence[i + 1] 
+      #   r = requests.get("https://ontology.birzeit.edu/sina/v2/api/ALMA_multi_wordDB/"+two_grams+"?apikey=samplekey", verify=False)
+      #   data = json.loads(r.text)
+        data = ALMA_multi_word(two_grams,2)
+        try :
+            # found two_grams
+            found_2Word_lemma = [two_grams,data[0]['glosses'], i, i + 1,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
+            output.append(found_2Word_lemma) 
+            i = i + 1    
+        except: # no record found on this multi_lema
+            i = i + 1 
+    return output
+
+
+def find_three_word_lemma(input_sentence):
+    i = 0
+    output = []
+    length = len(input_sentence)
+    while i < length - 2:
+        three_grams = input_sentence[i] +" "+ input_sentence[i + 1] + " "+ input_sentence[i + 2]
+        #r = requests.get("https://ontology.birzeit.edu/sina/v2/api/ALMA_multi_wordDB/"+three_grams+"?apikey=samplekey", verify=False)
+        #data = json.loads(r.text) 
+        data = ALMA_multi_word(three_grams,3)
+        try:
+           found_3Word_lemma = [three_grams, data[0]['glosses'], i, i + 2,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
+           output.append(found_3Word_lemma) 
+           i = i + 1    
+        except:  
+           i = i + 1 
+    return output
+
+def find_four_word_lemma(input_sentence):
+   i = 0
+   output = []
+   length = len(input_sentence)
+   while i < length - 3:
+      four_grams = input_sentence[i] +" "+ input_sentence[i + 1] + " "+ input_sentence[i + 2] + " "+ input_sentence[i + 3]
+      data = ALMA_multi_word(four_grams,4)
+      try:
+         found_4Word_lemma = [four_grams, data[0]['glosses'], i, i + 3,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
+         output.append(found_4Word_lemma) 
+         i = i + 1    
+      except:  
+         i = i + 1 
+   return output
+
+
+def find_five_word_lemma(input_sentence):
+   i = 0
+   output = []
+   length = len(input_sentence)
+   while i < length - 4:
+      five_grams = input_sentence[i] +" "+ input_sentence[i + 1] + " "+ input_sentence[i + 2] + " "+ input_sentence[i + 3] + " "+ input_sentence[i + 4]
+      data = ALMA_multi_word(five_grams,5)
+      try:
+         found_5Word_lemma = [five_grams, data[0]['glosses'], i, i + 4,data[0]['concept_count'], data[0]['undiac_multi_word_lemma'], data[0]['multi_word_lemma']]
+         output.append(found_5Word_lemma) 
+         i = i + 1    
+      except:  
+         i = i + 1 
+   return output
+
+def find_named_entities(string):
+   found_entities = []
+   entites = NER(string, "4")
+   tag_gloss = {
+      "PERS": "اسم شخص",
+      "ORG": "اسم مؤسسة",
+      #"NORP": "مجموعة من الناس", 
+      #"OCC": "منصب/مسمى وظيفي",
+      "LOC": "اسم منطقة جغرافية",
+      "FAC": "اسم لمَعلَم",
+      #"EVENT": "حدث",
+      "DATE": "فترة زمنية تدل على تاريخ",
+      "UNIT": "وحدة قياس",
+      "CURR": "عملة",
+      "GPE": "اسم بلد، له حدود إدارية/جيوسياسية",
+      "TIME": "فترة زمنية تدل على الوقت",
+      "CARDINAL": "عدد يدل على معدود",
+      "ORDINAL": "رقم، لا يدل على معدود",
+      "PERCENT": "نسبة مئوية",
+      "QUANTITY": "كمية",
+      "MONEY": "مبلغ مالي",
+      "LANGUAGE": "اسم للغة طبيعية",
+      "PRODUCT": "اسم منتج",
+      "LAW": "قانون"
+   }
+
+   for entity in entites:
+      gloss_ner = ""
+      if entity[1] in tag_gloss.keys():
+         gloss_ner = tag_gloss[entity[1]]  
+
+      if gloss_ner != "":
+         gloss = [{'concept_id': '', 'resource_id': '', 'resource_name': '', 'gloss': gloss_ner}]   
+         entity = [entity[0],gloss,int(entity[2]), int(entity[3]),1,arStrip(entity[0],True,True,True,False,True,False),entity[0]]   
+         found_entities.append(entity)
+   #print("list : ",found_entities)
+   return found_entities   
+
+
+def find_glosses_using_ALMA(word):
+   #r = requests.post('https://ontology.birzeit.edu/sina/v2/api/ALMADB/', json= {"sentence":word}, verify=False)
+   #data = json.loads(r.text)
+   data = lemmatize_sentence(word)
+   Diac_lemma = ""
+   pos = ""
+   Undiac_lemma = ""
+   glosses = []
+   #for values in data['resp']: ### Think about bugs in lemmatizer .ex: connection error...
+   Diac_lemma = data[0][1]
+   pos = data[0][2]
+   Undiac_lemma = arStrip(Diac_lemma, True, True, True, True, True, False) # Remove diacs , smallDiacs , shaddah ,  digit , alif , specialChars
+   glosses = data[0][4]
+   concept_count = data[0][3]
+   return word, Undiac_lemma, Diac_lemma, pos , concept_count, glosses
+   
+def disambiguate_glosses_using_SALMA(glosses, Diac_lemma, Undiac_lemma, word, sentence):
+   word = normalizearabert(word)
+   #print(" word After normalized : ", word)
+   glosses_dictionary = {}
+   if glosses != None:
+      for gloss in glosses:
+         # result = json.loads(gloss)
+         glosses_dictionary.update({gloss['concept_id'] : gloss['gloss']})
+      # Commented by Tymaa (2023-02-05) to call GlossPredictor as a web service from GPU machine 
+      print(" Before GlossPredictor on word = ", word)
+      concept_id, gloss = GlossPredictor(Diac_lemma, Undiac_lemma,word,sentence,glosses_dictionary)
+      print(" After GlossPredictor on word = ", word, " Concept_id : ", concept_id, " gloss : ", gloss)
+
+
+      # Added By Tymaa: 2023-02-05 to call GlossPredictor as a web service from GPU machine 
+      #data = {}
+      #data["Diac_lemma"] = Diac_lemma 
+      #data["Undiac_lemma"] = Undiac_lemma
+      #data["word"] = word
+      #data["sentence"] = sentence
+      #data["glosses_dictionary"] = glosses_dictionary
+      #print("Data : ", data)
+      #data = json.dumps(data).encode('utf8')
+      #req = Request(
+      #      url="http://185.19.228.221:8000/word_sense_disambiguation/",
+      #      data=data,
+      #      headers={'User-Agent': 'Mozilla/5.0', 'Content-Type': 'application/json'},
+      #      method='POST'
+      #)
+      #print("url decode : ", urlopen(req).read().decode())
+      #webpage = urlopen(req).read().decode()
+      #concept_id = json.loads(webpage)['concept_id']
+      #gloss = json.loads(webpage)['Gloss']
+
+      #url = "http://185.19.228.221:8000/word_sense_disambiguation/"
+      
+      #data = json.dumps(data).encode('utf8')
+      #print("encode data: " , data)
+      #response = requests.post(url, data=data, headers={'User-Agent': 'Mozilla/5.0', 'Content-Type': 'application/json'})
+      #print(response.status_code)
+      #if response.status_code == 200:
+      #    resp_text = json.loads(response.text)
+      #    concept_id = resp_text["concept_id"]
+      #    gloss = resp_text["Gloss"]  
+      #else:
+      #    concept_id = None
+      #    gloss = None
+      ##
+
+      my_json = {}    
+      my_json['Concept_id'] = concept_id
+      my_json['Gloss'] = gloss
+      my_json['word'] = word
+      my_json['Undiac_lemma'] = Undiac_lemma
+      my_json['Diac_lemma'] = Diac_lemma
+      return my_json
+   else:
+      #print(" word with gloss = None ", word)
+      my_json = {}    
+      my_json['word'] = word
+      my_json['Undiac_lemma'] = Undiac_lemma
+      my_json['Diac_lemma'] = Diac_lemma
+      return my_json
+
+
+
+
+def find_glosses(input_sentence, three_word_lemma, two_word_lemma, four_word_lemma, five_word_lemma, ner):
+      output_list = []
+      position = 0
+      while position < len(input_sentence):    
+         flag = "False"
+         output_from5word = delete_form_list(position, five_word_lemma)
+         five_word_lemma = output_from5word[0]
+         if output_from5word[1] != []: # output
+            position = output_from5word[2]  
+            flag = "True"
+            my_json = {}    
+            my_json['word'] = output_from5word[1][0][0]
+            my_json['concept_count'] = output_from5word[1][0][2]
+            my_json['glosses'] = output_from5word[1][0][1]
+            my_json['Diac_lemma'] = output_from5word[1][0][4]
+            my_json['Undiac_lemma'] = output_from5word[1][0][3]
+            output_list.append(my_json)
+            position = position + 1                
+
+
+
+         output_from4word = delete_form_list(position, four_word_lemma)
+         four_word_lemma = output_from4word[0]
+         if output_from4word[1] != []: # output
+            position = output_from4word[2]  
+            flag = "True"
+            my_json = {}    
+            my_json['word'] = output_from4word[1][0][0]
+            my_json['concept_count'] = output_from4word[1][0][2]
+            my_json['glosses'] = output_from4word[1][0][1]
+            my_json['Diac_lemma'] = output_from4word[1][0][4]
+            my_json['Undiac_lemma'] = output_from4word[1][0][3]
+            output_list.append(my_json)
+            position = position + 1                
+         
+         output_from3word = delete_form_list(position, three_word_lemma)
+         three_word_lemma = output_from3word[0]
+         if output_from3word[1] != []: # output
+            position = output_from3word[2]  
+            flag = "True"
+            my_json = {}    
+            my_json['word'] = output_from3word[1][0][0]
+            my_json['concept_count'] = output_from3word[1][0][2]
+            my_json['glosses'] = output_from3word[1][0][1]
+            my_json['Diac_lemma'] = output_from3word[1][0][4]
+            my_json['Undiac_lemma'] = output_from3word[1][0][3]
+            output_list.append(my_json)
+            position = position + 1                
+
+
+
+         output_from2Word = delete_form_list(position, two_word_lemma)
+         two_word_lemma = output_from2Word[0] 
+         if output_from2Word[1] != []:  
+            position = output_from2Word[2]
+            flag = "True"
+            my_json = {}    
+            word = output_from2Word[1][0][0]
+            my_json['word'] = word
+            my_json['concept_count'] = output_from2Word[1][0][2]
+            my_json['glosses'] = output_from2Word[1][0][1]
+            my_json['Diac_lemma'] = output_from2Word[1][0][4]
+            my_json['Undiac_lemma'] = output_from2Word[1][0][3] 
+            output_list.append(my_json)
+            position = position + 1                 
+               
+
+
+         output_from_ner = delete_form_list(position, ner)
+         ner = output_from_ner[0] 
+         if output_from_ner[1] != []:  
+            position = output_from_ner[2]
+            flag = "True"
+            my_json = {}    
+            word = output_from_ner[1][0][0]
+            my_json['word'] = word
+            my_json['concept_count'] = output_from_ner[1][0][2]
+            my_json['glosses'] = output_from_ner[1][0][1]
+            my_json['Diac_lemma'] = output_from_ner[1][0][4]
+            my_json['Undiac_lemma'] = output_from_ner[1][0][3] 
+            output_list.append(my_json)
+            position = position + 1                             
+         
+         if flag == "False": # Not found in ner or in multi_word_dictionary, ASK ALMA 
+            word = input_sentence[position]
+            word, Undiac_lemma, Diac_lemma, pos , concept_count, glosses = find_glosses_using_ALMA(word)   
+            my_json = {}    
+            my_json['word'] = word
+            my_json['concept_count'] = concept_count
+            my_json['glosses'] = glosses
+            my_json['Diac_lemma'] = Diac_lemma
+            my_json['Undiac_lemma'] = Undiac_lemma
+            output_list.append(my_json)
+            position = position + 1  
+      return output_list                    
+
+def disambiguate_glosses_main(word, sentence):
+   concept_count = word['concept_count']
+   if concept_count == 0:
+      print(" word : ", word['word'], " with concept count = 0", concept_count)
+      my_json = {}    
+      my_json['word'] = word['word']
+      my_json['Diac_lemma'] = word['Diac_lemma']
+      my_json['Undiac_lemma'] = word['Undiac_lemma']
+      return my_json
+   elif concept_count == 1:
+      print(" word : ", word['word'], " with concept count = 1", concept_count)
+      my_json = {}    
+      my_json['word'] = word['word']
+      #my_json['Gloss'] = word['glosses']
+      #glosses = json.loads(word['glosses'][0])
+      glosses = word['glosses'][0]
+      my_json['Gloss'] = glosses['gloss']
+      my_json['Concept_id'] = glosses['concept_id']
+      my_json['Diac_lemma'] = word['Diac_lemma']
+      my_json['Undiac_lemma'] = word['Undiac_lemma']
+      return my_json
+   else:   
+      print(" word : ", word['word'], " with concept count > 1", concept_count)
+      input_word = word['word']
+      concept_count = word['concept_count']
+      glosses = word['glosses']
+      Diac_lemma = word['Diac_lemma']
+      Undiac_lemma = word['Undiac_lemma']
+      return disambiguate_glosses_using_SALMA(glosses, Diac_lemma, Undiac_lemma, input_word, sentence)
+
+def WSD(sentence):
+   
+   input_sentence = simple_word_tokenize(sentence)
+   
+   five_word_lemma = find_five_word_lemma(input_sentence)
+   
+   four_word_lemma = find_four_word_lemma(input_sentence)
+   
+   three_word_lemma = find_three_word_lemma(input_sentence)
+   
+   two_word_lemma = find_two_word_lemma(input_sentence)
+   
+   ner = find_named_entities(" ".join(input_sentence))
+   #ner = []
+
+   output_list = find_glosses(input_sentence, three_word_lemma, two_word_lemma, four_word_lemma, five_word_lemma, ner)
+   
+   results = []
+   #with multiprocessing.Pool(processes=multiprocessing.cpu_count()) as pool:
+   #    results = pool.map(partial(disambiguate_glosses_main, sentence= sentence), output_list)
+   for word in output_list:
+      results.append(disambiguate_glosses_main(word, sentence))
+   #print("Number of processors: ", mp.cpu_count())   
+   #print("After multiProcessing : ", results)
+   return results
+
+@api_view(["POST"])
+def SALMA(request):
+      apikey = "" # defult apikey
+      if 'apikey' in request.GET: # check if user entered the apikey
+         apikey = request.GET['apikey'] # get apikey from URL request
+      else:
+         # if no apikey in URL return these message 
+         return JsonResponse({"statusText":"User is not authenticated","statusCode":-3} ) 
+      body_unicode = request.body.decode('utf-8')
+      body = json.dumps(json.JSONDecoder().decode(body_unicode))
+      d = json.loads(body)
+      sentence = d['sentence']
+      
+      if len(sentence) > 500:
+         content = {"statusText":"Input is too long","statusCode":-7}
+         return JsonResponse(content, safe=False, json_dumps_params={'ensure_ascii': False}) 
+      else: 
+         serviceName = request.path.split("/")[4] # get service_url from request to check if service_groups table contains this url
+         insertLog(request) # if apiKey is not null insert log in table api_tracking_logs
+         apikeyValidation = checkApikey(apikey , serviceName) # call checkApikey function to check apikey validation and limitation
+         if apikeyValidation == True: # if apikey valid, limitation not exceeded, and date has not expired
+            #try:
+               #print("Start with sentence : ", sentence)
+               results = WSD(sentence)
+               content = {"resp": results, "statusText":"OK","statusCode":0}
+               return JsonResponse(content, safe=False, json_dumps_params={'ensure_ascii': False})  
+            #except:
+            #   return JsonResponse({"statusText":"Error !!","statusCode":"-1"} )    # Note: check statusCode number ?-1         
+         else: # if apikey not valid return error message which came from checkApikey
             return JsonResponse(apikeyValidation)
```

### Comparing `nlptoolssna-0.9.2/nlptools/salma/wsd.py` & `nlptoolssna-0.9.3/nlptools/salma/wsd.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-# Comented by tymaa to Run service via GPU
-from nlptools.utils.implication import Implication
-from salma import settings 
-from pandas import read_excel, concat
-import re
-from transformers import BertTokenizer,BertForSequenceClassification
-from transformers import BertTokenizer,BertForSequenceClassification
-
-import warnings
-warnings.filterwarnings("ignore")
-import torch
-
-import numpy as np
-
-import pandas as pd
-
-from arabert.preprocess import ArabertPreprocessor
-
-def word_sense(word, sentence):
-    lemma = "مدخلة"
-    pos = "اسم"
-    concept_id = "39000001"
-    return word, lemma, pos, concept_id
-
-def normalizearabert(s):
-  model_name = 'aubmindlab/bert-base-arabertv02'
-  arabert_prep = ArabertPreprocessor(model_name.split("/")[-1])
-  return arabert_prep.preprocess(str(s))
-
-
-def load_data_model():
-  file = './modern_examples4bert_true_v4_newcorrectData_BZUthes.xlsx'
-  df = read_excel("{}".format(file))
-  df['Example'] = df['Example'].apply(lambda x: str(x).upper())
-  df['Example'] = df['Example'].apply(lambda x: re.sub(r'^((.?\[UNUSED0\].?){1})\[UNUSED0\]', r'\1[UNUSED1]', str(x)) )
-
-  dftrain = df[df['Is_training'] == 1]
-
-  dftrue = dftrain[dftrain['Label'] == 1]
- 
-  # Added by Tymaa 
-  # l=[]
-  # l.append("Concept_id")
-  # l.append("Diac_lemma")
-  # l.append("Undiac_lemma")
-  # l.append("Gloss")
-  # l.append("Target")
-  # l.append("Example")
-  # dftrue = "{}".format(l)
-  # print("df :  \n ",dftrue)
-
-
-#   dftrue['Lemma'] = dftrue['Lemma'].apply(normalizearabert)
-  name = './bert-base-arabertv02_22_May_2021_00h_allglosses_unused01'
-  model = BertForSequenceClassification.from_pretrained('{}'.format(name),
-                                                        output_hidden_states = True,
-                                                        num_labels=2
-                                                        )
-  tokenizer = BertTokenizer.from_pretrained('{}'.format('./bert-base-arabertv02'))
-  tokenizer.add_special_tokens({ "additional_special_tokens": [ "[UNUSED0]" ] })
-  tokenizer.add_special_tokens({ "additional_special_tokens": [ "[UNUSED1]" ] })
-
-  model.resize_token_embeddings(len(tokenizer))
-
-  return  dftrue,tokenizer, model
-
-
-def glosses1(dfcand,target):
-# """
-# takes a dataframe 
-# return 
-	# 'none' if the maximum logistic regression score for TRUE class is less than -2 OR
-	# the predicted gloss having the maximum logistic regression score
-# """
-  print("Before read data")
-  wic_c = []
-  wic_c, _ = read_data(dfcand,normalizearabert,target)
-  print("After read data")
-  tokenizedwic_c = np.array([settings.tokenizer.encode(x, max_length=512,padding='max_length',truncation='longest_first',add_special_tokens=True) for x in wic_c])
-  max_len = 512
-  segmentswic = torch.tensor([get_segments(settings.tokenizer.convert_ids_to_tokens(i),max_len) for i in tokenizedwic_c])
-  paddedwic = tokenizedwic_c
-  attention_maskwic = np.where(paddedwic != 0, 1, 0)
-  input_idswic = torch.tensor(paddedwic)  
-  attention_maskwic = torch.tensor(attention_maskwic)
-  print("Before EVAL function")
-  settings.model = settings.model.eval()
-  print("After EVAL function")
-  wicpredictions , wictrue_labels = [], []
-  b_input_ids = input_idswic
-  b_input_mask =  attention_maskwic
-  b_input_seg = segmentswic
-
-  print("BEFORE MODEL")
-  with torch.no_grad():
-    print("Inside model")
-    outputs = settings.model(b_input_ids,token_type_ids=b_input_seg,attention_mask=b_input_mask)
-    print("output")
-  print("AFTER MODEL")
-
-  logits = outputs[0]
-  wicpredictions.append(logits)
-  wicflat_predictions = np.concatenate(wicpredictions, axis=0)
-  # if wicflat_predictions[np.argmax(wicflat_predictions, axis=0).flatten()[1]][1] < -2:
-    # return 'none'
-  # return dfcand['Gloss'].to_list()[np.argmax(wicflat_predictions, axis=0).flatten()[1]]
-  
-  ### These two lines are commented by Tymaa on 2021-06-28
-  #if wicflat_predictions[np.argmax(wicflat_predictions, axis=0).flatten()[1]][1] < -2:
-  #  return 'none','none'
-  return dfcand['Concept_id'].to_list()[np.argmax(wicflat_predictions, axis=0).flatten()[1]],dfcand['Gloss'].to_list()[np.argmax(wicflat_predictions, axis=0).flatten()[1]]
-
-def read_data(data,normalize,target):
-  c = []
-  labels = []
-  for i,row in data.iterrows():
-      # lemma = normalize(row['Undiac_lemma'])
-      example = normalize(row['Example'])
-      gloss = normalize(row['Gloss'])
-      label = row['Label']
-      # target = normalize(row['Target'])
-      c.append('{} [SEP] {}: {}'.format(example,target,gloss))
-      if label == 1.0:
-          labels.append(1)
-      else:
-          labels.append(0)
-  return c,labels
-
-def inserttag1(sentence,tag,start,end):
-    before = sentence[:start]
-    after = sentence[end:]
-    target = sentence[start:end]
-    return before+tag+sentence[start:end]+tag+after
-
-def get_segments(tokens, max_seq_length):
-    # """Segments: 0 for the first sequence, 1 for the second"""
-    if len(tokens)>max_seq_length:
-        raise IndexError("Token length more than max seq length!")
-    segments = []
-    current_segment_id = 0
-    for token in tokens:
-        segments.append(current_segment_id)
-        if token == "[SEP]":
-            current_segment_id = 1
-    return segments + [0] * (max_seq_length - len(tokens))
-
-def senttarget(target,example): ### Make sure to tag words correctely ex:  ذهب الرجل ليشتري ذهب، / عند& عندهم
-  start = -1
-  try:
-    start = example.index(target)
-  except ValueError:
-    return -1
-  end = example.index(target)+len(target)
-  return inserttag1(example,"[UNUSED0]",start,end)
-
-
-def GlossPredictor(diac_lemma, undiac_lemma,target,example,glosses):
-# """ 
-# takes 
-	# a lemma
-	# corresponding target word 
-	# an example
-	# glosses as a dictionay, following an example:
-	#	glosses =	{"Concept_id1": "gloss1",  "Concept_id2": "gloss2",  "Concept_id3": "gloss3"}
-# returns 
-	# -1   if the example does not contain the target word  OR
-	# 'none' if no records in dftrue for the lemma and if the maximum logistic regression score for TRUE class is less than -2 OR
-	# the predicted gloss for the target word 
-	# 
-# """
-  example = senttarget(target,example)
-  if example == -1:
-    return -1,-1
-  # All records for Undiac_lemma
-  #dfcand1 = settings.dftrue[settings.dftrue['Undiac_lemma'] == undiac_lemma]
-  #m = dfcand1['Diac_lemma'].apply(lambda x: samelemma(x,diac_lemma))
-  ### Added by Tymaa ON 2021-06-13 in case m is empty 
-  #if len(m) <= 0:
-  #  m = dfcand1
-  # All records for Diac_lemma from dfcand1
-  #dfcand = dfcand1[m]
-  
-  data = []
-  for g in glosses:
-      data.append([g,diac_lemma,undiac_lemma, glosses[g], target,example,0,1,'','',''])
-  dfcolumns = ['Concept_id', 'Diac_lemma', 'Undiac_lemma', 'Gloss', 'Target', 'Example', 'Is_training', 'Label', 'concept_id', 'lemma_id', 'POS']
-  dfcand = pd.DataFrame(data,columns=dfcolumns)
-  
-  
-  if len(dfcand) > 0:
-    dfcand['Example'] = dfcand['Example'].apply(lambda x: example)
-    dfcand['Target'] = dfcand['Target'].apply(lambda x: target)
-    dfcand = dfcand.drop_duplicates()
-  
-    dfcand['Example'] = dfcand['Example'].apply(lambda x: x.upper())
-    dfcand['Example'] = dfcand['Example'].apply(lambda x: re.sub(r'^((.?\[UNUSED0\].?){1})\[UNUSED0\]', r'\1[UNUSED1]', x) )
-    print("Before glosses1 into GlossPredictor function  dfcand : ",dfcand, "  target: ",target)
-    return glosses1(dfcand,target)
-  else:
-    return 'none','none'
-
-
-def samelemma(w1,w2):
-  implication =  Implication(w1 , w2)
-  if implication.getResult() == 'Same':
-    return True
-  else:
+# Comented by tymaa to Run service via GPU
+from nlptools.utils.implication import Implication
+from salma import settings 
+from pandas import read_excel, concat
+import re
+from transformers import BertTokenizer,BertForSequenceClassification
+from transformers import BertTokenizer,BertForSequenceClassification
+
+import warnings
+warnings.filterwarnings("ignore")
+import torch
+
+import numpy as np
+
+import pandas as pd
+
+from arabert.preprocess import ArabertPreprocessor
+
+def word_sense(word, sentence):
+    lemma = "مدخلة"
+    pos = "اسم"
+    concept_id = "39000001"
+    return word, lemma, pos, concept_id
+
+def normalizearabert(s):
+  model_name = 'aubmindlab/bert-base-arabertv02'
+  arabert_prep = ArabertPreprocessor(model_name.split("/")[-1])
+  return arabert_prep.preprocess(str(s))
+
+
+def load_data_model():
+  file = './modern_examples4bert_true_v4_newcorrectData_BZUthes.xlsx'
+  df = read_excel("{}".format(file))
+  df['Example'] = df['Example'].apply(lambda x: str(x).upper())
+  df['Example'] = df['Example'].apply(lambda x: re.sub(r'^((.?\[UNUSED0\].?){1})\[UNUSED0\]', r'\1[UNUSED1]', str(x)) )
+
+  dftrain = df[df['Is_training'] == 1]
+
+  dftrue = dftrain[dftrain['Label'] == 1]
+ 
+  # Added by Tymaa 
+  # l=[]
+  # l.append("Concept_id")
+  # l.append("Diac_lemma")
+  # l.append("Undiac_lemma")
+  # l.append("Gloss")
+  # l.append("Target")
+  # l.append("Example")
+  # dftrue = "{}".format(l)
+  # print("df :  \n ",dftrue)
+
+
+#   dftrue['Lemma'] = dftrue['Lemma'].apply(normalizearabert)
+  name = './bert-base-arabertv02_22_May_2021_00h_allglosses_unused01'
+  model = BertForSequenceClassification.from_pretrained('{}'.format(name),
+                                                        output_hidden_states = True,
+                                                        num_labels=2
+                                                        )
+  tokenizer = BertTokenizer.from_pretrained('{}'.format('./bert-base-arabertv02'))
+  tokenizer.add_special_tokens({ "additional_special_tokens": [ "[UNUSED0]" ] })
+  tokenizer.add_special_tokens({ "additional_special_tokens": [ "[UNUSED1]" ] })
+
+  model.resize_token_embeddings(len(tokenizer))
+
+  return  dftrue,tokenizer, model
+
+
+def glosses1(dfcand,target):
+# """
+# takes a dataframe 
+# return 
+	# 'none' if the maximum logistic regression score for TRUE class is less than -2 OR
+	# the predicted gloss having the maximum logistic regression score
+# """
+  print("Before read data")
+  wic_c = []
+  wic_c, _ = read_data(dfcand,normalizearabert,target)
+  print("After read data")
+  tokenizedwic_c = np.array([settings.tokenizer.encode(x, max_length=512,padding='max_length',truncation='longest_first',add_special_tokens=True) for x in wic_c])
+  max_len = 512
+  segmentswic = torch.tensor([get_segments(settings.tokenizer.convert_ids_to_tokens(i),max_len) for i in tokenizedwic_c])
+  paddedwic = tokenizedwic_c
+  attention_maskwic = np.where(paddedwic != 0, 1, 0)
+  input_idswic = torch.tensor(paddedwic)  
+  attention_maskwic = torch.tensor(attention_maskwic)
+  print("Before EVAL function")
+  settings.model = settings.model.eval()
+  print("After EVAL function")
+  wicpredictions , wictrue_labels = [], []
+  b_input_ids = input_idswic
+  b_input_mask =  attention_maskwic
+  b_input_seg = segmentswic
+
+  print("BEFORE MODEL")
+  with torch.no_grad():
+    print("Inside model")
+    outputs = settings.model(b_input_ids,token_type_ids=b_input_seg,attention_mask=b_input_mask)
+    print("output")
+  print("AFTER MODEL")
+
+  logits = outputs[0]
+  wicpredictions.append(logits)
+  wicflat_predictions = np.concatenate(wicpredictions, axis=0)
+  # if wicflat_predictions[np.argmax(wicflat_predictions, axis=0).flatten()[1]][1] < -2:
+    # return 'none'
+  # return dfcand['Gloss'].to_list()[np.argmax(wicflat_predictions, axis=0).flatten()[1]]
+  
+  ### These two lines are commented by Tymaa on 2021-06-28
+  #if wicflat_predictions[np.argmax(wicflat_predictions, axis=0).flatten()[1]][1] < -2:
+  #  return 'none','none'
+  return dfcand['Concept_id'].to_list()[np.argmax(wicflat_predictions, axis=0).flatten()[1]],dfcand['Gloss'].to_list()[np.argmax(wicflat_predictions, axis=0).flatten()[1]]
+
+def read_data(data,normalize,target):
+  c = []
+  labels = []
+  for i,row in data.iterrows():
+      # lemma = normalize(row['Undiac_lemma'])
+      example = normalize(row['Example'])
+      gloss = normalize(row['Gloss'])
+      label = row['Label']
+      # target = normalize(row['Target'])
+      c.append('{} [SEP] {}: {}'.format(example,target,gloss))
+      if label == 1.0:
+          labels.append(1)
+      else:
+          labels.append(0)
+  return c,labels
+
+def inserttag1(sentence,tag,start,end):
+    before = sentence[:start]
+    after = sentence[end:]
+    target = sentence[start:end]
+    return before+tag+sentence[start:end]+tag+after
+
+def get_segments(tokens, max_seq_length):
+    # """Segments: 0 for the first sequence, 1 for the second"""
+    if len(tokens)>max_seq_length:
+        raise IndexError("Token length more than max seq length!")
+    segments = []
+    current_segment_id = 0
+    for token in tokens:
+        segments.append(current_segment_id)
+        if token == "[SEP]":
+            current_segment_id = 1
+    return segments + [0] * (max_seq_length - len(tokens))
+
+def senttarget(target,example): ### Make sure to tag words correctely ex:  ذهب الرجل ليشتري ذهب، / عند& عندهم
+  start = -1
+  try:
+    start = example.index(target)
+  except ValueError:
+    return -1
+  end = example.index(target)+len(target)
+  return inserttag1(example,"[UNUSED0]",start,end)
+
+
+def GlossPredictor(diac_lemma, undiac_lemma,target,example,glosses):
+# """ 
+# takes 
+	# a lemma
+	# corresponding target word 
+	# an example
+	# glosses as a dictionay, following an example:
+	#	glosses =	{"Concept_id1": "gloss1",  "Concept_id2": "gloss2",  "Concept_id3": "gloss3"}
+# returns 
+	# -1   if the example does not contain the target word  OR
+	# 'none' if no records in dftrue for the lemma and if the maximum logistic regression score for TRUE class is less than -2 OR
+	# the predicted gloss for the target word 
+	# 
+# """
+  example = senttarget(target,example)
+  if example == -1:
+    return -1,-1
+  # All records for Undiac_lemma
+  #dfcand1 = settings.dftrue[settings.dftrue['Undiac_lemma'] == undiac_lemma]
+  #m = dfcand1['Diac_lemma'].apply(lambda x: samelemma(x,diac_lemma))
+  ### Added by Tymaa ON 2021-06-13 in case m is empty 
+  #if len(m) <= 0:
+  #  m = dfcand1
+  # All records for Diac_lemma from dfcand1
+  #dfcand = dfcand1[m]
+  
+  data = []
+  for g in glosses:
+      data.append([g,diac_lemma,undiac_lemma, glosses[g], target,example,0,1,'','',''])
+  dfcolumns = ['Concept_id', 'Diac_lemma', 'Undiac_lemma', 'Gloss', 'Target', 'Example', 'Is_training', 'Label', 'concept_id', 'lemma_id', 'POS']
+  dfcand = pd.DataFrame(data,columns=dfcolumns)
+  
+  
+  if len(dfcand) > 0:
+    dfcand['Example'] = dfcand['Example'].apply(lambda x: example)
+    dfcand['Target'] = dfcand['Target'].apply(lambda x: target)
+    dfcand = dfcand.drop_duplicates()
+  
+    dfcand['Example'] = dfcand['Example'].apply(lambda x: x.upper())
+    dfcand['Example'] = dfcand['Example'].apply(lambda x: re.sub(r'^((.?\[UNUSED0\].?){1})\[UNUSED0\]', r'\1[UNUSED1]', x) )
+    print("Before glosses1 into GlossPredictor function  dfcand : ",dfcand, "  target: ",target)
+    return glosses1(dfcand,target)
+  else:
+    return 'none','none'
+
+
+def samelemma(w1,w2):
+  implication =  Implication(w1 , w2)
+  if implication.getResult() == 'Same':
+    return True
+  else:
     return False
```

### Comparing `nlptoolssna-0.9.2/nlptools/utils/implication.py` & `nlptoolssna-0.9.3/nlptools/utils/implication.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,665 +1,665 @@
-# Created: 16/03/2021 , By Mohammad A'bed
-# Trello task: https://trello.com/c/nHnmnFAe/19-re-implement-implication-function-in-python
-
-#  The Imply algorithm takes two words as input and produces the matching tuple defined by (Words Matching).
-#  The matching between two words is defined as a tuple:
-#  <w1, w2, implication direction, distance, conflicts, verdict, preferredWord> .
-
-from nlptools.utils.parser import arStrip
-class Implication:
-    """
-    The implication class computes whether the two Arabic words are the same or not, regardless of how they are diacritized. The output also contains implication direction, distance, number of conflicts, and other outputs. 
-    Argd:
-        :obj:`str' word1: input text
-        :obj:`str' word2: input text
-
-    """
-    # Diacritic Pair Distance Map
-    distanceTable = [
-    [0, 0, 1, 1, 1, 1, 1, 1, 15, 16, 16, 16, 0, 0, 0, 0 ],
-    [0, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
-    [1, 101, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
-    [1, 101, 101, 0, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
-    [1, 101, 101, 101, 0, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
-    [1, 101, 101, 101, 101, 0, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
-    [1, 101, 101, 101, 101, 101, 0, 101, 101, 101, 101, 101, 0, 0, 0, 0],
-    [1, 101, 101, 101, 101, 101, 101, 0, 101, 101, 101, 101, 0, 0, 0, 0],
-    [15, 101, 101, 101, 101, 101, 101, 101, 0, 1, 1, 1, 0, 0, 0, 0],
-    [16, 101, 101, 101, 101, 101, 101, 101, 1, 0, 101, 101, 0, 0, 0, 0],
-    [16, 101, 101, 101, 101, 101, 101, 101, 1, 101, 0, 101, 0, 0, 0, 0],
-    [16, 101, 101, 101, 101, 101, 101, 101, 1, 101, 101, 0, 0, 0, 0, 0],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 4, 4],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 0, 100, 100],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 100, 0, 100],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 100, 100, 0]
-    ]
-
-    # Implication direction  Map
-    directionTable =[
-    [3, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0],
-    [2, 3, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
-    [2, -1, 3, -1, -1, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
-    [2, -1, -1, 3, -1, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
-    [2, -1, -1, -1, 3, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
-    [2, -1, -1, -1, -1, 3, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
-    [2, -1, -1, -1, -1, -1, 3, -1, -1, -1, -1, -1, 0, 0, 0, 0],
-    [2, -1, -1, -1, -1, -1, -1, 3, -1, -1, -1, -1, 0, 0, 0, 0],
-    [2, -1, -1, -1, -1, -1, -1, -1, 3, 1, 1, 1, 0, 0, 0, 0],
-    [2, -1, -1, -1, -1, -1, -1, -1, 2, 3, -1, -1, 0, 0, 0, 0],
-    [2, -1, -1, -1, -1, -1, -1, -1, 2, -1, 3, -1, 0, 0, 0, 0],
-    [2, -1, -1, -1, -1, -1, -1, -1, 2, -1, -1, 3, 0, 0, 0, 0],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 1, 1, 1],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 3, -1, -1],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, -1, 3, -1],
-    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, -1, -1, 3]
-    ]
-
-    word1 , word2 = "" , "" # two words to be compared
-    conflictFlags =  [False for i in range(5)] 
-    verdict = "null"    # verdict:  takes one of the values: “compatible”, or “incompatible”
-    word1Undiac = ""    # word1 without diacritics 
-    word2Undiac = ""    # word2 without diacritics 
-    word1Diacritics = [] # Diacritics array of the first word
-    word2Diacritics = [] # Diacritics array of the second word
-    direction = -2147483648 # direction: is a number denoting the relationship between the two words, the defult value is given a low integer, arbitrarry value
-    distance = -2147483648 # distance: denotes the overall similarity of the diacritization between the two words, which we compute based on the distance map; the defult value is given a low integer, arbitrarry value
-    conflicts = -2147483648 # conflict: denotes the number of conflicting diacritics between the two words, the defult value is given a low integer, arbitrarry value
-    lettersDirection = [] # implication direction between diacritics 
-
-    def __init__(self , inputWord1 ,  inputWord2):
-        
-        #check if inputWord1 or inputWord2 is empty, then return the values below
-        if ( (not inputWord1) and (inputWord2) ) or  ( ( inputWord1) and (not inputWord2) ):
-            self.verdict = "Incompatible"
-            self.direction = -3 # the two words have different letters
-            self.distance = 3000
-            self.conflicts = 0
-            return
-
-        self.conflictFlags =  [False for i in range(5)] # reset conflictFlags array to Fales
-        self.word1 = Implication.normalize_alef(inputWord1) # unify alif 
-        self.word2 = Implication.normalize_alef(inputWord2) # unify alif 
-
-        if ( self.word1 ==  self.word2): # If w1 == w2 returns the values bellow 
-            self.verdict = "Compatible"
-            self.direction = 3 #  Both letters have exactly the same diacritics 
-            self.distance = 0
-            self.conflicts = 0
-            return
-        else: # If w1 and w2 are noot exact match
-            try:
-                self.lettersDirection = []
-                # build diacritics array for each word 
-                self.word1Diacritics = Implication.get_diacritics_array(self.word1)
-                self.word2Diacritics = Implication.get_diacritics_array(self.word2)
-
-                 # defined lettersDirection array with size of word1Diacritics and fill it by zeros
-                for x in range(0 , len(self.word1Diacritics) + 1): 
-                    self.lettersDirection.append(0)
-            except :
-                # In case of errors returns the values below 
-                self.verdict = "Incompatible"
-                self.direction = -3 # the two words have different letters
-                self.distance = 3000
-                self.conflicts = 0
-                return
-
-            # check if diacritics in both words for some of syntax errors then return Incompatible
-            if (  Implication.diacritics_syntax_error_in(self.word1Diacritics) == False and  Implication.diacritics_syntax_error_in(self.word2Diacritics) == False) : 
-                # If no syntax error found:
-                self.word1Undiac = arStrip(self.word1, diacs=False, shaddah=False)
-                self.word2Undiac = arStrip(self.word2, diacs=False, shaddah=False)
-                # return compatible if each word is one and same letter regardless of diacritics on this letter
-                if (len(self.word1Undiac) == 1 and len(self.word2Undiac) == 1 and self.word1Undiac == self.word2Undiac): 
-                        self.verdict = "Compatible"
-                        self.direction = 3  #  Both letters have exactly the same diacritics 
-                        self.distance = 0
-                        self.conflicts = 0
-                else : # If words are more than letter or deffirent letter then calculate the impication
-                    self.lettersDirection[0] = 3 
-                    self.calculate_words_implication()
-                
-            else : # If found syntax error in diacitics in word1 or word2 then return these:
-                self.verdict = "Incompatible"
-                self.direction = -3 # the two words have different letters
-                self.distance = 3000
-                self.conflicts = 0
-            
-    def get_non_preferred_word(self, word1, word2):
-        """
-        This method returns the non-preferred word from two given words.
-
-        Args:
-            :obj:`str' word1: The first word.
-            :obj:`str' word2: The second word.
-
-        Returns:
-            :obj:`str': The non-preferred word.
-
-        Raises:
-            None
-        """
-        # this function talkes 2-words and retuen preferredWord 
-        word1 = word1.strip()
-        word2 = word2.strip()
-        if (word1 != None and  word1 ) :
-            if (word2 != None and word2) :
-                preferredWord = ""
-                preferredWord = Implication.getPreferredWord(word1, word2)
-                if word1== preferredWord:
-                    return word2
-                else:
-                    return word1
-            else :
-                return word1
-        
-        else :
-            if word2 != None and word2:
-                return word2 
-            else:
-                return None
-    
-
-
-    def get_preferred_word( self , word1,   word2) :
-        """
-        This method returns the preferred word from two given words.
-
-        Args:
-            :obj:`str' word1: The first word.
-            :obj:`str' word2: The second word.
-
-        Returns:
-            :obj:`str': The preferred word.
-
-        Raises:
-            None
-        """        
-        word1 = word1.strip()
-        word2 = word2.strip()
-        if ( word1 != None and word1) :
-            if (word2 != None and word2) :
-                implication =  Implication(word1, word2) 
-                direction = implication.get_distance()
-                if (direction < 15) :
-                    if ( ( direction == 0 ) or
-                       (direction == 2 ) ):
-                        return word1
-                    elif direction == 1 :
-                        return word2
-                    elif direction == 3 :
-                        if ( ( not word1.endswith("َ") ) and ( not word1.endswith("ُ") ) ) : 
-                            return word2
-                        return word1
-
-                return ""
-            else :
-                return word1
-        
-        else :
-            if word2 != None and (not word2):
-                return  word2
-            else:
-                return None
-            
-    def normalize_alef(word):
-        """
-        This method normalizes the alif (ألف) character in the given word.
-
-        Args:
-            word (:obj:`str`): The input word to be normalized.
-
-        Returns:
-            :obj:`str`: The normalized word with alif characters modified.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication
-
-            word = Implication.normalize_alef("ًى")  # Returns "ىً"
-            word = Implication.normalize_alef("ًا")  # Returns "اً"
-            word = Implication.normalize_alef("ٱلكتاب")  # Returns "الكتاب"
-        """
-        # If the tanween is before the alif, then it is placed after it,
-        # because in the Arabic language this word is similar
-        if word.endswith("ًى"):
-            word = word[:len(word) - 2] + "ىً"
-
-        if word.endswith("ًا"):
-            word = word[:len(word) - 2] + "اً"
-        # Replace Alif-dhamma with Alif
-        if word.startswith("ٱ"):
-            word = "ا" + word[1:]
-        return word
-
-
-    def diacritics_syntax_error_in( diacriticsArray ) :
-        """
-        This method checks if the diacritics in a given array are incorrect.
-
-        Args:
-            diacritics_array (:obj:`list`): A list of diacritics to be checked.
-
-        Returns:
-            :obj:`bool`: True if there is a syntax error in the diacritics, False otherwise.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication 
-
-            diacritics = ["َ", "ُ", "ِ", "ّ"]
-            has_error = Implication.diacritics_syntax_error_in(diacritics)  # Returns False
-
-            diacritics = ["َ", "ُ", "ِ", "ٓ"]
-            has_error = Implication.diacritics_syntax_error_in(diacritics)  # Returns True
-        """
-        # This funcion return True when the diacritics is incorreclty 
-        try:
-            # check last letter diacritic
-            if ( Implication.wrong_end_diacritic(diacriticsArray[ len(diacriticsArray) - 1]) ) : 
-                return True
-            else :
-                # check All letters diacritic except the last letter diacritic
-                for i in range(0 , len(diacriticsArray) - 1 ) :
-                    if (Implication.wrong_middle_iacritic(diacriticsArray[i])) :
-                        return True 
-                return False
-            
-        except :
-            return False
-        
-
-    def wrong_end_diacritic(diac):
-        """
-        This method checks if the given diacritic is a wrong end diacritic.
-
-        Args:
-            diac (:obj:`int`): The diacritic value to be checked.
-
-        Returns:
-            :obj:`bool`: True if the diacritic is one of the follwoing number (85:SHADDAH WITH FATHATAN, 86:SHADDAH WITH KASRTA, 87:SHADDAH WITH DHAMTAN), False if diacritic is greator than or equal0 and diacritic is less than or equal 11.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication 
-
-            diacritic = 0
-            is_wrong_end = Implication.wrong_end_diacritic(diacritic)  # Returns False
-
-            diacritic = 85
-            is_wrong_end = Implication.wrong_end_diacritic(diacritic)  # Returns True
-        """
-        # 0 > No Diacritics , 1 > SUKUN, 2 > FATHA, 3 > KASRA, 4 > DAMMA, 5 > FATHATAN, 6 > KASRATAN,
-        #  7 > DAMMATAN, 8 > SHADDA, 9 > SHADDA with FATHA, 10 > SHADDA with KASRA, 11 > SHADDA with DAMMA
-        if (diac >= 0 and diac <= 11) :
-            return False
-        else :
-            # 85 - 86 - 87: SHADDAH WITH FATHATAN,SHADDAH WITH KASRTA, SHADDAH WITH DHAMTAN
-            return diac < 85 or diac > 87
-        
-    def wrong_middle_iacritic( diac) :
-
-        if (diac >= 0 and diac <= 4) :
-            return False
-        else :
-            return diac < 8 or diac > 15
-            
-    
-    def calculate_words_implication(self):
-        """
-        This method calculates the implication between two words, and updates the verdict, direction, distance, and conflicts attributes of the object based on the implication between the words.
-
-        Returns:
-            None
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication
-
-            implication = Implication(word1, word2)
-            implication.calculate_words_implication()
-            # Access the updated attributes
-            verdict = implication.verdict
-            direction = implication.direction
-            distance = implication.distance
-            conflicts = implication.conflicts
-        """
-
-        self.verdict = "Incompatible"
-        self.direction = -2 
-        self.distance = 1000
-        if (Implication.equal_words(self) == False): # If both words are not thge same return these values 
-            if ((len(self.word1Undiac) == 0 and len(self.word2Undiac) == 0)):
-                if (self.word1 == self.word2): 
-                    self.conflicts = 0
-                    self.distance = 0
-                    self.direction = 3 
-                else:
-                    self.conflicts = 1
-                    self.distance = 1000
-                    self.direction = -2 
-                
-            else:
-                self.conflicts = max(len(self.word1Undiac), len(self.word2Undiac))
-            
-        else:
-            if (Implication.calculate_letters_implication(self)):
-                self.direction = Implication.calculate_direction(self)
-                if (self.direction == -1) :
-                    self.distance = 101
-                else:
-                    self.verdict = "Compatible"
-                
-            else:
-                self.direction = -3 # the two words have different letters
-                self.distance = 3000
-                self.conflicts = 0
-
-    def equal_words( self ) :
-        """
-        This method updates the word1Undiac and word2Undiac attributes by removing the first letter, and returns True if the words are equal, False otherwise. 
-
-        Returns:
-            :obj:`bool`: True if the words are equal, False otherwise.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication Implication
-
-            implication = Implication(word1, word2)
-            result = implication.equal_words()
-            if result:
-                print("The words are equal")
-            else:
-                print("The words are not equal")
-        """
-       # check if the tow words are the same taking into account the alif as the first letter 
-        word1FirstLetter = self.word1Undiac[0 : 1] # First letter in word1 
-        word2FirstLetter = self.word2Undiac[0 : 1] # First letter in word2 
-        self.word1Undiac =  self.word1Undiac[1 : ] # all word1 letters without diacritics except first letter 
-        self.word2Undiac =  self.word2Undiac[1 : ] # all word2 letters without diacritics except first letter 
-        
-        # If both words withot first letter are not equal return false, otherwise continue 
-        if ( self.word1Undiac != self.word2Undiac):
-            return False
-
-        # If the first letter in both words the same and (the other letters are the same) then return true, otherwise continue  
-        if word1FirstLetter == word2FirstLetter :
-            return True
-
-        # check if first letter is any alif (the other letters are the same) then return below values 
-        if (word1FirstLetter != "ا" or word2FirstLetter != "آ" and word2FirstLetter != "أ" and word2FirstLetter != "إ") :
-            if ((word1FirstLetter == "آ" or word1FirstLetter == "أ" or word1FirstLetter == "إ") and word2FirstLetter == "ا") :
-                self.lettersDirection[0] = 2 # w2 implies w1
-                self.conflictFlags[3] = True
-                return True
-            else:
-                return False
-        else:
-            self.lettersDirection[0] = 1 # w1 implies w2
-            self.conflictFlags[2] = True
-            return True
-        
-        return False
-
-       
-    def calculate_letters_implication(self) :
-        """
-        This method updates the lettersDirection, conflictFlags, and distance attributes based on the directionTable and distanceTable values for each pair of diacritics. It returns True after the calculation is completed.
-
-        Returns:
-            :obj:`bool`: True indicating the calculation is completed.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication
-
-            implication = Implication(word1, word2)
-            result = implication.calculate_letters_implication()
-            if result:
-                print("Letters implication calculation completed")
-        """
-        self.distance = 0
-        word1Diac = 0
-        word2Diac = 0
-  
-        for i in range ( 0 , len(self.word1Diacritics) - 1) :
-            word1Diac = self.word1Diacritics[i];
-            word2Diac = self.word2Diacritics[i];
-
-            self.lettersDirection[i + 1] = self.directionTable[word1Diac][word2Diac];
-            self.conflictFlags[self.lettersDirection[i + 1] + 1] = True;
-            self.distance = self.distance + self.distanceTable[word1Diac][word2Diac];
-
-               
-        word1Diac = int( self.word1Diacritics[len(self.word1Diacritics) - 1] ) # last letter diacritics to word1
-        word2Diac = int( self.word2Diacritics[len(self.word1Diacritics) - 1] ) # last letter diacritics to word2
-        # 8: expresses the presence of shaddah
-        if (word1Diac == 8 or word2Diac == 8) :
-            self.lettersDirection[len(self.lettersDirection) - 1] = self.directionTable[word1Diac][word2Diac]
-            self.conflictFlags[self.lettersDirection[len(self.lettersDirection) - 1] + 1] = True
-            self.distance = self.distance + self.distanceTable[word1Diac][word2Diac]
-        return True
-
-        
-    def calculate_direction(self ): 
-        """
-        This method calculates the direction of compatibility based on a conflict flags.
-
-        Returns:
-            :obj:`int`: The direction of compatibility:
-               -1: Incompatible-diacritics
-                0: Compatible-imply each other
-                1: Compatible-w1 implies w2
-                2: Compatible-w2 implies w1
-                3: Compatible-exactly equal
-                -2147483648: Default value for an invalid direction
-        """
-        self.conflicts = 0
-        if (self.conflictFlags[0] == True): 
-            return -1 # Incompatible-diacritics
-        
-        if (self.conflictFlags[2] == True and self.conflictFlags[3] == True ):
-            return 0 # Compatible-imply each other
-        
-        if (self.conflictFlags[2] == True and self.conflictFlags[3] == False ):
-            return 1 # Compatible-w1 implies w2
-        
-        if (self.conflictFlags[2] == False and self.conflictFlags[3] == True ):
-            return 2 # Compatible-w2 implies w1
-        
-        if (self.conflictFlags[4]):
-            return 3 # Compatible-exactly equal
-        return -2147483648
-
-
-
-    def get_diacritics_array(word): 
-        """
-        This method converts diacritics in a word to digits and returns the array of diacritics.
-
-        Args:
-            word (:obj:`str`): The word with diacritics.
-
-        Returns:
-            :obj:`list`: The array of diacritics converted to digits.
-
-        Raises:
-            Exception: If the first character of the word is a digit.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication
-            word = "مُرَحَّبًا"
-            diacritics = Implication.calculate_direction(word)
-            print(diacritics)
-            Output: [4, 3, 8, 5, 0]
-        """ 
-        # Replace diacritics by digits 
-        word = word.replace(" ", "") #Space
-        word = word.replace("ْ", "1") #SUKUN  
-        word = word.replace("َ", "2") #FATHA
-        word = word.replace("ِ", "3") #KASRA
-        word = word.replace("ُ", "4") #DAMMA
-        word = word.replace("ً", "5") #FATHATAN
-        word = word.replace("ٍ", "6") #KASRATAN
-        word = word.replace("ٌ", "7") #DAMMATAN
-        word = word.replace("ّ", "8") #SHADDA
-        word = word.replace("11", "100") #SUKUN with SUKUN
-        word = word.replace("12", "100") #SUKUN with FATHA
-        word = word.replace("13", "100") #SUKUN with KASRA
-        word = word.replace("14", "100") #SUKUN with DAMMA
-        word = word.replace("15", "100") #SUKUN with FATHATAN
-        word = word.replace("82", "9") #SHADDA with FATHA
-        word = word.replace("83", "10") #SHADDA with KASRA
-        word = word.replace("84", "11") #SHADDA with DAMMA
-          # Standardization Alif
-        word = word[0 : 1].replace("ا", "ا12,") + word[1: ] 
-        word = word[0 : 1].replace("أ", "ا13,") + word[1: ] 
-        word = word[0 : 1].replace("إ", "ا14,") + word[1: ] 
-        word = word[0 : 1].replace("آ", "ا15,") + word[1: ] 
-        if word[0:1].isdigit(): # Because a word should not begin with a diacritics 
-            raise Exception("Sorry, First char is digit")
-        else:
-            # word = re.sub(r'[\u0600-\u06FF]' , ",",word) # replace all chars with ,
-            for x in word: 
-                if ( ( x.isalpha() or not x.isdigit() ) and x != ',' ): # If char is not digit then replace it by , 
-                    word = word.replace(x , ",")
-            # word = word.replace("\\D", ",")
-            word = word[0 : len(word) - 1] + word[ len(word ) - 1].replace(",", ",,") # last letter does not have diacritic problem
-           
-            while ( ",," in word ):
-                word = word.replace(",,", ",0,") # No-DIACRITIC 
-            
-            word = word[1 : len(word) ] # Ignore the first letter diacritic 
-            diacritics = []
-            diacritics = word.split(",") # diacritics is array of diacritics
-            if '' in diacritics: # Remove empty index if exist
-                diacritics.remove('')
-            var3 = diacritics[len(diacritics) - 1] # last letter diacritic
-
-
-            # SHADDA with FATHA,SHADDA with KASRA,SHADDA with DAMMA,SHADDAH WITH FATHATAN,SHADDAH WITH KASRTA, SHADDAH WITH DHAMTAN
-            if var3 == "8" or var3 == "9" or var3 == "10" or var3 == "11" or var3 == "85" or var3 == "86" or var3 == "87":
-                diacritics[len(diacritics )- 1] = "8"
-                     # SUKUN , FATHA , KASRA , DAMMA , FATHATAN , KASRATAN , DAMMATAN 
-            elif var3 == "1" or var3 == "2" or var3 == "3" or var3 == "4" or var3 == "5" or var3 == "6" or var3 == "7":
-                diacritics[len(diacritics )- 1] = "0"
-        
-        strDiacritics = []
-        strDiacritics = diacritics
-        
-        # Convert string array digits to integer digits array 
-        for x in range(0 , len(strDiacritics) ):
-            diacritics[x] = int(strDiacritics[x])
-        return diacritics
-    
-    # def removeDiacritics( word ): # remove all diacritics from Arabic word
-    #     word = word.replace(" ", "")
-    #     word = word.replace("ْ", "") #SUKUN
-    #     word = word.replace("َ", "") #FATHA
-    #     word = word.replace("ِ", "") #KASRA
-    #     word = word.replace("ُ", "") #DAMMA
-    #     word = word.replace("ً", "") #FATHATAN
-    #     word = word.replace("ٍ", "") #KASRATAN
-    #     word = word.replace("ٌ", "") #DAMMATAN
-    #     word = word.replace("ّ", "") #SHADDA
-    #     return word
-
-    def get_letters_array(word):
-        """
-        This method returns the array of letters from a given word.
-
-        Args:
-            word (:obj:`str`): The word from which to extract the letters.
-
-        Returns:
-            obj:`list`: The array of letters.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication
-            word = "مرحبا"
-            letters = get_letters_array(word)
-            print(letters)
-            Output: ['م', 'ر', 'ح', 'ب', 'ا']
-        """
-        word = arStrip(word, diacs=False, shaddah=False)
-        return list(word)
-
-    def get_verdict(self ): 
-        return self.verdict
-
-
-    def get_direction(self): 
-        return self.direction
-
-
-    def get_distance(self) :
-        return self.distance
-
-
-    def get_conflicts(self) :
-        return self.conflicts
-
-
-    def get_word1(self) :
-        return self.word1
-
-
-    def get_word2(self) :
-        return self.word2 
-
-    def get_result(self):
-        """
-        This method returns the result of the comparison between two words.
-
-        Returns:
-            :obj:`str`: The result of the comparison. Can be *Same* or *Different*.
-
-        **Example:**
-
-        .. highlight:: python
-        .. code-block:: python
-
-            from nlptools.utils.implication import Implication
-            w1 = "hello"
-            w2 = "hell"
-            implication = Implication(w1, w2)
-            result = implication.get_result()
-            print(result)
-            Output: "Same"
-        """
-        if Implication.get_direction(self) >= 0 and Implication.get_distance(self) < 15:
-            self.result = "Same"
-        else:
-            self.result = "Different"
-        return self.result
-
-    def toString(self) :
-        return self.word1 + "\t" + self.word2 + "\t" + str(self.verdict) + "\t" + str(self.direction) + "\t" + str(self.distance) + "\t"+ str(self.conflicts)
-
+# Created: 16/03/2021 , By Mohammad A'bed
+# Trello task: https://trello.com/c/nHnmnFAe/19-re-implement-implication-function-in-python
+
+#  The Imply algorithm takes two words as input and produces the matching tuple defined by (Words Matching).
+#  The matching between two words is defined as a tuple:
+#  <w1, w2, implication direction, distance, conflicts, verdict, preferredWord> .
+
+from nlptools.utils.parser import arStrip
+class Implication:
+    """
+    The implication class computes whether the two Arabic words are the same or not, regardless of how they are diacritized. The output also contains implication direction, distance, number of conflicts, and other outputs. 
+    Argd:
+        :obj:`str' word1: input text
+        :obj:`str' word2: input text
+
+    """
+    # Diacritic Pair Distance Map
+    distanceTable = [
+    [0, 0, 1, 1, 1, 1, 1, 1, 15, 16, 16, 16, 0, 0, 0, 0 ],
+    [0, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
+    [1, 101, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
+    [1, 101, 101, 0, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
+    [1, 101, 101, 101, 0, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
+    [1, 101, 101, 101, 101, 0, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
+    [1, 101, 101, 101, 101, 101, 0, 101, 101, 101, 101, 101, 0, 0, 0, 0],
+    [1, 101, 101, 101, 101, 101, 101, 0, 101, 101, 101, 101, 0, 0, 0, 0],
+    [15, 101, 101, 101, 101, 101, 101, 101, 0, 1, 1, 1, 0, 0, 0, 0],
+    [16, 101, 101, 101, 101, 101, 101, 101, 1, 0, 101, 101, 0, 0, 0, 0],
+    [16, 101, 101, 101, 101, 101, 101, 101, 1, 101, 0, 101, 0, 0, 0, 0],
+    [16, 101, 101, 101, 101, 101, 101, 101, 1, 101, 101, 0, 0, 0, 0, 0],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 4, 4],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 0, 100, 100],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 100, 0, 100],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 4, 100, 100, 0]
+    ]
+
+    # Implication direction  Map
+    directionTable =[
+    [3, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0],
+    [2, 3, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
+    [2, -1, 3, -1, -1, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
+    [2, -1, -1, 3, -1, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
+    [2, -1, -1, -1, 3, -1, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
+    [2, -1, -1, -1, -1, 3, -1, -1, -1, -1, -1, -1, 0, 0, 0, 0],
+    [2, -1, -1, -1, -1, -1, 3, -1, -1, -1, -1, -1, 0, 0, 0, 0],
+    [2, -1, -1, -1, -1, -1, -1, 3, -1, -1, -1, -1, 0, 0, 0, 0],
+    [2, -1, -1, -1, -1, -1, -1, -1, 3, 1, 1, 1, 0, 0, 0, 0],
+    [2, -1, -1, -1, -1, -1, -1, -1, 2, 3, -1, -1, 0, 0, 0, 0],
+    [2, -1, -1, -1, -1, -1, -1, -1, 2, -1, 3, -1, 0, 0, 0, 0],
+    [2, -1, -1, -1, -1, -1, -1, -1, 2, -1, -1, 3, 0, 0, 0, 0],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 1, 1, 1],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 3, -1, -1],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, -1, 3, -1],
+    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, -1, -1, 3]
+    ]
+
+    word1 , word2 = "" , "" # two words to be compared
+    conflictFlags =  [False for i in range(5)] 
+    verdict = "null"    # verdict:  takes one of the values: “compatible”, or “incompatible”
+    word1Undiac = ""    # word1 without diacritics 
+    word2Undiac = ""    # word2 without diacritics 
+    word1Diacritics = [] # Diacritics array of the first word
+    word2Diacritics = [] # Diacritics array of the second word
+    direction = -2147483648 # direction: is a number denoting the relationship between the two words, the defult value is given a low integer, arbitrarry value
+    distance = -2147483648 # distance: denotes the overall similarity of the diacritization between the two words, which we compute based on the distance map; the defult value is given a low integer, arbitrarry value
+    conflicts = -2147483648 # conflict: denotes the number of conflicting diacritics between the two words, the defult value is given a low integer, arbitrarry value
+    lettersDirection = [] # implication direction between diacritics 
+
+    def __init__(self , inputWord1 ,  inputWord2):
+        
+        #check if inputWord1 or inputWord2 is empty, then return the values below
+        if ( (not inputWord1) and (inputWord2) ) or  ( ( inputWord1) and (not inputWord2) ):
+            self.verdict = "Incompatible"
+            self.direction = -3 # the two words have different letters
+            self.distance = 3000
+            self.conflicts = 0
+            return
+
+        self.conflictFlags =  [False for i in range(5)] # reset conflictFlags array to Fales
+        self.word1 = Implication.normalize_alef(inputWord1) # unify alif 
+        self.word2 = Implication.normalize_alef(inputWord2) # unify alif 
+
+        if ( self.word1 ==  self.word2): # If w1 == w2 returns the values bellow 
+            self.verdict = "Compatible"
+            self.direction = 3 #  Both letters have exactly the same diacritics 
+            self.distance = 0
+            self.conflicts = 0
+            return
+        else: # If w1 and w2 are noot exact match
+            try:
+                self.lettersDirection = []
+                # build diacritics array for each word 
+                self.word1Diacritics = Implication.get_diacritics_array(self.word1)
+                self.word2Diacritics = Implication.get_diacritics_array(self.word2)
+
+                 # defined lettersDirection array with size of word1Diacritics and fill it by zeros
+                for x in range(0 , len(self.word1Diacritics) + 1): 
+                    self.lettersDirection.append(0)
+            except :
+                # In case of errors returns the values below 
+                self.verdict = "Incompatible"
+                self.direction = -3 # the two words have different letters
+                self.distance = 3000
+                self.conflicts = 0
+                return
+
+            # check if diacritics in both words for some of syntax errors then return Incompatible
+            if (  Implication.diacritics_syntax_error_in(self.word1Diacritics) == False and  Implication.diacritics_syntax_error_in(self.word2Diacritics) == False) : 
+                # If no syntax error found:
+                self.word1Undiac = arStrip(self.word1, diacs=False, shaddah=False)
+                self.word2Undiac = arStrip(self.word2, diacs=False, shaddah=False)
+                # return compatible if each word is one and same letter regardless of diacritics on this letter
+                if (len(self.word1Undiac) == 1 and len(self.word2Undiac) == 1 and self.word1Undiac == self.word2Undiac): 
+                        self.verdict = "Compatible"
+                        self.direction = 3  #  Both letters have exactly the same diacritics 
+                        self.distance = 0
+                        self.conflicts = 0
+                else : # If words are more than letter or deffirent letter then calculate the impication
+                    self.lettersDirection[0] = 3 
+                    self.calculate_words_implication()
+                
+            else : # If found syntax error in diacitics in word1 or word2 then return these:
+                self.verdict = "Incompatible"
+                self.direction = -3 # the two words have different letters
+                self.distance = 3000
+                self.conflicts = 0
+            
+    def get_non_preferred_word(self, word1, word2):
+        """
+        This method returns the non-preferred word from two given words.
+
+        Args:
+            :obj:`str' word1: The first word.
+            :obj:`str' word2: The second word.
+
+        Returns:
+            :obj:`str': The non-preferred word.
+
+        Raises:
+            None
+        """
+        # this function talkes 2-words and retuen preferredWord 
+        word1 = word1.strip()
+        word2 = word2.strip()
+        if (word1 != None and  word1 ) :
+            if (word2 != None and word2) :
+                preferredWord = ""
+                preferredWord = Implication.getPreferredWord(word1, word2)
+                if word1== preferredWord:
+                    return word2
+                else:
+                    return word1
+            else :
+                return word1
+        
+        else :
+            if word2 != None and word2:
+                return word2 
+            else:
+                return None
+    
+
+
+    def get_preferred_word( self , word1,   word2) :
+        """
+        This method returns the preferred word from two given words.
+
+        Args:
+            :obj:`str' word1: The first word.
+            :obj:`str' word2: The second word.
+
+        Returns:
+            :obj:`str': The preferred word.
+
+        Raises:
+            None
+        """        
+        word1 = word1.strip()
+        word2 = word2.strip()
+        if ( word1 != None and word1) :
+            if (word2 != None and word2) :
+                implication =  Implication(word1, word2) 
+                direction = implication.get_distance()
+                if (direction < 15) :
+                    if ( ( direction == 0 ) or
+                       (direction == 2 ) ):
+                        return word1
+                    elif direction == 1 :
+                        return word2
+                    elif direction == 3 :
+                        if ( ( not word1.endswith("َ") ) and ( not word1.endswith("ُ") ) ) : 
+                            return word2
+                        return word1
+
+                return ""
+            else :
+                return word1
+        
+        else :
+            if word2 != None and (not word2):
+                return  word2
+            else:
+                return None
+            
+    def normalize_alef(word):
+        """
+        This method normalizes the alif (ألف) character in the given word.
+
+        Args:
+            word (:obj:`str`): The input word to be normalized.
+
+        Returns:
+            :obj:`str`: The normalized word with alif characters modified.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+
+            word = Implication.normalize_alef("ًى")  # Returns "ىً"
+            word = Implication.normalize_alef("ًا")  # Returns "اً"
+            word = Implication.normalize_alef("ٱلكتاب")  # Returns "الكتاب"
+        """
+        # If the tanween is before the alif, then it is placed after it,
+        # because in the Arabic language this word is similar
+        if word.endswith("ًى"):
+            word = word[:len(word) - 2] + "ىً"
+
+        if word.endswith("ًا"):
+            word = word[:len(word) - 2] + "اً"
+        # Replace Alif-dhamma with Alif
+        if word.startswith("ٱ"):
+            word = "ا" + word[1:]
+        return word
+
+
+    def diacritics_syntax_error_in( diacriticsArray ) :
+        """
+        This method checks if the diacritics in a given array are incorrect.
+
+        Args:
+            diacritics_array (:obj:`list`): A list of diacritics to be checked.
+
+        Returns:
+            :obj:`bool`: True if there is a syntax error in the diacritics, False otherwise.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication 
+
+            diacritics = ["َ", "ُ", "ِ", "ّ"]
+            has_error = Implication.diacritics_syntax_error_in(diacritics)  # Returns False
+
+            diacritics = ["َ", "ُ", "ِ", "ٓ"]
+            has_error = Implication.diacritics_syntax_error_in(diacritics)  # Returns True
+        """
+        # This funcion return True when the diacritics is incorreclty 
+        try:
+            # check last letter diacritic
+            if ( Implication.wrong_end_diacritic(diacriticsArray[ len(diacriticsArray) - 1]) ) : 
+                return True
+            else :
+                # check All letters diacritic except the last letter diacritic
+                for i in range(0 , len(diacriticsArray) - 1 ) :
+                    if (Implication.wrong_middle_iacritic(diacriticsArray[i])) :
+                        return True 
+                return False
+            
+        except :
+            return False
+        
+
+    def wrong_end_diacritic(diac):
+        """
+        This method checks if the given diacritic is a wrong end diacritic.
+
+        Args:
+            diac (:obj:`int`): The diacritic value to be checked.
+
+        Returns:
+            :obj:`bool`: True if the diacritic is one of the follwoing number (85:SHADDAH WITH FATHATAN, 86:SHADDAH WITH KASRTA, 87:SHADDAH WITH DHAMTAN), False if diacritic is greator than or equal0 and diacritic is less than or equal 11.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication 
+
+            diacritic = 0
+            is_wrong_end = Implication.wrong_end_diacritic(diacritic)  # Returns False
+
+            diacritic = 85
+            is_wrong_end = Implication.wrong_end_diacritic(diacritic)  # Returns True
+        """
+        # 0 > No Diacritics , 1 > SUKUN, 2 > FATHA, 3 > KASRA, 4 > DAMMA, 5 > FATHATAN, 6 > KASRATAN,
+        #  7 > DAMMATAN, 8 > SHADDA, 9 > SHADDA with FATHA, 10 > SHADDA with KASRA, 11 > SHADDA with DAMMA
+        if (diac >= 0 and diac <= 11) :
+            return False
+        else :
+            # 85 - 86 - 87: SHADDAH WITH FATHATAN,SHADDAH WITH KASRTA, SHADDAH WITH DHAMTAN
+            return diac < 85 or diac > 87
+        
+    def wrong_middle_iacritic( diac) :
+
+        if (diac >= 0 and diac <= 4) :
+            return False
+        else :
+            return diac < 8 or diac > 15
+            
+    
+    def calculate_words_implication(self):
+        """
+        This method calculates the implication between two words, and updates the verdict, direction, distance, and conflicts attributes of the object based on the implication between the words.
+
+        Returns:
+            None
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+
+            implication = Implication(word1, word2)
+            implication.calculate_words_implication()
+            # Access the updated attributes
+            verdict = implication.verdict
+            direction = implication.direction
+            distance = implication.distance
+            conflicts = implication.conflicts
+        """
+
+        self.verdict = "Incompatible"
+        self.direction = -2 
+        self.distance = 1000
+        if (Implication.equal_words(self) == False): # If both words are not thge same return these values 
+            if ((len(self.word1Undiac) == 0 and len(self.word2Undiac) == 0)):
+                if (self.word1 == self.word2): 
+                    self.conflicts = 0
+                    self.distance = 0
+                    self.direction = 3 
+                else:
+                    self.conflicts = 1
+                    self.distance = 1000
+                    self.direction = -2 
+                
+            else:
+                self.conflicts = max(len(self.word1Undiac), len(self.word2Undiac))
+            
+        else:
+            if (Implication.calculate_letters_implication(self)):
+                self.direction = Implication.calculate_direction(self)
+                if (self.direction == -1) :
+                    self.distance = 101
+                else:
+                    self.verdict = "Compatible"
+                
+            else:
+                self.direction = -3 # the two words have different letters
+                self.distance = 3000
+                self.conflicts = 0
+
+    def equal_words( self ) :
+        """
+        This method updates the word1Undiac and word2Undiac attributes by removing the first letter, and returns True if the words are equal, False otherwise. 
+
+        Returns:
+            :obj:`bool`: True if the words are equal, False otherwise.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication Implication
+
+            implication = Implication(word1, word2)
+            result = implication.equal_words()
+            if result:
+                print("The words are equal")
+            else:
+                print("The words are not equal")
+        """
+       # check if the tow words are the same taking into account the alif as the first letter 
+        word1FirstLetter = self.word1Undiac[0 : 1] # First letter in word1 
+        word2FirstLetter = self.word2Undiac[0 : 1] # First letter in word2 
+        self.word1Undiac =  self.word1Undiac[1 : ] # all word1 letters without diacritics except first letter 
+        self.word2Undiac =  self.word2Undiac[1 : ] # all word2 letters without diacritics except first letter 
+        
+        # If both words withot first letter are not equal return false, otherwise continue 
+        if ( self.word1Undiac != self.word2Undiac):
+            return False
+
+        # If the first letter in both words the same and (the other letters are the same) then return true, otherwise continue  
+        if word1FirstLetter == word2FirstLetter :
+            return True
+
+        # check if first letter is any alif (the other letters are the same) then return below values 
+        if (word1FirstLetter != "ا" or word2FirstLetter != "آ" and word2FirstLetter != "أ" and word2FirstLetter != "إ") :
+            if ((word1FirstLetter == "آ" or word1FirstLetter == "أ" or word1FirstLetter == "إ") and word2FirstLetter == "ا") :
+                self.lettersDirection[0] = 2 # w2 implies w1
+                self.conflictFlags[3] = True
+                return True
+            else:
+                return False
+        else:
+            self.lettersDirection[0] = 1 # w1 implies w2
+            self.conflictFlags[2] = True
+            return True
+        
+        return False
+
+       
+    def calculate_letters_implication(self) :
+        """
+        This method updates the lettersDirection, conflictFlags, and distance attributes based on the directionTable and distanceTable values for each pair of diacritics. It returns True after the calculation is completed.
+
+        Returns:
+            :obj:`bool`: True indicating the calculation is completed.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+
+            implication = Implication(word1, word2)
+            result = implication.calculate_letters_implication()
+            if result:
+                print("Letters implication calculation completed")
+        """
+        self.distance = 0
+        word1Diac = 0
+        word2Diac = 0
+  
+        for i in range ( 0 , len(self.word1Diacritics) - 1) :
+            word1Diac = self.word1Diacritics[i];
+            word2Diac = self.word2Diacritics[i];
+
+            self.lettersDirection[i + 1] = self.directionTable[word1Diac][word2Diac];
+            self.conflictFlags[self.lettersDirection[i + 1] + 1] = True;
+            self.distance = self.distance + self.distanceTable[word1Diac][word2Diac];
+
+               
+        word1Diac = int( self.word1Diacritics[len(self.word1Diacritics) - 1] ) # last letter diacritics to word1
+        word2Diac = int( self.word2Diacritics[len(self.word1Diacritics) - 1] ) # last letter diacritics to word2
+        # 8: expresses the presence of shaddah
+        if (word1Diac == 8 or word2Diac == 8) :
+            self.lettersDirection[len(self.lettersDirection) - 1] = self.directionTable[word1Diac][word2Diac]
+            self.conflictFlags[self.lettersDirection[len(self.lettersDirection) - 1] + 1] = True
+            self.distance = self.distance + self.distanceTable[word1Diac][word2Diac]
+        return True
+
+        
+    def calculate_direction(self ): 
+        """
+        This method calculates the direction of compatibility based on a conflict flags.
+
+        Returns:
+            :obj:`int`: The direction of compatibility:
+               -1: Incompatible-diacritics
+                0: Compatible-imply each other
+                1: Compatible-w1 implies w2
+                2: Compatible-w2 implies w1
+                3: Compatible-exactly equal
+                -2147483648: Default value for an invalid direction
+        """
+        self.conflicts = 0
+        if (self.conflictFlags[0] == True): 
+            return -1 # Incompatible-diacritics
+        
+        if (self.conflictFlags[2] == True and self.conflictFlags[3] == True ):
+            return 0 # Compatible-imply each other
+        
+        if (self.conflictFlags[2] == True and self.conflictFlags[3] == False ):
+            return 1 # Compatible-w1 implies w2
+        
+        if (self.conflictFlags[2] == False and self.conflictFlags[3] == True ):
+            return 2 # Compatible-w2 implies w1
+        
+        if (self.conflictFlags[4]):
+            return 3 # Compatible-exactly equal
+        return -2147483648
+
+
+
+    def get_diacritics_array(word): 
+        """
+        This method converts diacritics in a word to digits and returns the array of diacritics.
+
+        Args:
+            word (:obj:`str`): The word with diacritics.
+
+        Returns:
+            :obj:`list`: The array of diacritics converted to digits.
+
+        Raises:
+            Exception: If the first character of the word is a digit.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+            word = "مُرَحَّبًا"
+            diacritics = Implication.calculate_direction(word)
+            print(diacritics)
+            Output: [4, 3, 8, 5, 0]
+        """ 
+        # Replace diacritics by digits 
+        word = word.replace(" ", "") #Space
+        word = word.replace("ْ", "1") #SUKUN  
+        word = word.replace("َ", "2") #FATHA
+        word = word.replace("ِ", "3") #KASRA
+        word = word.replace("ُ", "4") #DAMMA
+        word = word.replace("ً", "5") #FATHATAN
+        word = word.replace("ٍ", "6") #KASRATAN
+        word = word.replace("ٌ", "7") #DAMMATAN
+        word = word.replace("ّ", "8") #SHADDA
+        word = word.replace("11", "100") #SUKUN with SUKUN
+        word = word.replace("12", "100") #SUKUN with FATHA
+        word = word.replace("13", "100") #SUKUN with KASRA
+        word = word.replace("14", "100") #SUKUN with DAMMA
+        word = word.replace("15", "100") #SUKUN with FATHATAN
+        word = word.replace("82", "9") #SHADDA with FATHA
+        word = word.replace("83", "10") #SHADDA with KASRA
+        word = word.replace("84", "11") #SHADDA with DAMMA
+          # Standardization Alif
+        word = word[0 : 1].replace("ا", "ا12,") + word[1: ] 
+        word = word[0 : 1].replace("أ", "ا13,") + word[1: ] 
+        word = word[0 : 1].replace("إ", "ا14,") + word[1: ] 
+        word = word[0 : 1].replace("آ", "ا15,") + word[1: ] 
+        if word[0:1].isdigit(): # Because a word should not begin with a diacritics 
+            raise Exception("Sorry, First char is digit")
+        else:
+            # word = re.sub(r'[\u0600-\u06FF]' , ",",word) # replace all chars with ,
+            for x in word: 
+                if ( ( x.isalpha() or not x.isdigit() ) and x != ',' ): # If char is not digit then replace it by , 
+                    word = word.replace(x , ",")
+            # word = word.replace("\\D", ",")
+            word = word[0 : len(word) - 1] + word[ len(word ) - 1].replace(",", ",,") # last letter does not have diacritic problem
+           
+            while ( ",," in word ):
+                word = word.replace(",,", ",0,") # No-DIACRITIC 
+            
+            word = word[1 : len(word) ] # Ignore the first letter diacritic 
+            diacritics = []
+            diacritics = word.split(",") # diacritics is array of diacritics
+            if '' in diacritics: # Remove empty index if exist
+                diacritics.remove('')
+            var3 = diacritics[len(diacritics) - 1] # last letter diacritic
+
+
+            # SHADDA with FATHA,SHADDA with KASRA,SHADDA with DAMMA,SHADDAH WITH FATHATAN,SHADDAH WITH KASRTA, SHADDAH WITH DHAMTAN
+            if var3 == "8" or var3 == "9" or var3 == "10" or var3 == "11" or var3 == "85" or var3 == "86" or var3 == "87":
+                diacritics[len(diacritics )- 1] = "8"
+                     # SUKUN , FATHA , KASRA , DAMMA , FATHATAN , KASRATAN , DAMMATAN 
+            elif var3 == "1" or var3 == "2" or var3 == "3" or var3 == "4" or var3 == "5" or var3 == "6" or var3 == "7":
+                diacritics[len(diacritics )- 1] = "0"
+        
+        strDiacritics = []
+        strDiacritics = diacritics
+        
+        # Convert string array digits to integer digits array 
+        for x in range(0 , len(strDiacritics) ):
+            diacritics[x] = int(strDiacritics[x])
+        return diacritics
+    
+    # def removeDiacritics( word ): # remove all diacritics from Arabic word
+    #     word = word.replace(" ", "")
+    #     word = word.replace("ْ", "") #SUKUN
+    #     word = word.replace("َ", "") #FATHA
+    #     word = word.replace("ِ", "") #KASRA
+    #     word = word.replace("ُ", "") #DAMMA
+    #     word = word.replace("ً", "") #FATHATAN
+    #     word = word.replace("ٍ", "") #KASRATAN
+    #     word = word.replace("ٌ", "") #DAMMATAN
+    #     word = word.replace("ّ", "") #SHADDA
+    #     return word
+
+    def get_letters_array(word):
+        """
+        This method returns the array of letters from a given word.
+
+        Args:
+            word (:obj:`str`): The word from which to extract the letters.
+
+        Returns:
+            obj:`list`: The array of letters.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+            word = "مرحبا"
+            letters = get_letters_array(word)
+            print(letters)
+            Output: ['م', 'ر', 'ح', 'ب', 'ا']
+        """
+        word = arStrip(word, diacs=False, shaddah=False)
+        return list(word)
+
+    def get_verdict(self ): 
+        return self.verdict
+
+
+    def get_direction(self): 
+        return self.direction
+
+
+    def get_distance(self) :
+        return self.distance
+
+
+    def get_conflicts(self) :
+        return self.conflicts
+
+
+    def get_word1(self) :
+        return self.word1
+
+
+    def get_word2(self) :
+        return self.word2 
+
+    def get_result(self):
+        """
+        This method returns the result of the comparison between two words.
+
+        Returns:
+            :obj:`str`: The result of the comparison. Can be *Same* or *Different*.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+            w1 = "hello"
+            w2 = "hell"
+            implication = Implication(w1, w2)
+            result = implication.get_result()
+            print(result)
+            Output: "Same"
+        """
+        if Implication.get_direction(self) >= 0 and Implication.get_distance(self) < 15:
+            self.result = "Same"
+        else:
+            self.result = "Different"
+        return self.result
+
+    def toString(self) :
+        return self.word1 + "\t" + self.word2 + "\t" + str(self.verdict) + "\t" + str(self.direction) + "\t" + str(self.distance) + "\t"+ str(self.conflicts)
+
```

### Comparing `nlptoolssna-0.9.2/nlptools/utils/jaccard.py` & `nlptoolssna-0.9.3/nlptools/utils/jaccard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Dec  1 14:22:26 2021
-
-@author: Tymaa
-"""
-
-from nlptools.utils.parser import arStrip
-from nlptools.utils.implication import Implication
-
-
-def normalize_word(word: str, ignore_all_diacritics_but_not_shadda: bool=True, ignore_shadda_diacritic: bool=True) -> str:
-    """
-    Normalize a given Arabic word by removing diacritics and/or shadda diacritic.
-
-    Args:
-        word (:obj:`str`): The input text.
-        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A boolean flag indicating whether to remove all diacritics except shadda (default is True). 
-        ignore_shadda_diacritic (:obj:`bool`): A boolean flag indicating whether to remove shadda diacritic (default is True).
-
-    Returns:
-          :obj:`str` Normalized Arabic word.
-    """
-    if ignore_all_diacritics_but_not_shadda:
-        word = arStrip(word, True, True, False, False, False, False)
-        
-    if ignore_shadda_diacritic:
-        word = arStrip(word, False, False, True, False, False, False)
-    
-    return word
-
-    
-def get_preferred_word(word1, word2):
-    """
-    Returns the preferred word among two given words based on their implication.
-
-    Args:
-        word1 (:obj:`str`): The first word.
-        word2 (:obj:`str`): The second word.
-
-    Returns:
-        :obj:`str`: The preferred word among the two given words.
-    
-    """
-    implication = Implication(word1, word2)
-    
-    direction = implication.get_direction()
-    
-    if direction in (0, 2):
-        return word1
-       
-    elif direction == 1:
-        return word2
-       
-    elif direction == 3:
-        if not word1.endswith("َ") and not word1.endswith("ُ"):
-            return word2
-        return word1
-     
-    
-def get_non_preferred_word(word1, word2):
-    """
-    Returns the non-preferred word between the two input words.
-
-    Args:
-        word1 (:obj:`str`): The first word.
-        word2 (:obj:`str`): The second word.
-
-    Returns:
-        :obj:`str`: The non-preferred word. If there is no non-preferred word, The '#' is returned.
-
-    """
-
-    implication = Implication(word1, word2)
-    if implication.get_distance() < 15:
-        direction = implication.get_direction()
-        if direction == 0 or direction == 1:
-            return word1
-        elif direction == 2:
-            return word2
-        elif direction == 3:
-            if not word1.endswith("َ") and not word1.endswith("ُ"):
-                return word1
-            return word2
-    return "#"
-@TBD
-def get_intersection(list1, list2, ignore_all_diacritics_but_not_shadda=False, ignore_shadda_diacritic=False):
-    """
-    Get the intersection of two lists after normalization and ignoring diacritics based on input flags.
-
-    Args:
-        list1 (:obj:`list`): The first list.
-        list2 (:obj:`list`): The second list.
-        ignore_all_diacritics_but_not_shadda (:obj:`bool`, optional): A flag to ignore all diacritics except for the shadda. Defaults to False.
-        ignore_shadda_diacritic (:obj:`bool`, optional): A flag to ignore the shadda diacritic. Defaults to False.
-
-    Returns:
-         :obj:`list`: The intersection of the two lists after normalization and ignoring diacritics.
-
-    """
-
-    # Remove all None and empty values from first list
-    list1 = [str(i) for i in list1 if i not in (None, ' ', '')]
-    list1 = [str(i.strip()) for i in list1]
-
-    # Remove all None and empty values from second list
-    list2 = [str(i) for i in list2 if i not in (None, ' ', '')]
-    list2 = [str(i.strip()) for i in list2]
-
-    interection_list = []
-
-    # Add all Common words between the two list1 and list2 to interectionList
-    for list1_word in list1:
-        for list2_word in list2:
-            word1 = normalize_word(list1_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
-            word2 = normalize_word(list2_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
-
-            implication = Implication(word1, word2)
-            if implication.get_direction() >= 0 and implication.get_distance() < 15:
-                interection_list.append(get_preferred_word(word1, word2))
-
-    i = 0
-    while i < len(interection_list):
-        j = i + 1
-        while j < len(interection_list):
-            non_preferred_word = get_non_preferred_word(interection_list[i], interection_list[j])
-            if non_preferred_word != "#":
-                interection_list.remove(non_preferred_word)
-            j += 1
-        i += 1
-
-    return interection_list
-             
-
-
-def get_union(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic):
-    """
-    Finds the union of two lists by removing duplicates and normalizing words.
-
-    Args:
-        list1 (:obj:`list`): The first list.
-        list2 (:obj:`list`): The second list.
-        ignore_all_diacritics_but_not_shadda (:obj:`bool`): Whether to ignore all diacritics except shadda or not.
-        ignore_shadda_diacritic (:obj:`bool`): Whether to ignore shadda diacritic or not.
-   Returns:
-         :obj:`list`: The union of the two lists after removing duplicates and normalizing words.
-    """
-
-    list1 = [str(i) for i in list1 if i not in (None, ' ', '')]
-
-    list2 = [str(i) for i in list2 if i not in (None, ' ', '')]
-
-    union_list = []
-
-    for list1_word in list1:
-        word1 = normalize_word(list1_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
-        union_list.append(word1)
-
-    for list2_word in list2:
-        word2 = normalize_word(list2_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
-        union_list.append(word2)
-
-    i = 0
-    while i < len(union_list):
-        j = i + 1
-        while j < len(union_list):
-            non_preferred_word = get_non_preferred_word(union_list[i], union_list[j])
-            if (non_preferred_word != "#"):
-                union_list.remove(non_preferred_word)
-            j = j + 1
-        i = i + 1
-
-    return union_list
-      
-
-
-def jaccard_similarity(list1: list, list2: list, ignore_all_diacritics_but_not_shadda: bool, ignore_shadda_diacritic: bool) -> float:
-    """
-    Calculates the Jaccard similarity coefficient between two lists.
-
-    Args:
-        list1 (:obj:`list`): The first list.
-        list2 (:obj:`list`): The second list.
-        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A flag indicating whether to ignore all diacritics except for shadda.
-        ignore_shadda_diacritic (:obj:`bool`): A flag indicating whether to ignore the shadda diacritic.
-
-    Returns:
-         :obj:`float`: The Jaccard similarity coefficient between the two lists.
-    """
-    # Find the intersection between two sets
-    intersection_list = get_intersection(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
-    
-    # Find the union between two sets
-    union_list = get_union(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
-    
-    # Calculate the Jaccard similarity coefficient by dividing the length of the intersectionList by the length of the unionList
-    return float(len(intersection_list)) / float(len(union_list))
-   
-
-
-
-def jaccard(delimiter, str1, str2, selection, ignoreAllDiacriticsButNotShadda=True, ignoreShaddaDiacritic=True):
-    """
-    Compute the Jaccard similarity, union, or intersection of two sets of strings.
-
-    Args:
-        delimiter (:obj:`str`): The delimiter used to split the input strings.
-        str1 (:obj:`str`): The first input string to compare.
-        str2 (:obj:`str`): The second input string to compare.
-        selection (:obj:`str`): The desired operation to perform on the two sets of strings. 
-                         Must be one of *intersection*, *union*, *jaccardSimilarity*, or *jaccardAll*.
-        ignoreAllDiacriticsButNotShadda (:obj:`bool`): If True, ignore all diacritics except for the Shadda diacritic. (Defualt is True)
-        ignoreShaddaDiacritic (:obj:`bool`): If True, ignore the Shadda diacritic.(Default is True)
-
-    Returns:
-        The Jaccard similarity, union, or intersection of the two sets of strings, 
-        depending on the value of the `selection` argument.
-    
-    Note:
-        - If `selection` is *jaccardAll*, a list of the intersection, union, and Jaccard similarity 
-        of the two sets of strings will be returned.
-        - If an error occurs, the method will return the string "An error has occurred".
-          Online tool: https://sina.birzeit.edu/resources/jaccardFunction.html
-    """
-    try:
-        list1 = str1.split(delimiter)
-        list2 = str2.split(delimiter)
-
-        if selection == "intersection":
-            intersection = get_intersection(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
-            return intersection
-        elif selection == "union":
-            union = get_union(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
-            return union
-        elif selection == "jaccardSimilarity":      
-            similarity = jaccard_similarity(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
-            return similarity
-        elif selection == "jaccardAll":    
-            intersection = get_intersection(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
-            union = get_union(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
-            similarity = jaccard_similarity(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
-            output_list = ["intersection:", intersection, "union:", union, "similarity:", similarity]
-            return output_list
-        else:
-            return 'Invalid selection option'
-
-    except AttributeError as ae:
-        print(f"Attribute error occurred: {str(ae)}")
-        return 'Invalid input type'
-    except Exception as e:
-        print(f"Error occurred: {str(e)}")
-        return 'An error has occurred'
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Dec  1 14:22:26 2021
+
+@author: Tymaa
+"""
+
+from nlptools.utils.parser import arStrip
+from nlptools.utils.implication import Implication
+
+
+def normalize_word(word: str, ignore_all_diacritics_but_not_shadda: bool=True, ignore_shadda_diacritic: bool=True) -> str:
+    """
+    Normalize a given Arabic word by removing diacritics and/or shadda diacritic.
+
+    Args:
+        word (:obj:`str`): The input text.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A boolean flag indicating whether to remove all diacritics except shadda (default is True). 
+        ignore_shadda_diacritic (:obj:`bool`): A boolean flag indicating whether to remove shadda diacritic (default is True).
+
+    Returns:
+          :obj:`str` Normalized Arabic word.
+    """
+    if ignore_all_diacritics_but_not_shadda:
+        word = arStrip(word, True, True, False, False, False, False)
+        
+    if ignore_shadda_diacritic:
+        word = arStrip(word, False, False, True, False, False, False)
+    
+    return word
+
+    
+def get_preferred_word(word1, word2):
+    """
+    Returns the preferred word among two given words based on their implication.
+
+    Args:
+        word1 (:obj:`str`): The first word.
+        word2 (:obj:`str`): The second word.
+
+    Returns:
+        :obj:`str`: The preferred word among the two given words.
+    
+    """
+    implication = Implication(word1, word2)
+    
+    direction = implication.get_direction()
+    
+    if direction in (0, 2):
+        return word1
+       
+    elif direction == 1:
+        return word2
+       
+    elif direction == 3:
+        if not word1.endswith("َ") and not word1.endswith("ُ"):
+            return word2
+        return word1
+     
+    
+def get_non_preferred_word(word1, word2):
+    """
+    Returns the non-preferred word between the two input words.
+
+    Args:
+        word1 (:obj:`str`): The first word.
+        word2 (:obj:`str`): The second word.
+
+    Returns:
+        :obj:`str`: The non-preferred word. If there is no non-preferred word, The '#' is returned.
+
+    """
+
+    implication = Implication(word1, word2)
+    if implication.get_distance() < 15:
+        direction = implication.get_direction()
+        if direction == 0 or direction == 1:
+            return word1
+        elif direction == 2:
+            return word2
+        elif direction == 3:
+            if not word1.endswith("َ") and not word1.endswith("ُ"):
+                return word1
+            return word2
+    return "#"
+#@TBD
+def get_intersection(list1, list2, ignore_all_diacritics_but_not_shadda=False, ignore_shadda_diacritic=False):
+    """
+    Get the intersection of two lists after normalization and ignoring diacritics based on input flags.
+
+    Args:
+        list1 (:obj:`list`): The first list.
+        list2 (:obj:`list`): The second list.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`, optional): A flag to ignore all diacritics except for the shadda. Defaults to False.
+        ignore_shadda_diacritic (:obj:`bool`, optional): A flag to ignore the shadda diacritic. Defaults to False.
+
+    Returns:
+         :obj:`list`: The intersection of the two lists after normalization and ignoring diacritics.
+
+    """
+
+    # Remove all None and empty values from first list
+    list1 = [str(i) for i in list1 if i not in (None, ' ', '')]
+    list1 = [str(i.strip()) for i in list1]
+
+    # Remove all None and empty values from second list
+    list2 = [str(i) for i in list2 if i not in (None, ' ', '')]
+    list2 = [str(i.strip()) for i in list2]
+
+    interection_list = []
+
+    # Add all Common words between the two list1 and list2 to interectionList
+    for list1_word in list1:
+        for list2_word in list2:
+            word1 = normalize_word(list1_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
+            word2 = normalize_word(list2_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
+
+            implication = Implication(word1, word2)
+            if implication.get_direction() >= 0 and implication.get_distance() < 15:
+                interection_list.append(get_preferred_word(word1, word2))
+
+    i = 0
+    while i < len(interection_list):
+        j = i + 1
+        while j < len(interection_list):
+            non_preferred_word = get_non_preferred_word(interection_list[i], interection_list[j])
+            if non_preferred_word != "#":
+                interection_list.remove(non_preferred_word)
+            j += 1
+        i += 1
+
+    return interection_list
+             
+
+
+def get_union(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic):
+    """
+    Finds the union of two lists by removing duplicates and normalizing words.
+
+    Args:
+        list1 (:obj:`list`): The first list.
+        list2 (:obj:`list`): The second list.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`): Whether to ignore all diacritics except shadda or not.
+        ignore_shadda_diacritic (:obj:`bool`): Whether to ignore shadda diacritic or not.
+   Returns:
+         :obj:`list`: The union of the two lists after removing duplicates and normalizing words.
+    """
+
+    list1 = [str(i) for i in list1 if i not in (None, ' ', '')]
+
+    list2 = [str(i) for i in list2 if i not in (None, ' ', '')]
+
+    union_list = []
+
+    for list1_word in list1:
+        word1 = normalize_word(list1_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
+        union_list.append(word1)
+
+    for list2_word in list2:
+        word2 = normalize_word(list2_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
+        union_list.append(word2)
+
+    i = 0
+    while i < len(union_list):
+        j = i + 1
+        while j < len(union_list):
+            non_preferred_word = get_non_preferred_word(union_list[i], union_list[j])
+            if (non_preferred_word != "#"):
+                union_list.remove(non_preferred_word)
+            j = j + 1
+        i = i + 1
+
+    return union_list
+      
+
+
+def jaccard_similarity(list1: list, list2: list, ignore_all_diacritics_but_not_shadda: bool, ignore_shadda_diacritic: bool) -> float:
+    """
+    Calculates the Jaccard similarity coefficient between two lists.
+
+    Args:
+        list1 (:obj:`list`): The first list.
+        list2 (:obj:`list`): The second list.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A flag indicating whether to ignore all diacritics except for shadda.
+        ignore_shadda_diacritic (:obj:`bool`): A flag indicating whether to ignore the shadda diacritic.
+
+    Returns:
+         :obj:`float`: The Jaccard similarity coefficient between the two lists.
+    """
+    # Find the intersection between two sets
+    intersection_list = get_intersection(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
+    
+    # Find the union between two sets
+    union_list = get_union(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
+    
+    # Calculate the Jaccard similarity coefficient by dividing the length of the intersectionList by the length of the unionList
+    return float(len(intersection_list)) / float(len(union_list))
+   
+
+
+
+def jaccard(delimiter, str1, str2, selection, ignoreAllDiacriticsButNotShadda=True, ignoreShaddaDiacritic=True):
+    """
+    Compute the Jaccard similarity, union, or intersection of two sets of strings.
+
+    Args:
+        delimiter (:obj:`str`): The delimiter used to split the input strings.
+        str1 (:obj:`str`): The first input string to compare.
+        str2 (:obj:`str`): The second input string to compare.
+        selection (:obj:`str`): The desired operation to perform on the two sets of strings. 
+                         Must be one of *intersection*, *union*, *jaccardSimilarity*, or *jaccardAll*.
+        ignoreAllDiacriticsButNotShadda (:obj:`bool`): If True, ignore all diacritics except for the Shadda diacritic. (Defualt is True)
+        ignoreShaddaDiacritic (:obj:`bool`): If True, ignore the Shadda diacritic.(Default is True)
+
+    Returns:
+        The Jaccard similarity, union, or intersection of the two sets of strings, 
+        depending on the value of the `selection` argument.
+    
+    Note:
+        - If `selection` is *jaccardAll*, a list of the intersection, union, and Jaccard similarity 
+        of the two sets of strings will be returned.
+        - If an error occurs, the method will return the string "An error has occurred".
+          Online tool: https://sina.birzeit.edu/resources/jaccardFunction.html
+    """
+    try:
+        list1 = str1.split(delimiter)
+        list2 = str2.split(delimiter)
+
+        if selection == "intersection":
+            intersection = get_intersection(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
+            return intersection
+        elif selection == "union":
+            union = get_union(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
+            return union
+        elif selection == "jaccardSimilarity":      
+            similarity = jaccard_similarity(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
+            return similarity
+        elif selection == "jaccardAll":    
+            intersection = get_intersection(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
+            union = get_union(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
+            similarity = jaccard_similarity(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
+            output_list = ["intersection:", intersection, "union:", union, "similarity:", similarity]
+            return output_list
+        else:
+            return 'Invalid selection option'
+
+    except AttributeError as ae:
+        print(f"Attribute error occurred: {str(ae)}")
+        return 'Invalid input type'
+    except Exception as e:
+        print(f"Error occurred: {str(e)}")
+        return 'An error has occurred'
```

### Comparing `nlptoolssna-0.9.2/nlptools/utils/parser.py` & `nlptoolssna-0.9.3/nlptools/utils/parser.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import re 
-
-def arStrip(text , diacs=True , smallDiacs=True , shaddah=True , digit=True, alif=True , specialChars=True ):
-    
-    """
-    This method removes Arabic diacritics, small diacritcs, shaddah, Latin and Arabic digits, and unify alif.
-    And remove special characters, spaces, underscore and Arabic tatwelah from the input text.
-
-    Args:
-        text (:obj:`str`): Arabic text to be processed.
-        diacs (:obj:`bool`): flag to remove Arabic diacretics [ ًٌٍَُِْ] (default is True).
-        smallDiacs (:obj:`bool`): flag to remove small diacretics (default is True).
-        shaddah (:obj:`bool`): flag to remove shaddah (default is True).
-        digit (:obj:`bool`): flag to remove Latin and Arabic digits (default is True).
-        alif (:obj:`bool`): flag to unify alif (default is True).
-        specialChars (:obj:`bool`): flag to remove special characters (default is True).
-
-    Returns:
-        :obj:`str`: stripped text.
-
-    **Example:**
-
-    .. highlight:: python
-    .. code-block:: python
-
-        from nlptools.utils import parser
-        processed_text =parser.arStrip('2023الجو جميلُ')
-        print(processed_text)
-
-        #putput
-        الجو جميل
-
-        name =parser.arStrip('أَلَمۡ یَأۡنِ لِلَّذِینَ ءَامَنُوۤا۟ أَن تَخۡشَعَ قُلُوبُهُمۡ لِذِكۡرِ ٱللَّهِ وَمَا نَزَلَ مِنَ ٱلۡحَقِّ وَلَا یَكُونُوا۟ كَٱلَّذِینَ أُوتُوا۟ ٱلۡكِتَـٰبَ مِن قَبۡلُ فَطَالَ عَلَیۡهِمُ ٱلۡأَمَدُ فَقَسَتۡ قُلُوبُهُمۡۖ وَكَثِیر مِّنۡهُمۡ فَـسِقُونَ' , True , True , True ,  True , True , True )
-        print(name)
-        #putput
-        الم یان للذین ءامنوا ان تخشع قلوبهم لذكر الله وما نزل من الحق ولا یكونوا كالذین اوتوا الكتٰب من قبل فطال علیهم الامد فقست قلوبهم وكثیر منهم فسقون
-
-
-    """
-    try:
-        if text: # if the input string is not empty do the following
-            #print("in if")
-            if diacs == True :
-                text = re.sub(r'[\u064B-\u0650]+', '',text) # Remove all Arabic diacretics [ ًٌٍَُِْ]
-                text = re.sub(r'[\u0652]+', '',text) # Remove SUKUN
-            if shaddah == True:
-                text = re.sub(r'[\u0651]+', '',text) # Remove shddah
-            if smallDiacs == True:
-                text = re.sub(r'[\u06D6-\u06ED]+', '',text) # Remove all small Quranic annotation signs
-            if digit == True:
-                text = re.sub('[0-9]+', ' ',text) # Remove English digits
-                text = re.sub('[٠-٩]+', ' ',text)# Remove Arabic digits
-            
-            if alif == True:                             # Unify alif with hamzah: 
-                text = re.sub('ٱ', 'ا',text);
-                text = re.sub('أ', 'ا',text);
-                text = re.sub('إ', 'ا',text);
-                text = re.sub('آ', 'ا',text);
-            if specialChars == True:
-                text = re.sub('[?؟!@#$%-]+' , '' , text) # Remove some of special chars 
-
-            text = re.sub('[\\s]+'," ",text) # Remove all spaces
-            text = text.replace("_" , '') #Remove underscore
-            text = text.replace("ـ" , '') # Remove Arabic tatwelah
-            text = text.strip() # Trim input string
-    except:
-        return text
-    return text
-    
-def remove_punctuation(text):
-    """
-    Removes punctuation marks from the text.
-    
-    Args:
-      text (:obj:`str`): The input text.
-    
-    Returns:
-      :obj:`str`: The output text without punctuation marks.
-
-    **Example:**
-
-    .. highlight:: python
-    .. code-block:: python
-    
-        from nlptools.utils import parser
-        return parser.remove_punctuation("te!@#،$%%؟st")
-
-        #output
-        test
-
-        output= parser.remove_punctuation(" {يَا أَيُّهَا الَّذِينَ آمَنُوا لِيَسْتَأْذِنْكُمُ ....}")
-        print(output)
-
-        #output
-        يَا أَيُّهَا الَّذِينَ آمَنُوا لِيَسْتَأْذِنْكُمُ  
-
-    """
-    try:
-        if text:
-            punctuation_marks = [r'[\u0021-\u002F]+', r'[U+060C]+', r'[\u003A-\u0040]+',
-                                 r'[\u005B-\u0060]+', r'[\u007B-\u007E]+', r'[\u060C]+',
-                                 r'[\u061B]+', r'[\u061E]+', r'[\u061F]+', r'[\u0640]+',
-                                 r'[\u0653]+', r'[\u065C]+', r'[\u066C]+', r'[\u066A]+',
-                                 r'["}"]+', r'["{"]+']
-            outputString = text
-            for punctuation in punctuation_marks:
-                outputString = re.sub(punctuation, '', outputString)
-    except:
-        return text
-    return outputString
-
-def remove_latin(text):
-    """
-    This method removes all Latin characters from the input text.
-
-    Args:
-        text (:obj:`str`): The input text.
-
-    Returns:
-         outputString (:obj:`str`): The text without Latin characters.
-    Note:
-        If an error occurs during processing, the original text is returned.
-    **Example:**
-
-    .. highlight:: python
-    .. code-block:: python
-
-        from nlptools.utils import parser
-        return parser.remove_latin("miojkdujhvaj1546545spkdpoqfoiehwv nWEQFGWERHERTJETAWIKUYFC")
-    
-        #output
-        1546545  
-
-        output =parser.remove_latin("أصل المسمى «تخطيط موارد المؤسسة» هو تعريب لمسمى التخطيط باللغة الإنجليزية Enterprise Resource Planning")
-        print(output)
-
-        #output
-        أصل المسمى «تخطيط موارد المؤسسة» هو تعريب لمسمى التخطيط باللغة الإنجليزية      
-    """
-    try:
-        if text:
-            text = re.sub('[a-zA-Z]+', ' ', text)
-    except:
-        return text
-    return text
-
-
+import re 
+
+def arStrip(text , diacs=True , smallDiacs=True , shaddah=True , digit=True, alif=True , specialChars=True ):
+    
+    """
+    This method removes Arabic diacritics, small diacritcs, shaddah, Latin and Arabic digits, and unify alif.
+    And remove special characters, spaces, underscore and Arabic tatwelah from the input text.
+
+    Args:
+        text (:obj:`str`): Arabic text to be processed.
+        diacs (:obj:`bool`): flag to remove Arabic diacretics [ ًٌٍَُِْ] (default is True).
+        smallDiacs (:obj:`bool`): flag to remove small diacretics (default is True).
+        shaddah (:obj:`bool`): flag to remove shaddah (default is True).
+        digit (:obj:`bool`): flag to remove Latin and Arabic digits (default is True).
+        alif (:obj:`bool`): flag to unify alif (default is True).
+        specialChars (:obj:`bool`): flag to remove special characters (default is True).
+
+    Returns:
+        :obj:`str`: stripped text.
+
+    **Example:**
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from nlptools.utils import parser
+        processed_text =parser.arStrip('2023الجو جميلُ')
+        print(processed_text)
+
+        #putput
+        الجو جميل
+
+        name =parser.arStrip('أَلَمۡ یَأۡنِ لِلَّذِینَ ءَامَنُوۤا۟ أَن تَخۡشَعَ قُلُوبُهُمۡ لِذِكۡرِ ٱللَّهِ وَمَا نَزَلَ مِنَ ٱلۡحَقِّ وَلَا یَكُونُوا۟ كَٱلَّذِینَ أُوتُوا۟ ٱلۡكِتَـٰبَ مِن قَبۡلُ فَطَالَ عَلَیۡهِمُ ٱلۡأَمَدُ فَقَسَتۡ قُلُوبُهُمۡۖ وَكَثِیر مِّنۡهُمۡ فَـسِقُونَ' , True , True , True ,  True , True , True )
+        print(name)
+        #putput
+        الم یان للذین ءامنوا ان تخشع قلوبهم لذكر الله وما نزل من الحق ولا یكونوا كالذین اوتوا الكتٰب من قبل فطال علیهم الامد فقست قلوبهم وكثیر منهم فسقون
+
+
+    """
+    try:
+        if text: # if the input string is not empty do the following
+            #print("in if")
+            if diacs == True :
+                text = re.sub(r'[\u064B-\u0650]+', '',text) # Remove all Arabic diacretics [ ًٌٍَُِْ]
+                text = re.sub(r'[\u0652]+', '',text) # Remove SUKUN
+            if shaddah == True:
+                text = re.sub(r'[\u0651]+', '',text) # Remove shddah
+            if smallDiacs == True:
+                text = re.sub(r'[\u06D6-\u06ED]+', '',text) # Remove all small Quranic annotation signs
+            if digit == True:
+                text = re.sub('[0-9]+', ' ',text) # Remove English digits
+                text = re.sub('[٠-٩]+', ' ',text)# Remove Arabic digits
+            
+            if alif == True:                             # Unify alif with hamzah: 
+                text = re.sub('ٱ', 'ا',text);
+                text = re.sub('أ', 'ا',text);
+                text = re.sub('إ', 'ا',text);
+                text = re.sub('آ', 'ا',text);
+            if specialChars == True:
+                text = re.sub('[?؟!@#$%-]+' , '' , text) # Remove some of special chars 
+
+            text = re.sub('[\\s]+'," ",text) # Remove all spaces
+            text = text.replace("_" , '') #Remove underscore
+            text = text.replace("ـ" , '') # Remove Arabic tatwelah
+            text = text.strip() # Trim input string
+    except:
+        return text
+    return text
+    
+def remove_punctuation(text):
+    """
+    Removes punctuation marks from the text.
+    
+    Args:
+      text (:obj:`str`): The input text.
+    
+    Returns:
+      :obj:`str`: The output text without punctuation marks.
+
+    **Example:**
+
+    .. highlight:: python
+    .. code-block:: python
+    
+        from nlptools.utils import parser
+        return parser.remove_punctuation("te!@#،$%%؟st")
+
+        #output
+        test
+
+        output= parser.remove_punctuation(" {يَا أَيُّهَا الَّذِينَ آمَنُوا لِيَسْتَأْذِنْكُمُ ....}")
+        print(output)
+
+        #output
+        يَا أَيُّهَا الَّذِينَ آمَنُوا لِيَسْتَأْذِنْكُمُ  
+
+    """
+    try:
+        if text:
+            punctuation_marks = [r'[\u0021-\u002F]+', r'[U+060C]+', r'[\u003A-\u0040]+',
+                                 r'[\u005B-\u0060]+', r'[\u007B-\u007E]+', r'[\u060C]+',
+                                 r'[\u061B]+', r'[\u061E]+', r'[\u061F]+', r'[\u0640]+',
+                                 r'[\u0653]+', r'[\u065C]+', r'[\u066C]+', r'[\u066A]+',
+                                 r'["}"]+', r'["{"]+']
+            outputString = text
+            for punctuation in punctuation_marks:
+                outputString = re.sub(punctuation, '', outputString)
+    except:
+        return text
+    return outputString
+
+def remove_latin(text):
+    """
+    This method removes all Latin characters from the input text.
+
+    Args:
+        text (:obj:`str`): The input text.
+
+    Returns:
+         outputString (:obj:`str`): The text without Latin characters.
+    Note:
+        If an error occurs during processing, the original text is returned.
+    **Example:**
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from nlptools.utils import parser
+        return parser.remove_latin("miojkdujhvaj1546545spkdpoqfoiehwv nWEQFGWERHERTJETAWIKUYFC")
+    
+        #output
+        1546545  
+
+        output =parser.remove_latin("أصل المسمى «تخطيط موارد المؤسسة» هو تعريب لمسمى التخطيط باللغة الإنجليزية Enterprise Resource Planning")
+        print(output)
+
+        #output
+        أصل المسمى «تخطيط موارد المؤسسة» هو تعريب لمسمى التخطيط باللغة الإنجليزية      
+    """
+    try:
+        if text:
+            text = re.sub('[a-zA-Z]+', ' ', text)
+    except:
+        return text
+    return text
+
+
```

### Comparing `nlptoolssna-0.9.2/nlptools/utils/text_transliteration.py` & `nlptoolssna-0.9.3/nlptools/utils/text_transliteration.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-# Created: 07/03/2021 , By Mohammad A'bed , Tested on SAMA lemma DB  
-# Trello task: https://trello.com/c/wsiMd4iW/20-buckwalter-to-arabic-and-vice-versa
-from collections import deque
-
-# This is a mapping dictionery of Arabic letters to BW 
-# dictionery contains: key -> Unicode to Arabic, value -> BW chars
-# It includes all BW mappings in addition to other special characters
-#  that are used in the SAMA database but not part of the BW character set such as numbers and Qur'anic diacritics
-ar2bw_map = {
-    '\u0621' : '\'' , # ء
-    '\u0622' : '|' , # آ
-    '\u0623' : '>' , # أ
-    '\u0624' : '&' , # ؤ
-    '\u0625' : '<' , # إ
-    '\u0626' : '}' , # ئ
-    '\u0627' : 'A' , # ا
-    '\u0628' : 'b' , # ب
-    '\u0629' : 'p' , # ة
-    '\u062A' : 't' , # ت
-    '\u062B' : 'v' , # ث
-    '\u062C' : 'j' , # ج
-    '\u062D' : 'H' , # ح
-    '\u062E' : 'x' , # خ
-    '\u062F' : 'd' , # د
-    '\u0630' : '*' , # ذ
-    '\u0631' : 'r' , # ر
-    '\u0632' : 'z' , # ز
-    '\u0633' : 's' , # س
-    '\u0634' : '$' , # ش
-    '\u0635' : 'S' , # ص
-    '\u0636' : 'D' , # ض
-    '\u0637' : 'T' , # ط
-    '\u0638' : 'Z' , # ظ
-    '\u0639' : 'E' , # ع
-    '\u063A' : 'g' , # غ
-    '\u0020' : ' ' , #Space is replaced by space 
-    '\u0640' : '_' , #ـ
-    '\u0641' : 'f' , # ف
-    '\u0642' : 'q' , # ق
-    '\u0643' : 'k' , # ك
-    '\u0644' : 'l' , # ل
-    '\u0645' : 'm' , # م
-    '\u0646' : 'n' , # ن
-    '\u0647' : 'h' , # ه
-    '\u0648' : 'w' , # و
-    '\u0649' : 'Y' , # ى
-    '\u064A' : 'y' , # ي
-    '\u064B' : 'F' , # TANWEEN FATH ً
-    '\u064C' : 'N' , #TANWEEN DHAM ٌ
-    '\u064D' : 'K' , #TANWEE KASR ٍ
-    '\u064E' : 'a' , #FATHA َ
-    '\u064F' : 'u' , #DHAMMA ُ
-    '\u0650' : 'i' , #KASRA ِ
-    '\u0651' : '~' , # SHADDAH ّ
-    '\u0652' : 'o' , #SUKON ْ
-    '\u0670' : '`' , # SHORT ALEF (dagger alif) ٰ
-    '\u0671' : '{' , #AL WITH HAMZA QATE'/WASEL MARK ٱ
-    '\u067E' : 'P' , # پ 
-    '\u0686' : 'J' , # چ 
-    '\u06A4' : 'V' , # ڤ 
-    '\u06AF' : 'G' , # گ 
-    '\u06EA' : '-' , # ۪ Not BW standerd
-    '\u0654' : '#' , # ٔ     Not BW standerd
-    '\u06DC ' : ':' , # short sen ۜ  Not BW standerd  
-    '\u06E0' : '"' , # small circle ۟  ,Not BW standerd
-    '\u06E2' : '[' , # short meem ۢ  , Not BW standerd
-    '\u06E3 ' : ';' , #small sen below letter  ۣ  , Not BW standerd
-    '\u06E5 ' : ',' , # samall wa ۥ  , Not BW standerd
-    '\u06E6' : '.' , # ۦ   Not BW standerd
-    '\u06E8 ' : '!' , # small noon ۨ  Not BW standerd
-    '\u06EA' : '-' , # special qura'nic arabic ( littel circule underneath), is not part of standerd BW , not in Buckwalter ۪  Not BW standerd
-    '\u06EC' : '%' , # small solid circle ۬  Not BW standerd
-    '\u06ED ' : ']',  # small meem ۭ  Not BW standerd
-    '0' : '0' , #
-    '1' : '1' , #
-    '2' : '2' , #
-    '3' : '3' , #
-    '4' : '4' , #
-    '5' : '5' , #
-    '6' : '6' , #
-    '7' : '7' , #
-    '8' : '8' , #
-    '9' : '9'  #
-}
-
-# This is a mapping dictionery of BW  letters to  Arabic
-# It includes all Arabic mappings in addition to other special characters
-#  that are used in the SAMA database but not part of the Arabic character set such as numbers and Qur'anic diacritics
-bw2ar_map = {
-    '\'' : '\u0621' , # ء
-    '|' : '\u0622' , # آ
-    '>' : '\u0623' , # أ
-    '&' : '\u0624' , # ؤ
-    '<' : '\u0625' , # إ
-    '}' : '\u0626' , # ئ
-    'A' : '\u0627' , # ا
-    'b' : '\u0628' , # ب
-    'p' : '\u0629' , # ة
-    't' : '\u062A' , # ت
-    'v' : '\u062B' , # ث
-    'j' : '\u062C' , # ج
-    'H' : '\u062D' , # ح
-    'x' : '\u062E' , # خ
-    'd' : '\u062F' , # د
-    '*' : '\u0630' , # ذ
-    'r' : '\u0631' , # ر
-    'z' : '\u0632' , # ز
-    's' : '\u0633' , # س
-    '$' : '\u0634' , # ش
-    'S' : '\u0635' , # ص
-    'D' : '\u0636' , # ض
-    'T' : '\u0637' , # ط
-    'Z' : '\u0638' , # ظ
-    'E' : '\u0639' , # ع
-    'g' : '\u063A' , # غ
-    ' ' : '\u0020' , #Space is replaced by space 
-    '_' : ' ' , #ـ    This is Temporary
-    # '_' : '\u0640' , #ـ
-    'f' : '\u0641' , # ف
-    'q' : '\u0642' , # ق
-    'k' : '\u0643' , # ك
-    'l' : '\u0644' , # ل
-    'm' : '\u0645' , # م
-    'n' : '\u0646' , # ن
-    'h' : '\u0647' , # ه
-    'w' : '\u0648' , # و
-    'Y' : '\u0649' , # ى
-    'y' : '\u064A' , # ي
-    'F' : '\u064B' , # TANWEEN FATH  ً
-    'N' : '\u064C' , #TANWEEN DHAM  ٌ
-    'K' : '\u064D' , #TANWEE KASR  ٍ
-    'a' : '\u064E' , #FATHA  َ
-    'u' : '\u064F' , #DHAMMA  ُ
-    'i' : '\u0650' , #KASRA  ِ
-    '~' : '\u0651' , # SHADDAH  ّ
-    'o' : '\u0652' , #SUKON  ْ
-    '`' : '\u0670' , # SHORT ALEF (dagger alif) ٰ
-    '{' : '\u0671' , #AL WITH HAMZA QATE'/WASEL MARK ٱ
-    'P' : '\u067E' , # پ 
-    'J' : '\u0686' , # چ 
-    'V' : '\u06A4' , # ڤ 
-    'G' : '\u06AF' , # گ 
-    '-' : '\u06EA' , # ۪ Not BW standerd
-    '#' : '\u0654' , # ٔ  ARABIC HAMZA ABOVE   Not BW standerd
-    ':' : '\u06DC ' , # short sen ۜ  Not BW standerd  
-    '"' : '\u06E0' , # small circle ۟  ,Not BW standerd
-    '[' : '\u06E2' , # short meem ۢ  , Not BW standerd
-    ';' : '\u06E3 ' , #small sen below letter  ۣ  , Not BW standerd
-    ',' : '\u06E5 ' , # samall wa ۥ  , Not BW standerd
-    '.' : '\u06E6' , # ۦ   Not BW standerd
-    '!' : '\u06E8 ' , # small noon ۨ  Not BW standerd
-    '-' : '\u06EA' , # special qura'nic arabic ( littel circule underneath), is not part of standerd BW , not in Buckwalter ۪  Not BW standerd
-    '%' : '\u06EC' , # small solid circle ۬  Not BW standerd
-    ']' : '\u06ED ',  # small meem ۭ  Not BW standerd
-    '0' : '0' , #
-    '1' : '1' , #
-    '2' : '2' , #
-    '3' : '3' , #
-    '4' : '4' , #
-    '5' : '5' , #
-    '6' : '6' , #
-    '7' : '7' , #
-    '8' : '8' , #
-    '9' : '9'  #
-}
-# A transliterate Function to transliterate Arabic letters and vice versa
-#It takes a text and the schema as input and return 2-values: the transliteration and a flag of whether all chars are transliterated or not
-def perform_transliteration(text , schema ):
-    """
-    This method takes a text and a schema as input and returns a tuple of two values: the transliteration of the text based on the given schema and a flag indicating whether all characters in the text were transliterated or not.
-
-    Args:
-        text (:obj:`str`): The input text to be transliterated.
-        schema (:obj:`str`): The transliteration schema to be used. Should be either `bw2ar` to transliterate Buckwalter-encoded Arabic text to Arabic script, or `ar2bw` to transliterate Arabic script to Buckwalter-encoded Arabic text.
-
-    Returns:
-        :obj:`tuple`: A tuple of two values:
-        - The transliterated text based on the given schema.
-        - A boolean flag indicating whether all characters in the input text were successfully transliterated or not.
-
-    **Example:**
-
-    .. highlight:: python
-    .. code-block:: python
-
-        from nlptools.utils import text_transliteration
-
-        print(text_transliteration.perform_transliteration("مُحَمَدٌ نَـشِيْطٌـ1"  , "ar2bw"))
-        print(text_transliteration.perform_transliteration("muHamadN"  , "bw2ar"))
-        print(text_transliteration.perform_transliteration("شَنُعُ۪ـ1"  , "ar2bw"))
-        print(text_transliteration.perform_transliteration("$aw~aH_2"  , "bw2ar"))
-
-        #output
-        ('muHamadN na_$iyoTN_1', True)
-        ('مُحَمَدٌ', True)
-        ('$anuE-u_1', True)
-        ('شَوَّح 2', True)
-    """
-    # to map BW into Arabic  
-    if schema == "bw2ar":
-        transliterated_text = deque() #Empty deque list
-        
-        is_all_mapped = True
-        for char in text:
-            # lockup every charecters in the dictionary, if not found return the original char 
-            char_value = bw2ar_map.get(char)
-   
-            if char_value is None:
-                is_all_mapped = False  # False if one cjars is not in map
-                transliterated_text.append(char)
-            else:
-                transliterated_text.append(char_value)
-
-        return ''.join(transliterated_text)  , is_all_mapped
-    # to map Arabic into BW
-    elif schema == "ar2bw":
-
-        transliterated_text = deque()
-   
-        is_all_mapped = True
-        for char in text:
-            # lockup evry charecters in the dictionary, if not found return the original char 
-            char_value = ar2bw_map.get(char)
-          
-            if char_value is None:
-                is_all_mapped = False   # False if one cjars is not in map
-                transliterated_text.append(char)
-            else:
-                transliterated_text.append(char_value)
-
-    return ''.join(transliterated_text)  , is_all_mapped
-
-
-
+# Created: 07/03/2021 , By Mohammad A'bed , Tested on SAMA lemma DB  
+# Trello task: https://trello.com/c/wsiMd4iW/20-buckwalter-to-arabic-and-vice-versa
+from collections import deque
+
+# This is a mapping dictionery of Arabic letters to BW 
+# dictionery contains: key -> Unicode to Arabic, value -> BW chars
+# It includes all BW mappings in addition to other special characters
+#  that are used in the SAMA database but not part of the BW character set such as numbers and Qur'anic diacritics
+ar2bw_map = {
+    '\u0621' : '\'' , # ء
+    '\u0622' : '|' , # آ
+    '\u0623' : '>' , # أ
+    '\u0624' : '&' , # ؤ
+    '\u0625' : '<' , # إ
+    '\u0626' : '}' , # ئ
+    '\u0627' : 'A' , # ا
+    '\u0628' : 'b' , # ب
+    '\u0629' : 'p' , # ة
+    '\u062A' : 't' , # ت
+    '\u062B' : 'v' , # ث
+    '\u062C' : 'j' , # ج
+    '\u062D' : 'H' , # ح
+    '\u062E' : 'x' , # خ
+    '\u062F' : 'd' , # د
+    '\u0630' : '*' , # ذ
+    '\u0631' : 'r' , # ر
+    '\u0632' : 'z' , # ز
+    '\u0633' : 's' , # س
+    '\u0634' : '$' , # ش
+    '\u0635' : 'S' , # ص
+    '\u0636' : 'D' , # ض
+    '\u0637' : 'T' , # ط
+    '\u0638' : 'Z' , # ظ
+    '\u0639' : 'E' , # ع
+    '\u063A' : 'g' , # غ
+    '\u0020' : ' ' , #Space is replaced by space 
+    '\u0640' : '_' , #ـ
+    '\u0641' : 'f' , # ف
+    '\u0642' : 'q' , # ق
+    '\u0643' : 'k' , # ك
+    '\u0644' : 'l' , # ل
+    '\u0645' : 'm' , # م
+    '\u0646' : 'n' , # ن
+    '\u0647' : 'h' , # ه
+    '\u0648' : 'w' , # و
+    '\u0649' : 'Y' , # ى
+    '\u064A' : 'y' , # ي
+    '\u064B' : 'F' , # TANWEEN FATH ً
+    '\u064C' : 'N' , #TANWEEN DHAM ٌ
+    '\u064D' : 'K' , #TANWEE KASR ٍ
+    '\u064E' : 'a' , #FATHA َ
+    '\u064F' : 'u' , #DHAMMA ُ
+    '\u0650' : 'i' , #KASRA ِ
+    '\u0651' : '~' , # SHADDAH ّ
+    '\u0652' : 'o' , #SUKON ْ
+    '\u0670' : '`' , # SHORT ALEF (dagger alif) ٰ
+    '\u0671' : '{' , #AL WITH HAMZA QATE'/WASEL MARK ٱ
+    '\u067E' : 'P' , # پ 
+    '\u0686' : 'J' , # چ 
+    '\u06A4' : 'V' , # ڤ 
+    '\u06AF' : 'G' , # گ 
+    '\u06EA' : '-' , # ۪ Not BW standerd
+    '\u0654' : '#' , # ٔ     Not BW standerd
+    '\u06DC ' : ':' , # short sen ۜ  Not BW standerd  
+    '\u06E0' : '"' , # small circle ۟  ,Not BW standerd
+    '\u06E2' : '[' , # short meem ۢ  , Not BW standerd
+    '\u06E3 ' : ';' , #small sen below letter  ۣ  , Not BW standerd
+    '\u06E5 ' : ',' , # samall wa ۥ  , Not BW standerd
+    '\u06E6' : '.' , # ۦ   Not BW standerd
+    '\u06E8 ' : '!' , # small noon ۨ  Not BW standerd
+    '\u06EA' : '-' , # special qura'nic arabic ( littel circule underneath), is not part of standerd BW , not in Buckwalter ۪  Not BW standerd
+    '\u06EC' : '%' , # small solid circle ۬  Not BW standerd
+    '\u06ED ' : ']',  # small meem ۭ  Not BW standerd
+    '0' : '0' , #
+    '1' : '1' , #
+    '2' : '2' , #
+    '3' : '3' , #
+    '4' : '4' , #
+    '5' : '5' , #
+    '6' : '6' , #
+    '7' : '7' , #
+    '8' : '8' , #
+    '9' : '9'  #
+}
+
+# This is a mapping dictionery of BW  letters to  Arabic
+# It includes all Arabic mappings in addition to other special characters
+#  that are used in the SAMA database but not part of the Arabic character set such as numbers and Qur'anic diacritics
+bw2ar_map = {
+    '\'' : '\u0621' , # ء
+    '|' : '\u0622' , # آ
+    '>' : '\u0623' , # أ
+    '&' : '\u0624' , # ؤ
+    '<' : '\u0625' , # إ
+    '}' : '\u0626' , # ئ
+    'A' : '\u0627' , # ا
+    'b' : '\u0628' , # ب
+    'p' : '\u0629' , # ة
+    't' : '\u062A' , # ت
+    'v' : '\u062B' , # ث
+    'j' : '\u062C' , # ج
+    'H' : '\u062D' , # ح
+    'x' : '\u062E' , # خ
+    'd' : '\u062F' , # د
+    '*' : '\u0630' , # ذ
+    'r' : '\u0631' , # ر
+    'z' : '\u0632' , # ز
+    's' : '\u0633' , # س
+    '$' : '\u0634' , # ش
+    'S' : '\u0635' , # ص
+    'D' : '\u0636' , # ض
+    'T' : '\u0637' , # ط
+    'Z' : '\u0638' , # ظ
+    'E' : '\u0639' , # ع
+    'g' : '\u063A' , # غ
+    ' ' : '\u0020' , #Space is replaced by space 
+    '_' : ' ' , #ـ    This is Temporary
+    # '_' : '\u0640' , #ـ
+    'f' : '\u0641' , # ف
+    'q' : '\u0642' , # ق
+    'k' : '\u0643' , # ك
+    'l' : '\u0644' , # ل
+    'm' : '\u0645' , # م
+    'n' : '\u0646' , # ن
+    'h' : '\u0647' , # ه
+    'w' : '\u0648' , # و
+    'Y' : '\u0649' , # ى
+    'y' : '\u064A' , # ي
+    'F' : '\u064B' , # TANWEEN FATH  ً
+    'N' : '\u064C' , #TANWEEN DHAM  ٌ
+    'K' : '\u064D' , #TANWEE KASR  ٍ
+    'a' : '\u064E' , #FATHA  َ
+    'u' : '\u064F' , #DHAMMA  ُ
+    'i' : '\u0650' , #KASRA  ِ
+    '~' : '\u0651' , # SHADDAH  ّ
+    'o' : '\u0652' , #SUKON  ْ
+    '`' : '\u0670' , # SHORT ALEF (dagger alif) ٰ
+    '{' : '\u0671' , #AL WITH HAMZA QATE'/WASEL MARK ٱ
+    'P' : '\u067E' , # پ 
+    'J' : '\u0686' , # چ 
+    'V' : '\u06A4' , # ڤ 
+    'G' : '\u06AF' , # گ 
+    '-' : '\u06EA' , # ۪ Not BW standerd
+    '#' : '\u0654' , # ٔ  ARABIC HAMZA ABOVE   Not BW standerd
+    ':' : '\u06DC ' , # short sen ۜ  Not BW standerd  
+    '"' : '\u06E0' , # small circle ۟  ,Not BW standerd
+    '[' : '\u06E2' , # short meem ۢ  , Not BW standerd
+    ';' : '\u06E3 ' , #small sen below letter  ۣ  , Not BW standerd
+    ',' : '\u06E5 ' , # samall wa ۥ  , Not BW standerd
+    '.' : '\u06E6' , # ۦ   Not BW standerd
+    '!' : '\u06E8 ' , # small noon ۨ  Not BW standerd
+    '-' : '\u06EA' , # special qura'nic arabic ( littel circule underneath), is not part of standerd BW , not in Buckwalter ۪  Not BW standerd
+    '%' : '\u06EC' , # small solid circle ۬  Not BW standerd
+    ']' : '\u06ED ',  # small meem ۭ  Not BW standerd
+    '0' : '0' , #
+    '1' : '1' , #
+    '2' : '2' , #
+    '3' : '3' , #
+    '4' : '4' , #
+    '5' : '5' , #
+    '6' : '6' , #
+    '7' : '7' , #
+    '8' : '8' , #
+    '9' : '9'  #
+}
+# A transliterate Function to transliterate Arabic letters and vice versa
+#It takes a text and the schema as input and return 2-values: the transliteration and a flag of whether all chars are transliterated or not
+def perform_transliteration(text , schema ):
+    """
+    This method takes a text and a schema as input and returns a tuple of two values: the transliteration of the text based on the given schema and a flag indicating whether all characters in the text were transliterated or not.
+
+    Args:
+        text (:obj:`str`): The input text to be transliterated.
+        schema (:obj:`str`): The transliteration schema to be used. Should be either `bw2ar` to transliterate Buckwalter-encoded Arabic text to Arabic script, or `ar2bw` to transliterate Arabic script to Buckwalter-encoded Arabic text.
+
+    Returns:
+        :obj:`tuple`: A tuple of two values:
+        - The transliterated text based on the given schema.
+        - A boolean flag indicating whether all characters in the input text were successfully transliterated or not.
+
+    **Example:**
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from nlptools.utils import text_transliteration
+
+        print(text_transliteration.perform_transliteration("مُحَمَدٌ نَـشِيْطٌـ1"  , "ar2bw"))
+        print(text_transliteration.perform_transliteration("muHamadN"  , "bw2ar"))
+        print(text_transliteration.perform_transliteration("شَنُعُ۪ـ1"  , "ar2bw"))
+        print(text_transliteration.perform_transliteration("$aw~aH_2"  , "bw2ar"))
+
+        #output
+        ('muHamadN na_$iyoTN_1', True)
+        ('مُحَمَدٌ', True)
+        ('$anuE-u_1', True)
+        ('شَوَّح 2', True)
+    """
+    # to map BW into Arabic  
+    if schema == "bw2ar":
+        transliterated_text = deque() #Empty deque list
+        
+        is_all_mapped = True
+        for char in text:
+            # lockup every charecters in the dictionary, if not found return the original char 
+            char_value = bw2ar_map.get(char)
+   
+            if char_value is None:
+                is_all_mapped = False  # False if one cjars is not in map
+                transliterated_text.append(char)
+            else:
+                transliterated_text.append(char_value)
+
+        return ''.join(transliterated_text)  , is_all_mapped
+    # to map Arabic into BW
+    elif schema == "ar2bw":
+
+        transliterated_text = deque()
+   
+        is_all_mapped = True
+        for char in text:
+            # lockup evry charecters in the dictionary, if not found return the original char 
+            char_value = ar2bw_map.get(char)
+          
+            if char_value is None:
+                is_all_mapped = False   # False if one cjars is not in map
+                transliterated_text.append(char)
+            else:
+                transliterated_text.append(char_value)
+
+    return ''.join(transliterated_text)  , is_all_mapped
+
+
+
```

### Comparing `nlptoolssna-0.9.2/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.9.3/nlptoolssna.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: nlptoolssna
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
+Description: ========
+        nlptools
+        ========
+        
+        
+        .. image:: https://img.shields.io/pypi/v/nlptools.svg
+                :target: https://pypi.python.org/pypi/nlptools
+        
+        .. image:: https://img.shields.io/travis/eng-aomar/nlptools.svg
+                :target: https://travis-ci.com/eng-aomar/nlptools
+        
+        .. image:: https://readthedocs.org/projects/nlptools/badge/?version=latest
+                :target: https://nlptools.readthedocs.io/en/latest/?version=latest
+                :alt: Documentation Status
+        
+        
+        
+        
+        Python Boilerplate contains all the boilerplate you need to create a Python package.
+        
+        
+        * Free software: MIT license
+        * Documentation: https://nlptools.readthedocs.io.
+        
+        
+        Features
+        --------
+        
+        * TODO
+        
+        Credits
+        -------
+        
+        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+        
+        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
+        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+        
+        
+        =======
+        History
+        =======
+        
+        0.1.0 (2023-04-15)
+        ------------------
+        
+        * First release on PyPI.
+        
 Keywords: nlptools
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-========
-nlptools
-========
-
-
-.. image:: https://img.shields.io/pypi/v/nlptools.svg
-        :target: https://pypi.python.org/pypi/nlptools
-
-.. image:: https://img.shields.io/travis/eng-aomar/nlptools.svg
-        :target: https://travis-ci.com/eng-aomar/nlptools
-
-.. image:: https://readthedocs.org/projects/nlptools/badge/?version=latest
-        :target: https://nlptools.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-
-
-Python Boilerplate contains all the boilerplate you need to create a Python package.
-
-
-* Free software: MIT license
-* Documentation: https://nlptools.readthedocs.io.
-
-
-Features
---------
-
-* TODO
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-
-=======
-History
-=======
-
-0.1.0 (2023-04-15)
-------------------
-
-* First release on PyPI.
```

### Comparing `nlptoolssna-0.9.2/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.9.3/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 docs/source/api/morphology.rst
 docs/source/api/utils.rst
 docs/source/api/DataDownload/downloader.rst
 docs/source/api/morphology/morph_analyzer.rst
 docs/source/api/utils/implication.rst
 docs/source/api/utils/jaccard.rst
 docs/source/api/utils/parser.rst
+docs/source/api/utils/sentence_tokenizer.rst
 docs/source/api/utils/text_transliteration.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
 nlptools/DataDownload/__init__.py
 nlptools/DataDownload/downloader.py
 nlptools/arabiner/__init__.py
@@ -47,30 +48,28 @@
 nlptools/arabiner/nn/BertNestedTagger.py
 nlptools/arabiner/nn/BertSeqTagger.py
 nlptools/arabiner/nn/__init__.py
 nlptools/arabiner/utils/__init__.py
 nlptools/arabiner/utils/data.py
 nlptools/arabiner/utils/helpers.py
 nlptools/arabiner/utils/metrics.py
-nlptools/data/my_data.pickle
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
 nlptools/salma/__init__.py
 nlptools/salma/views.py
 nlptools/salma/wsd.py
 nlptools/utils/__init__.py
-nlptools/utils/corpus.py
 nlptools/utils/implication.py
 nlptools/utils/jaccard.py
 nlptools/utils/parser.py
+nlptools/utils/sentence_tokenizer.py
 nlptools/utils/text_transliteration.py
-nlptools/utils/tokenizer.py
 nlptools/utils/utils.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
 nlptoolssna.egg-info/dependency_links.txt
 nlptoolssna.egg-info/entry_points.txt
 nlptoolssna.egg-info/not-zip-safe
 nlptoolssna.egg-info/requires.txt
```

### Comparing `nlptoolssna-0.9.2/setup.cfg` & `nlptoolssna-0.9.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [bumpversion]
-VERSION_FILE = os.path.join(os.path.dirname(__file__),
+version_file = os.path.join(os.path.dirname(__file__),
 	'nlptools',
 	'VERSION')
-with open(VERSION_FILE, encoding = 'utf-8') as version_fp:
+with open(version_file, encoding = 'utf-8') as version_fp:
 	VERSION = version_fp.read().strip()
 current_version = VERSION
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
```

### Comparing `nlptoolssna-0.9.2/setup.py` & `nlptoolssna-0.9.3/setup.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-import os 
-from setuptools import setup, find_packages
-VERSION_FILE = os.path.join(os.path.dirname(__file__),
-                            'nlptools',
-                            'VERSION')
-with open(VERSION_FILE, encoding='utf-8') as version_fp:
-    VERSION = version_fp.read().strip()
-with open('README.rst') as readme_file:
-    readme = readme_file.read()
-
-with open('HISTORY.rst') as history_file:
-    history = history_file.read()
-
-requirements = [
-    'six',
-    'farasapy',
-    'tqdm',
-    'requests',
-    'regex',
-    'pathlib',
-    'torch==1.13.0',
-    'transformers==4.24.0',
-    'torchtext==0.14.0',
-    'torchvision==0.14.0',
-    'seqeval==1.2.2',
-    'natsort==7.1.1'
-]
-
-test_requirements = [ ]
-
-setup(
-    author="Alaa' Omar",
-    author_email='alaa.omer2009@gmail.com',
-    python_requires='>=3.6',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
-    entry_points={
-        'console_scripts': [
-            'nlptools=nlptools.cli:main',
-        ],
-    },
-    package_data={'nlptools': ['data/*.pickle']},
-    install_requires=requirements,
-    license="MIT license",
-    long_description=readme + '\n\n' + history,
-    include_package_data=True,
-    keywords='nlptools',
-    name='nlptoolssna',
-    packages=find_packages(include=['nlptools', 'nlptools.*']),
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/eng-aomar/nlptools',
-    version=VERSION,
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+import os 
+from setuptools import setup, find_packages
+VERSION_FILE = os.path.join(os.path.dirname(__file__),
+                            'nlptools',
+                            'VERSION')
+with open(VERSION_FILE, encoding='utf-8') as version_fp:
+    VERSION = version_fp.read().strip()
+with open('README.rst') as readme_file:
+    readme = readme_file.read()
+
+with open('HISTORY.rst') as history_file:
+    history = history_file.read()
+
+requirements = [
+    'six',
+    'farasapy',
+    'tqdm',
+    'requests',
+    'regex',
+    'pathlib',
+    'torch==1.13.0',
+    'transformers==4.24.0',
+    'torchtext==0.14.0',
+    'torchvision==0.14.0',
+    'seqeval==1.2.2',
+    'natsort==7.1.1'
+]
+
+test_requirements = [ ]
+
+setup(
+    author="Alaa' Omar",
+    author_email='alaa.omer2009@gmail.com',
+    python_requires='>=3.6',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
+    entry_points={
+        'console_scripts': [
+            'nlptools=nlptools.cli:main',
+        ],
+    },
+    package_data={'nlptools': ['data/*.pickle']},
+    install_requires=requirements,
+    license="MIT license",
+    long_description=readme + '\n\n' + history,
+    include_package_data=True,
+    keywords='nlptools',
+    name='nlptoolssna',
+    packages=find_packages(include=['nlptools', 'nlptools.*']),
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/eng-aomar/nlptools',
+    version=VERSION,
+    zip_safe=False,
+)
```

