# Comparing `tmp/textarium-0.1.1.tar.gz` & `tmp/textarium-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textarium-0.1.1.tar", max compression
+gzip compressed data, was "textarium-0.1.2.tar", max compression
```

## Comparing `textarium-0.1.1.tar` & `textarium-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1063 2023-06-04 21:46:32.803392 textarium-0.1.1/LICENSE
--rw-r--r--   0        0        0     1249 2023-06-04 21:46:32.803392 textarium-0.1.1/README.md
--rw-r--r--   0        0        0      578 2023-06-04 21:46:32.803392 textarium-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-04 21:46:32.803392 textarium-0.1.1/textarium/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-04 21:46:32.803392 textarium-0.1.1/textarium/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 21:46:32.803392 textarium-0.1.1/textarium/collections/__init__.py
--rw-r--r--   0        0        0     2484 2023-06-04 21:46:32.803392 textarium-0.1.1/textarium/collections/en_stopwords.txt
--rw-r--r--   0        0        0       14 2023-06-04 21:46:32.803392 textarium-0.1.1/textarium/collections/ru_stopwords.txt
--rw-r--r--   0        0        0      305 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/collections/stopwords.py
--rw-r--r--   0        0        0     1509 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/extraction.py
--rw-r--r--   0        0        0      145 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/models.py
--rw-r--r--   0        0        0     4547 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/preprocessing.py
--rw-r--r--   0        0        0        0 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/tests/__init__.py
--rw-r--r--   0        0        0      431 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/tests/test_collections.py
--rw-r--r--   0        0        0     1947 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/tests/test_extraction.py
--rw-r--r--   0        0        0     2630 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/tests/test_preprocessing.py
--rw-r--r--   0        0        0      727 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/tests/test_text.py
--rw-r--r--   0        0        0     1092 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/text.py
--rw-r--r--   0        0        0      567 2023-06-04 21:46:32.811392 textarium-0.1.1/textarium/utils.py
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 textarium-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-05 15:11:50.925595 textarium-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1486 2023-06-05 15:11:50.925595 textarium-0.1.2/README.md
+-rw-r--r--   0        0        0      602 2023-06-05 15:11:50.929596 textarium-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/.DS_Store
+-rw-r--r--   0        0        0     1829 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/__init__.py
+-rw-r--r--   0        0        0     5229 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/en_stopwords.txt
+-rw-r--r--   0        0        0     4536 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/ru_stopwords.txt
+-rw-r--r--   0        0        0      305 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/stopwords.py
+-rw-r--r--   0        0        0     1509 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/extraction.py
+-rw-r--r--   0        0        0      216 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/models.py
+-rw-r--r--   0        0        0     4655 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test__all__.py
+-rw-r--r--   0        0        0      431 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_collections.py
+-rw-r--r--   0        0        0     2243 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_extraction.py
+-rw-r--r--   0        0        0     2935 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     1638 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_text.py
+-rw-r--r--   0        0        0     1092 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/text.py
+-rw-r--r--   0        0        0      567 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/utils.py
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 textarium-0.1.2/PKG-INFO
```

### Comparing `textarium-0.1.1/LICENSE` & `textarium-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textarium-0.1.1/README.md` & `textarium-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,38 @@
 [![License](https://img.shields.io/pypi/l/textarium)](https://github.com/6b656b/textarium/blob/main/LICENSE)
 [![Activity](https://img.shields.io/github/commit-activity/m/6b656b/textarium)](https://github.com/6b656b/textarium/pulse)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## What is it?
 
-**textarium** is a Python package that provides flexible text processing functions designed to 
-make working with texts intuitive and easy. It aims to be the high-level tool for
-preparing text-data for complex analysis or NLP modeling.
+**textarium** is a Python package that provides flexible text analysis functions designed to 
+make text analysis intuitive and easy. It aims to be the high-level tool for
+preparing text-data and complex analysis or NLP modeling.
 
 ## Installation
 Binary installer for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/textarium).
 
 ```sh
 # Type this in your command-line
 pip install textarium
 ```
+
+## Getting started
+
+```py
+from textarium import Text
+import nltk
+nltk.download('wordnet')
+
+s = "This a text example. You can preprocess and analyze it with this package."
+text = Text(s, lang='en')
+text.prepare()
+
+print(text.prepared_text)
+```
 ## License
 [MIT](LICENSE)
 
 ## Documentation
 The official documentation is hosted on Github.io: https://6b656b.github.io/textarium
```

### Comparing `textarium-0.1.1/pyproject.toml` & `textarium-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "textarium"
-version = "0.1.1"
-description = "Package for text cleaning and processing"
+version = "0.1.2"
+description = "Textarium is a Python package for text analysis"
 authors = ["6b656b"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytest = "^7.1.3"
 setuptools = "^65.6.3"
 nltk = "^3.8.1"
 razdel = "^0.5.0"
 pymorphy2 = "^0.9.1"
 pymorphy2-dicts = "^2.4.393442.3710985"
+toml = "^0.10.2"
 
 
 [tool.poetry.group.test.dependencies]
 unittest = "^0.0"
 nose = "^1.3.7"
```

### Comparing `textarium-0.1.1/textarium/.DS_Store` & `textarium-0.1.2/textarium/.DS_Store`

 * *Files identical despite different names*

### Comparing `textarium-0.1.1/textarium/extraction.py` & `textarium-0.1.2/textarium/extraction.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.1/textarium/preprocessing.py` & `textarium-0.1.2/textarium/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Text cleaning and preprocessing functions.
 """
 
 import string
 import re
 from typing import List, Union
-from textarium.models import morph_ru
+from textarium.models import morph_ru, morph_en
 import textarium.extraction as extraction
 
 def remove_extra_spaces(text: str) -> str:
     """Removes extra spaces from a string
 
     Args:
         text (str): Any string
@@ -145,15 +145,15 @@
         text (str): Any string
 
     Returns:
         str: Lowercase text
     """
     return text.lower()
 
-def lemmatize(text: Union[List, str], lang: str = 'ru') -> str:
+def lemmatize(text: Union[List, str], lang: str) -> str:
     """Lemmatizes all words in a text
 
     Args:
         text (Union[List, str]): Any string or a list of words
         morph (_type_): _description_
 
     Returns:
@@ -162,11 +162,13 @@
     if type(text) == str:
         words = extraction.extract_words(text)
     elif type(text) == list:
         words = text
     
     if lang == 'ru':
         lemmatized_words = [morph_ru.parse(w)[0].normal_form for w in words]
+    elif lang == 'en':
+        lemmatized_words = [morph_en.lemmatize(w) for w in words]
     else:
-        raise NotImplementedError("This package supports following languages: 'ru' (russian).")
+        raise NotImplementedError("This package supports following languages: 'en' (english), 'ru' (russian).")
 
     return " ".join(lemmatized_words)
```

### Comparing `textarium-0.1.1/textarium/tests/test_extraction.py` & `textarium-0.1.2/textarium/tests/test_extraction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from unittest import TestCase
 
 import textarium.extraction as extraction
 
 class TestExtraction(TestCase):
-    def test_extract_words_0(self):
+    def test_extract_words_en_0(self):
         test_input = "This line has 5 tokens"
         expected_result = ["This", "line", "has", "5", "tokens"]
         result = extraction.extract_words(test_input)
         self.assertEqual(expected_result, result)
 
+    def test_extract_words_ru_0(self):
+        test_input = "В этой строке 5 токенов"
+        expected_result = ["В", "этой", "строке", "5", "токенов"]
+        result = extraction.extract_words(test_input)
+        self.assertEqual(expected_result, result)
+
     def test_extract_sentences_en_0(self):
         text_input = """
         Hello! My name is Robbie. 
         Please, write an email to Mr. Parker. 
         His email: parker@gmail.com.
         """
         expected_result = [
```

### Comparing `textarium-0.1.1/textarium/tests/test_preprocessing.py` & `textarium-0.1.2/textarium/tests/test_preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,12 +45,18 @@
 
     def test_remove_punctuation_0(self):
         test_input = "Hello! I ne-ed remove, all : punctuation."
         expected_result = "Hello I ne ed remove all punctuation"
         result = preprocessing.remove_punctuation(test_input)
         self.assertEqual(expected_result, result)
 
-    def test_lemmatize_0(self):
+    def test_lemmatize_ru_0(self):
         test_input = "эти дети скоро пойдут в школу и выучат английский и немецкий языки"
         expected_result = "этот ребёнок скоро пойти в школа и выучить английский и немецкий язык"
-        result = preprocessing.lemmatize(test_input)
+        result = preprocessing.lemmatize(test_input, lang='ru')
+        self.assertEqual(expected_result, result)
+
+    def test_lemmatize_en_0(self):
+        test_input = "These children are doing very dangerous things"
+        expected_result = "These child are doing very dangerous thing"
+        result = preprocessing.lemmatize(test_input, lang='en')
         self.assertEqual(expected_result, result)
```

### Comparing `textarium-0.1.1/textarium/text.py` & `textarium-0.1.2/textarium/text.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.1/textarium/utils.py` & `textarium-0.1.2/textarium/utils.py`

 * *Files identical despite different names*

