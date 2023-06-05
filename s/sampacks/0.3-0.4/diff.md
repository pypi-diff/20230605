# Comparing `tmp/sampacks-0.3.tar.gz` & `tmp/sampacks-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampacks-0.3.tar", last modified: Mon Jun  5 09:09:50 2023, max compression
+gzip compressed data, was "sampacks-0.4.tar", last modified: Mon Jun  5 12:50:31 2023, max compression
```

## Comparing `sampacks-0.3.tar` & `sampacks-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:09:50.278620 sampacks-0.3/
--rw-rw-rw-   0        0        0     3127 2023-06-05 09:09:50.273607 sampacks-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 09:09:50.255608 sampacks-0.3/sampacks/
--rw-rw-rw-   0        0        0       36 2023-06-05 08:58:05.000000 sampacks-0.3/sampacks/__init__.py
--rw-rw-rw-   0        0        0     5460 2023-06-05 09:09:07.000000 sampacks-0.3/sampacks/funcs.py
--rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 sampacks-0.3/sampacks/non_use_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:09:50.271607 sampacks-0.3/sampacks.egg-info/
--rw-rw-rw-   0        0        0     3127 2023-06-05 09:09:49.000000 sampacks-0.3/sampacks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-05 09:09:50.000000 sampacks-0.3/sampacks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:09:49.000000 sampacks-0.3/sampacks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-05 09:09:49.000000 sampacks-0.3/sampacks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 09:09:49.000000 sampacks-0.3/sampacks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 09:09:50.278620 sampacks-0.3/setup.cfg
--rw-rw-rw-   0        0        0     3379 2023-06-05 07:55:42.000000 sampacks-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:50:31.734717 sampacks-0.4/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 12:50:31.733719 sampacks-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 12:50:31.719718 sampacks-0.4/sampacks/
+-rw-rw-rw-   0        0        0       36 2023-06-05 08:58:05.000000 sampacks-0.4/sampacks/__init__.py
+-rw-rw-rw-   0        0        0     6050 2023-06-05 12:48:35.000000 sampacks-0.4/sampacks/funcs.py
+-rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 sampacks-0.4/sampacks/non_use_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:50:31.730720 sampacks-0.4/sampacks.egg-info/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 12:50:30.000000 sampacks-0.4/sampacks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-05 12:50:30.000000 sampacks-0.4/sampacks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 12:50:30.000000 sampacks-0.4/sampacks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-05 12:50:30.000000 sampacks-0.4/sampacks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 12:50:30.000000 sampacks-0.4/sampacks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 12:50:31.734717 sampacks-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3379 2023-06-05 12:50:08.000000 sampacks-0.4/setup.py
```

### Comparing `sampacks-0.3/PKG-INFO` & `sampacks-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampacks
-Version: 0.3
+Version: 0.4
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `sampacks-0.3/sampacks/funcs.py` & `sampacks-0.4/sampacks/funcs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import os
 import requests
 import random
+import time
+from win10toast import ToastNotifier
 from sampacks.non_use_funcs import (
     image_downloader,
     image_check
 )
 
+# Declarations
+
+toaster = ToastNotifier()
+
 class mainfuncs:
     def __init__(self):
         pass
 
     def coder(self, text):
         """
         Encodes the given text by adding random letters before and after the reversed string.
@@ -159,9 +165,25 @@
                 os.chdir(location)
             except OSError:
                 pass
             with open(name, 'wb') as files:
                 for i in file.iter_content(chunk_size=chunk):
                     files.write(i)
 
+    def reminder(timing, message, title):
+        """
+        Reminds User A Specific Message On Certain Time.
+        Args:
+            timing: Intervals Between Reminder
+            message: Message To Reminded
+            title: Title Of The Reminder
+        Returns:
+            Reminder As Windows Notification.
+        """
+        toaster.show_toast(title, message, duration=timing, threaded=True)
+        while toaster.notification_active:
+            time.sleep(1)
+
+
+
```

### Comparing `sampacks-0.3/sampacks/non_use_funcs.py` & `sampacks-0.4/sampacks/non_use_funcs.py`

 * *Files identical despite different names*

### Comparing `sampacks-0.3/sampacks.egg-info/PKG-INFO` & `sampacks-0.4/sampacks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampacks
-Version: 0.3
+Version: 0.4
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `sampacks-0.3/setup.py` & `sampacks-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Furthermore, Sampacks includes a powerful code generation module, which automates the process of generating boilerplate code. This module allows users to create skeleton code for various frameworks, libraries, and design patterns with just a few simple commands. Whether you're starting a new project or integrating an existing one, Sampacks' code generation module helps you get up and running swiftly, eliminating the need for manual and error-prone boilerplate code creation.
 
 Sampacks also comes equipped with an intelligent code completion feature, providing real-time suggestions and autocompletion for code snippets, functions, and variables. This intelligent assistant analyzes your code as you write, offering helpful suggestions based on context, syntax, and the underlying codebase. This feature saves significant time by reducing the need to look up function signatures or constantly switch between documentation and code files.
 
 With its user-friendly interface and comprehensive documentation, Sampacks ensures a smooth learning curve and seamless integration into existing development workflows. By leveraging Sampacks' powerful functions, snippets, and code generation capabilities, developers can write high-quality code faster, optimize their workflow, and focus on building innovative and robust applications."""
 
-setup(name="sampacks", version="0.3", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
+setup(name="sampacks", version="0.4", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
 packages=find_packages(),
 install_requires=[
     "Functions",
     "pillow",
     'setuptools',
     'requests'
 ], extra_requires=["twine>=4.0.2", "pytest>=7.0"],
```

