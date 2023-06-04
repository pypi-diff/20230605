# Comparing `tmp/tree-of-thoughts-0.3.2.tar.gz` & `tmp/tree-of-thoughts-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.3.2.tar", last modified: Thu Jun  1 02:10:00 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.3.3.tar", last modified: Sun Jun  4 23:08:56 2023, max compression
```

## Comparing `tree-of-thoughts-0.3.2.tar` & `tree-of-thoughts-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-01 02:09:47.000000 tree-of-thoughts-0.3.2/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:10:00.663338 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 02:10:00.000000 tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/abstractLanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/guidanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/huggingModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/openaiModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42213 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.3.2/LICENSE` & `tree-of-thoughts-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.2/PKG-INFO` & `tree-of-thoughts-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.3.2/setup.py` & `tree-of-thoughts-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.3.2',
+  version = '0.3.3',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.3.2/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.3.3/tree_of_thoughts/guidanceModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.2/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.3.3/tree_of_thoughts/huggingModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.2/tree_of_thoughts/openaiModels.py` & `tree-of-thoughts-0.3.3/tree_of_thoughts/openaiModels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import os
 import openai
 import time
 from  tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
 import concurrent.futures
+import logging 
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+logger = logging.getLogger(__name__)
+
 
 class OpenAILanguageModel(AbstractLanguageModel):
     def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=True):
         if api_key == "" or api_key == None:
             api_key = os.environ.get("OPENAI_API_KEY", "")
         if api_key != "":
             openai.api_key = api_key
@@ -78,22 +83,22 @@
             text = choice.text.strip()
         return text
     
     def generate_text(self, prompt, k):
         if self.use_chat_api:
             thoughts = []
             for _ in range(k):
-                response = self.openai_api_call_handler(prompt, 1000, 0.5, k)
+                response = self.openai_api_call_handler(prompt, 400, 0.5, k)
                 text = self.openai_choice2text_handler(response.choices[0])
                 thoughts += [text]
-                print(f'thoughts: {thoughts}')
+                # print(f'thoughts: {thoughts}')
             return thoughts
             
         else:
-            response = self.openai_api_call_handler(prompt, 1000, 0.5, k)
+            response = self.openai_api_call_handler(prompt, 300, 0.5, k)
             thoughts = [self.openai_choice2text_handler(choice) for choice in response.choices]
             return thoughts
 
 
 
     def generate_thoughts(self, state, k, initial_prompt, rejected_solutions=None):
         if (type(state) == str):
@@ -109,53 +114,61 @@
         ###{rejected_solutions}###, 
         complete the {initial_prompt} without making the same mistakes you did with the evaluated rejected solutions. Be simple. Be direct. Provide intuitive solutions as soon as you think of them."""
         
         prompt += self.ReAct_prompt
         # print(prompt)
         thoughts = self.generate_text(prompt, k)
         # print(thoughts)
-        print(f"Generated thoughts: {thoughts}")
+        # print(f"Generated thoughts: {thoughts}")
         return thoughts
 
         
     def generate_solution(self, initial_prompt, state, rejected_solutions=None):
-        if (type(state) == str):
-            state_text = state
-        else:
-            state_text = '\n'.join(state)
-        
-        prompt = f"""You're an TreeofThoughts, an superintelligent AI model devoted to helping Humans by any means necessary. You're purpose is to generate a series of solutions to comply with the user's instructions, you must generate solutions on the basis of determining the most reliable solution in the shortest amount of time, while taking rejected solutions into account and learning from them. 
-        Considering the reasoning provided:\n\n
-        ###'{state_text}'\n\n###
-        Devise the best possible solution for the task: {initial_prompt}, Here are evaluated solutions that were rejected: 
-        ###{rejected_solutions}###, 
-        complete the {initial_prompt} without making the same mistakes you did with the evaluated rejected solutions. Be simple. Be direct. Provide intuitive solutions as soon as you think of them."""
-        answer = self.generate_text(prompt, 1)
-        # print(thoughts)
-        print(f"General Solution : {answer}")
-        return answer
+        try:
+                
+            if isinstance(state, list):
+                state_text = '\n'.join(state)
+            else:
+                state_text = state
+            
+            prompt = f"""You're an TreeofThoughts, an superintelligent AI model devoted to helping Humans by any means necessary. You're purpose is to generate a series of solutions to comply with the user's instructions, you must generate solutions on the basis of determining the most reliable solution in the shortest amount of time, while taking rejected solutions into account and learning from them. 
+            Considering the reasoning provided:\n\n
+            ###'{state_text}'\n\n###
+            Devise the best possible solution for the task: {initial_prompt}, Here are evaluated solutions that were rejected: 
+            ###{rejected_solutions}###, 
+            complete the {initial_prompt} without making the same mistakes you did with the evaluated rejected solutions. Be simple. Be direct. Provide intuitive solutions as soon as you think of them."""
+            answer = self.generate_text(prompt, 1)
+            print(f'Answerrrrrr {answer}')
+            # print(thoughts)
+            # print(f"General Solution : {answer}")
+            return answer
+        except Exception as e:
+            logger.error(f"Error in generate_solutions: {e}")
+            return None
 
     def evaluate_states(self, states, initial_prompt):
-
+        if not states:
+            return {}
 
         if self.evaluation_strategy == 'value':
             state_values = {}
             for state in states:
                 if (type(state) == str):
                     state_text = state
                 else:
                     state_text = '\n'.join(state)
                 print("We receive a state of type", type(state), "For state: ", state, "\n\n")
                 # prompt = f"Given the current state of reasoning: '{state_text}', evaluate its value as a float between 0 and 1, become very pessimistic think of potential adverse risks on the probability of this state of reasoning achieveing {initial_prompt} and DO NOT RESPOND WITH ANYTHING ELSE: OTHER THAN AN FLOAT"
-                prompt = f""" To achieve the following goal: '{initial_prompt}', value the context of the past solutions and more importantly the latest generated solution you had AS A FLOAT BETWEEN 0 AND 1\n
+                prompt = f""" To achieve the following goal: '{initial_prompt}', pessimistically value the context of the past solutions and more importantly the latest generated solution you had AS A FLOAT BETWEEN 0 AND 1\n
                     Past solutions:\n\n
                     {state_text}\n       
                     If the solutions is not directly concretely making fast progress in achieving the goal, give it a lower score.
-                    Evaluation AS A FLOAT BETWEEN 0 and 1:\n, and then inside backticks provide an simple and direct bulletpoint list as to why you evaluated this thought the way you did. Provide simple yet intuitive feedback.
+                    Evaluate all solutions AS A FLOAT BETWEEN 0 and 1:\n,  DO NOT RETURN ANYTHING ELSE
                 """
+                # and then inside backticks provide an simple and direct bulletpoint list as to why you evaluated this thought the way you did. Provide simple yet intuitive feedback.
                 
                 response = self.openai_api_call_handler(prompt, 10, 1)
                 try:
                     value_text = self.openai_choice2text_handler(response.choices[0])
                     # print(f'state: {value_text}')
                     value = float(value_text)
                     print(f"Evaluated Thought Value: {value}")
```

### Comparing `tree-of-thoughts-0.3.2/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

