# Comparing `tmp/notebook_copilot-0.1.tar.gz` & `tmp/notebook_copilot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_copilot-0.1.tar", last modified: Sun Jun  4 02:45:28 2023, max compression
+gzip compressed data, was "notebook_copilot-0.1.2.tar", last modified: Sun Jun  4 23:29:14 2023, max compression
```

## Comparing `notebook_copilot-0.1.tar` & `notebook_copilot-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 02:45:28.173856 notebook_copilot-0.1/
--rw-r--r--   0 tp         (501) staff       (20)     2954 2023-06-04 02:45:28.173735 notebook_copilot-0.1/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)     2668 2023-06-04 02:45:11.000000 notebook_copilot-0.1/README.md
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 02:45:28.172774 notebook_copilot-0.1/notebook_copilot/
--rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.1/notebook_copilot/__init__.py
--rw-r--r--   0 tp         (501) staff       (20)     1678 2023-06-03 00:21:02.000000 notebook_copilot-0.1/notebook_copilot/agents.py
--rw-r--r--   0 tp         (501) staff       (20)     1300 2023-06-03 23:50:52.000000 notebook_copilot-0.1/notebook_copilot/chains.py
--rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.1/notebook_copilot/context.py
--rw-r--r--   0 tp         (501) staff       (20)     4554 2023-06-03 23:28:59.000000 notebook_copilot-0.1/notebook_copilot/notebook_copilot.py
--rw-r--r--   0 tp         (501) staff       (20)     2469 2023-06-03 23:53:58.000000 notebook_copilot-0.1/notebook_copilot/output.py
--rw-r--r--   0 tp         (501) staff       (20)     2775 2023-06-03 23:49:21.000000 notebook_copilot-0.1/notebook_copilot/prompts.py
--rw-r--r--   0 tp         (501) staff       (20)     2430 2023-06-03 23:30:56.000000 notebook_copilot-0.1/notebook_copilot/tools.py
--rw-r--r--   0 tp         (501) staff       (20)      316 2023-06-01 20:58:10.000000 notebook_copilot-0.1/notebook_copilot/utils.py
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 02:45:28.173539 notebook_copilot-0.1/notebook_copilot.egg-info/
--rw-r--r--   0 tp         (501) staff       (20)     2954 2023-06-04 02:45:28.000000 notebook_copilot-0.1/notebook_copilot.egg-info/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)      472 2023-06-04 02:45:28.000000 notebook_copilot-0.1/notebook_copilot.egg-info/SOURCES.txt
--rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-04 02:45:28.000000 notebook_copilot-0.1/notebook_copilot.egg-info/dependency_links.txt
--rw-r--r--   0 tp         (501) staff       (20)       25 2023-06-04 02:45:28.000000 notebook_copilot-0.1/notebook_copilot.egg-info/requires.txt
--rw-r--r--   0 tp         (501) staff       (20)       17 2023-06-04 02:45:28.000000 notebook_copilot-0.1/notebook_copilot.egg-info/top_level.txt
--rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-04 02:45:28.173893 notebook_copilot-0.1/setup.cfg
--rw-r--r--   0 tp         (501) staff       (20)      531 2023-06-04 02:19:07.000000 notebook_copilot-0.1/setup.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 23:29:14.648773 notebook_copilot-0.1.2/
+-rw-r--r--   0 tp         (501) staff       (20)     2947 2023-06-04 23:29:14.648656 notebook_copilot-0.1.2/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)     2668 2023-06-04 02:45:11.000000 notebook_copilot-0.1.2/README.md
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 23:29:14.647812 notebook_copilot-0.1.2/notebook_copilot/
+-rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.1.2/notebook_copilot/__init__.py
+-rw-r--r--   0 tp         (501) staff       (20)     1678 2023-06-03 00:21:02.000000 notebook_copilot-0.1.2/notebook_copilot/agents.py
+-rw-r--r--   0 tp         (501) staff       (20)     1300 2023-06-03 23:50:52.000000 notebook_copilot-0.1.2/notebook_copilot/chains.py
+-rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.1.2/notebook_copilot/context.py
+-rw-r--r--   0 tp         (501) staff       (20)     4554 2023-06-03 23:28:59.000000 notebook_copilot-0.1.2/notebook_copilot/notebook_copilot.py
+-rw-r--r--   0 tp         (501) staff       (20)     2469 2023-06-03 23:53:58.000000 notebook_copilot-0.1.2/notebook_copilot/output.py
+-rw-r--r--   0 tp         (501) staff       (20)     2775 2023-06-03 23:49:21.000000 notebook_copilot-0.1.2/notebook_copilot/prompts.py
+-rw-r--r--   0 tp         (501) staff       (20)     2430 2023-06-03 23:30:56.000000 notebook_copilot-0.1.2/notebook_copilot/tools.py
+-rw-r--r--   0 tp         (501) staff       (20)      316 2023-06-01 20:58:10.000000 notebook_copilot-0.1.2/notebook_copilot/utils.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 23:29:14.648491 notebook_copilot-0.1.2/notebook_copilot.egg-info/
+-rw-r--r--   0 tp         (501) staff       (20)     2947 2023-06-04 23:29:14.000000 notebook_copilot-0.1.2/notebook_copilot.egg-info/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)      472 2023-06-04 23:29:14.000000 notebook_copilot-0.1.2/notebook_copilot.egg-info/SOURCES.txt
+-rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-04 23:29:14.000000 notebook_copilot-0.1.2/notebook_copilot.egg-info/dependency_links.txt
+-rw-r--r--   0 tp         (501) staff       (20)       85 2023-06-04 23:29:14.000000 notebook_copilot-0.1.2/notebook_copilot.egg-info/requires.txt
+-rw-r--r--   0 tp         (501) staff       (20)       17 2023-06-04 23:29:14.000000 notebook_copilot-0.1.2/notebook_copilot.egg-info/top_level.txt
+-rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-04 23:29:14.648811 notebook_copilot-0.1.2/setup.cfg
+-rw-r--r--   0 tp         (501) staff       (20)      606 2023-06-04 23:29:11.000000 notebook_copilot-0.1.2/setup.py
```

### Comparing `notebook_copilot-0.1/PKG-INFO` & `notebook_copilot-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: notebook_copilot
-Version: 0.1
-Summary: A magic command for using OpenAI in Jupyter notebooks.
+Version: 0.1.2
+Summary: The Bridge from Thoughts to Well-Crafted Code
 Home-page: https://github.com/talperetz/notebook_copilot
 Author: Tal Peretz
 Author-email: tp@aihumanlabs.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # 🚀 Notebook Copilot: Your AI Guide Through the Jupyter Universe
```

### Comparing `notebook_copilot-0.1/README.md` & `notebook_copilot-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot/agents.py` & `notebook_copilot-0.1.2/notebook_copilot/agents.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot/chains.py` & `notebook_copilot-0.1.2/notebook_copilot/chains.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot/context.py` & `notebook_copilot-0.1.2/notebook_copilot/context.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot/notebook_copilot.py` & `notebook_copilot-0.1.2/notebook_copilot/notebook_copilot.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot/output.py` & `notebook_copilot-0.1.2/notebook_copilot/output.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot/prompts.py` & `notebook_copilot-0.1.2/notebook_copilot/prompts.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot/tools.py` & `notebook_copilot-0.1.2/notebook_copilot/tools.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1/notebook_copilot.egg-info/PKG-INFO` & `notebook_copilot-0.1.2/notebook_copilot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: notebook-copilot
-Version: 0.1
-Summary: A magic command for using OpenAI in Jupyter notebooks.
+Version: 0.1.2
+Summary: The Bridge from Thoughts to Well-Crafted Code
 Home-page: https://github.com/talperetz/notebook_copilot
 Author: Tal Peretz
 Author-email: tp@aihumanlabs.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # 🚀 Notebook Copilot: Your AI Guide Through the Jupyter Universe
```

