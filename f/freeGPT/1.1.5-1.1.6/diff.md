# Comparing `tmp/freeGPT-1.1.5.tar.gz` & `tmp/freeGPT-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.1.5.tar", last modified: Thu Jun  1 07:58:15 2023, max compression
+gzip compressed data, was "freeGPT-1.1.6.tar", last modified: Mon Jun  5 09:16:21 2023, max compression
```

## Comparing `freeGPT-1.1.5.tar` & `freeGPT-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 07:58:15.338979 freeGPT-1.1.5/
--rw-rw-rw-   0        0        0    35149 2023-06-01 07:56:30.000000 freeGPT-1.1.5/LICENSE
--rw-rw-rw-   0        0        0       98 2023-06-01 07:56:30.000000 freeGPT-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3226 2023-06-01 07:58:15.338007 freeGPT-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2023-06-01 07:56:30.000000 freeGPT-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 07:58:15.309973 freeGPT-1.1.5/freeGPT/
--rw-rw-rw-   0        0        0     2340 2023-06-01 07:56:30.000000 freeGPT-1.1.5/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:58:15.314974 freeGPT-1.1.5/freeGPT/alpaca/
--rw-rw-rw-   0        0        0     1530 2023-06-01 07:56:30.000000 freeGPT-1.1.5/freeGPT/alpaca/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:58:15.316975 freeGPT-1.1.5/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     5171 2023-06-01 07:56:30.000000 freeGPT-1.1.5/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:58:15.318976 freeGPT-1.1.5/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6799 2023-06-01 07:56:30.000000 freeGPT-1.1.5/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:58:15.313974 freeGPT-1.1.5/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3226 2023-06-01 07:58:15.000000 freeGPT-1.1.5/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-06-01 07:58:15.000000 freeGPT-1.1.5/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 07:58:15.000000 freeGPT-1.1.5/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-01 07:58:15.000000 freeGPT-1.1.5/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 07:58:15.000000 freeGPT-1.1.5/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 07:58:15.338979 freeGPT-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1518 2023-06-01 07:56:30.000000 freeGPT-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.838091 freeGPT-1.1.6/
+-rw-rw-rw-   0        0        0    35149 2023-06-05 09:10:43.000000 freeGPT-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-06-05 09:10:43.000000 freeGPT-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3399 2023-06-05 09:16:21.822446 freeGPT-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2324 2023-06-05 09:10:43.000000 freeGPT-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.791195 freeGPT-1.1.6/freeGPT/
+-rw-rw-rw-   0        0        0     2319 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.806823 freeGPT-1.1.6/freeGPT/alpaca_7b/
+-rw-rw-rw-   0        0        0     1530 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/alpaca_7b/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.822446 freeGPT-1.1.6/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     5171 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.822446 freeGPT-1.1.6/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     6799 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.806823 freeGPT-1.1.6/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3399 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 09:16:21.838091 freeGPT-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1539 2023-06-05 09:10:43.000000 freeGPT-1.1.6/setup.py
```

### Comparing `freeGPT-1.1.5/LICENSE` & `freeGPT-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.5/PKG-INFO` & `freeGPT-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.5
+Version: 1.1.6
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
+Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,alpaca-7b,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,23 +22,27 @@
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
-*Get started by doing: `pip install freeGPT==1.1.3`*
+Get started by installing the package:
+```
+py -m pip install --upgrade freeGPT
+```
 
 ## Source:
-*Models with .web have internet access on.*
+*Both GPT models have internet access.*
 <br>
-| Models            | Websites                                 |
-| ----------------- | -----------------------------------------|
-| gpt3              | [you.com](https://you.com)               |
-| gpt4              | [forefront.ai](https://chat.forefront.ai)|
+| Models            | Websites                                             |
+| ----------------- | -----------------------------------------------------|
+| gpt3              | [you.com](https://you.com)                           |
+| gpt4              | [forefront.ai](https://chat.forefront.ai)            |
+| alpaca_7b         | [chatllama.baseten.co](https://chatllama.baseten.co/)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
@@ -49,23 +53,14 @@
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
-#### Alpaca-7b:
-```python
-from freeGPT import alpaca
-
-while True:
-    prompt = input("👦 > ")
-    resp = alpaca.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp}")
-```
 #### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
     resp = gpt3.Completion.create(prompt=prompt)
@@ -79,10 +74,20 @@
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
     resp = gpt4.Completion.create(prompt=prompt, token=token)
     print(f"🤖 > {resp.text}")
 ```
 
+#### Alpaca-7b:
+```python
+from freeGPT import alpaca_7b
+
+while True:
+    prompt = input("👦 > ")
+    resp = alpaca_7b.Completion.create(prompt=prompt)
+    print(f"🤖 > {resp}")
+```
+
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.5/README.md` & `freeGPT-1.1.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
-*Get started by doing: `pip install freeGPT==1.1.3`*
+Get started by installing the package:
+```
+py -m pip install --upgrade freeGPT
+```
 
 ## Source:
-*Models with .web have internet access on.*
+*Both GPT models have internet access.*
 <br>
-| Models            | Websites                                 |
-| ----------------- | -----------------------------------------|
-| gpt3              | [you.com](https://you.com)               |
-| gpt4              | [forefront.ai](https://chat.forefront.ai)|
+| Models            | Websites                                             |
+| ----------------- | -----------------------------------------------------|
+| gpt3              | [you.com](https://you.com)                           |
+| gpt4              | [forefront.ai](https://chat.forefront.ai)            |
+| alpaca_7b         | [chatllama.baseten.co](https://chatllama.baseten.co/)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
@@ -27,23 +31,14 @@
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
-#### Alpaca-7b:
-```python
-from freeGPT import alpaca
-
-while True:
-    prompt = input("👦 > ")
-    resp = alpaca.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp}")
-```
 #### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
     resp = gpt3.Completion.create(prompt=prompt)
@@ -57,10 +52,20 @@
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
     resp = gpt4.Completion.create(prompt=prompt, token=token)
     print(f"🤖 > {resp.text}")
 ```
 
+#### Alpaca-7b:
+```python
+from freeGPT import alpaca_7b
+
+while True:
+    prompt = input("👦 > ")
+    resp = alpaca_7b.Completion.create(prompt=prompt)
+    print(f"🤖 > {resp}")
+```
+
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.5/freeGPT/__init__.py` & `freeGPT-1.1.6/freeGPT/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,78 @@
 from enum import Enum
-from freeGPT import gpt3, gpt4, alpaca
+from freeGPT import gpt3, gpt4, alpaca_7b
 
 __author__ = "Ruu3f"
-__version__ = "1.1.5"
+__version__ = "1.1.6"
 __all__ = ["Provider", "Completion"]
 
 
 class Provider(Enum):
     """Enum class representing the available GPT providers."""
 
-    ALPACA = "alpaca"
+    ALPACA_7B = "alpaca_7b"
     GPT3 = "gpt3"
     GPT4 = "gpt4"
 
 
 class Completion:
     """Class for generating completions using different GPT providers."""
 
     @staticmethod
     def create(provider: Provider, prompt: str, **kwargs) -> str:
-        """
-        Generates a completion using the specified provider.
+        """Generates a completion using the specified provider.
 
         Args:
             provider (Provider): The GPT provider to use.
             prompt (str): The prompt text for completion.
             **kwargs: Additional keyword arguments specific to the provider.
 
         Returns:
             str: The generated completion text.
 
         Raises:
             Exception: If the provider doesn't exist.
         """
-        if provider == Provider.ALPACA:
+        if provider == Provider.ALPACA_7B:
             return Completion._alpaca_service(prompt, **kwargs)
         elif provider == Provider.GPT3:
             return Completion._gpt3_service(prompt, **kwargs)
         elif provider == Provider.GPT4:
             return Completion._gpt4_service(prompt, **kwargs)
         else:
             raise Exception("Provider doesn't exist. Please check it again.")
 
     @staticmethod
     def _alpaca_service(prompt: str) -> str:
-        """
-        Generates a completion using the Alpaca provider.
+        """Generates a completion using the Alpaca provider.
 
         Args:
             prompt (str): The prompt text for completion.
 
         Returns:
             str: The generated completion text.
         """
-        return alpaca.Completion.create(prompt=prompt)
+        return alpaca_7b.Completion.create(prompt=prompt)
 
     @staticmethod
     def _gpt3_service(prompt: str) -> str:
-        """
-        Generates a completion using the GPT-3 provider.
+        """Generates a completion using the GPT-3 provider.
 
         Args:
             prompt (str): The prompt text for completion.
 
         Returns:
             str: The generated completion text.
         """
         resp = gpt3.Completion.create(prompt=prompt)
         return resp["text"]
 
     @staticmethod
     def _gpt4_service(prompt: str) -> str:
-        """
-        Generates a completion using the GPT-4 provider.
+        """Generates a completion using the GPT-4 provider.
 
         Args:
             prompt (str): The prompt text for completion.
 
         Returns:
             str: The generated completion text.
         """
```

### Comparing `freeGPT-1.1.5/freeGPT/alpaca/__init__.py` & `freeGPT-1.1.6/freeGPT/alpaca_7b/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.5/freeGPT/gpt3/__init__.py` & `freeGPT-1.1.6/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.5/freeGPT/gpt4/__init__.py` & `freeGPT-1.1.6/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.5/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.6/freeGPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.5
+Version: 1.1.6
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
+Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,alpaca-7b,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,23 +22,27 @@
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
-*Get started by doing: `pip install freeGPT==1.1.3`*
+Get started by installing the package:
+```
+py -m pip install --upgrade freeGPT
+```
 
 ## Source:
-*Models with .web have internet access on.*
+*Both GPT models have internet access.*
 <br>
-| Models            | Websites                                 |
-| ----------------- | -----------------------------------------|
-| gpt3              | [you.com](https://you.com)               |
-| gpt4              | [forefront.ai](https://chat.forefront.ai)|
+| Models            | Websites                                             |
+| ----------------- | -----------------------------------------------------|
+| gpt3              | [you.com](https://you.com)                           |
+| gpt4              | [forefront.ai](https://chat.forefront.ai)            |
+| alpaca_7b         | [chatllama.baseten.co](https://chatllama.baseten.co/)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
@@ -49,23 +53,14 @@
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
-#### Alpaca-7b:
-```python
-from freeGPT import alpaca
-
-while True:
-    prompt = input("👦 > ")
-    resp = alpaca.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp}")
-```
 #### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
     resp = gpt3.Completion.create(prompt=prompt)
@@ -79,10 +74,20 @@
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
     resp = gpt4.Completion.create(prompt=prompt, token=token)
     print(f"🤖 > {resp.text}")
 ```
 
+#### Alpaca-7b:
+```python
+from freeGPT import alpaca_7b
+
+while True:
+    prompt = input("👦 > ")
+    resp = alpaca_7b.Completion.create(prompt=prompt)
+    print(f"🤖 > {resp}")
+```
+
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.5/setup.py` & `freeGPT-1.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.5",
+    version="1.1.6",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
         "artificial-intelligence",
         "machine-learning",
         "ai-models",
         "chatllama",
+        "alpaca-7b",
         "gpt4free",
         "freegpt",
         "chatgpt",
         "python",
         "alpaca",
         "openai",
         "gpt3",
```

