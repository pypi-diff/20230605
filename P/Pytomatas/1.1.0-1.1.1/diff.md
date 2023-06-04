# Comparing `tmp/Pytomatas-1.1.0.tar.gz` & `tmp/Pytomatas-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytomatas-1.1.0.tar", last modified: Sun Jun  4 23:00:57 2023, max compression
+gzip compressed data, was "Pytomatas-1.1.1.tar", last modified: Sun Jun  4 23:18:32 2023, max compression
```

## Comparing `Pytomatas-1.1.0.tar` & `Pytomatas-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-04 23:00:45.000000 Pytomatas-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-04 23:00:45.000000 Pytomatas-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-04 23:00:45.000000 Pytomatas-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/src/Pytomatas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:18:32.779573 Pytomatas-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-04 23:18:17.000000 Pytomatas-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-04 23:18:32.779573 Pytomatas-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-04 23:18:17.000000 Pytomatas-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:18:32.779573 Pytomatas-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-04 23:18:17.000000 Pytomatas-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:18:32.775573 Pytomatas-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:18:32.775573 Pytomatas-1.1.1/src/Pytomatas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-04 23:18:32.000000 Pytomatas-1.1.1/src/Pytomatas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-04 23:18:32.000000 Pytomatas-1.1.1/src/Pytomatas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:18:32.000000 Pytomatas-1.1.1/src/Pytomatas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:18:32.000000 Pytomatas-1.1.1/src/Pytomatas.egg-info/top_level.txt
```

### Comparing `Pytomatas-1.1.0/LICENSE` & `Pytomatas-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Pytomatas-1.1.0/PKG-INFO` & `Pytomatas-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytomatas
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines
 Home-page: https://github.com/arhcoder/Pytomatas
 Author: arhcoder
 Author-email: arhcoder@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/arhcoder/Pytomatas/issues
 Project-URL: Contribution, https://github.com/arhcoder/Pytomatas/pulls
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖 Pytomatas
 
-**📌 Version 1.0.0**
+**📌 Version 1.1.1**
 
 <hr>
 
 Pytomatas allows to simulate Acceptor Automata in the console with Python, implementing its characteristics using different definitions (mathematics included), with the following types:
 
 * **[DFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/dfa.md  "DFA") (Deterministic Finite Automaton)**;
 * **[NFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/nfa.md "NFA") (Non-deterministic Finite Automaton)**;
```

### Comparing `Pytomatas-1.1.0/README.md` & `Pytomatas-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 🤖 Pytomatas
 
-**📌 Version 1.0.0**
+**📌 Version 1.1.1**
 
 <hr>
 
 Pytomatas allows to simulate Acceptor Automata in the console with Python, implementing its characteristics using different definitions (mathematics included), with the following types:
 
 * **[DFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/dfa.md  "DFA") (Deterministic Finite Automaton)**;
 * **[NFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/nfa.md "NFA") (Non-deterministic Finite Automaton)**;
```

### Comparing `Pytomatas-1.1.0/setup.py` & `Pytomatas-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setup(
     name="Pytomatas",
-    version="1.1.0",
+    version="1.1.1",
     author="arhcoder",
     author_email="arhcoder@gmail.com",
     description="Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arhcoder/Pytomatas",
     license="MIT License",
```

### Comparing `Pytomatas-1.1.0/src/Pytomatas.egg-info/PKG-INFO` & `Pytomatas-1.1.1/src/Pytomatas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytomatas
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines
 Home-page: https://github.com/arhcoder/Pytomatas
 Author: arhcoder
 Author-email: arhcoder@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/arhcoder/Pytomatas/issues
 Project-URL: Contribution, https://github.com/arhcoder/Pytomatas/pulls
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖 Pytomatas
 
-**📌 Version 1.0.0**
+**📌 Version 1.1.1**
 
 <hr>
 
 Pytomatas allows to simulate Acceptor Automata in the console with Python, implementing its characteristics using different definitions (mathematics included), with the following types:
 
 * **[DFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/dfa.md  "DFA") (Deterministic Finite Automaton)**;
 * **[NFA](https://github.com/arhcoder/Pytomatas/blob/master/docs/nfa.md "NFA") (Non-deterministic Finite Automaton)**;
```

