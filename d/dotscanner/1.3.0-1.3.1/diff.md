# Comparing `tmp/dotscanner-1.3.0.tar.gz` & `tmp/dotscanner-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.3.0.tar", last modified: Mon Jun  5 03:16:55 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.3.1.tar", last modified: Mon Jun  5 03:35:34 2023, max compression
```

## Comparing `dotscanner-1.3.0.tar` & `dotscanner-1.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.392806 dotscanner-1.3.0/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.0/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    13274 2023-06-05 03:16:55.392655 dotscanner-1.3.0/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    12617 2023-06-05 03:13:05.000000 dotscanner-1.3.0/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.387288 dotscanner-1.3.0/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3552 2023-06-05 02:53:53.000000 dotscanner-1.3.0/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     9355 2023-06-05 02:34:51.000000 dotscanner-1.3.0/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     6128 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)    10494 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     5321 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.389727 dotscanner-1.3.0/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3343 2023-06-05 02:53:52.000000 dotscanner-1.3.0/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5569 2023-06-05 02:53:50.000000 dotscanner-1.3.0/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    16340 2023-06-05 02:53:51.000000 dotscanner-1.3.0/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    14995 2023-06-05 02:53:52.000000 dotscanner-1.3.0/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-05 02:53:49.000000 dotscanner-1.3.0/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.388224 dotscanner-1.3.0/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13274 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.390485 dotscanner-1.3.0/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6218 2023-06-05 02:24:39.000000 dotscanner-1.3.0/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.0/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-05 03:16:55.392863 dotscanner-1.3.0/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-05 03:16:55.000000 dotscanner-1.3.0/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.391579 dotscanner-1.3.0/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     4068 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.392401 dotscanner-1.3.0/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)      962 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-05 02:53:50.000000 dotscanner-1.3.0/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     8414 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.356963 dotscanner-1.3.1/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.1/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    13299 2023-06-05 03:35:34.356796 dotscanner-1.3.1/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    12644 2023-06-05 03:33:17.000000 dotscanner-1.3.1/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.352445 dotscanner-1.3.1/dotscanner/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3552 2023-06-05 02:53:53.000000 dotscanner-1.3.1/dotscanner/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     9355 2023-06-05 02:34:51.000000 dotscanner-1.3.1/dotscanner/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     6128 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10494 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     5539 2023-06-05 03:33:14.000000 dotscanner-1.3.1/dotscanner/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.354595 dotscanner-1.3.1/dotscanner/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3343 2023-06-05 02:53:52.000000 dotscanner-1.3.1/dotscanner/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5569 2023-06-05 02:53:50.000000 dotscanner-1.3.1/dotscanner/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    16340 2023-06-05 02:53:51.000000 dotscanner-1.3.1/dotscanner/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    15201 2023-06-05 03:33:12.000000 dotscanner-1.3.1/dotscanner/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/dotscanner/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-05 02:53:49.000000 dotscanner-1.3.1/dotscanner/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.353346 dotscanner-1.3.1/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    13299 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-05 03:35:34.000000 dotscanner-1.3.1/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.354989 dotscanner-1.3.1/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6218 2023-06-05 02:24:39.000000 dotscanner-1.3.1/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.1/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-05 03:35:34.357026 dotscanner-1.3.1/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-05 03:35:34.000000 dotscanner-1.3.1/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.355801 dotscanner-1.3.1/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     4369 2023-06-05 03:33:15.000000 dotscanner-1.3.1/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:35:34.356561 dotscanner-1.3.1/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)      962 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-05 02:53:50.000000 dotscanner-1.3.1/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     8414 2023-06-05 02:24:39.000000 dotscanner-1.3.1/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.3.0/LICENSE` & `dotscanner-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/PKG-INFO` & `dotscanner-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.0
+Version: 1.3.1
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -148,14 +148,16 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
+* 1.3.1
+     * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
      * Added startup processes to check the configuration file for errors
```

### Comparing `dotscanner-1.3.0/README.md` & `dotscanner-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,16 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
+* 1.3.1
+     * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
      * Added startup processes to check the configuration file for errors
```

### Comparing `dotscanner-1.3.0/dotscanner/__main__.py` & `dotscanner-1.3.1/dotscanner/__main__.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/dataprocessing.py` & `dotscanner-1.3.1/dotscanner/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/density.py` & `dotscanner-1.3.1/dotscanner/density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/files.py` & `dotscanner-1.3.1/dotscanner/files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/lifetime.py` & `dotscanner-1.3.1/dotscanner/lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/strings.py` & `dotscanner-1.3.1/dotscanner/strings.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,19 @@
 	return f"{filename} {dotTotal} {surveyedArea} {density} {error} {thresholds[0]} \
 {thresholds[1]} {thresholds[2]} {blobSize} {dotSize} {lowerContrast} {upperContrast} \
 {verticesString}\n"
 
 def fileSkippedNotification(filename):
 	return f"\nFile {filename} skipped"
 
+def invalidAnalysisFileWarning(filepath):
+	filename = filepath.split("/")[-1]
+	return f'\nInvalid analysis file selected: "{filename}". A valid file has a .txt extension \
+and contains density or lifetime data.'
+
 def lifetimeOutputFileHeader(microscopeImage, userSettings):
 	verticesStringList = []
 	for vertex in microscopeImage.polygon[:-1]:
 		y, x = vertex
 		verticesStringList.append(f"({x}, {y})")
 	verticesString = ", ".join(verticesStringList)
```

### Comparing `dotscanner-1.3.0/dotscanner/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.3.1/dotscanner/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/ui/DialogWindow.py` & `dotscanner-1.3.1/dotscanner/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/ui/MicroscopeImage.py` & `dotscanner-1.3.1/dotscanner/ui/MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/ui/RegionSelector.py` & `dotscanner-1.3.1/dotscanner/ui/RegionSelector.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/ui/ThresholdAdjuster.py` & `dotscanner-1.3.1/dotscanner/ui/ThresholdAdjuster.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner/ui/UserSettings.py` & `dotscanner-1.3.1/dotscanner/ui/UserSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,19 @@
 			self.labelWarning.pack()
 		self.checkForWarning()
 	
 	def usePreviousAnalysis(self):
 		chosenFile = filedialog.askopenfilename(initialdir=self.filepath, 
 			title="Select a .txt file generated by a previous analysis")
 		if chosenFile not in ["", " ", "/"]:
+			extension = chosenFile.split(".")[-1]
+			if extension != "txt":
+				print(strings.invalidAnalysisFileWarning(chosenFile))
+				return
+			
 			self.reanalysis = True
 			self.parseAnalysisFile(chosenFile)
 	
 	def parseAnalysisFile(self, chosenFile):
 		with open(chosenFile, "r") as file:
 			for line in file:
 				if not line.startswith("#"):
@@ -312,14 +317,16 @@
 					programString = lineArray[5]
 					if programString == "density":
 						self.program = ProgramType.DENSITY
 						self.parseDensityFile(chosenFile)
 					else:
 						self.program = ProgramType.LIFETIME
 						self.parseLifetimeFile(chosenFile)
+		
+		print(strings.invalidAnalysisFileWarning(chosenFile))
 	
 	def parseDensityFile(self, chosenFile):
 		self.filepath = os.path.dirname(chosenFile)
 		with open(chosenFile, "r") as file:
 			for line in file:
 				if line.startswith("#"):
 					continue
```

### Comparing `dotscanner-1.3.0/dotscanner/ui/window.py` & `dotscanner-1.3.1/dotscanner/ui/window.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.3.1/dotscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.0
+Version: 1.3.1
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -148,14 +148,16 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
+* 1.3.1
+     * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
      * Added startup processes to check the configuration file for errors
```

### Comparing `dotscanner-1.3.0/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.3.1/dotscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/settings/config.py` & `dotscanner-1.3.1/settings/config.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/settings/configmanagement.py` & `dotscanner-1.3.1/settings/configmanagement.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/setup.py` & `dotscanner-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.3.0', # Required 
+    version='1.3.1', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
```

### Comparing `dotscanner-1.3.0/tests/test_dataprocessing.py` & `dotscanner-1.3.1/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/tests/test_density.py` & `dotscanner-1.3.1/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/tests/test_files.py` & `dotscanner-1.3.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/tests/test_lifetime.py` & `dotscanner-1.3.1/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/tests/test_strings.py` & `dotscanner-1.3.1/tests/test_strings.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         )
     
     def test_fileSkippedNotification(self):
         output = strings.fileSkippedNotification("test.png")
         
         self.assertEqual(output, "\nFile test.png skipped")
     
+    def test_invalidAnalysisFileWarning(self):
+        self.assertEqual(
+            strings.invalidAnalysisFileWarning("test_file.png"),
+            f'\nInvalid analysis file selected: "test_file.png". A valid file has a .txt extension \
+and contains density or lifetime data.'
+        )
+    
     def test_lifetimeOutputFileHeader(self):
         polygon = [[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]]
         thresholds = (1.5, 5.0, 2.0)
         fakeMicroscopeImage = FakeMicroscopeImage(polygon, thresholds)
         fakeUserSettings = FakeUserSettings(
                                 dotSize=2, 
                                 blobSize=5,
```

### Comparing `dotscanner-1.3.0/tests/ui/FakeUserSettings.py` & `dotscanner-1.3.1/tests/ui/FakeUserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/tests/ui/test_MicroscopeImage.py` & `dotscanner-1.3.1/tests/ui/test_MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.0/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.3.1/tests/ui/test_ThresholdAdjuster.py`

 * *Files identical despite different names*

