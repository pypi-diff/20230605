# Comparing `tmp/epubsum-0.2.tar.gz` & `tmp/epubsum-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubsum-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "epubsum-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `epubsum-0.2.tar` & `epubsum-0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       72 2023-06-04 03:35:53.450919 epubsum-0.2/.gitignore
--rw-r--r--   0        0        0      344 2023-05-20 22:00:00.000000 epubsum-0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-06-04 03:37:00.100590 epubsum-0.2/LICENSE
--rw-r--r--   0        0        0      382 2023-06-04 05:50:00.000000 epubsum-0.2/README.md
--rw-r--r--   0        0        0     1113 2023-06-04 05:04:00.000000 epubsum-0.2/epubsum/__init__.py
--rw-r--r--   0        0        0       69 2022-08-29 23:28:00.000000 epubsum-0.2/epubsum/__main__.py
--rw-r--r--   0        0        0     2242 2023-06-04 05:58:00.000000 epubsum-0.2/epubsum/epubsum.py
--rw-r--r--   0        0        0      745 2023-06-03 22:49:00.000000 epubsum-0.2/pyproject.toml
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 epubsum-0.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-06-04 03:35:53.450919 epubsum-0.3/.gitignore
+-rw-r--r--   0        0        0      344 2023-05-20 22:00:00.000000 epubsum-0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-06-04 03:37:00.100590 epubsum-0.3/LICENSE
+-rw-r--r--   0        0        0      558 2023-06-05 05:09:18.242738 epubsum-0.3/README.md
+-rw-r--r--   0        0        0     1560 2023-06-05 04:42:00.000000 epubsum-0.3/epubsum/__init__.py
+-rw-r--r--   0        0        0       69 2022-08-29 23:28:00.000000 epubsum-0.3/epubsum/__main__.py
+-rw-r--r--   0        0        0     2411 2023-06-05 04:37:00.000000 epubsum-0.3/epubsum/epubsum.py
+-rw-r--r--   0        0        0      745 2023-06-03 22:49:00.000000 epubsum-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 epubsum-0.3/PKG-INFO
```

### Comparing `epubsum-0.2/LICENSE` & `epubsum-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epubsum-0.2/epubsum/epubsum.py` & `epubsum-0.3/epubsum/epubsum.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 from cleantext import clean
 from ebooklib import ITEM_DOCUMENT, epub
 from textsum.summarize import Summarizer
 from textwrap import wrap
 
 
 def extract_sections_from_epub(epub_file_path):
-    book = epub.read_epub(epub_file_path)
+    try:
+        book = epub.read_epub(epub_file_path)
+    except:
+        print(f'Failed to read epub file {epub_file_path}; file may be missing or corrupted')
+        return {}
+
     section_texts = {}
 
     for item in book.get_items():
         if isinstance(item, epub.EpubHtml) and item.is_chapter():
             title = item.title if item.title else item.get_name()
             content = item.get_content()
             soup = BeautifulSoup(content, 'html.parser')
@@ -31,35 +36,35 @@
         paragraphs = summary.split('\n')
         summary = '\n\n'.join(['\n'.join(wrap(p)) for p in paragraphs])
         parts.append(summary)
 
     return ''.join(parts)
 
 
-def summarize_epub_files(summarizer, directory, preamble, overwrite):
+def summarize_epub_files(summarizer, directory, preamble, suffix, overwrite):
     for root, dirs, files in os.walk(directory):
         for file in files:
             if file.endswith('.epub'):
                 epub_path = os.path.join(root, file)
-                summary_path = os.path.splitext(epub_path)[0] + '-summary.txt'
+                summary_path = os.path.splitext(epub_path)[0] + suffix
                 if overwrite or not os.path.exists(summary_path):
                     summary = summarize_epub_file(summarizer, epub_path, preamble)
                     with open(summary_path, 'w') as summary_file:
                         summary_file.write(summary)
 
 
-def summarize(target, preamble='', large=False, overwrite=False):
+def summarize(target, preamble='', suffix='-summary.txt', large=False, overwrite=False):
     if large:
         summarizer = Summarizer(model_name_or_path='pszemraj/long-t5-tglobal-xl-16384-book-summary')
     else:
         # pszemraj/long-t5-tglobal-base-16384-book-summary
         summarizer = Summarizer()
 
     if os.path.isdir(target):
-        summarize_epub_files(summarizer, target, preamble, overwrite)
+        summarize_epub_files(summarizer, target, preamble, suffix, overwrite)
     else:
         print(summarize_epub_file(summarizer, target, preamble))
```

### Comparing `epubsum-0.2/pyproject.toml` & `epubsum-0.3/pyproject.toml`

 * *Files identical despite different names*

