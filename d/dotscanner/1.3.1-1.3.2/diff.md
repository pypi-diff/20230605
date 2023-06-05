# Comparing `tmp/dotscanner-1.3.1.tar.gz` & `tmp/dotscanner-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.3.1.tar", last modified: Mon Jun  5 03:35:34 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.3.2.tar", last modified: Mon Jun  5 04:43:53 2023, max compression
```

## Comparing `dotscanner-1.3.1.tar` & `dotscanner-1.3.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.356963 dotscanner-1.3.1/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.1/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    13299 2023-06-05 03:35:34.356796 dotscanner-1.3.1/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    12644 2023-06-05 03:33:17.000000 dotscanner-1.3.1/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.352445 dotscanner-1.3.1/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3552 2023-06-05 02:53:53.000000 dotscanner-1.3.1/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     9355 2023-06-05 02:34:51.000000 dotscanner-1.3.1/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     6128 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)    10494 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     5539 2023-06-05 03:33:14.000000 dotscanner-1.3.1/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.354595 dotscanner-1.3.1/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3343 2023-06-05 02:53:52.000000 dotscanner-1.3.1/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5569 2023-06-05 02:53:50.000000 dotscanner-1.3.1/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    16340 2023-06-05 02:53:51.000000 dotscanner-1.3.1/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    15201 2023-06-05 03:33:12.000000 dotscanner-1.3.1/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-05 02:53:49.000000 dotscanner-1.3.1/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.353346 dotscanner-1.3.1/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13299 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.354989 dotscanner-1.3.1/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6218 2023-06-05 02:24:39.000000 dotscanner-1.3.1/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.1/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-05 03:35:34.357026 dotscanner-1.3.1/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-05 03:35:34.000000 dotscanner-1.3.1/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.355801 dotscanner-1.3.1/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     4369 2023-06-05 03:33:15.000000 dotscanner-1.3.1/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.356561 dotscanner-1.3.1/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)      962 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-05 02:53:50.000000 dotscanner-1.3.1/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     8414 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.366342 dotscanner-1.3.2/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.2/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-05 04:43:53.366196 dotscanner-1.3.2/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    12762 2023-06-05 04:37:56.000000 dotscanner-1.3.2/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.361753 dotscanner-1.3.2/dotscanner/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3552 2023-06-05 04:38:00.000000 dotscanner-1.3.2/dotscanner/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     9355 2023-06-05 02:34:51.000000 dotscanner-1.3.2/dotscanner/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     6128 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10494 2023-06-05 04:38:05.000000 dotscanner-1.3.2/dotscanner/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6692 2023-06-05 04:38:08.000000 dotscanner-1.3.2/dotscanner/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.363905 dotscanner-1.3.2/dotscanner/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3343 2023-06-05 02:53:52.000000 dotscanner-1.3.2/dotscanner/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5569 2023-06-05 04:37:59.000000 dotscanner-1.3.2/dotscanner/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    16340 2023-06-05 02:53:51.000000 dotscanner-1.3.2/dotscanner/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    15085 2023-06-05 04:38:06.000000 dotscanner-1.3.2/dotscanner/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-05 02:53:49.000000 dotscanner-1.3.2/dotscanner/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.362648 dotscanner-1.3.2/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.364313 dotscanner-1.3.2/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6218 2023-06-05 02:24:39.000000 dotscanner-1.3.2/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.2/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-05 04:43:53.366398 dotscanner-1.3.2/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-05 04:43:53.000000 dotscanner-1.3.2/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.365222 dotscanner-1.3.2/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     5884 2023-06-05 04:38:07.000000 dotscanner-1.3.2/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.365961 dotscanner-1.3.2/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)      962 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-05 02:53:50.000000 dotscanner-1.3.2/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     8414 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.3.1/LICENSE` & `dotscanner-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/PKG-INFO` & `dotscanner-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.1
+Version: 1.3.2
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -85,15 +85,15 @@
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
 #### Use previous analysis
-This opens a new window that allows the user to browse for a previous analysis file to use to repeat analysis.
+This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat the analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file.
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
 
 ### Descriptions of Configuration Options for the Lifetime Program
 
 #### Start image
 This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
@@ -148,15 +148,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.1
+* 1.3.2
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.1/README.md` & `dotscanner-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
 #### Use previous analysis
-This opens a new window that allows the user to browse for a previous analysis file to use to repeat analysis.
+This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat the analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file.
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
 
 ### Descriptions of Configuration Options for the Lifetime Program
 
 #### Start image
 This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
@@ -128,15 +128,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.1
+* 1.3.2
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.1/dotscanner/__main__.py` & `dotscanner-1.3.2/dotscanner/__main__.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/dataprocessing.py` & `dotscanner-1.3.2/dotscanner/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/density.py` & `dotscanner-1.3.2/dotscanner/density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/files.py` & `dotscanner-1.3.2/dotscanner/files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/lifetime.py` & `dotscanner-1.3.2/dotscanner/lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.3.2/dotscanner/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/ui/DialogWindow.py` & `dotscanner-1.3.2/dotscanner/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/ui/MicroscopeImage.py` & `dotscanner-1.3.2/dotscanner/ui/MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/ui/RegionSelector.py` & `dotscanner-1.3.2/dotscanner/ui/RegionSelector.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/ui/ThresholdAdjuster.py` & `dotscanner-1.3.2/dotscanner/ui/ThresholdAdjuster.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner/ui/UserSettings.py` & `dotscanner-1.3.2/dotscanner/ui/UserSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,14 @@
 			title="Select a .txt file generated by a previous analysis")
 		if chosenFile not in ["", " ", "/"]:
 			extension = chosenFile.split(".")[-1]
 			if extension != "txt":
 				print(strings.invalidAnalysisFileWarning(chosenFile))
 				return
 			
-			self.reanalysis = True
 			self.parseAnalysisFile(chosenFile)
 	
 	def parseAnalysisFile(self, chosenFile):
 		with open(chosenFile, "r") as file:
 			for line in file:
 				if not line.startswith("#"):
 					break
@@ -349,15 +348,16 @@
 				for pair in polygonPairsStringArray:
 					x, y = pair.split(",")
 					polygon.append([int(y), int(x)]) # More convenient shape for densities
 				polygon.append([polygon[0][0], polygon[0][1]])
 				
 				self.densityData[filename] = [lowerDotThreshScale, upperDotThreshScale, 
 				lowerBlobThreshScale, blobSize, dotSize, lowerContrast, upperContrast, polygon]
-						
+		
+		self.reanalysis = True			
 		self.window.destroy()
 		self.window.quit()
 	
 	def parseLifetimeFile(self, chosenFile):
 		self.filepath = os.path.dirname(chosenFile)
 		self.polygon = [[], []]
 		with open(chosenFile, "r") as file:
@@ -390,13 +390,11 @@
 					self.lowerContrast = round(parsedContrasts[0], 1)
 					self.upperContrast = round(parsedContrasts[1], 1)
 				
 				elif lineArray[1] == "Dot" and lineArray[2] == "size:":
 					valueArray = [item.split(":")[1] for item in line.split("|")]
 					self.dotSize = int(valueArray[0])
 					self.blobSize = int(valueArray[1])
-					self.removeEdgeFrames = bool(valueArray[2])
-					self.saveFigures = bool(valueArray[3])
-					self.skipsAllowed = int(valueArray[4])
-				
+		
+		self.reanalysis = True		
 		self.window.destroy()
 		self.window.quit()
```

### Comparing `dotscanner-1.3.1/dotscanner/ui/window.py` & `dotscanner-1.3.2/dotscanner/ui/window.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.3.2/dotscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.1
+Version: 1.3.2
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -85,15 +85,15 @@
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
 #### Use previous analysis
-This opens a new window that allows the user to browse for a previous analysis file to use to repeat analysis.
+This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat the analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file.
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
 
 ### Descriptions of Configuration Options for the Lifetime Program
 
 #### Start image
 This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
@@ -148,15 +148,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.1
+* 1.3.2
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.1/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.3.2/dotscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/settings/config.py` & `dotscanner-1.3.2/settings/config.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/settings/configmanagement.py` & `dotscanner-1.3.2/settings/configmanagement.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/setup.py` & `dotscanner-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.3.1', # Required 
+    version='1.3.2', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
```

### Comparing `dotscanner-1.3.1/tests/test_dataprocessing.py` & `dotscanner-1.3.2/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/tests/test_density.py` & `dotscanner-1.3.2/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/tests/test_files.py` & `dotscanner-1.3.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/tests/test_lifetime.py` & `dotscanner-1.3.2/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/tests/test_strings.py` & `dotscanner-1.3.2/tests/test_strings.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,14 +43,26 @@
     def test_invalidAnalysisFileWarning(self):
         self.assertEqual(
             strings.invalidAnalysisFileWarning("test_file.png"),
             f'\nInvalid analysis file selected: "test_file.png". A valid file has a .txt extension \
 and contains density or lifetime data.'
         )
     
+    def test_outputFileTopHeader(self):
+        self.assertEqual(
+            strings.outputFileTopHeader(strings.ProgramType.DENSITY),
+            f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
+# Generated output file for density measurement\n#"
+        )
+        self.assertEqual(
+            strings.outputFileTopHeader(strings.ProgramType.LIFETIME),
+            f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
+# Generated output file for lifetime measurement\n#"
+        )
+    
     def test_lifetimeOutputFileHeader(self):
         polygon = [[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]]
         thresholds = (1.5, 5.0, 2.0)
         fakeMicroscopeImage = FakeMicroscopeImage(polygon, thresholds)
         fakeUserSettings = FakeUserSettings(
                                 dotSize=2, 
                                 blobSize=5, 
@@ -61,18 +73,28 @@
         output = strings.lifetimeOutputFileHeader(fakeMicroscopeImage, fakeUserSettings)
         
         self.assertEqual(
             output,
 "# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n\
 #\n\
+# If this file is selected for re-analysis, the following settings will be read in and used unless \
+changed in the threshold adjustment window. The re-analyzed data will then be given in a new \
+output file in this same directory.\n\
+#\n\
 # Polygon vertices (x, y): (1, 1), (1, 10), (10, 10), (10, 1)\n\
 # Threshold scales: 1.5, 5.0, 2.0\n\
 # Contrast settings: 0.0, 5.0\n\
-# Dot size: 2 | Blob size: 5 | Remove edge frames: True | Save figures: False | Skips allowed: 1\n\
+# Dot size: 2 | Blob size: 5\n\
+#\n\
+# The following settings were used in this analysis, but will not be read in during re-analysis \
+(these and other settings can be adjusted in the config file using the \"Edit defaults\" button \
+in the main configuration window):\n\
+#\n\
+# Remove edge frames: True | Save figures: False | Skips allowed: 1\n\
 #\n\
 # The data columns are organized as follows:\n\
 # x | y | lifetime | starting image | displacement squared (sq px)\n#\n"
         )
     
     def test_lifetimeOutputFileHeaderWithStartImage(self):
         polygon = [[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]]
@@ -89,18 +111,28 @@
         output = strings.lifetimeOutputFileHeader(fakeMicroscopeImage, fakeUserSettings)
         
         self.assertEqual(
             output,
 "# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n\
 #\n\
+# If this file is selected for re-analysis, the following settings will be read in and used unless \
+changed in the threshold adjustment window. The re-analyzed data will then be given in a new \
+output file in this same directory.\n\
+#\n\
 # Polygon vertices (x, y): (1, 1), (1, 10), (10, 10), (10, 1)\n\
 # Threshold scales: 1.5, 5.0, 2.0\n\
 # Contrast settings: 0.0, 5.0\n\
-# Dot size: 2 | Blob size: 5 | Remove edge frames: True | Save figures: False | \
+# Dot size: 2 | Blob size: 5\n\
+#\n\
+# The following settings were used in this analysis, but will not be read in during re-analysis \
+(these and other settings can be adjusted in the config file using the \"Edit defaults\" button \
+in the main configuration window):\n\
+#\n\
+# Remove edge frames: True | Save figures: False | \
 Skips allowed: 1 | Start image: image.png\n\
 #\n\
 # The data columns are organized as follows:\n\
 # x | y | lifetime | starting image | displacement squared (sq px)\n#\n"
         )
 
 if __name__ == "__main__":
```

### Comparing `dotscanner-1.3.1/tests/ui/FakeUserSettings.py` & `dotscanner-1.3.2/tests/ui/FakeUserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/tests/ui/test_MicroscopeImage.py` & `dotscanner-1.3.2/tests/ui/test_MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.1/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.3.2/tests/ui/test_ThresholdAdjuster.py`

 * *Files identical despite different names*

