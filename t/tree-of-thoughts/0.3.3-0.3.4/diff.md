# Comparing `tmp/tree-of-thoughts-0.3.3.tar.gz` & `tmp/tree-of-thoughts-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.3.3.tar", last modified: Sun Jun  4 23:08:56 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.3.4.tar", last modified: Mon Jun  5 20:28:19 2023, max compression
```

## Comparing `tree-of-thoughts-0.3.3.tar` & `tree-of-thoughts-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    42213 2023-06-04 23:08:42.000000 tree-of-thoughts-0.3.3/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:08:56.078582 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 23:08:56.000000 tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/abstractLanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/guidanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/huggingModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/openaiModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.3.3/LICENSE` & `tree-of-thoughts-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.3/PKG-INFO` & `tree-of-thoughts-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.3.3/README.md` & `tree-of-thoughts-0.3.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,42 @@
+# Agora
+This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research!
+
+
+![Agora banner](agora-banner.png)
+
+[Join our Discord and contribute to this project](https://discord.gg/qUtxnK2NMf)
+
 # Tree of Thoughts 🌳🌲🌴🌿🍃
 
 ![tree of thoughts banner](tree-of-thoughts.png)
 
 [Paper link](https://arxiv.org/pdf/2305.10601.pdf)
 
 Tree of Thoughts (ToT) is an all-new powerful and flexible algorithm that advances model reasoning by a whopping 70%. This is an plug in and play verision, connect your own models and enjoy superintelligence!
 
+## 🔥 All-New Search Algorithms
 
-Share this repository by clicking on the following buttons 😊 
+* MonteCarlo
 
-[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
-[![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
+* A* Search 
 
-# Join Agora, Creators United
-This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research!
+* Best First Search
 
+#### Coming soon!
+* Iterative Depth Search 
+
+* Any search algorithms you like?? Open an issue 😊 
+
+
+Help cultivate this repository to democratize superintelligence! Share this repository by clicking on the following buttons 😊 
+
+[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
+[![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 
-[Join our Discord and contribute to this project](https://discord.gg/qUtxnK2NMf)
 
 
 # Basic Prompts:
 No complex implementations, just pass in one of these prompts to your model: head over to `prompts.txt`
 
 'Three experts with exceptional logical thinking skills are collaboratively answering a question using a tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The question is...'
 
@@ -37,19 +53,18 @@
 
 ```git clone https://github.com/kyegomez/tree-of-thoughts```
 
 ``` 
 cd tree-of-thoughts
 python3 -m pip install -r requirements.txt
 cd tree_of_thoughts
-python3 treeofthoughts.py --problem "Design the architecture for an modern city optimized for happiness" --search_algorithm="BFS"
 ```
-Add ` OPENAI_API_KEY='API KEY'` in the .env!
+Then go to `montecarlo_example.py` and fill in your api key! 
 
-!!!! For much improved performance provide custom few prompt shots in the generate thoughts and generate states! !!!!!
+# 🔥 For much improved performance provide custom few prompt shots in the generate thoughts and generate states 🔥 
 
 And in the `examples` folder we have other examples for huggingface transformers + hugginggface pipelines
 
 ## Method2
 or:
 
 ```pip install tree-of-thoughts ```
@@ -151,55 +166,14 @@
 3. Create a state evaluator function V(pθ, S) with two strategies:
    a. Value each state independently.
    b. Vote across states.
 4. Choose a search algorithm (BFS or DFS) based on the tree structure.
 5. Implement the chosen search algorithm.
 6. Execute the chosen search algorithm with the input problem, thought generator, state evaluator, and other required parameters.
 
-## Tree of Thoughts Class
-``` python
-class TreeofThoughts:
-    
-    def __init__(self, model, search_algorithm):
-        self.model = model
-        self.search_algorithm = search_algorithm
-
-    def solve(self, x, k, T, b, vth):
-        if self.search_algorithm == 'BFS':
-            return self.tot_bfs(x, k, T, b)
-        elif self.search_algorithm == 'DFS':
-            return self.tot_dfs(x, k, T, vth)
-        else:
-            raise ValueError("Invalid search algorithm. Choose 'BFS' or 'DFS'.")
-
-    def tot_bfs(self, x, k, T, b):
-        S0 = {x}
-        for t in range(1, T + 1):
-            S0_t = {(*s, z) for s in S0 for z in self.model.generate_thoughts(s, k)}
-            Vt = self.model.evaluate_states(S0_t)
-            St = sorted(S0_t, key=lambda s: Vt[s], reverse=True)[:b]
-            S0 = set(St)
-        return self.model.generate_thoughts(max(St, key=lambda s: Vt[s]), 1)
-
-    def tot_dfs(self, x, k, T, vth):
-        output = []
-
-        def dfs(s, t):
-            if t > T:
-                output.append(self.model.generate_thoughts(s, 1))
-                return
-            for s_prime in sorted(self.model.generate_thoughts(s, k)):
-                if self.model.evaluate_states({s_prime})[s_prime] > vth:
-                    dfs((*s, s_prime), t + 1)
-
-        dfs(x, 1)
-        return output
-    
-```
-
 
 ## Usage Examples
 
 ### OpenAI API
 
 To use Tree of Thoughts with OpenAI's API, create a custom model class that inherits from `AbstractLanguageModel` and implements the required methods using OpenAI's API. Then, create an instance of the `TreeOfThoughts` class with the custom model and the desired search algorithm ('BFS' or 'DFS').
```

### Comparing `tree-of-thoughts-0.3.3/setup.py` & `tree-of-thoughts-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.3.3',
+  version = '0.3.4',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.3.3/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.3.4/tree_of_thoughts/guidanceModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.3/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.3.4/tree_of_thoughts/huggingModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.3/tree_of_thoughts/openaiModels.py` & `tree-of-thoughts-0.3.4/tree_of_thoughts/openaiModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.3/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

