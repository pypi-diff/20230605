# Comparing `tmp/nrpylatex-1.3.tar.gz` & `tmp/nrpylatex-1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrpylatex-1.3.tar", last modified: Mon Jun  5 17:51:12 2023, max compression
+gzip compressed data, was "nrpylatex-1.3.post1.tar", last modified: Mon Jun  5 20:18:59 2023, max compression
```

## Comparing `nrpylatex-1.3.tar` & `nrpylatex-1.3.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/
--rw-r--r--   0 ksible   (240660) campus    (1313)     1327 2022-12-18 22:56:57.000000 nrpylatex-1.3/LICENSE
--rw-r--r--   0 ksible   (240660) campus    (1313)     5690 2023-06-05 17:51:12.854257 nrpylatex-1.3/PKG-INFO
--rw-r--r--   0 ksible   (240660) campus    (1313)     4925 2023-06-02 22:29:45.000000 nrpylatex-1.3/README.md
-drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.850257 nrpylatex-1.3/nrpylatex/
--rw-r--r--   0 ksible   (240660) campus    (1313)      474 2023-06-02 23:36:58.000000 nrpylatex-1.3/nrpylatex/__init__.py
-drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex/core/
--rw-r--r--   0 ksible   (240660) campus    (1313)        0 2022-12-18 22:56:57.000000 nrpylatex-1.3/nrpylatex/core/__init__.py
--rw-r--r--   0 ksible   (240660) campus    (1313)    18012 2023-06-05 17:15:06.000000 nrpylatex-1.3/nrpylatex/core/generator.py
--rw-r--r--   0 ksible   (240660) campus    (1313)    63993 2023-06-05 17:16:27.000000 nrpylatex-1.3/nrpylatex/core/parser.py
--rw-r--r--   0 ksible   (240660) campus    (1313)     6356 2023-06-05 17:24:12.000000 nrpylatex-1.3/nrpylatex/core/scanner.py
--rw-r--r--   0 ksible   (240660) campus    (1313)     4209 2023-06-05 16:42:18.000000 nrpylatex-1.3/nrpylatex/parse_latex.py
-drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex/tests/
--rw-r--r--   0 ksible   (240660) campus    (1313)        0 2022-12-18 22:56:57.000000 nrpylatex-1.3/nrpylatex/tests/__init__.py
--rw-r--r--   0 ksible   (240660) campus    (1313)    21131 2023-06-05 16:41:31.000000 nrpylatex-1.3/nrpylatex/tests/test_parse_latex.py
-drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex/utils/
--rw-r--r--   0 ksible   (240660) campus    (1313)        0 2023-06-01 17:16:50.000000 nrpylatex-1.3/nrpylatex/utils/__init__.py
--rw-r--r--   0 ksible   (240660) campus    (1313)     4817 2023-06-01 17:16:50.000000 nrpylatex-1.3/nrpylatex/utils/assertion.py
--rw-r--r--   0 ksible   (240660) campus    (1313)      773 2023-06-05 17:37:40.000000 nrpylatex-1.3/nrpylatex/utils/exceptions.py
--rw-r--r--   0 ksible   (240660) campus    (1313)     2555 2023-06-01 17:16:50.000000 nrpylatex-1.3/nrpylatex/utils/functional.py
--rw-r--r--   0 ksible   (240660) campus    (1313)    19691 2023-06-01 17:34:36.000000 nrpylatex-1.3/nrpylatex/utils/structures.py
-drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex.egg-info/
--rw-r--r--   0 ksible   (240660) campus    (1313)     5690 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/PKG-INFO
--rw-r--r--   0 ksible   (240660) campus    (1313)      554 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/SOURCES.txt
--rw-r--r--   0 ksible   (240660) campus    (1313)        1 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/dependency_links.txt
--rw-r--r--   0 ksible   (240660) campus    (1313)        6 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/requires.txt
--rw-r--r--   0 ksible   (240660) campus    (1313)       10 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/top_level.txt
--rw-r--r--   0 ksible   (240660) campus    (1313)       38 2023-06-05 17:51:12.854257 nrpylatex-1.3/setup.cfg
--rw-r--r--   0 ksible   (240660) campus    (1313)     1149 2023-06-01 17:16:50.000000 nrpylatex-1.3/setup.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 20:18:59.751320 nrpylatex-1.3.post1/
+-rw-r--r--   0 ksible   (240660) campus    (1313)     1327 2022-12-18 22:56:57.000000 nrpylatex-1.3.post1/LICENSE
+-rw-r--r--   0 ksible   (240660) campus    (1313)     5696 2023-06-05 20:18:59.751320 nrpylatex-1.3.post1/PKG-INFO
+-rw-r--r--   0 ksible   (240660) campus    (1313)     4925 2023-06-05 20:12:43.000000 nrpylatex-1.3.post1/README.md
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 20:18:59.747321 nrpylatex-1.3.post1/nrpylatex/
+-rw-r--r--   0 ksible   (240660) campus    (1313)      480 2023-06-05 19:01:17.000000 nrpylatex-1.3.post1/nrpylatex/__init__.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 20:18:59.747321 nrpylatex-1.3.post1/nrpylatex/core/
+-rw-r--r--   0 ksible   (240660) campus    (1313)        0 2022-12-18 22:56:57.000000 nrpylatex-1.3.post1/nrpylatex/core/__init__.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    18012 2023-06-05 17:15:06.000000 nrpylatex-1.3.post1/nrpylatex/core/generator.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    63993 2023-06-05 17:16:27.000000 nrpylatex-1.3.post1/nrpylatex/core/parser.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     6356 2023-06-05 17:24:12.000000 nrpylatex-1.3.post1/nrpylatex/core/scanner.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     4209 2023-06-05 16:42:18.000000 nrpylatex-1.3.post1/nrpylatex/parse_latex.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 20:18:59.747321 nrpylatex-1.3.post1/nrpylatex/tests/
+-rw-r--r--   0 ksible   (240660) campus    (1313)        0 2022-12-18 22:56:57.000000 nrpylatex-1.3.post1/nrpylatex/tests/__init__.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    21131 2023-06-05 16:41:31.000000 nrpylatex-1.3.post1/nrpylatex/tests/test_parse_latex.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 20:18:59.751320 nrpylatex-1.3.post1/nrpylatex/utils/
+-rw-r--r--   0 ksible   (240660) campus    (1313)        0 2023-06-01 17:16:50.000000 nrpylatex-1.3.post1/nrpylatex/utils/__init__.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     4817 2023-06-01 17:16:50.000000 nrpylatex-1.3.post1/nrpylatex/utils/assertion.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)      825 2023-06-05 18:17:33.000000 nrpylatex-1.3.post1/nrpylatex/utils/exceptions.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     2555 2023-06-01 17:16:50.000000 nrpylatex-1.3.post1/nrpylatex/utils/functional.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    19691 2023-06-01 17:34:36.000000 nrpylatex-1.3.post1/nrpylatex/utils/structures.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 20:18:59.747321 nrpylatex-1.3.post1/nrpylatex.egg-info/
+-rw-r--r--   0 ksible   (240660) campus    (1313)     5696 2023-06-05 20:18:59.000000 nrpylatex-1.3.post1/nrpylatex.egg-info/PKG-INFO
+-rw-r--r--   0 ksible   (240660) campus    (1313)      554 2023-06-05 20:18:59.000000 nrpylatex-1.3.post1/nrpylatex.egg-info/SOURCES.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)        1 2023-06-05 20:18:59.000000 nrpylatex-1.3.post1/nrpylatex.egg-info/dependency_links.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)        6 2023-06-05 20:18:59.000000 nrpylatex-1.3.post1/nrpylatex.egg-info/requires.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)       10 2023-06-05 20:18:59.000000 nrpylatex-1.3.post1/nrpylatex.egg-info/top_level.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)       38 2023-06-05 20:18:59.751320 nrpylatex-1.3.post1/setup.cfg
+-rw-r--r--   0 ksible   (240660) campus    (1313)     1155 2023-06-05 19:01:23.000000 nrpylatex-1.3.post1/setup.py
```

### Comparing `nrpylatex-1.3/LICENSE` & `nrpylatex-1.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/PKG-INFO` & `nrpylatex-1.3.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrpylatex
-Version: 1.3
+Version: 1.3.post1
 Summary: LaTeX Interface to SymPy (CAS) for General Relativity
 Home-page: https://github.com/zachetienne/nrpylatex
 Author: Ken Sible
 Author-email: ksible@outlook.com
 License: BSD License (BSD)
 Keywords: General Relativity,LaTeX,CAS
 Classifier: Operating System :: OS Independent
@@ -19,16 +19,16 @@
 License-File: LICENSE
 
 [![NRPyLaTeX Logo](https://raw.githubusercontent.com/zachetienne/nrpylatex/main/docs/imgs/logo.png)](https://zachetienne.github.io/nrpylatex/)
 
 ---
 
 [![CI](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml/badge.svg)](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
 [![PyPI](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2111.05861-B31B1B)](https://arxiv.org/abs/2111.05861)
 
 [NRPy+](https://github.com/zachetienne/nrpytutorial)'s LaTeX Interface to SymPy (CAS) for General Relativity
 
 - automatic expansion of
   - [Einstein summation convention](https://en.wikipedia.org/wiki/Einstein_notation)
   - Levi-Civita and Christoffel symbols
```

### Comparing `nrpylatex-1.3/README.md` & `nrpylatex-1.3.post1/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![NRPyLaTeX Logo](https://raw.githubusercontent.com/zachetienne/nrpylatex/main/docs/imgs/logo.png)](https://zachetienne.github.io/nrpylatex/)
 
 ---
 
 [![CI](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml/badge.svg)](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
 [![PyPI](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2111.05861-B31B1B)](https://arxiv.org/abs/2111.05861)
 
 [NRPy+](https://github.com/zachetienne/nrpytutorial)'s LaTeX Interface to SymPy (CAS) for General Relativity
 
 - automatic expansion of
   - [Einstein summation convention](https://en.wikipedia.org/wiki/Einstein_notation)
   - Levi-Civita and Christoffel symbols
```

### Comparing `nrpylatex-1.3/nrpylatex/core/generator.py` & `nrpylatex-1.3.post1/nrpylatex/core/generator.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex/core/parser.py` & `nrpylatex-1.3.post1/nrpylatex/core/parser.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex/core/scanner.py` & `nrpylatex-1.3.post1/nrpylatex/core/scanner.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex/parse_latex.py` & `nrpylatex-1.3.post1/nrpylatex/parse_latex.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex/tests/test_parse_latex.py` & `nrpylatex-1.3.post1/nrpylatex/tests/test_parse_latex.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex/utils/assertion.py` & `nrpylatex-1.3.post1/nrpylatex/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex/utils/exceptions.py` & `nrpylatex-1.3.post1/nrpylatex/utils/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """ NRPyLaTeX Exceptions """
 # Author: Ken Sible
 # Email:  ksible *at* outlook *dot* com
 
-import sys
-
 class NRPyLaTeXError(Exception):
 
     def __init__(self, message, sentence=None, position=None):
         if position is not None:
             length = 0
             for _, substring in enumerate(sentence.split('\n')):
                 if position - length <= len(substring):
                     sentence = substring.lstrip()
                     position += len(sentence) - len(substring) - length
                     break
                 length += len(substring) + 1
-            sys.stderr.write('  %s\n%s^\n' % (sentence, (position + 2) * ' '))
-        super(NRPyLaTeXError, self).__init__(message)
+            super(NRPyLaTeXError, self).__init__(message
+                + '\n  %s\n%s^' % (sentence, (position + 2) * ' '))
+        else:
+            super(NRPyLaTeXError, self).__init__(message)
 
 class NamespaceError(Exception):
     """ Illegal Namespace Import """
```

### Comparing `nrpylatex-1.3/nrpylatex/utils/functional.py` & `nrpylatex-1.3.post1/nrpylatex/utils/functional.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex/utils/structures.py` & `nrpylatex-1.3.post1/nrpylatex/utils/structures.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/nrpylatex.egg-info/PKG-INFO` & `nrpylatex-1.3.post1/nrpylatex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrpylatex
-Version: 1.3
+Version: 1.3.post1
 Summary: LaTeX Interface to SymPy (CAS) for General Relativity
 Home-page: https://github.com/zachetienne/nrpylatex
 Author: Ken Sible
 Author-email: ksible@outlook.com
 License: BSD License (BSD)
 Keywords: General Relativity,LaTeX,CAS
 Classifier: Operating System :: OS Independent
@@ -19,16 +19,16 @@
 License-File: LICENSE
 
 [![NRPyLaTeX Logo](https://raw.githubusercontent.com/zachetienne/nrpylatex/main/docs/imgs/logo.png)](https://zachetienne.github.io/nrpylatex/)
 
 ---
 
 [![CI](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml/badge.svg)](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
 [![PyPI](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2111.05861-B31B1B)](https://arxiv.org/abs/2111.05861)
 
 [NRPy+](https://github.com/zachetienne/nrpytutorial)'s LaTeX Interface to SymPy (CAS) for General Relativity
 
 - automatic expansion of
   - [Einstein summation convention](https://en.wikipedia.org/wiki/Einstein_notation)
   - Levi-Civita and Christoffel symbols
```

### Comparing `nrpylatex-1.3/nrpylatex.egg-info/SOURCES.txt` & `nrpylatex-1.3.post1/nrpylatex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.3/setup.py` & `nrpylatex-1.3.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # HERE = pathlib.Path(__file__).parent
 # README = (HERE / "README.md").read_text()
 with open('README.md') as README:
     long_description = README.read()
 
 setup(
     name="nrpylatex",
-    version="1.3",
+    version="1.3.post1",
     description="LaTeX Interface to SymPy (CAS) for General Relativity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zachetienne/nrpylatex",
     author="Ken Sible",
     author_email="ksible@outlook.com",
     license="BSD License (BSD)",
```

