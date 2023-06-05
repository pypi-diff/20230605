# Comparing `tmp/sampacks-0.5.tar.gz` & `tmp/sampacks-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampacks-0.5.tar", last modified: Mon Jun  5 13:02:20 2023, max compression
+gzip compressed data, was "sampacks-0.6.tar", last modified: Mon Jun  5 14:14:59 2023, max compression
```

## Comparing `sampacks-0.5.tar` & `sampacks-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:02:20.157434 sampacks-0.5/
--rw-rw-rw-   0        0        0     3127 2023-06-05 13:02:20.137435 sampacks-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 13:02:20.121439 sampacks-0.5/sampacks/
--rw-rw-rw-   0        0        0       36 2023-06-05 08:58:05.000000 sampacks-0.5/sampacks/__init__.py
--rw-rw-rw-   0        0        0     6050 2023-06-05 12:48:35.000000 sampacks-0.5/sampacks/funcs.py
--rw-rw-rw-   0        0        0     1399 2023-06-05 07:03:26.000000 sampacks-0.5/sampacks/non_use_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:02:20.136439 sampacks-0.5/sampacks.egg-info/
--rw-rw-rw-   0        0        0     3127 2023-06-05 13:02:19.000000 sampacks-0.5/sampacks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-05 13:02:20.000000 sampacks-0.5/sampacks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:02:19.000000 sampacks-0.5/sampacks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-05 13:02:19.000000 sampacks-0.5/sampacks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 13:02:19.000000 sampacks-0.5/sampacks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 13:02:20.157434 sampacks-0.5/setup.cfg
--rw-rw-rw-   0        0        0     3379 2023-06-05 13:02:16.000000 sampacks-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:14:59.254466 sampacks-0.6/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 14:14:59.249456 sampacks-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 14:14:59.047461 sampacks-0.6/sampacks/
+-rw-rw-rw-   0        0        0       36 2023-06-05 08:58:05.000000 sampacks-0.6/sampacks/__init__.py
+-rw-rw-rw-   0        0        0     5972 2023-06-05 14:13:53.000000 sampacks-0.6/sampacks/funcs.py
+-rw-rw-rw-   0        0        0     1522 2023-06-05 14:13:12.000000 sampacks-0.6/sampacks/non_use_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:14:59.247458 sampacks-0.6/sampacks.egg-info/
+-rw-rw-rw-   0        0        0     3127 2023-06-05 14:14:58.000000 sampacks-0.6/sampacks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-05 14:14:58.000000 sampacks-0.6/sampacks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:14:58.000000 sampacks-0.6/sampacks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-05 14:14:58.000000 sampacks-0.6/sampacks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 14:14:58.000000 sampacks-0.6/sampacks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 14:14:59.254466 sampacks-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3379 2023-06-05 14:14:38.000000 sampacks-0.6/setup.py
```

### Comparing `sampacks-0.5/PKG-INFO` & `sampacks-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampacks
-Version: 0.5
+Version: 0.6
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `sampacks-0.5/sampacks/funcs.py` & `sampacks-0.6/sampacks/funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,18 +125,17 @@
         Kwargs:
             name: Enter The Name Of The File
             chunk: Chunck_Size For Iter_Content
             location: Where To Save The File.
         Returns:
             Downloads: The Files.
         """
-        img = image_check(url)
-        if type(img) == list:
-            image_extension = img[1]
-            image_downloader(url, image_extension, **kwargs)
+
+        if image_check(url) == True:
+            image_downloader(url, **kwargs)
         else:
             if 'name' in kwargs:
                     name = kwargs['name']     
                     raws = url.split('/')[-1]
                     join = ''.join(raws)
                     if 'extension' in kwargs:
                         name = name + kwargs['extension']
@@ -165,14 +164,15 @@
                 os.chdir(location)
             except OSError:
                 pass
             with open(name, 'wb') as files:
                 for i in file.iter_content(chunk_size=chunk):
                     files.write(i)
 
+
     def reminder(timing, message, title):
         """
         Reminds User A Specific Message On Certain Time.
         Args:
             timing: Intervals Between Reminder
             message: Message To Reminded
             title: Title Of The Reminder
@@ -182,8 +182,7 @@
         toaster.show_toast(title, message, duration=timing, threaded=True)
         while toaster.notification_active:
             time.sleep(1)
 
 
 
 
-
```

### Comparing `sampacks-0.5/sampacks/non_use_funcs.py` & `sampacks-0.6/sampacks/non_use_funcs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # Sub_Funcs 
 import os
 import requests
 
-def image_downloader(url, extension, **kwargs):
+def image_downloader(url, **kwargs):
     """
         Downloads a file from a given url.
         Args:
             url: Url For The File You Wanna Download.
         Kwargs:
             name: Enter The Name Of The Image.
             chunk: Chunck_Size For Iter_Content.
             location: Where To Save The Image.
         Returns:
             The Downloaded Image
     """
+    if 'extension' in kwargs:
+        extension = kwargs['extension']
+        if extension.startswith('.'):
+            extension = extension.replace('.', '')
+    else:
+        extension = '.png'
 
     if 'name' in kwargs:
         name = kwargs['name'] + extension
     else:
-        name = 'default.png' 
+        name = 'default' + extension 
     
     if 'chunk' in kwargs:
         chunk = kwargs['chunk']
     else:
         chunk = 500
 
     if 'location' in kwargs:
@@ -31,22 +37,21 @@
         location = ''
 
     try:
         os.chdir(location)
     except OSError:
         pass
     request = requests.get(url, stream=True)
-    with open(name, 'wb') as file:
+    with open(f"{name}", 'wb') as file:
         for i in request.iter_content(chunk_size=chunk):
             file.write(i)
 
 
+
 def image_check(url):
-    if url.split('/')[2] == 'encrypted-tbn0.gstatic.com' or url.endswith('.png') or ''.join(url.split('/')[1]).startswith('png'): 
-        extension = '.png'
-        return [True, extension]
-    elif url.endswith('.jpg') or ''.join(url.split('/')[1]).startswith('jpg'): 
-        extension = '.jpg'
-        return [True, extension]
-    else:
-        return False
+    valid_extensions = ('png', 'jpg', 'jpeg', 'webp', 'svg')
+    valid_domains = ('encrypted-tbn0.gstatic.com', 'unsplash', 'pexels')
+
+    if any(url.endswith(ext) for ext in valid_extensions) or any(domain in url for domain in valid_domains):
+        return True
+    return False
```

### Comparing `sampacks-0.5/sampacks.egg-info/PKG-INFO` & `sampacks-0.6/sampacks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampacks
-Version: 0.5
+Version: 0.6
 Summary: In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.
 Author: Abdus-Samad
 Author-email: Samadgame0910@gmail.com
 Description-Content-Type: text/markdown
 
 Sampacks is a dynamic Python package designed to enhance the coding experience and boost productivity for developers. With a range of efficient functions and utilities, Sampacks empowers users to write code rapidly and efficiently, reducing development time and increasing overall efficiency.
```

### Comparing `sampacks-0.5/setup.py` & `sampacks-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Furthermore, Sampacks includes a powerful code generation module, which automates the process of generating boilerplate code. This module allows users to create skeleton code for various frameworks, libraries, and design patterns with just a few simple commands. Whether you're starting a new project or integrating an existing one, Sampacks' code generation module helps you get up and running swiftly, eliminating the need for manual and error-prone boilerplate code creation.
 
 Sampacks also comes equipped with an intelligent code completion feature, providing real-time suggestions and autocompletion for code snippets, functions, and variables. This intelligent assistant analyzes your code as you write, offering helpful suggestions based on context, syntax, and the underlying codebase. This feature saves significant time by reducing the need to look up function signatures or constantly switch between documentation and code files.
 
 With its user-friendly interface and comprehensive documentation, Sampacks ensures a smooth learning curve and seamless integration into existing development workflows. By leveraging Sampacks' powerful functions, snippets, and code generation capabilities, developers can write high-quality code faster, optimize their workflow, and focus on building innovative and robust applications."""
 
-setup(name="sampacks", version="0.5", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
+setup(name="sampacks", version="0.6", long_description=Desc, description="In summary, Sampacks is a game-changing Python package that empowers developers to write code swiftly and efficiently. By providing shorthand functions, code snippets, intelligent code completion, and code generation capabilities, Sampacks streamlines the coding process, enabling developers to accelerate their productivity and deliver high-quality code with ease.", author="Abdus-Samad", author_email="Samadgame0910@gmail.com",
 packages=find_packages(),
 install_requires=[
     "Functions",
     "pillow",
     'setuptools',
     'requests'
 ], extra_requires=["twine>=4.0.2", "pytest>=7.0"],
```

