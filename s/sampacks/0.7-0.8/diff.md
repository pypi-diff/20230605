# Comparing `tmp/sampacks-0.7.tar.gz` & `tmp/sampacks-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampacks-0.7.tar", last modified: Mon Jun  5 14:48:26 2023, max compression
+gzip compressed data, was "sampacks-0.8.tar", last modified: Mon Jun  5 15:30:02 2023, max compression
```

## Comparing `sampacks-0.7.tar` & `sampacks-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:48:26.726442 sampacks-0.7/
--rw-rw-rw-   0        0        0     3127 2023-06-05 14:48:26.725443 sampacks-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 14:48:26.713447 sampacks-0.7/sampacks/
--rw-rw-rw-   0        0        0       36 2023-06-05 08:58:05.000000 sampacks-0.7/sampacks/__init__.py
--rw-rw-rw-   0        0        0     5972 2023-06-05 14:13:53.000000 sampacks-0.7/sampacks/funcs.py
--rw-rw-rw-   0        0        0     1867 2023-06-05 14:48:08.000000 sampacks-0.7/sampacks/non_use_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:48:26.723443 sampacks-0.7/sampacks.egg-info/
--rw-rw-rw-   0        0        0     3127 2023-06-05 14:48:26.000000 sampacks-0.7/sampacks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-05 14:48:26.000000 sampacks-0.7/sampacks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:48:26.000000 sampacks-0.7/sampacks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-05 14:48:26.000000 sampacks-0.7/sampacks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 14:48:26.000000 sampacks-0.7/sampacks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 14:48:26.727443 sampacks-0.7/setup.cfg
--rw-rw-rw-   0        0        0     3379 2023-06-05 14:48:02.000000 sampacks-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:30:02.091102 sampacks-0.8/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 15:30:02.090101 sampacks-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 15:30:02.050102 sampacks-0.8/sampacks/
+-rw-rw-rw-   0        0        0       36 2023-06-05 08:58:05.000000 sampacks-0.8/sampacks/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-06-05 15:29:55.000000 sampacks-0.8/sampacks/funcs.py
+-rw-rw-rw-   0        0        0     1842 2023-06-05 15:29:51.000000 sampacks-0.8/sampacks/non_use_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:30:02.088102 sampacks-0.8/sampacks.egg-info/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 15:30:01.000000 sampacks-0.8/sampacks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-05 15:30:01.000000 sampacks-0.8/sampacks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:30:01.000000 sampacks-0.8/sampacks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-05 15:30:01.000000 sampacks-0.8/sampacks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 15:30:01.000000 sampacks-0.8/sampacks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:30:02.091102 sampacks-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3379 2023-06-05 14:54:01.000000 sampacks-0.8/setup.py
```

### Comparing `sampacks-0.7/PKG-INFO` & `sampacks-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampacks
-Version: 0.7
+Version: 0.8
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `sampacks-0.7/sampacks/funcs.py` & `sampacks-0.8/sampacks/funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import requests
 import random
 import time
 from win10toast import ToastNotifier
 from sampacks.non_use_funcs import (
     image_downloader,
-    image_check
 )
 
 # Declarations
 
 toaster = ToastNotifier()
 
 class mainfuncs:
@@ -113,28 +112,46 @@
             lowercase_words = [word.lower() for word in words]
             lowercase_text = ' '.join(lowercase_words)
             return lowercase_text
         elif isinstance(obj, list):
             lowercase_words = [word.lower() for word in obj]
             return lowercase_words
         
+    def image_check(self, url):
+        valid_extensions = ('png', 'jpg', 'jpeg', 'webp', 'svg')
+        valid_domains = ('encrypted-tbn0.gstatic.com', 'unsplash', 'pexels', 'image')
+        check = None
+
+        for i in valid_extensions:
+            if url.split('/')[1] != '' and url.split('/')[1].startswith(i):
+                check = True
+            elif url.split('/')[1] != '' and url.split('/')[2].startswith(i):
+                check = True
+            else:
+                check = False
+
+        if any(url.endswith(ext) for ext in valid_extensions) or any(domain in url for domain in valid_domains) or check == True:
+            return True
+        return False
+
     def downloader(self, url, **kwargs):
         """
         Downloads a file from a given url.
         Args:
             url: Url For The File You Wanna Download.
         Kwargs:
             name: Enter The Name Of The File
             chunk: Chunck_Size For Iter_Content
             location: Where To Save The File.
         Returns:
             Downloads: The Files.
+            0.8
         """
 
-        if image_check(url) == True:
+        if mainfuncs.image_check(self, url) == True:
             image_downloader(url, **kwargs)
         else:
             if 'name' in kwargs:
                     name = kwargs['name']     
                     raws = url.split('/')[-1]
                     join = ''.join(raws)
                     if 'extension' in kwargs:
@@ -179,10 +196,7 @@
         Returns:
             Reminder As Windows Notification.
         """
         toaster.show_toast(title, message, duration=timing, threaded=True)
         while toaster.notification_active:
             time.sleep(1)
 
-
-
-
```

### Comparing `sampacks-0.7/sampacks/non_use_funcs.py` & `sampacks-0.8/sampacks/non_use_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,19 +45,18 @@
         for i in request.iter_content(chunk_size=chunk):
             file.write(i)
 
 
 
 def image_check(url):
     valid_extensions = ('png', 'jpg', 'jpeg', 'webp', 'svg')
-    valid_domains = ('encrypted-tbn0.gstatic.com', 'unsplash', 'pexels')
+    valid_domains = ('encrypted-tbn0.gstatic.com', 'unsplash', 'pexels', 'image')
     check = None
 
     for i in valid_extensions:
-        print(url.split('/')[1])
         if url.split('/')[1] != '' and url.split('/')[1].startswith(i):
             check = True
         elif url.split('/')[1] != '' and url.split('/')[2].startswith(i):
             check = True
         else:
             check = False
```

### Comparing `sampacks-0.7/sampacks.egg-info/PKG-INFO` & `sampacks-0.8/sampacks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampacks
-Version: 0.7
+Version: 0.8
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `sampacks-0.7/setup.py` & `sampacks-0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Furthermore, Sampacks includes a powerful code generation module, which automates the process of generating boilerplate code. This module allows users to create skeleton code for various frameworks, libraries, and design patterns with just a few simple commands. Whether you're starting a new project or integrating an existing one, Sampacks' code generation module helps you get up and running swiftly, eliminating the need for manual and error-prone boilerplate code creation.
 
 Sampacks also comes equipped with an intelligent code completion feature, providing real-time suggestions and autocompletion for code snippets, functions, and variables. This intelligent assistant analyzes your code as you write, offering helpful suggestions based on context, syntax, and the underlying codebase. This feature saves significant time by reducing the need to look up function signatures or constantly switch between documentation and code files.
 
 With its user-friendly interface and comprehensive documentation, Sampacks ensures a smooth learning curve and seamless integration into existing development workflows. By leveraging Sampacks' powerful functions, snippets, and code generation capabilities, developers can write high-quality code faster, optimize their workflow, and focus on building innovative and robust applications."""
 
-setup(name="sampacks", version="0.7", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
+setup(name="sampacks", version="0.8", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
 packages=find_packages(),
 install_requires=[
     "Functions",
     "pillow",
     'setuptools',
     'requests'
 ], extra_requires=["twine>=4.0.2", "pytest>=7.0"],
```

