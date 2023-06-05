# Comparing `tmp/atpublic-3.1.2.tar.gz` & `tmp/atpublic-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atpublic-3.1.2.tar", last modified: Thu Jun  1 05:03:42 2023, max compression
+gzip compressed data, was "atpublic-4.0.tar", last modified: Mon Jun  5 19:41:14 2023, max compression
```

## Comparing `atpublic-3.1.2.tar` & `atpublic-4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      556 2023-06-01 05:03:16.165251 atpublic-3.1.2/LICENSE
--rw-r--r--   0        0        0      721 2023-06-01 05:03:16.165251 atpublic-3.1.2/README.rst
--rw-r--r--   0        0        0     3304 2023-06-01 05:03:16.166251 atpublic-3.1.2/conftest.py
--rw-r--r--   0        0        0     3148 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/NEWS.rst
--rw-r--r--   0        0        0        0 2023-06-01 05:03:16.189250 atpublic-3.1.2/docs/__init__.py
--rw-r--r--   0        0        0      175 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/apiref.rst
--rw-r--r--   0        0        0     7326 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/conf.py
--rw-r--r--   0        0        0     2250 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/index.rst
--rw-r--r--   0        0        0     8020 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/using.rst
--rw-r--r--   0        0        0     2852 2023-06-01 05:03:42.619331 atpublic-3.1.2/pyproject.toml
--rw-r--r--   0        0        0      509 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/__init__.py
--rw-r--r--   0        0        0      759 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/private.py
--rw-r--r--   0        0        0     3057 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/public.py
--rw-r--r--   0        0        0        0 2023-06-01 05:03:16.189250 atpublic-3.1.2/src/public/py.typed
--rw-r--r--   0        0        0      107 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/types.py
--rw-r--r--   0        0        0        0 2023-06-01 05:03:16.189250 atpublic-3.1.2/test/__init__.py
--rw-r--r--   0        0        0      204 2023-06-01 05:03:16.167251 atpublic-3.1.2/test/test_mypy.py
--rw-r--r--   0        0        0      923 2023-06-01 05:03:16.167251 atpublic-3.1.2/test/test_private.py
--rw-r--r--   0        0        0     3104 2023-06-01 05:03:16.167251 atpublic-3.1.2/test/test_public.py
--rw-r--r--   0        0        0      780 2023-06-01 05:03:16.167251 atpublic-3.1.2/tox.ini
--rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 atpublic-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0      556 2023-06-05 19:40:47.993511 atpublic-4.0/LICENSE
+-rw-r--r--   0        0        0      721 2023-06-05 19:40:47.993511 atpublic-4.0/README.rst
+-rw-r--r--   0        0        0     3439 2023-06-05 19:40:47.993511 atpublic-4.0/conftest.py
+-rw-r--r--   0        0        0     3810 2023-06-05 19:40:47.993511 atpublic-4.0/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-06-05 19:40:48.021511 atpublic-4.0/docs/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-05 19:40:47.993511 atpublic-4.0/docs/apiref.rst
+-rw-r--r--   0        0        0     7326 2023-06-05 19:40:47.993511 atpublic-4.0/docs/conf.py
+-rw-r--r--   0        0        0     2250 2023-06-05 19:40:47.993511 atpublic-4.0/docs/index.rst
+-rw-r--r--   0        0        0     8667 2023-06-05 19:40:47.993511 atpublic-4.0/docs/using.rst
+-rw-r--r--   0        0        0     2902 2023-06-05 19:41:14.937368 atpublic-4.0/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-06-05 19:40:47.994511 atpublic-4.0/src/public/__init__.py
+-rw-r--r--   0        0        0      760 2023-06-05 19:40:47.994511 atpublic-4.0/src/public/private.py
+-rw-r--r--   0        0        0     3741 2023-06-05 19:40:47.994511 atpublic-4.0/src/public/public.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:40:48.022511 atpublic-4.0/src/public/py.typed
+-rw-r--r--   0        0        0      107 2023-06-05 19:40:47.994511 atpublic-4.0/src/public/types.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:40:48.022511 atpublic-4.0/test/__init__.py
+-rw-r--r--   0        0        0      204 2023-06-05 19:40:47.994511 atpublic-4.0/test/test_mypy.py
+-rw-r--r--   0        0        0      923 2023-06-05 19:40:47.994511 atpublic-4.0/test/test_private.py
+-rw-r--r--   0        0        0     2978 2023-06-05 19:40:47.994511 atpublic-4.0/test/test_public.py
+-rw-r--r--   0        0        0      764 2023-06-05 19:40:47.994511 atpublic-4.0/tox.ini
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 atpublic-4.0/PKG-INFO
```

### Comparing `atpublic-3.1.2/LICENSE` & `atpublic-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.2/README.rst` & `atpublic-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.2/conftest.py` & `atpublic-4.0/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,19 @@
         # same list object here.
         #
         # There is some further discussion in this Sybil ticket:
         # https://github.com/cjw296/sybil/issues/21
         self._testmod = ModuleType('testmod')
         namespace['__name__'] = self._testmod.__name__
         sys.modules[self._testmod.__name__] = self._testmod
-        self._testmod.__all__ = namespace['__all__'] = []
+        # Used in the doctests to provide a clean __all__.
+        def reset():
+            self._testmod.__all__ = namespace['__all__'] = []
+        reset()
+        namespace['reset'] = reset
 
     def teardown(self, namespace):
         del sys.modules[self._testmod.__name__]
 
 
 namespace = DoctestNamespace()
```

### Comparing `atpublic-3.1.2/docs/NEWS.rst` & `atpublic-4.0/docs/NEWS.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 ==================
 @public change log
 ==================
 
+4.0 (2023-06-05)
+================
+* Drop Python 3.7 support (GL#16)
+* Remove ``public.install()`` which was used to inject the ``public`` and
+  ``private`` functions into the ``builtins`` namespace.  This isn't very
+  helpful and could be actively harmful.  Explicit is better than
+  implicit. (GL#14)
+* The functional form of ``public()`` now returns the argument *values* in the
+  order they are given.  This allows you to explicitly bind those values to
+  names in the global namespace.  While this is redundant, it does solve some
+  linter problems.  (GL#12)
+* Switch from ``flake8`` and ``isort`` to ``ruff`` for code quality. (GL#32)
+* Bump dependencies.
+
 3.1.2 (2023-05-31)
 ==================
 * Switch to ``pdm-backend`` (GL#15)
 * Bump dependencies.
 * More GitLab CI integration improvements.
 
 3.1.1 (2022-09-02)
```

### Comparing `atpublic-3.1.2/docs/conf.py` & `atpublic-4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,34 @@
 import sys, os
 from datetime import date
 import importlib.metadata
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+sys.path.insert(0, os.path.abspath('../src'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
-    'sphinx_autodoc_typehints',
     ]
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/', None),
     }
 
+autodoc_typehints = 'both'
+
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
```

### Comparing `atpublic-3.1.2/docs/index.rst` & `atpublic-4.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 provides a top-level module named ``public``, the PyPI package is called
 ``atpublic`` due to name conflicts.
 
 
 Requirements
 ============
 
-``public`` requires Python 3.7 or newer.
+``public`` requires Python 3.8 or newer.
 
 
 Documentation
 =============
 
 A `simple guide`_ to using the library is available, along with a detailed
 `API reference`_.
```

### Comparing `atpublic-3.1.2/docs/using.rst` & `atpublic-4.0/docs/using.rst`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 And that's the second purpose of ``__all__``; it serves as module
 documentation, explicitly naming the public objects it wants to export.  You
 can print a module's ``__all__`` and get an explicit declaration of its public
 API.
 
 
-The problem
-===========
+The problem with __all__
+========================
 
 ``__all__`` has two problems.
 
 First, it separates the declaration of a name's public export semantics from
 the implementation of that name.  Usually the ``__all__`` is put at the top of
 the module, although this isn't required, and in some cases it's `actively
 prohibited`_.  So when you're looking at the definition of a function or class
@@ -83,102 +83,122 @@
     >>> print(__all__)
     ['foo', 'Bar']
 
 Note that you do not need to initialize ``__all__`` in the module, since
 ``public`` will do it for you.  Of course, if your module *already* has an
 ``__all__``, it will add any new names to the existing list.
 
+
+Function call form
+==================
+
 The requirements to use the ``@public`` decorator are simple: the decorated
 thing must have a ``__name__`` attribute.  Since you'll overwhelmingly use it
 to decorate functions and classes, this will always be the case.  If the
 object has a ``__module__`` attribute, that string is used to look up the
 module object in ``sys.modules``, otherwise the module is extracted from the
 globals where the decorator is called.
 
 There's one other common use case that isn't covered by the ``@public``
 decorator.  Sometimes you want to declare simple constants or instances as
 publicly available.  You can't use the ``@public`` decorator for two reasons:
 constants don't have a ``__name__`` and Python's syntax doesn't allow you to
 decorate such constructs.
 
 To solve this use case, ``public`` is also a callable function accepting
-keyword arguments.  An example makes this obvious::
+keyword arguments.  An example makes this obvious.  We'll start by resetting
+the ``__all__``.
 
+    >>> reset()
     >>> public(SEVEN=7)
+    7
     >>> public(a_bar=Bar())
+    <...Bar object ...>
 
 The module's ``__all__`` now contains both of the keys::
 
     >>> print(__all__)
-    ['foo', 'Bar', 'SEVEN', 'a_bar']
+    ['SEVEN', 'a_bar']
 
 and as should be obvious, the module contains name bindings for these
 constants::
 
     >>> print(SEVEN)
     7
     >>> print(a_bar)
     <....Bar object at ...>
 
 Multiple keyword arguments are allowed::
 
     >>> public(ONE=1, TWO=2)
+    (1, 2)
     >>> print(__all__)
-    ['foo', 'Bar', 'SEVEN', 'a_bar', 'ONE', 'TWO']
+    ['SEVEN', 'a_bar', 'ONE', 'TWO']
 
     >>> print(ONE)
     1
     >>> print(TWO)
     2
 
+You'll notice that the functional form of ``public()`` returns the values in
+its keyword arguments in order.  This is to help with a use case where some
+linters complain bcause they can't see that ``public()`` binds the names in
+the global namespace.  In the above example they might report erroneously that
+``ONE`` and ``TWO`` aren't defined.  To work around this, when ``public()`` is
+used in its functional form, it will return the values in the order they are
+seen [#]_ and you can simply assign them to explicit local variable names.
+
+    >>> a, b, c = public(a=3, b=2, c=1)
+    >>> print(__all__)
+    ['SEVEN', 'a_bar', 'ONE', 'TWO', 'a', 'b', 'c']
+    >>> print(a, b, c)
+    3 2 1
+
+It also works if you bind only a single value.
+
+    >>> d = public(d=9)
+    >>> print(__all__)
+    ['SEVEN', 'a_bar', 'ONE', 'TWO', 'a', 'b', 'c', 'd']
+    >>> print(d)
+    9
+
 
 @private
 ========
 
 You might also want to be explicit about your private, i.e. non-public names.
 This library also provides an ``@private`` decorator for this purpose.  While
 it mostly serves for documentation purposes, this decorator also ensures that
-the decorated object's name does *not* appear in the ``__all__``::
+the decorated object's name does *not* appear in the ``__all__``.  As above,
+we'll start by resetting ``__all__``::
 
+    >>> reset()
     >>> from public import private
 
     >>> @private
     ... def foo():
     ...    pass
 
     >>> print(__all__)
-    ['Bar', 'SEVEN', 'a_bar', 'ONE', 'TWO']
+    []
 
 You can see here that ``foo`` has been removed from the ``__all__``.  It's
 okay if the name doesn't appear in ``__all__`` at all::
 
     >>> @private
     ... class Baz:
     ...     pass
 
     >>> print(__all__)
-    ['Bar', 'SEVEN', 'a_bar', 'ONE', 'TWO']
+    []
 
 In this case, ``Baz`` never appears in ``__all__``.  Like with ``@public``,
-the ``@private`` decorator will add any missing ``__all__``, but if it exists
-in the module, it must be a list.  There is no functional API for ``@private``.
-
-
-Making @public and @private built-ins
-=====================================
-
-It can get rather tedious if you have to add the above import in every module
-where you want to use it.  What if you could put ``public`` into Python's
-builtins_?  Then it would be available in all your code for free::
-
-    >>> from public import install
-    >>> install()
-
-and now you can just use ``@public`` and ``@private`` without having to import
-anything in your other modules.
+the ``@private`` decorator will initialize ``__all__`` if needed, but if it
+exists in the module, it must be a list.  There is no functional API for
+``@private``.
 
 
 Caveats
 =======
 
 There are some important usage restrictions you should be aware of:
 
@@ -206,14 +226,18 @@
 others.  This package:
 
 * uses keyword arguments to map names which don't have an ``__name__``
   attribute;
 * can be used to bind names and values into a module's globals;
 * can optionally put ``public`` in builtins.
 
+.. rubric:: Footnotes
+
+.. [#] This is ordering is guaranteed by `PEP 468 <https://peps.python.org/pep-0468/>`_.
+
 
 .. _`issue 26632`: http://bugs.python.org/issue26632
 .. _builtins: https://docs.python.org/3/library/builtins.html
 .. _`directly controls`: https://docs.python.org/3/tutorial/modules.html#importing-from-a-package
 .. _`actively prohibited`: http://pep8.readthedocs.io/en/latest/intro.html?highlight=e402#error-codes
 .. _`out of sync`: http://bugs.python.org/issue23883
 .. _Other: https://pypi.python.org/pypi/public
```

### Comparing `atpublic-3.1.2/pyproject.toml` & `atpublic-4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "atpublic"
 authors = [
     { name = "Barry Warsaw", email = "barry@python.org" },
 ]
 description = "Keep all y'all's __all__'s in sync"
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "__all__",
     "public",
     "private",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -23,27 +23,25 @@
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 dependencies = []
 dynamic = []
-version = "3.1.2"
+version = "4.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://public.readthedocs.io"
 Documentation = "https://public.readthedocs.io"
 Source = "https://gitlab.com/warsaw/public.git"
 "Bug Tracker" = "https://gitlab.com/warsaw/public/issues"
 
-[project.optional-dependencies]
-
 [tool.pdm.version]
 source = "file"
 path = "src/public/__init__.py"
 
 [tool.pdm.build]
 source-includes = [
     "docs/",
@@ -60,22 +58,20 @@
     "coverage[toml]",
     "diff-cover",
     "pytest",
     "pytest-cov",
     "sybil",
 ]
 qa = [
-    "flake8",
-    "isort",
+    "ruff",
     "mypy",
     "blue",
 ]
 docs = [
     "sphinx",
-    "sphinx-autodoc-typehints",
     "furo",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=public --cov-report=term --cov-report=xml -p no:doctest"
 testpaths = "test docs"
 
@@ -83,25 +79,44 @@
 fail_under = 100
 show_missing = true
 
 [tool.coverage.run]
 branch = true
 parallel = true
 
-[tool.isort]
-include_trailing_comma = true
-known_first_party = "public"
-length_sort_straight = true
-lines_after_imports = 2
-lines_between_types = 1
-multi_line_output = 3
-order_by_type = false
-skip = [
-    "conf.py",
+[tool.ruff]
+line-length = 79
+src = [
+    "src",
+]
+select = [
+    "B",
+    "D",
+    "E",
+    "F",
+    "I",
+    "RUF100",
+    "UP",
+    "W",
+]
+ignore = [
+    "D100",
+    "D104",
+]
+
+[tool.ruff.pydocstyle]
+convention = "pep257"
+
+[tool.ruff.isort]
+known-first-party = [
+    "public",
 ]
+lines-after-imports = 2
+lines-between-types = 1
+order-by-type = true
 
 [tool.mypy]
 mypy_path = "src"
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = false
 disallow_untyped_defs = true
```

### Comparing `atpublic-3.1.2/src/public/private.py` & `atpublic-4.0/src/public/private.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from .types import ModuleAware
 
 
 def private(thing: ModuleAware) -> ModuleAware:
-    """Remove names from __all__
+    """Remove names from __all__.
 
     This decorator documents private names and ensures that the names do not
     appear in the module's __all__.
 
     :param thing: An object with both a __module__ and a __name__ argument.
     :return: The original `thing` object.
     :raises ValueError: When this function finds a non-list __all__ attribute.
```

### Comparing `atpublic-3.1.2/src/public/public.py` & `atpublic-4.0/src/public/public.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 import sys
 
-from typing import Any, overload
+
+# Tuple can go away in Python >= 3.9
+# Union can go away in Python >= 3.10
+from typing import Any, Tuple, Union, overload
 
 from .types import ModuleAware
 
 
 @overload
 def public(thing: ModuleAware) -> ModuleAware:
     ...                                           # pragma: no cover
 
 
 @overload
-def public(**kws: Any) -> None:
+def public(**kws: Any) -> Union[Any, Tuple[Any]]:
     ...                                           # pragma: no cover
 
 
 def public(thing=None, **kws):                    # type: ignore
-    """Add a name or names to __all__
+    """Add a name or names to __all__.
 
     There are two forms of use for this function.  Most commonly it will
     be used as a decorator on a class or function at module scope.  In
-    this case, `thing` will be an object with both __module__ and
-    __name__ attributes, and the name is added to the module's __all__
-    list, creating that if necessary.
-
-    When used in its function call form, `thing` will be None.  __all__
-    is looked up in the globals at the function's call site, and each
-    key in the keyword arguments is added to the __all__.  In addition,
-    the key will be bound to the value in the globals.
+    this case, ``thing`` will be an object with both ``__module__`` and
+    ``__name__`` attributes, and the name is added to the module's
+    ``__all__`` list, creating that if necessary.
+
+    When used in its function call form, ``thing`` will be None.  ``__all__``
+    is looked up in the globals at the function's call site, and each key in
+    the keyword arguments is added to the ``__all__``.  In addition, the key
+    will be bound to the value in the globals.  This form returns the keyword
+    argument values in order.  If only a single keyword argument is given, its
+    value is return, otherwise a tuple of the values is returned.
 
     Only one or the other format may be used.
 
     :param thing: None, or an object with both a __module__ and a __name__
         argument.
     :param kws: Keyword arguments.
-    :return: The original `thing` object.
+    :return: In the decorator form, the original ``thing`` object is
+        returned.  In the functional form, the keyword argument value is
+        returned if only a single keyword argument is given, otherwise a
+        tuple of the keyword argument values is returned.
     :raises ValueError: When the inputs are invalid, or this function finds
-        a non-list __all__ attribute.
+        a non-list ``__all__`` attribute.
     """
     # 2020-07-14(warsaw): I considered using inspect.getmodule() here but
     # looking at its implementation, I feel like it does a ton of unnecessary
     # work in the oddball cases (i.e. where the object does not have an
     # __module__ attribute).  Because @public runs at module import time, and
     # because I'm not really sure we even want to support those oddball cases,
     # I'm taking the more straightforward approach of just looking the module
@@ -53,20 +61,25 @@
         else sys.modules[thing.__module__].__dict__
     )
     dunder_all = mdict.setdefault('__all__', [])
     if not isinstance(dunder_all, list):
         raise ValueError(f'__all__ must be a list not: {type(dunder_all)}')
     if thing is None:
         # The function call form.
+        retval = []
         for key, value in kws.items():
             # This overwrites any previous similarly named __all__ entry.
             if key not in dunder_all:
                 dunder_all.append(key)
             # We currently do not check for duplications in the globals.
             mdict[key] = value
+            retval.append(value)
+        if len(retval) == 1:
+            return retval[0]
+        return tuple(retval)
     else:
         # I think it's impossible to use the @public decorator and pass in
         # keyword arguments.  Not quite syntactically impossible, but you'll
         # get a TypeError if you try it, before you even get to this code.
         assert (
             len(kws) == 0
         ), 'Keyword arguments are incompatible with use as decorator'
```

### Comparing `atpublic-3.1.2/test/test_private.py` & `atpublic-4.0/test/test_private.py`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.2/test/test_public.py` & `atpublic-4.0/test/test_public.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import builtins
 
 from importlib import import_module
 
 import pytest
 
-from public import install
-
 
 def test_atpublic_function(example):
     example("""\
 from public import public
 
 @public
 def a_function():
@@ -188,14 +186,7 @@
 
 @public
 def bar():
     pass
 """)
     with pytest.raises(ValueError):
         import_module('example')
-
-
-def test_install():
-    try:
-        install()
-    finally:
-        delattr(builtins, 'public')
```

### Comparing `atpublic-3.1.2/tox.ini` & `atpublic-4.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py{37,38,39,310,311},qa,docs
+envlist = py{38,39,310,311},qa,docs
 skip_missing_interpreters = true
 isolated_build = true
 
 [testenv]
 allowlist_externals = pdm
 setenv =
     PDM_IGNORE_SAVED_PYTHON="1"
@@ -17,22 +17,21 @@
     # The following is only useful in a git repository.
     -diff-cover coverage.xml
 usedevelop = true
 
 [testenv:qa]
 commands =
     pdm install -G qa
-    flake8 {env:MODULE_PATH}
-    isort {env:MODULE_PATH}
+    ruff check {env:MODULE_PATH}
     blue --check {env:MODULE_PATH}
     mypy -p {env:MODULE_NAME}
 
 [testenv:fixit]
 commands =
     pdm install -G qa
-    isort {env:MODULE_PATH}
+    ruff check --fix {env:MODULE_PATH}
     blue {env:MODULE_PATH}
 
 [testenv:docs]
 commands =
     pdm install -G docs
     sphinx-build docs build/html
```

### Comparing `atpublic-3.1.2/PKG-INFO` & `atpublic-4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atpublic
-Version: 3.1.2
+Version: 4.0
 Summary: Keep all y'all's __all__'s in sync
 Keywords: __all__ public private
 Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Project-URL: Home page, https://public.readthedocs.io
 Project-URL: Documentation, https://public.readthedocs.io
 Project-URL: Source, https://gitlab.com/warsaw/public.git
 Project-URL: Bug tracker, https://gitlab.com/warsaw/public/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 ======================
  @public and @private
 ======================
 
 This library provides two very simple decorators that document the
```

