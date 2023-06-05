# Comparing `tmp/PyShortsByAbdus-0.3.tar.gz` & `tmp/PyShortsByAbdus-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyShortsByAbdus-0.3.tar", last modified: Mon Jun  5 07:06:31 2023, max compression
+gzip compressed data, was "PyShortsByAbdus-0.4.tar", last modified: Mon Jun  5 07:10:30 2023, max compression
```

## Comparing `PyShortsByAbdus-0.3.tar` & `PyShortsByAbdus-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.083500 PyShortsByAbdus-0.3/
--rw-rw-rw-   0        0        0     3134 2023-06-05 07:06:31.080504 PyShortsByAbdus-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.053504 PyShortsByAbdus-0.3/PyShorts/
-drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.077501 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/
--rw-rw-rw-   0        0        0        0 2023-06-04 14:35:09.000000 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/__init__.py
--rw-rw-rw-   0        0        0     5351 2023-06-05 07:04:02.000000 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/funcs.py
--rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/non_use_funcs.py
--rw-rw-rw-   0        0        0      218 2023-06-05 06:49:36.000000 PyShortsByAbdus-0.3/PyShorts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.068500 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/
--rw-rw-rw-   0        0        0     3134 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 07:06:31.084501 PyShortsByAbdus-0.3/setup.cfg
--rw-rw-rw-   0        0        0     3386 2023-06-04 13:40:29.000000 PyShortsByAbdus-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:10:30.972780 PyShortsByAbdus-0.4/
+-rw-rw-rw-   0        0        0     3134 2023-06-05 07:10:30.971781 PyShortsByAbdus-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 07:10:30.951781 PyShortsByAbdus-0.4/PyShorts/
+drwxrwxrwx   0        0        0        0 2023-06-05 07:10:30.969781 PyShortsByAbdus-0.4/PyShorts/Sub_Functions/
+-rw-rw-rw-   0        0        0        0 2023-06-04 14:35:09.000000 PyShortsByAbdus-0.4/PyShorts/Sub_Functions/__init__.py
+-rw-rw-rw-   0        0        0     5351 2023-06-05 07:04:02.000000 PyShortsByAbdus-0.4/PyShorts/Sub_Functions/funcs.py
+-rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 PyShortsByAbdus-0.4/PyShorts/Sub_Functions/non_use_funcs.py
+-rw-rw-rw-   0        0        0       41 2023-06-05 07:09:47.000000 PyShortsByAbdus-0.4/PyShorts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:10:30.962782 PyShortsByAbdus-0.4/PyShortsByAbdus.egg-info/
+-rw-rw-rw-   0        0        0     3134 2023-06-05 07:10:30.000000 PyShortsByAbdus-0.4/PyShortsByAbdus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-05 07:10:30.000000 PyShortsByAbdus-0.4/PyShortsByAbdus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:10:30.000000 PyShortsByAbdus-0.4/PyShortsByAbdus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-05 07:10:30.000000 PyShortsByAbdus-0.4/PyShortsByAbdus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 07:10:30.000000 PyShortsByAbdus-0.4/PyShortsByAbdus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:10:30.973782 PyShortsByAbdus-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3386 2023-06-05 07:10:22.000000 PyShortsByAbdus-0.4/setup.py
```

### Comparing `PyShortsByAbdus-0.3/PKG-INFO` & `PyShortsByAbdus-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShortsByAbdus
-Version: 0.3
+Version: 0.4
 Summary: In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 PyShorts is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, PyShorts empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `PyShortsByAbdus-0.3/PyShorts/Sub_Functions/funcs.py` & `PyShortsByAbdus-0.4/PyShorts/Sub_Functions/funcs.py`

 * *Files identical despite different names*

### Comparing `PyShortsByAbdus-0.3/PyShorts/Sub_Functions/non_use_funcs.py` & `PyShortsByAbdus-0.4/PyShorts/Sub_Functions/non_use_funcs.py`

 * *Files identical despite different names*

### Comparing `PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/PKG-INFO` & `PyShortsByAbdus-0.4/PyShortsByAbdus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShortsByAbdus
-Version: 0.3
+Version: 0.4
 Summary: In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 PyShorts is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, PyShorts empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `PyShortsByAbdus-0.3/setup.py` & `PyShortsByAbdus-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Furthermore, PyShorts includes a powerful code generation module, which automates the process of generating boilerplate code. This module allows users to create skeleton code for various frameworks, libraries, and design patterns with just a few simple commands. Whether you're starting a new project or integrating an existing one, PyShorts' code generation module helps you get up and running swiftly, eliminating the need for manual and error-prone boilerplate code creation.
 
 PyShorts also comes equipped with an intelligent code completion feature, providing real-time suggestions and autocompletion for code snippets, functions, and variables. This intelligent assistant analyzes your code as you write, offering helpful suggestions based on context, syntax, and the underlying codebase. This feature saves significant time by reducing the need to look up function signatures or constantly switch between documentation and code files.
 
 With its user-friendly interface and comprehensive documentation, PyShorts ensures a smooth learning curve and seamless integration into existing development workflows. By leveraging PyShorts' powerful functions, snippets, and code generation capabilities, developers can write high-quality code faster, optimize their workflow, and focus on building innovative and robust applications."""
 
-setup(name="PyShortsByAbdus", version="0.3", long_description=Desc, description="In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
+setup(name="PyShortsByAbdus", version="0.4", long_description=Desc, description="In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
 packages=find_packages(),
 install_requires=[
     "Functions",
     "pillow",
     'setuptools',
     'requests'
 ], extra_requires=["twine>=4.0.2", "pytest>=7.0"],
```

