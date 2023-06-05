# Comparing `tmp/pylogics-0.1.1.tar.gz` & `tmp/pylogics-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogics-0.1.1.tar", last modified: Sat Sep 25 14:03:06 2021, max compression
+gzip compressed data, was "pylogics-0.2.0.tar", max compression
```

## Comparing `pylogics-0.1.1.tar` & `pylogics-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     7652 2021-06-07 20:04:32.466048 pylogics-0.1.1/LICENSE
--rw-r--r--   0        0        0     2701 2021-09-25 14:00:26.173235 pylogics-0.1.1/README.md
--rw-r--r--   0        0        0      872 2021-09-25 14:00:26.177235 pylogics-0.1.1/pylogics/__init__.py
--rw-r--r--   0        0        0     1057 2021-06-07 20:04:32.502049 pylogics-0.1.1/pylogics/exceptions.py
--rw-r--r--   0        0        0      833 2021-06-07 20:04:32.506049 pylogics-0.1.1/pylogics/helpers/__init__.py
--rw-r--r--   0        0        0     3209 2021-06-07 20:04:32.506049 pylogics-0.1.1/pylogics/helpers/cache_hash.py
--rw-r--r--   0        0        0     3921 2021-06-07 20:04:32.510049 pylogics-0.1.1/pylogics/helpers/misc.py
--rw-r--r--   0        0        0     1011 2021-06-07 20:04:32.510049 pylogics-0.1.1/pylogics/parsers/__init__.py
--rw-r--r--   0        0        0     3561 2021-06-07 20:04:32.514049 pylogics-0.1.1/pylogics/parsers/base.py
--rw-r--r--   0        0        0     1838 2021-06-07 20:04:32.514049 pylogics-0.1.1/pylogics/parsers/ldl.lark
--rw-r--r--   0        0        0     6002 2021-09-25 14:00:26.177235 pylogics-0.1.1/pylogics/parsers/ldl.py
--rw-r--r--   0        0        0     1873 2021-06-07 20:04:32.518049 pylogics-0.1.1/pylogics/parsers/ltl.lark
--rw-r--r--   0        0        0     4476 2021-06-07 20:04:32.518049 pylogics-0.1.1/pylogics/parsers/ltl.py
--rw-r--r--   0        0        0      823 2021-06-07 20:04:32.522049 pylogics-0.1.1/pylogics/parsers/pl.lark
--rw-r--r--   0        0        0     3216 2021-06-07 20:04:32.522049 pylogics-0.1.1/pylogics/parsers/pl.py
--rw-r--r--   0        0        0     1665 2021-06-07 20:04:32.526049 pylogics-0.1.1/pylogics/parsers/pltl.lark
--rw-r--r--   0        0        0     4008 2021-06-07 20:04:32.526049 pylogics-0.1.1/pylogics/parsers/pltl.py
--rw-r--r--   0        0        0      842 2021-06-07 20:04:32.530049 pylogics-0.1.1/pylogics/semantics/__init__.py
--rw-r--r--   0        0        0     2835 2021-06-07 20:04:32.530049 pylogics-0.1.1/pylogics/semantics/base.py
--rw-r--r--   0        0        0     3501 2021-06-07 20:04:32.530049 pylogics-0.1.1/pylogics/semantics/pl.py
--rw-r--r--   0        0        0      837 2021-06-07 20:04:32.534049 pylogics-0.1.1/pylogics/syntax/__init__.py
--rw-r--r--   0        0        0    19685 2021-09-25 14:00:26.181234 pylogics-0.1.1/pylogics/syntax/base.py
--rw-r--r--   0        0        0     4190 2021-06-07 20:04:32.538049 pylogics-0.1.1/pylogics/syntax/ldl.py
--rw-r--r--   0        0        0     3591 2021-06-07 20:04:32.538049 pylogics-0.1.1/pylogics/syntax/ltl.py
--rw-r--r--   0        0        0     1040 2021-06-07 20:04:32.542049 pylogics-0.1.1/pylogics/syntax/pl.py
--rw-r--r--   0        0        0     3293 2021-06-07 20:04:32.542049 pylogics-0.1.1/pylogics/syntax/pltl.py
--rw-r--r--   0        0        0      797 2021-06-07 20:04:32.542049 pylogics-0.1.1/pylogics/utils/__init__.py
--rw-r--r--   0        0        0     7881 2021-06-07 20:04:32.546049 pylogics-0.1.1/pylogics/utils/to_string.py
--rw-r--r--   0        0        0     1963 2021-09-25 14:00:26.181234 pylogics-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3598 2021-09-25 14:03:06.536026 pylogics-0.1.1/setup.py
--rw-r--r--   0        0        0     3852 2021-09-25 14:03:06.536264 pylogics-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-05 17:30:04.142063 pylogics-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2701 2023-06-05 17:30:04.142063 pylogics-0.2.0/README.md
+-rw-r--r--   0        0        0      872 2023-06-05 17:30:04.142063 pylogics-0.2.0/pylogics/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-05 17:30:04.142063 pylogics-0.2.0/pylogics/exceptions.py
+-rw-r--r--   0        0        0      833 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/helpers/__init__.py
+-rw-r--r--   0        0        0     3209 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/helpers/cache_hash.py
+-rw-r--r--   0        0        0     3921 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/helpers/misc.py
+-rw-r--r--   0        0        0     1011 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/__init__.py
+-rw-r--r--   0        0        0     3561 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/base.py
+-rw-r--r--   0        0        0     1838 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ldl.lark
+-rw-r--r--   0        0        0     6002 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ldl.py
+-rw-r--r--   0        0        0     1993 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ltl.lark
+-rw-r--r--   0        0        0     4476 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ltl.py
+-rw-r--r--   0        0        0     1515 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pl.lark
+-rw-r--r--   0        0        0     3216 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pl.py
+-rw-r--r--   0        0        0     1655 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pltl.lark
+-rw-r--r--   0        0        0     3923 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pltl.py
+-rw-r--r--   0        0        0      842 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/semantics/__init__.py
+-rw-r--r--   0        0        0     2835 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/semantics/base.py
+-rw-r--r--   0        0        0     3501 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/semantics/pl.py
+-rw-r--r--   0        0        0      837 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/__init__.py
+-rw-r--r--   0        0        0    20222 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/base.py
+-rw-r--r--   0        0        0     4190 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/ldl.py
+-rw-r--r--   0        0        0     3591 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/ltl.py
+-rw-r--r--   0        0        0     1040 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/pl.py
+-rw-r--r--   0        0        0     3231 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/pltl.py
+-rw-r--r--   0        0        0      797 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/utils/__init__.py
+-rw-r--r--   0        0        0     7881 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/utils/to_string.py
+-rw-r--r--   0        0        0     2111 2023-06-05 17:30:04.146062 pylogics-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3897 1970-01-01 00:00:00.000000 pylogics-0.2.0/PKG-INFO
```

### Comparing `pylogics-0.1.1/LICENSE` & `pylogics-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/README.md` & `pylogics-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/__init__.py` & `pylogics-0.2.0/pylogics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with pylogics.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 """A Python library for logic formalisms representation and manipulation."""
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
```

### Comparing `pylogics-0.1.1/pylogics/exceptions.py` & `pylogics-0.2.0/pylogics/exceptions.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/helpers/__init__.py` & `pylogics-0.2.0/pylogics/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/helpers/cache_hash.py` & `pylogics-0.2.0/pylogics/helpers/cache_hash.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/helpers/misc.py` & `pylogics-0.2.0/pylogics/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/parsers/__init__.py` & `pylogics-0.2.0/pylogics/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/parsers/base.py` & `pylogics-0.2.0/pylogics/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/parsers/ldl.lark` & `pylogics-0.2.0/pylogics/parsers/ldl.lark`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/parsers/ldl.py` & `pylogics-0.2.0/pylogics/parsers/ldl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/parsers/ltl.py` & `pylogics-0.2.0/pylogics/parsers/ltl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/parsers/pl.py` & `pylogics-0.2.0/pylogics/parsers/pl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/parsers/pltl.lark` & `pylogics-0.2.0/pylogics/parsers/pltl.lark`

 * *Files 25% similar despite different names*

```diff
@@ -21,29 +21,27 @@
              |       LEFT_PARENTHESIS pltlf_formula RIGHT_PARENTHESIS
 ?pltlf_atom:       pltlf_symbol
            |       pltlf_true
            |       pltlf_false
            |       pltlf_tt
            |       pltlf_ff
            |       pltlf_start
-           |       pltlf_first
 
 pltlf_symbol: SYMBOL_NAME
 pltlf_true: prop_true
 pltlf_false: prop_false
 pltlf_tt: TT
 pltlf_ff: FF
 pltlf_start: START
-pltlf_first: FIRST
 
 // Operators must not be part of a word
-SINCE.2: "S"
-HISTORICALLY.2: "H"
-ONCE.2: "O"
-BEFORE.2: "Y"
+SINCE.2: /S(?=[ "\(])/
+HISTORICALLY.2: /H(?=[ "\(])/
+ONCE.2: /O(?=[ "\(])/
+BEFORE.2: /Y(?=[ "\(])/
 FIRST.2: /first/
 START.2: /start/
 
 %ignore /\s+/
 
 %import  .pl.SYMBOL_NAME -> SYMBOL_NAME
 %import  .pl.prop_true -> prop_true
```

### Comparing `pylogics-0.1.1/pylogics/parsers/pltl.py` & `pylogics-0.2.0/pylogics/parsers/pltl.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     Not,
     Or,
     make_boolean,
 )
 from pylogics.syntax.pltl import (
     Atomic,
     Before,
-    First,
     Historically,
     Once,
     PropositionalFalse,
     PropositionalTrue,
     Since,
     Start,
 )
@@ -124,18 +123,14 @@
         return make_boolean(False, logic=Logic.PLTL)
 
     @classmethod
     def pltlf_start(cls, _args):
         return Start()
 
     @classmethod
-    def pltlf_first(cls, _args):
-        return First()
-
-    @classmethod
     def pltlf_symbol(cls, args):
         assert len(args) == 1
         token = args[0]
         symbol = str(token)
         return Atomic(symbol)
```

### Comparing `pylogics-0.1.1/pylogics/semantics/__init__.py` & `pylogics-0.2.0/pylogics/semantics/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/semantics/base.py` & `pylogics-0.2.0/pylogics/semantics/base.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/semantics/pl.py` & `pylogics-0.2.0/pylogics/semantics/pl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/syntax/__init__.py` & `pylogics-0.2.0/pylogics/syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/syntax/base.py` & `pylogics-0.2.0/pylogics/syntax/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,17 +598,31 @@
     :param is_none_true: if true, None reduces to TrueFormula; FalseFormula otherwise.
     :return: the same set, or an empty set if the arg was None.
     """
     return f if f is not None else TrueFormula() if is_none_true else FalseFormula()
 
 
 class AtomName(RegexConstrainedString):
-    """A string that denotes an atomic propositional symbol."""
+    """
+    A string that denotes an atomic propositional symbol.
+
+    Symbols cannot start with uppercase letters, because these are reserved. Moreover, any word between quotes is a
+     symbol.
+
+    More in detail:
+
+    1) either start with [a-z_], followed by at least one [a-zA-Z0-9_-], and by one [a-zA-Z0-9_] (i.e. hyphens only in
+       between);
+    2) or, start with [a-z_] and follows with any sequence of [a-zA-Z0-9_] (no hyphens);
+    3) or, any sequence of ASCII printable characters (i.e. going from ' ' to '~'), except '"'.
+    """
 
-    REGEX = re.compile(r"[A-Za-z][A-Za-z0-9_]*|\"\w+\"")
+    REGEX = re.compile(
+        r"[a-z_]([a-zA-Z0-9_-]+[a-zA-Z0-9_])|[a-z_][a-zA-Z0-9_]*|\"[ -!#-~]+?\""
+    )
 
 
 _AtomNameOrStr = Union[str, AtomName]
 
 
 class AbstractAtomic(Formula, ABC):
     """An abstract atomic proposition."""
```

### Comparing `pylogics-0.1.1/pylogics/syntax/ldl.py` & `pylogics-0.2.0/pylogics/syntax/ldl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/syntax/ltl.py` & `pylogics-0.2.0/pylogics/syntax/ltl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/syntax/pl.py` & `pylogics-0.2.0/pylogics/syntax/pl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/syntax/pltl.py` & `pylogics-0.2.0/pylogics/syntax/pltl.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,9 +129,8 @@
 
 class Historically(_PLTLUnaryOp):
     """The "historically" formula in PLTL."""
 
     SYMBOL = "historically"
 
 
-Start = partial(Historically, FalseFormula(logic=Logic.PLTL))
-First = partial(Not, Before(TrueFormula(logic=Logic.PLTL)))
+Start = partial(Not, Before(TrueFormula(logic=Logic.PLTL)))
```

### Comparing `pylogics-0.1.1/pylogics/utils/__init__.py` & `pylogics-0.2.0/pylogics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pylogics/utils/to_string.py` & `pylogics-0.2.0/pylogics/utils/to_string.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.1.1/pyproject.toml` & `pylogics-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylogics"
-version = "0.1.1"
+version = "0.2.0"
 description = "A Python library for logic formalisms representation and manipulation."
 authors = ["MarcoFavorito <marco.favorito@gmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://whitemech.github.io/pylogics"
 repository = "https://github.com/whitemech/pylogics.git"
 documentation = "https://whitemech.github.io/pylogics"
@@ -16,61 +16,67 @@
 ]
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 #packages = []
 include = []
 
 
 #[tool.poetry.scripts]
 #script_name = 'path/to/script'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/whitemech/pylogics/issues"
 "Pull Requests" = "https://github.com/whitemech/pylogics/pulls"
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
-lark-parser = "^0.11.2"
+python = ">=3.8.1,<4.0"
+lark = "^1.1.5"
 
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.1"
-pytest-cov = "^2.10.1"
-pytest-randomly = "^3.5.0"
-tox = "^3.23.0"
-codecov = "^2.1.11"
-black = "==20.8b1"
-mypy = "^0.812"
-isort = "^5.7.0"
-flake8 = "^3.9.1"
-flake8-docstrings = "^1.5.0"
-flake8-bugbear = "^21.4.3"
-flake8-eradicate = "^1.0.0"
-flake8-isort = "^4.0.0"
-pylint = "^2.6.0"
-safety = "^1.10.1"
-vulture = "^2.1"
-bandit = "^1.7.0"
-mkdocs = "^1.1.2"
-markdown_include = "^0.6.0"
-mkdocs-material = "^7.1.1"
-ipython = "^7.18.1"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+black = "^23.3.0"
+codecov = "^2.1.13"
+flake8-bugbear = "^23.5.9"
+flake8-docstrings = "^1.7.0"
+flake8-eradicate = "^1.5.0"
+flake8-isort = "^6.0.0"
+hypothesis = "^6.76.0"
+hypothesis-pytest = "^0.19.0"
+ipython = "^8.12.2"
+isort = "^5.12.0"
 jupyter = "^1.0.0"
-mknotebooks = "^0.7.0"
 markdown = "^3.3.4"
-twine = "^3.3.0"
-hypothesis = "^6.10.0"
-hypothesis-pytest = "^0.19.0"
-mistune = {version = "^2.0.0-rc.1", allow-prereleases = true}
+markdown-include = "^0.8.1"
+mistune = "^2.0.5"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.15"
+mknotebooks = "^0.7.1"
+mypy = "^1.3.0"
+packaging = "^23.0"
+pylint = "^2.17.4"
+pymdown-extensions = "^10.0.1"
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+pytest-randomly = "^3.12.0"
+safety = "^2.4.0b1"
+toml = "^0.10.2"
+tox = "^4.4.12"
+twine = "^4.0.2"
+types-requests = "^2.31.0.1"
+types-setuptools = "^67.8.0.0"
+types-toml = "^0.10.8.6"
+vulture = "^2.7"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pylogics-0.1.1/PKG-INFO` & `pylogics-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pylogics
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library for logic formalisms representation and manipulation.
 Home-page: https://whitemech.github.io/pylogics
 License: LGPL-3.0-or-later
 Keywords: logic,propositional logic,predicate logic,temporal logic
 Author: MarcoFavorito
 Author-email: marco.favorito@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: lark-parser (>=0.11.2,<0.12.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: lark (>=1.1.5,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/whitemech/pylogics/issues
 Project-URL: Documentation, https://whitemech.github.io/pylogics
 Project-URL: Pull Requests, https://github.com/whitemech/pylogics/pulls
 Project-URL: Repository, https://github.com/whitemech/pylogics.git
 Description-Content-Type: text/markdown
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pylogics Version: 0.1.1 Summary: A Python library
+Metadata-Version: 2.1 Name: pylogics Version: 0.2.0 Summary: A Python library
 for logic formalisms representation and manipulation. Home-page: https://
 whitemech.github.io/pylogics License: LGPL-3.0-or-later Keywords:
 logic,propositional logic,predicate logic,temporal logic Author: MarcoFavorito
-Author-email: marco.favorito@gmail.com Requires-Python: >=3.7,<4.0 Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
-later (LGPLv3+) Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Dist: lark-parser (>=0.11.2,<0.12.0)
-Project-URL: Bug Tracker, https://github.com/whitemech/pylogics/issues Project-
-URL: Documentation, https://whitemech.github.io/pylogics Project-URL: Pull
-Requests, https://github.com/whitemech/pylogics/pulls Project-URL: Repository,
-https://github.com/whitemech/pylogics.git Description-Content-Type: text/
-markdown
+Author-email: marco.favorito@gmail.com Requires-Python: >=3.8.1,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: License :: OSI Approved :: GNU Lesser General Public
+License v3 or later (LGPLv3+) Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.8 Requires-Dist: lark (>=1.1.5,<2.0.0) Project-URL: Bug
+Tracker, https://github.com/whitemech/pylogics/issues Project-URL:
+Documentation, https://whitemech.github.io/pylogics Project-URL: Pull Requests,
+https://github.com/whitemech/pylogics/pulls Project-URL: Repository, https://
+github.com/whitemech/pylogics.git Description-Content-Type: text/markdown
                             ****** PyLogics ******
 [PyPI] [PyPI_-_Python_Version] [PyPI - Status] [PyPI - Implementation] [PyPI -
                                 Wheel] [GitHub]
                         [test] [lint] [docs] [codecov]
                                     [black]
 A Python library for logic formalisms representation and manipulation. ##
 Install To install the package from PyPI: ``` pip install pylogics ``` ## Tests
```

