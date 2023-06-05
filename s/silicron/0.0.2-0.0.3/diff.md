# Comparing `tmp/silicron-0.0.2.tar.gz` & `tmp/silicron-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicron-0.0.2.tar", last modified: Fri May 26 07:42:54 2023, max compression
+gzip compressed data, was "silicron-0.0.3.tar", last modified: Mon Jun  5 04:14:12 2023, max compression
```

## Comparing `silicron-0.0.2.tar` & `silicron-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 07:42:54.317426 silicron-0.0.2/
--rw-r--r--   0 michael    (501) staff       (20)      320 2023-05-26 07:42:54.317295 silicron-0.0.2/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1063 2023-05-26 07:37:06.000000 silicron-0.0.2/README.md
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-26 07:42:54.317479 silicron-0.0.2/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      558 2023-05-26 07:41:26.000000 silicron-0.0.2/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 07:42:54.316462 silicron-0.0.2/silicron/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-24 06:45:57.000000 silicron-0.0.2/silicron/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-26 07:42:39.000000 silicron-0.0.2/silicron/api.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 07:42:54.317079 silicron-0.0.2/silicron.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      320 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      183 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 04:14:12.350742 silicron-0.0.3/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-05 04:14:12.350581 silicron-0.0.3/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2094 2023-06-05 03:52:57.000000 silicron-0.0.3/README.md
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-05 04:14:12.350804 silicron-0.0.3/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      530 2023-06-05 04:13:48.000000 silicron-0.0.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 04:14:12.349271 silicron-0.0.3/silicron/
+-rw-r--r--   0 michael    (501) staff       (20)       26 2023-05-26 09:29:50.000000 silicron-0.0.3/silicron/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     7029 2023-06-05 04:11:37.000000 silicron-0.0.3/silicron/api.py
+-rw-r--r--   0 michael    (501) staff       (20)      362 2023-06-05 03:45:00.000000 silicron-0.0.3/silicron/models.py
+-rw-r--r--   0 michael    (501) staff       (20)      837 2023-06-05 03:45:00.000000 silicron-0.0.3/silicron/utils.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 04:14:12.350241 silicron-0.0.3/silicron.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-05 04:14:11.000000 silicron-0.0.3/silicron.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      220 2023-06-05 04:14:12.000000 silicron-0.0.3/silicron.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-05 04:14:11.000000 silicron-0.0.3/silicron.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2023-06-05 04:14:12.000000 silicron-0.0.3/silicron.egg-info/top_level.txt
```

### Comparing `silicron-0.0.2/setup.py` & `silicron-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # Read the content of README file
 with open("silicron/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="silicron",
-    version="0.0.2",
+    version="0.0.3",
     url="https://github.com/michaelliangau",
     author="Michael Liang",
     author_email="michaelliang15@gmail.com",
-    description="Easily extend your chatbot with a knowledge base.",
     packages=find_packages(),
+    description="Give chatbots memory.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
 )
```

