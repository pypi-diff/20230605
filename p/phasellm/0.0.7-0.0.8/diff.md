# Comparing `tmp/phasellm-0.0.7.tar.gz` & `tmp/phasellm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.7.tar", last modified: Sun May 28 04:11:42 2023, max compression
+gzip compressed data, was "phasellm-0.0.8.tar", last modified: Mon Jun  5 00:28:05 2023, max compression
```

## Comparing `phasellm-0.0.7.tar` & `phasellm-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-28 04:11:42.374458 phasellm-0.0.7/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-05-23 17:50:05.000000 phasellm-0.0.7/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-28 04:11:42.374458 phasellm-0.0.7/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4999 2023-05-23 17:50:05.000000 phasellm-0.0.7/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-28 04:11:42.374458 phasellm-0.0.7/phasellm/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      653 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5152 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/agents.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4802 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/eval.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4372 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/exceptions.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    17411 2023-05-28 02:53:32.000000 phasellm-0.0.7/phasellm/llms.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-28 04:11:42.374458 phasellm-0.0.7/phasellm.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      282 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      126 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-05-28 04:11:42.374458 phasellm-0.0.7/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1167 2023-05-28 02:47:44.000000 phasellm-0.0.7/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 00:28:05.722988 phasellm-0.0.8/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-06-02 18:12:47.000000 phasellm-0.0.8/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-06-05 00:28:05.722988 phasellm-0.0.8/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4999 2023-06-02 18:12:47.000000 phasellm-0.0.8/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 00:28:05.722988 phasellm-0.0.8/phasellm/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      653 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5152 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/agents.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4802 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/eval.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4372 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/exceptions.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3044 2023-06-02 23:00:21.000000 phasellm-0.0.8/phasellm/html.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    17831 2023-06-02 18:38:12.000000 phasellm-0.0.8/phasellm/llms.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 00:28:05.722988 phasellm-0.0.8/phasellm.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      299 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      126 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-06-05 00:28:05.722988 phasellm-0.0.8/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1167 2023-06-02 18:18:06.000000 phasellm-0.0.8/setup.py
```

### Comparing `phasellm-0.0.7/LICENSE` & `phasellm-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.7/PKG-INFO` & `phasellm-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.7/README.md` & `phasellm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.7/phasellm/__init__.py` & `phasellm-0.0.8/phasellm/__init__.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.7/phasellm/agents.py` & `phasellm-0.0.8/phasellm/agents.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.7/phasellm/eval.py` & `phasellm-0.0.8/phasellm/eval.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.7/phasellm/exceptions.py` & `phasellm-0.0.8/phasellm/exceptions.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.7/phasellm/llms.py` & `phasellm-0.0.8/phasellm/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Abstract classes and wrappers for LLMs, chatbots, and prompts.
 """
 
 import requests
 import json
 import re
+import time 
+from datetime import datetime 
 
 # Imports for external APIs
 import openai
 import cohere
 
 # Hugging Face and PyTorch imports
 from transformers import pipeline
@@ -470,19 +472,29 @@
         
         Warning: not all LLMs are trained to use instructions provided in a system prompt.
         """
         self.llm = llm 
         self.messages = []
         self._append_message('system', initial_system_prompt)
 
-    def _append_message(self, role, message):
+    def _append_message(self, role, message, log_time_seconds=None):
         """
         Saves a message to the chatbot's message queue.
         """
-        self.messages.append({"role":role, "content":message})
+
+        append_me = {"role":role, "content":message}
+
+        # Adding time stamps
+        append_me["timestamp_utc"] = datetime.now()
+        
+        # Save how long it took to run the query.
+        if log_time_seconds is not None:
+            append_me["log_time_seconds"] = log_time_seconds
+
+        self.messages.append(append_me)
 
     def resend(self):
         """
         If the last message in the messages stack (i.e. array of role and content pairs) is from the user, it will resend the message and return the response. It's similar to erasing the last message in the stack and resending the last user message to the chat model.
 
         This is useful if a model has errored out or if you are building a broader messages stack outside of the actual chatbot.
         """
@@ -496,11 +508,12 @@
             return None 
 
     def chat(self, message):
         """
         Chats with the chatbot.
         """
         self._append_message('user', message)
+        start_time = time.time()
         response = self.llm.complete_chat(self.messages, "assistant")
-        self._append_message('assistant', response)
+        self._append_message('assistant', response, log_time_seconds = time.time() - start_time)
         return response
```

### Comparing `phasellm-0.0.7/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.8/phasellm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.7/setup.py` & `phasellm-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 DESCRIPTION = "Wrappers for common large langugae models (LLMs) with support for evaluation."
 
 LONG_DESCRIPTION = "PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use."
 
 setup(
     name="phasellm",
```

