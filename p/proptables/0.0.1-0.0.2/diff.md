# Comparing `tmp/proptables-0.0.1.tar.gz` & `tmp/proptables-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proptables-0.0.1.tar", last modified: Mon Jun  5 13:23:00 2023, max compression
+gzip compressed data, was "proptables-0.0.2.tar", last modified: Mon Jun  5 16:05:49 2023, max compression
```

## Comparing `proptables-0.0.1.tar` & `proptables-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:23:00.626232 proptables-0.0.1/
--rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       24 2023-06-05 13:17:38.000000 proptables-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1243 2023-06-05 13:23:00.626232 proptables-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-06-05 13:17:20.000000 proptables-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 13:23:00.609505 proptables-0.0.1/proptables/
--rw-rw-rw-   0        0        0     2347 2023-06-02 17:01:37.000000 proptables-0.0.1/proptables/R134a_PresSat.csv
--rw-rw-rw-   0        0        0      239 2023-06-03 09:24:40.000000 proptables-0.0.1/proptables/R134a_SupPreSat.csv
--rw-rw-rw-   0        0        0     9777 2023-06-03 09:06:51.000000 proptables-0.0.1/proptables/R134a_Super.csv
--rw-rw-rw-   0        0        0     3736 2023-06-02 17:03:14.000000 proptables-0.0.1/proptables/R134a_TempSat.csv
--rw-rw-rw-   0        0        0       33 2023-06-05 13:16:54.000000 proptables-0.0.1/proptables/__init__.py
--rw-rw-rw-   0        0        0     3388 2023-06-05 13:16:10.000000 proptables-0.0.1/proptables/calSatData.py
--rw-rw-rw-   0        0        0     5060 2023-06-05 13:16:18.000000 proptables-0.0.1/proptables/calSuperHeatData.py
--rw-rw-rw-   0        0        0      130 2023-06-05 13:16:47.000000 proptables-0.0.1/proptables/import_data.py
--rw-rw-rw-   0        0        0      113 2023-06-02 19:28:41.000000 proptables-0.0.1/proptables/interpolate.py
--rw-rw-rw-   0        0        0     1155 2023-06-05 13:17:05.000000 proptables-0.0.1/proptables/main.py
--rw-rw-rw-   0        0        0     5655 2023-06-05 13:21:32.000000 proptables-0.0.1/proptables/superheated.py
--rw-rw-rw-   0        0        0     1700 2023-06-05 13:16:58.000000 proptables-0.0.1/proptables/test.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:23:00.624685 proptables-0.0.1/proptables.egg-info/
--rw-rw-rw-   0        0        0     1243 2023-06-05 13:23:00.000000 proptables-0.0.1/proptables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-05 13:23:00.000000 proptables-0.0.1/proptables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:23:00.000000 proptables-0.0.1/proptables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 13:23:00.000000 proptables-0.0.1/proptables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-06-05 13:23:00.626232 proptables-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 16:05:49.692846 proptables-0.0.2/
+-rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       24 2023-06-05 13:17:38.000000 proptables-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1243 2023-06-05 16:05:49.692846 proptables-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2023-06-05 13:17:20.000000 proptables-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:05:49.682834 proptables-0.0.2/proptables/
+-rw-rw-rw-   0        0        0     2347 2023-06-02 17:01:37.000000 proptables-0.0.2/proptables/R134a_PresSat.csv
+-rw-rw-rw-   0        0        0      239 2023-06-03 09:24:40.000000 proptables-0.0.2/proptables/R134a_SupPreSat.csv
+-rw-rw-rw-   0        0        0     9777 2023-06-03 09:06:51.000000 proptables-0.0.2/proptables/R134a_Super.csv
+-rw-rw-rw-   0        0        0     3736 2023-06-02 17:03:14.000000 proptables-0.0.2/proptables/R134a_TempSat.csv
+-rw-rw-rw-   0        0        0       33 2023-06-05 13:16:54.000000 proptables-0.0.2/proptables/__init__.py
+-rw-rw-rw-   0        0        0     3340 2023-06-05 15:23:13.000000 proptables-0.0.2/proptables/calSatData.py
+-rw-rw-rw-   0        0        0     5031 2023-06-05 15:22:59.000000 proptables-0.0.2/proptables/calSuperHeatData.py
+-rw-rw-rw-   0        0        0      621 2023-06-05 16:05:15.000000 proptables-0.0.2/proptables/import_data.py
+-rw-rw-rw-   0        0        0      113 2023-06-02 19:28:41.000000 proptables-0.0.2/proptables/interpolate.py
+-rw-rw-rw-   0        0        0     1155 2023-06-05 14:57:32.000000 proptables-0.0.2/proptables/main.py
+-rw-rw-rw-   0        0        0     5646 2023-06-05 15:23:49.000000 proptables-0.0.2/proptables/superheated.py
+-rw-rw-rw-   0        0        0     1704 2023-06-05 15:16:17.000000 proptables-0.0.2/proptables/test.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:05:49.692846 proptables-0.0.2/proptables.egg-info/
+-rw-rw-rw-   0        0        0     1243 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-06-05 16:05:49.692846 proptables-0.0.2/setup.cfg
```

### Comparing `proptables-0.0.1/LICENCE.txt` & `proptables-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `proptables-0.0.1/PKG-INFO` & `proptables-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.1
+Version: 0.0.2
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proptables-0.0.1/README.md` & `proptables-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `proptables-0.0.1/proptables/R134a_PresSat.csv` & `proptables-0.0.2/proptables/R134a_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.1/proptables/R134a_Super.csv` & `proptables-0.0.2/proptables/R134a_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.1/proptables/R134a_TempSat.csv` & `proptables-0.0.2/proptables/R134a_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.1/proptables/calSatData.py` & `proptables-0.0.2/proptables/calSatData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import pandas as pd
 from pathlib import Path
-
-data_path3 = Path(Path.cwd(), 'proptables', 'R134a_PresSat.csv')
-data_path4 = Path(Path.cwd(), 'proptables', 'R134a_TempSat.csv')
+from proptables.import_data import data_path_TempSat,data_path_PresSat
 
 class SaturatedData:
     def __init__(self):
-        self.dfPressure=pd.read_csv(data_path3)
+        self.dfPressure=pd.read_csv(data_path_PresSat)
         self.dfPressure=self.dfPressure.iloc[: , :-1]
-        self.dfTemperature=pd.read_csv(data_path4)
+        self.dfTemperature=pd.read_csv(data_path_TempSat)
         self.dfTemperature=self.dfTemperature.iloc[: , :-1]
 
 
     def FindbyTemp(self,Temperature):
         if Temperature in self.dfTemperature["degC"].unique():
             indexing=self.dfTemperature[self.dfTemperature["degC"]==Temperature].index.values
             row=self.dfTemperature.iloc[indexing]
```

### Comparing `proptables-0.0.1/proptables/calSuperHeatData.py` & `proptables-0.0.2/proptables/calSuperHeatData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pandas as pd
 from proptables.superheated import superheatedtable
-from pathlib import Path
+from proptables.import_data import data_path_SupPreSat
 
-data_path1 = Path(Path.cwd(), 'proptables', 'R134a_SupPreSat.csv')
 class HeatedCalculater:
     def __init__(self):
-        self.dfSupSat=pd.read_csv(data_path1)
+        self.dfSupSat=pd.read_csv(data_path_SupPreSat)
 
     def superheatedTable(self,Pressure):
         result=superheatedtable(Pressure)
         result=result.reset_index(drop=True)
         result=result.set_axis(["Temp","v","energy","enthalpy","entropy"],axis=1)
         if Pressure in self.dfSupSat["Pressure"].values:
             indexing=self.dfSupSat[self.dfSupSat["Pressure"].values==Pressure].index.values
```

### Comparing `proptables-0.0.1/proptables/main.py` & `proptables-0.0.2/proptables/main.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.1/proptables/superheated.py` & `proptables-0.0.2/proptables/superheated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import pandas as pd
 from bisect import bisect_left
 from pathlib import Path
-
-data_path2 = Path(Path.cwd(), 'proptables', 'R134a_Super.csv')
+from proptables.import_data import data_path_Super
 
 class SuperHeated:
     def __init__(self):   
-        self.dfSuperHeated=pd.read_csv(data_path2,header=None)
+        self.dfSuperHeated=pd.read_csv(data_path_Super,header=None)
 
 
     ######################################################### Super Heated 1st Tables###################################
     def superheated_Pres_60(self):
         table=self.dfSuperHeated.iloc[2:17,0:5]
         return table
```

### Comparing `proptables-0.0.1/proptables/test.py` & `proptables-0.0.2/proptables/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from proptables.main import R134a
+from proptables.__init__ import R134a
 
 
 #################### Check for Temp Saturated Table####################
 
 check_1=True
 
 if check_1:
```

### Comparing `proptables-0.0.1/proptables.egg-info/PKG-INFO` & `proptables-0.0.2/proptables.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.1
+Version: 0.0.2
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proptables-0.0.1/setup.cfg` & `proptables-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7074 6162 6c65 730d 0a76   = proptables..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e31 0d0a  ersion = 0.0.1..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
 00000030: 6175 7468 6f72 203d 2042 7564 6468 6920  author = Buddhi 
 00000040: 5769 6a65 6e61 7961 6b65 0d0a 6175 7468  Wijenayake..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696a 656e  or_email = wijen
 00000060: 6179 616b 6562 7564 6468 6933 3438 3032  ayakebuddhi34802
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 466f 7220 6765  ription = For ge
 00000090: 6e65 7261 7469 6e67 2070 726f 7065 7274  nerating propert
```

