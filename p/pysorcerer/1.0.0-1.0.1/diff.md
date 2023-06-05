# Comparing `tmp/pysorcerer-1.0.0.tar.gz` & `tmp/pysorcerer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysorcerer-1.0.0.tar", last modified: Fri Jun  2 17:16:12 2023, max compression
+gzip compressed data, was "pysorcerer-1.0.1.tar", last modified: Mon Jun  5 15:35:46 2023, max compression
```

## Comparing `pysorcerer-1.0.0.tar` & `pysorcerer-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:16:12.584338 pysorcerer-1.0.0/
--rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 pysorcerer-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1239 2023-06-02 17:16:12.584338 pysorcerer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1988 2023-06-02 17:12:53.000000 pysorcerer-1.0.0/README.md
--rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 pysorcerer-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-02 17:16:12.568713 pysorcerer-1.0.0/pysorcerer.egg-info/
--rw-rw-rw-   0        0        0     1239 2023-06-02 17:16:12.000000 pysorcerer-1.0.0/pysorcerer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-02 17:16:12.000000 pysorcerer-1.0.0/pysorcerer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:16:12.000000 pysorcerer-1.0.0/pysorcerer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 17:16:12.000000 pysorcerer-1.0.0/pysorcerer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-02 17:16:12.000000 pysorcerer-1.0.0/pysorcerer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13665 2023-06-02 17:12:16.000000 pysorcerer-1.0.0/pysorcerer.py
--rw-rw-rw-   0        0        0       42 2023-06-02 17:16:12.584338 pysorcerer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1351 2023-06-02 17:13:21.000000 pysorcerer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:35:46.335870 pysorcerer-1.0.1/
+-rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 pysorcerer-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1239 2023-06-05 15:35:46.308887 pysorcerer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-06-05 15:33:10.000000 pysorcerer-1.0.1/README.md
+-rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 pysorcerer-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-05 15:35:46.276906 pysorcerer-1.0.1/pysorcerer.egg-info/
+-rw-rw-rw-   0        0        0     1239 2023-06-05 15:35:45.000000 pysorcerer-1.0.1/pysorcerer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-05 15:35:46.000000 pysorcerer-1.0.1/pysorcerer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:35:45.000000 pysorcerer-1.0.1/pysorcerer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 15:35:45.000000 pysorcerer-1.0.1/pysorcerer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 15:35:45.000000 pysorcerer-1.0.1/pysorcerer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12714 2023-06-04 08:09:14.000000 pysorcerer-1.0.1/pysorcerer.py
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:35:46.342866 pysorcerer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1351 2023-06-05 15:33:22.000000 pysorcerer-1.0.1/setup.py
```

### Comparing `pysorcerer-1.0.0/LICENSE` & `pysorcerer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysorcerer-1.0.0/PKG-INFO` & `pysorcerer-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysorcerer
-Version: 1.0.0
+Version: 1.0.1
 Summary: All the power of Python...in the palm of your hand.
 Author: Omer Drkić
 Author-email: omerdrkic2501@gmail.com
 License: Boost Software License 1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `pysorcerer-1.0.0/README.md` & `pysorcerer-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,8 +24,14 @@
 
 ### `choose(*values)`
 
 The `choose()` function returns a randomly chosen item from the specified list which can have as many items. For example, `choose("apple", "banana", "pear")` will return either "apple", "banana", or "pear".
 
 ## Support
 
-If you have any suggestions or ideas, please share them with me through e-mail. If you have any critics, be sure to e-mail as well. Also, please report any bugs you find - that way you help the rest of the community. Thank you for using Pysorcerer!
+If you have any suggestions or ideas, please share them with me through e-mail. If you have any critics, be sure to e-mail as well. Also, please report any bugs you find - that way you help the rest of the community. Thank you for using Pysorcerer!
+
+## Changelogs
+
+Fixes:
+
+- Draw functions no longer output any weird lines.
```

### Comparing `pysorcerer-1.0.0/pysorcerer.egg-info/PKG-INFO` & `pysorcerer-1.0.1/pysorcerer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysorcerer
-Version: 1.0.0
+Version: 1.0.1
 Summary: All the power of Python...in the palm of your hand.
 Author: Omer Drkić
 Author-email: omerdrkic2501@gmail.com
 License: Boost Software License 1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `pysorcerer-1.0.0/pysorcerer.py` & `pysorcerer-1.0.1/pysorcerer.py`

 * *Files 20% similar despite different names*

```diff
@@ -506,103 +506,77 @@
 
 class drawclass:
   def line(length: int, formation: int = 0, fixed_width: bool = True):
     """
     Draws a line in the console using full block characters.
     """
     if fixed_width:
-      if formation == 0:
-        for i in range(length):
-          print("██", end = "")
-      elif formation == 1:
-        indent = 0
-        for i in range(length):
-          for i in range(indent):
-            print("  ", end = "")
-          print("██", end = "\n")
-          indent += 1
-      elif formation == 2:
-        for i in range(length):
-          print("██", end = "\n")
-      elif formation == 3:
-        indent = length - 1
-        for i in range(length):
-          for i in range(indent):
-            print("  ", end = "")
-          print("██", end = "\n")
-          indent -= 1
+      block = "██"
+      space = "  "
     else:
-      if formation == 0:
-        for i in range(length):
-          print("█", end = "")
-      elif formation == 1:
-        indent = 0
-        for i in range(length):
-          for i in range(indent):
-            print(" ", end = "")
-          print("█", end = "\n")
-          indent += 1
-      elif formation == 2:
-        for i in range(length):
-          print("█", end = "\n")
-      elif formation == 3:
-        indent = length - 1
-        for i in range(length):
-          for i in range(indent):
-            print(" ", end = "")
-          print("█", end = "\n")
-          indent -= 1
-    print()
+      block = "█"
+      space = " "
+    if formation == 0:
+      for i in range(length):
+        print(block, end = "")
+    elif formation == 1:
+      indent = 0
+      for i in range(length):
+        for i in range(indent):
+          print(space, end = "")
+        print(block, end = "\n")
+        indent += 1
+    elif formation == 2:
+      for i in range(length):
+        print(block, end = "\n")
+    elif formation == 3:
+      indent = length - 1
+      for i in range(length):
+        for i in range(indent):
+          print(space, end = "")
+        print(block, end = "\n")
+        indent -= 1
 
   def rect(width: int, height: int, fixed_width: bool = True):
     """
     Draws a rectangle in the console using full block characters.
     """
     if fixed_width:
-      for i in range(height):
-        for i in range(width):
-          print("██", end = "")
-        print()
+      block = "██"
     else:
-      for i in range(height):
-        for i in range(width):
-          print("█", end = "")
-        print()
-    print()
+      block = "█"
+    for i in range(height):
+      for i in range(width):
+        print(block, end = "")
+      print()
 
   def rectb(width: int, height: int, fixed_width: bool = True):
     """
     Draws a rectangle border in the console using full block characters.
     """
     if fixed_width:
-      for i in range(width):
-        print("██", end = "")
-      print()
-      for i in range(height):
-        print("██", end = "")
-        for i in range(2, width):
-          print("  ", end = "")
-        print("██", end = "")
-        print()
-      for i in range(width):
-        print("██", end = "")
+      block = "██"
+      space = "  "
     else:
-      for i in range(width):
-        print("█", end = "")
+      block = "█"
+      space = " "
+    for i in range(width):
+      print(block, end = "")
+    print()
+    for i in range(2, height):
+      print(block, end = "")
+      for i in range(2, width):
+        print(space, end = "")
+      print(block, end = "")
       print()
-      for i in range(height):
-        print("█", end = "")
-        for i in range(2, width):
-          print(" ", end = "")
-        print("█", end = "")
-        print()
-      for i in range(width):
-        print("█", end = "")
+    for i in range(width):
+      print(block, end = "")
     print()
 
+
 math = mathclass
 """
 A sub-class of Pysorcerer that extends the math library.
 """
 
 draw = drawclass
 """
```

### Comparing `pysorcerer-1.0.0/setup.py` & `pysorcerer-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿from setuptools import setup
 
 setup(
   name = "pysorcerer",
-  version = "1.0.0",
+  version = "1.0.1",
   description = "All the power of Python...in the palm of your hand.",
   long_description = "Pysorcerer is a module programmed by Omer Drkić that adds loads of new features and makes Python easier to use. The module adds some features that the developer felt like they were missing from Python. It also adds some extension to the 'math' library and to the actual Python environment, as well as some useful data manipulation tools.",
   author = "Omer Drkić",
   author_email = "omerdrkic2501@gmail.com",
   py_modules = [
     "pysorcerer"
   ],
```

