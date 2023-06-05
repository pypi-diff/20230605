# Comparing `tmp/stockwell-1.0.7.tar.gz` & `tmp/stockwell-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockwell-1.0.7.tar", last modified: Wed Jul 27 17:24:27 2022, max compression
+gzip compressed data, was "stockwell-1.1.tar", last modified: Mon Jun  5 13:44:01 2023, max compression
```

## Comparing `stockwell-1.0.7.tar` & `stockwell-1.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:27.193891 stockwell-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-07-27 17:24:20.000000 stockwell-1.0.7/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21782 2022-07-27 17:24:20.000000 stockwell-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-07-27 17:24:20.000000 stockwell-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-07-27 17:24:27.193891 stockwell-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-07-27 17:24:20.000000 stockwell-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-07-27 17:24:20.000000 stockwell-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-07-27 17:24:27.193891 stockwell-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-07-27 17:24:20.000000 stockwell-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:27.193891 stockwell-1.0.7/stockwell/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-27 17:24:27.193891 stockwell-1.0.7/stockwell/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:27.189891 stockwell-1.0.7/stockwell/c_libs/
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/c_libs/sinemodule.c
--rw-r--r--   0 runner    (1001) docker     (121)     8704 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/c_libs/st.c
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/c_libs/st_types.h
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/c_libs/stmodule.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:27.189891 stockwell-1.0.7/stockwell/lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:27.189891 stockwell-1.0.7/stockwell/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-07-27 17:24:20.000000 stockwell-1.0.7/stockwell/tests/test_stockwell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 17:24:27.189891 stockwell-1.0.7/stockwell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-07-27 17:24:27.000000 stockwell-1.0.7/stockwell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-27 17:24:27.000000 stockwell-1.0.7/stockwell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 17:24:27.000000 stockwell-1.0.7/stockwell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-27 17:24:27.000000 stockwell-1.0.7/stockwell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-27 17:24:27.000000 stockwell-1.0.7/stockwell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    70144 2022-07-27 17:24:20.000000 stockwell-1.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 13:43:54.000000 stockwell-1.1/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-05 13:43:54.000000 stockwell-1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-05 13:43:54.000000 stockwell-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-05 13:44:01.197198 stockwell-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-05 13:43:54.000000 stockwell-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-05 13:43:54.000000 stockwell-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 13:44:01.197198 stockwell-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-05 13:43:54.000000 stockwell-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/c_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/c_libs/sine.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/c_libs/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/c_libs/st_types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/lib_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/tests/test_stockwell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-05 13:43:54.000000 stockwell-1.1/versioneer.py
```

### Comparing `stockwell-1.0.7/PKG-INFO` & `stockwell-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockwell
-Version: 1.0.7
+Version: 1.1
 Summary: Time-frequency analysis through Stockwell transform
 Home-page: https://github.com/claudiodsf/stockwell
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: CeCILL Free Software License Agreement, Version 2.1
 Description: # Stockwell
         
@@ -12,37 +12,34 @@
         
         Based on original code from [NIMH MEG Core Facility].
         
         [![cf-badge]][cf-link]
         [![PyPI-badge]][PyPI-link]
         [![license-badge]][license-link]
         
-        
         ## Installation
         
         ### Using Anaconda
         
         If you use [Anaconda], the latest release of Stockwell is available via
         [conda-forge][cf-link].
         
         To install, simply run:
         
             conda install -c conda-forge stockwell
         
-        
         ### Using pip and PyPI
         
         The latest release of Stockwell is available on the
         [Python Package Index][PyPI-link].
         
         You can install it easily through `pip`:
         
             pip install stockwell
         
-        
         ### Installation from source
         
         If no precompiled package is available for you architecture on PyPI, or if you
         want to work on the source code, you will need to compile this package from
         source.
         
         To obtain the source code, download the latest release from the
@@ -85,15 +82,14 @@
         
             pip install .
         
         Or, alternatively, in "editable" mode:
         
             pip install -e .
         
-        
         ## Usage
         
         Example usage:
         
         ```python
         import numpy as np
         from scipy.signal import chirp
@@ -135,33 +131,30 @@
         ax[1].plot(t, w - inv_stock)
         ax[1].set_xlim(0, 10)
         ax[1].set(xlabel='time (s)', ylabel='amplitude difference')
         plt.show()
         ```
         ![inv_stockwell.png](https://cdn.jsdelivr.net/gh/claudiodsf/stockwell/inv_stockwell.png)
         
-        
         ## References
         
         Stockwell, R.G., Mansinha, L. & Lowe, R.P., 1996. Localization of the complex
         spectrum: the S transform, IEEE Trans. Signal Process., 44(4), 998–1001,
         doi:[10.1109/78.492555](https://doi.org/10.1109/78.492555)
         
         [S transform on Wikipedia].
         
-        
-        
         [NIMH MEG Core Facility]: https://kurage.nimh.nih.gov/meglab/Meg/Stockwell
         
         [cf-badge]: http://img.shields.io/conda/vn/conda-forge/stockwell.svg
         [cf-link]: https://anaconda.org/conda-forge/stockwell
         [PyPI-badge]: http://img.shields.io/pypi/v/stockwell.svg
         [PyPI-link]: https://pypi.python.org/pypi/stockwell
-        [license-badge]: https://img.shields.io/badge/license-CeCILL--2.1-green
-        [license-link]: http://www.cecill.info/licences.en.html
+        [license-badge]: https://img.shields.io/badge/license-GPLv3-green
+        [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
         [releases-link]: https://github.com/claudiodsf/stockwell/releases
         
         [Anaconda]: https://www.anaconda.com/products/individual
         [Microsoft C++ Build Tools]:
         https://visualstudio.microsoft.com/visual-cpp-build-tools
         [FFTW]: http://www.fftw.org
         [S transform on Wikipedia]: https://en.wikipedia.org/wiki/S_transform
@@ -173,10 +166,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `stockwell-1.0.7/README.md` & `stockwell-1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,37 +4,34 @@
 
 Based on original code from [NIMH MEG Core Facility].
 
 [![cf-badge]][cf-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
 
-
 ## Installation
 
 ### Using Anaconda
 
 If you use [Anaconda], the latest release of Stockwell is available via
 [conda-forge][cf-link].
 
 To install, simply run:
 
     conda install -c conda-forge stockwell
 
-
 ### Using pip and PyPI
 
 The latest release of Stockwell is available on the
 [Python Package Index][PyPI-link].
 
 You can install it easily through `pip`:
 
     pip install stockwell
 
-
 ### Installation from source
 
 If no precompiled package is available for you architecture on PyPI, or if you
 want to work on the source code, you will need to compile this package from
 source.
 
 To obtain the source code, download the latest release from the
@@ -77,15 +74,14 @@
 
     pip install .
 
 Or, alternatively, in "editable" mode:
 
     pip install -e .
 
-
 ## Usage
 
 Example usage:
 
 ```python
 import numpy as np
 from scipy.signal import chirp
@@ -127,33 +123,30 @@
 ax[1].plot(t, w - inv_stock)
 ax[1].set_xlim(0, 10)
 ax[1].set(xlabel='time (s)', ylabel='amplitude difference')
 plt.show()
 ```
 ![inv_stockwell.png](inv_stockwell.png)
 
-
 ## References
 
 Stockwell, R.G., Mansinha, L. & Lowe, R.P., 1996. Localization of the complex
 spectrum: the S transform, IEEE Trans. Signal Process., 44(4), 998–1001,
 doi:[10.1109/78.492555](https://doi.org/10.1109/78.492555)
 
 [S transform on Wikipedia].
 
-
-
 [NIMH MEG Core Facility]: https://kurage.nimh.nih.gov/meglab/Meg/Stockwell
 
 [cf-badge]: http://img.shields.io/conda/vn/conda-forge/stockwell.svg
 [cf-link]: https://anaconda.org/conda-forge/stockwell
 [PyPI-badge]: http://img.shields.io/pypi/v/stockwell.svg
 [PyPI-link]: https://pypi.python.org/pypi/stockwell
-[license-badge]: https://img.shields.io/badge/license-CeCILL--2.1-green
-[license-link]: http://www.cecill.info/licences.en.html
+[license-badge]: https://img.shields.io/badge/license-GPLv3-green
+[license-link]: https://www.gnu.org/licenses/gpl-3.0.html
 [releases-link]: https://github.com/claudiodsf/stockwell/releases
 
 [Anaconda]: https://www.anaconda.com/products/individual
 [Microsoft C++ Build Tools]:
 https://visualstudio.microsoft.com/visual-cpp-build-tools
 [FFTW]: http://www.fftw.org
 [S transform on Wikipedia]: https://en.wikipedia.org/wiki/S_transform
```

### Comparing `stockwell-1.0.7/pyproject.toml` & `stockwell-1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 [tool.cibuildwheel.macos]
 before-all = 'brew install fftw'
 
 [tool.cibuildwheel.windows]
 before-all = '%CONDA%\Scripts\conda.exe install fftw'
 before-build = 'pip install delvewheel'
 repair-wheel-command = 'delvewheel repair --add-path %CONDA%\Library\bin -w {dest_dir} {wheel}'
-# test-requires = 'nose'
-# test-command = 'nosetests stockwell'
+test-requires = ''
+test-command = 'python -m stockwell.tests.test_stockwell'
```

### Comparing `stockwell-1.0.7/setup.py` & `stockwell-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 # -*- coding: utf-8 -*-
 """setup.py: setuptools control."""
-import sys
 import os
 from setuptools import setup
 from distutils.core import Extension
 import versioneer
-try:
-    import numpy
-except ImportError:
-    sys.exit('NumPy is required for installation. Please install it first.')
 
 with open('README.md', 'rb') as f:
     long_descr = f.read().decode('utf-8').replace(
         '(stockwell.png)',
         '(https://cdn.jsdelivr.net/gh/claudiodsf/stockwell/stockwell.png)'
     ).replace(
         '(inv_stockwell.png)',
         '(https://cdn.jsdelivr.net/gh/claudiodsf/stockwell/inv_stockwell.png)'
     )
 
-include_dirs_st = [numpy.get_include()]
+include_dirs_st = []
 library_dirs_st = []
 # This seems necessary only for Windows
 if 'CONDA_PREFIX' in os.environ:
     include_dirs_st.append(
         os.path.join(os.environ['CONDA_PREFIX'], 'Library', 'include'))
     library_dirs_st.append(
         os.path.join(os.environ['CONDA_PREFIX'], 'Library', 'lib'))
 # This is needed for Miniconda on GitHub-hosted Windows runner
 if 'CONDA' in os.environ:
     include_dirs_st.append(
         os.path.join(os.environ['CONDA'], 'Library', 'include'))
     library_dirs_st.append(
         os.path.join(os.environ['CONDA'], 'Library', 'lib'))
 
-ext_modules = []
-ext_modules.append(Extension(
-    'st',
-    sources=['stockwell/c_libs/st.c', 'stockwell/c_libs/stmodule.c'],
-    include_dirs=include_dirs_st,
-    library_dirs=library_dirs_st,
-    libraries=['fftw3']
-    ))
-ext_modules.append(Extension(
-    'sine',
-    sources=['stockwell/c_libs/sinemodule.c'],
-    include_dirs=[numpy.get_include()]
-    ))
+ext_modules = [
+    Extension(
+        'st',
+        sources=['stockwell/c_libs/st.c'],
+        include_dirs=include_dirs_st,
+        library_dirs=library_dirs_st,
+        libraries=['fftw3'],
+    ),
+    Extension(
+        'sine',
+        sources=['stockwell/c_libs/sine.c'],
+    )
+]
 
 setup(
     name='stockwell',
     packages=['stockwell', 'stockwell.tests'],
     include_package_data=True,
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
@@ -73,11 +68,12 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics'],
     install_requires=['numpy>=1.18']
     )
```

### Comparing `stockwell-1.0.7/stockwell/c_libs/st.c` & `stockwell-1.1/stockwell/c_libs/st.c`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <math.h>
 #include <fftw3.h>
 #include "st_types.h"
 
+// the following is for Windows
+void PyInit_st() {}
+
 char *Wisfile = NULL;
 #if defined(WIN32) || defined(_WIN32) || defined(__WIN32__) || defined(__NT__)
 	const char *Wistemplate = "%s\.fftwis";
 #else
 	const char *Wistemplate = "%s/.fftwis";
 #endif
 #define WISLEN 8
@@ -62,14 +65,20 @@
 number of time points, and it need not be a power of two. The lo and hi
 arguments specify the range of frequencies to return, in samples. If they are
 both zero, they default to lo = 0 and hi = len / 2. The result is
 returned in the complex array result, which must be preallocated, with
 n rows and len columns, where n is hi - lo + 1. For the default values of
 lo and hi, n is len / 2 + 1. */
 
+#ifdef __cplusplus
+extern "C"
+#endif
+#ifdef _MSC_VER
+__declspec(dllexport)
+#endif
 void st(int len, int lo, int hi, double gamma, enum WINDOW window_code, double *data, double *result)
 {
 	int i, k, n, l2;
 	double s, *p;
 	FILE *wisdom;
 	static int planlen = 0;
 	static double *g;
@@ -223,14 +232,20 @@
 {
 	return 1/(1+((m * m * gamma  / n) * (m * m * gamma  / n)));
 }
 
 
 /* Inverse Stockwell transform. */
 
+#ifdef __cplusplus
+extern "C"
+#endif
+#ifdef _MSC_VER
+__declspec(dllexport)
+#endif
 void ist(int len, int lo, int hi, double *data, double *result)
 {
 	int i, n, l2;
 	double *p;
 	FILE *wisdom;
 	static int planlen = 0;
 	static fftw_plan p2;
@@ -310,14 +325,20 @@
 	for (i = 0; i < len; i++) {
 		*p++ = h[i][0] / len;
 	}
 }
 
 /* This does just the Hilbert transform. */
 
+#ifdef __cplusplus
+extern "C"
+#endif
+#ifdef _MSC_VER
+__declspec(dllexport)
+#endif
 void hilbert(int len, double *data, double *result)
 {
 	int i, l2;
 	double *p;
 	FILE *wisdom;
 	static int planlen = 0;
 	static fftw_plan p1, p2;
```

### Comparing `stockwell-1.0.7/stockwell.egg-info/PKG-INFO` & `stockwell-1.1/stockwell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockwell
-Version: 1.0.7
+Version: 1.1
 Summary: Time-frequency analysis through Stockwell transform
 Home-page: https://github.com/claudiodsf/stockwell
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: CeCILL Free Software License Agreement, Version 2.1
 Description: # Stockwell
         
@@ -12,37 +12,34 @@
         
         Based on original code from [NIMH MEG Core Facility].
         
         [![cf-badge]][cf-link]
         [![PyPI-badge]][PyPI-link]
         [![license-badge]][license-link]
         
-        
         ## Installation
         
         ### Using Anaconda
         
         If you use [Anaconda], the latest release of Stockwell is available via
         [conda-forge][cf-link].
         
         To install, simply run:
         
             conda install -c conda-forge stockwell
         
-        
         ### Using pip and PyPI
         
         The latest release of Stockwell is available on the
         [Python Package Index][PyPI-link].
         
         You can install it easily through `pip`:
         
             pip install stockwell
         
-        
         ### Installation from source
         
         If no precompiled package is available for you architecture on PyPI, or if you
         want to work on the source code, you will need to compile this package from
         source.
         
         To obtain the source code, download the latest release from the
@@ -85,15 +82,14 @@
         
             pip install .
         
         Or, alternatively, in "editable" mode:
         
             pip install -e .
         
-        
         ## Usage
         
         Example usage:
         
         ```python
         import numpy as np
         from scipy.signal import chirp
@@ -135,33 +131,30 @@
         ax[1].plot(t, w - inv_stock)
         ax[1].set_xlim(0, 10)
         ax[1].set(xlabel='time (s)', ylabel='amplitude difference')
         plt.show()
         ```
         ![inv_stockwell.png](https://cdn.jsdelivr.net/gh/claudiodsf/stockwell/inv_stockwell.png)
         
-        
         ## References
         
         Stockwell, R.G., Mansinha, L. & Lowe, R.P., 1996. Localization of the complex
         spectrum: the S transform, IEEE Trans. Signal Process., 44(4), 998–1001,
         doi:[10.1109/78.492555](https://doi.org/10.1109/78.492555)
         
         [S transform on Wikipedia].
         
-        
-        
         [NIMH MEG Core Facility]: https://kurage.nimh.nih.gov/meglab/Meg/Stockwell
         
         [cf-badge]: http://img.shields.io/conda/vn/conda-forge/stockwell.svg
         [cf-link]: https://anaconda.org/conda-forge/stockwell
         [PyPI-badge]: http://img.shields.io/pypi/v/stockwell.svg
         [PyPI-link]: https://pypi.python.org/pypi/stockwell
-        [license-badge]: https://img.shields.io/badge/license-CeCILL--2.1-green
-        [license-link]: http://www.cecill.info/licences.en.html
+        [license-badge]: https://img.shields.io/badge/license-GPLv3-green
+        [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
         [releases-link]: https://github.com/claudiodsf/stockwell/releases
         
         [Anaconda]: https://www.anaconda.com/products/individual
         [Microsoft C++ Build Tools]:
         https://visualstudio.microsoft.com/visual-cpp-build-tools
         [FFTW]: http://www.fftw.org
         [S transform on Wikipedia]: https://en.wikipedia.org/wiki/S_transform
@@ -173,10 +166,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `stockwell-1.0.7/versioneer.py` & `stockwell-1.1/versioneer.py`

 * *Files identical despite different names*

