# Comparing `tmp/roboduck-0.4.2.tar.gz` & `tmp/roboduck-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboduck-0.4.2.tar", last modified: Mon Jun  5 00:00:22 2023, max compression
+gzip compressed data, was "roboduck-0.5.0.tar", last modified: Mon Jun  5 00:25:22 2023, max compression
```

## Comparing `roboduck-0.4.2.tar` & `roboduck-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:00:22.015594 roboduck-0.4.2/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.4.2/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)    12895 2023-06-05 00:00:22.015085 roboduck-0.4.2/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)    12450 2023-06-04 23:59:53.000000 roboduck-0.4.2/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.4.2/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:00:22.001391 roboduck-0.4.2/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-06-05 00:00:07.000000 roboduck-0.4.2/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:00:22.005979 roboduck-0.4.2/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.4.2/roboduck/cli/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     3412 2023-05-28 04:07:25.000000 roboduck-0.4.2/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.4.2/roboduck/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    22975 2023-05-31 07:15:56.000000 roboduck-0.4.2/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10858 2023-05-29 22:16:38.000000 roboduck-0.4.2/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)    11439 2023-05-29 23:13:09.000000 roboduck-0.4.2/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.4.2/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:00:22.007699 roboduck-0.4.2/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.4.2/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.4.2/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.4.2/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.4.2/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6333 2023-05-29 23:12:35.000000 roboduck-0.4.2/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5183 2023-05-31 05:27:53.000000 roboduck-0.4.2/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:00:22.008465 roboduck-0.4.2/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.4.2/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:00:22.014117 roboduck-0.4.2/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.4.2/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.4.2/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.4.2/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.4.2/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.4.2/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-28 03:58:55.000000 roboduck-0.4.2/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)    15138 2023-05-28 04:07:13.000000 roboduck-0.4.2/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:00:22.005125 roboduck-0.4.2/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)    12895 2023-06-05 00:00:21.000000 roboduck-0.4.2/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      843 2023-06-05 00:00:21.000000 roboduck-0.4.2/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-06-05 00:00:21.000000 roboduck-0.4.2/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-06-05 00:00:21.000000 roboduck-0.4.2/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-06-05 00:00:21.000000 roboduck-0.4.2/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-06-05 00:00:21.000000 roboduck-0.4.2/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-06-05 00:00:22.015733 roboduck-0.4.2/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)     1656 2023-06-04 04:37:00.000000 roboduck-0.4.2/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.981409 roboduck-0.5.0/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.5.0/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)    12999 2023-06-05 00:25:22.981059 roboduck-0.5.0/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)    12531 2023-06-05 00:24:46.000000 roboduck-0.5.0/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.5.0/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.972094 roboduck-0.5.0/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-06-05 00:21:58.000000 roboduck-0.5.0/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.975451 roboduck-0.5.0/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.5.0/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     3412 2023-05-28 04:07:25.000000 roboduck-0.5.0/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.5.0/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    22975 2023-05-31 07:15:56.000000 roboduck-0.5.0/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10858 2023-05-29 22:16:38.000000 roboduck-0.5.0/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11439 2023-05-29 23:13:09.000000 roboduck-0.5.0/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.5.0/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.977151 roboduck-0.5.0/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.5.0/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.5.0/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.5.0/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.5.0/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6333 2023-05-29 23:12:35.000000 roboduck-0.5.0/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5183 2023-05-31 05:27:53.000000 roboduck-0.5.0/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.978175 roboduck-0.5.0/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.5.0/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.980599 roboduck-0.5.0/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.5.0/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.5.0/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.5.0/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.5.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.5.0/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-28 03:58:55.000000 roboduck-0.5.0/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    15138 2023-05-28 04:07:13.000000 roboduck-0.5.0/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.974708 roboduck-0.5.0/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)    12999 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      843 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-06-05 00:25:22.981500 roboduck-0.5.0/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)     1685 2023-06-05 00:21:18.000000 roboduck-0.5.0/setup.py
```

### Comparing `roboduck-0.4.2/PKG-INFO` & `roboduck-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.4.2
+Version: 0.5.0
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://hdmamin.github.io/roboduck/
 Project-URL: Repository, https://github.com/hdmamin/roboduck
 Keywords: debugging,llm,language model,dev tools,errors,jupyter magic,gpt,openai,langchain
 Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/hdmamin/roboduck/main/data/images/roboduck_blue_banner.png" alt="roboduck logo">
 <p></p>
 <a href="https://hdmamin.github.io/roboduck/"><img src="https://img.shields.io/badge/Documentation-Online-blue.svg" alt="Documentation"></a>
 <a href="https://badge.fury.io/py/roboduck"><img src="https://badge.fury.io/py/roboduck.svg" alt="PyPI version"></a>
 <a href="https://github.com/hdmamin/roboduck/actions/workflows/main.yml"><img src="https://github.com/hdmamin/roboduck/actions/workflows/main.yml/badge.svg" alt="Build Status"></a>
 <a href="https://colab.research.google.com/github/hdmamin/roboduck/blob/main/notebooks/quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"></a>
+<img alt="Python Version" src="https://img.shields.io/badge/python-3.8%2B-blue">
 <p></p>
 </div>
 
 **rubber duck debugging**: a method of debugging code by articulating a problem in spoken or written natural language. The name is a reference to a story in the book The Pragmatic Programmer in which a programmer would carry around a rubber duck and debug their code by forcing themselves to explain it, line-by-line, to the duck. [[1](https://en.wikipedia.org/wiki/Rubber_duck_debugging)]
 
 **robo duck debugging**: a bit like rubber duck debugging, but the duck talks back.
```

### Comparing `roboduck-0.4.2/README.md` & `roboduck-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <div align="center">
 <img src="https://raw.githubusercontent.com/hdmamin/roboduck/main/data/images/roboduck_blue_banner.png" alt="roboduck logo">
 <p></p>
 <a href="https://hdmamin.github.io/roboduck/"><img src="https://img.shields.io/badge/Documentation-Online-blue.svg" alt="Documentation"></a>
 <a href="https://badge.fury.io/py/roboduck"><img src="https://badge.fury.io/py/roboduck.svg" alt="PyPI version"></a>
 <a href="https://github.com/hdmamin/roboduck/actions/workflows/main.yml"><img src="https://github.com/hdmamin/roboduck/actions/workflows/main.yml/badge.svg" alt="Build Status"></a>
 <a href="https://colab.research.google.com/github/hdmamin/roboduck/blob/main/notebooks/quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"></a>
+<img alt="Python Version" src="https://img.shields.io/badge/python-3.8%2B-blue">
 <p></p>
 </div>
 
 **rubber duck debugging**: a method of debugging code by articulating a problem in spoken or written natural language. The name is a reference to a story in the book The Pragmatic Programmer in which a programmer would carry around a rubber duck and debug their code by forcing themselves to explain it, line-by-line, to the duck. [[1](https://en.wikipedia.org/wiki/Rubber_duck_debugging)]
 
 **robo duck debugging**: a bit like rubber duck debugging, but the duck talks back.
```

### Comparing `roboduck-0.4.2/roboduck/__init__.py` & `roboduck-0.5.0/roboduck/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from roboduck.debug import duck, DuckDB, CodeCompletionCache
 from roboduck.langchain.chat import Chat, DummyChatModel
 from roboduck.config import update_config, load_config, set_openai_api_key
 from roboduck.ipy_utils import is_colab
 from roboduck.utils import available_models
 
 
-__version__ = '0.4.2'
+__version__ = '0.5.0'
 set_openai_api_key()
 if is_colab():
     warnings.warn(
         'It looks like you\'re using Google Colab, which may make your '
         'roboduck experience slightly sub-optimal (e.g. typing can be a bit '
         'laggy).'
     )
```

### Comparing `roboduck-0.4.2/roboduck/cli/cli.py` & `roboduck-0.5.0/roboduck/cli/cli.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/config.py` & `roboduck-0.5.0/roboduck/config.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/debug.py` & `roboduck-0.5.0/roboduck/debug.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/decorators.py` & `roboduck-0.5.0/roboduck/decorators.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/errors.py` & `roboduck-0.5.0/roboduck/errors.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/ipy_utils.py` & `roboduck-0.5.0/roboduck/ipy_utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/langchain/callbacks.py` & `roboduck-0.5.0/roboduck/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/langchain/chat.py` & `roboduck-0.5.0/roboduck/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/langchain/utils.py` & `roboduck-0.5.0/roboduck/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/logging.py` & `roboduck-0.5.0/roboduck/logging.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/magic.py` & `roboduck-0.5.0/roboduck/magic.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.5.0/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/prompts/chat/debug.yaml` & `roboduck-0.5.0/roboduck/prompts/chat/debug.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.5.0/roboduck/prompts/chat/debug_full.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.5.0/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.5.0/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/prompts/utils.py` & `roboduck-0.5.0/roboduck/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck/utils.py` & `roboduck-0.5.0/roboduck/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/roboduck.egg-info/PKG-INFO` & `roboduck-0.5.0/roboduck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.4.2
+Version: 0.5.0
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://hdmamin.github.io/roboduck/
 Project-URL: Repository, https://github.com/hdmamin/roboduck
 Keywords: debugging,llm,language model,dev tools,errors,jupyter magic,gpt,openai,langchain
 Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/hdmamin/roboduck/main/data/images/roboduck_blue_banner.png" alt="roboduck logo">
 <p></p>
 <a href="https://hdmamin.github.io/roboduck/"><img src="https://img.shields.io/badge/Documentation-Online-blue.svg" alt="Documentation"></a>
 <a href="https://badge.fury.io/py/roboduck"><img src="https://badge.fury.io/py/roboduck.svg" alt="PyPI version"></a>
 <a href="https://github.com/hdmamin/roboduck/actions/workflows/main.yml"><img src="https://github.com/hdmamin/roboduck/actions/workflows/main.yml/badge.svg" alt="Build Status"></a>
 <a href="https://colab.research.google.com/github/hdmamin/roboduck/blob/main/notebooks/quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"></a>
+<img alt="Python Version" src="https://img.shields.io/badge/python-3.8%2B-blue">
 <p></p>
 </div>
 
 **rubber duck debugging**: a method of debugging code by articulating a problem in spoken or written natural language. The name is a reference to a story in the book The Pragmatic Programmer in which a programmer would carry around a rubber duck and debug their code by forcing themselves to explain it, line-by-line, to the duck. [[1](https://en.wikipedia.org/wiki/Rubber_duck_debugging)]
 
 **robo duck debugging**: a bit like rubber duck debugging, but the duck talks back.
```

### Comparing `roboduck-0.4.2/roboduck.egg-info/SOURCES.txt` & `roboduck-0.5.0/roboduck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.2/setup.py` & `roboduck-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     with open(path, 'r') as f:
         return f.read()
 
 
 setuptools.setup(
     name='roboduck',
     version=version(),
+    python_requires='>=3.8',
     author='Harrison Mamin',
     author_email='harrisonmamin@gmail.com',
     description='A natural language debugger.',
     long_description=load_file('README.md'),
     long_description_content_type='text/markdown',
     install_requires=requirements(),
     packages=setuptools.find_packages(),
```

