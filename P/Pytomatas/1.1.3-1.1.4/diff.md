# Comparing `tmp/Pytomatas-1.1.3.tar.gz` & `tmp/Pytomatas-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytomatas-1.1.3.tar", last modified: Mon Jun  5 02:28:29 2023, max compression
+gzip compressed data, was "Pytomatas-1.1.4.tar", last modified: Mon Jun  5 02:39:01 2023, max compression
```

## Comparing `Pytomatas-1.1.3.tar` & `Pytomatas-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:28:29.679160 Pytomatas-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-05 02:28:29.679160 Pytomatas-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 02:28:29.679160 Pytomatas-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:28:29.675161 Pytomatas-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:28:29.679160 Pytomatas-1.1.3/src/Pytomatas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/src/Pytomatas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/src/Pytomatas/dfa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/src/Pytomatas/nfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/src/Pytomatas/pda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-05 02:28:14.000000 Pytomatas-1.1.3/src/Pytomatas/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:28:29.679160 Pytomatas-1.1.3/src/Pytomatas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-05 02:28:29.000000 Pytomatas-1.1.3/src/Pytomatas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 02:28:29.000000 Pytomatas-1.1.3/src/Pytomatas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 02:28:29.000000 Pytomatas-1.1.3/src/Pytomatas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 02:28:29.000000 Pytomatas-1.1.3/src/Pytomatas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:39:01.596555 Pytomatas-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-05 02:39:01.596555 Pytomatas-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 02:39:01.596555 Pytomatas-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:39:01.596555 Pytomatas-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:39:01.596555 Pytomatas-1.1.4/src/Pytomatas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/src/Pytomatas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/src/Pytomatas/dfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/src/Pytomatas/nfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/src/Pytomatas/pda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-05 02:38:47.000000 Pytomatas-1.1.4/src/Pytomatas/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:39:01.596555 Pytomatas-1.1.4/src/Pytomatas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-05 02:39:01.000000 Pytomatas-1.1.4/src/Pytomatas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 02:39:01.000000 Pytomatas-1.1.4/src/Pytomatas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 02:39:01.000000 Pytomatas-1.1.4/src/Pytomatas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 02:39:01.000000 Pytomatas-1.1.4/src/Pytomatas.egg-info/top_level.txt
```

### Comparing `Pytomatas-1.1.3/LICENSE` & `Pytomatas-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Pytomatas-1.1.3/PKG-INFO` & `Pytomatas-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytomatas
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines
 Home-page: https://github.com/arhcoder/Pytomatas
 Author: arhcoder
 Author-email: arhcoder@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/arhcoder/Pytomatas/issues
 Project-URL: Author, https://github.com/arhcoder
@@ -17,15 +17,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖 Pytomatas
 
-**📌 Version 1.1.3**
+**📌 Version 1.1.4**
 
 <hr>
 
 Pytomatas allows to simulate Acceptor Automata in the console with Python, implementing its characteristics using different definitions (mathematics included), with the following types:
 
 * **[DFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/dfa.md  "DFA") (Deterministic Finite Automaton)**;
 * **[NFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/nfa.md "NFA") (Non-deterministic Finite Automaton)**;
@@ -61,15 +61,15 @@
 <br>
 
 ## 🛠 Installation
 
 You can install Pytomatas using pip:
 
 ```bash
-pip install -i https://pypi.org/simple/ Pytomatas
+pip install Pytomatas
 ```
 
 <br>
 
 ## 💻 Usage
 
 There are two ways in which automata can be implemented:
```

### Comparing `Pytomatas-1.1.3/README.md` & `Pytomatas-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 🤖 Pytomatas
 
-**📌 Version 1.1.3**
+**📌 Version 1.1.4**
 
 <hr>
 
 Pytomatas allows to simulate Acceptor Automata in the console with Python, implementing its characteristics using different definitions (mathematics included), with the following types:
 
 * **[DFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/dfa.md  "DFA") (Deterministic Finite Automaton)**;
 * **[NFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/nfa.md "NFA") (Non-deterministic Finite Automaton)**;
@@ -40,15 +40,15 @@
 <br>
 
 ## 🛠 Installation
 
 You can install Pytomatas using pip:
 
 ```bash
-pip install -i https://pypi.org/simple/ Pytomatas
+pip install Pytomatas
 ```
 
 <br>
 
 ## 💻 Usage
 
 There are two ways in which automata can be implemented:
```

### Comparing `Pytomatas-1.1.3/setup.py` & `Pytomatas-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setup(
     name="Pytomatas",
-    version="1.1.3",
+    version="1.1.4",
     packages=["Pytomatas"] or find_packages("src"),
     package_dir={"": "src"},
     author="arhcoder",
     author_email="arhcoder@gmail.com",
     description="Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `Pytomatas-1.1.3/src/Pytomatas/dfa.py` & `Pytomatas-1.1.4/src/Pytomatas/dfa.py`

 * *Files identical despite different names*

### Comparing `Pytomatas-1.1.3/src/Pytomatas/nfa.py` & `Pytomatas-1.1.4/src/Pytomatas/nfa.py`

 * *Files identical despite different names*

### Comparing `Pytomatas-1.1.3/src/Pytomatas/pda.py` & `Pytomatas-1.1.4/src/Pytomatas/pda.py`

 * *Files identical despite different names*

### Comparing `Pytomatas-1.1.3/src/Pytomatas/tm.py` & `Pytomatas-1.1.4/src/Pytomatas/tm.py`

 * *Files identical despite different names*

### Comparing `Pytomatas-1.1.3/src/Pytomatas.egg-info/PKG-INFO` & `Pytomatas-1.1.4/src/Pytomatas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytomatas
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines
 Home-page: https://github.com/arhcoder/Pytomatas
 Author: arhcoder
 Author-email: arhcoder@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/arhcoder/Pytomatas/issues
 Project-URL: Author, https://github.com/arhcoder
@@ -17,15 +17,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖 Pytomatas
 
-**📌 Version 1.1.3**
+**📌 Version 1.1.4**
 
 <hr>
 
 Pytomatas allows to simulate Acceptor Automata in the console with Python, implementing its characteristics using different definitions (mathematics included), with the following types:
 
 * **[DFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/dfa.md  "DFA") (Deterministic Finite Automaton)**;
 * **[NFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/nfa.md "NFA") (Non-deterministic Finite Automaton)**;
@@ -61,15 +61,15 @@
 <br>
 
 ## 🛠 Installation
 
 You can install Pytomatas using pip:
 
 ```bash
-pip install -i https://pypi.org/simple/ Pytomatas
+pip install Pytomatas
 ```
 
 <br>
 
 ## 💻 Usage
 
 There are two ways in which automata can be implemented:
```

