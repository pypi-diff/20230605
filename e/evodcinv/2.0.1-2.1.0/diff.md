# Comparing `tmp/evodcinv-2.0.1.tar.gz` & `tmp/evodcinv-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodcinv-2.0.1.tar", last modified: Thu Dec 16 09:13:10 2021, max compression
+gzip compressed data, was "evodcinv-2.1.0.tar", last modified: Mon Jun  5 20:03:30 2023, max compression
```

## Comparing `evodcinv-2.0.1.tar` & `evodcinv-2.1.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-12-16 09:13:10.743716 evodcinv-2.0.1/
--rw-rw-rw-   0        0        0     1546 2021-12-13 00:06:49.000000 evodcinv-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     6949 2021-12-16 09:13:10.743716 evodcinv-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5974 2021-12-13 00:07:23.000000 evodcinv-2.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2021-12-16 09:13:10.646268 evodcinv-2.0.1/evodcinv/
--rw-rw-rw-   0        0        0      210 2021-12-13 00:02:37.000000 evodcinv-2.0.1/evodcinv/__about__.py
--rw-rw-rw-   0        0        0      305 2021-12-13 00:07:29.000000 evodcinv-2.0.1/evodcinv/__init__.py
--rw-rw-rw-   0        0        0      110 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_common.py
--rw-rw-rw-   0        0        0     4332 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_curve.py
--rw-rw-rw-   0        0        0      224 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_helpers.py
-drwxrwxrwx   0        0        0        0 2021-12-16 09:13:10.694824 evodcinv-2.0.1/evodcinv/_io/
--rw-rw-rw-   0        0        0      104 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_io/__init__.py
--rw-rw-rw-   0        0        0     2672 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_io/_helpers.py
-drwxrwxrwx   0        0        0        0 2021-12-16 09:13:10.717058 evodcinv-2.0.1/evodcinv/_io/h5/
--rw-rw-rw-   0        0        0      150 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_io/h5/__init__.py
--rw-rw-rw-   0        0        0     1248 2021-12-16 08:30:00.000000 evodcinv-2.0.1/evodcinv/_io/h5/_h5.py
-drwxrwxrwx   0        0        0        0 2021-12-16 09:13:10.734705 evodcinv-2.0.1/evodcinv/_io/json/
--rw-rw-rw-   0        0        0      156 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_io/json/__init__.py
--rw-rw-rw-   0        0        0     1497 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_io/json/_json.py
--rw-rw-rw-   0        0        0     2009 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_layer.py
--rw-rw-rw-   0        0        0    13211 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_model.py
--rw-rw-rw-   0        0        0      641 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_progress.py
--rw-rw-rw-   0        0        0    17308 2021-12-13 00:06:49.000000 evodcinv-2.0.1/evodcinv/_result.py
-drwxrwxrwx   0        0        0        0 2021-12-16 09:13:10.682437 evodcinv-2.0.1/evodcinv.egg-info/
--rw-rw-rw-   0        0        0     6949 2021-12-16 09:13:10.000000 evodcinv-2.0.1/evodcinv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2021-12-16 09:13:10.000000 evodcinv-2.0.1/evodcinv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-16 09:13:10.000000 evodcinv-2.0.1/evodcinv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2021-12-16 09:13:10.000000 evodcinv-2.0.1/evodcinv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-12-16 09:13:10.000000 evodcinv-2.0.1/evodcinv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2021-12-13 00:06:49.000000 evodcinv-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1163 2021-12-16 09:13:10.752163 evodcinv-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-12-16 09:13:10.742708 evodcinv-2.0.1/test/
--rw-rw-rw-   0        0        0      166 2021-12-13 00:06:49.000000 evodcinv-2.0.1/test/test_model.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.826051 evodcinv-2.1.0/
+-rw-rw-rw-   0        0        0     1546 2023-05-28 06:48:01.000000 evodcinv-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7013 2023-06-05 20:03:30.826051 evodcinv-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5989 2023-06-05 19:59:55.000000 evodcinv-2.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.797313 evodcinv-2.1.0/evodcinv/
+-rw-rw-rw-   0        0        0        5 2023-06-05 18:07:27.000000 evodcinv-2.1.0/evodcinv/VERSION
+-rw-rw-rw-   0        0        0      159 2023-06-05 18:08:41.000000 evodcinv-2.1.0/evodcinv/__about__.py
+-rw-rw-rw-   0        0        0      305 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/__init__.py
+-rw-rw-rw-   0        0        0      110 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_common.py
+-rw-rw-rw-   0        0        0     4332 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_curve.py
+-rw-rw-rw-   0        0        0      224 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.819531 evodcinv-2.1.0/evodcinv/_io/
+-rw-rw-rw-   0        0        0      104 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/__init__.py
+-rw-rw-rw-   0        0        0     2672 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.821536 evodcinv-2.1.0/evodcinv/_io/h5/
+-rw-rw-rw-   0        0        0      150 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/h5/__init__.py
+-rw-rw-rw-   0        0        0     1328 2023-06-05 18:11:52.000000 evodcinv-2.1.0/evodcinv/_io/h5/_h5.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.823536 evodcinv-2.1.0/evodcinv/_io/json/
+-rw-rw-rw-   0        0        0      156 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/json/__init__.py
+-rw-rw-rw-   0        0        0     1497 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/json/_json.py
+-rw-rw-rw-   0        0        0     2009 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_layer.py
+-rw-rw-rw-   0        0        0    13304 2023-06-05 18:11:52.000000 evodcinv-2.1.0/evodcinv/_model.py
+-rw-rw-rw-   0        0        0      641 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_progress.py
+-rw-rw-rw-   0        0        0    17413 2023-06-05 18:11:52.000000 evodcinv-2.1.0/evodcinv/_result.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.817371 evodcinv-2.1.0/evodcinv.egg-info/
+-rw-rw-rw-   0        0        0     7013 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-05-28 06:48:01.000000 evodcinv-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1271 2023-06-05 20:03:30.838564 evodcinv-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.825043 evodcinv-2.1.0/tests/
+-rw-rw-rw-   0        0        0      166 2023-05-28 06:48:01.000000 evodcinv-2.1.0/tests/test_model.py
```

### Comparing `evodcinv-2.0.1/LICENSE` & `evodcinv-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evodcinv-2.0.1/PKG-INFO` & `evodcinv-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: evodcinv
-Version: 2.0.1
+Version: 2.1.0
 Summary: Inversion of dispersion curves using Evolutionary Algorithms
 Home-page: https://github.com/keurfonluu/evodcinv
 Author: Keurfon Luu
 License: BSD 3-Clause License
 Project-URL: Code, https://github.com/keurfonluu/evodcinv
 Project-URL: Issues, https://github.com/keurfonluu/evodcinv/issues
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 evodcinv
 ========
 
-|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Travis| |DOI|
+|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Docs| |DOI|
 
 **evodcinv** is a Python library to invert surface wave dispersion data (e.g., phase velocity dispersion curves) for an isotropic layered velocity model using Evolutionary Algorithms. It relies on `stochopy <https://github.com/keurfonluu/stochopy>`__ for the evolutionary optimizers while forward modeling is heavy-lifted by `disba <https://github.com/keurfonluu/disba>`__.
 
 .. figure:: https://raw.githubusercontent.com/keurfonluu/evodcinv/master/.github/sample.png
    :alt: sample
    :width: 100%
    :align: center
@@ -166,14 +167,12 @@
 
 .. |Codecov| image:: https://img.shields.io/codecov/c/github/keurfonluu/evodcinv.svg?style=flat
    :target: https://codecov.io/gh/keurfonluu/evodcinv
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5775193.svg?style=flat
    :target: https://doi.org/10.5281/zenodo.5775193
 
-.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/evodcinv/Python%20package
+.. |Build| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/evodcinv/ci.yml
    :target: https://github.com/keurfonluu/evodcinv
 
-.. |Travis| image:: https://img.shields.io/travis/com/keurfonluu/evodcinv/master?label=docs
+.. |Docs| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/evodcinv/doc.yml?label=docs
    :target: https://keurfonluu.github.io/evodcinv/
-
-
```

### Comparing `evodcinv-2.0.1/README.rst` & `evodcinv-2.1.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 evodcinv
 ========
 
-|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Travis| |DOI|
+|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Docs| |DOI|
 
 **evodcinv** is a Python library to invert surface wave dispersion data (e.g., phase velocity dispersion curves) for an isotropic layered velocity model using Evolutionary Algorithms. It relies on `stochopy <https://github.com/keurfonluu/stochopy>`__ for the evolutionary optimizers while forward modeling is heavy-lifted by `disba <https://github.com/keurfonluu/disba>`__.
 
 .. figure:: https://raw.githubusercontent.com/keurfonluu/evodcinv/master/.github/sample.png
    :alt: sample
    :width: 100%
    :align: center
@@ -142,12 +142,12 @@
 
 .. |Codecov| image:: https://img.shields.io/codecov/c/github/keurfonluu/evodcinv.svg?style=flat
    :target: https://codecov.io/gh/keurfonluu/evodcinv
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5775193.svg?style=flat
    :target: https://doi.org/10.5281/zenodo.5775193
 
-.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/evodcinv/Python%20package
+.. |Build| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/evodcinv/ci.yml
    :target: https://github.com/keurfonluu/evodcinv
 
-.. |Travis| image:: https://img.shields.io/travis/com/keurfonluu/evodcinv/master?label=docs
+.. |Docs| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/evodcinv/doc.yml?label=docs
    :target: https://keurfonluu.github.io/evodcinv/
```

### Comparing `evodcinv-2.0.1/evodcinv/_curve.py` & `evodcinv-2.1.0/evodcinv/_curve.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.0.1/evodcinv/_io/_helpers.py` & `evodcinv-2.1.0/evodcinv/_io/_helpers.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.0.1/evodcinv/_io/h5/_h5.py` & `evodcinv-2.1.0/evodcinv/_io/h5/_h5.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,11 +38,15 @@
     compression_opts : int, optional, default 4
         Compression level for gzip compression. May be an integer from 0 to 9.
 
     """
     with h5py.File(filename, "w") as f:
         for k, v in result.items():
             if np.ndim(v) == 0:
-                f.create_dataset(k, data=(v,), compression="gzip", compression_opts=compression_opts)
+                f.create_dataset(
+                    k, data=(v,), compression="gzip", compression_opts=compression_opts
+                )
 
             else:
-                f.create_dataset(k, data=v, compression="gzip", compression_opts=compression_opts)
+                f.create_dataset(
+                    k, data=v, compression="gzip", compression_opts=compression_opts
+                )
```

### Comparing `evodcinv-2.0.1/evodcinv/_io/json/_json.py` & `evodcinv-2.1.0/evodcinv/_io/json/_json.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.0.1/evodcinv/_layer.py` & `evodcinv-2.1.0/evodcinv/_layer.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.0.1/evodcinv/_model.py` & `evodcinv-2.1.0/evodcinv/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,14 @@
             "maxiter": 100,
             "popsize": 10,
             "seed": None,
         }
         _optimizer_args.update(optimizer_args)
 
         maxiter = _optimizer_args["maxiter"]
-        popsize = _optimizer_args["popsize"]
 
         # Overwrite options
         constraints = {
             "cmaes": "Penalize",
             "cpso": "Shrink",
             "de": "Random",
             "pso": "Shrink",
@@ -276,14 +275,15 @@
                     bounds,
                     method=method,
                     options=_optimizer_args,
                     callback=callback,
                 )
 
             # Parse output
+            popsize = x.xall.shape[1]
             velocity_models = np.empty((maxiter, popsize, self.n_layers, 4))
             for i in range(x.nit):
                 for j in range(popsize):
                     velocity_models[i, j] = self.transform(x.xall[i, j])
 
             result = InversionResult(
                 xs=np.concatenate(x.xall),
@@ -365,15 +365,19 @@
                         dt,
                     )
                     idx = c > 0.0
                     dcalc = c[idx]
 
                 else:
                     ell = Ellipticity(
-                        thickness, velocity_p, velocity_s, density, dc=dc,
+                        thickness,
+                        velocity_p,
+                        velocity_s,
+                        density,
+                        dc=dc,
                     )
                     rel = ell(curve.period, mode=curve.mode)
                     dcalc = np.abs(rel.ellipticity)
 
                 n = len(dcalc)
                 if n > 0:
                     sigma = (
```

### Comparing `evodcinv-2.0.1/evodcinv/_progress.py` & `evodcinv-2.1.0/evodcinv/_progress.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.0.1/evodcinv/_result.py` & `evodcinv-2.1.0/evodcinv/_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,20 @@
 
                 return c[idx]
 
         else:
 
             def get_y(thickness, velocity_p, velocity_s, density):
                 ell = Ellipticity(
-                    thickness, velocity_p, velocity_s, density, "dunkin", dc,
+                    thickness,
+                    velocity_p,
+                    velocity_s,
+                    density,
+                    "dunkin",
+                    dc,
                 )
                 rel = ell(period, mode)
 
                 return np.abs(rel.ellipticity)
 
         # Plot arguments
         plot_args = plot_args if plot_args is not None else {}
```

### Comparing `evodcinv-2.0.1/evodcinv.egg-info/PKG-INFO` & `evodcinv-2.1.0/evodcinv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: evodcinv
-Version: 2.0.1
+Version: 2.1.0
 Summary: Inversion of dispersion curves using Evolutionary Algorithms
 Home-page: https://github.com/keurfonluu/evodcinv
 Author: Keurfon Luu
 License: BSD 3-Clause License
 Project-URL: Code, https://github.com/keurfonluu/evodcinv
 Project-URL: Issues, https://github.com/keurfonluu/evodcinv/issues
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 evodcinv
 ========
 
-|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Travis| |DOI|
+|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Docs| |DOI|
 
 **evodcinv** is a Python library to invert surface wave dispersion data (e.g., phase velocity dispersion curves) for an isotropic layered velocity model using Evolutionary Algorithms. It relies on `stochopy <https://github.com/keurfonluu/stochopy>`__ for the evolutionary optimizers while forward modeling is heavy-lifted by `disba <https://github.com/keurfonluu/disba>`__.
 
 .. figure:: https://raw.githubusercontent.com/keurfonluu/evodcinv/master/.github/sample.png
    :alt: sample
    :width: 100%
    :align: center
@@ -166,14 +167,12 @@
 
 .. |Codecov| image:: https://img.shields.io/codecov/c/github/keurfonluu/evodcinv.svg?style=flat
    :target: https://codecov.io/gh/keurfonluu/evodcinv
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5775193.svg?style=flat
    :target: https://doi.org/10.5281/zenodo.5775193
 
-.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/evodcinv/Python%20package
+.. |Build| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/evodcinv/ci.yml
    :target: https://github.com/keurfonluu/evodcinv
 
-.. |Travis| image:: https://img.shields.io/travis/com/keurfonluu/evodcinv/master?label=docs
+.. |Docs| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/evodcinv/doc.yml?label=docs
    :target: https://keurfonluu.github.io/evodcinv/
-
-
```

### Comparing `evodcinv-2.0.1/evodcinv.egg-info/SOURCES.txt` & `evodcinv-2.1.0/evodcinv.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
+evodcinv/VERSION
 evodcinv/__about__.py
 evodcinv/__init__.py
 evodcinv/_common.py
 evodcinv/_curve.py
 evodcinv/_helpers.py
 evodcinv/_layer.py
 evodcinv/_model.py
@@ -18,8 +19,8 @@
 evodcinv.egg-info/top_level.txt
 evodcinv/_io/__init__.py
 evodcinv/_io/_helpers.py
 evodcinv/_io/h5/__init__.py
 evodcinv/_io/h5/_h5.py
 evodcinv/_io/json/__init__.py
 evodcinv/_io/json/_json.py
-test/test_model.py
+tests/test_model.py
```

### Comparing `evodcinv-2.0.1/setup.cfg` & `evodcinv-2.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 766f 6463 696e 760d 0a76 6572   = evodcinv..ver
-00000020: 7369 6f6e 203d 2032 2e30 2e31 0d0a 6175  sion = 2.0.1..au
-00000030: 7468 6f72 203d 204b 6575 7266 6f6e 204c  thor = Keurfon L
-00000040: 7575 0d0a 656d 6169 6c20 3d20 6b65 7572  uu..email = keur
-00000050: 666f 6e6c 7575 406f 7574 6c6f 6f6b 2e63  fonluu@outlook.c
-00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
-00000070: 3d20 496e 7665 7273 696f 6e20 6f66 2064  = Inversion of d
-00000080: 6973 7065 7273 696f 6e20 6375 7276 6573  ispersion curves
-00000090: 2075 7369 6e67 2045 766f 6c75 7469 6f6e   using Evolution
-000000a0: 6172 7920 416c 676f 7269 7468 6d73 0d0a  ary Algorithms..
-000000b0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-000000c0: 7468 7562 2e63 6f6d 2f6b 6575 7266 6f6e  thub.com/keurfon
-000000d0: 6c75 752f 6576 6f64 6369 6e76 0d0a 7072  luu/evodcinv..pr
-000000e0: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-000000f0: 436f 6465 3d68 7474 7073 3a2f 2f67 6974  Code=https://git
-00000100: 6875 622e 636f 6d2f 6b65 7572 666f 6e6c  hub.com/keurfonl
-00000110: 7575 2f65 766f 6463 696e 760d 0a09 4973  uu/evodcinv...Is
-00000120: 7375 6573 3d68 7474 7073 3a2f 2f67 6974  sues=https://git
-00000130: 6875 622e 636f 6d2f 6b65 7572 666f 6e6c  hub.com/keurfonl
-00000140: 7575 2f65 766f 6463 696e 762f 6973 7375  uu/evodcinv/issu
-00000150: 6573 0d0a 6c6f 6e67 5f64 6573 6372 6970  es..long_descrip
-00000160: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-00000170: 444d 452e 7273 740d 0a6c 6f6e 675f 6465  DME.rst..long_de
-00000180: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000190: 745f 7479 7065 203d 2074 6578 742f 782d  t_type = text/x-
-000001a0: 7273 740d 0a6c 6963 656e 7365 203d 2042  rst..license = B
-000001b0: 5344 2033 2d43 6c61 7573 6520 4c69 6365  SD 3-Clause Lice
-000001c0: 6e73 650d 0a70 6c61 7466 6f72 6d73 203d  nse..platforms =
-000001d0: 2061 6e79 0d0a 636c 6173 7369 6669 6572   any..classifier
-000001e0: 7320 3d20 0d0a 094c 6963 656e 7365 203a  s = ...License :
-000001f0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000200: 3a20 4253 4420 4c69 6365 6e73 650d 0a09  : BSD License...
-00000210: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000220: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000230: 6e74 0d0a 0944 6576 656c 6f70 6d65 6e74  nt...Development
-00000240: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
-00000250: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
-00000260: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
-00000270: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
-00000280: 5265 7365 6172 6368 0d0a 0954 6f70 6963  Research...Topic
-00000290: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-000002a0: 6e67 696e 6565 7269 6e67 0d0a 0954 6f70  ngineering...Top
-000002b0: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
-000002c0: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
-000002d0: 5068 7973 6963 730d 0a09 5072 6f67 7261  Physics...Progra
-000002e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002f0: 3a20 5079 7468 6f6e 203a 3a20 332e 360d  : Python :: 3.6.
-00000300: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000310: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000320: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
-00000330: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000340: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-00000350: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000360: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000370: 203a 3a20 332e 390d 0a0d 0a5b 6f70 7469   :: 3.9....[opti
-00000380: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
-00000390: 2066 696e 643a 0d0a 696e 7374 616c 6c5f   find:..install_
-000003a0: 7265 7175 6972 6573 203d 200d 0a09 696d  requires = ...im
-000003b0: 706f 7274 6c69 625f 6d65 7461 6461 7461  portlib_metadata
-000003c0: 0d0a 096e 756d 7079 0d0a 096d 6174 706c  ...numpy...matpl
-000003d0: 6f74 6c69 620d 0a09 6a6f 626c 6962 0d0a  otlib...joblib..
-000003e0: 0968 3570 790d 0a09 7072 6f67 7265 7373  .h5py...progress
-000003f0: 0d0a 0964 6973 6261 203e 3d20 302e 362e  ...disba >= 0.6.
-00000400: 310d 0a09 7374 6f63 686f 7079 203e 3d20  1...stochopy >= 
-00000410: 322e 322e 300d 0a70 7974 686f 6e5f 7265  2.2.0..python_re
-00000420: 7175 6972 6573 203d 203e 3d20 332e 360d  quires = >= 3.6.
-00000430: 0a73 6574 7570 5f72 6571 7569 7265 7320  .setup_requires 
-00000440: 3d20 0d0a 0973 6574 7570 746f 6f6c 7320  = ...setuptools 
-00000450: 3e3d 2034 320d 0a09 7768 6565 6c0d 0a0d  >= 42...wheel...
-00000460: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000470: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000480: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000020: 7369 6f6e 203d 2066 696c 653a 2065 766f  sion = file: evo
+00000030: 6463 696e 762f 5645 5253 494f 4e0d 0a61  dcinv/VERSION..a
+00000040: 7574 686f 7220 3d20 4b65 7572 666f 6e20  uthor = Keurfon 
+00000050: 4c75 750d 0a65 6d61 696c 203d 206b 6575  Luu..email = keu
+00000060: 7266 6f6e 6c75 7540 6f75 746c 6f6f 6b2e  rfonluu@outlook.
+00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
+00000080: 203d 2049 6e76 6572 7369 6f6e 206f 6620   = Inversion of 
+00000090: 6469 7370 6572 7369 6f6e 2063 7572 7665  dispersion curve
+000000a0: 7320 7573 696e 6720 4576 6f6c 7574 696f  s using Evolutio
+000000b0: 6e61 7279 2041 6c67 6f72 6974 686d 730d  nary Algorithms.
+000000c0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+000000d0: 6974 6875 622e 636f 6d2f 6b65 7572 666f  ithub.com/keurfo
+000000e0: 6e6c 7575 2f65 766f 6463 696e 760d 0a70  nluu/evodcinv..p
+000000f0: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000100: 0943 6f64 653d 6874 7470 733a 2f2f 6769  .Code=https://gi
+00000110: 7468 7562 2e63 6f6d 2f6b 6575 7266 6f6e  thub.com/keurfon
+00000120: 6c75 752f 6576 6f64 6369 6e76 0d0a 0949  luu/evodcinv...I
+00000130: 7373 7565 733d 6874 7470 733a 2f2f 6769  ssues=https://gi
+00000140: 7468 7562 2e63 6f6d 2f6b 6575 7266 6f6e  thub.com/keurfon
+00000150: 6c75 752f 6576 6f64 6369 6e76 2f69 7373  luu/evodcinv/iss
+00000160: 7565 730d 0a6c 6f6e 675f 6465 7363 7269  ues..long_descri
+00000170: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
+00000180: 4144 4d45 2e72 7374 0d0a 6c6f 6e67 5f64  ADME.rst..long_d
+00000190: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+000001a0: 6e74 5f74 7970 6520 3d20 7465 7874 2f78  nt_type = text/x
+000001b0: 2d72 7374 0d0a 6c69 6365 6e73 6520 3d20  -rst..license = 
+000001c0: 4253 4420 332d 436c 6175 7365 204c 6963  BSD 3-Clause Lic
+000001d0: 656e 7365 0d0a 706c 6174 666f 726d 7320  ense..platforms 
+000001e0: 3d20 616e 790d 0a63 6c61 7373 6966 6965  = any..classifie
+000001f0: 7273 203d 200d 0a09 4c69 6365 6e73 6520  rs = ...License 
+00000200: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000210: 3a3a 2042 5344 204c 6963 656e 7365 0d0a  :: BSD License..
+00000220: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000230: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000240: 656e 740d 0a09 4465 7665 6c6f 706d 656e  ent...Developmen
+00000250: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
+00000260: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
+00000270: 650d 0a09 496e 7465 6e64 6564 2041 7564  e...Intended Aud
+00000280: 6965 6e63 6520 3a3a 2053 6369 656e 6365  ience :: Science
+00000290: 2f52 6573 6561 7263 680d 0a09 546f 7069  /Research...Topi
+000002a0: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+000002b0: 456e 6769 6e65 6572 696e 670d 0a09 546f  Engineering...To
+000002c0: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
+000002d0: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
+000002e0: 2050 6879 7369 6373 0d0a 0950 726f 6772   Physics...Progr
+000002f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000300: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+00000310: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000320: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000330: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
+00000340: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000350: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+00000360: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000370: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000380: 6e20 3a3a 2033 2e31 300d 0a09 5072 6f67  n :: 3.10...Prog
+00000390: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000003a0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000003b0: 3131 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  11....[options].
+000003c0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000003d0: 3a0d 0a69 6e73 7461 6c6c 5f72 6571 7569  :..install_requi
+000003e0: 7265 7320 3d20 0d0a 0969 6d70 6f72 746c  res = ...importl
+000003f0: 6962 5f6d 6574 6164 6174 610d 0a09 6e75  ib_metadata...nu
+00000400: 6d70 790d 0a09 6d61 7470 6c6f 746c 6962  mpy...matplotlib
+00000410: 0d0a 096a 6f62 6c69 620d 0a09 6835 7079  ...joblib...h5py
+00000420: 0d0a 0970 726f 6772 6573 730d 0a09 6469  ...progress...di
+00000430: 7362 6120 3e3d 2030 2e36 2e31 0d0a 0973  sba >= 0.6.1...s
+00000440: 746f 6368 6f70 7920 3e3d 2032 2e33 2e30  tochopy >= 2.3.0
+00000450: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000460: 7320 3d20 3e3d 2033 2e37 0d0a 7365 7475  s = >= 3.7..setu
+00000470: 705f 7265 7175 6972 6573 203d 200d 0a09  p_requires = ...
+00000480: 7365 7475 7074 6f6f 6c73 203e 3d20 3432  setuptools >= 42
+00000490: 0d0a 0977 6865 656c 0d0a 0d0a 5b6f 7074  ...wheel....[opt
+000004a0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
+000004b0: 615d 0d0a 6576 6f64 6369 6e76 203d 200d  a]..evodcinv = .
+000004c0: 0a09 5645 5253 494f 4e0d 0a0d 0a5b 6567  ..VERSION....[eg
+000004d0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000004e0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000004f0: 3d20 300d 0a0d 0a                        = 0....
```

