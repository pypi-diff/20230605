# Comparing `tmp/ecape-0.0.3.tar.gz` & `tmp/ecape-0.0.4.tar.gz`

## Comparing `ecape-0.0.3.tar` & `ecape-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.3/src/ecape_py/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.3/src/ecape_py/__init__.py
--rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 ecape-0.0.3/src/ecape_py/ecape.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.3/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 ecape-0.0.3/README.md
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 ecape-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 ecape-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.4/.ruff_cache/content/a29a86d92757c5f3
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.4/src/ecape/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.4/src/ecape/__init__.py
+-rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 ecape-0.0.4/src/ecape/calc.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 ecape-0.0.4/README.md
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 ecape-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 ecape-0.0.4/PKG-INFO
```

### Comparing `ecape-0.0.3/src/ecape_py/ecape.py` & `ecape-0.0.4/src/ecape/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 
 
 @check_units("[pressure]", "[length]", "[temperature]", "[mass]/[mass]")
 def calc_mse(
     pressure: PintList, height: PintList, temperature: PintList, specific_humidity: PintList
 ) -> Tuple[PintList, PintList]:
     """
+    Calculate the moist static energy terms of interest.
 
     Args:
         pressure:
             Total atmospheric pressure
         height:
             Atmospheric heights at the levels given by 'pressure'.
         temperature:
@@ -316,28 +317,28 @@
     v_wind: PintList,
     cape_type: str = "most_unstable",
 ) -> pint.Quantity:
     """
     Calculate the entraining CAPE (ECAPE) of a parcel
 
     Parameters:
-    ----------
-        height:
+    ------------
+        height: np.ndarray[pint.Quantity]
             Atmospheric heights at the levels given by 'pressure'.
-        pressure:
+        pressure: np.ndarray[pint.Quantity]
             Total atmospheric pressure
-        temperature:
+        temperature: np.ndarray[pint.Quantity]
             Air temperature
-        specific humidity:
+        specific humidity: np.ndarray[pint.Quantity]
             Specific humidity
-        u_wind:
+        u_wind: np.ndarray[pint.Quantity]
             X component of the wind
-        v_wind
+        v_wind np.ndarray[pint.Quantity]
             Y component of the wind
-        cape_type:
+        cape_type: np.ndarray[pint.Quantity]
             Variation of CAPE desired. 'most_unstable' (default), 'surface_based', or 'mixed_layer'
 
     Returns:
     ----------
         ecape : 'pint.Quantity'
             Entraining CAPE
     """
```

### Comparing `ecape-0.0.3/LICENSE.txt` & `ecape-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.3/pyproject.toml` & `ecape-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/docs", "/tests"]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/ecape_py"]
+packages = ["src/ecape", "docs", "tests"]
 
 [project]
 name = "ecape"
 dynamic = ["version"]
 description = 'Calculate the entraining CAPE (ECAPE) of a parcel.'
 readme = "README.md"
 requires-python = ">=3.7"
@@ -38,15 +38,15 @@
 
 [project.urls]
 Documentation = "https://citylikeamradio.github.io/ecape"
 Issues = "https://github.com/citylikeamradio/ecape/issues"
 Source = "https://github.com/citylikeamradio/ecape"
 
 [tool.hatch.version]
-path = "src/ecape_py/__about__.py"
+path = "src/ecape/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
@@ -68,15 +68,15 @@
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
 ]
 [tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/ecape_py tests}"
+typing = "mypy --install-types --non-interactive {args:src/ecape tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
   "black {args:.}",
   "ruff --fix {args:.}",
@@ -134,33 +134,33 @@
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["ecape_py"]
+known-first-party = ["ecape"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
-source_pkgs = ["ecape_py", "tests"]
+source_pkgs = ["ecape", "tests"]
 branch = true
 parallel = true
 omit = [
-  "src/ecape_py/__about__.py",
+  "src/ecape/__about__.py",
 ]
 
 [tool.coverage.paths]
-ecape_py = ["src/ecape_py", "*/ecape/src/ecape_py"]
+ecape = ["src/ecape", "*/ecape/src/ecape"]
 tests = ["tests", "*/ecape/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
```

### Comparing `ecape-0.0.3/PKG-INFO` & `ecape-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.3
+Version: 0.0.4
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -28,44 +28,63 @@
 ecape is a simple module that contains an entraining CAPE, or ECAPE, calculation described by Peters et. al. 2023.
 Additionally, Peters et. al. 2023 -provided MatLab scripts serve as a reference and test verification data.
 The module leans heavily on Metpy for meteorological calculations.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ecape.svg)](https://pypi.org/project/ecape)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ecape.svg)](https://pypi.org/project/ecape)
 
-Installation
-------------
+## Installation & Use
+
 
 ```console
 pip install ecape
 ```
 
-Documentation, Source
--------------
+See the example in linked documentation:
+
+```python
+   from ecape.calc import calc_ecape
+   ...
+   ecape = calc_ecape(height, pressure, temperature, specific_humidity, u_wind, v_wind, cape_type)
+```
+
+### Documentation & Source
+
 https://github.com/citylikeamradio/ecape
 
-https://citylikeamradio.github.io/ecape/html/index.html
+https://citylikeamradio.github.io/ecape
+
+### Contact
 
-Contact
--------------
  - Robert Capella
  - bob.capella@gmail.com
  - https://twitter.com/minusthebob
 
-Future Work
--------------
+Questions, comments, and feedback are certainly welcome. This project is a personal exercise
+in learning how to publish packages to Github & PyPI, so excuse the excessive documentation for
+one function.
+
+### Future Work
  - if useful, incorporate into MetPy
- - provide .nc, .csv, & aws support
- - provide just-in-time compiling support for faster 2D work
+ - provide cli .nc, .csv, & aws support
+
+### Disclaimer
+There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
+This is primarily due to a difference in calculated CAPE. The tests describe other sources of error.
+
+Since:
+ - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
+ - Peters et. al. specifically mention MetPy for determining CAPE
+ - MetPy is a reliable, open-source, and frequently used meteorological calculation package
+
+MetPy's CAPE calculations were chosen for ease of readability and implementation.
 
-References
-------------
+### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
 John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
 
-Licence
-------------
+### Licence
 
 `ecape` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

