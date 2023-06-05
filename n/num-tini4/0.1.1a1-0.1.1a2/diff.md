# Comparing `tmp/num_tini4-0.1.1a1.tar.gz` & `tmp/num_tini4-0.1.1a2.tar.gz`

## Comparing `num_tini4-0.1.1a1.tar` & `num_tini4-0.1.1a2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/README-dev.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/make.bat
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/source/conf.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/source/index.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/source/modules.rst
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/source/src.num_tini4.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/docs/source/src.primes.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/src/num_tini4/__init__.py
--rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/src/num_tini4/num.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/src/primes/__init__.py
--rw-r--r--   0        0        0  6106672 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/src/primes/primes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/tests/__init__.py
--rw-r--r--   0        0        0   105838 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/tests/test_num.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/tests/test_speed.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/.gitignore
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/LICENSE
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 num_tini4-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/README-dev.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/.gitignore
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/make.bat
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/conf.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/index.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/modules.rst
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/src.num_tini4.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/docs/source/src.primes.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/num_tini4/__init__.py
+-rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/num_tini4/num.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/primes/__init__.py
+-rw-r--r--   0        0        0  6106672 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/src/primes/primes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/tests/__init__.py
+-rw-r--r--   0        0        0   105838 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/tests/test_num.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/tests/test_speed.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/.gitignore
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/README.md
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 num_tini4-0.1.1a2/PKG-INFO
```

### Comparing `num_tini4-0.1.1a1/README-dev.md` & `num_tini4-0.1.1a2/README-dev.md`

 * *Files 5% similar despite different names*

```diff
@@ -107,7 +107,9 @@
 - https://stackoverflow.com/questions/53668052/sphinx-cannot-find-my-python-files-says-no-module-named
 
 ## 5
 - https://stackoverflow.com/questions/26344081/efficient-prime-factorization-for-large-numbers#26344929
 
 make html
 make clean html
+
+* https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
```

### Comparing `num_tini4-0.1.1a1/.github/workflows/codecov.yml` & `num_tini4-0.1.1a2/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/.github/workflows/pylint.yml` & `num_tini4-0.1.1a2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/.github/workflows/python-publish.yml` & `num_tini4-0.1.1a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/docs/Makefile` & `num_tini4-0.1.1a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/docs/make.bat` & `num_tini4-0.1.1a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/docs/source/conf.py` & `num_tini4-0.1.1a2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/src/num_tini4/num.py` & `num_tini4-0.1.1a2/src/num_tini4/num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/src/primes/primes.py` & `num_tini4-0.1.1a2/src/primes/primes.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/tests/test_num.py` & `num_tini4-0.1.1a2/tests/test_num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/README.md` & `num_tini4-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `num_tini4-0.1.1a1/PKG-INFO` & `num_tini4-0.1.1a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: num_tini4
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: Python precise number type.
 Project-URL: Documentation, https://github.com/Tini4/Num/wiki
 Project-URL: Source Code, https://github.com/Tini4/Num
 Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
 Author-email: Tini4 <tilen.jurican@gmail.com>
+License: Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License
+        
+        https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

