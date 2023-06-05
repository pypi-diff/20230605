# Comparing `tmp/catencfamily-0.0.63.tar.gz` & `tmp/catencfamily-0.0.64.tar.gz`

## Comparing `catencfamily-0.0.63.tar` & `catencfamily-0.0.64.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.63/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.63/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    21868 2020-02-02 00:00:00.000000 catencfamily-0.0.63/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.63/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.63/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.63/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.63/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.64/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.64/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    21665 2020-02-02 00:00:00.000000 catencfamily-0.0.64/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.64/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.64/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.64/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.64/PKG-INFO
```

### Comparing `catencfamily-0.0.63/src/catencfamily/encoders.py` & `catencfamily-0.0.64/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.63/src/catencfamily/utils.py` & `catencfamily-0.0.64/src/catencfamily/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,36 +79,14 @@
     sns.barplot(x='importance', y='feature', data=feature_importance, color='skyblue', errorbar='sd')
     plt.xlabel('Importance', fontsize=14)
     plt.ylabel('Feature', fontsize=14)
     plt.title(f'{title} Feature Importance', fontsize=18)
     plt.grid(True, axis='x')
     plt.show()
     
-    
-    
-for name, models in trained_models.items():
-    if name in list(trained_models.keys()):
-        visualize_importance(models, list(X_train.columns), name)
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
 
 
 # https://stackoverflow.com/a/44674459
 # ToDO REMOVE zero variance threshold   <=== *****
 def remCorrFeatures(data, threshold):
     """
     Desc
```

### Comparing `catencfamily-0.0.63/LICENSE` & `catencfamily-0.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.63/README.md` & `catencfamily-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.63/pyproject.toml` & `catencfamily-0.0.64/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.63"
+version = "0.0.64"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.63/PKG-INFO` & `catencfamily-0.0.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.63
+Version: 0.0.64
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

