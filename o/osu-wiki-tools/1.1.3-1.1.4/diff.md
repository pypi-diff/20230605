# Comparing `tmp/osu-wiki-tools-1.1.3.tar.gz` & `tmp/osu-wiki-tools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu-wiki-tools-1.1.3.tar", last modified: Wed Feb  8 18:05:36 2023, max compression
+gzip compressed data, was "osu-wiki-tools-1.1.4.tar", last modified: Mon Jun  5 18:45:59 2023, max compression
```

## Comparing `osu-wiki-tools-1.1.3.tar` & `osu-wiki-tools-1.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 18:05:36.583564 osu-wiki-tools-1.1.3/
--rw-rw-rw-   0        0        0     1083 2022-06-05 22:05:02.000000 osu-wiki-tools-1.1.3/LICENCE.md
--rw-rw-rw-   0        0        0      962 2023-02-08 18:05:36.583564 osu-wiki-tools-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-01-29 20:05:06.000000 osu-wiki-tools-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-08 18:05:36.535555 osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/
--rw-rw-rw-   0        0        0      962 2023-02-08 18:05:36.000000 osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2023-02-08 18:05:36.000000 osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 18:05:36.000000 osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-02-08 18:05:36.000000 osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-02-08 18:05:36.000000 osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-02-08 18:05:36.000000 osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-08 18:05:36.583564 osu-wiki-tools-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1186 2023-02-04 09:12:16.000000 osu-wiki-tools-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-08 18:05:36.559568 osu-wiki-tools-1.1.3/tests/
--rw-rw-rw-   0        0        0    12105 2023-02-04 12:22:04.000000 osu-wiki-tools-1.1.3/tests/test_article_parser.py
--rw-rw-rw-   0        0        0     3883 2023-02-08 17:38:06.000000 osu-wiki-tools-1.1.3/tests/test_check_links.py
--rw-rw-rw-   0        0        0    21144 2022-07-31 07:21:51.000000 osu-wiki-tools-1.1.3/tests/test_check_outdated_articles.py
--rw-rw-rw-   0        0        0     2354 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.3/tests/test_code_block_parser.py
--rw-rw-rw-   0        0        0     1492 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.3/tests/test_comment_parser.py
--rw-rw-rw-   0        0        0     4275 2022-07-31 07:27:16.000000 osu-wiki-tools-1.1.3/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     4370 2022-05-06 12:01:04.000000 osu-wiki-tools-1.1.3/tests/test_identifier_parser.py
--rw-rw-rw-   0        0        0    28589 2023-02-04 18:17:30.000000 osu-wiki-tools-1.1.3/tests/test_link_checker.py
--rw-rw-rw-   0        0        0     9219 2022-07-31 07:21:51.000000 osu-wiki-tools-1.1.3/tests/test_link_parser.py
--rw-rw-rw-   0        0        0      849 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.3/tests/test_redirect_parser.py
--rw-rw-rw-   0        0        0     2747 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.3/tests/test_reference_parser.py
--rw-rw-rw-   0        0        0     4223 2023-01-29 20:05:06.000000 osu-wiki-tools-1.1.3/tests/test_yaml_rules.py
-drwxrwxrwx   0        0        0        0 2023-02-08 18:05:36.575564 osu-wiki-tools-1.1.3/wikitools/
--rw-rw-rw-   0        0        0        0 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.3/wikitools/__init__.py
--rw-rw-rw-   0        0        0     6547 2023-02-04 13:14:56.000000 osu-wiki-tools-1.1.3/wikitools/article_parser.py
--rw-rw-rw-   0        0        0     3449 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.3/wikitools/code_block_parser.py
--rw-rw-rw-   0        0        0     3029 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.3/wikitools/comment_parser.py
--rw-rw-rw-   0        0        0      258 2022-05-06 12:30:44.000000 osu-wiki-tools-1.1.3/wikitools/console.py
--rw-rw-rw-   0        0        0     3770 2023-02-04 18:28:19.000000 osu-wiki-tools-1.1.3/wikitools/errors.py
--rw-rw-rw-   0        0        0     2942 2023-02-08 17:52:39.000000 osu-wiki-tools-1.1.3/wikitools/file_utils.py
--rw-rw-rw-   0        0        0     1314 2022-07-31 07:21:51.000000 osu-wiki-tools-1.1.3/wikitools/git_utils.py
--rw-rw-rw-   0        0        0     2993 2022-05-06 12:01:04.000000 osu-wiki-tools-1.1.3/wikitools/identifier_parser.py
--rw-rw-rw-   0        0        0     5921 2023-02-04 18:26:10.000000 osu-wiki-tools-1.1.3/wikitools/link_checker.py
--rw-rw-rw-   0        0        0     7820 2022-07-31 07:21:47.000000 osu-wiki-tools-1.1.3/wikitools/link_parser.py
--rw-rw-rw-   0        0        0      553 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.3/wikitools/redirect_parser.py
--rw-rw-rw-   0        0        0     2536 2022-04-14 08:51:50.000000 osu-wiki-tools-1.1.3/wikitools/reference_parser.py
--rw-rw-rw-   0        0        0     5405 2023-01-29 20:05:06.000000 osu-wiki-tools-1.1.3/wikitools/yaml_rules.py
-drwxrwxrwx   0        0        0        0 2023-02-08 18:05:36.575564 osu-wiki-tools-1.1.3/wikitools_cli/
--rw-rw-rw-   0        0        0       19 2023-02-08 17:55:24.000000 osu-wiki-tools-1.1.3/wikitools_cli/VERSION.py
--rw-rw-rw-   0        0        0        0 2022-06-05 22:05:02.000000 osu-wiki-tools-1.1.3/wikitools_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 18:05:36.583564 osu-wiki-tools-1.1.3/wikitools_cli/commands/
--rw-rw-rw-   0        0        0        0 2022-07-31 07:21:51.000000 osu-wiki-tools-1.1.3/wikitools_cli/commands/__init__.py
--rw-rw-rw-   0        0        0     6158 2023-02-04 17:57:19.000000 osu-wiki-tools-1.1.3/wikitools_cli/commands/check_links.py
--rw-rw-rw-   0        0        0    10199 2023-02-05 18:22:34.000000 osu-wiki-tools-1.1.3/wikitools_cli/commands/check_outdated_articles.py
--rw-rw-rw-   0        0        0     3766 2023-01-29 20:05:06.000000 osu-wiki-tools-1.1.3/wikitools_cli/commands/check_yaml.py
--rw-rw-rw-   0        0        0     2270 2023-02-04 07:20:06.000000 osu-wiki-tools-1.1.3/wikitools_cli/osu_wiki_tools.py
--rw-rw-rw-   0        0        0     1728 2022-06-20 03:50:12.000000 osu-wiki-tools-1.1.3/wikitools_cli/update_tournament_countries.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:45:59.072838 osu-wiki-tools-1.1.4/
+-rw-rw-rw-   0        0        0     1083 2022-06-05 22:05:02.000000 osu-wiki-tools-1.1.4/LICENCE.md
+-rw-rw-rw-   0        0        0      962 2023-06-05 18:45:59.071831 osu-wiki-tools-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 18:45:58.772237 osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/
+-rw-rw-rw-   0        0        0      962 2023-06-05 18:45:58.000000 osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2023-06-05 18:45:58.000000 osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 18:45:58.000000 osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-05 18:45:58.000000 osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-06-05 18:45:58.000000 osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-05 18:45:58.000000 osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 18:45:59.072838 osu-wiki-tools-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:45:58.878397 osu-wiki-tools-1.1.4/tests/
+-rw-rw-rw-   0        0        0    12105 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/tests/test_article_parser.py
+-rw-rw-rw-   0        0        0     3883 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/tests/test_check_links.py
+-rw-rw-rw-   0        0        0    21144 2023-02-26 14:18:34.000000 osu-wiki-tools-1.1.4/tests/test_check_outdated_articles.py
+-rw-rw-rw-   0        0        0     2354 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.4/tests/test_code_block_parser.py
+-rw-rw-rw-   0        0        0     1492 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.4/tests/test_comment_parser.py
+-rw-rw-rw-   0        0        0     4419 2023-06-05 18:36:12.000000 osu-wiki-tools-1.1.4/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     4370 2022-05-06 12:01:04.000000 osu-wiki-tools-1.1.4/tests/test_identifier_parser.py
+-rw-rw-rw-   0        0        0    28589 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/tests/test_link_checker.py
+-rw-rw-rw-   0        0        0     9219 2022-07-31 07:21:51.000000 osu-wiki-tools-1.1.4/tests/test_link_parser.py
+-rw-rw-rw-   0        0        0      849 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.4/tests/test_redirect_parser.py
+-rw-rw-rw-   0        0        0     2747 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.4/tests/test_reference_parser.py
+-rw-rw-rw-   0        0        0     4223 2023-06-05 18:38:34.000000 osu-wiki-tools-1.1.4/tests/test_yaml_rules.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:45:59.039024 osu-wiki-tools-1.1.4/wikitools/
+-rw-rw-rw-   0        0        0        0 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.4/wikitools/__init__.py
+-rw-rw-rw-   0        0        0     6547 2023-06-05 18:38:34.000000 osu-wiki-tools-1.1.4/wikitools/article_parser.py
+-rw-rw-rw-   0        0        0     3449 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.4/wikitools/code_block_parser.py
+-rw-rw-rw-   0        0        0     3029 2022-04-16 18:18:34.000000 osu-wiki-tools-1.1.4/wikitools/comment_parser.py
+-rw-rw-rw-   0        0        0      258 2022-05-06 12:30:44.000000 osu-wiki-tools-1.1.4/wikitools/console.py
+-rw-rw-rw-   0        0        0     3770 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/wikitools/errors.py
+-rw-rw-rw-   0        0        0     3042 2023-06-05 18:40:12.000000 osu-wiki-tools-1.1.4/wikitools/file_utils.py
+-rw-rw-rw-   0        0        0     1314 2022-07-31 07:21:51.000000 osu-wiki-tools-1.1.4/wikitools/git_utils.py
+-rw-rw-rw-   0        0        0     2993 2022-05-06 12:01:04.000000 osu-wiki-tools-1.1.4/wikitools/identifier_parser.py
+-rw-rw-rw-   0        0        0     5921 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/wikitools/link_checker.py
+-rw-rw-rw-   0        0        0     7820 2022-07-31 07:21:47.000000 osu-wiki-tools-1.1.4/wikitools/link_parser.py
+-rw-rw-rw-   0        0        0      553 2022-04-14 00:20:54.000000 osu-wiki-tools-1.1.4/wikitools/redirect_parser.py
+-rw-rw-rw-   0        0        0     2536 2022-04-14 08:51:50.000000 osu-wiki-tools-1.1.4/wikitools/reference_parser.py
+-rw-rw-rw-   0        0        0     5405 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/wikitools/yaml_rules.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:45:59.048119 osu-wiki-tools-1.1.4/wikitools_cli/
+-rw-rw-rw-   0        0        0       19 2023-06-05 18:43:06.000000 osu-wiki-tools-1.1.4/wikitools_cli/VERSION.py
+-rw-rw-rw-   0        0        0        0 2022-06-05 22:05:02.000000 osu-wiki-tools-1.1.4/wikitools_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:45:59.069905 osu-wiki-tools-1.1.4/wikitools_cli/commands/
+-rw-rw-rw-   0        0        0        0 2022-07-31 07:21:51.000000 osu-wiki-tools-1.1.4/wikitools_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0     6158 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/wikitools_cli/commands/check_links.py
+-rw-rw-rw-   0        0        0    10199 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/wikitools_cli/commands/check_outdated_articles.py
+-rw-rw-rw-   0        0        0     3766 2023-02-26 14:18:44.000000 osu-wiki-tools-1.1.4/wikitools_cli/commands/check_yaml.py
+-rw-rw-rw-   0        0        0     2270 2023-06-05 18:38:34.000000 osu-wiki-tools-1.1.4/wikitools_cli/osu_wiki_tools.py
+-rw-rw-rw-   0        0        0     1728 2022-06-20 03:50:12.000000 osu-wiki-tools-1.1.4/wikitools_cli/update_tournament_countries.py
```

### Comparing `osu-wiki-tools-1.1.3/LICENCE.md` & `osu-wiki-tools-1.1.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/PKG-INFO` & `osu-wiki-tools-1.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu-wiki-tools
-Version: 1.1.3
+Version: 1.1.4
 Summary: Various tools for osu! wiki contributors
 Home-page: https://github.com/Walavouchey/osu-wiki-tools
 Author: Walavouchey
 Author-email: wala@yui.tv
 Project-URL: Bug Tracker, https://github.com/Walavouchey/osu-wiki-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/PKG-INFO` & `osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu-wiki-tools
-Version: 1.1.3
+Version: 1.1.4
 Summary: Various tools for osu! wiki contributors
 Home-page: https://github.com/Walavouchey/osu-wiki-tools
 Author: Walavouchey
 Author-email: wala@yui.tv
 Project-URL: Bug Tracker, https://github.com/Walavouchey/osu-wiki-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `osu-wiki-tools-1.1.3/osu_wiki_tools.egg-info/SOURCES.txt` & `osu-wiki-tools-1.1.4/osu_wiki_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/setup.py` & `osu-wiki-tools-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_article_parser.py` & `osu-wiki-tools-1.1.4/tests/test_article_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_check_links.py` & `osu-wiki-tools-1.1.4/tests/test_check_links.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_check_outdated_articles.py` & `osu-wiki-tools-1.1.4/tests/test_check_outdated_articles.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_code_block_parser.py` & `osu-wiki-tools-1.1.4/tests/test_code_block_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_comment_parser.py` & `osu-wiki-tools-1.1.4/tests/test_comment_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_file_utils.py` & `osu-wiki-tools-1.1.4/tests/test_file_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from wikitools import file_utils
 
 class TestFileUtils:
     def test__list_all_article_files(self, root):
         article_paths = [
             'wiki/Article/en.md',
             'wiki/Article/fr.md',
+            'wiki/Article/fil.md',
             'wiki/Article/pt-br.md',
             'wiki/Article/zh-tw.md',
             'wiki/Article/TRANSLATING.md',
             'wiki/Article/TEMPLATE.md',
             'wiki/Category1/Article/en.md',
             'wiki/Category1/Article/fr.md',
             'wiki/Category1/Article/pt-br.md',
@@ -33,14 +34,15 @@
 
         assert multiset(file_utils.list_all_articles()) == multiset(utils.remove(article_paths, "TEMPLATE.md", "TRANSLATING.md"))
 
     def test__list_all_article_dirs(self, root):
         article_paths = [
             'wiki/Article/en.md',
             'wiki/Article/fr.md',
+            'wiki/Article/fil.md',
             'wiki/Article/pt-br.md',
             'wiki/Article/zh-tw.md',
             'wiki/Article/TRANSLATING.md',
             'wiki/Article/TEMPLATE.md',
             'wiki/Category1/Article/en.md',
             'wiki/Category1/Article/fr.md',
             'wiki/Category1/Article/pt-br.md',
@@ -59,27 +61,29 @@
 
         assert multiset(file_utils.list_all_article_dirs()) == multiset(set(os.path.dirname(path) for path in article_paths))
 
     def test__list_all_translations(self, root):
         article_paths = [
             'wiki/Article/en.md',
             'wiki/Article/fr.md',
+            'wiki/Article/fil.md',
             'wiki/Article/pt-br.md',
             'wiki/Article/zh-tw.md',
             'wiki/Article/TRANSLATING.md',
             'wiki/Article/TEMPLATE.md',
         ]
 
         utils.create_files(root, *((path, '# Article') for path in article_paths))
 
-        assert multiset(file_utils.list_all_translations(["wiki/Article"])) == multiset(article_paths[1:4])
+        assert multiset(file_utils.list_all_translations(["wiki/Article"])) == multiset(article_paths[1:5])
 
     def test_list_all_articles_and_newsposts(self, root):
         article_paths = [
             'wiki/Article/en.md',
+            'wiki/Article/fil.md',
             'wiki/Article/fr.md',
             'wiki/Article/pt-br.md',
             'wiki/Article/zh-tw.md',
             'wiki/Article/TRANSLATING.md',
             'wiki/Article/TEMPLATE.md',
         ]
 
@@ -93,8 +97,8 @@
             'news/2028-07-28-introducing-osu-lite-smartwatch-edition.md',
             '.remarkrc.js'
         ]
 
         utils.create_files(root, *((path, '# Article') for path in article_paths))
         utils.create_files(root, *((path, '# News post') for path in newspost_paths))
 
-        assert multiset(file_utils.list_all_articles_and_newsposts()) == multiset(article_paths[0:4] + newspost_paths[0:-1])
+        assert multiset(file_utils.list_all_articles_and_newsposts()) == multiset(article_paths[0:5] + newspost_paths[0:-1])
```

### Comparing `osu-wiki-tools-1.1.3/tests/test_identifier_parser.py` & `osu-wiki-tools-1.1.4/tests/test_identifier_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_link_checker.py` & `osu-wiki-tools-1.1.4/tests/test_link_checker.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_link_parser.py` & `osu-wiki-tools-1.1.4/tests/test_link_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_redirect_parser.py` & `osu-wiki-tools-1.1.4/tests/test_redirect_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_reference_parser.py` & `osu-wiki-tools-1.1.4/tests/test_reference_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/tests/test_yaml_rules.py` & `osu-wiki-tools-1.1.4/tests/test_yaml_rules.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/article_parser.py` & `osu-wiki-tools-1.1.4/wikitools/article_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/code_block_parser.py` & `osu-wiki-tools-1.1.4/wikitools/code_block_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/comment_parser.py` & `osu-wiki-tools-1.1.4/wikitools/comment_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/errors.py` & `osu-wiki-tools-1.1.4/wikitools/errors.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/file_utils.py` & `osu-wiki-tools-1.1.4/wikitools/file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,24 +28,26 @@
     )
 
 
 def is_article(path: str) -> bool:
     filename = os.path.basename(path)
     return (
         fnmatch.fnmatch(filename, "??.md") or
+        fnmatch.fnmatch(filename, "???.md") or
         fnmatch.fnmatch(filename, "??-??.md")
     )
 
 
 def is_translation(path: str) -> bool:
     filename = os.path.basename(path)
     return (
         filename != "en.md" and
         (
             fnmatch.fnmatch(filename, "??.md") or
+            fnmatch.fnmatch(filename, "???.md") or
             fnmatch.fnmatch(filename, "??-??.md")
         )
     )
 
 
 def is_original(path: str) -> bool:
     return os.path.basename(path) == "en.md"
```

### Comparing `osu-wiki-tools-1.1.3/wikitools/git_utils.py` & `osu-wiki-tools-1.1.4/wikitools/git_utils.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/identifier_parser.py` & `osu-wiki-tools-1.1.4/wikitools/identifier_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/link_checker.py` & `osu-wiki-tools-1.1.4/wikitools/link_checker.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/link_parser.py` & `osu-wiki-tools-1.1.4/wikitools/link_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/redirect_parser.py` & `osu-wiki-tools-1.1.4/wikitools/redirect_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/reference_parser.py` & `osu-wiki-tools-1.1.4/wikitools/reference_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools/yaml_rules.py` & `osu-wiki-tools-1.1.4/wikitools/yaml_rules.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools_cli/commands/check_links.py` & `osu-wiki-tools-1.1.4/wikitools_cli/commands/check_links.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools_cli/commands/check_outdated_articles.py` & `osu-wiki-tools-1.1.4/wikitools_cli/commands/check_outdated_articles.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools_cli/commands/check_yaml.py` & `osu-wiki-tools-1.1.4/wikitools_cli/commands/check_yaml.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools_cli/osu_wiki_tools.py` & `osu-wiki-tools-1.1.4/wikitools_cli/osu_wiki_tools.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-1.1.3/wikitools_cli/update_tournament_countries.py` & `osu-wiki-tools-1.1.4/wikitools_cli/update_tournament_countries.py`

 * *Files identical despite different names*

