# Comparing `tmp/sastadev-0.0.3.tar.gz` & `tmp/sastadev-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sastadev-0.0.3.tar", last modified: Tue Dec  6 13:28:46 2022, max compression
+gzip compressed data, was "sastadev-0.0.4a1.tar", last modified: Mon Jun  5 11:39:09 2023, max compression
```

## Comparing `sastadev-0.0.3.tar` & `sastadev-0.0.4a1.tar`

### file list

```diff
@@ -1,38 +1,33 @@
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.598135 sastadev-0.0.3/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      143 2022-12-06 13:19:30.000000 sastadev-0.0.3/MANIFEST.in
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      565 2022-12-06 13:28:46.598135 sastadev-0.0.3/PKG-INFO
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      207 2022-05-25 12:11:06.000000 sastadev-0.0.3/README.md
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.570135 sastadev-0.0.3/sastadev/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1533 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/LICENSE
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      136 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/__init__.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     4753 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/alpinoparsing.py
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.566135 sastadev-0.0.3/sastadev/celexlexicon/
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.594135 sastadev-0.0.3/sastadev/celexlexicon/dutch/
--rw-rw-r--   0 sheean    (1000) sheean    (1000) 10433870 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/celexlexicon/dutch/DMLCD.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000) 11540324 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/celexlexicon/dutch/DMWCDOK.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)  4092534 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/celexlexicon/dutch/DSLCD.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    11241 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/celexlexicon.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      365 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/config.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    23928 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/deregularise.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)   111180 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/inflectioncorrection.tsv.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     5419 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/lexicon.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      197 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/memoize.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     5296 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/metadata.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1436 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/namepartlexicon.py
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.566135 sastadev-0.0.3/sastadev/names/
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.598135 sastadev-0.0.3/sastadev/names/nameparts/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)   104652 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/names/nameparts/namepartlexicon.csv
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/py.typed
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     2029 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/query.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1957 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/sastatoken.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     2588 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/sastatypes.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1282 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/sentence_parser.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    15967 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/stringfunctions.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    81977 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev/treebankfunctions.py
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-12-06 13:28:46.570135 sastadev-0.0.3/sastadev.egg-info/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      565 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev.egg-info/PKG-INFO
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      747 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev.egg-info/SOURCES.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        1 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev.egg-info/dependency_links.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        9 2022-12-06 13:28:46.000000 sastadev-0.0.3/sastadev.egg-info/top_level.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)       38 2022-12-06 13:28:46.598135 sastadev-0.0.3/setup.cfg
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      654 2022-12-06 13:19:30.000000 sastadev-0.0.3/setup.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      143 2023-05-26 18:33:04.000000 sastadev-0.0.4a1/MANIFEST.in
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/PKG-INFO
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      207 2022-05-25 12:11:06.000000 sastadev-0.0.4a1/README.md
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/sastadev/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1533 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/LICENSE
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      136 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     4753 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/alpinoparsing.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    11249 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/celexlexicon.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      365 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/config.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    23928 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/deregularise.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)   111180 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/inflectioncorrection.tsv.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     5419 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/lexicon.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      197 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/memoize.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     5296 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/metadata.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1436 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/namepartlexicon.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.503196 sastadev-0.0.4a1/sastadev/names/
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/sastadev/names/nameparts/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)   104652 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/names/nameparts/namepartlexicon.csv
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/py.typed
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2029 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/query.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1957 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/sastatoken.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     3321 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/sastatypes.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1282 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/sentence_parser.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    15967 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/stringfunctions.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    76827 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev/treebankfunctions.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/sastadev.egg-info/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/PKG-INFO
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      631 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        1 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        9 2023-06-05 11:39:09.000000 sastadev-0.0.4a1/sastadev.egg-info/top_level.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)       38 2023-06-05 11:39:09.507196 sastadev-0.0.4a1/setup.cfg
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      656 2023-06-05 11:38:45.000000 sastadev-0.0.4a1/setup.py
```

### Comparing `sastadev-0.0.3/PKG-INFO` & `sastadev-0.0.4a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.0.3
+Version: 0.0.4a1
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Digital Humanities Lab, Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `sastadev-0.0.3/sastadev/LICENSE` & `sastadev-0.0.4a1/sastadev/LICENSE`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/alpinoparsing.py` & `sastadev-0.0.4a1/sastadev/alpinoparsing.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/celexlexicon.py` & `sastadev-0.0.4a1/sastadev/celexlexicon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 The CELEX lexicon consists of 3 backslash-separated value files:
 
 * DMW (dmwcdok.txt): word forms and their properties
 * DML (dmlcd.txt): lemmas and their morphological properties
 * DSL (dslcd.txt): lemmas and their syntactic properties
 
-These files can be found in the folder celexlexicon/dutch in the code folder.
+These files can be found in the folder celexlexicondata/dutch in the code folder.
 
 We store these in the celexlexicon module in python dictionaries:
 
 * dmwkeydict: key = word identifier, value = whole record for this identifier
 * dmldict: key = lemma identifier, value = whole record for this identifier
 * dsldict: key = lemma identifier, value = whole dsl record for this identifier
 
@@ -48,15 +48,15 @@
 # verbs that do not necessarily have a t suffix  in present tense singular
 no_t_verbs = {'mogen', 'kunnen', 'zullen', 'willen'}
 
 logfile = sys.stderr
 
 # initialisation
 # read the celex lexicon
-inputfolder = os.path.join(SD_DIR, 'celexlexicon', 'dutch')
+inputfolder = os.path.join(SD_DIR, 'celexlexicondata', 'dutch')
 
 dmwfilename = 'DMWCDOK.txt'
 dmwfullname = os.path.join(inputfolder, dmwfilename)
 dmwdict: Dict[str, List[str]] = {}
 dmwlemmakeyinflindex: Dict[Tuple[str, str], List[str]] = defaultdict(list)
 dmwkeydict = {}
```

### Comparing `sastadev-0.0.3/sastadev/deregularise.py` & `sastadev-0.0.4a1/sastadev/deregularise.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/inflectioncorrection.tsv.txt` & `sastadev-0.0.4a1/sastadev/inflectioncorrection.tsv.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/lexicon.py` & `sastadev-0.0.4a1/sastadev/lexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/metadata.py` & `sastadev-0.0.4a1/sastadev/metadata.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/namepartlexicon.py` & `sastadev-0.0.4a1/sastadev/namepartlexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/names/nameparts/namepartlexicon.csv` & `sastadev-0.0.4a1/sastadev/names/nameparts/namepartlexicon.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/query.py` & `sastadev-0.0.4a1/sastadev/query.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/sastatoken.py` & `sastadev-0.0.4a1/sastadev/sastatoken.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/sastatypes.py` & `sastadev-0.0.4a1/sastadev/sastatypes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 '''
 This module contains definitions of types used in multiple modules
 '''
 
 from typing import Dict, List, Tuple, Callable, Optional, Union
+from typing_extensions import TypeAlias
 from lxml import etree  # type: ignore
 from collections import Counter
 from query import Query
 from sastatoken import Token
 
-AltId = int
-BackPlacement = int
-CapitalName = str
-CountryName = str
-ContinentName = str
-CELEXPosCode = str
-FirstName = str
-LocationName = str
-DCOIPt = str
-DeHet = str
-CELEX_INFL = str
-DCOITuple = Tuple
-Lemma = str
-CorrectionMode = str  # Literal['0','1','n']
-ErrorDict = Dict[str, List[List[str]]]
-Level = str  # in the future perhaps NewType('Level', str)
-Item = str  # in the future perhaps NewType('Item', str)
-Item_Level = Tuple[Item, Level]
-IntSpan = Tuple[int, int]
-AltCodeDict = Dict[Item_Level, Item_Level]
-QId = str  # in the futute perhaps NewType('QId', str)
-UttId = str  # in the future perhaps NewType('UttId', str)
-Position = int  # in the future perhapos NewType('Position', int)
-PositionStr = str
-Stage = int
-#SynTree = etree._Element  # type: ignore
-SynTree = etree.Element  # type: ignore
-GoldTuple = Tuple[str, str, Counter]
-Item2LevelsDict = Dict[Item, List[Level]]
-Match = Tuple[SynTree, SynTree]
-Matches = List[Match]
-MatchesDict = Dict[Tuple[QId, UttId], Matches]
-MetaElement = etree.Element
-ExactResult = Tuple[UttId, Position]
-ExactResults = List[ExactResult]
-ExactResultsDict = Dict[QId, ExactResults]  # qid
-Gender = str
-Penalty = int
-PhiTriple = Tuple[str, str, str]
-OptPhiTriple = Optional[PhiTriple]
-PositionMap = Dict[Position, Position]
-QueryDict = Dict[QId, Query]
-QIdCount = Dict[QId, int]
-MethodName = str  # perhaps in the future NewType('MethodName', str)
-FileName = str  # perhaps in the future NewType('FileName', str)
-ReplacementMode = int
-ResultsCounter = Counter  # Counter[UttId]  # Dict[UttId, int]
-ResultsDict = Dict[QId, ResultsCounter]
-Span = Tuple[PositionStr, PositionStr]
-Item_Level2QIdDict = Dict[Item_Level, QId]
-Nort = Union[SynTree, Token]
-ExactResultsFilter = Callable[[Query, ExactResultsDict, ExactResult], bool]
-Targets = int
-Treebank = etree.Element
-TreePredicate = Callable[[SynTree], bool]
-TokenTreePredicate = Callable[[Token, SynTree], bool]
-URL = str
-UttTokenDict = Dict[UttId, List[Token]]
-UttWordDict = Dict[UttId, List[str]]
-WordInfo = Tuple[Optional[CELEXPosCode], Optional[DeHet], Optional[CELEX_INFL], Optional[Lemma]]
+AltId: TypeAlias = int
+BackPlacement: TypeAlias = int
+CapitalName: TypeAlias = str
+CountryName: TypeAlias = str
+ContinentName: TypeAlias = str
+CELEXPosCode: TypeAlias = str
+FirstName: TypeAlias = str
+LocationName: TypeAlias = str
+DCOIPt: TypeAlias = str
+DeHet: TypeAlias = str
+CELEX_INFL: TypeAlias = str
+DCOITuple: TypeAlias = Tuple
+Lemma: TypeAlias = str
+CorrectionMode: TypeAlias = str  # Literal['0','1','n']
+ErrorDict: TypeAlias = Dict[str, List[List[str]]]
+Level: TypeAlias = str  # in the future perhaps NewType('Level', str)
+Item: TypeAlias = str  # in the future perhaps NewType('Item', str)
+Item_Level: TypeAlias = Tuple[Item, Level]
+IntSpan: TypeAlias = Tuple[int, int]
+AltCodeDict: TypeAlias = Dict[Item_Level, Item_Level]
+QId: TypeAlias = str  # in the futute perhaps NewType('QId', str)
+UttId: TypeAlias = str  # in the future perhaps NewType('UttId', str)
+Position: TypeAlias = int  # in the future perhapos NewType('Position', int)
+PositionStr: TypeAlias = str
+Stage: TypeAlias = int
+#SynTree: TypeAlias = etree._Element  # type: ignore
+SynTree: TypeAlias = etree.Element  # type: ignore
+GoldTuple: TypeAlias = Tuple[str, str, Counter]
+Item2LevelsDict: TypeAlias = Dict[Item, List[Level]]
+Match: TypeAlias = Tuple[SynTree, SynTree]
+Matches: TypeAlias = List[Match]
+MatchesDict: TypeAlias = Dict[Tuple[QId, UttId], Matches]
+MetaElement: TypeAlias = etree.Element
+ExactResult: TypeAlias = Tuple[UttId, Position]
+ExactResults: TypeAlias = List[ExactResult]
+ExactResultsDict: TypeAlias = Dict[QId, ExactResults]  # qid
+Gender: TypeAlias = str
+Penalty: TypeAlias = int
+PhiTriple: TypeAlias = Tuple[str, str, str]
+OptPhiTriple: TypeAlias = Optional[PhiTriple]
+PositionMap: TypeAlias = Dict[Position, Position]
+QueryDict: TypeAlias = Dict[QId, Query]
+QIdCount: TypeAlias = Dict[QId, int]
+MethodName: TypeAlias = str  # perhaps in the future NewType('MethodName', str)
+FileName: TypeAlias = str  # perhaps in the future NewType('FileName', str)
+ReplacementMode: TypeAlias = int
+ResultsCounter: TypeAlias = Counter  # Counter[UttId]  # Dict[UttId, int]
+ResultsDict: TypeAlias = Dict[QId, ResultsCounter]
+Span: TypeAlias = Tuple[PositionStr, PositionStr]
+Item_Level2QIdDict: TypeAlias = Dict[Item_Level, QId]
+Nort: TypeAlias = Union[SynTree, Token]
+ExactResultsFilter: TypeAlias = Callable[[Query, ExactResultsDict, ExactResult], bool]
+Targets: TypeAlias = int
+Treebank: TypeAlias = etree.Element
+TreePredicate: TypeAlias = Callable[[SynTree], bool]
+TokenTreePredicate: TypeAlias = Callable[[Token, SynTree], bool]
+URL: TypeAlias = str
+UttTokenDict: TypeAlias = Dict[UttId, List[Token]]
+UttWordDict: TypeAlias = Dict[UttId, List[str]]
+WordInfo: TypeAlias = Tuple[Optional[CELEXPosCode], Optional[DeHet], Optional[CELEX_INFL], Optional[Lemma]]
 # moved the following to allresuls.py
-#CoreQueryFunction = Callable[[SynTree], List[SynTree]]
-#PostQueryFunction = Callable[[SynTree, allresults.AllResults], List[SynTree]]
-#QueryFunction = Union[CoreQueryFunction, PostQueryFunction]
+#CoreQueryFunction: TypeAlias = Callable[[SynTree], List[SynTree]]
+#PostQueryFunction: TypeAlias = Callable[[SynTree, allresults.AllResults], List[SynTree]]
+#QueryFunction: TypeAlias = Union[CoreQueryFunction, PostQueryFunction]
```

### Comparing `sastadev-0.0.3/sastadev/sentence_parser.py` & `sastadev-0.0.4a1/sastadev/sentence_parser.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/stringfunctions.py` & `sastadev-0.0.4a1/sastadev/stringfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.3/sastadev/treebankfunctions.py` & `sastadev-0.0.4a1/sastadev/treebankfunctions.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 # import logging
 from copy import copy, deepcopy
 from lxml import etree
 from config import SDLOGGER
 from stringfunctions import allconsonants
 # from lexicon import informlexiconpos, isa_namepart_uc, informlexicon, isa_namepart
-import lexicon as lex
+#import lexicon as lex
 from config import PARSE_FUNC
 
 from sastatoken import Token
 from metadata import Meta
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from sastatypes import FileName, OptPhiTriple, PhiTriple, Position, PositionMap, PositionStr, Span, SynTree, UttId
@@ -587,23 +587,46 @@
             result1 = results[0]
             result = number2intstring(result1)
         else:
             result = None
     return result
 
 
+def getattval_fallback(node: SynTree, att: str, fallback: str = '') -> str:
+    """Gets the attribute from the current node or goes up in parents to find it
+
+    Args:
+        node (SynTree): node to search
+        att (str): attribute name
+        fallback (str): if nothing is found
+
+    Returns:
+        str: attribute value or fallback value if none is found
+    """
+    while True:
+        if not node:
+            return fallback
+        val = getattval(node, att)
+        if val:
+            return val
+        parent = node.getparent()
+        if not parent:
+            return fallback
+        node = parent
+
+
 def getnodeyield(syntree: SynTree) -> List[SynTree]:
     resultlist = []
     if syntree is None:
         return []
     else:
         for node in syntree.iter():
             if 'pt' in node.attrib or 'pos' in node.attrib:
                 resultlist.append(node)
-        sortedresultlist = sorted(resultlist, key=lambda x: int(getattval(x, 'end')))
+        sortedresultlist = sorted(resultlist, key=lambda x: int(getattval_fallback(x, 'end', '9999')))
         return sortedresultlist
 
 
 def getyield(syntree: SynTree) -> List[str]:  # deze herformuleren in termen van getnodeyield na testen
     resultlist = []
     if syntree is None:
         theyield = []
@@ -848,103 +871,14 @@
 
 
 def onbvnwdet(node: SynTree) -> bool:
     result = getattval(node, 'lemma') in potentialdet_onbvnws
     return result
 
 
-def asta_recognised_lexnode(node: SynTree) -> bool:
-    '''
-    The function *asta_recognised_lexnode* determines whether *node* should count as a
-    lexical verb in the ASTA method.
-
-    This is the case if *pt* equals *ww* and the node is not a substantivised verb as
-    determined by the function *issubstantivised_verb*:
-
-    .. autofunction:: treebankfunctions::issubstantivised_verb
-
-    '''
-    if issubstantivised_verb(node):
-        result = False
-    else:
-        result = getattval(node, 'pt') == 'ww'
-    return result
-
-
-def asta_recognised_nounnode(node: SynTree) -> bool:
-    '''
-    The function *asta_recognised_nounnode* determines whether *node* should count as a
-    noun in the ASTA method.
-
-    This is the case if
-
-    * either the node meets the conditions of *sasta_pseudonym*
-
-       .. autofunction:: treebankfunctions::sasta_pseudonym
-
-    * or the node meets the conditions of *spec_noun*
-
-       .. autofunction:: treebankfunctions::spec_noun
-
-    * or the node meets the conditions of *is_duplicate_spec_noun*
-
-       .. autofunction:: treebankfunctions::is_duplicate_spec_noun
-
-    * or the node meets the conditions of *sasta_long*
-
-       .. autofunction:: treebankfunctions::sasta_long
-
-    * or the node meets the conditions of *recognised_wordnodepos*
-
-       .. autofunction:: treebankfunctions::recognised_wordnodepos
-
-    * or the node meets the conditions of *recognised_lemmanodepos(node, pos)*
-
-       .. autofunction:: treebankfunctions::recognised_lemmanodepos(node, pos)
-
-    However, the node should:
-
-    * neither consist of lower case consonants only, as determined by *all_lower_consonantsnode*:
-
-       .. autofunction:: treebankfunctions::all_lower_consonantsnode
-
-    * nor satisfy the conditions of *short_nucl_n*:
-
-       .. autofunction:: treebankfunctions::short_nucl_n
-
-    '''
-
-    if issubstantivised_verb(node):
-        pos = 'ww'
-    else:
-        pos = 'n'
-    result = sasta_pseudonym(node)
-    result = result or spec_noun(node)
-    result = result or is_duplicate_spec_noun(node)
-    result = result or sasta_long(node)
-    result = result or recognised_wordnodepos(node, pos)
-    result = result or recognised_lemmanodepos(node, pos)
-    result = result and not (all_lower_consonantsnode(node))
-    result = result and not (short_nucl_n(node))
-    return result
-
-
-def asta_recognised_wordnode(node: SynTree) -> bool:
-    result = sasta_pseudonym(node)
-    result = result or spec_noun(node)
-    result = result or is_duplicate_spec_noun(node)
-    result = result or sasta_long(node)
-    result = result or recognised_wordnode(node)
-    result = result or recognised_lemmanode(node)
-    result = result or isnumber(node)
-    result = result and not (all_lower_consonantsnode(node))
-    result = result and not (short_nucl_n(node))
-    return result
-
-
 def isnumber(node: SynTree) -> bool:
     word = getattval(node, 'word')
     thematch = numberre.match(word)
     result = thematch is not None
     return result
 
 
@@ -1003,100 +937,14 @@
     '''
     word = getattval(node, 'word')
     match = pseudonymre.match(word)
     result = match is not None
     return result
 
 
-def recognised_wordnodepos(node: SynTree, pos: str) -> bool:
-    '''
-    The function *recognised_wordnodepos* determines for *node* whether it is a known
-    word of part of speech code *pos*.
-
-    It distinguishes several subcases that yield the result True:
-
-    * the value of the *word* attribute of *node* is a known word form (as determined by the function *lex.informlexiconpos*
-
-    * the lower-cased value of the *word* attribute of *node* is a known word form (as determined by the function *lex.informlexiconpos*
-
-    * the node is a node for a compound, as determined by the function *iscompound*:
-
-        .. autofunction:: treebankfunctions::iscompound
-           :noindex:
-
-    * the node is a node for a diminutive, as determined by the function *isdiminutive*:
-
-        .. autofunction:: treebankfunctions::isdiminutive
-           :noindex:
-
-    * the node is a node for a name part, as determined by the function *lex.isa_namepart*
-
-
-    '''
-    word = getattval(node, 'word')
-    lcword = word.lower()
-    result = lex.informlexiconpos(word, pos) or lex.informlexiconpos(lcword, pos) or \
-        iscompound(node) or isdiminutive(node) or lex.isa_namepart_uc(word)
-    return result
-
-
-def recognised_wordnode(node: SynTree) -> bool:
-    '''
-    The function *recognised_wordnode* determines for *node* whether it is a known word.
-
-    It distinguishes several subcases that yield the result True:
-
-    * the value of the *word* attribute of *node* is a known word form (as determined
-    by the function *lex.informlexicon*
-
-    * the lower-cased value of the *word* attribute of *node* is a known word form (as
-    determined by the function *lex.informlexicon
-
-    * the node is a node for a compound, as determined by the function *iscompound*:
-
-        .. autofunction:: treebankfunctions::iscompound
-
-    * the node is node for a diminutive, as determined by the function *isdiminutive*:
-
-        .. autofunction:: treebankfunctions::isdiminutive
-
-    * the node is a node for a name part, as determined by the function *lex.isa_namepart*
-
-
-    '''
-
-    word = getattval(node, 'word')
-    lcword = word.lower()
-    result = lex.informlexicon(word) or lex.informlexicon(lcword) or iscompound(node) or isdiminutive(
-        node) or lex.isa_namepart(word)
-    return result
-
-
-def recognised_lemmanode(node: SynTree) -> bool:
-    '''
-    The function *recognised_lemmanode* checks whether the *lemma* of *node* is in
-    the lexicon  (as determined by the function *lex.informlexicon*).
-
-    '''
-    lemma = getattval(node, 'lemma')
-    result = lex.informlexicon(lemma)
-    return result
-
-
-def recognised_lemmanodepos(node: SynTree, pos: str) -> bool:
-    '''
-    The function *recognised_lemmanodepos* checks whether the *lemma* of *node* is in
-    the lexicon with part of speech *pos* (as determined by * lex.informlexiconpos*).
-
-    '''
-    lemma = getattval(node, 'lemma')
-    result = lex.informlexiconpos(lemma, pos)
-    return result
-
-
 nodeformat = '{}/{}{}'
 nodeformatplus = nodeformat + '['
 
 ##@@need to add a variant that returns a string
 
 
 def simpleshow(stree: SynTree, showchildren: bool = True, newline: bool = True) -> None:
```

### Comparing `sastadev-0.0.3/sastadev.egg-info/PKG-INFO` & `sastadev-0.0.4a1/sastadev.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.0.3
+Version: 0.0.4a1
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Digital Humanities Lab, Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `sastadev-0.0.3/sastadev.egg-info/SOURCES.txt` & `sastadev-0.0.4a1/sastadev.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -19,11 +19,8 @@
 sastadev/sentence_parser.py
 sastadev/stringfunctions.py
 sastadev/treebankfunctions.py
 sastadev.egg-info/PKG-INFO
 sastadev.egg-info/SOURCES.txt
 sastadev.egg-info/dependency_links.txt
 sastadev.egg-info/top_level.txt
-sastadev/celexlexicon/dutch/DMLCD.txt
-sastadev/celexlexicon/dutch/DMWCDOK.txt
-sastadev/celexlexicon/dutch/DSLCD.txt
 sastadev/names/nameparts/namepartlexicon.csv
```

### Comparing `sastadev-0.0.3/setup.py` & `sastadev-0.0.4a1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name='sastadev',
     python_requires='>=3.7, <4',
-    version='0.0.3',
+    version='0.0.4a1',
     description='Linguistic functions for SASTA tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Digital Humanities Lab, Utrecht University',
     author_email='digitalhumanities@uu.nl',
     url='https://github.com/UUDigitalHumanitieslab/sastadev',
     license='BSD-3-Clause',
```

