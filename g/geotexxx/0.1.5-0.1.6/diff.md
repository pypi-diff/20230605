# Comparing `tmp/geotexxx-0.1.5.tar.gz` & `tmp/geotexxx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotexxx-0.1.5.tar", last modified: Wed May 31 14:19:51 2023, max compression
+gzip compressed data, was "geotexxx-0.1.6.tar", last modified: Mon Jun  5 08:50:43 2023, max compression
```

## Comparing `geotexxx-0.1.5.tar` & `geotexxx-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.455959 geotexxx-0.1.5/
--rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3831 2023-05-31 14:19:51.454963 geotexxx-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3573 2023-04-04 15:09:05.000000 geotexxx-0.1.5/README.md
--rw-rw-rw-   0        0        0      405 2023-05-31 14:19:37.000000 geotexxx-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 14:19:51.455959 geotexxx-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.431904 geotexxx-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.442969 geotexxx-0.1.5/src/geotexxx/
--rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.1.5/src/geotexxx/__init__.py
--rw-rw-rw-   0        0        0   103425 2023-05-31 14:17:40.000000 geotexxx-0.1.5/src/geotexxx/gefxml_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.452959 geotexxx-0.1.5/src/geotexxx.egg-info/
--rw-rw-rw-   0        0        0     3831 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 08:50:43.504740 geotexxx-0.1.6/
+-rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3831 2023-06-05 08:50:43.502616 geotexxx-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3573 2023-04-04 15:09:05.000000 geotexxx-0.1.6/README.md
+-rw-rw-rw-   0        0        0      405 2023-06-05 08:50:17.000000 geotexxx-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 08:50:43.504740 geotexxx-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 08:50:43.406331 geotexxx-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 08:50:43.432958 geotexxx-0.1.6/src/geotexxx/
+-rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.1.6/src/geotexxx/__init__.py
+-rw-rw-rw-   0        0        0   103793 2023-06-05 08:49:59.000000 geotexxx-0.1.6/src/geotexxx/gefxml_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:50:43.500616 geotexxx-0.1.6/src/geotexxx.egg-info/
+-rw-rw-rw-   0        0        0     3831 2023-06-05 08:50:43.000000 geotexxx-0.1.6/src/geotexxx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-05 08:50:43.000000 geotexxx-0.1.6/src/geotexxx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:50:43.000000 geotexxx-0.1.6/src/geotexxx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-05 08:50:43.000000 geotexxx-0.1.6/src/geotexxx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 08:50:43.000000 geotexxx-0.1.6/src/geotexxx.egg-info/top_level.txt
```

### Comparing `geotexxx-0.1.5/LICENSE.txt` & `geotexxx-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geotexxx-0.1.5/PKG-INFO` & `geotexxx-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
```

### Comparing `geotexxx-0.1.5/README.md` & `geotexxx-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `geotexxx-0.1.5/src/geotexxx/gefxml_reader.py` & `geotexxx-0.1.6/src/geotexxx/gefxml_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1649,21 +1649,27 @@
         return soillayers
 
 @dataclass
 class Multibore():
     def __init__(self):
         self.bores = []
 
-    def load_xml_sikb0101(self, xmlFile, projectName, saveFiles=True): 
+    def load_xml_sikb0101(self, xmlFile, projectName, saveFiles=True, fromFile=True): 
 
         # lees boringen in vanuit een SIKB0101 XML
         # anders dan de BRO komen alle boringen van een project in 1 bestand
-        tree = ElementTree()
-        tree.parse(xmlFile)
-        root = tree.getroot()
+        if fromFile:
+            # Standaard functionaliteit voor wanneer de XML uit een file wordt gelezen
+            tree = ElementTree()
+            tree.parse(xmlFile)
+            root = tree.getroot()
+        else:
+            # Indien het fromFile argument op False wordt gezet, kan de data uit een string worden gelezen (lezen via API)
+            # xmlFile is dan de string met XML 
+            root = ET.fromstring(xmlFile)
 
         boreholes = {} # om Layer te koppelen aan Borehole
         layers = {} # om Analysis te koppelen aan Layer
         samples = {} # om analyses te koppelen aan Sample
         filters = {} # om Sample te koppelen aan Filter
         properties = {} # voor eigenschappen 
         uppers = {} # voor niveaus van Layer, Sample en Filter
```

### Comparing `geotexxx-0.1.5/src/geotexxx.egg-info/PKG-INFO` & `geotexxx-0.1.6/src/geotexxx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
```

