# Comparing `tmp/ecape-0.0.4.tar.gz` & `tmp/ecape-0.0.5.tar.gz`

## Comparing `ecape-0.0.4.tar` & `ecape-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.4/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.4/.ruff_cache/content/a29a86d92757c5f3
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.4/src/ecape/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.4/src/ecape/__init__.py
--rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 ecape-0.0.4/src/ecape/calc.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.4/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 ecape-0.0.4/README.md
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 ecape-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 ecape-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.5/.ruff_cache/content/a29a86d92757c5f3
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.5/src/ecape/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.5/src/ecape/__init__.py
+-rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 ecape-0.0.5/src/ecape/calc.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ecape-0.0.5/README.md
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 ecape-0.0.5/PKG-INFO
```

### Comparing `ecape-0.0.4/src/ecape/calc.py` & `ecape-0.0.5/src/ecape/calc.py`

 * *Files identical despite different names*

### Comparing `ecape-0.0.4/LICENSE.txt` & `ecape-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.4/README.md` & `ecape-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # ecape
 
 ecape is a simple module that contains an entraining CAPE, or ECAPE, calculation described by Peters et. al. 2023.
-Additionally, Peters et. al. 2023 -provided MatLab scripts serve as a reference and test verification data.
-The module leans heavily on Metpy for meteorological calculations.
+Additionally, Peters-provided MatLab scripts serve as a reference and test verification data.
+The module leans heavily on MetPy for meteorological calculations.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ecape.svg)](https://pypi.org/project/ecape)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ecape.svg)](https://pypi.org/project/ecape)
 
 ## Installation & Use
 
+In console:
 
 ```console
 pip install ecape
 ```
 
-See the example in linked documentation:
+See the example in linked documentation.
 
 ```python
    from ecape.calc import calc_ecape
    ...
    ecape = calc_ecape(height, pressure, temperature, specific_humidity, u_wind, v_wind, cape_type)
 ```
 
@@ -40,15 +41,15 @@
 
 ### Future Work
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
 ### Disclaimer
 There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
-This is primarily due to a difference in calculated CAPE. The tests describe other sources of error.
+This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
 
 Since:
  - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
  - Peters et. al. specifically mention MetPy for determining CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
 MetPy's CAPE calculations were chosen for ease of readability and implementation.
```

### Comparing `ecape-0.0.4/pyproject.toml` & `ecape-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,33 +9,30 @@
 packages = ["src/ecape", "docs", "tests"]
 
 [project]
 name = "ecape"
 dynamic = ["version"]
 description = 'Calculate the entraining CAPE (ECAPE) of a parcel.'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Robert Capella", email = "bob.capella@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "MetPy==1.5.0",
+  "MetPy>=1.2.0",
   "numpy>=1.18.0",
   "pytest"
 ]
 
 [project.urls]
 Documentation = "https://citylikeamradio.github.io/ecape"
 Issues = "https://github.com/citylikeamradio/ecape/issues"
@@ -58,15 +55,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
```

### Comparing `ecape-0.0.4/PKG-INFO` & `ecape-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: metpy==1.5.0
+Requires-Python: >=3.8
+Requires-Dist: metpy>=1.2.0
 Requires-Dist: numpy>=1.18.0
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # ecape
 
 ecape is a simple module that contains an entraining CAPE, or ECAPE, calculation described by Peters et. al. 2023.
-Additionally, Peters et. al. 2023 -provided MatLab scripts serve as a reference and test verification data.
-The module leans heavily on Metpy for meteorological calculations.
+Additionally, Peters-provided MatLab scripts serve as a reference and test verification data.
+The module leans heavily on MetPy for meteorological calculations.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ecape.svg)](https://pypi.org/project/ecape)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ecape.svg)](https://pypi.org/project/ecape)
 
 ## Installation & Use
 
+In console:
 
 ```console
 pip install ecape
 ```
 
-See the example in linked documentation:
+See the example in linked documentation.
 
 ```python
    from ecape.calc import calc_ecape
    ...
    ecape = calc_ecape(height, pressure, temperature, specific_humidity, u_wind, v_wind, cape_type)
 ```
 
@@ -65,15 +63,15 @@
 
 ### Future Work
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
 ### Disclaimer
 There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
-This is primarily due to a difference in calculated CAPE. The tests describe other sources of error.
+This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
 
 Since:
  - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
  - Peters et. al. specifically mention MetPy for determining CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
 MetPy's CAPE calculations were chosen for ease of readability and implementation.
```

