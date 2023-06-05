# Comparing `tmp/num_tini4-0.1.2a1.tar.gz` & `tmp/num_tini4-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "num_tini4-0.1.2a1.tar", last modified: Mon Jun  5 13:05:19 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `num_tini4-0.1.2a1.tar` & `num_tini4-0.2.0a1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/num_tini4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/num_tini4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/num_tini4/num.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/num_tini4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 13:05:19.000000 num_tini4-0.1.2a1/src/num_tini4.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.763167 num_tini4-0.1.2a1/src/primes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/primes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  6106672 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/src/primes/primes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:05:19.771167 num_tini4-0.1.2a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   105838 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/tests/test_num.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 13:05:08.000000 num_tini4-0.1.2a1/tests/test_speed.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/README-dev.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/setup.cfg
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/docs/.gitignore
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/docs/make.bat
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/docs/source/conf.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/docs/source/index.rst
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/docs/source/modules.rst
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/docs/source/num_tini4.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/num_tini4/__init__.py
+-rw-r--r--   0        0        0    18965 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/num_tini4/num.py
+-rw-r--r--   0        0        0  6106672 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/num_tini4/primes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/tests/__init__.py
+-rw-r--r--   0        0        0   105830 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/tests/test_num.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/tests/test_speed.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/.gitignore
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 num_tini4-0.2.0a1/PKG-INFO
```

### Comparing `num_tini4-0.1.2a1/PKG-INFO` & `num_tini4-0.2.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: num_tini4
-Version: 0.1.2a1
+Version: 0.2.0a1
 Summary: Python precise number type.
-Home-page: https://github.com/Tini4/Num
-Author: Tini4
-Author-email: tilen.jurican@gmail.com
 Project-URL: Documentation, https://github.com/Tini4/Num/wiki
 Project-URL: Source Code, https://github.com/Tini4/Num
 Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
+Author-email: Tini4 <tilen.jurican@gmail.com>
+License: Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License
+        
+        https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode
+License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Num
 
 [![Pylint](https://github.com/Tini4/Num/actions/workflows/pylint.yml/badge.svg)](https://github.com/Tini4/Num/actions/workflows/pylint.yml)
 [![CodeCov](https://codecov.io/gh/Tini4/Num/branch/master/graph/badge.svg?token=BILTI4331O)](https://codecov.io/gh/Tini4/Num)
 
 Python precise number type.
@@ -105,11 +106,7 @@
 # Inaccurate!!! Slow!!! Avoid!!!
 num1.set_float(18 / 11)
 print(num1)                 # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}]
 print(num1.get_fraction())  # (7369526662969903, 4503599627370496)
 print(num1.get_float())     # 1.6363636363636365
 print(18 / 11)              # 1.6363636363636365
 ```
-
-Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License
-
-https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode
```

### Comparing `num_tini4-0.1.2a1/README.md` & `num_tini4-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.2a1/setup.cfg` & `num_tini4-0.2.0a1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -3,32 +3,27 @@
 version = 0.1.2a1
 author = Tini4
 author_email = tilen.jurican@gmail.com
 description = Python precise number type.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/Tini4/Num
-project_urls = 
-	Documentation = https://github.com/Tini4/Num/wiki
-	Source Code = https://github.com/Tini4/Num
-	Bug Tracker = https://github.com/Tini4/Num/issues
-classifiers = 
-	Development Status :: 1 - Planning
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
-	License :: Other/Proprietary License
-	Operating System :: OS Independent
-	Topic :: Scientific/Engineering :: Mathematics
+project_urls =
+    Documentation = https://github.com/Tini4/Num/wiki
+    Source Code = https://github.com/Tini4/Num
+    Bug Tracker = https://github.com/Tini4/Num/issues
+classifiers =
+    Development Status :: 1 - Planning
+    Programming Language :: Python :: 3.10
+    Programming Language :: Python :: 3.11
+    License :: Other/Proprietary License
+    Operating System :: OS Independent
+    Topic :: Scientific/Engineering :: Mathematics
 
 [options]
-package_dir = 
-	= src
+package_dir =
+    = src
 packages = find:
 python_requires = >=3.10
 
 [options.packages.find]
 where = src
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
```

### Comparing `num_tini4-0.1.2a1/src/num_tini4/num.py` & `num_tini4-0.2.0a1/num_tini4/num.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from math import inf, sqrt  # , log10
 
 # noinspection PyUnresolvedReferences
-from src.primes.primes import PRIMES, PRIMES_TO
+from num_tini4.primes import PRIMES, PRIMES_TO
 
 
 class Num:
     class Sign(Enum):
         POSITIVE = 1
         NEGATIVE = -1
```

### Comparing `num_tini4-0.1.2a1/src/num_tini4.egg-info/PKG-INFO` & `num_tini4-0.2.0a1/README-dev.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: num-tini4
-Version: 0.1.2a1
-Summary: Python precise number type.
-Home-page: https://github.com/Tini4/Num
-Author: Tini4
-Author-email: tilen.jurican@gmail.com
-Project-URL: Documentation, https://github.com/Tini4/Num/wiki
-Project-URL: Source Code, https://github.com/Tini4/Num
-Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
-Classifier: Development Status :: 1 - Planning
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Num
 
 [![Pylint](https://github.com/Tini4/Num/actions/workflows/pylint.yml/badge.svg)](https://github.com/Tini4/Num/actions/workflows/pylint.yml)
 [![CodeCov](https://codecov.io/gh/Tini4/Num/branch/master/graph/badge.svg?token=BILTI4331O)](https://codecov.io/gh/Tini4/Num)
 
 Python precise number type.
 
@@ -44,72 +24,88 @@
 
 ## Usage
 
 ```python
 # Import the Num class
 from num_tini4.num import Num
 
-
 # Declare variables
 num1: Num = Num()
 num2: Num = Num()
 
-
 # Define variables
 num1.set_fraction(1, 11)  # 1/11
-num2.set_int(-18)         # -18
+num2.set_int(-18)  # -18
 
 print(num1)  # [NUMBER, POSITIVE, {11: -1}]
 print(num2)  # [NUMBER, NEGATIVE, {2: 1, 3: 2}]
 
 print(repr(num1))  # Num(primes={11: -1}, sign=<Sign.POSITIVE: 1>, case=<Case.NUMBER: 1>)
 print(repr(num2))  # Num(primes={2: 1, 3: 2}, sign=<Sign.NEGATIVE: -1>, case=<Case.NUMBER: 1>)
 
 print(float(num1))  # 0.09090909090909091
 print(float(num2))  # -18.0
 
-
 # Arithmetic Operators
 print((num1 + num2).get_fraction())  # (-197, 11)
-print((num1 + num2).get_float())     # -17.90909090909091
-print((1 / 11) + -18.0)              # -17.90909090909091
+print((num1 + num2).get_float())  # -17.90909090909091
+print((1 / 11) + -18.0)  # -17.90909090909091
 print('--------------------------------------------------')
 
 print((num1 - num2).get_fraction())  # (199, 11)
-print((num1 - num2).get_float())     # 18.09090909090909
-print((1 / 11) - -18.0)              # 18.09090909090909
+print((num1 - num2).get_float())  # 18.09090909090909
+print((1 / 11) - -18.0)  # 18.09090909090909
 print('--------------------------------------------------')
 
 print((num1 * num2).get_fraction())  # (-18, 11)
-print((num1 * num2).get_float())     # -1.6363636363636365
-print((1 / 11) * -18.0)              # -1.6363636363636365
+print((num1 * num2).get_float())  # -1.6363636363636365
+print((1 / 11) * -18.0)  # -1.6363636363636365
 print('--------------------------------------------------')
 
 print((num1 / num2).get_fraction())  # (-1, 198)
-print((num1 / num2).get_float())     # -0.00505050505050505
-print((1 / 11) / -18.0)              # -0.005050505050505051
+print((num1 / num2).get_float())  # -0.00505050505050505
+print((1 / 11) / -18.0)  # -0.005050505050505051
 print('--------------------------------------------------')
 
-
 # todo: Assignment Operators
 #  +=, -=, *=, /=
 
 
 # todo: Comparison Operators
 #  <, >, <=, >=, ==, !=
 
 
 # Other
 # -, abs(), float()
 
 
 # Inaccurate!!! Slow!!! Avoid!!!
 num1.set_float(18 / 11)
-print(num1)                 # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}]
+print(num1)  # [NUMBER, POSITIVE, {2: -52, 19: 1, 26041: 1, 14894582557: 1}]
 print(num1.get_fraction())  # (7369526662969903, 4503599627370496)
-print(num1.get_float())     # 1.6363636363636365
-print(18 / 11)              # 1.6363636363636365
+print(num1.get_float())  # 1.6363636363636365
+print(18 / 11)  # 1.6363636363636365
 ```
 
-Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License
+## 1
+- http://www.java2s.com/Tutorials/Python/Class/Overload_divide_operator.htm
+- https://www.geeksforgeeks.org/operator-overloading-in-python/
+
+## 2
+- https://t5k.org/lists/small/millions/
+- https://t5k.org/notes/faq/LongestList.html
+- http://compoasso.free.fr/primelistweb/page/prime/liste_online_en.php
+
+## 3
+- https://www.sphinx-doc.org/en/master/usage/quickstart.html
+- https://towardsdatascience.com/documenting-python-code-with-sphinx-554e1d6c4f6d
+
+## 4
+- https://stackoverflow.com/questions/53668052/sphinx-cannot-find-my-python-files-says-no-module-named
+
+## 5
+- https://stackoverflow.com/questions/26344081/efficient-prime-factorization-for-large-numbers#26344929
+
+make html
+make clean html
 
-https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode
+* https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
```

### Comparing `num_tini4-0.1.2a1/src/primes/primes.py` & `num_tini4-0.2.0a1/num_tini4/primes.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.2a1/tests/test_num.py` & `num_tini4-0.2.0a1/tests/test_num.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src.num_tini4.num import Num
+from num_tini4 import Num
 
 
 class TestNumEnum(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_sign(self):  # todo
```

