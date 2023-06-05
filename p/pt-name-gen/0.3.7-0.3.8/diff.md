# Comparing `tmp/pt_name_gen-0.3.7.tar.gz` & `tmp/pt_name_gen-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_name_gen-0.3.7.tar", last modified: Wed Mar 29 15:16:21 2023, max compression
+gzip compressed data, was "pt_name_gen-0.3.8.tar", last modified: Mon Jun  5 20:34:32 2023, max compression
```

## Comparing `pt_name_gen-0.3.7.tar` & `pt_name_gen-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-03-29 15:16:21.568471 pt_name_gen-0.3.7/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1678 2023-03-29 15:16:21.568255 pt_name_gen-0.3.7/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1396 2022-12-28 17:58:01.000000 pt_name_gen-0.3.7/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-03-29 15:16:21.565452 pt_name_gen-0.3.7/pt_name_gen/
--rw-r--r--   0 filterfeed   (501) staff       (20)        0 2022-12-28 15:35:12.000000 pt_name_gen-0.3.7/pt_name_gen/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)  5439608 2023-03-29 14:11:41.000000 pt_name_gen-0.3.7/pt_name_gen/first_names.csv
--rw-r--r--   0 filterfeed   (501) staff       (20)     6773 2023-03-29 14:15:43.000000 pt_name_gen-0.3.7/pt_name_gen/last_names.csv
--rw-r--r--   0 filterfeed   (501) staff       (20)     1551 2023-03-29 15:14:35.000000 pt_name_gen-0.3.7/pt_name_gen/name_match.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     2444 2023-03-29 15:16:02.000000 pt_name_gen-0.3.7/pt_name_gen/pt_name_gen.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-03-29 15:16:21.567930 pt_name_gen-0.3.7/pt_name_gen.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1678 2023-03-29 15:16:21.000000 pt_name_gen-0.3.7/pt_name_gen.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      362 2023-03-29 15:16:21.000000 pt_name_gen-0.3.7/pt_name_gen.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-03-29 15:16:21.000000 pt_name_gen-0.3.7/pt_name_gen.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       58 2023-03-29 15:16:21.000000 pt_name_gen-0.3.7/pt_name_gen.egg-info/entry_points.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       10 2023-03-29 15:16:21.000000 pt_name_gen-0.3.7/pt_name_gen.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-03-29 15:16:21.000000 pt_name_gen-0.3.7/pt_name_gen.egg-info/top_level.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-03-29 15:16:21.568536 pt_name_gen-0.3.7/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      714 2023-03-29 15:16:20.000000 pt_name_gen-0.3.7/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-05 20:34:32.892175 pt_name_gen-0.3.8/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2534 2023-06-05 20:34:32.892024 pt_name_gen-0.3.8/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1396 2022-12-28 17:58:01.000000 pt_name_gen-0.3.8/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-05 20:34:32.890925 pt_name_gen-0.3.8/pt_name_gen/
+-rw-r--r--   0 filterfeed   (501) staff       (20)      103 2023-06-05 20:16:46.000000 pt_name_gen-0.3.8/pt_name_gen/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1856 2023-06-05 20:29:46.000000 pt_name_gen-0.3.8/pt_name_gen/name_match.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2444 2023-03-29 15:16:02.000000 pt_name_gen-0.3.8/pt_name_gen/pt_name_gen.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-05 20:34:32.891831 pt_name_gen-0.3.8/pt_name_gen.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2534 2023-06-05 20:34:32.000000 pt_name_gen-0.3.8/pt_name_gen.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      269 2023-06-05 20:34:32.000000 pt_name_gen-0.3.8/pt_name_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-05 20:34:32.000000 pt_name_gen-0.3.8/pt_name_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       10 2023-06-05 20:34:32.000000 pt_name_gen-0.3.8/pt_name_gen.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-05 20:34:32.000000 pt_name_gen-0.3.8/pt_name_gen.egg-info/top_level.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-05 20:34:32.892225 pt_name_gen-0.3.8/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1080 2023-06-05 20:34:22.000000 pt_name_gen-0.3.8/setup.py
```

### Comparing `pt_name_gen-0.3.7/PKG-INFO` & `pt_name_gen-0.3.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: pt_name_gen
-Version: 0.3.7
-Summary: A name generator in Portuguese, with support to gender classification. Um gerador de nomes em português, com suporte para classificação de gênero.
-Author: Victor Figueredo
-Description-Content-Type: text/markdown
-
 # pt_name_gen #
 
 A Python module for generating random names in Portuguese.
 
 ### Installation ###
 
 To install the name_generator module, use pip:
@@ -44,8 +37,8 @@
 ### Dependencies ### 
 `pt_name_gen` requires the `unidecode` library to remove special characters from the generated names.
 
 ### License ###
 
 The `pt_name_gen` module is released under the MIT License.
 
-I hope this helps! Let me know if you have any questions.
+I hope this helps! Let me know if you have any questions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pt_name_gen-0.3.7/pt_name_gen/name_match.py` & `pt_name_gen-0.3.8/pt_name_gen/name_match.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,22 @@
-"""
-# Usage
-name_to_search = "Victor"
-name_matcher = NameMatcher()
-gender = name_matcher.find_name(name_to_search)
-
-if gender is not None:
-    print(f"Gender for the name '{name_to_search}' is: {gender}")
-else:
-    print(f"No matching name found")
-"""
-
 import csv
 from typing import Optional, Dict
 import importlib.resources
 
 class NameMatcher:
     """Class to find the gender of a given name by searching in a CSV file.
     """
+    instance = None
+    name_data: Dict[str, str] = {}
 
     def __init__(self, file_name: str = "first_names.csv"):
-        self.file_name = file_name
-        self.name_data = self._load_name_data()
+        if not NameMatcher.instance:
+            NameMatcher.instance = self
+            self.file_name = file_name
+            NameMatcher.name_data = self._load_name_data()
 
     def _load_name_data(self) -> Dict[str, str]:
         """
         Load name data from the CSV file into a dictionary.
 
         Returns:
             Dict[str, str]: A dictionary with names as keys and gender classification as values.
@@ -48,9 +40,23 @@
         Args:
             name (str): The name to search for.
 
         Returns:
             Optional[str]: The gender of the name if found, otherwise None.
         """
         name = name.upper()
-        return self.name_data.get(name, None)
+        return NameMatcher.name_data.get(name, None)
+
+    @staticmethod
+    def get_gender(name: str) -> Optional[str]:
+        """
+        Get the gender of the given name.
 
+        Args:
+            name (str): The name to search for.
+
+        Returns:
+            Optional[str]: The gender of the name if found, otherwise None.
+        """
+        if not NameMatcher.instance:
+            NameMatcher()
+        return NameMatcher.instance.find_name(name)
```

### Comparing `pt_name_gen-0.3.7/pt_name_gen/pt_name_gen.py` & `pt_name_gen-0.3.8/pt_name_gen/pt_name_gen.py`

 * *Files identical despite different names*

