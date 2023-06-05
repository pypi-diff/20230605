# Comparing `tmp/PyShortsByAbdus-0.2.tar.gz` & `tmp/PyShortsByAbdus-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyShortsByAbdus-0.2.tar", last modified: Sun Jun  4 11:14:59 2023, max compression
+gzip compressed data, was "PyShortsByAbdus-0.3.tar", last modified: Mon Jun  5 07:06:31 2023, max compression
```

## Comparing `PyShortsByAbdus-0.2.tar` & `PyShortsByAbdus-0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 11:14:59.542694 PyShortsByAbdus-0.2/
--rw-rw-rw-   0        0        0     3134 2023-06-04 11:14:59.542694 PyShortsByAbdus-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 11:14:59.503705 PyShortsByAbdus-0.2/PyShorts/
--rw-rw-rw-   0        0        0        0 2023-06-04 10:56:21.000000 PyShortsByAbdus-0.2/PyShorts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:14:59.539693 PyShortsByAbdus-0.2/PyShortsByAbdus.egg-info/
--rw-rw-rw-   0        0        0     3134 2023-06-04 11:14:59.000000 PyShortsByAbdus-0.2/PyShortsByAbdus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-06-04 11:14:59.000000 PyShortsByAbdus-0.2/PyShortsByAbdus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 11:14:59.000000 PyShortsByAbdus-0.2/PyShortsByAbdus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-04 11:14:59.000000 PyShortsByAbdus-0.2/PyShortsByAbdus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-04 11:14:59.000000 PyShortsByAbdus-0.2/PyShortsByAbdus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 11:14:59.544704 PyShortsByAbdus-0.2/setup.cfg
--rw-rw-rw-   0        0        0     3351 2023-06-04 11:14:48.000000 PyShortsByAbdus-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.083500 PyShortsByAbdus-0.3/
+-rw-rw-rw-   0        0        0     3134 2023-06-05 07:06:31.080504 PyShortsByAbdus-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.053504 PyShortsByAbdus-0.3/PyShorts/
+drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.077501 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/
+-rw-rw-rw-   0        0        0        0 2023-06-04 14:35:09.000000 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/__init__.py
+-rw-rw-rw-   0        0        0     5351 2023-06-05 07:04:02.000000 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/funcs.py
+-rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 PyShortsByAbdus-0.3/PyShorts/Sub_Functions/non_use_funcs.py
+-rw-rw-rw-   0        0        0      218 2023-06-05 06:49:36.000000 PyShortsByAbdus-0.3/PyShorts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:06:31.068500 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/
+-rw-rw-rw-   0        0        0     3134 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 07:06:30.000000 PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:06:31.084501 PyShortsByAbdus-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3386 2023-06-04 13:40:29.000000 PyShortsByAbdus-0.3/setup.py
```

### Comparing `PyShortsByAbdus-0.2/PKG-INFO` & `PyShortsByAbdus-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShortsByAbdus
-Version: 0.2
+Version: 0.3
 Summary: In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 PyShorts is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, PyShorts empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `PyShortsByAbdus-0.2/PyShortsByAbdus.egg-info/PKG-INFO` & `PyShortsByAbdus-0.3/PyShortsByAbdus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShortsByAbdus
-Version: 0.2
+Version: 0.3
 Summary: In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 PyShorts is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, PyShorts empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `PyShortsByAbdus-0.2/setup.py` & `PyShortsByAbdus-0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 Desc = """PyShorts is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, PyShorts empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
 
 One of the key features of PyShorts is its extensive library of shorthand functions. These functions are carefully crafted to simplify common coding tasks, allowing users to write concise and expressive code with minimal effort. Whether it's performing complex mathematical calculations, manipulating strings, or working with data structures, PyShorts provides intuitive and streamlined functions that significantly speed up the development process.
 
 Additionally, PyShorts offers a collection of code snippets, templates, and shortcuts that can be easily incorporated into your projects. These ready-to-use code snippets cover a wide range of programming scenarios, enabling users to quickly implement common functionalities and algorithms without reinventing the wheel. By leveraging PyShorts' extensive snippet library, developers can focus more on solving higher-level problems rather than getting bogged down by repetitive or time-consuming coding tasks.
 
 Furthermore, PyShorts includes a powerful code generation module, which automates the process of generating boilerplate code. This module allows users to create skeleton code for various frameworks, libraries, and design patterns with just a few simple commands. Whether you're starting a new project or integrating an existing one, PyShorts' code generation module helps you get up and running swiftly, eliminating the need for manual and error-prone boilerplate code creation.
 
 PyShorts also comes equipped with an intelligent code completion feature, providing real-time suggestions and autocompletion for code snippets, functions, and variables. This intelligent assistant analyzes your code as you write, offering helpful suggestions based on context, syntax, and the underlying codebase. This feature saves significant time by reducing the need to look up function signatures or constantly switch between documentation and code files.
 
 With its user-friendly interface and comprehensive documentation, PyShorts ensures a smooth learning curve and seamless integration into existing development workflows. By leveraging PyShorts' powerful functions, snippets, and code generation capabilities, developers can write high-quality code faster, optimize their workflow, and focus on building innovative and robust applications."""
 
-setup(name="PyShortsByAbdus", version="0.2", long_description=Desc, description="In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
-packages=['PyShorts'],
+setup(name="PyShortsByAbdus", version="0.3", long_description=Desc, description="In summary, PyShorts is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, PyShorts streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
+packages=find_packages(),
 install_requires=[
     "Functions",
     "pillow",
-    'setuptools'
+    'setuptools',
+    'requests'
 ], extra_requires=["twine>=4.0.2", "pytest>=7.0"],
 long_description_content_type="text/markdown")
```

