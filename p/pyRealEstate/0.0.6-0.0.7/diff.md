# Comparing `tmp/pyRealEstate-0.0.6.tar.gz` & `tmp/pyRealEstate-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.6.tar", last modified: Mon Jun  5 17:13:53 2023, max compression
+gzip compressed data, was "pyRealEstate-0.0.7.tar", last modified: Mon Jun  5 17:41:31 2023, max compression
```

## Comparing `pyRealEstate-0.0.6.tar` & `pyRealEstate-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:13:53.328677 pyRealEstate-0.0.6/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/Pre_Processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/Time_Trending.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/Pre_Processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/Time_Trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/setup.cfg
```

### Comparing `pyRealEstate-0.0.6/LICENSE` & `pyRealEstate-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.6/PKG-INFO` & `pyRealEstate-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.6
+Version: 0.0.7
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.0.6/README.md` & `pyRealEstate-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.6/pyRealEstate/Pre_Processing.py` & `pyRealEstate-0.0.7/pyRealEstate/Pre_Processing.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,11 +16,11 @@
   if n_unique == 1:
     rtn = uniquecols[uniquecols == 1].index.tolist()
   else :
     rtn = uniquecols[uniquecols <=  n_unique ].index.tolist()
   return rtn
 
 
-def ID_in_Data(dataf , n_unique = 1):
+def ID_in_Data(dataf ):
   ML = len(dataf)
   uniquecols = dataf.apply(pd.Series.nunique)
   return uniquecols[uniquecols == ML].index.tolist()
```

### Comparing `pyRealEstate-0.0.6/pyRealEstate/RealEstateMetrics.py` & `pyRealEstate-0.0.7/pyRealEstate/RealEstateMetrics.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.6/pyRealEstate/Time_Trending.py` & `pyRealEstate-0.0.7/pyRealEstate/Time_Trending.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,34 +31,34 @@
                               , columns = bestTimeModel.model.data.param_names
                               , index = bestTimeModel.model.data.row_labels)
 
     predData = pd.DataFrame({
                                'const' : 1
                                , 'Months' : range(0, modelData['Months'].max() + 1)} , index = range(0, modelData['Months'].max() + 1))
 
-    if Time_Model.df_model > 1:
-      for x in range(2, int(Time_Model.df_model) + 1):
+    if bestTimeModel.df_model > 1:
+      for x in range(2, int(bestTimeModel.df_model) + 1):
         predData['Months' + str(x)] = predData['Months'] ** x
     self.pred_data = predData
 
     if return_model ==True:
       return bestTimeModel
   
   def Display_Time_Trend(self): 
     plt.plot(-self.pred_data['Months'], self.Time_Model.predict(self.pred_data), '-', color = 'red', linewidth = 3)
     plt.axhline(self.Time_Model.predict(self.pred_data).loc[0], color='k', linestyle='--')
     plt.show()
 
   def Adjustment_Rate_Return(self, as_pandas =False):
     if as_pandas == True :
-      predDataResults = predData.copy()
-      predDataResults['Model_Prediction'] = Time_Model.predict(predData)
-      predDataResults['AdjustMent_Rate'] = Time_Model.predict(predData).loc[0] / Time_Model.predict(predData)
+      predDataResults = self.pred_data.copy()
+      predDataResults['Model_Prediction'] = self.Time_Model.predict(self.pred_data)
+      predDataResults['AdjustMent_Rate'] = self.Time_Model.predict(self.pred_data).loc[0] / self.Time_Model.predict(self.pred_data)
       return predDataResults[['Months','AdjustMent_Rate']]
 
     else:
-      rateTable = self.Time_Model.predict(self.pred_data).loc[0] / Time_Model.predict(self.pred_data)
+      rateTable = self.Time_Model.predict(self.pred_data).loc[0] / self.Time_Model.predict(self.pred_data)
       rateTable.name = 'AdjRate'
       return rateTable
     
   def trend_summary(self):
     return self.Time_Model.summary()
```

### Comparing `pyRealEstate-0.0.6/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.0.7/pyRealEstate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.6
+Version: 0.0.7
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.0.6/pypi_description.md` & `pyRealEstate-0.0.7/pypi_description.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.6/setup.cfg` & `pyRealEstate-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.0.6
+version = 0.0.7
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
```

