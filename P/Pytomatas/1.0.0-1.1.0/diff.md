# Comparing `tmp/Pytomatas-1.0.0.tar.gz` & `tmp/Pytomatas-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytomatas-1.0.0.tar", last modified: Sun Jun  4 22:37:17 2023, max compression
+gzip compressed data, was "Pytomatas-1.1.0.tar", last modified: Sun Jun  4 23:00:57 2023, max compression
```

## Comparing `Pytomatas-1.0.0.tar` & `Pytomatas-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:37:17.110974 Pytomatas-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-04 22:37:05.000000 Pytomatas-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-04 22:37:17.110974 Pytomatas-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-04 22:37:05.000000 Pytomatas-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:37:17.110974 Pytomatas-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-04 22:37:05.000000 Pytomatas-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:37:17.110974 Pytomatas-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:37:17.110974 Pytomatas-1.0.0/src/Pytomatas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-04 22:37:17.000000 Pytomatas-1.0.0/src/Pytomatas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-04 22:37:17.000000 Pytomatas-1.0.0/src/Pytomatas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:37:17.000000 Pytomatas-1.0.0/src/Pytomatas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:37:17.000000 Pytomatas-1.0.0/src/Pytomatas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-04 23:00:45.000000 Pytomatas-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-04 23:00:45.000000 Pytomatas-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-04 23:00:45.000000 Pytomatas-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:00:57.318496 Pytomatas-1.1.0/src/Pytomatas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:00:57.000000 Pytomatas-1.1.0/src/Pytomatas.egg-info/top_level.txt
```

### Comparing `Pytomatas-1.0.0/LICENSE` & `Pytomatas-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pytomatas-1.0.0/PKG-INFO` & `Pytomatas-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: Pytomatas
-Version: 1.0.0
+Version: 1.1.0
 Summary: Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines
 Home-page: https://github.com/arhcoder/Pytomatas
 Author: arhcoder
 Author-email: arhcoder@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/arhcoder/Pytomatas/issues
 Project-URL: Contribution, https://github.com/arhcoder/Pytomatas/pulls
+Project-URL: Author, https://github.com/arhcoder
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -76,15 +77,15 @@
 Example of a DFA implementation...
 
 #### 🧿 First implementation
 
 **1. Creating empty automata and then give the data:**
 
 ```python
-from pytomatas import DFA
+from Pytomatas.dfa import DFA
 
 # Creates a DFA called "my_dfa":
 my_dfa = DFA()
 
 # Define to "my_dfa" a set of states names:
 my_dfa.setStates( {"q0", "q1", "qfinal"} )
 
@@ -125,15 +126,15 @@
 ```
 
 #### 🧿 Second implementation
 
 **2. Creating the automata passing the data:**
 
 ```python
-from pytomatas import DFA
+from Pytomatas.dfa import DFA
 
 # Declare the States:
 Q = {"q0", "qa", "q1", "qb", "q2", "qf", "qx"}
 
 # Declare the Alphabet:
 A = {"a", "b"}
```

### Comparing `Pytomatas-1.0.0/README.md` & `Pytomatas-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 Example of a DFA implementation...
 
 #### 🧿 First implementation
 
 **1. Creating empty automata and then give the data:**
 
 ```python
-from pytomatas import DFA
+from Pytomatas.dfa import DFA
 
 # Creates a DFA called "my_dfa":
 my_dfa = DFA()
 
 # Define to "my_dfa" a set of states names:
 my_dfa.setStates( {"q0", "q1", "qfinal"} )
 
@@ -107,15 +107,15 @@
 ```
 
 #### 🧿 Second implementation
 
 **2. Creating the automata passing the data:**
 
 ```python
-from pytomatas import DFA
+from Pytomatas.dfa import DFA
 
 # Declare the States:
 Q = {"q0", "qa", "q1", "qb", "q2", "qf", "qx"}
 
 # Declare the Alphabet:
 A = {"a", "b"}
```

### Comparing `Pytomatas-1.0.0/setup.py` & `Pytomatas-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setup(
     name="Pytomatas",
-    version="1.0.0",
+    version="1.1.0",
     author="arhcoder",
     author_email="arhcoder@gmail.com",
     description="Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arhcoder/Pytomatas",
     license="MIT License",
     packages=find_packages(),
     include_package_data=True,
     project_urls={
         "Bug Tracker": "https://github.com/arhcoder/Pytomatas/issues",
-        "Contribution": "https://github.com/arhcoder/Pytomatas/pulls"
+        "Contribution": "https://github.com/arhcoder/Pytomatas/pulls",
+        "Author": "https://github.com/arhcoder"
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     package_dir={"": "src"},
```

### Comparing `Pytomatas-1.0.0/src/Pytomatas.egg-info/PKG-INFO` & `Pytomatas-1.1.0/src/Pytomatas.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: Pytomatas
-Version: 1.0.0
+Version: 1.1.0
 Summary: Simulates Automatons Acceptors DFA, NFA, PDA and Turing Machines
 Home-page: https://github.com/arhcoder/Pytomatas
 Author: arhcoder
 Author-email: arhcoder@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/arhcoder/Pytomatas/issues
 Project-URL: Contribution, https://github.com/arhcoder/Pytomatas/pulls
+Project-URL: Author, https://github.com/arhcoder
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -76,15 +77,15 @@
 Example of a DFA implementation...
 
 #### 🧿 First implementation
 
 **1. Creating empty automata and then give the data:**
 
 ```python
-from pytomatas import DFA
+from Pytomatas.dfa import DFA
 
 # Creates a DFA called "my_dfa":
 my_dfa = DFA()
 
 # Define to "my_dfa" a set of states names:
 my_dfa.setStates( {"q0", "q1", "qfinal"} )
 
@@ -125,15 +126,15 @@
 ```
 
 #### 🧿 Second implementation
 
 **2. Creating the automata passing the data:**
 
 ```python
-from pytomatas import DFA
+from Pytomatas.dfa import DFA
 
 # Declare the States:
 Q = {"q0", "qa", "q1", "qb", "q2", "qf", "qx"}
 
 # Declare the Alphabet:
 A = {"a", "b"}
```

