# Comparing `tmp/Sampacks-0.1.tar.gz` & `tmp/sampacks-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sampacks-0.1.tar", last modified: Mon Jun  5 07:43:38 2023, max compression
+gzip compressed data, was "sampacks-0.2.tar", last modified: Mon Jun  5 07:49:40 2023, max compression
```

## Comparing `Sampacks-0.1.tar` & `sampacks-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 07:43:38.925737 Sampacks-0.1/
--rw-rw-rw-   0        0        0     3127 2023-06-05 07:43:38.924747 Sampacks-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 07:43:38.909754 Sampacks-0.1/Sampacks/
--rw-rw-rw-   0        0        0       36 2023-06-05 07:43:23.000000 Sampacks-0.1/Sampacks/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-05 07:43:17.000000 Sampacks-0.1/Sampacks/funcs.py
--rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 Sampacks-0.1/Sampacks/non_use_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:43:38.922742 Sampacks-0.1/Sampacks.egg-info/
--rw-rw-rw-   0        0        0     3127 2023-06-05 07:43:38.000000 Sampacks-0.1/Sampacks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-05 07:43:38.000000 Sampacks-0.1/Sampacks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 07:43:38.000000 Sampacks-0.1/Sampacks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-05 07:43:38.000000 Sampacks-0.1/Sampacks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 07:43:38.000000 Sampacks-0.1/Sampacks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 07:43:38.925737 Sampacks-0.1/setup.cfg
--rw-rw-rw-   0        0        0     3379 2023-06-05 07:42:42.000000 Sampacks-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:49:40.959871 sampacks-0.2/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 07:49:40.958876 sampacks-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 07:49:40.946869 sampacks-0.2/sampacks/
+-rw-rw-rw-   0        0        0       36 2023-06-05 07:49:10.000000 sampacks-0.2/sampacks/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-06-05 07:49:07.000000 sampacks-0.2/sampacks/funcs.py
+-rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 sampacks-0.2/sampacks/non_use_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:49:40.956885 sampacks-0.2/sampacks.egg-info/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 07:49:40.000000 sampacks-0.2/sampacks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-05 07:49:40.000000 sampacks-0.2/sampacks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:49:40.000000 sampacks-0.2/sampacks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-05 07:49:40.000000 sampacks-0.2/sampacks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 07:49:40.000000 sampacks-0.2/sampacks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:49:40.960868 sampacks-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3379 2023-06-05 07:49:31.000000 sampacks-0.2/setup.py
```

### Comparing `Sampacks-0.1/PKG-INFO` & `sampacks-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Sampacks
-Version: 0.1
+Name: sampacks
+Version: 0.2
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `Sampacks-0.1/Sampacks/funcs.py` & `sampacks-0.2/sampacks/funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import requests
 import random
-from Sampacks.non_use_funcs import (
+from sampacks.non_use_funcs import (
     image_downloader,
     image_check
 )
 
 class mainfuncs:
     def __init__(self):
         pass
```

### Comparing `Sampacks-0.1/Sampacks/non_use_funcs.py` & `sampacks-0.2/sampacks/non_use_funcs.py`

 * *Files identical despite different names*

### Comparing `Sampacks-0.1/Sampacks.egg-info/PKG-INFO` & `sampacks-0.2/sampacks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Sampacks
-Version: 0.1
+Name: sampacks
+Version: 0.2
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `Sampacks-0.1/setup.py` & `sampacks-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Furthermore, Sampacks includes a powerful code generation module, which automates the process of generating boilerplate code. This module allows users to create skeleton code for various frameworks, libraries, and design patterns with just a few simple commands. Whether you're starting a new project or integrating an existing one, Sampacks' code generation module helps you get up and running swiftly, eliminating the need for manual and error-prone boilerplate code creation.
 
 Sampacks also comes equipped with an intelligent code completion feature, providing real-time suggestions and autocompletion for code snippets, functions, and variables. This intelligent assistant analyzes your code as you write, offering helpful suggestions based on context, syntax, and the underlying codebase. This feature saves significant time by reducing the need to look up function signatures or constantly switch between documentation and code files.
 
 With its user-friendly interface and comprehensive documentation, Sampacks ensures a smooth learning curve and seamless integration into existing development workflows. By leveraging Sampacks' powerful functions, snippets, and code generation capabilities, developers can write high-quality code faster, optimize their workflow, and focus on building innovative and robust applications."""
 
-setup(name="Sampacks", version="0.1", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
+setup(name="sampacks", version="0.2", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
 packages=find_packages(),
 install_requires=[
     "Functions",
     "pillow",
     'setuptools',
     'requests'
 ], extra_requires=["twine>=4.0.2", "pytest>=7.0"],
```

