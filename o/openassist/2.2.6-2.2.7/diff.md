# Comparing `tmp/openassist-2.2.6.tar.gz` & `tmp/openassist-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openassist-2.2.6.tar", max compression
+gzip compressed data, was "openassist-2.2.7.tar", max compression
```

## Comparing `openassist-2.2.6.tar` & `openassist-2.2.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1087 2023-06-04 14:20:56.512929 openassist-2.2.6/LICENSE
--rw-r--r--   0        0        0      539 2023-06-04 15:16:43.084255 openassist-2.2.6/pyproject.toml
--rw-r--r--   0        0        0     3074 2023-06-04 15:16:40.670420 openassist-2.2.6/README.md
--rw-r--r--   0        0        0       55 2023-06-04 14:23:45.664873 openassist-2.2.6/src/openassist/__init__.py
--rw-r--r--   0        0        0    20110 2023-06-04 14:22:10.572141 openassist-2.2.6/src/openassist/openassist.py
--rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 openassist-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-04 14:20:56.512929 openassist-2.2.7/LICENSE
+-rw-r--r--   0        0        0      539 2023-06-05 14:17:10.440049 openassist-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3220 2023-06-05 14:18:45.803557 openassist-2.2.7/README.md
+-rw-r--r--   0        0        0       55 2023-06-04 14:23:45.664873 openassist-2.2.7/src/openassist/__init__.py
+-rw-r--r--   0        0        0    20208 2023-06-05 14:18:58.155273 openassist-2.2.7/src/openassist/openassist.py
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 openassist-2.2.7/PKG-INFO
```

### Comparing `openassist-2.2.6/LICENSE` & `openassist-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openassist-2.2.6/pyproject.toml` & `openassist-2.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openassist"
-version = "2.2.6"
+version = "2.2.7"
 description = "OpenAssist is a module for Python that allows you to create an AI assistant using import openai with ease."
 authors = ["Free Zoloft <mybusinessemaildbb@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["README.md"]
 
 [tool.poetry.dependencies]
```

### Comparing `openassist-2.2.6/README.md` & `openassist-2.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,8 +64,15 @@
     insert(index, dictionary) - Insert a dictionary into the memory list at the specified index
     clear() - Clear the memory list
     view_list() - View the memory list
     return_list() - Return the memory list
     edit(dictionary, index) - Edit a dictionary in the memory list at the specified index
     get_index(dictionary) - Get the index of a dictionary in the memory list
 """
+```
+
+## Dev Log:
+
+```python
+# 2.2.6 - Initial Release
+# 2.2.7 - Added max_tokens parameter to chat_completion() and completion() functions
 ```
```

### Comparing `openassist-2.2.6/src/openassist/openassist.py` & `openassist-2.2.7/src/openassist/openassist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OpenAssist v2.2 - FZ#2023
+# OpenAssist v2.2.7 - FZ#2023
 # OpenAssist is a module for Python that allows you to create an AI assistant using import openai with ease.
 
 # Usage:
 
 # ROLES :                  'system' = System Guide, 'assistant' = Ai Assistant, 'user' = User
 # DEFAULT GPT DICT :       {'role': 'system', 'content': 'You are a friendly assistant.'}
 # DEFAULT ROLES FILE :     'roles.txt'
@@ -17,19 +17,19 @@
 Example Of Initializing Classes -
     Memory1 = OpenAssist.Memory() - Initialize the memory list
     Roles = OpenAssist.Roles("roles.txt") - Initialize the roles list with the specified file/path
 
 Example Of OpenAI Completions -
     OpenAIRes = OpenAssist.OpenAIResponse(api_key, model_id="gpt-4") - Initialize the OpenAIResponse class (model_id is optional but defaults to gpt-4)
     OpenAIRes.chat_completion(Memory1.return_list()) - Run the OpenAI Chat Completion function
-    OpenAIRes.completion(prompt, max_tokens=100) - Run the OpenAI Completion function
+    OpenAIRes.completion(prompt, max_tokens=150) - Run the OpenAI Completion function
 
 OpenAIResponse -
-    chat_completion(memory_list) - Run the OpenAI Chat Completion function
-    completion(prompt, max_tokens=100) - Run the OpenAI Completion function (max_tokens is optional but defaults to 100)
+    chat_completion(memory_list, max_tokens=150) - Run the OpenAI Chat Completion function
+    completion(prompt, max_tokens=150) - Run the OpenAI Completion function (max_tokens is optional but defaults to 100)
 
 Roles -
     [Roles.] - Instance Name
     add(role_name, role_content, as_role) - Add a role to the roles list
     remove(role_name) - Remove a role from the roles list
     view() - View the roles list
     select(role_name) - Get a selected role from the roles list
@@ -73,45 +73,48 @@
 
             openai.api_key = self.api_key
         except Exception as e:
             raise Exception(f"Unexpected error: {e}")
 
     # OpenAssist.OpenAIResponse.functions - OpenAIResponse.chat_completion(), OpenAIResponse.completion()
 
-    def chat_completion(self, memory_list):
+    def chat_completion(self, memory_list, max_tokens=150):
         """
         Run the OpenAI Chat Completion function.
         
         memory_list - The memory list to use for the chat completion.
         """
 
         try:
             if not isinstance(memory_list, list):
                 raise ValueError("Memory list must be a list.")
             if not memory_list:
                 raise ValueError("Memory list cannot be empty.")
+            if not isinstance(max_tokens, int):
+                raise ValueError("Max tokens must be an integer.")
 
             try:
                 response = openai.ChatCompletion.create(
                     model=self.model_id,
-                    messages=memory_list
+                    messages=memory_list,
+                    max_tokens=max_tokens
                 )
             except openai.error.OpenAIError as e:
                 raise Exception(f"OpenAI error: {e}")
             except Exception as e:
                 raise Exception(f"Unexpected error: {e}")
 
             try:
                 return response.choices[0].message.content
             except (AttributeError, IndexError):
                 raise Exception("Unexpected response structure from API.")
         except Exception as e:
             raise Exception(f"Unexpected error: {e}")
     
-    def completion(self, prompt, max_tokens=100):
+    def completion(self, prompt, max_tokens=150):
         """
         Run the OpenAI Completion function.
         
         prompt - The prompt to use for the completion.
         max_tokens - The maximum number of tokens to generate.
         """
 
@@ -119,16 +122,14 @@
 
             if not isinstance(prompt, str):
                 raise ValueError("Prompt must be a string.")
             if not prompt:
                 raise ValueError("Prompt cannot be empty.")
             if not isinstance(max_tokens, int):
                 raise ValueError("Max tokens must be an integer.")
-            if not max_tokens:
-                raise ValueError("Max tokens cannot be empty.")
             
             try:
                 response = openai.Completion.create(
                     engine=self.model_id,
                     prompt=prompt,
                     max_tokens=max_tokens
                 )
```

### Comparing `openassist-2.2.6/PKG-INFO` & `openassist-2.2.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openassist
-Version: 2.2.6
+Version: 2.2.7
 Summary: OpenAssist is a module for Python that allows you to create an AI assistant using import openai with ease.
 License: MIT
 Author: Free Zoloft
 Author-email: mybusinessemaildbb@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -80,7 +80,14 @@
     clear() - Clear the memory list
     view_list() - View the memory list
     return_list() - Return the memory list
     edit(dictionary, index) - Edit a dictionary in the memory list at the specified index
     get_index(dictionary) - Get the index of a dictionary in the memory list
 """
 ```
+
+## Dev Log:
+
+```python
+# 2.2.6 - Initial Release
+# 2.2.7 - Added max_tokens parameter to chat_completion() and completion() functions
+```
```

