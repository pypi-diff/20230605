# Comparing `tmp/num_tini4-0.1.1a2.tar.gz` & `tmp/num_tini4-0.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "num_tini4-0.1.2a1.tar", last modified: Mon Jun  5 13:05:19 2023, max compression
```

## Comparing `num_tini4-0.1.1a2.tar` & `num_tini4-0.1.2a1.tar`

### file list

```diff
@@ -1,25 +1,21 @@
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/README-dev.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/make.bat
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/conf.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/index.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/modules.rst
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/src.num_tini4.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/src.primes.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/num_tini4/__init__.py
--rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/num_tini4/num.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/primes/__init__.py
--rw-r--r--   0        0        0  6106672 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/primes/primes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/tests/__init__.py
--rw-r--r--   0        0        0   105838 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/tests/test_num.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/tests/test_speed.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.gitignore
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/LICENSE
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/README.md
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/num_tini4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/num_tini4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/num_tini4/num.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/num_tini4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/primes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/primes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  6106672 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/primes/primes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   105838 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/tests/test_num.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/tests/test_speed.py
```

### Comparing `num_tini4-0.1.1a2/README-dev.md` & `num_tini4-0.1.2a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: num_tini4
+Version: 0.1.2a1
+Summary: Python precise number type.
+Home-page: https://github.com/Tini4/Num
+Author: Tini4
+Author-email: tilen.jurican@gmail.com
+Project-URL: Documentation, https://github.com/Tini4/Num/wiki
+Project-URL: Source Code, https://github.com/Tini4/Num
+Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
+Classifier: Development Status :: 1 - Planning
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Num
 
 [![Pylint](https://github.com/Tini4/Num/actions/workflows/pylint.yml/badge.svg)](https://github.com/Tini4/Num/actions/workflows/pylint.yml)
 [![CodeCov](https://codecov.io/gh/Tini4/Num/branch/master/graph/badge.svg?token=BILTI4331O)](https://codecov.io/gh/Tini4/Num)
 
 Python precise number type.
 
@@ -22,15 +42,15 @@
 pip install num-tini4
 ```
 
 ## Usage
 
 ```python
 # Import the Num class
-from src.num_tini4.num import Num
+from num_tini4.num import Num
 
 
 # Declare variables
 num1: Num = Num()
 num2: Num = Num()
 
 
@@ -86,30 +106,10 @@
 num1.set_float(18 / 11)
 print(num1)                 # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}]
 print(num1.get_fraction())  # (7369526662969903, 4503599627370496)
 print(num1.get_float())     # 1.6363636363636365
 print(18 / 11)              # 1.6363636363636365
 ```
 
-## 1
-- http://www.java2s.com/Tutorials/Python/Class/Overload_divide_operator.htm
-- https://www.geeksforgeeks.org/operator-overloading-in-python/
-
-## 2
-- https://t5k.org/lists/small/millions/
-- https://t5k.org/notes/faq/LongestList.html
-- http://compoasso.free.fr/primelistweb/page/prime/liste_online_en.php
-
-## 3
-- https://www.sphinx-doc.org/en/master/usage/quickstart.html
-- https://towardsdatascience.com/documenting-python-code-with-sphinx-554e1d6c4f6d
-
-## 4
-- https://stackoverflow.com/questions/53668052/sphinx-cannot-find-my-python-files-says-no-module-named
-
-## 5
-- https://stackoverflow.com/questions/26344081/efficient-prime-factorization-for-large-numbers#26344929
-
-make html
-make clean html
+Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License
 
-* https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
+https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode
```

### Comparing `num_tini4-0.1.1a2/src/num_tini4/num.py` & `num_tini4-0.1.2a1/src/num_tini4/num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a2/src/primes/primes.py` & `num_tini4-0.1.2a1/src/primes/primes.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a2/tests/test_num.py` & `num_tini4-0.1.2a1/tests/test_num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a2/README.md` & `num_tini4-0.1.2a1/README.md`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a2/PKG-INFO` & `num_tini4-0.1.2a1/src/num_tini4.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
-Name: num_tini4
-Version: 0.1.1a2
+Name: num-tini4
+Version: 0.1.2a1
 Summary: Python precise number type.
+Home-page: https://github.com/Tini4/Num
+Author: Tini4
+Author-email: tilen.jurican@gmail.com
 Project-URL: Documentation, https://github.com/Tini4/Num/wiki
 Project-URL: Source Code, https://github.com/Tini4/Num
 Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
-Author-email: Tini4 <tilen.jurican@gmail.com>
-License: Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License
-        
-        https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode
-License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Num
 
 [![Pylint](https://github.com/Tini4/Num/actions/workflows/pylint.yml/badge.svg)](https://github.com/Tini4/Num/actions/workflows/pylint.yml)
 [![CodeCov](https://codecov.io/gh/Tini4/Num/branch/master/graph/badge.svg?token=BILTI4331O)](https://codecov.io/gh/Tini4/Num)
 
 Python precise number type.
@@ -106,7 +105,11 @@
 # Inaccurate!!! Slow!!! Avoid!!!
 num1.set_float(18 / 11)
 print(num1)                 # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}]
 print(num1.get_fraction())  # (7369526662969903, 4503599627370496)
 print(num1.get_float())     # 1.6363636363636365
 print(18 / 11)              # 1.6363636363636365
 ```
+
+Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License
+
+https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode
```

