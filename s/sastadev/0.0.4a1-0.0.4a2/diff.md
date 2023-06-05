# Comparing `tmp/sastadev-0.0.4a1.tar.gz` & `tmp/sastadev-0.0.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sastadev-0.0.4a1.tar", last modified: Mon Jun  5 11:39:09 2023, max compression
+gzip compressed data, was "sastadev-0.0.4a2.tar", last modified: Mon Jun  5 11:57:04 2023, max compression
```

## Comparing `sastadev-0.0.4a1.tar` & `sastadev-0.0.4a2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      143 2023-05-26 18:33:04.000000 sastadev-0.0.4a1/MANIFEST.in
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/PKG-INFO
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      207 2022-05-25 12:11:06.000000 sastadev-0.0.4a1/README.md
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/sastadev/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1533 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/LICENSE
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      136 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/__init__.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     4753 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/alpinoparsing.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    11249 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/celexlexicon.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      365 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/config.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    23928 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/deregularise.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)   111180 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/inflectioncorrection.tsv.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     5419 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/lexicon.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      197 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/memoize.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     5296 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/metadata.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1436 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/namepartlexicon.py
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.503196 sastadev-0.0.4a1/sastadev/names/
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/sastadev/names/nameparts/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)   104652 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/names/nameparts/namepartlexicon.csv
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/py.typed
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     2029 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/query.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1957 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/sastatoken.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     3321 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/sastatypes.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1282 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/sentence_parser.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    15967 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/stringfunctions.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    76827 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/treebankfunctions.py
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/sastadev.egg-info/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/PKG-INFO
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      631 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/SOURCES.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        1 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/dependency_links.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        9 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/top_level.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)       38 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/setup.cfg
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      656 2023-06-05 11:38:45.000000 sastadev-0.0.4a1/setup.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      143 2023-05-26 18:33:04.000000 sastadev-0.0.4a2/MANIFEST.in
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/PKG-INFO
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      207 2022-05-25 12:11:06.000000 sastadev-0.0.4a2/README.md
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/sastadev/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1533 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/LICENSE
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      136 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     4753 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/alpinoparsing.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    11249 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/celexlexicon.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      365 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/config.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    23928 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/deregularise.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)   111180 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/inflectioncorrection.tsv.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     5419 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/lexicon.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      197 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/memoize.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     5296 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/metadata.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1436 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/namepartlexicon.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.600349 sastadev-0.0.4a2/sastadev/names/
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/sastadev/names/nameparts/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)   104652 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/names/nameparts/namepartlexicon.csv
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/py.typed
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2029 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/query.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1957 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/sastatoken.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     3269 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/sastatypes.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1282 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/sentence_parser.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    15967 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/stringfunctions.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    76835 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/treebankfunctions.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/sastadev.egg-info/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/PKG-INFO
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      662 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        1 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        5 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/requires.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        9 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/top_level.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)       38 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/setup.cfg
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      687 2023-06-05 11:56:46.000000 sastadev-0.0.4a2/setup.py
```

### Comparing `sastadev-0.0.4a1/PKG-INFO` & `sastadev-0.0.4a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.0.4a1
+Version: 0.0.4a2
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Digital Humanities Lab, Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `sastadev-0.0.4a1/sastadev/LICENSE` & `sastadev-0.0.4a2/sastadev/LICENSE`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/alpinoparsing.py` & `sastadev-0.0.4a2/sastadev/alpinoparsing.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/celexlexicon.py` & `sastadev-0.0.4a2/sastadev/celexlexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/deregularise.py` & `sastadev-0.0.4a2/sastadev/deregularise.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/inflectioncorrection.tsv.txt` & `sastadev-0.0.4a2/sastadev/inflectioncorrection.tsv.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/lexicon.py` & `sastadev-0.0.4a2/sastadev/lexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/metadata.py` & `sastadev-0.0.4a2/sastadev/metadata.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/namepartlexicon.py` & `sastadev-0.0.4a2/sastadev/namepartlexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/names/nameparts/namepartlexicon.csv` & `sastadev-0.0.4a2/sastadev/names/nameparts/namepartlexicon.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/query.py` & `sastadev-0.0.4a2/sastadev/query.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/sastatoken.py` & `sastadev-0.0.4a2/sastadev/sastatoken.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/sastatypes.py` & `sastadev-0.0.4a2/sastadev/sastatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 IntSpan: TypeAlias = Tuple[int, int]
 AltCodeDict: TypeAlias = Dict[Item_Level, Item_Level]
 QId: TypeAlias = str  # in the futute perhaps NewType('QId', str)
 UttId: TypeAlias = str  # in the future perhaps NewType('UttId', str)
 Position: TypeAlias = int  # in the future perhapos NewType('Position', int)
 PositionStr: TypeAlias = str
 Stage: TypeAlias = int
-#SynTree: TypeAlias = etree._Element  # type: ignore
-SynTree: TypeAlias = etree.Element  # type: ignore
+SynTree: TypeAlias = etree._Element  # type: ignore
 GoldTuple: TypeAlias = Tuple[str, str, Counter]
 Item2LevelsDict: TypeAlias = Dict[Item, List[Level]]
 Match: TypeAlias = Tuple[SynTree, SynTree]
 Matches: TypeAlias = List[Match]
 MatchesDict: TypeAlias = Dict[Tuple[QId, UttId], Matches]
 MetaElement: TypeAlias = etree.Element
 ExactResult: TypeAlias = Tuple[UttId, Position]
```

### Comparing `sastadev-0.0.4a1/sastadev/sentence_parser.py` & `sastadev-0.0.4a2/sastadev/sentence_parser.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/stringfunctions.py` & `sastadev-0.0.4a2/sastadev/stringfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a1/sastadev/treebankfunctions.py` & `sastadev-0.0.4a2/sastadev/treebankfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,21 +599,21 @@
         att (str): attribute name
         fallback (str): if nothing is found
 
     Returns:
         str: attribute value or fallback value if none is found
     """
     while True:
-        if not node:
+        if node is None:
             return fallback
         val = getattval(node, att)
         if val:
             return val
         parent = node.getparent()
-        if not parent:
+        if parent is None:
             return fallback
         node = parent
 
 
 def getnodeyield(syntree: SynTree) -> List[SynTree]:
     resultlist = []
     if syntree is None:
```

### Comparing `sastadev-0.0.4a1/sastadev.egg-info/PKG-INFO` & `sastadev-0.0.4a2/sastadev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.0.4a1
+Version: 0.0.4a2
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Digital Humanities Lab, Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `sastadev-0.0.4a1/sastadev.egg-info/SOURCES.txt` & `sastadev-0.0.4a2/sastadev.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 sastadev/sastatypes.py
 sastadev/sentence_parser.py
 sastadev/stringfunctions.py
 sastadev/treebankfunctions.py
 sastadev.egg-info/PKG-INFO
 sastadev.egg-info/SOURCES.txt
 sastadev.egg-info/dependency_links.txt
+sastadev.egg-info/requires.txt
 sastadev.egg-info/top_level.txt
 sastadev/names/nameparts/namepartlexicon.csv
```

### Comparing `sastadev-0.0.4a1/setup.py` & `sastadev-0.0.4a2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name='sastadev',
     python_requires='>=3.7, <4',
-    version='0.0.4a1',
+    version='0.0.4a2',
     description='Linguistic functions for SASTA tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Digital Humanities Lab, Utrecht University',
     author_email='digitalhumanities@uu.nl',
     url='https://github.com/UUDigitalHumanitieslab/sastadev',
     license='BSD-3-Clause',
     include_package_data=True,
+    install_requires=['lxml'],
     packages=['sastadev'],
     package_data={
         'sastadev': ['*.txt', 'LICENSE', 'py.typed']
     }
 )
```

