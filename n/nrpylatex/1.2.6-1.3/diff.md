# Comparing `tmp/nrpylatex-1.2.6.tar.gz` & `tmp/nrpylatex-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrpylatex-1.2.6.tar", last modified: Thu Mar  9 21:20:00 2023, max compression
+gzip compressed data, was "nrpylatex-1.3.tar", last modified: Mon Jun  5 17:51:12 2023, max compression
```

## Comparing `nrpylatex-1.2.6.tar` & `nrpylatex-1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 kensible   (501) staff       (20)        0 2023-03-09 21:20:00.017619 nrpylatex-1.2.6/
--rw-r--r--   0 kensible   (501) staff       (20)     1327 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/LICENSE
--rw-r--r--   0 kensible   (501) staff       (20)     5608 2023-03-09 21:20:00.017473 nrpylatex-1.2.6/PKG-INFO
--rw-r--r--   0 kensible   (501) staff       (20)     4841 2023-03-09 20:59:59.000000 nrpylatex-1.2.6/README.md
-drwxr-xr-x   0 kensible   (501) staff       (20)        0 2023-03-09 21:20:00.014374 nrpylatex-1.2.6/nrpylatex/
--rw-r--r--   0 kensible   (501) staff       (20)      227 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/__init__.py
-drwxr-xr-x   0 kensible   (501) staff       (20)        0 2023-03-09 21:20:00.016514 nrpylatex-1.2.6/nrpylatex/core/
--rw-r--r--   0 kensible   (501) staff       (20)        0 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/core/__init__.py
--rw-r--r--   0 kensible   (501) staff       (20)     4821 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/core/assertion.py
--rw-r--r--   0 kensible   (501) staff       (20)     5100 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/core/exprtree.py
--rw-r--r--   0 kensible   (501) staff       (20)     2555 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/core/functional.py
--rw-r--r--   0 kensible   (501) staff       (20)     9521 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/core/indexed_symbol.py
--rw-r--r--   0 kensible   (501) staff       (20)    89075 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/core/parser.py
--rw-r--r--   0 kensible   (501) staff       (20)     6964 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/core/scanner.py
-drwxr-xr-x   0 kensible   (501) staff       (20)        0 2023-03-09 21:20:00.016876 nrpylatex-1.2.6/nrpylatex/extension/
--rw-r--r--   0 kensible   (501) staff       (20)      133 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/extension/__init__.py
--rw-r--r--   0 kensible   (501) staff       (20)     2580 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/extension/parse_magic.py
--rw-r--r--   0 kensible   (501) staff       (20)     2254 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/parse_latex.py
-drwxr-xr-x   0 kensible   (501) staff       (20)        0 2023-03-09 21:20:00.017198 nrpylatex-1.2.6/nrpylatex/tests/
--rw-r--r--   0 kensible   (501) staff       (20)        0 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/tests/__init__.py
--rw-r--r--   0 kensible   (501) staff       (20)    21148 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/nrpylatex/tests/test_parse_latex.py
-drwxr-xr-x   0 kensible   (501) staff       (20)        0 2023-03-09 21:20:00.015208 nrpylatex-1.2.6/nrpylatex.egg-info/
--rw-r--r--   0 kensible   (501) staff       (20)     5608 2023-03-09 21:19:59.000000 nrpylatex-1.2.6/nrpylatex.egg-info/PKG-INFO
--rw-r--r--   0 kensible   (501) staff       (20)      563 2023-03-09 21:19:59.000000 nrpylatex-1.2.6/nrpylatex.egg-info/SOURCES.txt
--rw-r--r--   0 kensible   (501) staff       (20)        1 2023-03-09 21:19:59.000000 nrpylatex-1.2.6/nrpylatex.egg-info/dependency_links.txt
--rw-r--r--   0 kensible   (501) staff       (20)        6 2023-03-09 21:19:59.000000 nrpylatex-1.2.6/nrpylatex.egg-info/requires.txt
--rw-r--r--   0 kensible   (501) staff       (20)       10 2023-03-09 21:19:59.000000 nrpylatex-1.2.6/nrpylatex.egg-info/top_level.txt
--rw-r--r--   0 kensible   (501) staff       (20)       38 2023-03-09 21:20:00.017665 nrpylatex-1.2.6/setup.cfg
--rw-r--r--   0 kensible   (501) staff       (20)     1155 2023-03-09 20:25:27.000000 nrpylatex-1.2.6/setup.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/
+-rw-r--r--   0 ksible   (240660) campus    (1313)     1327 2022-12-18 22:56:57.000000 nrpylatex-1.3/LICENSE
+-rw-r--r--   0 ksible   (240660) campus    (1313)     5690 2023-06-05 17:51:12.854257 nrpylatex-1.3/PKG-INFO
+-rw-r--r--   0 ksible   (240660) campus    (1313)     4925 2023-06-02 22:29:45.000000 nrpylatex-1.3/README.md
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.850257 nrpylatex-1.3/nrpylatex/
+-rw-r--r--   0 ksible   (240660) campus    (1313)      474 2023-06-02 23:36:58.000000 nrpylatex-1.3/nrpylatex/__init__.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex/core/
+-rw-r--r--   0 ksible   (240660) campus    (1313)        0 2022-12-18 22:56:57.000000 nrpylatex-1.3/nrpylatex/core/__init__.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    18012 2023-06-05 17:15:06.000000 nrpylatex-1.3/nrpylatex/core/generator.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    63993 2023-06-05 17:16:27.000000 nrpylatex-1.3/nrpylatex/core/parser.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     6356 2023-06-05 17:24:12.000000 nrpylatex-1.3/nrpylatex/core/scanner.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     4209 2023-06-05 16:42:18.000000 nrpylatex-1.3/nrpylatex/parse_latex.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex/tests/
+-rw-r--r--   0 ksible   (240660) campus    (1313)        0 2022-12-18 22:56:57.000000 nrpylatex-1.3/nrpylatex/tests/__init__.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    21131 2023-06-05 16:41:31.000000 nrpylatex-1.3/nrpylatex/tests/test_parse_latex.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex/utils/
+-rw-r--r--   0 ksible   (240660) campus    (1313)        0 2023-06-01 17:16:50.000000 nrpylatex-1.3/nrpylatex/utils/__init__.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     4817 2023-06-01 17:16:50.000000 nrpylatex-1.3/nrpylatex/utils/assertion.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)      773 2023-06-05 17:37:40.000000 nrpylatex-1.3/nrpylatex/utils/exceptions.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)     2555 2023-06-01 17:16:50.000000 nrpylatex-1.3/nrpylatex/utils/functional.py
+-rw-r--r--   0 ksible   (240660) campus    (1313)    19691 2023-06-01 17:34:36.000000 nrpylatex-1.3/nrpylatex/utils/structures.py
+drwxr-xr-x   0 ksible   (240660) campus    (1313)        0 2023-06-05 17:51:12.854257 nrpylatex-1.3/nrpylatex.egg-info/
+-rw-r--r--   0 ksible   (240660) campus    (1313)     5690 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/PKG-INFO
+-rw-r--r--   0 ksible   (240660) campus    (1313)      554 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/SOURCES.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)        1 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/dependency_links.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)        6 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/requires.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)       10 2023-06-05 17:51:12.000000 nrpylatex-1.3/nrpylatex.egg-info/top_level.txt
+-rw-r--r--   0 ksible   (240660) campus    (1313)       38 2023-06-05 17:51:12.854257 nrpylatex-1.3/setup.cfg
+-rw-r--r--   0 ksible   (240660) campus    (1313)     1149 2023-06-01 17:16:50.000000 nrpylatex-1.3/setup.py
```

### Comparing `nrpylatex-1.2.6/LICENSE` & `nrpylatex-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.2.6/PKG-INFO` & `nrpylatex-1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrpylatex
-Version: 1.2.6
+Version: 1.3
 Summary: LaTeX Interface to SymPy (CAS) for General Relativity
 Home-page: https://github.com/zachetienne/nrpylatex
 Author: Ken Sible
 Author-email: ksible@outlook.com
 License: BSD License (BSD)
 Keywords: General Relativity,LaTeX,CAS
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,22 @@
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![NRPyLaTeX Logo](/docs/imgs/logo.png)
+[![NRPyLaTeX Logo](https://raw.githubusercontent.com/zachetienne/nrpylatex/main/docs/imgs/logo.png)](https://zachetienne.github.io/nrpylatex/)
 
 ---
 
 [![CI](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml/badge.svg)](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml)
-[![pypi version](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
+[![PyPI](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
 [![arXiv](https://img.shields.io/badge/arXiv-2111.05861-B31B1B)](https://arxiv.org/abs/2111.05861)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=notebook%2FNRPyLaTeX%20Tutorial.ipynb)
 
 [NRPy+](https://github.com/zachetienne/nrpytutorial)'s LaTeX Interface to SymPy (CAS) for General Relativity
 
 - automatic expansion of
   - [Einstein summation convention](https://en.wikipedia.org/wiki/Einstein_notation)
   - Levi-Civita and Christoffel symbols
   - Lie and covariant derivatives
@@ -54,62 +54,62 @@
     for var in namespace:
         exec(f'{var} = mathematica_code({var})')
 
 If you are using a different CAS, reference the SymPy [documentation](https://docs.sympy.org/latest/modules/printing.html) to find the relevant printing function.
 
 ## &#167; Interactive Tutorial (MyBinder)
 
-[Quick Start](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=notebook%2FNRPyLaTeX%20Tutorial.ipynb) | [NRPy+ Integration](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-SymPy_LaTeX_Interface.ipynb) | [Guided Example (BSSN Formalism)](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-LaTeX_Interface_Example-BSSN_Cartesian.ipynb)
+[Quick Start](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb) | [NRPy+ Integration](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-SymPy_LaTeX_Interface.ipynb) | [Guided Example (BSSN Formalism)](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-LaTeX_Interface_Example-BSSN_Cartesian.ipynb)
 
 ## &#167; Documentation and Usage
 
 [Getting Started and API Reference](https://zachetienne.github.io/nrpylatex/)
 
 ### Simple Example ([Kretschmann Scalar](https://en.wikipedia.org/wiki/Kretschmann_scalar))
 
 **Python REPL or Script (*.py)**
 
     >>> from nrpylatex import parse_latex
     >>> parse_latex(r"""
     ...     % ignore "\begin{align}" "\end{align}"
     ...     \begin{align}
     ...         % coord [t, r, \theta, \phi]
-    ...         % define gDD --dim 4 --zero
+    ...         % define gDD --dim 4 --zeros
     ...         % define G M --const
     ...         %% define Schwarzschild metric diagonal
     ...         g_{t t} &= -\left(1 - \frac{2GM}{r}\right) \\
     ...         g_{r r} &=  \left(1 - \frac{2GM}{r}\right)^{-1} \\
     ...         g_{\theta \theta} &= r^2 \\
-    ...         g_{\phi \phi} &= r^2 \sin^2\theta \\
+    ...         g_{\phi \phi} &= r^2 \sin^2{\theta} \\
     ...         %% generate metric inverse gUU, determinant det(gDD), and connection GammaUDD
     ...         % assign gDD --metric
     ...         R^\alpha{}_{\beta \mu \nu} &= \partial_\mu \Gamma^\alpha_{\beta \nu} - \partial_\nu \Gamma^\alpha_{\beta \mu}
     ...             + \Gamma^\alpha_{\mu \gamma} \Gamma^\gamma_{\beta \nu} - \Gamma^\alpha_{\nu \sigma} \Gamma^\sigma_{\beta \mu} \\
     ...         K &= R^{\alpha \beta \mu \nu} R_{\alpha \beta \mu \nu}
     ...     \end{align}
     ... """)
     ('G', 'GammaUDD', 'gDD', 'gUU', 'epsilonUUUU', 'RUDDD', 'K', 'RUUUU', 'M', 'r', 'theta', 'RDDDD', 'gdet')
     >>> from sympy import simplify
     >>> print(simplify(K))
     48*G**2*M**2/r**6
 
 **IPython REPL or Jupyter Notebook**
 
-    In [1]: %load_ext nrpylatex.extension
+    In [1]: %load_ext nrpylatex
     In [2]: %%parse_latex
        ...: % ignore "\begin{align}" "\end{align}"
        ...: \begin{align}
        ...:     % coord [t, r, \theta, \phi]
-       ...:     % define gDD --dim 4 --zero
+       ...:     % define gDD --dim 4 --zeros
        ...:     % define G M --const
        ...:     %% define Schwarzschild metric diagonal
        ...:     g_{t t} &= -\left(1 - \frac{2GM}{r}\right) \\
        ...:     g_{r r} &=  \left(1 - \frac{2GM}{r}\right)^{-1} \\
        ...:     g_{\theta \theta} &= r^2 \\
-       ...:     g_{\phi \phi} &= r^2 \sin^2\theta \\
+       ...:     g_{\phi \phi} &= r^2 \sin^2{\theta} \\
        ...:     %% generate metric inverse gUU, determinant det(gDD), and connection GammaUDD
        ...:     % assign gDD --metric
        ...:     R^\alpha{}_{\beta \mu \nu} &= \partial_\mu \Gamma^\alpha_{\beta \nu} - \partial_\nu \Gamma^\alpha_{\beta \mu}
        ...:         + \Gamma^\alpha_{\mu \gamma} \Gamma^\gamma_{\beta \nu} - \Gamma^\alpha_{\nu \sigma} \Gamma^\sigma_{\beta \mu} \\
        ...:     K &= R^{\alpha \beta \mu \nu} R_{\alpha \beta \mu \nu}
        ...: \end{align}
     Out[2]: ('G', 'GammaUDD', 'gDD', 'gUU', 'epsilonUUUU', 'RUDDD', 'K', 'RUUUU', 'M', 'r', 'theta', 'RDDDD', 'gdet')
```

### Comparing `nrpylatex-1.2.6/README.md` & `nrpylatex-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-![NRPyLaTeX Logo](/docs/imgs/logo.png)
+[![NRPyLaTeX Logo](https://raw.githubusercontent.com/zachetienne/nrpylatex/main/docs/imgs/logo.png)](https://zachetienne.github.io/nrpylatex/)
 
 ---
 
 [![CI](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml/badge.svg)](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml)
-[![pypi version](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
+[![PyPI](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
 [![arXiv](https://img.shields.io/badge/arXiv-2111.05861-B31B1B)](https://arxiv.org/abs/2111.05861)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=notebook%2FNRPyLaTeX%20Tutorial.ipynb)
 
 [NRPy+](https://github.com/zachetienne/nrpytutorial)'s LaTeX Interface to SymPy (CAS) for General Relativity
 
 - automatic expansion of
   - [Einstein summation convention](https://en.wikipedia.org/wiki/Einstein_notation)
   - Levi-Civita and Christoffel symbols
   - Lie and covariant derivatives
@@ -34,62 +34,62 @@
     for var in namespace:
         exec(f'{var} = mathematica_code({var})')
 
 If you are using a different CAS, reference the SymPy [documentation](https://docs.sympy.org/latest/modules/printing.html) to find the relevant printing function.
 
 ## &#167; Interactive Tutorial (MyBinder)
 
-[Quick Start](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=notebook%2FNRPyLaTeX%20Tutorial.ipynb) | [NRPy+ Integration](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-SymPy_LaTeX_Interface.ipynb) | [Guided Example (BSSN Formalism)](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-LaTeX_Interface_Example-BSSN_Cartesian.ipynb)
+[Quick Start](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb) | [NRPy+ Integration](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-SymPy_LaTeX_Interface.ipynb) | [Guided Example (BSSN Formalism)](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-LaTeX_Interface_Example-BSSN_Cartesian.ipynb)
 
 ## &#167; Documentation and Usage
 
 [Getting Started and API Reference](https://zachetienne.github.io/nrpylatex/)
 
 ### Simple Example ([Kretschmann Scalar](https://en.wikipedia.org/wiki/Kretschmann_scalar))
 
 **Python REPL or Script (*.py)**
 
     >>> from nrpylatex import parse_latex
     >>> parse_latex(r"""
     ...     % ignore "\begin{align}" "\end{align}"
     ...     \begin{align}
     ...         % coord [t, r, \theta, \phi]
-    ...         % define gDD --dim 4 --zero
+    ...         % define gDD --dim 4 --zeros
     ...         % define G M --const
     ...         %% define Schwarzschild metric diagonal
     ...         g_{t t} &= -\left(1 - \frac{2GM}{r}\right) \\
     ...         g_{r r} &=  \left(1 - \frac{2GM}{r}\right)^{-1} \\
     ...         g_{\theta \theta} &= r^2 \\
-    ...         g_{\phi \phi} &= r^2 \sin^2\theta \\
+    ...         g_{\phi \phi} &= r^2 \sin^2{\theta} \\
     ...         %% generate metric inverse gUU, determinant det(gDD), and connection GammaUDD
     ...         % assign gDD --metric
     ...         R^\alpha{}_{\beta \mu \nu} &= \partial_\mu \Gamma^\alpha_{\beta \nu} - \partial_\nu \Gamma^\alpha_{\beta \mu}
     ...             + \Gamma^\alpha_{\mu \gamma} \Gamma^\gamma_{\beta \nu} - \Gamma^\alpha_{\nu \sigma} \Gamma^\sigma_{\beta \mu} \\
     ...         K &= R^{\alpha \beta \mu \nu} R_{\alpha \beta \mu \nu}
     ...     \end{align}
     ... """)
     ('G', 'GammaUDD', 'gDD', 'gUU', 'epsilonUUUU', 'RUDDD', 'K', 'RUUUU', 'M', 'r', 'theta', 'RDDDD', 'gdet')
     >>> from sympy import simplify
     >>> print(simplify(K))
     48*G**2*M**2/r**6
 
 **IPython REPL or Jupyter Notebook**
 
-    In [1]: %load_ext nrpylatex.extension
+    In [1]: %load_ext nrpylatex
     In [2]: %%parse_latex
        ...: % ignore "\begin{align}" "\end{align}"
        ...: \begin{align}
        ...:     % coord [t, r, \theta, \phi]
-       ...:     % define gDD --dim 4 --zero
+       ...:     % define gDD --dim 4 --zeros
        ...:     % define G M --const
        ...:     %% define Schwarzschild metric diagonal
        ...:     g_{t t} &= -\left(1 - \frac{2GM}{r}\right) \\
        ...:     g_{r r} &=  \left(1 - \frac{2GM}{r}\right)^{-1} \\
        ...:     g_{\theta \theta} &= r^2 \\
-       ...:     g_{\phi \phi} &= r^2 \sin^2\theta \\
+       ...:     g_{\phi \phi} &= r^2 \sin^2{\theta} \\
        ...:     %% generate metric inverse gUU, determinant det(gDD), and connection GammaUDD
        ...:     % assign gDD --metric
        ...:     R^\alpha{}_{\beta \mu \nu} &= \partial_\mu \Gamma^\alpha_{\beta \nu} - \partial_\nu \Gamma^\alpha_{\beta \mu}
        ...:         + \Gamma^\alpha_{\mu \gamma} \Gamma^\gamma_{\beta \nu} - \Gamma^\alpha_{\nu \sigma} \Gamma^\sigma_{\beta \mu} \\
        ...:     K &= R^{\alpha \beta \mu \nu} R_{\alpha \beta \mu \nu}
        ...: \end{align}
     Out[2]: ('G', 'GammaUDD', 'gDD', 'gUU', 'epsilonUUUU', 'RUDDD', 'K', 'RUUUU', 'M', 'r', 'theta', 'RDDDD', 'gdet')
```

### Comparing `nrpylatex-1.2.6/nrpylatex/core/assertion.py` & `nrpylatex-1.3/nrpylatex/utils/assertion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Assert SymPy Expression Equality """
+""" SymPy Expression Equivalence """
 # Author: Ken Sible
 # Email:  ksible *at* outlook *dot* com
 
 from mpmath import mp, mpf, mpc, fabs, log10
 import sympy as sp, sys, random
 
 precision = 30
```

### Comparing `nrpylatex-1.2.6/nrpylatex/core/functional.py` & `nrpylatex-1.3/nrpylatex/utils/functional.py`

 * *Files identical despite different names*

### Comparing `nrpylatex-1.2.6/nrpylatex/core/parser.py` & `nrpylatex-1.3/nrpylatex/core/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """ NRPyLaTeX Parser """
 # Author: Ken Sible
 # Email:  ksible *at* outlook *dot* com
 
-from sympy import Function, Derivative, Symbol, Integer, Rational, Float, Pow, Add
-from sympy import sin, cos, tan, sinh, cosh, tanh, asin, acos, atan, asinh, acosh, atanh
-from sympy import pi, exp, log, sqrt, expand, diff, srepr
-from nrpylatex.core.functional import uniquify, product, flatten
-from nrpylatex.core.exprtree import ExprTree
-from nrpylatex.core.indexed_symbol import symdef
 from nrpylatex.core.scanner import Scanner
+from nrpylatex.core.generator import Generator
+from nrpylatex.utils.structures import ExprTree, CoordinateSystem, symdef
+from nrpylatex.utils.structures import IndexedSymbol, IndexedSymbolError
+from nrpylatex.utils.exceptions import NRPyLaTeXError
+from nrpylatex.utils.functional import product
+from sympy import Function, Derivative, Symbol, Integer, Rational, Float, Pow
+from sympy import sin, cos, tan, sinh, cosh, tanh, asin, acos, atan, asinh, acosh, atanh
+from sympy import pi, exp, log, sqrt, expand, diff
 from collections import OrderedDict
-import warnings, math, re
+import re
 
 class Parser:
-    """ The following class will parse a tokenized LaTeX sentence. """
 
     _namespace, _property = OrderedDict(), {}
 
     def __init__(self, debug=False):
         self.scanner = Scanner()
+        self.generator = Generator(self)
         self.state = OrderedDict()
         if not self._property:
             self.initialize()
         self._property['debug'] = int(debug)
         for symbol in self._namespace:
             self._namespace[symbol].overridden = False
 
@@ -142,39 +144,37 @@
             self._srepl()
         elif self.peek('COORD_MACRO'):
             self._coord()
         elif self.peek('INDEX_MACRO'):
             self._index()
         else:
             sentence, position = self.scanner.sentence, self.scanner.mark()
-            raise ParseError('unsupported macro \'%s\' at position %d' %
+            raise ParserError('unsupported macro \'%s\' at position %d' %
                 (macro, position), sentence, position)
 
-    # <DEFINE> -> <DEFINE_MACRO> { <VARIABLE> }+ { '--' ( <ZERO> | <KRON> | <CONST> | <OPTION> ) }*
+    # <DEFINE> -> <DEFINE_MACRO> { <VARIABLE> }+ { '--' ( <CONST> | <ZEROS> | <OPTION> ) }*
     def _define(self):
         self.scanner.whitespace = True
         self.expect('DEFINE_MACRO')
         symbols = []
         while True:
             self.accept('WHITESPACE')
             symbols.append(self._variable())
             self.accept('WHITESPACE')
             if self.peek('MINUS') or self.peek('LINEBREAK'): break
         dimension = suffix = symmetry = metric = weight = None
-        zero = kron = const = False
+        const = zeros = False
         while self.accept('MINUS'):
             self.expect('MINUS')
             self.accept('WHITESPACE')
-            zero = self.accept('ZERO')
-            self.accept('WHITESPACE')
-            kron = self.accept('KRON')
-            self.accept('WHITESPACE')
             const = self.accept('CONST')
             self.accept('WHITESPACE')
-            if not (zero or kron or const):
+            zeros = self.accept('ZEROS')
+            self.accept('WHITESPACE')
+            if not (const or zeros):
                 option, value = self._option().split('<>')
                 if option == 'dimension':
                     dimension = int(value)
                 elif option == 'suffix':
                     if suffix != 'none':
                         suffix = value
                 elif option == 'symmetry':
@@ -186,29 +186,25 @@
             self.accept('WHITESPACE')
         for symbol in symbols:
             if const:
                 self._namespace[symbol] = Function('Constant')(Symbol(symbol, real=True))
                 self.state[symbol] = None
             else:
                 function = Function('Tensor')(Symbol(symbol, real=True))
-                tensor = Tensor(function, dimension, suffix=suffix, metric=metric, weight=weight)
-                if kron:
-                    if tensor.rank != 2:
-                        raise TensorError('cannot instantiate Kronecker delta of rank ' + str(tensor.rank))
-                    tensor.structure = [[1 if i == j else 0 for j in range(dimension)] for i in range(dimension)]
-                tensor.symmetry = ('sym01' if symmetry in ('kron', 'metric') else symmetry)
-                self._define_tensor(tensor, zero=zero)
+                tensor = IndexedSymbol(function, dimension, suffix=suffix, metric=metric, weight=weight)
+                tensor.symmetry = 'sym01' if symmetry == 'metric' else symmetry
+                self._define_tensor(tensor, zeros=zeros)
                 if symmetry == 'metric':
                     diacritic = next(diacritic for diacritic in ('bar', 'hat', 'tilde', '') if diacritic in symbol)
                     self._property['metric'][diacritic] = re.split(diacritic if diacritic else r'[UD]', symbol)[0]
                     with self.scanner.new_context():
                         self.scanner.whitespace = False
                         self.accept('WHITESPACE')
                         self.accept('LINEBREAK')
-                        self.parse_latex(self._generate_metric(symbol, dimension, diacritic, suffix))
+                        self.parse_latex(Generator.generate_metric(symbol, dimension, diacritic, suffix))
         self.scanner.whitespace = False
         self.accept('WHITESPACE')
         self.accept('LINEBREAK')
 
     # <ASSIGN> -> <ASSIGN_MACRO> { <VARIABLE> }+ { '--' <OPTION> }+
     def _assign(self):
         self.scanner.whitespace = True
@@ -234,64 +230,64 @@
             elif option == 'metric':
                 metric = value
             elif option == 'weight':
                 weight = value
             self.accept('WHITESPACE')
         for symbol in symbols:
             if symbol not in self._namespace:
-                raise TensorError('cannot assign attribute(s) to undefined variable \'{symbol}\''.format(symbol=symbol))
+                raise IndexedSymbolError('cannot assign attribute(s) to undefined variable \'{symbol}\''.format(symbol=symbol))
             tensor = self._namespace[symbol]
             if dimension:
                 if tensor.rank > 0:
-                    raise TensorError('cannot assign dimension to \'{symbol}\' since rank({symbol}) > 0'.format(symbol=symbol))
+                    raise IndexedSymbolError('cannot assign dimension to \'{symbol}\' since rank({symbol}) > 0'.format(symbol=symbol))
                 tensor.dimension = dimension
             if suffix:
                 tensor.suffix = suffix
             if symmetry:
                 tensor.symmetry = 'sym01' if symmetry == 'metric' else symmetry
             if metric:
                 tensor.metric = metric
             if weight:
                 tensor.weight = weight
             if symmetry == 'metric':
                 if symbol not in self._namespace:
-                    raise TensorError('cannot assign --metric to undefined variable \'{symbol}\''.format(symbol=symbol))
+                    raise IndexedSymbolError('cannot assign --metric to undefined variable \'{symbol}\''.format(symbol=symbol))
                 tensor = self._namespace[symbol]
                 if tensor.rank != 2:
-                    raise TensorError('cannot assign --metric to \'{symbol}\' since rank({symbol}) != 2'.format(symbol=symbol))
+                    raise IndexedSymbolError('cannot assign --metric to \'{symbol}\' since rank({symbol}) != 2'.format(symbol=symbol))
                 structure = tensor.structure
                 for i in range(tensor.dimension):
                     for j in range(tensor.dimension):
                         if structure[i][j] == 0:
                             structure[i][j] = structure[j][i]
                         elif structure[j][i] == 0:
                             structure[j][i] = structure[i][j]
                         if structure[i][j] != structure[j][i]:
-                            raise TensorError('cannot assign --metric to \'{symbol}\' since {symbol}[{i}][{j}] != {symbol}[{j}][{i}]'
+                            raise IndexedSymbolError('cannot assign --metric to \'{symbol}\' since {symbol}[{i}][{j}] != {symbol}[{j}][{i}]'
                                 .format(symbol=symbol, i=i, j=j))
                 diacritic = next(diacritic for diacritic in ('bar', 'hat', 'tilde', '') if diacritic in symbol)
                 self._property['metric'][diacritic] = re.split(diacritic if diacritic else r'[UD]', symbol)[0]
                 with self.scanner.new_context():
                     self.scanner.whitespace = False
                     self.accept('WHITESPACE')
                     self.accept('LINEBREAK')
-                    self.parse_latex(self._generate_metric(symbol, tensor.dimension, diacritic, tensor.suffix))
+                    self.parse_latex(Generator.generate_metric(symbol, tensor.dimension, diacritic, tensor.suffix))
             base_symbol = re.split(r'_d|_dup|_cd|_ld', symbol)[0]
             if base_symbol and tensor.suffix:
                 rank = 0
                 for rank_symbol in re.split(r'_d|_dup|_cd|_ld', symbol):
                     for character in reversed(rank_symbol):
                         if character in ('U', 'D'):
                             rank += 1
                         else: break
                 if base_symbol in self._namespace:
                     self._namespace[base_symbol].suffix = tensor.suffix
                 elif rank == 0:
                     function = Function('Tensor')(Symbol(base_symbol, real=True))
-                    self._define_tensor(Tensor(function, suffix=tensor.suffix))
+                    self._define_tensor(IndexedSymbol(function, suffix=tensor.suffix))
         self.scanner.whitespace = False
         self.accept('WHITESPACE')
         self.accept('LINEBREAK')
 
     # <IGNORE> -> <IGNORE_MACRO> { <STRING> }+
     def _ignore(self):
         self.expect('IGNORE_MACRO')
@@ -393,15 +389,15 @@
         else:
             self.expect('LBRACK')
             del self._property['coord'][:]
             while True:
                 symbol = self._strip(self._symbol())
                 if symbol in self._property['coord']:
                     sentence, position = self.scanner.sentence, self.scanner.mark()
-                    raise ParseError('duplicate coord symbol \'%s\' at position %d' %
+                    raise ParserError('duplicate coord symbol \'%s\' at position %d' %
                         (sentence[position], position), sentence, position)
                 self._property['coord'].append(Symbol(symbol, real=True))
                 if not self.accept('COMMA'): break
             self.expect('RBRACK')
 
     # <INDEX> -> <INDEX_MACRO> [ { <LETTER> | '[' <LETTER> '-' <LETTER> ']' }+ | '--' <DEFAULT> ] '--' <DIM> <INTEGER>
     def _index(self):
@@ -417,15 +413,15 @@
                 if self.accept('LBRACK'):
                     index_1 = self._strip(self.scanner.lexeme)
                     self.expect('LETTER')
                     self.expect('MINUS')
                     index_2 = self._strip(self.scanner.lexeme)
                     self.expect('LETTER')
                     if len(index_1) > 1 or len(index_2) > 1:
-                        raise ParseError('unsupported index range \'%s\' at position %d' %
+                        raise ParserError('unsupported index range \'%s\' at position %d' %
                             (sentence[position:self.scanner.index], position), sentence, position)
                     indices.extend([chr(i) for i in range(ord(index_1), ord(index_2) + 1)])
                     self.expect('RBRACK')
                 elif self.peek('LETTER'):
                     indices.append(self._strip(self.scanner.lexeme))
                     self.expect('LETTER')
                 if self.peek('MINUS'): break
@@ -437,43 +433,46 @@
         dimension = int(dimension)
         if self.accept('MINUS'):
             self.expect('MINUS')
             self.expect('DEFAULT')
             indices = [index for index in self._property['index']]
         self._property['index'].update({index: dimension for index in indices})
 
-    # <OPTION> -> <DIM> <INTEGER> | <SYM> <SYMMETRY> | <WEIGHT> <NUMBER> | <DERIV> <SUFFIX> | <METRIC> [ <VARIABLE> ]
+    # <OPTION> -> <DIM> <INTEGER> | <SYM> <SYMMETRY> | <WEIGHT> <NUMBER> | <SUFFIX> <VARIABLE> | <METRIC> [ <VARIABLE> ]
     def _option(self):
         if self.accept('DIM'):
             self.accept('WHITESPACE')
             dimension = self.scanner.lexeme
             self.expect('INTEGER')
             return 'dimension<>' + dimension
         if self.accept('SYM'):
             self.accept('WHITESPACE')
             symmetry = self.scanner.lexeme
             self.expect('SYMMETRY')
             return 'symmetry<>' + symmetry
         if self.accept('WEIGHT'):
             self.accept('WHITESPACE')
             weight = self._number()
-            return 'weight<>' + weight
-        if self.accept('DERIV'):
+            return 'weight<>' + str(weight)
+        if self.accept('SUFFIX'):
             self.accept('WHITESPACE')
-            suffix = self.scanner.lexeme
-            self.expect('SUFFIX')
+            sentence, position = self.scanner.sentence, self.scanner.mark()
+            suffix = self._variable()
+            if suffix[0] != 'd' or suffix[-1] != 'D':
+                raise ParserError('unsupported suffix \'%s\' at position %d' %
+                    (suffix, position), sentence, position)
             return 'suffix<>' + suffix
         if self.accept('METRIC'):
             self.accept('WHITESPACE')
             if self.peek('LETTER'):
                 metric = self._variable()
                 return 'metric<>' + metric
             return 'symmetry<>metric'
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unexpected \'%s\' at position %d' %
+        raise ParserError('unexpected \'%s\' at position %d' %
             (sentence[position], position), sentence, position)
 
     # <ASSIGNMENT> -> <OPERATOR> = <EXPRESSION> [ '\\' ] [ '%' <NOIMPSUM> ]
     def _assignment(self):
         function = self._operator('LHS')
         indexed = function.func == Function('Tensor') and len(function.args) > 1
         self.expect('EQUAL')
@@ -482,54 +481,36 @@
         self.accept('NEWLINE')
         position_2 = self.scanner.mark()
         impsum = True
         if self.accept('COMMENT'):
             if self.accept('NOIMPSUM'):
                 impsum = False
             else: self.scanner.reset()
-        equation = ((Tensor.latex_format(function), sentence[position_1:position_2]), tree.root.expr)
+        equation = ((IndexedSymbol.latex_format(function), sentence[position_1:position_2]), tree.root.expr)
         if self._property['debug']:
             (latex_LHS, latex_RHS), expr_RHS = equation
             lineno = '[%d]' % self._property['debug']
-            print('%s LaTeX Input' % lineno)
-            print('%s     %s = %s' % (len(lineno) * ' ', latex_LHS, latex_RHS.rstrip()))
-            print('%s SymPy Output' % (len(lineno) * ' '))
-            print('%s     %s = %s' % (len(lineno) * ' ', function, expr_RHS))
+            print('%s LaTeX' % lineno)
+            print('%s   %s = %s' % (len(lineno) * ' ', latex_LHS, latex_RHS.rstrip()))
+            print('%s SymPy' % (len(lineno) * ' '))
+            print('%s   %s = %s' % (len(lineno) * ' ', function, expr_RHS))
         if not indexed:
             for subtree in tree.preorder():
                 subexpr, rank = subtree.expr, len(subtree.expr.args)
                 if subexpr.func == Function('Tensor') and rank > 1:
                     indexed = True
         LHS, RHS = function, expand(tree.root.expr) if indexed else tree.root.expr
-        # perform implied summation on indexed expression
-        LHS_RHS, dimension = self._summation(LHS, RHS, impsum=impsum)
-        if self._property['debug']:
-            lineno = '[%d]' % self._property['debug']
-            print('%s Python Output' % (len(lineno) * ' '))
-            print('%s     %s\n' % (len(lineno) * ' ', LHS_RHS))
-            self._property['debug'] += 1
-        global_env = dict(self._namespace)
-        for key in global_env:
-            if isinstance(global_env[key], Tensor):
-                global_env[key] = global_env[key].structure
-            if isinstance(global_env[key], Function('Constant')):
-                global_env[key] = global_env[key].args[0]
-        global_env['coord'] = self._property['coord']
-        exec('from sympy import *', global_env)
-        # evaluate every implied summation and update namespace
-        try: exec(LHS_RHS, global_env)
-        except IndexError:
-            raise ParseError('index out of range; change loop/summation range')
+        global_env, dimension = self.generator.generate(LHS, RHS, impsum)
         symbol, indices = str(function.args[0]), function.args[1:]
         if any(isinstance(index, Integer) for index in indices):
             tensor = self._namespace[symbol]
             tensor.structure = global_env[symbol]
         else:
             suffix = self._namespace[symbol].suffix if symbol in self._namespace else None
-            tensor = Tensor(function, dimension, structure=global_env[symbol],
+            tensor = IndexedSymbol(function, dimension, structure=global_env[symbol],
                 equation=equation, suffix=suffix, impsum=impsum)
         self._namespace[symbol] = tensor
         self.state[symbol] = None
 
     # <EXPRESSION> -> <TERM> { ( '+' | '-' ) <TERM> }*
     def _expression(self):
         expr = self._term()
@@ -545,86 +526,90 @@
         expr = self._factor()
         while any(self.peek(token) for token in ('DIVIDE',
                 'RATIONAL', 'DECIMAL', 'INTEGER', 'PI', 'PAR_SYM', 'COV_SYM', 'LIE_SYM',
                 'SYMB_CMD', 'FUNC_CMD', 'FRAC_CMD', 'SQRT_CMD', 'NLOG_CMD', 'TRIG_CMD',
                 'LPAREN', 'LBRACK', 'DIACRITIC', 'LETTER', 'COMMAND', 'COMMENT', 'BACKSLASH')):
             self.scanner.mark()
             if self.accept('COMMENT'):
-                if not self.peek('DERIV'):
+                if not self.peek('SUFFIX'):
                     self.scanner.reset()
                     return expr
                 self.scanner.reset()
             if self.accept('BACKSLASH'):
                 if self.peek('RBRACE'):
                     self.scanner.reset()
                     return expr
                 self.scanner.reset()
             if self.accept('DIVIDE'):
                 expr /= self._factor()
             else: expr *= self._factor()
         return expr
 
-    # <FACTOR> -> <BASE> { '^' <EXPONENT> }*
+    # <FACTOR> -> [ '-' ] <ATOM>
     def _factor(self):
+        sign = -1 if self.accept('MINUS') else 1
+        return sign * self._atom()
+
+    # <ATOM> -> <BASE> { '^' <EXPONENT> }*
+    def _atom(self):
         stack = [self._base()]
         while self.accept('CARET'):
             stack.append(self._exponent())
         if len(stack) == 1: stack.append(1)
         expr = stack.pop()
         for subexpr in reversed(stack):
             exponential = (subexpr == Function('Tensor')(Symbol('e', real=True)))
             expr = exp(expr) if exponential else subexpr ** expr
         return expr
 
-    # <BASE> -> [ '-' ] ( <NUMBER> | <COMMAND> | <OPERATOR> | <SUBEXPR> )
+    # <BASE> -> <BASE> -> <NUMBER> | <COMMAND> | <OPERATOR> | <SUBEXPR>
     def _base(self):
-        sign = -1 if self.accept('MINUS') else 1
         if self.peek('LETTER') or self.peek('SYMB_CMD'):
             self.scanner.mark()
             symbol = self._strip(self._symbol())
             if symbol in ('epsilon', 'Gamma', 'D'):
                 self.scanner.reset()
-                return sign * self._operator()
+                return self._operator()
             if symbol in self._namespace:
                 variable = self._namespace[symbol]
-                if isinstance(variable, Tensor) and variable.rank > 0:
+                if isinstance(variable, IndexedSymbol) and variable.rank > 0:
                     self.scanner.reset()
-                    return sign * self._operator()
+                    return self._operator()
             for key in self._namespace:
                 base_symbol = key
                 for i, character in enumerate(reversed(base_symbol)):
                     if character not in ('U', 'D'):
                         base_symbol = base_symbol[:len(base_symbol) - i]; break
-                if isinstance(self._namespace[key], Tensor) and symbol == base_symbol \
+                if isinstance(self._namespace[key], IndexedSymbol) and symbol == base_symbol \
                         and self._namespace[key].rank > 0:
                     self.scanner.reset()
-                    return sign * self._operator()
+                    return self._operator()
             if self.peek('CARET'):
                 function = Function('Tensor')(Symbol(symbol, real=True))
                 if symbol in self._namespace:
                     if isinstance(self._namespace[symbol], Function('Constant')):
-                        return sign * self._namespace[symbol]
+                        return self._namespace[symbol]
                 else:
-                    self._define_tensor(Tensor(function))
-                return sign * function
+                    self._define_tensor(IndexedSymbol(function))
+                return function
             self.scanner.reset()
-            return sign * self._operator()
+            return self._operator()
         if any(self.peek(token) for token in
                 ('RATIONAL', 'DECIMAL', 'INTEGER', 'PI')):
-            return sign * self._number()
+            return self._number()
         if any(self.peek(token) for token in
                 ('FUNC_CMD', 'FRAC_CMD', 'SQRT_CMD', 'NLOG_CMD', 'TRIG_CMD', 'COMMAND')):
-            return sign * self._command()
+            return self._command()
         if any(self.peek(token) for token in
                 ('PAR_SYM', 'COV_SYM', 'LIE_SYM', 'COMMENT', 'DIACRITIC')):
-            return sign * self._operator()
+            return self._operator()
         if any(self.peek(i) for i in ('LPAREN', 'LBRACK', 'BACKSLASH')):
-            return sign * self._subexpr()
+            return self._subexpr()
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unexpected \'%s\' at position %d' %
+        raise ParserError('unexpected \'%s\' at position %d' %
             (sentence[position], position), sentence, position)
 
     # <EXPONENT> -> <BASE> | '{' <EXPRESSION> '}' | '{' '{' <EXPRESSION> '}' '}'
     def _exponent(self):
         if self.accept('LBRACE'):
             if self.accept('LBRACE'):
                 base = self._expression()
@@ -645,15 +630,15 @@
         elif self.accept('BACKSLASH'):
             self.expect('LBRACE')
             expr = self._expression()
             self.expect('BACKSLASH')
             self.expect('RBRACE')
         else:
             sentence, position = self.scanner.sentence, self.scanner.mark()
-            raise ParseError('unexpected \'%s\' at position %d' %
+            raise ParserError('unexpected \'%s\' at position %d' %
                 (sentence[position], position), sentence, position)
         return expr
 
     # <COMMAND> -> <FUNC> | <FRAC> | <SQRT> | <NLOG> | <TRIG>
     def _command(self):
         command = self.scanner.lexeme
         if self.peek('FUNC_CMD'):
@@ -663,28 +648,28 @@
         if self.peek('SQRT_CMD'):
             return self._sqrt()
         if self.peek('NLOG_CMD'):
             return self._nlog()
         if self.peek('TRIG_CMD'):
             return self._trig()
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unsupported command \'%s\' at position %d' %
+        raise ParserError('unsupported command \'%s\' at position %d' %
             (command, position), sentence, position)
 
-    # <FUNC> -> <FUNC_CMD> '(' <EXPRESSION> ')'
+    # <FUNC> -> <FUNC_CMD> '{' <EXPRESSION> '}'
     def _func(self):
         func = self._strip(self.scanner.lexeme)
         self.expect('FUNC_CMD')
-        self.expect('LPAREN')
+        self.expect('LBRACE')
         expr = self._expression()
-        self.expect('RPAREN')
+        self.expect('RBRACE')
         if func == 'exp':
             return exp(expr)
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unsupported function \'%s\' at position %d' %
+        raise ParserError('unsupported function \'%s\' at position %d' %
             (func, position), sentence, position)
 
     # <FRAC> -> <FRAC_CMD> '{' <EXPRESSION> '}' '{' <EXPRESSION> '}'
     def _frac(self):
         self.expect('FRAC_CMD')
         self.expect('LBRACE')
         numerator = self._expression()
@@ -706,43 +691,34 @@
         self.expect('LBRACE')
         expr = self._expression()
         self.expect('RBRACE')
         if root == Rational(1, 2):
             return sqrt(expr)
         return Pow(expr, root)
 
-    # <NLOG> -> <NLOG_CMD> [ '_' ( <NUMBER> | '{' <NUMBER> '}' ) ] ( <NUMBER> | <TENSOR> | <SUBEXPR> )
+    # <NLOG> -> <NLOG_CMD> [ '_' ( <NUMBER> | '{' <NUMBER> '}' ) ] '{' <EXPRESSION> '}'
     def _nlog(self):
         func = self._strip(self.scanner.lexeme)
         self.expect('NLOG_CMD')
         if func == 'log':
             if self.accept('UNDERSCORE'):
                 if self.accept('LBRACE'):
                     base = self._number()
                     self.expect('RBRACE')
                 else:
                     base = self._number()
                 base = int(base)
             else: base = 10
-        if any(self.peek(token) for token in
-                ('RATIONAL', 'DECIMAL', 'INTEGER', 'PI')):
-            expr = self._number()
-        elif any(self.peek(token) for token in
-                ('LETTER', 'DIACRITIC', 'SYMB_CMD')):
-            expr = self._tensor()
-        elif any(self.peek(i) for i in ('LPAREN', 'LBRACK', 'LBRACE')):
-            expr = self._subexpr()
-        else:
-            sentence, position = self.scanner.sentence, self.scanner.mark()
-            raise ParseError('unexpected \'%s\' at position %d' %
-                (sentence[position], position), sentence, position)
+        self.expect('LBRACE')
+        expr = self._expression()
+        self.expect('RBRACE')
         if func == 'ln': return log(expr)
         return log(expr, base)
 
-    # <TRIG> -> <TRIG_CMD> [ '^' ( <NUMBER> | '{' <NUMBER> '}' ) ] ( <NUMBER> | <TENSOR> | <SUBEXPR> )
+    # <TRIG> -> <TRIG_CMD> [ '^' ( <NUMBER> | '{' <NUMBER> '}' ) ] '{' <EXPRESSION> '}'
     def _trig(self):
         func = self._strip(self.scanner.lexeme)
         self.expect('TRIG_CMD')
         if self.accept('CARET'):
             if self.accept('LBRACE'):
                 exponent = self._number()
                 self.expect('RBRACE')
@@ -752,36 +728,26 @@
         else: exponent = 1
         if   func == 'cosh': trig = acosh if exponent == -1 else cosh
         elif func == 'sinh': trig = asinh if exponent == -1 else sinh
         elif func == 'tanh': trig = atanh if exponent == -1 else tanh
         elif func == 'cos':  trig = acos  if exponent == -1 else cos
         elif func == 'sin':  trig = asin  if exponent == -1 else sin
         elif func == 'tan':  trig = atan  if exponent == -1 else tan
-        if any(self.peek(token) for token in
-                ('RATIONAL', 'DECIMAL', 'INTEGER', 'PI')):
-            expr = self._number()
-        elif any(self.peek(token) for token in
-                ('LETTER', 'DIACRITIC', 'SYMB_CMD')):
-            expr = self._tensor()
-        elif any(self.peek(i) for i in ('LPAREN', 'LBRACK', 'LBRACE')):
-            expr = self._subexpr()
-        else:
-            sentence, position = self.scanner.sentence, self.scanner.mark()
-            raise ParseError('unexpected \'%s\' at position %d' %
-                (sentence[position], position), sentence, position)
+        self.expect('LBRACE')
+        expr = self._expression()
+        self.expect('RBRACE')
         if exponent == -1: return trig(expr)
         return trig(expr) ** exponent
 
-    # <OPERATOR> -> [ '%' <DERIV> <SUFFIX> ] ( <PARDRV> | <COVDRV> | <LIEDRV> | <TENSOR> )
+    # <OPERATOR> -> [ '%' <SUFFIX> <VARIABLE> ] ( <PARDRV> | <COVDRV> | <LIEDRV> | <TENSOR> )
     def _operator(self, location='RHS'):
         global_suffix = self._property['suffix']
         if self.accept('COMMENT'):
-            self.expect('DERIV')
-            suffix = self.scanner.lexeme
             self.expect('SUFFIX')
+            suffix = self._variable()
             self._property['suffix'] = suffix
         if not global_suffix and location == 'LHS':
             self._property['suffix'] = 'dD'
         operator = self.scanner.lexeme
         if self.peek('PAR_SYM'):
             pardrv = self._pardrv(location)
             self._property['suffix'] = global_suffix
@@ -806,15 +772,15 @@
             self._property['suffix'] = global_suffix
             return liedrv
         if any(self.peek(token) for token in ('LETTER', 'DIACRITIC', 'SYMB_CMD')):
             tensor = self._tensor(location)
             self._property['suffix'] = global_suffix
             return tensor
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unsupported operator \'%s\' at position %d' %
+        raise ParserError('unsupported operator \'%s\' at position %d' %
             (operator, position), sentence, position)
 
     # <PARDRV> -> <PAR_SYM> '_' <INDEXING_2> ( <OPERATOR> | <SUBEXPR> )
     def _pardrv(self, location='RHS'):
         self.expect('PAR_SYM')
         self.expect('UNDERSCORE')
         sentence, position = self.scanner.sentence, self.scanner.mark()
@@ -842,15 +808,15 @@
                         symbol = str(function.args[0])
                         tensor = self._namespace[symbol]
                         global_suffix = self._property['suffix']
                         suffix = tensor.suffix
                         if global_suffix and suffix:
                             suffix = global_suffix
                         if not isinstance(index, Symbol) and suffix is None:
-                            raise ParseError('cannot perform numeric indexing on a symbolic derivative', sentence, position)
+                            raise ParserError('cannot perform numeric indexing on a symbolic derivative', sentence, position)
                         subtree.expr = self._define_pardrv(function, location, suffix, index)
                     del subtree.children[:]
                 elif subexpr.func == Function('Function'):
                     subtree.expr = subexpr.args[0]
                     del subtree.children[:]
             return tree.reconstruct()
         function = self._operator()
@@ -859,15 +825,15 @@
         symbol = str(function.args[0])
         tensor = self._namespace[symbol]
         global_suffix = self._property['suffix']
         suffix = tensor.suffix
         if global_suffix and suffix:
             suffix = global_suffix
         if not isinstance(index, Symbol) and suffix is None:
-            raise ParseError('cannot perform numeric indexing on a symbolic derivative', sentence, position)
+            raise ParserError('cannot perform numeric indexing on a symbolic derivative', sentence, position)
         return self._define_pardrv(function, location, suffix, index)
 
     # <COVDRV> -> ( <COV_SYM> | <DIACRITIC> '{' <COV_SYM> '}' ) ( '^' | '_' ) <INDEXING_2> ( <OPERATOR> | <SUBEXPR> )
     def _covdrv(self, location='RHS'):
         diacritic, position = '', self.scanner.mark()
         if self.peek('DIACRITIC'):
             diacritic = self._strip(self.scanner.lexeme)
@@ -881,36 +847,36 @@
         else:
             operator = '\\nabla'
             if self.peek('LETTER') and self.scanner.lexeme == 'D':
                 self.scanner.lex()
             else: self.expect('COV_SYM')
         metric = self._property['metric'][diacritic] + diacritic
         if metric + 'DD' not in self._namespace:
-            raise ParseError('cannot generate covariant derivative without defined metric \'%s\'' %
+            raise ParserError('cannot generate covariant derivative without defined metric \'%s\'' %
                 metric, self.scanner.sentence, position)
         if len(metric) > 1:
             metric = '\\mathrm{' + metric + '}'
         if self.accept('CARET'):
             index = (self._indexing_2(), 'U')
         elif self.accept('UNDERSCORE'):
             index = (self._indexing_2(), 'D')
         else:
             sentence, position = self.scanner.sentence, self.scanner.mark()
-            raise ParseError('unexpected \'%s\' at position %d' %
+            raise ParserError('unexpected \'%s\' at position %d' %
                 (sentence[position], position), sentence, position)
         func_list, expression = self._expand_product(location, 'cd' + diacritic, index[1], index[0])
         for symbol, function in func_list:
             if index[1] == 'U':
                 equation = [operator, ' = ', '', operator]
-                idx_gen = index_count()
+                idx_gen = IndexedSymbol.index_count()
                 indexing = [str(i) for i in function.args[1:]] + [str(index[0])]
                 for i, idx in enumerate(indexing):
                     if idx in indexing[:i]:
                         indexing[i] = next(x for x in idx_gen if x not in indexing)
-                latex = Tensor.latex_format(Function('Tensor')(function.args[0],
+                latex = IndexedSymbol.latex_format(Function('Tensor')(function.args[0],
                             *(Symbol(i) for i in indexing[:-1])))
                 covdrv_index = indexing[-1]
                 if '_' in str(covdrv_index):
                     base, subscript = str(covdrv_index).split('_')
                     if len(base) > 1:
                         covdrv_index = '\\%s_%s' % (base, subscript)
                 elif len(str(covdrv_index)) > 1:
@@ -923,33 +889,33 @@
                 else:
                     equation[0] += '_{' + covdrv_index + '} '
                     equation[3] += '_{' + covdrv_index + '} '
                 equation[0], equation[3] = equation[0] + latex, equation[3] + latex
             if location == 'RHS' and (self._property['suffix'] or symbol not in self._namespace):
                 with self.scanner.new_context():
                     if index[1] == 'U':
-                        config = ' % assign ' + symbol + ' --deriv dD\n'
+                        config = ' % assign ' + symbol + ' --suffix dD\n'
                         self.parse_latex(''.join(equation) + config)
                     else:
-                        self.parse_latex(self._generate_covdrv(function, index[0], symbol, diacritic))
+                        self.parse_latex(Generator.generate_covdrv(function, index[0], symbol, diacritic))
         return expression
 
     # <LIEDRV> -> <LIE_SYM> '_' <SYMBOL> ( <OPERATOR> | <SUBEXPR> )
     def _liedrv(self, location='RHS'):
         self.expect('LIE_SYM')
         self.expect('UNDERSCORE')
         vector = self._strip(self._symbol())
         func_list, expression = self._expand_product(location, 'ld', vector)
         for symbol, function in func_list:
             if location == 'RHS' and (self._property['suffix'] or symbol not in self._namespace):
                 sentence, position = self.scanner.sentence, self.scanner.mark()
                 symbol = str(function.args[0])
-                tensor = Tensor(function, self._namespace[symbol].dimension)
+                tensor = IndexedSymbol(function, self._namespace[symbol].dimension)
                 tensor.weight = self._namespace[symbol].weight
-                self.parse_latex(self._generate_liedrv(function, vector, tensor.weight))
+                self.parse_latex(Generator.generate_liedrv(function, vector, tensor.weight))
                 self.scanner.initialize(sentence, position)
                 self.scanner.lex()
         return expression
 
     # <TENSOR> -> <SYMBOL> [ ( '_' <INDEXING_4> ) | ( '^' <INDEXING_3> [ '_' <INDEXING_4> ] ) ]
     def _tensor(self, location='RHS'):
         sentence, position = self.scanner.sentence, self.scanner.mark()
@@ -964,30 +930,30 @@
             symbol.extend((len(index) - order) * ['D'])
             if order > 0:
                 sentence = self.scanner.sentence
                 suffix = '_cd' if covariant else '_d'
                 symbol.append(suffix + order * 'D')
                 function = Function('Tensor')(Symbol(''.join(symbol)), *indexing)
                 old_latex = sentence[position:self.scanner.mark()]
-                new_latex = Tensor(function).latex_format(function)
+                new_latex = IndexedSymbol(function).latex_format(function)
                 self.scanner.sentence = sentence.replace(old_latex, new_latex)
                 self.scanner.marker = position
                 self.scanner.reset()
                 return self._operator()
         self.scanner.mark()
         if self.accept('CARET'):
             if self.accept('LBRACE'):
                 if self.accept('LBRACE'):
                     self.scanner.reset()
                     symbol = ''.join(symbol)
                     function = Function('Tensor')(Symbol(symbol, real=True))
                     if symbol in self._namespace:
                         if isinstance(self._namespace[symbol], Function('Constant')):
                             return self._namespace[symbol]
-                    else: self._define_tensor(Tensor(function))
+                    else: self._define_tensor(IndexedSymbol(function))
                     return function
                 self.scanner.reset(); self.scanner.lex()
             index = self._indexing_3()
             indexing.extend(index)
             symbol.extend(len(index) * ['U'])
             if self.accept('UNDERSCORE'):
                 index, order = self._indexing_4()
@@ -998,25 +964,25 @@
                 symbol.extend((len(index) - order) * ['D'])
                 if order > 0:
                     sentence = self.scanner.sentence
                     suffix = '_cd' if covariant else '_d'
                     symbol.append(suffix + order * 'D')
                     function = Function('Tensor')(Symbol(''.join(symbol)), *indexing)
                     old_latex = sentence[position:self.scanner.mark()]
-                    new_latex = Tensor(function).latex_format(function)
+                    new_latex = IndexedSymbol(function).latex_format(function)
                     self.scanner.sentence = sentence.replace(old_latex, new_latex)
                     self.scanner.marker = position
                     self.scanner.reset()
                     return self._operator()
         symbol = ''.join(symbol)
         if symbol in self._namespace:
             if isinstance(self._namespace[symbol], Function('Constant')):
                 return self._namespace[symbol]
         function = Function('Tensor')(Symbol(symbol, real=True), *indexing)
-        tensor = Tensor(function)
+        tensor = IndexedSymbol(function)
         if symbol not in self._namespace and location == 'RHS':
             if symbol[:7] == 'epsilon':
                 # instantiate permutation (Levi-Civita) symbol using parity
                 def sgn(sequence):
                     """ Permutation Signature (Parity)"""
                     cycle_length = 0
                     for n, i in enumerate(sequence[:-1]):
@@ -1030,67 +996,67 @@
                     for i in range(1, tensor.rank + 1))
                 tensor.structure = eval(prefix + suffix, {'sgn': sgn})
                 tensor.dimension = tensor.rank
                 self._define_tensor(tensor)
             else:
                 if tensor.rank > 0:
                     if any(suffix in symbol for suffix in ('_d', '_dup', '_cd', '_ld')):
-                        raise ParseError('cannot index undefined variable \'%s\' at position %d' %
+                        raise ParserError('cannot index undefined variable \'%s\' at position %d' %
                             (symbol, position), sentence, position)
                     i, base_symbol = len(symbol) - 1, symbol
                     while i >= 0:
                         if base_symbol[i] not in ('U', 'D'):
                             base_symbol = base_symbol[:(i + 1)]
                             break
                         i -= 1
-                    for suffix in product(*('UD' if i == 'U' else 'DU' for _, i in Tensor.indexing(function))):
+                    for suffix in product(*('UD' if i == 'U' else 'DU' for _, i in IndexedSymbol.indexing(function))):
                         symbol_RHS = base_symbol + ''.join(suffix)
                         if symbol_RHS in self._namespace:
                             with self.scanner.new_context():
                                 diacritic = 'bar'   if 'bar'   in symbol \
                                        else 'hat'   if 'hat'   in symbol \
                                        else 'tilde' if 'tilde' in symbol \
                                        else ''
                                 metric = self._namespace[symbol_RHS].metric if self._namespace[symbol_RHS].metric else \
                                     self._property['metric'][diacritic] + diacritic
                                 if metric + 'DD' not in self._namespace:
-                                    raise ParseError('cannot raise/lower index for \'%s\' without defined metric at position %d' %
+                                    raise ParserError('cannot raise/lower index for \'%s\' without defined metric at position %d' %
                                         (symbol, position), sentence, position)
                                 indexing_LHS = indexing_RHS = [str(index) for index in indexing]
-                                idx_gen = index_count()
+                                idx_gen = IndexedSymbol.index_count()
                                 for i, index in enumerate(indexing_LHS):
                                     if index in indexing_LHS[:i]:
                                         indexing_LHS[i] = next(x for x in idx_gen if x not in indexing_LHS)
                                 function_LHS = Function('Tensor')(function.args[0],
                                     *(Symbol(i) for i in indexing_LHS))
-                                latex = Tensor.latex_format(function_LHS) + ' = '
-                                for i, (idx, pos) in enumerate(Tensor.indexing(function_LHS)):
+                                latex = IndexedSymbol.latex_format(function_LHS) + ' = '
+                                for i, (idx, pos) in enumerate(IndexedSymbol.indexing(function_LHS)):
                                     if pos != suffix[i]:
                                         indexing_RHS[i] = next(x for x in idx_gen if x not in indexing_LHS)
                                         if '_' in str(idx):
                                             base, subscript = str(idx).split('_')
                                             if len(base) > 1:
                                                 idx = '\\%s_%s' % (base, subscript)
                                         elif len(str(idx)) > 1:
                                             idx = '\\' + str(idx)
                                         if pos == 'U':
                                             latex += '\\mathrm{%s}^{%s %s} ' % (metric, idx, indexing_RHS[i])
                                         else:
                                             latex += '\\mathrm{%s}_{%s %s} ' % (metric, idx, indexing_RHS[i])
-                                latex += Tensor.latex_format(Function('Tensor')(Symbol(symbol_RHS, real=True), *indexing_RHS))
+                                latex += IndexedSymbol.latex_format(Function('Tensor')(Symbol(symbol_RHS, real=True), *indexing_RHS))
                                 suffix = self._namespace[symbol_RHS].suffix
                                 if suffix or self._namespace[symbol_RHS].metric:
                                     latex += ' % assign ' + symbol
                                     if suffix:
-                                        latex += ' --deriv ' + suffix + ' '
+                                        latex += ' --suffix ' + suffix + ' '
                                     if self._namespace[symbol_RHS].metric:
                                         latex += ' --metric ' + metric + ' '
                                 self.parse_latex(latex)
                             return function
-                    raise ParseError('cannot index undefined variable \'%s\' at position %d' %
+                    raise ParserError('cannot index undefined variable \'%s\' at position %d' %
                         (symbol, position), sentence, position)
                 else: self._define_tensor(tensor)
         return function
 
     # <SYMBOL> -> <LETTER> | <SYMB_CMD> '{' <VARIABLE> '}' | <DIACRITIC> '{' <SYMBOL> '}'
     def _symbol(self):
         lexeme = self.scanner.lexeme
@@ -1103,29 +1069,29 @@
             return symbol
         if self.accept('DIACRITIC'):
             self.expect('LBRACE')
             symbol = self._symbol() + lexeme[1:]
             self.expect('RBRACE')
             return symbol
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unexpected \'%s\' at position %d' %
+        raise ParserError('unexpected \'%s\' at position %d' %
             (sentence[position], position), sentence, position)
 
     # <INDEXING_1> -> <LETTER> [ '_' <INDEXING_2> ] | <INTEGER>
     def _indexing_1(self):
         lexeme = self._strip(self.scanner.lexeme)
         if self.accept('LETTER'):
             index = Symbol(lexeme, real=True) if not self.accept('UNDERSCORE') \
                 else Symbol('%s_%s' % (lexeme, self._indexing_2()), real=True)
             return index if index not in self._property['coord'] \
                 else Integer(self._property['coord'].index(index))
         elif self.accept('INTEGER'):
             return Integer(lexeme)
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unexpected \'%s\' at position %d' %
+        raise ParserError('unexpected \'%s\' at position %d' %
             (sentence[position], position), sentence, position)
 
     # <INDEXING_2> -> <LETTER> | <INTEGER> | '{' <INDEXING_1> '}'
     def _indexing_2(self):
         lexeme = self._strip(self.scanner.lexeme)
         if self.accept('LETTER'):
             index = Symbol(lexeme, real=True)
@@ -1134,15 +1100,15 @@
         elif self.accept('INTEGER'):
             return Integer(lexeme)
         elif self.accept('LBRACE'):
             indexing = self._indexing_1()
             self.expect('RBRACE')
             return indexing
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unexpected \'%s\' at position %d' %
+        raise ParserError('unexpected \'%s\' at position %d' %
             (sentence[position], position), sentence, position)
 
     # <INDEXING_3> -> <INDEXING_2> | '{' { <INDEXING_1> }+ '}'
     def _indexing_3(self):
         indexing = []
         if self.accept('LBRACE'):
             while not self.accept('RBRACE'):
@@ -1173,41 +1139,42 @@
             return indexing, order
         return [self._indexing_2()], order
 
     # <VARIABLE> -> <LETTER> { [ '_' ] ( <LETTER> | <INTEGER> ) }*
     def _variable(self):
         variable = self.scanner.lexeme
         self.expect('LETTER')
-        while any(self.peek(token) for token in ('UNDERSCORE', 'LETTER', 'SUFFIX', 'INTEGER')):
+        while any(self.peek(token) for token in ('UNDERSCORE', 'LETTER', 'INTEGER')):
             variable += self.scanner.lexeme
             self.scanner.lex()
         return variable
 
-    # <NUMBER> -> <RATIONAL> | <DECIMAL> | <INTEGER> | <PI>
+    # <NUMBER> -> [ '-' ] ( <RATIONAL> | <DECIMAL> | <INTEGER> | <PI> )
     def _number(self):
+        sign = -1 if self.accept('MINUS') else 1
         number = self.scanner.lexeme
         if self.accept('RATIONAL'):
-            rational = re.match(r'(\-?[0-9]+)\/(\-?[1-9][0-9]*)', number)
-            return Rational(rational.group(1), rational.group(2))
+            rational = re.match(r'([0-9]+)\/([1-9][0-9]*)', number)
+            return sign * Rational(rational.group(1), rational.group(2))
         if self.accept('DECIMAL'):
-            return Float(number)
+            return sign * Float(number)
         if self.accept('INTEGER'):
-            return Integer(number)
+            return sign * Integer(number)
         if self.accept('PI'):
-            return pi
+            return sign * pi
         sentence, position = self.scanner.sentence, self.scanner.mark()
-        raise ParseError('unexpected \'%s\' at position %d' %
+        raise ParserError('unexpected \'%s\' at position %d' %
             (sentence[position], position), sentence, position)
 
-    def _define_tensor(self, tensor, zero=False):
+    def _define_tensor(self, tensor, zeros=False):
         symbol, dimension = tensor.symbol, tensor.dimension
         symmetry = tensor.symmetry if tensor.rank > 1 else None
         if not tensor.structure:
             tensor.structure = Symbol(symbol, real=True) if tensor.rank == 0 \
-                else symdef(tensor.rank, symbol if not zero else None, symmetry, dimension)
+                else symdef(tensor.rank, symbol if not zeros else None, symmetry, dimension)
         self._namespace[symbol] = tensor
         self.state[symbol] = None
 
     def _define_pardrv(self, function, location, suffix, index):
         if suffix is None:
             return Derivative(function, index)
         symbol, indices = str(function.args[0]), list(function.args[1:]) + [index]
@@ -1221,15 +1188,15 @@
                     tree, idx_set = ExprTree(tensor.equation[1]), set()
                     for subtree in tree.preorder():
                         subexpr = subtree.expr
                         if subexpr.func == Function('Tensor'):
                             idx_set.update(subexpr.args[1:])
                     idx_set = {str(i) for i in idx_set}
                     if index in idx_set:
-                        idx_gen = index_count()
+                        idx_gen = IndexedSymbol.index_count()
                         index = next(x for x in idx_gen if x not in idx_set)
                     if '_' in str(index):
                         base, subscript = str(index).split('_')
                         if len(base) > 1:
                             index = '\\%s_%s' % (base, subscript)
                     elif len(str(index)) > 1:
                         index = '\\' + str(index)
@@ -1240,15 +1207,15 @@
         if symbol not in self._namespace:
             symmetry = 'nosym'
             if len(symbol.split(suffix)[1]) == 2:
                 position = len(indices) - 2
                 symmetry = 'sym%d%d' % (position, position + 1)
             if tensor.symmetry and tensor.symmetry != 'nosym':
                 symmetry = tensor.symmetry + ('_' + symmetry if symmetry != 'nosym' else '')
-            self._define_tensor(Tensor(function, tensor.dimension,
+            self._define_tensor(IndexedSymbol(function, tensor.dimension,
                 symmetry=symmetry, suffix=tensor.suffix))
         return function
 
     def _expand_product(self, location, suffix_1, suffix_2, index=None):
         func_list, product = [], None
         if any(self.peek(i) for i in ('LPAREN', 'LBRACK', 'LBRACE')):
             subexpr = self._subexpr()
@@ -1311,278 +1278,14 @@
             else: symbol += '_' + suffix_1
             symbol += suffix_2
             func_list.append((symbol, function))
             product = Function('Tensor')(Symbol(symbol, real=True), *indices)
         return func_list, product
 
     @staticmethod
-    def _separate_indexing(indexing, symbol_LHS, impsum=True):
-        free_index, bound_index = [], []
-        indexing = [(str(idx), pos) for idx, pos in indexing]
-        # iterate over every unique index in the subexpression
-        for index in uniquify([idx for idx, _ in indexing]):
-            count = U = D = 0; index_tuple = []
-            # count index occurrence and position occurrence
-            for index_, position in indexing:
-                if index_ == index:
-                    index_tuple.append((index_, position))
-                    if position == 'U': U += 1
-                    if position == 'D': D += 1
-                    count += 1
-            # identify every bound index on the RHS
-            if count > 1:
-                if impsum and (count != 2 or U != D):
-                    # raise exception upon violation of the following rule:
-                    # a bound index must appear exactly once as a superscript
-                    # and exactly once as a subscript in any single term
-                    raise TensorError('illegal bound index \'%s\' in %s' % (index, symbol_LHS))
-                bound_index.append(index)
-            # identify every free index on the RHS
-            else: free_index.extend(index_tuple)
-        return uniquify(free_index), bound_index
-
-    def _summation(self, LHS, RHS, impsum=True):
-        tree, indexing = ExprTree(LHS), []
-        for subtree in tree.preorder():
-            subexpr = subtree.expr
-            if subexpr.func == Function('Tensor'):
-                for index, position in Tensor.indexing(subexpr):
-                    if re.match(r'[a-zA-Z]+(?:_[0-9]+)?', str(index)):
-                        indexing.append((index, position))
-            elif subexpr.func == Derivative:
-                for index, _ in subexpr.args[1:]:
-                    if index not in self._property['coord']:
-                        if re.match(r'[a-zA-Z]+(?:_[0-9]+)?', str(index)):
-                            indexing.append((index, 'D'))
-        symbol_LHS = Tensor(LHS).symbol
-        # construct a tuple list of every LHS free index
-        free_index_LHS = self._separate_indexing(indexing, symbol_LHS, impsum=impsum)[0] if impsum \
-            else uniquify([(str(idx), pos) for idx, pos in indexing])
-        # construct a tuple list of every RHS free index
-        free_index_RHS = []
-        iterable = RHS.args if RHS.func == Add else [RHS]
-        LHS, RHS = Tensor(LHS).array_format(LHS), srepr(RHS)
-        for element in iterable:
-            index_range = self._property['index'].copy()
-            original = srepr(element)
-            if original[0] == '-':
-                original = original[1:]
-            modified = original
-            indexing = []
-            tree = ExprTree(element)
-            for subtree in tree.preorder():
-                subexpr = subtree.expr
-                if subexpr.func == Function('Tensor'):
-                    symbol = str(subexpr.args[0])
-                    dimension = self._namespace[symbol].dimension
-                    for index in subexpr.args[1:]:
-                        if str(index) in self._property['index']:
-                            dimension = self._property['index'][str(index)]
-                        if str(index) in index_range and dimension != index_range[str(index)]:
-                            raise ParseError('inconsistent loop/summation range for index \'%s\'' %
-                                index, self.scanner.sentence)
-                        index_range[str(index)] = dimension
-                    function = Tensor(subexpr).array_format(subexpr)
-                    modified = modified.replace(srepr(subexpr), function)
-                    for index, position in Tensor.indexing(subexpr):
-                        if re.match(r'[a-zA-Z]+(?:_[0-9]+)?', str(index)):
-                            indexing.append((index, position))
-                elif subexpr.func == Function('Constant'):
-                    constant = str(subexpr.args[0])
-                    modified = modified.replace(srepr(subexpr), constant)
-                elif subexpr.func == Derivative:
-                    argument = subexpr.args[0]
-                    derivative = 'diff(' + srepr(argument)
-                    symbol = str(argument.args[0])
-                    dimension = self._namespace[symbol].dimension
-                    for index, order in subexpr.args[1:]:
-                        if str(index) in self._property['index']:
-                            dimension = self._property['index'][str(index)]
-                        if str(index) in index_range and dimension != index_range[str(index)]:
-                            raise ParseError('inconsistent loop/summation range for index \'%s\'' %
-                                index, self.scanner.sentence)
-                        index_range[str(index)] = dimension
-                        if index not in self._property['coord']:
-                            derivative += ', (coord[%s], %s)' % (index, order)
-                            if re.match(r'[a-zA-Z]+(?:_[0-9]+)?', str(index)):
-                                indexing.append((index, 'D'))
-                        else: derivative += ', (%s, %s)' % (index, order)
-                    derivative += ')'
-                    modified = modified.replace(srepr(subexpr), derivative)
-                    tmp = srepr(subexpr).replace(srepr(argument), Tensor(argument).array_format(argument))
-                    modified = modified.replace(tmp, derivative)
-            if impsum:
-                free_index, bound_index = self._separate_indexing(indexing, symbol_LHS, impsum=impsum)
-                free_index_RHS.append(free_index)
-                # generate implied summation over every bound index
-                for idx in bound_index:
-                    modified = 'sum(%s for %s in range(%d))' % (modified, idx, index_range[idx])
-            else:
-                free_index_RHS.append(indexing)
-            RHS = RHS.replace(original, modified)
-        if impsum:
-            set_LHS = set((str(idx), pos) for idx, pos in free_index_LHS)
-            set_RHS = set((str(idx), pos) for idx, pos in flatten(free_index_RHS))
-            set_diff = set_RHS.symmetric_difference(set_LHS)
-            if len(set_diff) > 0:
-                # raise exception upon violation of the following rule:
-                # a free index must appear in every term with the same
-                # position and cannot be summed over in any term
-                raise TensorError('unbalanced free indices %s in %s' % \
-                    (set(str(idx) for idx, _ in set_diff), symbol_LHS))
-        else:
-            set_LHS = set(str(idx) for idx, _ in free_index_LHS)
-            set_RHS = set(str(idx) for idx, _ in flatten(free_index_RHS))
-            set_diff = set_RHS.difference(set_LHS)
-            if len(set_diff) > 0:
-                # raise exception upon violation of the following rule:
-                # every index on the RHS must appear at least once on
-                # the LHS with the noimpsum annotation applied
-                raise TensorError('unbalanced indices %s in %s' % (set_diff, symbol_LHS))
-        # generate tensor instantiation with implied summation
-        if symbol_LHS in self._namespace:
-            equation = len(free_index_LHS) * '    ' + '%s = %s' % (LHS, RHS)
-            for i, (idx, _) in enumerate(reversed(free_index_LHS)):
-                indent = len(free_index_LHS) - (i + 1)
-                equation = indent * '    ' + 'for %s in range(%d):\n' % (idx, index_range[idx]) + equation
-            equation = [equation]
-        else:
-            for idx, _ in reversed(free_index_LHS):
-                RHS = '[%s for %s in range(%d)]' % (RHS, idx, index_range[idx])
-            equation = [LHS.split('[')[0], RHS]
-        dimension_LHS = None
-        if free_index_LHS:
-            if len(uniquify(index_range[index] for index, _ in free_index_LHS)) > 1:
-                raise ParseError('cannot infer dimension of \'%s\'' % symbol_LHS, self.scanner.sentence)
-            index, _ = free_index_LHS[0]
-            dimension_LHS = index_range[index]
-        # shift tensor indexing forward whenever dimension > upper bound
-        for subtree in tree.preorder():
-            subexpr = subtree.expr
-            if subexpr.func == Function('Tensor'):
-                symbol = str(subexpr.args[0])
-                dimension = self._namespace[symbol].dimension
-                tensor = Tensor(subexpr, dimension)
-                indexing = Tensor.indexing(subexpr)
-                for index in subexpr.args[1:]:
-                    if str(index) in self._property['index']:
-                        upper_bound = self._property['index'][str(index)]
-                        if dimension > upper_bound:
-                            shift = dimension - upper_bound
-                            for i, (idx, pos) in enumerate(indexing):
-                                if str(idx) == str(index):
-                                    indexing[i] = ('%s + %s' % (idx, shift), pos)
-                equation[-1] = equation[-1].replace(tensor.array_format(subexpr), tensor.array_format(indexing))
-        return ' = '.join(equation), dimension_LHS
-
-    @staticmethod
-    def _generate_metric(symbol, dimension, diacritic, suffix):
-        latex_config = ''
-        if 'U' in symbol:
-            prefix = r'\epsilon_{' + ' '.join('i_' + str(i) for i in range(1, 1 + dimension)) + '} ' + \
-                     r'\epsilon_{' + ' '.join('j_' + str(i) for i in range(1, 1 + dimension)) + '} '
-            det_latex = prefix + ' '.join(r'\mathrm{{{symbol}}}^{{i_{n} j_{n}}}'.format(symbol=symbol[:-2], n=i) for i in range(1, 1 + dimension))
-            inv_latex = prefix + ' '.join(r'\mathrm{{{symbol}}}^{{i_{n} j_{n}}}'.format(symbol=symbol[:-2], n=i) for i in range(2, 1 + dimension))
-            latex_config += r"""
-\mathrm{{{symbol}det}} = \frac{{1}}{{({dimension})({factorial})}} {det_latex} \\
-\mathrm{{{symbol}}}_{{i_1 j_1}} = \frac{{1}}{{{factorial}}} \mathrm{{{symbol}det}}^{{{{-1}}}} ({inv_latex})""" \
-                .format(symbol=symbol[:-2], inv_symbol=symbol.replace('U', 'D'), dimension=dimension,
-                    factorial=math.factorial(dimension - 1), det_latex=det_latex, inv_latex=inv_latex)
-            latex_config += '\n' + r"% assign {symbol}det --dim {dimension}".format(symbol=symbol[:-2], dimension=dimension)
-            if suffix:
-                latex_config += '\n' + r"% assign {symbol}det {inv_symbol} --deriv {suffix}" \
-                    .format(suffix=suffix, symbol=symbol[:-2], inv_symbol=symbol.replace('U', 'D'))
-        else:
-            prefix = r'\epsilon^{' + ' '.join('i_' + str(i) for i in range(1, 1 + dimension)) + '} ' + \
-                     r'\epsilon^{' + ' '.join('j_' + str(i) for i in range(1, 1 + dimension)) + '} '
-            det_latex = prefix + ' '.join(r'\mathrm{{{symbol}}}_{{i_{n} j_{n}}}'.format(symbol=symbol[:-2], n=i) for i in range(1, 1 + dimension))
-            inv_latex = prefix + ' '.join(r'\mathrm{{{symbol}}}_{{i_{n} j_{n}}}'.format(symbol=symbol[:-2], n=i) for i in range(2, 1 + dimension))
-            latex_config += r"""
-\mathrm{{{symbol}det}} = \frac{{1}}{{({dimension})({factorial})}} {det_latex} \\
-\mathrm{{{symbol}}}^{{i_1 j_1}} = \frac{{1}}{{{factorial}}} \mathrm{{{symbol}det}}^{{{{-1}}}} ({inv_latex})""" \
-                .format(symbol=symbol[:-2], inv_symbol=symbol.replace('D', 'U'), dimension=dimension,
-                    factorial=math.factorial(dimension - 1), det_latex=det_latex, inv_latex=inv_latex)
-            latex_config += '\n' + r"% assign {symbol}det --dim {dimension}".format(symbol=symbol[:-2], dimension=dimension)
-            if suffix:
-                latex_config += '\n' + r"% assign {symbol}det {inv_symbol} --deriv {suffix}" \
-                    .format(suffix=suffix, symbol=symbol[:-2], inv_symbol=symbol.replace('D', 'U'))
-        metric = '\\mathrm{' + re.split(r'[UD]', symbol)[0] + '}'
-        latex_config += '\n' + r'\mathrm{{Gamma{diacritic}}}^{{i_1}}_{{i_2 i_3}} = \frac{{1}}{{2}} {metric}^{{i_1 i_4}} (\partial_{{i_2}} {metric}_{{i_3 i_4}} + \partial_{{i_3}} {metric}_{{i_4 i_2}} - \partial_{{i_4}} {metric}_{{i_2 i_3}})'.format(metric=metric, diacritic=diacritic)
-        return latex_config
-
-    @staticmethod
-    def _generate_covdrv(function, covdrv_index, symbol=None, diacritic=None):
-        indexing = [str(index) for index in function.args[1:]] + [str(covdrv_index)]
-        idx_gen = index_count()
-        for i, index in enumerate(indexing):
-            if index in indexing[:i]:
-                indexing[i] = next(x for x in idx_gen if x not in indexing)
-        covdrv_index = indexing[-1]
-        if '_' in str(covdrv_index):
-            base, subscript = str(covdrv_index).split('_')
-            if len(base) > 1:
-                covdrv_index = '\\%s_%s' % (base, subscript)
-        elif len(str(covdrv_index)) > 1:
-            covdrv_index = '\\' + str(covdrv_index)
-        latex = Tensor.latex_format(Function('Tensor')(function.args[0],
-            *(Symbol(i) for i in indexing[:-1])))
-        LHS = ('\\%s{\\nabla}' % diacritic if diacritic else '\\nabla') + ('_{%s} %s' % (covdrv_index, latex))
-        RHS = '\\partial_{%s} %s' % (covdrv_index, latex)
-        for index, (_, position) in zip(indexing, Tensor.indexing(function)):
-            idx_gen = index_count()
-            bound_index = next(x for x in idx_gen if x not in indexing)
-            latex = Tensor.latex_format(Function('Tensor')(function.args[0],
-                *(Symbol(bound_index) if i == index else Symbol(i) for i in indexing[:-1])))
-            if '_' in str(index):
-                base, subscript = str(index).split('_')
-                if len(base) > 1:
-                    index = '\\%s_%s' % (base, subscript)
-            elif len(str(index)) > 1:
-                index = '\\' + str(index)
-            RHS += ' + ' if position == 'U' else ' - '
-            RHS += '\\%s{\\mathrm{Gamma}}' % diacritic if diacritic else '\\mathrm{Gamma}'
-            if position == 'U':
-                RHS += '^{%s}_{%s %s} (%s)' % (index, bound_index, covdrv_index, latex)
-            else:
-                RHS += '^{%s}_{%s %s} (%s)' % (bound_index, index, covdrv_index, latex)
-        config = (' % assign ' + symbol + ' --deriv dD\n') if symbol else ''
-        return LHS + ' = ' + RHS + config
-
-    @staticmethod
-    def _generate_liedrv(function, vector, weight=None):
-        if len(str(vector)) > 1:
-            vector = '\\mathrm{' + str(vector) + '}'
-        indexing = [str(index) for index, _ in Tensor.indexing(function)]
-        idx_gen = index_count()
-        for i, index in enumerate(indexing):
-            if index in indexing[:i]:
-                indexing[i] = next(x for x in idx_gen if x not in indexing)
-        latex = Tensor.latex_format(function)
-        LHS = '\\mathcal{L}_%s %s' % (vector, latex)
-        bound_index = next(x for x in idx_gen if x not in indexing)
-        RHS = '%s^{%s} \\partial_{%s} %s' % (vector, bound_index, bound_index, latex)
-        for index, position in Tensor.indexing(function):
-            latex = Tensor.latex_format(Function('Tensor')(function.args[0],
-                *(Symbol(bound_index) if i == str(index) else Symbol(i) for i in indexing)))
-            if '_' in str(index):
-                base, subscript = str(index).split('_')
-                if len(base) > 1:
-                    index = '\\%s_%s' % (base, subscript)
-            elif len(str(index)) > 1:
-                index = '\\' + str(index)
-            if position == 'U':
-                RHS += ' - (\\partial_{%s} %s^{%s}) %s' % (bound_index, vector, index, latex)
-            else:
-                RHS += ' + (\\partial_{%s} %s^{%s}) %s' % (index, vector, bound_index, latex)
-        if weight:
-            latex = Tensor.latex_format(function)
-            RHS += ' + (%s)(\\partial_{%s} %s^{%s}) %s' % (weight, bound_index, vector, bound_index, latex)
-        return LHS + ' = ' + RHS
-
-    @staticmethod
     def _strip(symbol):
         return symbol[1:] if symbol[0] == '\\' else symbol
 
     def peek(self, token):
         if self.scanner.token is None and token == 'LINEBREAK':
             return True
         return self.scanner.token == token
@@ -1592,204 +1295,14 @@
             self.scanner.lex()
             return True
         return False
 
     def expect(self, token):
         if not self.accept(token):
             sentence, position = self.scanner.sentence, self.scanner.mark()
-            raise ParseError('expected token %s at position %d' %
+            raise ParserError('expected token %s at position %d' %
                 (token, position), sentence, position)
 
-def index_count():
-    n = 1
-    while True:
-        yield 'i_' + str(n)
-        n += 1
-
-class ParseError(Exception):
-    """ Invalid LaTeX Sentence """
+class ParserError(NRPyLaTeXError):
 
     def __init__(self, message, sentence=None, position=None):
-        if position is not None:
-            length = 0
-            for _, substring in enumerate(sentence.split('\n')):
-                if position - length <= len(substring):
-                    sentence = substring.lstrip()
-                    position += len(sentence) - len(substring) - length
-                    break
-                length += len(substring) + 1
-            super(ParseError, self).__init__('%s\n%s^\n' % (sentence, (12 + position) * ' ') + message)
-        else: super(ParseError, self).__init__(message)
-
-class TensorError(Exception):
-    """ Invalid Tensor Indexing or Dimension """
-
-class OverrideWarning(UserWarning):
-    """ Overridden Namespace Variable """
-
-def _formatwarning(message, category, filename=None, lineno=None, file=None, line=None):
-    return '%s: %s\n' % (category.__name__, message)
-warnings.formatwarning = _formatwarning
-warnings.simplefilter('always', OverrideWarning)
-
-class Tensor:
-    """ Tensor Structure """
-
-    def __init__(self, function, dimension=None, structure=None, equation=None,
-            symmetry=None, suffix=None, metric=None, weight=None, impsum=True):
-        self.overridden  = False
-        self.symbol      = str(function.args[0])
-        self.rank        = 0
-        for symbol in re.split(r'_d|_dup|_cd|_ld', self.symbol):
-            for character in reversed(symbol):
-                if character in ('U', 'D'):
-                    self.rank += 1
-                else: break
-        self.dimension   = dimension
-        self.structure   = structure
-        self.equation    = equation
-        self.symmetry    = symmetry
-        self.suffix      = suffix
-        self.metric      = metric
-        self.weight      = weight
-        self.impsum      = impsum
-
-    @staticmethod
-    def indexing(function):
-        """ Tensor Indexing from SymPy Function """
-        symbol, indices = function.args[0], function.args[1:]
-        i, indexing = len(indices) - 1, []
-        for symbol in reversed(re.split(r'_d|_dup|_cd|_ld', str(symbol))):
-            for character in reversed(symbol):
-                if character in ('U', 'D'):
-                    indexing.append((indices[i], character))
-                else: break
-                i -= 1
-        return list(reversed(indexing))
-
-    # TODO change method type to static (class) method
-    def array_format(self, function):
-        """ Tensor Notation for Array Formatting """
-        if isinstance(function, Function('Tensor')):
-            indexing = self.indexing(function)
-        else: indexing = function
-        if not indexing:
-            return self.symbol
-        return self.symbol + ''.join(['[' + str(index) + ']' for index, _ in indexing])
-
-    @staticmethod
-    def latex_format(function):
-        """ Tensor Notation for LaTeX Formatting """
-        symbol, indexing = str(function.args[0]), Tensor.indexing(function)
-        operator, i_2 = '', len(symbol)
-        for i_1 in range(len(symbol), 0, -1):
-            subsym = symbol[i_1:i_2]
-            if '_d' in subsym:
-                suffix = re.split('_d|_dup', subsym)[-1]
-                for _ in reversed(suffix):
-                    index = str(indexing.pop()[0])
-                    if '_' in index:
-                        base, subscript = index.split('_')
-                        if len(base) > 1:
-                            index = '\\%s_{%s}' % (base, subscript)
-                    elif len(index) > 1:
-                        index = '\\' + index
-                    operator += '\\partial_{' + index + '} '
-                i_2 = i_1
-            elif '_cd' in subsym:
-                suffix = subsym.split('_cd')[-1]
-                diacritic = 'bar'   if 'bar'   in suffix \
-                       else 'hat'   if 'hat'   in suffix \
-                       else 'tilde' if 'tilde' in suffix \
-                       else None
-                if diacritic:
-                    suffix = suffix[len(diacritic):]
-                for position in reversed(suffix):
-                    index = str(indexing.pop()[0])
-                    if '_' in index:
-                        base, subscript = index.split('_')
-                        if len(base) > 1:
-                            index = '\\%s_{%s}' % (base, subscript)
-                    elif len(index) > 1:
-                        index = '\\' + index
-                    operator += '\\' + diacritic + '{\\nabla}' if diacritic \
-                        else '\\nabla'
-                    if position == 'U':
-                        operator += '^{' + index + '}'
-                    else:
-                        operator += '_{' + index + '}'
-                    operator += ' '
-                i_2 = i_1
-            elif '_ld' in subsym:
-                vector = re.split('_ld', subsym)[-1]
-                if len(vector) > 1:
-                    vector = '\\mathrm{' + vector + '}'
-                operator += '\\mathcal{L}_' + vector + ' '
-                i_2 = i_1
-        symbol = re.split(r'_d|_dup|_cd|_ld', symbol)[0]
-        for i, character in enumerate(reversed(symbol)):
-            if character not in ('U', 'D'):
-                symbol = symbol[:len(symbol) - i]; break
-        latex = [symbol, [], []]
-        if len(latex[0]) > 1:
-            latex[0] = '\\mathrm{' + str(latex[0]) + '}'
-        latex[0] = operator + latex[0]
-        U_count, D_count = 0, 0
-        for index, position in indexing:
-            index = str(index)
-            if '_' in index:
-                base, subscript = index.split('_')
-                if len(base) > 1:
-                    index = '\\%s_{%s}' % (base, subscript)
-            elif len(index) > 1:
-                index = '\\' + index
-            if position == 'U':
-                latex[1].append(index)
-                U_count += 1
-            else:
-                latex[2].append(index)
-                D_count += 1
-        latex[1] = ' '.join(latex[1])
-        latex[2] = ' '.join(latex[2])
-        if U_count > 0:
-            latex[1] = '^{' + latex[1] + '}'
-        if D_count > 0:
-            latex[2] = '_{' + latex[2] + '}'
-        return ''.join(latex)
-
-    def __repr__(self):
-        symbol = ('*' if self.overridden else '') + self.symbol
-        if self.rank == 0:
-            return 'Scalar(%s)' % symbol
-        return 'Tensor(%s, %dD)' % (symbol, self.dimension)
-
-    __str__ = __repr__
-
-class CoordinateSystem(list):
-    """ Coordinate System (Default List) """
-
-    def __init__(self, symbol):
-        self.symbol = symbol
-
-    def default(self, n):
-        return Symbol('%s_%d' % (self.symbol, n), real=True)
-
-    def index(self, value):
-        pattern = re.match(self.symbol + '_([0-9][0-9]*)', str(value))
-        if pattern is not None:
-            return pattern.group(1)
-        return list.index(self, value)
-
-    def __missing__(self, index):
-        return self.default(index)
-
-    def __getitem__(self, index):
-        try:
-            return list.__getitem__(self, index)
-        except IndexError:
-            return self.__missing__(index)
-
-    def __contains__(self, key):
-        return list.__contains__(self, key) or re.match(self.symbol + '_[0-9][0-9]*', str(key))
-
-    def __eq__(self, other):
-        return list.__eq__(self, other) and self.symbol == other.symbol
+        super(ParserError, self).__init__(message, sentence, position)
```

### Comparing `nrpylatex-1.2.6/nrpylatex/core/scanner.py` & `nrpylatex-1.3/nrpylatex/core/scanner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ NRPyLaTeX Scanner """
 # Author: Ken Sible
 # Email:  ksible *at* outlook *dot* com
 
+from nrpylatex.utils.exceptions import NRPyLaTeXError
 import re
 
 class Scanner:
-    """ The following class will tokenize a LaTeX sentence for parsing. """
 
     def __init__(self):
         # define a regex pattern for every token, create a named capture group for
         # every pattern, join together the resulting pattern list using a pipe symbol
         # for regex alternation, and compile the generated regular expression
         symmetry = r'nosym|(?:sym|anti)[0-9]+(?:_(?:sym|anti)[0-9]+)*'
         alphabet = '|'.join(letter for letter in (r'\\[aA]lpha', r'\\[bB]eta', r'\\[gG]amma', r'\\[dD]elta',
@@ -19,17 +19,17 @@
             r'\\varphi', r'\\varpi', r'\\varrho', r'\\varsigma', r'\\vartheta', r'[a-zA-Z]'))
         self.token_dict = [
             ('LINEBREAK',       r'\r?\n'),
             ('WHITESPACE',      r'\s+'),
             ('SYMMETRY',        symmetry),
             ('STRING',          r'\"[^\"]*\"'),
             ('GROUP',           r'\<[0-9]+(\.{2})?\>'),
-            ('RATIONAL',        r'\-?[0-9]+\/\-?[1-9][0-9]*'),
-            ('DECIMAL',         r'\-?[0-9]+\.[0-9]+'),
-            ('INTEGER',         r'\-?[0-9]+'),
+            ('RATIONAL',        r'[0-9]+\/\-?[1-9][0-9]*'),
+            ('DECIMAL',         r'[0-9]+\.[0-9]+'),
+            ('INTEGER',         r'[0-9]+'),
             ('ARROW',           r'\-\>'),
             ('PLUS',            r'\+'),
             ('MINUS',           r'\-'),
             ('DIVIDE',          r'\/'),
             ('EQUAL',           r'\='),
             ('CARET',           r'\^'),
             ('UNDERSCORE',      r'\_'),
@@ -43,38 +43,36 @@
             ('LBRACK',          r'\['),
             ('RBRACK',          r'\]'),
             ('LBRACE',          r'\{'),
             ('RBRACE',          r'\}'),
             ('PAR_SYM',         r'\\partial'),
             ('COV_SYM',         r'\\nabla'),
             ('LIE_SYM',         r'\\mathcal\{L\}'),
-            ('SYMB_CMD',        r'\\mathrm|\\text'),
+            ('SYMB_CMD',        r'\\mathrm'),
             ('FUNC_CMD',        r'\\exp'),
             ('FRAC_CMD',        r'\\frac'),
             ('SQRT_CMD',        r'\\sqrt'),
             ('NLOG_CMD',        r'\\ln|\\log'),
             ('TRIG_CMD',        r'\\sinh|\\cosh|\\tanh|\\sin|\\cos|\\tan'),
             ('DEFINE_MACRO',    r'define'),
             ('ASSIGN_MACRO',    r'assign'),
             ('IGNORE_MACRO',    r'ignore'),
             ('SREPL_MACRO',     r'srepl'),
             ('INDEX_MACRO',     r'index'),
             ('COORD_MACRO',     r'coord'),
-            ('ZERO',            r'zero'),
-            ('KRON',            r'kron'),
+            ('ZEROS',           r'zeros'),
             ('CONST',           r'const'),
             ('DIM',             r'dim'),
             ('SYM',             r'sym'),
             ('WEIGHT',          r'weight'),
-            ('DERIV',           r'deriv'),
+            ('SUFFIX',          r'suffix'),
             ('METRIC',          r'metric'),
             ('DEFAULT',         r'default'),
             ('PERSIST',         r'persist'),
             ('NOIMPSUM',        r'noimpsum'),
-            ('SUFFIX',          r'none|dD|dupD'),
             ('DIACRITIC',       r'\\hat|\\tilde|\\bar'),
             ('PI',              r'\\pi'),
             ('LETTER',          alphabet),
             ('COMMAND',         r'\\[a-zA-Z]+'),
             ('NEWLINE',         r'\\{2}'),
             ('BACKSLASH',       r'\\')]
         self.regex = re.compile('|'.join(['(?P<%s>%s)' % pattern for pattern in self.token_dict]))
@@ -97,15 +95,15 @@
         """ Tokenize Sentence
 
             :return: token iterator
         """
         while self.index < len(self.sentence):
             token = self.regex.match(self.sentence, self.index)
             if token is None:
-                raise ScanError('unexpected \'%s\' at position %d' %
+                raise ScannerError('unexpected \'%s\' at position %d' %
                     (self.sentence[self.index], self.index), self.sentence, self.index)
             self.index = token.end()
             if self.whitespace or token.lastgroup not in ('WHITESPACE', 'LINEBREAK'):
                 self.lexeme = token.group()
                 yield token.lastgroup
 
     def lex(self):
@@ -157,21 +155,11 @@
 
         def __enter__(self): return
 
         def __exit__(self, exc_type, exc_value, exc_tb):
             self.scanner.initialize(*self.state)
             self.scanner.lex()
 
-class ScanError(Exception):
-    """ Invalid LaTeX Sentence """
+class ScannerError(NRPyLaTeXError):
 
     def __init__(self, message, sentence=None, position=None):
-        if position is not None:
-            length = 0
-            for _, substring in enumerate(sentence.split('\n')):
-                if position - length <= len(substring):
-                    sentence = substring.lstrip()
-                    position += len(sentence) - len(substring) - length
-                    break
-                length += len(substring) + 1
-            super(ScanError, self).__init__('%s\n%s^\n' % (sentence, (12 + position) * ' ') + message)
-        else: super(ScanError, self).__init__(message)
+        super(ScannerError, self).__init__(message, sentence, position)
```

### Comparing `nrpylatex-1.2.6/nrpylatex/tests/test_parse_latex.py` & `nrpylatex-1.3/nrpylatex/tests/test_parse_latex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-""" parse_latex.py Unit Testing """
+""" NRPyLaTeX Unit Testing """
 # Author: Ken Sible
 # Email:  ksible *at* outlook *dot* com
 
-from nrpylatex.core.assertion import assert_equal
+from nrpylatex.utils.assertion import assert_equal
 import nrpylatex as nl, sympy as sp, unittest
-parse_latex = lambda sentence: nl.parse_latex(sentence, reset=True, ignore_warning=True)
+parse_latex = lambda sentence: nl.parse_latex(sentence, reset=True)
 
 class TestParser(unittest.TestCase):
 
     def setUp(self):
         self.maxDiff = None
 
     def test_expression_1(self):
         expr = r'-(\frac{2}{3} + 2\sqrt[5]{x + 3})'
         self.assertEqual(
             str(parse_latex(expr)),
             '-2*(x + 3)**(1/5) - 2/3'
         )
 
     def test_expression_2(self):
-        expr = r'e^{\ln x} + \sin(\sin^{-1} y) - \tanh(xy)'
+        expr = r'e^{\ln{x}} + \sin{\sin^{-1}{y}} - \tanh{xy}'
         self.assertEqual(
             str(parse_latex(expr)),
             'x + y - tanh(x*y)'
         )
 
     def test_expression_3(self):
         expr = r'\partial_x (x^2 + 2x)'
@@ -31,79 +31,79 @@
             str(parse_latex(expr).doit()),
             '2*x + 2'
         )
 
     def test_expression_4(self):
         function = sp.Function('Tensor')(sp.Symbol('T'))
         self.assertEqual(
-            nl.Parser._generate_covdrv(function, 'beta'),
+            nl.Generator.generate_covdrv(function, 'beta'),
             r'\nabla_{\beta} T = \partial_{\beta} T'
         )
         function = sp.Function('Tensor')(sp.Symbol('TUU'), sp.Symbol('mu'), sp.Symbol('nu'))
         self.assertEqual(
-            nl.Parser._generate_covdrv(function, 'beta'),
+            nl.Generator.generate_covdrv(function, 'beta'),
             r'\nabla_{\beta} T^{\mu \nu} = \partial_{\beta} T^{\mu \nu} + \mathrm{Gamma}^{\mu}_{i_1 \beta} (T^{i_1 \nu}) + \mathrm{Gamma}^{\nu}_{i_1 \beta} (T^{\mu i_1})'
         )
         function = sp.Function('Tensor')(sp.Symbol('TUD'), sp.Symbol('mu'), sp.Symbol('nu'))
         self.assertEqual(
-            nl.Parser._generate_covdrv(function, 'beta'),
+            nl.Generator.generate_covdrv(function, 'beta'),
             r'\nabla_{\beta} T^{\mu}_{\nu} = \partial_{\beta} T^{\mu}_{\nu} + \mathrm{Gamma}^{\mu}_{i_1 \beta} (T^{i_1}_{\nu}) - \mathrm{Gamma}^{i_1}_{\nu \beta} (T^{\mu}_{i_1})'
         )
         function = sp.Function('Tensor')(sp.Symbol('TDD'), sp.Symbol('mu'), sp.Symbol('nu'))
         self.assertEqual(
-            nl.Parser._generate_covdrv(function, 'beta'),
+            nl.Generator.generate_covdrv(function, 'beta'),
             r'\nabla_{\beta} T_{\mu \nu} = \partial_{\beta} T_{\mu \nu} - \mathrm{Gamma}^{i_1}_{\mu \beta} (T_{i_1 \nu}) - \mathrm{Gamma}^{i_1}_{\nu \beta} (T_{\mu i_1})'
         )
 
     def test_expression_5(self):
         parse_latex(r"""
-            % define gDD --dim 4 --deriv dD --metric
-            % define vU --dim 4 --deriv dD
+            % define gDD --dim 4 --suffix dD --metric
+            % define vU --dim 4 --suffix dD
             % index b --dim 4
             T^\mu_b = \nabla_b v^\mu
         """)
         function = sp.Function('Tensor')(sp.Symbol('vU_cdD'), sp.Symbol('mu'), sp.Symbol('b'))
         self.assertEqual(
-            nl.Parser._generate_covdrv(function, 'a'),
+            nl.Generator.generate_covdrv(function, 'a'),
             r'\nabla_{a} \nabla_{b} v^{\mu} = \partial_{a} \nabla_{b} v^{\mu} + \mathrm{Gamma}^{\mu}_{i_1 a} (\nabla_{b} v^{i_1}) - \mathrm{Gamma}^{i_1}_{b a} (\nabla_{i_1} v^{\mu})'
         )
 
     def test_expression_6(self):
         function = sp.Function('Tensor')(sp.Symbol('g'))
         self.assertEqual(
-            nl.Parser._generate_liedrv(function, 'beta', 2),
+            nl.Generator.generate_liedrv(function, 'beta', 2),
             r'\mathcal{L}_\mathrm{beta} g = \mathrm{beta}^{i_1} \partial_{i_1} g + (2)(\partial_{i_1} \mathrm{beta}^{i_1}) g'
         )
         function = sp.Function('Tensor')(sp.Symbol('gUU'), sp.Symbol('i'), sp.Symbol('j'))
         self.assertEqual(
-            nl.Parser._generate_liedrv(function, 'beta'),
+            nl.Generator.generate_liedrv(function, 'beta'),
             r'\mathcal{L}_\mathrm{beta} g^{i j} = \mathrm{beta}^{i_1} \partial_{i_1} g^{i j} - (\partial_{i_1} \mathrm{beta}^{i}) g^{i_1 j} - (\partial_{i_1} \mathrm{beta}^{j}) g^{i i_1}'
         )
         function = sp.Function('Tensor')(sp.Symbol('gUD'), sp.Symbol('i'), sp.Symbol('j'))
         self.assertEqual(
-            nl.Parser._generate_liedrv(function, 'beta'),
+            nl.Generator.generate_liedrv(function, 'beta'),
             r'\mathcal{L}_\mathrm{beta} g^{i}_{j} = \mathrm{beta}^{i_1} \partial_{i_1} g^{i}_{j} - (\partial_{i_1} \mathrm{beta}^{i}) g^{i_1}_{j} + (\partial_{j} \mathrm{beta}^{i_1}) g^{i}_{i_1}'
         )
         function = sp.Function('Tensor')(sp.Symbol('gDD'), sp.Symbol('i'), sp.Symbol('j'))
         self.assertEqual(
-            nl.Parser._generate_liedrv(function, 'beta'),
+            nl.Generator.generate_liedrv(function, 'beta'),
             r'\mathcal{L}_\mathrm{beta} g_{i j} = \mathrm{beta}^{i_1} \partial_{i_1} g_{i j} + (\partial_{i} \mathrm{beta}^{i_1}) g_{i_1 j} + (\partial_{j} \mathrm{beta}^{i_1}) g_{i i_1}'
         )
 
     def test_srepl_macro(self):
         nl.parse_latex(r"""
             % srepl "<1>'" -> "\mathrm{<1>prime}" --persist
             % srepl "\mathrm{<1..>}_<2>" -> "\mathrm{(<1..>)<2>}" --persist
             % srepl "<1>_{<2>}" -> "<1>_<2>" --persist
             % srepl "<1>_<2>" -> "\mathrm{<1>_<2>}" --persist
             % srepl "\mathrm{(<1..>)<2>}" -> "\mathrm{<1..>_<2>}" --persist
             % srepl "<1>^{<2>}" -> "<1>^<2>" --persist
             % srepl "<1>^<2>" -> "<1>^{{<2>}}" --persist
         """)
-        expr = r"x_n^4 + x'_n \exp(x_n y_n^2)"
+        expr = r"x_n^4 + x'_n \exp{x_n y_n^2}"
         self.assertEqual(
             str(nl.parse_latex(expr)),
             "x_n**4 + xprime_n*exp(x_n*y_n**2)"
         )
         parse_latex(r""" % srepl "<1>'^{<2..>}" -> "\mathrm{<1>prime}" --persist """)
         expr = r"v'^{label}"
         self.assertEqual(
@@ -111,90 +111,90 @@
             "vprime"
         )
 
     def test_assignment_1(self):
         self.assertEqual(
             set(parse_latex(r"""
                 % index --default --dim 2
-                % define vU wU --dim 2 --deriv dD
+                % define vU wU --dim 2 --suffix dD
                 T^{ab}_c = \partial_c (v^a w^b)
             """)),
             {'vU', 'wU', 'vU_dD', 'wU_dD', 'TUUD'}
         )
         self.assertEqual(str(TUUD[0][0][0]),
             'vU0*wU_dD00 + vU_dD00*wU0'
         )
 
     def test_assignment_2(self):
         self.assertEqual(
             set(parse_latex(r"""
                 % index --default --dim 2
-                % define vU --dim 2 --deriv dD
+                % define vU --dim 2 --suffix dD
                 % define w --const
-                T^a_c = % deriv dupD
+                T^a_c = % suffix dupD
                 \partial_c (v^a w)
             """)),
             {'w', 'vU', 'vU_dupD', 'TUD'}
         )
         self.assertEqual(str(TUD),
             '[[vU_dupD00*w, vU_dupD01*w], [vU_dupD10*w, vU_dupD11*w]]'
         )
 
     def test_assignment_3(self):
         self.assertEqual(
             set(parse_latex(r"""
                 % index --default --dim 4
-                % define gDD --dim 4 --deriv dD --metric
-                % define vU --dim 4 --deriv dD
+                % define gDD --dim 4 --suffix dD --metric
+                % define vU --dim 4 --suffix dD
                 T^{ab} = \nabla^b v^a
             """)),
             {'gUU', 'gdet', 'epsilonUUUU', 'gDD', 'vU', 'vU_dD', 'gDD_dD', 'GammaUDD', 'vU_cdD', 'vU_cdU', 'TUU'}
         )
 
     def test_assignment_4(self):
         self.assertEqual(
             set(parse_latex(r"""
                 % coord [x, y]
                 % index --default --dim 2
                 % define uD wD --dim 2
                 u_x = x^2 + 2x \\
                 u_y = y\sqrt{x} \\
                 v_a = u_a + w_a \\
-                % assign wD vD --deriv dD
+                % assign wD vD --suffix dD
                 T_{ab} = \partial_b v_a
             """)),
             {'x', 'y', 'uD', 'wD', 'vD', 'vD_dD', 'wD_dD', 'TDD'}
         )
         self.assertEqual(str(TDD),
             '[[wD_dD00 + 2*x + 2, wD_dD01], [wD_dD10 + y/(2*sqrt(x)), wD_dD11 + sqrt(x)]]'
         )
 
     def test_assignment_5(self):
         self.assertEqual(
             set(parse_latex(r"""
                 % index --default --dim 2
-                % define vD uD wD --dim 2 --deriv dD
+                % define vD uD wD --dim 2 --suffix dD
                 T_{abc} = ((v_a + u_a)_{,b} - w_{a,b})_{,c}
             """)),
             {'vD', 'uD', 'wD', 'TDDD', 'uD_dD', 'vD_dD', 'wD_dD', 'wD_dDD', 'uD_dDD', 'vD_dDD'}
         )
         self.assertEqual(str(TDDD[0][0][0]),
             'uD_dDD000 + vD_dDD000 - wD_dDD000'
         )
 
     def test_assignment_6(self):
         parse_latex(r"""
             % coord [\theta, \phi]
             % index --default --dim 2
-            % define gDD --dim 2 --zero
+            % define gDD --dim 2 --zeros
             % define r --const
             % ignore "\begin{align*}" "\end{align*}"
             \begin{align*}
                 g_{0 0} &= r^2 \\
-                g_{1 1} &= r^2 \sin^2(\theta)
+                g_{1 1} &= r^2 \sin^2{\theta}
             \end{align*}
             % assign gDD --metric
             \begin{align*}
                 R^\alpha_{\beta\mu\nu} &= \partial_\mu \Gamma^\alpha_{\beta\nu} - \partial_\nu \Gamma^\alpha_{\beta\mu} + \Gamma^\alpha_{\mu\gamma}\Gamma^\gamma_{\beta\nu} - \Gamma^\alpha_{\nu\sigma}\Gamma^\sigma_{\beta\mu} \\
                 R_{\alpha\beta\mu\nu} &= g_{\alpha a} R^a_{\beta\mu\nu} \\
                 R_{\beta\nu} &= R^\alpha_{\beta\alpha\nu} \\
                 R &= g^{\beta\nu} R_{\beta\nu}
@@ -269,51 +269,52 @@
             'vD2'
         )
 
     def test_assignment_11(self):
         self.assertEqual(
             set(parse_latex(r"""
                 % coord [x, y, z]
-                % define vD --dim 3 --zero
+                % define vD --dim 3 --zeros
                 v_z = y^2 + 2y \\
                 w = v_{x_2}
             """)),
             {'vD', 'y', 'w'}
         )
         self.assertEqual(str(w),
             'y**2 + 2*y'
         )
 
     def test_assignment_12(self):
         self.assertEqual(
             set(parse_latex(r"""
-                % define deltaDD --dim 3 --kron
+                % define deltaDD --dim 3 --zeros
+                \delta_{ii} = 1 % noimpsum
                 % \hat{\gamma}_{ij} = \delta_{ij}
                 % assign gammahatDD --metric
-                % define hDD --dim 3 --deriv dD --sym sym01
+                % define hDD --dim 3 --suffix dD --sym sym01
                 % \bar{\gamma}_{ij} = h_{ij} + \hat{\gamma}_{ij}
-                % assign gammabarDD --deriv dD --metric
+                % assign gammabarDD --suffix dD --metric
             """)),
             {'gammabardet', 'GammabarUDD', 'gammabarDD', 'gammabarDD_dD', 'gammahatdet', 'hDD', 'GammahatUDD', 'hDD_dD', 'gammahatUU', 'deltaDD', 'gammabarUU', 'epsilonUUU', 'gammahatDD'}
         )
 
     def test_assignment_13(self):
         self.assertEqual(
             set(parse_latex(r"""
                 % coord [r, \theta, \phi]
                 % define vD --dim 3
                 % v_0 = 1
                 % v_1 = r
-                % v_2 = r \sin \theta
+                % v_2 = r \sin{\theta}
                 % R_{ij} = v_i v_j
-                % define gammahatDD --dim 3 --zero
+                % define gammahatDD --dim 3 --zeros
                 % \hat{\gamma}_{ii} = R_{ii} % noimpsum
-                % define hDD --dim 3 --deriv dD
+                % define hDD --dim 3 --suffix dD
                 % \bar{\gamma}_{ij} = h_{ij} R_{ij} + \hat{\gamma}_{ij} % noimpsum
-                % assign gammabarDD --deriv dD
+                % assign gammabarDD --suffix dD
                 T_{ijk} = \partial_k \bar{\gamma}_{ij}
             """)),
             {'gammabarDD_dD', 'RDD', 'r', 'vD', 'theta', 'gammahatDD', 'TDDD', 'hDD', 'gammabarDD', 'hDD_dD'}
         )
         self.assertEqual(str(gammahatDD),
             '[[1, 0, 0], [0, r**2, 0], [0, 0, r**2*sin(theta)**2]]'
         )
@@ -358,54 +359,54 @@
         self.assertEqual(str(uD),
             '[vU1*wU2 - vU2*wU1, -vU0*wU2 + vU2*wU0, vU0*wU1 - vU1*wU0]'
         )
 
     def test_example_4(self):
         self.assertEqual(
             set(parse_latex(r"""
-                % define FUU --dim 4 --deriv dD --sym anti01
-                % define gDD --dim 4 --deriv dD --metric
+                % define FUU --dim 4 --suffix dD --sym anti01
+                % define gDD --dim 4 --suffix dD --metric
                 % define k --const
                 J^\mu = (4\pi k)^{-1} F^{\mu\nu}_{;\nu}
             """)),
             {'FUU', 'gUU', 'gdet', 'epsilonUUUU', 'gDD', 'k', 'FUU_dD', 'gDD_dD', 'GammaUDD', 'FUU_cdD', 'JU'}
         )
         self.assertEqual(
             set(parse_latex(r"""
-                % define FUU --dim 4 --deriv dD --sym anti01
-                % define gDD --dim 4 --deriv dD --metric
+                % define FUU --dim 4 --suffix dD --sym anti01
+                % define gDD --dim 4 --suffix dD --metric
                 % define k --const
                 J^\mu = (4\pi k)^{-1} \nabla_\nu F^{\mu\nu}
             """)),
             {'FUU', 'gUU', 'gdet', 'epsilonUUUU', 'gDD', 'k', 'FUU_dD', 'gDD_dD', 'GammaUDD', 'FUU_cdD', 'JU'}
         )
         self.assertEqual(
             set(parse_latex(r"""
-                % define FUU --dim 4 --deriv dD --sym anti01
-                % define ghatDD --dim 4 --deriv dD --metric
+                % define FUU --dim 4 --suffix dD --sym anti01
+                % define ghatDD --dim 4 --suffix dD --metric
                 % define k --const
                 J^\mu = (4\pi k)^{-1} \hat{\nabla}_\nu F^{\mu\nu}
             """)),
             {'FUU', 'ghatUU', 'ghatdet', 'epsilonUUUU', 'k',  'ghatDD', 'FUU_dD', 'ghatDD_dD', 'GammahatUDD', 'FUU_cdhatD', 'JU'}
         )
 
     def test_example_5_1(self):
         nl.parse_latex(r"""
             % coord [t, r, \theta, \phi]
-            % define gDD --dim 4 --zero
+            % define gDD --dim 4 --zeros
             % define G M --const
             % ignore "\begin{align}" "\end{align}"
             \begin{align}
                 g_{t t} &= -\left(1 - \frac{2GM}{r}\right) \\
                 g_{r r} &=  \left(1 - \frac{2GM}{r}\right)^{-1} \\
                 g_{\theta \theta} &= r^2 \\
-                g_{\phi \phi} &= r^2 \sin^2\theta
+                g_{\phi \phi} &= r^2 \sin^2{\theta}
             \end{align}
             % assign gDD --metric
-        """, ignore_warning=True)
+        """)
         self.assertEqual(str(gDD[0][0]),
             '2*G*M/r - 1'
         )
         self.assertEqual(str(gDD[1][1]),
             '1/(-2*G*M/r + 1)'
         )
         self.assertEqual(str(gDD[2][2]),
@@ -423,15 +424,15 @@
             \begin{align}
                 R^\alpha{}_{\beta\mu\nu} &= \partial_\mu \Gamma^\alpha_{\beta\nu} - \partial_\nu \Gamma^\alpha_{\beta\mu} + \Gamma^\alpha_{\mu\gamma}\Gamma^\gamma_{\beta\nu} - \Gamma^\alpha_{\nu\sigma}\Gamma^\sigma_{\beta\mu} \\
                 K &= R^{\alpha\beta\mu\nu} R_{\alpha\beta\mu\nu} \\
                 R_{\beta\nu} &= R^\alpha_{\beta\alpha\nu} \\
                 R &= g^{\beta\nu} R_{\beta\nu} \\
                 G_{\beta\nu} &= R_{\beta\nu} - \frac{1}{2}g_{\beta\nu}R
             \end{align}
-        """, ignore_warning=True)
+        """)
         assert_equal(GammaUDD[0][0][1] - GammaUDD[0][1][0], 0, suppress_message=True)
         self.assertEqual(str(GammaUDD[0][0][1]),
             '-G*M/(r**2*(2*G*M/r - 1))'
         )
         self.assertEqual(str(GammaUDD[1][0][0]),
             'G*M*(-2*G*M/r + 1)/r**2'
         )
@@ -472,46 +473,46 @@
                 \gamma_{ij} &= g_{ij} \\
                 % assign gammaDD --metric
                 \beta_i &= g_{0 i} \\
                 \alpha &= \sqrt{\gamma^{ij}\beta_i\beta_j - g_{0 0}} \\
                 K_{ij} &= \frac{1}{2\alpha}\left(\nabla_i \beta_j + \nabla_j \beta_i\right) \\
                 K &= \gamma^{ij} K_{ij}
             \end{align}
-        """, ignore_warning=True)
+        """)
         for i in range(3):
             for j in range(3):
                 assert_equal(KDD[i][j], 0, suppress_message=True)
 
     def test_example_6_2(self):
         nl.parse_latex(r"""
             \begin{align}
                 R_{ij} &= \partial_k \Gamma^k_{ij} - \partial_j \Gamma^k_{ik}
                     + \Gamma^k_{ij}\Gamma^l_{kl} - \Gamma^l_{ik}\Gamma^k_{lj} \\
                 R &= \gamma^{ij} R_{ij} \\
                 E &= \frac{1}{16\pi}\left(R + K^{{2}} - K_{ij}K^{ij}\right) \\
                 p_i &= \frac{1}{8\pi}\left(D_j \gamma^{jk} K_{ki} - D_i K\right)
             \end{align}
-        """, ignore_warning=True)
+        """)
         # assert_equal(E, 0, suppress_message=True)
         self.assertEqual(sp.simplify(E), 0)
         for i in range(3):
             assert_equal(pD[i], 0, suppress_message=True)
 
     @staticmethod
     def test_metric_symmetry():
         parse_latex(r"""
-            % define gDD --dim 3 --zero
+            % define gDD --dim 3 --zeros
             g_{1 0} = 1 \\
             g_{2 0} = 2
             % assign gDD --metric
         """)
         assert_equal(gDD[0][1], 1, suppress_message=True)
         assert_equal(gDD[0][2], 2, suppress_message=True)
         parse_latex(r"""
-            % define gDD --dim 3 --zero
+            % define gDD --dim 3 --zeros
             g_{0 1} = 1 \\
             g_{0 2} = 2
             % assign gDD --metric
         """)
         assert_equal(gDD[1][0], 1, suppress_message=True)
         assert_equal(gDD[2][0], 2, suppress_message=True)
```

### Comparing `nrpylatex-1.2.6/nrpylatex.egg-info/PKG-INFO` & `nrpylatex-1.3/nrpylatex.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrpylatex
-Version: 1.2.6
+Version: 1.3
 Summary: LaTeX Interface to SymPy (CAS) for General Relativity
 Home-page: https://github.com/zachetienne/nrpylatex
 Author: Ken Sible
 Author-email: ksible@outlook.com
 License: BSD License (BSD)
 Keywords: General Relativity,LaTeX,CAS
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,22 @@
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![NRPyLaTeX Logo](/docs/imgs/logo.png)
+[![NRPyLaTeX Logo](https://raw.githubusercontent.com/zachetienne/nrpylatex/main/docs/imgs/logo.png)](https://zachetienne.github.io/nrpylatex/)
 
 ---
 
 [![CI](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml/badge.svg)](https://github.com/zachetienne/nrpylatex/actions/workflows/main.yaml)
-[![pypi version](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb)
+[![PyPI](https://img.shields.io/pypi/v/nrpylatex.svg)](https://pypi.org/project/nrpylatex/)
 [![arXiv](https://img.shields.io/badge/arXiv-2111.05861-B31B1B)](https://arxiv.org/abs/2111.05861)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=notebook%2FNRPyLaTeX%20Tutorial.ipynb)
 
 [NRPy+](https://github.com/zachetienne/nrpytutorial)'s LaTeX Interface to SymPy (CAS) for General Relativity
 
 - automatic expansion of
   - [Einstein summation convention](https://en.wikipedia.org/wiki/Einstein_notation)
   - Levi-Civita and Christoffel symbols
   - Lie and covariant derivatives
@@ -54,62 +54,62 @@
     for var in namespace:
         exec(f'{var} = mathematica_code({var})')
 
 If you are using a different CAS, reference the SymPy [documentation](https://docs.sympy.org/latest/modules/printing.html) to find the relevant printing function.
 
 ## &#167; Interactive Tutorial (MyBinder)
 
-[Quick Start](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=notebook%2FNRPyLaTeX%20Tutorial.ipynb) | [NRPy+ Integration](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-SymPy_LaTeX_Interface.ipynb) | [Guided Example (BSSN Formalism)](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-LaTeX_Interface_Example-BSSN_Cartesian.ipynb)
+[Quick Start](https://mybinder.org/v2/gh/zachetienne/nrpylatex.git/HEAD?filepath=docs%2FNRPyLaTeX%20Tutorial.ipynb) | [NRPy+ Integration](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-SymPy_LaTeX_Interface.ipynb) | [Guided Example (BSSN Formalism)](https://mybinder.org/v2/gh/zachetienne/nrpytutorial/HEAD?filepath=Tutorial-LaTeX_Interface_Example-BSSN_Cartesian.ipynb)
 
 ## &#167; Documentation and Usage
 
 [Getting Started and API Reference](https://zachetienne.github.io/nrpylatex/)
 
 ### Simple Example ([Kretschmann Scalar](https://en.wikipedia.org/wiki/Kretschmann_scalar))
 
 **Python REPL or Script (*.py)**
 
     >>> from nrpylatex import parse_latex
     >>> parse_latex(r"""
     ...     % ignore "\begin{align}" "\end{align}"
     ...     \begin{align}
     ...         % coord [t, r, \theta, \phi]
-    ...         % define gDD --dim 4 --zero
+    ...         % define gDD --dim 4 --zeros
     ...         % define G M --const
     ...         %% define Schwarzschild metric diagonal
     ...         g_{t t} &= -\left(1 - \frac{2GM}{r}\right) \\
     ...         g_{r r} &=  \left(1 - \frac{2GM}{r}\right)^{-1} \\
     ...         g_{\theta \theta} &= r^2 \\
-    ...         g_{\phi \phi} &= r^2 \sin^2\theta \\
+    ...         g_{\phi \phi} &= r^2 \sin^2{\theta} \\
     ...         %% generate metric inverse gUU, determinant det(gDD), and connection GammaUDD
     ...         % assign gDD --metric
     ...         R^\alpha{}_{\beta \mu \nu} &= \partial_\mu \Gamma^\alpha_{\beta \nu} - \partial_\nu \Gamma^\alpha_{\beta \mu}
     ...             + \Gamma^\alpha_{\mu \gamma} \Gamma^\gamma_{\beta \nu} - \Gamma^\alpha_{\nu \sigma} \Gamma^\sigma_{\beta \mu} \\
     ...         K &= R^{\alpha \beta \mu \nu} R_{\alpha \beta \mu \nu}
     ...     \end{align}
     ... """)
     ('G', 'GammaUDD', 'gDD', 'gUU', 'epsilonUUUU', 'RUDDD', 'K', 'RUUUU', 'M', 'r', 'theta', 'RDDDD', 'gdet')
     >>> from sympy import simplify
     >>> print(simplify(K))
     48*G**2*M**2/r**6
 
 **IPython REPL or Jupyter Notebook**
 
-    In [1]: %load_ext nrpylatex.extension
+    In [1]: %load_ext nrpylatex
     In [2]: %%parse_latex
        ...: % ignore "\begin{align}" "\end{align}"
        ...: \begin{align}
        ...:     % coord [t, r, \theta, \phi]
-       ...:     % define gDD --dim 4 --zero
+       ...:     % define gDD --dim 4 --zeros
        ...:     % define G M --const
        ...:     %% define Schwarzschild metric diagonal
        ...:     g_{t t} &= -\left(1 - \frac{2GM}{r}\right) \\
        ...:     g_{r r} &=  \left(1 - \frac{2GM}{r}\right)^{-1} \\
        ...:     g_{\theta \theta} &= r^2 \\
-       ...:     g_{\phi \phi} &= r^2 \sin^2\theta \\
+       ...:     g_{\phi \phi} &= r^2 \sin^2{\theta} \\
        ...:     %% generate metric inverse gUU, determinant det(gDD), and connection GammaUDD
        ...:     % assign gDD --metric
        ...:     R^\alpha{}_{\beta \mu \nu} &= \partial_\mu \Gamma^\alpha_{\beta \nu} - \partial_\nu \Gamma^\alpha_{\beta \mu}
        ...:         + \Gamma^\alpha_{\mu \gamma} \Gamma^\gamma_{\beta \nu} - \Gamma^\alpha_{\nu \sigma} \Gamma^\sigma_{\beta \mu} \\
        ...:     K &= R^{\alpha \beta \mu \nu} R_{\alpha \beta \mu \nu}
        ...: \end{align}
     Out[2]: ('G', 'GammaUDD', 'gDD', 'gUU', 'epsilonUUUU', 'RUDDD', 'K', 'RUUUU', 'M', 'r', 'theta', 'RDDDD', 'gdet')
```

### Comparing `nrpylatex-1.2.6/nrpylatex.egg-info/SOURCES.txt` & `nrpylatex-1.3/nrpylatex.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 nrpylatex/parse_latex.py
 nrpylatex.egg-info/PKG-INFO
 nrpylatex.egg-info/SOURCES.txt
 nrpylatex.egg-info/dependency_links.txt
 nrpylatex.egg-info/requires.txt
 nrpylatex.egg-info/top_level.txt
 nrpylatex/core/__init__.py
-nrpylatex/core/assertion.py
-nrpylatex/core/exprtree.py
-nrpylatex/core/functional.py
-nrpylatex/core/indexed_symbol.py
+nrpylatex/core/generator.py
 nrpylatex/core/parser.py
 nrpylatex/core/scanner.py
-nrpylatex/extension/__init__.py
-nrpylatex/extension/parse_magic.py
 nrpylatex/tests/__init__.py
-nrpylatex/tests/test_parse_latex.py
+nrpylatex/tests/test_parse_latex.py
+nrpylatex/utils/__init__.py
+nrpylatex/utils/assertion.py
+nrpylatex/utils/exceptions.py
+nrpylatex/utils/functional.py
+nrpylatex/utils/structures.py
```

### Comparing `nrpylatex-1.2.6/setup.py` & `nrpylatex-1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # HERE = pathlib.Path(__file__).parent
 # README = (HERE / "README.md").read_text()
 with open('README.md') as README:
     long_description = README.read()
 
 setup(
     name="nrpylatex",
-    version="1.2.6",
+    version="1.3",
     description="LaTeX Interface to SymPy (CAS) for General Relativity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zachetienne/nrpylatex",
     author="Ken Sible",
     author_email="ksible@outlook.com",
     license="BSD License (BSD)",
-    packages=["nrpylatex", "nrpylatex.core", "nrpylatex.extension", "nrpylatex.tests"],
+    packages=["nrpylatex", "nrpylatex.core", "nrpylatex.utils", "nrpylatex.tests"],
     install_requires=["sympy"],
     keywords=['General Relativity', 'LaTeX', 'CAS'],
     classifiers=[
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
```

