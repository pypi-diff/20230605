# Comparing `tmp/roughsets-base-1.0.1.1.tar.gz` & `tmp/roughsets-base-1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roughsets-base-1.0.1.1.tar", last modified: Sat Feb  5 19:12:46 2022, max compression
+gzip compressed data, was "roughsets-base-1.0.1.2.tar", last modified: Sun Jun  4 21:55:10 2023, max compression
```

## Comparing `roughsets-base-1.0.1.1.tar` & `roughsets-base-1.0.1.2.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxrwx   0 darek     (1000) darek     (1000)        0 2022-02-05 19:12:46.774525 roughsets-base-1.0.1.1/
--rwxrwxrwx   0 darek     (1000) darek     (1000)     1552 2021-11-11 12:57:23.000000 roughsets-base-1.0.1.1/LICENSE
--rwxrwxrwx   0 darek     (1000) darek     (1000)     1552 2021-11-11 12:57:23.000000 roughsets-base-1.0.1.1/LICENSE.txt
--rwxrwxrwx   0 darek     (1000) darek     (1000)        0 2021-06-10 22:14:45.000000 roughsets-base-1.0.1.1/MANIFEST.in
--rwxrwxrwx   0 darek     (1000) darek     (1000)     4061 2022-02-05 19:12:46.776531 roughsets-base-1.0.1.1/PKG-INFO
--rwxrwxrwx   0 darek     (1000) darek     (1000)     3010 2022-02-03 10:26:36.000000 roughsets-base-1.0.1.1/README.md
--rwxrwxrwx   0 darek     (1000) darek     (1000)      108 2021-06-10 21:39:32.000000 roughsets-base-1.0.1.1/pyproject.toml
--rwxrwxrwx   0 darek     (1000) darek     (1000)     1144 2022-02-05 19:12:46.789526 roughsets-base-1.0.1.1/setup.cfg
-drwxrwxrwx   0 darek     (1000) darek     (1000)        0 2022-02-05 19:12:46.160587 roughsets-base-1.0.1.1/src/
-drwxrwxrwx   0 darek     (1000) darek     (1000)        0 2022-02-05 19:12:46.594528 roughsets-base-1.0.1.1/src/roughsets_base/
--rwxrwxrwx   0 darek     (1000) darek     (1000)       93 2022-02-03 08:11:45.000000 roughsets-base-1.0.1.1/src/roughsets_base/__init__.py
--rwxrwxrwx   0 darek     (1000) darek     (1000)     7685 2021-11-30 23:32:46.000000 roughsets-base-1.0.1.1/src/roughsets_base/roughset_dt.py
--rwxrwxrwx   0 darek     (1000) darek     (1000)     5163 2021-11-28 23:58:24.000000 roughsets-base-1.0.1.1/src/roughsets_base/roughset_si.py
-drwxrwxrwx   0 darek     (1000) darek     (1000)        0 2022-02-05 19:12:46.748526 roughsets-base-1.0.1.1/src/roughsets_base.egg-info/
--rwxrwxrwx   0 darek     (1000) darek     (1000)     4061 2022-02-05 19:12:45.000000 roughsets-base-1.0.1.1/src/roughsets_base.egg-info/PKG-INFO
--rwxrwxrwx   0 darek     (1000) darek     (1000)      374 2022-02-05 19:12:46.000000 roughsets-base-1.0.1.1/src/roughsets_base.egg-info/SOURCES.txt
--rwxrwxrwx   0 darek     (1000) darek     (1000)        1 2022-02-05 19:12:46.000000 roughsets-base-1.0.1.1/src/roughsets_base.egg-info/dependency_links.txt
--rwxrwxrwx   0 darek     (1000) darek     (1000)       12 2022-02-05 19:12:46.000000 roughsets-base-1.0.1.1/src/roughsets_base.egg-info/requires.txt
--rwxrwxrwx   0 darek     (1000) darek     (1000)       15 2022-02-05 19:12:46.000000 roughsets-base-1.0.1.1/src/roughsets_base.egg-info/top_level.txt
+drwxr-xr-x   0 darek     (1000) darek     (1000)        0 2023-06-04 21:55:10.507942 roughsets-base-1.0.1.2/
+-rw-r--r--   0 darek     (1000) darek     (1000)     1552 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/LICENSE
+-rw-r--r--   0 darek     (1000) darek     (1000)     1552 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/LICENSE.txt
+-rw-r--r--   0 darek     (1000) darek     (1000)        0 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/MANIFEST.in
+-rw-r--r--   0 darek     (1000) darek     (1000)     4277 2023-06-04 21:55:10.507942 roughsets-base-1.0.1.2/PKG-INFO
+-rw-r--r--   0 darek     (1000) darek     (1000)     3269 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/README.md
+-rw-r--r--   0 darek     (1000) darek     (1000)      108 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/pyproject.toml
+-rw-r--r--   0 darek     (1000) darek     (1000)     1144 2023-06-04 21:55:10.517938 roughsets-base-1.0.1.2/setup.cfg
+drwxr-xr-x   0 darek     (1000) darek     (1000)        0 2023-06-04 21:55:10.452452 roughsets-base-1.0.1.2/src/
+drwxr-xr-x   0 darek     (1000) darek     (1000)        0 2023-06-04 21:55:10.473715 roughsets-base-1.0.1.2/src/roughsets_base/
+-rw-r--r--   0 darek     (1000) darek     (1000)      144 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/src/roughsets_base/__init__.py
+-rw-r--r--   0 darek     (1000) darek     (1000)     7645 2023-06-04 21:28:40.000000 roughsets-base-1.0.1.2/src/roughsets_base/roughset_dt.py
+-rw-r--r--   0 darek     (1000) darek     (1000)     5151 2023-06-04 20:57:58.000000 roughsets-base-1.0.1.2/src/roughsets_base/roughset_si.py
+drwxr-xr-x   0 darek     (1000) darek     (1000)        0 2023-06-04 21:55:10.498027 roughsets-base-1.0.1.2/src/roughsets_base.egg-info/
+-rw-r--r--   0 darek     (1000) darek     (1000)     4277 2023-06-04 21:55:10.000000 roughsets-base-1.0.1.2/src/roughsets_base.egg-info/PKG-INFO
+-rw-r--r--   0 darek     (1000) darek     (1000)      504 2023-06-04 21:55:10.000000 roughsets-base-1.0.1.2/src/roughsets_base.egg-info/SOURCES.txt
+-rw-r--r--   0 darek     (1000) darek     (1000)        1 2023-06-04 21:55:10.000000 roughsets-base-1.0.1.2/src/roughsets_base.egg-info/dependency_links.txt
+-rw-r--r--   0 darek     (1000) darek     (1000)       12 2023-06-04 21:55:10.000000 roughsets-base-1.0.1.2/src/roughsets_base.egg-info/requires.txt
+-rw-r--r--   0 darek     (1000) darek     (1000)       15 2023-06-04 21:55:10.000000 roughsets-base-1.0.1.2/src/roughsets_base.egg-info/top_level.txt
+drwxr-xr-x   0 darek     (1000) darek     (1000)        0 2023-06-04 21:55:10.506939 roughsets-base-1.0.1.2/tests/
+-rw-r--r--   0 darek     (1000) darek     (1000)      318 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/tests/test_dataset_1.py
+-rw-r--r--   0 darek     (1000) darek     (1000)      459 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/tests/test_dataset_2.py
+-rw-r--r--   0 darek     (1000) darek     (1000)      304 2023-06-04 20:42:03.000000 roughsets-base-1.0.1.2/tests/test_dataset_3.py
+-rw-r--r--   0 darek     (1000) darek     (1000)     5458 2023-06-04 21:53:16.000000 roughsets-base-1.0.1.2/tests/test_dataset_KDD99.py
+-rw-r--r--   0 darek     (1000) darek     (1000)      893 2023-06-04 21:49:26.000000 roughsets-base-1.0.1.2/tests/test_t_abstract_base.py
```

### Comparing `roughsets-base-1.0.1.1/LICENSE` & `roughsets-base-1.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `roughsets-base-1.0.1.1/LICENSE.txt` & `roughsets-base-1.0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roughsets-base-1.0.1.1/PKG-INFO` & `roughsets-base-1.0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: roughsets-base
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: "The library contains base functions of the RoughSets Theory (introduced by Zdzisław Pawlak in 1982)."
 Home-page: https://github.com/darekjk/roughsets-base
 Author: Dariusz Jankowski
 Author-email: darekjki@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/darekjk/roughsets-base/issues
 Project-URL: Documentation, https://github.com/darekjk/roughsets-base/
 Project-URL: Source Code, https://github.com/darekjk/roughsets-base
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -94,21 +92,25 @@
 
 For checking of unit tests' results was used algorithms from well known reference library:  
 https://www.rdocumentation.org/packages/RoughSets/topics/RoughSets-package
 
 
 Re-Build sphinx documentation
 --------------------------
-pip install -r requirements.ci.txt  
+pip install -r requirements.dev.txt  
 sphinx-build -b html ./doc ./doc/_build/html  
 sphinx-build -b man ./doc ./doc/_build/man  
 
 
 Recommended packages
 --------------------
 
 sklearn-pandas https://github.com/scikit-learn-contrib/sklearn-pandas   
 pandas ecosystem: https://pandas.pydata.org/community/ecosystem.html  
 
 
+Citation
+--------
+  
+If You would like to use this library in Your research, please cite it.
 
-
+Jankowski, D. (2022). Roughsets-base: Python library for base Roughsets methods. (v1.0.1) [Computer software]. Zenodo. https://doi.org/10.5281/ZENODO.5957474
```

### Comparing `roughsets-base-1.0.1.1/README.md` & `roughsets-base-1.0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,19 +67,25 @@
 
 For checking of unit tests' results was used algorithms from well known reference library:  
 https://www.rdocumentation.org/packages/RoughSets/topics/RoughSets-package
 
 
 Re-Build sphinx documentation
 --------------------------
-pip install -r requirements.ci.txt  
+pip install -r requirements.dev.txt  
 sphinx-build -b html ./doc ./doc/_build/html  
 sphinx-build -b man ./doc ./doc/_build/man  
 
 
 Recommended packages
 --------------------
 
 sklearn-pandas https://github.com/scikit-learn-contrib/sklearn-pandas   
 pandas ecosystem: https://pandas.pydata.org/community/ecosystem.html  
 
 
+Citation
+--------
+  
+If You would like to use this library in Your research, please cite it.
+
+Jankowski, D. (2022). Roughsets-base: Python library for base Roughsets methods. (v1.0.1) [Computer software]. Zenodo. https://doi.org/10.5281/ZENODO.5957474
```

### Comparing `roughsets-base-1.0.1.1/setup.cfg` & `roughsets-base-1.0.1.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = roughsets-base
-version = 1.0.1.1
+version = 1.0.1.2
 author = Dariusz Jankowski
 author_email = darekjki@gmail.com
 description = "The library contains base functions of the RoughSets Theory (introduced by Zdzisław Pawlak in 1982)."
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darekjk/roughsets-base
 project_urls =
```

### Comparing `roughsets-base-1.0.1.1/src/roughsets_base/roughset_dt.py` & `roughsets-base-1.0.1.2/src/roughsets_base/roughset_dt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import logging
 
 import pandas as pd
-from pandas import DataFrame, Series, Int64Index
+from pandas import DataFrame, Series
 
 from roughsets_base.roughset_si import RoughSetSI
 
 
 class RoughSetDT(RoughSetSI):
     """Class RoughSet to model a decision table (DT).
 
@@ -158,43 +158,43 @@
         IND_OF_X_by_concept = IND_OF_X_EXT[IND_OF_X_EXT[self.ind_index_name].isin(IND_concept)]
 
         # Get a lower approximation (if only one concept) or sum of lower approximations (if more than one concept)
         # (DataFrame's indexes of dataset X)
         ind_index_of_lower_approximation: Series = IND_OF_X_by_concept[
             IND_OF_X_by_concept["y_class_count"] == 1
         ][self.ind_index_name]
-        lower_approximation_of_X: Int64Index = X_IND[
+        lower_approximation_of_X = X_IND[
             X_IND[self.ind_index_name].isin(ind_index_of_lower_approximation)
         ].index
 
         # Get a boundary region (DataFrame's indexes of dataset X)
         ind_index_of_boundary_region: Series = IND_OF_X_by_concept[
             IND_OF_X_by_concept["y_class_count"] > 1
         ][self.ind_index_name]
-        boundary_region_of_X: Int64Index = X_IND[
+        boundary_region_of_X = X_IND[
             X_IND[self.ind_index_name].isin(ind_index_of_boundary_region)
         ].index
 
         # Get a upper approximation (if only one concept) or sum of upper approximations (if more than one concept)
         # (DataFrame's indexes of dataset X)
-        upper_approximation_of_X: Int64Index = lower_approximation_of_X.append(boundary_region_of_X).sort_values()
+        upper_approximation_of_X = lower_approximation_of_X.append(boundary_region_of_X)
 
         # Get a negative region (DataFrame's indexes of dataset X)
-        negative_region_of_X = self.X.index.delete(upper_approximation_of_X).sort_values()
+        negative_region_of_X = self.X.index.difference(upper_approximation_of_X)
 
         # Get a negative region (DataFrame's indexes of dataset X) (method 2)
         # IND_OF_X_negative_by_concept = IND_OF_X_EXT[
         #     ~IND_OF_X_EXT[self.ind_index_name].isin(IND_concept)
         # ]
         # ind_index_of_negative_region: Series = IND_OF_X_negative_by_concept[self.ind_index_name]
-        # negative_region_of_X: Int64Index = X_IND[
+        # negative_region_of_X = X_IND[
         #     X_IND[self.ind_index_name].isin(ind_index_of_negative_region)
         # ].index
 
-        return lower_approximation_of_X, boundary_region_of_X, upper_approximation_of_X, negative_region_of_X
+        return lower_approximation_of_X.sort_values(), boundary_region_of_X.sort_values(), upper_approximation_of_X.sort_values(), negative_region_of_X.sort_values()
 
-    def get_approximation_objects(self, approximation_indices: Int64Index) -> (DataFrame, Series):
+    def get_approximation_objects(self, approximation_indices) -> (DataFrame, Series):
         """
         Get subset (defined by approximation_indices) of X and y objects
         """
         selection = self.y.index.isin(approximation_indices)
         return self.X[selection], self.y[selection]
```

### Comparing `roughsets-base-1.0.1.1/src/roughsets_base/roughset_si.py` & `roughsets-base-1.0.1.2/src/roughsets_base/roughset_si.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import logging
 
 import pandas as pd
-from pandas import DataFrame, Series, Int64Index
+from pandas import DataFrame, Series
 
 
 class RoughSetSI:
     """Class RoughSet to model an Information System SI = (X, A).
 
     DT = f(X, A, y),
```

### Comparing `roughsets-base-1.0.1.1/src/roughsets_base.egg-info/PKG-INFO` & `roughsets-base-1.0.1.2/src/roughsets_base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: roughsets-base
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: "The library contains base functions of the RoughSets Theory (introduced by Zdzisław Pawlak in 1982)."
 Home-page: https://github.com/darekjk/roughsets-base
 Author: Dariusz Jankowski
 Author-email: darekjki@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/darekjk/roughsets-base/issues
 Project-URL: Documentation, https://github.com/darekjk/roughsets-base/
 Project-URL: Source Code, https://github.com/darekjk/roughsets-base
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -94,21 +92,25 @@
 
 For checking of unit tests' results was used algorithms from well known reference library:  
 https://www.rdocumentation.org/packages/RoughSets/topics/RoughSets-package
 
 
 Re-Build sphinx documentation
 --------------------------
-pip install -r requirements.ci.txt  
+pip install -r requirements.dev.txt  
 sphinx-build -b html ./doc ./doc/_build/html  
 sphinx-build -b man ./doc ./doc/_build/man  
 
 
 Recommended packages
 --------------------
 
 sklearn-pandas https://github.com/scikit-learn-contrib/sklearn-pandas   
 pandas ecosystem: https://pandas.pydata.org/community/ecosystem.html  
 
 
+Citation
+--------
+  
+If You would like to use this library in Your research, please cite it.
 
-
+Jankowski, D. (2022). Roughsets-base: Python library for base Roughsets methods. (v1.0.1) [Computer software]. Zenodo. https://doi.org/10.5281/ZENODO.5957474
```

