# Comparing `tmp/catencfamily-0.0.62.tar.gz` & `tmp/catencfamily-0.0.63.tar.gz`

## Comparing `catencfamily-0.0.62.tar` & `catencfamily-0.0.63.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catencfamily-0.0.62/.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.62/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.62/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 catencfamily-0.0.62/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.62/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.62/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.62/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.62/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.63/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.63/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    21868 2020-02-02 00:00:00.000000 catencfamily-0.0.63/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.63/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.63/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.63/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.63/PKG-INFO
```

### Comparing `catencfamily-0.0.62/src/catencfamily/encoders.py` & `catencfamily-0.0.63/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.62/src/catencfamily/utils.py` & `catencfamily-0.0.63/src/catencfamily/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 3rd June, 2023
+# 5th June, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
@@ -55,14 +55,60 @@
         # Also save these features
         filename = pathlib.Path(master) / filename
         with open(filename,'w') as tfile:
             tfile.write('\n'.join(fe_1))
     return fe_1, fe_0
    
 
+# Ref: https://www.kaggle.com/code/tetsutani/ps3e16-eda-ensemble-ml-pipeline
+# For multiple models
+def visualize_importance(models, feature_cols, title, top=9):
+    importances = []
+    feature_importance = pd.DataFrame()
+    for i, model in enumerate(models):
+        _df = pd.DataFrame()
+        _df["importance"] = model.feature_importances_
+        _df["feature"] = pd.Series(feature_cols)
+        _df["fold"] = i
+        _df = _df.sort_values('importance', ascending=False)
+        _df = _df.head(top)
+        feature_importance = pd.concat([feature_importance, _df], axis=0, ignore_index=True)
+        
+    feature_importance = feature_importance.sort_values('importance', ascending=False)
+    # display(feature_importance.groupby(["feature"]).mean().reset_index().drop('fold', axis=1))
+    plt.figure(figsize=(12, 4))
+    sns.barplot(x='importance', y='feature', data=feature_importance, color='skyblue', errorbar='sd')
+    plt.xlabel('Importance', fontsize=14)
+    plt.ylabel('Feature', fontsize=14)
+    plt.title(f'{title} Feature Importance', fontsize=18)
+    plt.grid(True, axis='x')
+    plt.show()
+    
+    
+    
+for name, models in trained_models.items():
+    if name in list(trained_models.keys()):
+        visualize_importance(models, list(X_train.columns), name)
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
 
 # https://stackoverflow.com/a/44674459
 # ToDO REMOVE zero variance threshold   <=== *****
 def remCorrFeatures(data, threshold):
     """
     Desc
@@ -110,16 +156,21 @@
     df['max'] = np.max(df,axis =1)
     df['kurtosis'] = kurtosis(df.values, axis =1 )
     return df
 
 
 
 # Generate data using sklearn's make_classification
-def generateSklearnData(X,y, test_size = 0.25, bins = 20, genColName = True):
+def transformToCatFeatures(X,y, test_size = 0.25, bins = 20, genColName = True):
     """
+    Calls: transformFeatures()
+    Called by: main()
+    
+    Desc
+    ----
     The function discretises X assuming all features in X
     have continuous values. Discretisation of all features 
     is perfomed as per number of 'bins' specified. 
     We then have two datasets: original and discretised.
     Both original and discretised versions continue to have 
     the same row-orderings. And hence returned sample of continuous
     data corresponds to returned sample of discrete data.
@@ -144,15 +195,15 @@
         Has discrete features
 
     """
     X_data = np.array(X)
     y_data = np.array(y)
     colnames = list(X.columns)
     
-    orig_train, orig_test,train_binned,test_binned = transformToCatFeatures(X_data,y_data, test_size, bins, colnames, genColName)
+    orig_train, orig_test,train_binned,test_binned = transformFeatures(X_data,y_data, test_size, bins, colnames, genColName)
     return orig_train, orig_test, train_binned, test_binned    
 
 
 
 
 
 
@@ -202,22 +253,27 @@
                                 class_sep = class_sep,
                                 flip_y = flip_y
                              )
     
     X_data = np.array(X)
     y_data = np.array(y)
     
-    orig_train, orig_test,train_binned,test_binned = transformToCatFeatures(X_data,y_data, test_size, bins, genColName)
+    orig_train, orig_test,train_binned,test_binned = transformFeatures(X_data,y_data, test_size, bins, genColName)
     return orig_train, orig_test, train_binned, test_binned    
 
 
  
-def transformToCatFeatures(X_data,y_data, test_size = 0.25, bins= 20,  colnames = None, genColName = True):
+def transformFeatures(X_data,y_data, test_size = 0.25, bins= 20,  colnames = None, genColName = True):
     
     """
+    Called by: transformToCatFeatures() , generateClassificationData
+    Calls: None
+    
+    Desc
+    ----
     Given a DataFrame X_data having only continuous features, 
     and y_data the target, the function bins each feature. 
     The resulting dataframe as also the original is partitioned
     into train/test as per specified test_size.
     Parameters
     ----------
     X_data : A pandas DataFrame (data features)
```

### Comparing `catencfamily-0.0.62/LICENSE` & `catencfamily-0.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.62/README.md` & `catencfamily-0.0.63/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.62/pyproject.toml` & `catencfamily-0.0.63/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.62"
+version = "0.0.63"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.62/PKG-INFO` & `catencfamily-0.0.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.62
+Version: 0.0.63
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

