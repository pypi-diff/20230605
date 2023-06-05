# Comparing `tmp/Mold2_pywrapper-0.0.3.post2.tar.gz` & `tmp/Mold2_pywrapper-0.0.3.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mold2_pywrapper-0.0.3.post2.tar", last modified: Mon Jun  5 08:54:41 2023, max compression
+gzip compressed data, was "Mold2_pywrapper-0.0.3.post3.tar", last modified: Mon Jun  5 09:20:43 2023, max compression
```

## Comparing `Mold2_pywrapper-0.0.3.post2.tar` & `Mold2_pywrapper-0.0.3.post3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 08:54:41.234106 Mold2_pywrapper-0.0.3.post2/
--rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post2/LICENSE
--rw-rw-rw-   0        0        0     4964 2023-06-05 08:54:41.234106 Mold2_pywrapper-0.0.3.post2/PKG-INFO
--rw-rw-rw-   0        0        0     4047 2023-02-07 12:55:23.000000 Mold2_pywrapper-0.0.3.post2/README.md
--rw-rw-rw-   0        0        0     1301 2023-06-05 08:54:41.237117 Mold2_pywrapper-0.0.3.post2/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:54:41.214081 Mold2_pywrapper-0.0.3.post2/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 08:54:41.221083 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper/
--rw-rw-rw-   0        0        0      127 2023-06-05 08:54:13.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper/__init__.py
--rw-rw-rw-   0        0        0    47176 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper/descriptors.json
--rw-rw-rw-   0        0        0    13943 2023-06-05 08:52:51.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper/mold2_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:54:41.233187 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     4964 2023-06-05 08:54:41.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-06-05 08:54:41.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 08:54:41.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-06-05 08:54:41.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 08:54:41.000000 Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 09:20:43.475376 Mold2_pywrapper-0.0.3.post3/
+-rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post3/LICENSE
+-rw-rw-rw-   0        0        0     4964 2023-06-05 09:20:43.475376 Mold2_pywrapper-0.0.3.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     4047 2023-02-07 12:55:23.000000 Mold2_pywrapper-0.0.3.post3/README.md
+-rw-rw-rw-   0        0        0     1301 2023-06-05 09:20:43.477365 Mold2_pywrapper-0.0.3.post3/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:20:43.451362 Mold2_pywrapper-0.0.3.post3/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 09:20:43.461360 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper/
+-rw-rw-rw-   0        0        0      127 2023-06-05 09:19:38.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    47122 2023-06-05 09:19:01.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper/descriptors.json
+-rw-rw-rw-   0        0        0    13943 2023-06-05 08:52:51.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper/mold2_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:20:43.474376 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     4964 2023-06-05 09:20:43.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2023-06-05 09:20:43.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 09:20:43.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-06-05 09:20:43.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 09:20:43.000000 Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/top_level.txt
```

### Comparing `Mold2_pywrapper-0.0.3.post2/LICENSE` & `Mold2_pywrapper-0.0.3.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post2/PKG-INFO` & `Mold2_pywrapper-0.0.3.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mold2_pywrapper
-Version: 0.0.3.post2
+Version: 0.0.3.post3
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `Mold2_pywrapper-0.0.3.post2/README.md` & `Mold2_pywrapper-0.0.3.post3/README.md`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post2/setup.cfg` & `Mold2_pywrapper-0.0.3.post3/setup.cfg`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper/descriptors.json` & `Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper/descriptors.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9292149292149292%*

 * *Differences: {"'D143'": "'sum of atomic Van Der Waals Carbon-scale'",*

 * * "'D144'": "'mean atomic van der Waals Carbon-scale'",*

 * * "'D145'": "'sum of atomic electronegativities Pauling-Scale on Carbon'",*

 * * "'D147'": "'sum of atomic electronegativities Sanderson-scaled on Carbon'",*

 * * "'D149'": "'sum of atomic electronegativities Allred-Rochow-scaled on Carbon'",*

 * * "'D150'": "'mean atomic electronegativity Allred-Rochow-scaled on Carbon'",*

 * * "'D158'": "'valence electrons of principal quantum index'",*

 * * "'D160'": "'Schultz type Mole […]*

```diff
@@ -137,32 +137,32 @@
     "D136": "Narumi-type topological index",
     "D137": "harmonic topological index",
     "D138": "geometric topological index",
     "D139": "topological distance count order-3",
     "D140": "log of vertex distance path count",
     "D141": "average of vertex distance path count",
     "D142": "Balaban type of mean square vertex distance index",
-    "D143": "sum of atomic Van Der Waals Carbon-Scele",
-    "D144": "mean atoic van der Waals Carbon-scale",
-    "D145": "sum of atomic electronegativites Pauling-Scale on Carbon",
+    "D143": "sum of atomic Van Der Waals Carbon-scale",
+    "D144": "mean atomic van der Waals Carbon-scale",
+    "D145": "sum of atomic electronegativities Pauling-Scale on Carbon",
     "D146": "mean atomic electronegativities Pauling-scaled on Carbon",
-    "D147": "sum of atomic electrongativities Sanderson-scaled on Carbon",
+    "D147": "sum of atomic electronegativities Sanderson-scaled on Carbon",
     "D148": "mean atomic electronegativity Sanderson-scaled on Carbon",
-    "D149": "sum of atomic electrongativities Allred-Rochow-scaled on Carbon",
-    "D150": "mean atomic electrongativity Allred-Rochow-scaled on Carbon",
+    "D149": "sum of atomic electronegativities Allred-Rochow-scaled on Carbon",
+    "D150": "mean atomic electronegativity Allred-Rochow-scaled on Carbon",
     "D151": "sum of atomic polarizabilities scaled on Carbon-SP3",
     "D152": "mean atomic polarizability scaled on Carbon-SP3",
     "D153": "Zagreb order-1 index",
     "D154": "Zagreb order-1 index with value of valence vertex degrees",
     "D155": "Zagreb order-2 index",
     "D156": "vertex degree topological index",
     "D157": "second Zagreb order-2 index with value of valence vertex degrees",
-    "D158": "valence electrions of principal quantum index",
+    "D158": "valence electrons of principal quantum index",
     "D159": "Schultz type Molecular Topological index",
-    "D160": "Schultz type Molecular Topolgical Index of valence vertex degrees",
+    "D160": "Schultz type Molecular Topological Index of valence vertex degrees",
     "D161": "molecular Topological Distance Index",
     "D162": "molecular Topological Distance Index of valence vertex degrees",
     "D163": "molecular size and branching index",
     "D164": "index of terminal vertex matrix",
     "D165": "Wiener index",
     "D166": "average Path length in Wiener Index",
     "D167": "reciprocal index of Wiener distance matrix",
@@ -170,36 +170,36 @@
     "D169": "index of Laplacian Matrix",
     "D170": "first No-Zero eigenvalue of Laplacian matrix",
     "D171": "Wiener\u2013Path index",
     "D172": "reciprocal Wiener-Path index",
     "D173": "Mohar order-2 index",
     "D174": "maximum Path Index",
     "D175": "Wiener Type Maximum Path Index",
-    "D176": "reciprocal Wiener Type Maximum Path Inde",
+    "D176": "reciprocal Wiener Type Maximum Path Index",
     "D177": "minimum-Path/Maximum-Path Index",
     "D178": "all-Path Wiener - sum of the edges in the shortest paths between all pairs of non-hydrogen atoms",
     "D179": "heteroatoms and Multiple bonds weighted Distance Matrix",
     "D180": "mass Weighted Distance Matrix",
     "D181": "index of Van Der Waals Weighted Distance Matrix",
     "D182": "distance Matrix of Electronegativity Weighted with Electronegativities Pauling-Scale",
     "D183": "distance Matrix of Electronegativity Weighted with Sanderson Electronegativities",
-    "D184": "distance Matrix of Electronegativity Weighted with Allred-Rochow Electronegativites",
+    "D184": "distance Matrix of Electronegativity Weighted with Allred-Rochow Electronegativities",
     "D185": "polarizability weighted distance matrix",
     "D186": "average vertex distance connectivity index",
     "D187": "Balaban heteroatoms bonds weighted index",
     "D188": "Balaban mass weighted index",
     "D189": "Balaban van der Waals weighted index",
     "D190": "Balaban electronegativity weighted with Pauling-Scale index",
     "D191": "Balaban electronegativity weighted with Sanderson-Scale index",
     "D192": "Balaban electronegativity weighted with Allred-Rochow-Scale index",
     "D193": "Balaban-type polarizability weighted index",
     "D194": "maximal valence vertex electrotopological negative variation",
     "D195": "maximal valence vertex electrotopological positive variation",
-    "D196": "sum absolute electrotopological negtive variation",
-    "D197": "electrotoplogical index",
+    "D196": "sum absolute electrotopological negative variation",
+    "D197": "electrotopological index",
     "D198": "sum electrotopological states index",
     "D199": "mean electrotopological states index",
     "D200": "vertex connectivity order-0 index",
     "D201": "vertex connectivity order-1 index",
     "D202": "vertex connectivity order-2 index",
     "D203": "vertex connectivity order-3 index",
     "D204": "vertex connectivity order-4 index",
@@ -246,15 +246,15 @@
     "D245": "shortest path centralization index",
     "D246": "maximum value of variation",
     "D247": "eXP2 of Path-distance / Walk-distance over all atoms",
     "D248": "eXP3 of Path-distance / Walk-distance over all atoms",
     "D249": "eXP4 of Path-distance / Walk-distance over all atoms",
     "D250": "eXP5 of Path-distance / Walk-distance over all atoms",
     "D251": "Petitjean index",
-    "D252": "sturcture centric index",
+    "D252": "structure centric index",
     "D253": "structure lopping centric group index",
     "D254": "radial centric index",
     "D255": "vertex distance count equality index",
     "D256": "vertex distance count magnitude index",
     "D257": "total vertex distance count equality index",
     "D258": "total vertex distance count magnitude index",
     "D259": "mean of distance degree equality index",
@@ -457,22 +457,22 @@
     "D456": "Geary topological structure autocorrelation length-2 weighted by atomic van der Waals volumes",
     "D457": "Geary topological structure autocorrelation length-3 weighted by atomic van der Waals volumes",
     "D458": "Geary topological structure autocorrelation length-4 weighted by atomic van der Waals volumes",
     "D459": "Geary topological structure autocorrelation length-5 weighted by atomic van der Waals volumes",
     "D460": "Geary topological structure autocorrelation length-6 weighted by atomic van der Waals volumes",
     "D461": "Geary topological structure autocorrelation length-7 weighted by atomic van der Waals volumes",
     "D462": "Geary topological structure autocorrelation length-8 weighted by atomic van der Waals volumes",
-    "D463": "eary topological structure autocorrelation length-1 weighted by atomic Sandersonelectronegativities",
-    "D464": "eary topological structure autocorrelation length-2 weighted by atomic Sandersonelectronegativities",
-    "D465": "eary topological structure autocorrelation length-3 weighted by atomic Sandersonelectronegativities",
-    "D466": "eary topological structure autocorrelation length-4 weighted by atomic Sandersonelectronegativities",
-    "D467": "eary topological structure autocorrelation length-5 weighted by atomic Sandersonelectronegativities",
-    "D468": "eary topological structure autocorrelation length-6 weighted by atomic Sandersonelectronegativities",
-    "D469": "eary topological structure autocorrelation length-7 weighted by atomic Sandersonelectronegativities",
-    "D470": "eary topological structure autocorrelation length-8 weighted by atomic Sandersonelectronegativities",
+    "D463": "Geary topological structure autocorrelation length-1 weighted by atomic Sanderson electronegativities",
+    "D464": "Geary topological structure autocorrelation length-2 weighted by atomic Sanderson electronegativities",
+    "D465": "Geary topological structure autocorrelation length-3 weighted by atomic Sanderson electronegativities",
+    "D466": "Geary topological structure autocorrelation length-4 weighted by atomic Sanderson electronegativities",
+    "D467": "Geary topological structure autocorrelation length-5 weighted by atomic Sanderson electronegativities",
+    "D468": "Geary topological structure autocorrelation length-6 weighted by atomic Sanderson electronegativities",
+    "D469": "Geary topological structure autocorrelation length-7 weighted by atomic Sanderson electronegativities",
+    "D470": "Geary topological structure autocorrelation length-8 weighted by atomic Sanderson electronegativities",
     "D471": "Geary topological structure autocorrelation length-1 weighted by atomic polarizabilities",
     "D472": "Geary topological structure autocorrelation length-2 weighted by atomic polarizabilities",
     "D473": "Geary topological structure autocorrelation length-3 weighted by atomic polarizabilities",
     "D474": "Geary topological structure autocorrelation length-4 weighted by atomic polarizabilities",
     "D475": "Geary topological structure autocorrelation length-5 weighted by atomic polarizabilities",
     "D476": "Geary topological structure autocorrelation length-6 weighted by atomic polarizabilities",
     "D477": "Geary topological structure autocorrelation length-7 weighted by atomic polarizabilities",
@@ -489,22 +489,22 @@
     "D488": "Moran topological structure autocorrelation length-2 weighted by atomic van der Waals volumes",
     "D489": "Moran topological structure autocorrelation length-3 weighted by atomic van der Waals volumes",
     "D490": "Moran topological structure autocorrelation length-4 weighted by atomic van der Waals volumes",
     "D491": "Moran topological structure autocorrelation length-5 weighted by atomic van der Waals volumes",
     "D492": "Moran topological structure autocorrelation length-6 weighted by atomic van der Waals volumes",
     "D493": "Moran topological structure autocorrelation length-7 weighted by atomic van der Waals volumes",
     "D494": "Moran topological structure autocorrelation length-8 weighted by atomic van der Waals volumes",
-    "D495": "oran topological structure autocorrelation length-1 weighted by atomic Sandersonelectronegativities",
-    "D496": "oran topological structure autocorrelation length-2 weighted by atomic Sandersonelectronegativities",
-    "D497": "oran topological structure autocorrelation length-3 weighted by atomic Sandersonelectronegativities",
-    "D498": "oran topological structure autocorrelation length-4 weighted by atomic Sandersonelectronegativities",
-    "D499": "oran topological structure autocorrelation length-5 weighted by atomic Sandersonelectronegativities",
-    "D500": "oran topological structure autocorrelation length-6 weighted by atomic Sandersonelectronegativities",
-    "D501": "oran topological structure autocorrelation length-7 weighted by atomic Sandersonelectronegativities",
-    "D502": "oran topological structure autocorrelation length-8 weighted by atomic Sandersonelectronegativities",
+    "D495": "Moran topological structure autocorrelation length-1 weighted by atomic Sanderson electronegativities",
+    "D496": "Moran topological structure autocorrelation length-2 weighted by atomic Sanderson electronegativities",
+    "D497": "Moran topological structure autocorrelation length-3 weighted by atomic Sanderson electronegativities",
+    "D498": "Moran topological structure autocorrelation length-4 weighted by atomic Sanderson electronegativities",
+    "D499": "Moran topological structure autocorrelation length-5 weighted by atomic Sanderson electronegativities",
+    "D500": "Moran topological structure autocorrelation length-6 weighted by atomic Sanderson electronegativities",
+    "D501": "Moran topological structure autocorrelation length-7 weighted by atomic Sanderson electronegativities",
+    "D502": "Moran topological structure autocorrelation length-8 weighted by atomic Sanderson electronegativities",
     "D503": "Moran topological structure autocorrelation length-1 weighted by atomic polarizabilities",
     "D504": "Moran topological structure autocorrelation length-2 weighted by atomic polarizabilities",
     "D505": "Moran topological structure autocorrelation length-3 weighted by atomic polarizabilities",
     "D506": "Moran topological structure autocorrelation length-4 weighted by atomic polarizabilities",
     "D507": "Moran topological structure autocorrelation length-5 weighted by atomic polarizabilities",
     "D508": "Moran topological structure autocorrelation length-6 weighted by atomic polarizabilities",
     "D509": "Moran topological structure autocorrelation length-7 weighted by atomic polarizabilities",
@@ -526,78 +526,78 @@
     "D525": "mean molecular topological order-5 charge index",
     "D526": "mean molecular topological order-6 charge index",
     "D527": "mean molecular topological order-7 charge index",
     "D528": "mean molecular topological order-8 charge index",
     "D529": "mean molecular topological order-9 charge index",
     "D530": "mean molecular topological order-10 charge index",
     "D531": "sum of molecular topological mean charge index",
-    "D532": "lowest eigenvalue from Burdex matrix weighteed by masses order-1",
-    "D533": "lowest eigenvalue from Burdex matrix weighteed by masses order-2",
-    "D534": "lowest eigenvalue from Burdex matrix weighteed by masses order-3",
-    "D535": "lowest eigenvalue from Burdex matrix weighteed by masses order-4",
-    "D536": "lowest eigenvalue from Burdex matrix weighteed by masses order-5",
-    "D537": "lowest eigenvalue from Burdex matrix weighteed by masses order-6",
-    "D538": "lowest eigenvalue from Burdex matrix weighteed by masses order-7",
-    "D539": "lowest eigenvalue from Burdex matrix weighteed by masses order-8",
-    "D540": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-1",
-    "D541": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-2",
-    "D542": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-3",
-    "D543": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-4",
-    "D544": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-5",
-    "D545": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-6",
-    "D546": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-7",
-    "D547": "lowest eigenvalue from Burdex matrix weighteed by van der Walls order-8",
-    "D548": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-1",
-    "D549": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-2",
-    "D550": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-3",
-    "D551": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-4",
-    "D552": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-5",
-    "D553": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-6",
-    "D554": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-7",
-    "D555": "lowest eigenvalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-8",
-    "D556": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-1",
-    "D557": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-2",
-    "D558": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-3",
-    "D559": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-4",
-    "D560": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-5",
-    "D561": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-6",
-    "D562": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-7",
-    "D563": "lowest eigenvalue from Burdex matrix weighteed by polarizabilities order-8",
-    "D564": "hightest eignevalue from Burdex matrix weighteed by masses order-1",
-    "D565": "hightest eignevalue from Burdex matrix weighteed by masses order-2",
-    "D566": "hightest eignevalue from Burdex matrix weighteed by masses order-3",
-    "D567": "hightest eignevalue from Burdex matrix weighteed by masses order-4",
-    "D568": "hightest eignevalue from Burdex matrix weighteed by masses order-5",
-    "D569": "hightest eignevalue from Burdex matrix weighteed by masses order-6",
-    "D570": "hightest eignevalue from Burdex matrix weighteed by masses order-7",
-    "D571": "hightest eignevalue from Burdex matrix weighteed by masses order-8",
-    "D572": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-1",
-    "D573": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-2",
-    "D574": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-3",
-    "D575": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-4",
-    "D576": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-5",
-    "D577": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-6",
-    "D578": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-7",
-    "D579": "hightest eignevalue from Burdex matrix weighteed by van der Walls order-8",
-    "D580": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-1",
-    "D581": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-2",
-    "D582": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-3",
-    "D583": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-4",
-    "D584": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-5",
-    "D585": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-6",
-    "D586": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-7",
-    "D587": "hightest eignevalue from Burdex matrix weighteed by electronegativities Sanderson-Scale order-8",
-    "D588": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-1",
-    "D589": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-2",
-    "D590": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-3",
-    "D591": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-4",
-    "D592": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-5",
-    "D593": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-6",
-    "D594": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-7",
-    "D595": "hightest eignevalue from Burdex matrix weighteed by polarizabilities order-8",
+    "D532": "lowest eigenvalue from Burden matrix weighted by masses order-1",
+    "D533": "lowest eigenvalue from Burden matrix weighted by masses order-2",
+    "D534": "lowest eigenvalue from Burden matrix weighted by masses order-3",
+    "D535": "lowest eigenvalue from Burden matrix weighted by masses order-4",
+    "D536": "lowest eigenvalue from Burden matrix weighted by masses order-5",
+    "D537": "lowest eigenvalue from Burden matrix weighted by masses order-6",
+    "D538": "lowest eigenvalue from Burden matrix weighted by masses order-7",
+    "D539": "lowest eigenvalue from Burden matrix weighted by masses order-8",
+    "D540": "lowest eigenvalue from Burden matrix weighted by van der Walls order-1",
+    "D541": "lowest eigenvalue from Burden matrix weighted by van der Walls order-2",
+    "D542": "lowest eigenvalue from Burden matrix weighted by van der Walls order-3",
+    "D543": "lowest eigenvalue from Burden matrix weighted by van der Walls order-4",
+    "D544": "lowest eigenvalue from Burden matrix weighted by van der Walls order-5",
+    "D545": "lowest eigenvalue from Burden matrix weighted by van der Walls order-6",
+    "D546": "lowest eigenvalue from Burden matrix weighted by van der Walls order-7",
+    "D547": "lowest eigenvalue from Burden matrix weighted by van der Walls order-8",
+    "D548": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-1",
+    "D549": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-2",
+    "D550": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-3",
+    "D551": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-4",
+    "D552": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-5",
+    "D553": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-6",
+    "D554": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-7",
+    "D555": "lowest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-8",
+    "D556": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-1",
+    "D557": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-2",
+    "D558": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-3",
+    "D559": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-4",
+    "D560": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-5",
+    "D561": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-6",
+    "D562": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-7",
+    "D563": "lowest eigenvalue from Burden matrix weighted by polarizabilities order-8",
+    "D564": "highest eigenvalue from Burden matrix weighted by masses order-1",
+    "D565": "highest eigenvalue from Burden matrix weighted by masses order-2",
+    "D566": "highest eigenvalue from Burden matrix weighted by masses order-3",
+    "D567": "highest eigenvalue from Burden matrix weighted by masses order-4",
+    "D568": "highest eigenvalue from Burden matrix weighted by masses order-5",
+    "D569": "highest eigenvalue from Burden matrix weighted by masses order-6",
+    "D570": "highest eigenvalue from Burden matrix weighted by masses order-7",
+    "D571": "highest eigenvalue from Burden matrix weighted by masses order-8",
+    "D572": "highest eigenvalue from Burden matrix weighted by van der Walls order-1",
+    "D573": "highest eigenvalue from Burden matrix weighted by van der Walls order-2",
+    "D574": "highest eigenvalue from Burden matrix weighted by van der Walls order-3",
+    "D575": "highest eigenvalue from Burden matrix weighted by van der Walls order-4",
+    "D576": "highest eigenvalue from Burden matrix weighted by van der Walls order-5",
+    "D577": "highest eigenvalue from Burden matrix weighted by van der Walls order-6",
+    "D578": "highest eigenvalue from Burden matrix weighted by van der Walls order-7",
+    "D579": "highest eigenvalue from Burden matrix weighted by van der Walls order-8",
+    "D580": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-1",
+    "D581": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-2",
+    "D582": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-3",
+    "D583": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-4",
+    "D584": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-5",
+    "D585": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-6",
+    "D586": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-7",
+    "D587": "highest eigenvalue from Burden matrix weighted by electronegativities Sanderson-Scale order-8",
+    "D588": "highest eigenvalue from Burden matrix weighted by polarizabilities order-1",
+    "D589": "highest eigenvalue from Burden matrix weighted by polarizabilities order-2",
+    "D590": "highest eigenvalue from Burden matrix weighted by polarizabilities order-3",
+    "D591": "highest eigenvalue from Burden matrix weighted by polarizabilities order-4",
+    "D592": "highest eigenvalue from Burden matrix weighted by polarizabilities order-5",
+    "D593": "highest eigenvalue from Burden matrix weighted by polarizabilities order-6",
+    "D594": "highest eigenvalue from Burden matrix weighted by polarizabilities order-7",
+    "D595": "highest eigenvalue from Burden matrix weighted by polarizabilities order-8",
     "D596": "number of total primary C-sp3",
     "D597": "number of total secondary C-sp3",
     "D598": "number of total tertiary C-sp3",
     "D599": "number of total quaternary C-sp3",
     "D600": "number of ring secondary C-sp3",
     "D601": "number of ring tertiary C-sp3",
     "D602": "number of ring quaternary C-sp3",
@@ -605,22 +605,22 @@
     "D604": "number of substituted aromatic C-sp2",
     "D605": "number of primary C-sp2",
     "D606": "number of secondary C-sp2",
     "D607": "number of tertiary C-sp2",
     "D608": "number of group allenes",
     "D609": "number of terminal C-sp",
     "D610": "number of non-terminal C-sp",
-    "D611": "number of group cianates (aliphatic)",
-    "D612": "number of group cianates (aromatic)",
-    "D613": "number of group isocianates (aliphatic)",
-    "D614": "number of group isocianates (aromatic)",
-    "D615": "number of group thiocianates (aliphatic)",
-    "D616": "number of group thiocianates (aromatic)",
-    "D617": "number of group isothiocianates (aliphatic)",
-    "D618": "number of group isothiocianates (aromatic)",
+    "D611": "number of group cyanates (aliphatic)",
+    "D612": "number of group cyanates (aromatic)",
+    "D613": "number of group isocyanates (aliphatic)",
+    "D614": "number of group isocyanates (aromatic)",
+    "D615": "number of group thiocyanates (aliphatic)",
+    "D616": "number of group thiocyanates (aromatic)",
+    "D617": "number of group isothiocyanates (aliphatic)",
+    "D618": "number of group isothiocyanates (aromatic)",
     "D619": "number of group carboxylic acids (aliphatic)",
     "D620": "number of group carboxylic acids (aromatic)",
     "D621": "number of group esters (aliphatic)",
     "D622": "number of group esters (aromatic)",
     "D623": "number of group primary amides (aliphatic)",
     "D624": "number of group primary amides (aromatic)",
     "D625": "number of group secondary amides (aliphatic)",
@@ -629,16 +629,16 @@
     "D628": "number of group tertiary amides (aromatic)",
     "D629": "number of group carbamates (aliphatic)",
     "D630": "number of group carbamates (aromatic)",
     "D631": "number of group acyl halogenides (aliphatic)",
     "D632": "number of group acyl halogenides (aromatic)",
     "D633": "number of group thioacids (aliphatic)",
     "D634": "number of group thioacids (aromatic)",
-    "D635": "number of group ditioacids (aliphatic)",
-    "D636": "number of group ditioacids (aromatic)",
+    "D635": "number of group dithioacids (aliphatic)",
+    "D636": "number of group dithioacids (aromatic)",
     "D637": "number of group thioesters (aliphatic)",
     "D638": "number of group thioesters (aromatic)",
     "D639": "number of group dithioesters (aliphatic)",
     "D640": "number of group dithioesters (aromatic)",
     "D641": "number of group aldehydes (aliphatic)",
     "D642": "number of group aldehydes (aromatic)",
     "D643": "number of group ketones (aliphatic)",
@@ -648,15 +648,15 @@
     "D647": "number of group primary amines (aliphatic)",
     "D648": "number of group primary amines (aromatic)",
     "D649": "number of group secondary amines (aliphatic)",
     "D650": "number of group secondary amines (aromatic)",
     "D651": "number of group tertiary amines (aliphatic)",
     "D652": "number of group tertiary amines (aromatic)",
     "D653": "number of group N-hydrazines (aliphatic)",
-    "D654": "number of group N-hydrazines (aromatic)",
+    "D654": "number of group N-hydrazine (aromatic)",
     "D655": "number of group N-azo (aliphatic)",
     "D656": "number of group N-azo (aromatic)",
     "D657": "number of group nitriles (aliphatic)",
     "D658": "number of group nitriles (aromatic)",
     "D659": "number of group immines (aliphatic)",
     "D660": "number of group immines (aromatic)",
     "D661": "number of group ammonium groups (aliphatic)",
@@ -671,35 +671,35 @@
     "D670": "number of group nitroso (aromatic)",
     "D671": "number of group nitro (aliphatic)",
     "D672": "number of group nitro (aromatic)",
     "D673": "number of group imides",
     "D674": "number of group total hydroxyl groups",
     "D675": "number of group phenols",
     "D676": "number of group primary alcohols (aliphatic)",
-    "D677": "number of group secondary alcohols (alinhatic)",
+    "D677": "number of group secondary alcohols (aliphatic)",
     "D678": "number of group tertiary alcohols (aliphatic)",
     "D679": "number of group ethers (aliphatic)",
     "D680": "number of group ethers (aromatic)",
     "D681": "number of group hypohalogenydes (aliphatic)",
     "D682": "number of group hypohalogenydes (aromatic)",
     "D683": "number of group water molecules",
     "D684": "number of group sulfoxides",
     "D685": "number of group sulfones",
     "D686": "number of group sulfates",
-    "D687": "number of group thioles",
+    "D687": "number of group thiols",
     "D688": "number of group thioketones",
-    "D689": "number of group solfures",
-    "D690": "number of group disolfures",
+    "D689": "number of group sulfurs",
+    "D690": "number of group disulfurs",
     "D691": "number of group sulfonic acids",
     "D692": "number of group sulfonamides",
     "D693": "number of group phosphites",
     "D694": "number of group phosphates",
     "D695": "number of group phosphothionates",
     "D696": "number of group phosphodithionates",
-    "D697": "number of group phosphothioates",
+    "D697": "number of group phosphorothioates",
     "D698": "number of group CH2X",
     "D699": "number of group CR2HX",
     "D700": "number of group CR3X",
     "D701": "number of group R=CHX",
     "D702": "number of group R=CRX",
     "D703": "number of group R#CX",
     "D704": "number of group CHRX2",
@@ -770,10 +770,10 @@
     "D770": "number of group R2S or RS-SR",
     "D771": "number of group R=S",
     "D772": "number of group R-SO-R",
     "D773": "number of group R-SO2-R",
     "D774": "unsaturation index weighted by conventional bonds order",
     "D775": "hydrophilic factor index",
     "D776": "aromatic bonds ratio",
-    "D777": "molecular regresson confficients surface LogP index",
+    "D777": "molecular regression coefficients surface LogP index",
     "F766": "number of group Ar-NO2 or RO-NO2"
 }
```

### Comparing `Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper/mold2_wrapper.py` & `Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper/mold2_wrapper.py`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/PKG-INFO` & `Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mold2-pywrapper
-Version: 0.0.3.post2
+Version: 0.0.3.post3
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `Mold2_pywrapper-0.0.3.post2/src/Mold2_pywrapper.egg-info/SOURCES.txt` & `Mold2_pywrapper-0.0.3.post3/src/Mold2_pywrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

