# Comparing `tmp/generaltool-0.1.1.tar.gz` & `tmp/generaltool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generaltool-0.1.1.tar", last modified: Fri Jun  2 21:27:37 2023, max compression
+gzip compressed data, was "generaltool-0.1.2.tar", last modified: Mon Jun  5 09:31:08 2023, max compression
```

## Comparing `generaltool-0.1.1.tar` & `generaltool-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:37.864517 generaltool-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 21:27:06.000000 generaltool-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 21:27:06.000000 generaltool-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-02 21:27:37.864517 generaltool-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-02 21:27:07.000000 generaltool-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:37.864517 generaltool-0.1.1/generaltool/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 21:25:01.000000 generaltool-0.1.1/generaltool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-02 21:25:01.000000 generaltool-0.1.1/generaltool/enforce_literal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:37.864517 generaltool-0.1.1/generaltool/test/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 21:25:01.000000 generaltool-0.1.1/generaltool/test/test_generaltool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-02 21:25:01.000000 generaltool-0.1.1/generaltool/test/test_literal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:37.864517 generaltool-0.1.1/generaltool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-02 21:27:37.000000 generaltool-0.1.1/generaltool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 21:27:37.000000 generaltool-0.1.1/generaltool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:27:37.000000 generaltool-0.1.1/generaltool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 21:27:37.000000 generaltool-0.1.1/generaltool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-02 21:27:06.000000 generaltool-0.1.1/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:27:37.864517 generaltool-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-02 21:27:07.000000 generaltool-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:08.008459 generaltool-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 09:30:32.000000 generaltool-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 09:30:32.000000 generaltool-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-05 09:31:08.008459 generaltool-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-05 09:30:33.000000 generaltool-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:08.008459 generaltool-0.1.2/generaltool/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 09:27:47.000000 generaltool-0.1.2/generaltool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-05 09:27:47.000000 generaltool-0.1.2/generaltool/enforce_literal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:08.008459 generaltool-0.1.2/generaltool/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 09:27:47.000000 generaltool-0.1.2/generaltool/test/test_generaltool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-05 09:27:47.000000 generaltool-0.1.2/generaltool/test/test_literal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:08.008459 generaltool-0.1.2/generaltool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-05 09:31:07.000000 generaltool-0.1.2/generaltool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-05 09:31:07.000000 generaltool-0.1.2/generaltool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:31:07.000000 generaltool-0.1.2/generaltool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 09:31:07.000000 generaltool-0.1.2/generaltool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-05 09:30:32.000000 generaltool-0.1.2/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:31:08.008459 generaltool-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-05 09:30:33.000000 generaltool-0.1.2/setup.py
```

### Comparing `generaltool-0.1.1/LICENSE` & `generaltool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `generaltool-0.1.1/PKG-INFO` & `generaltool-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generaltool
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library code with no dependencies.
 Home-page: https://github.com/ManderaGeneral/generaltool
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,21 +36,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 1 fill:#482
@@ -68,15 +68,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.1](https://pypi.org/project/generaltool/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 99.1 %  |
+| [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.2](https://pypi.org/project/generaltool/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 99.1 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
@@ -92,11 +92,11 @@
 
 Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generaltool/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generaltool/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: generaltool Version: 0.1.1 Summary: Library code
+Metadata-Version: 2.1 Name: generaltool Version: 0.1.2 Summary: Library code
 with no dependencies. Home-page: https://github.com/ManderaGeneral/generaltool
 Author: Rickard "Mandera" Abraham Author-email: rickard.abraham@gmail.com
 License: mit Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
@@ -14,17 +14,17 @@
 ââ Dependency_Diagram_for_ManderaGeneral
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
-[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
-([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
+```mermaid flowchart LR 2([library]) --> 4([vector]) 1([tool]) --> 2([library])
+3([file]) --> 5([packager]) 2([library]) --> 3([file]) 0([import]) --> 2(
+[library]) 0([import]) --> 3([file]) 2([library]) --> 5([packager]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 1 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generaltool` | |:------------------|:----------------| | *No
@@ -32,20 +32,20 @@
 ***** Information *****
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -----------------------------------------------|:------------------------------
 -----------------|:----------------------|:------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------|:----------------|:------
---| | [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.1]
-(https://pypi.org/project/generaltool/) | 2023-06-02 23:27 CEST | [3.8](https:/
+--| | [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.2]
+(https://pypi.org/project/generaltool/) | 2023-06-05 11:30 CEST | [3.8](https:/
 /www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/
 downloads/release/python-390/), [3.10](https://www.python.org/downloads/
 release/python-3100/), [3.11](https://www.python.org/downloads/release/python-
 3110/) | Windows, Ubuntu | 99.1 % |
 ***** Attributes *****
 Module:_generaltool
 ââ Function:_enforce_literals
 
 ***** Contributions *****
 Issue-creation, discussions and pull requests are most welcome!  Generated
-2023-06-02 23:27 CEST for commit master.
+2023-06-05 11:30 CEST for commit master.
```

### Comparing `generaltool-0.1.1/README.md` & `generaltool-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 1 fill:#482
@@ -50,15 +50,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.1](https://pypi.org/project/generaltool/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 99.1 %  |
+| [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.2](https://pypi.org/project/generaltool/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 99.1 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
@@ -74,11 +74,11 @@
 
 Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generaltool/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generaltool/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 ââ Dependency_Diagram_for_ManderaGeneral
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
-[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
-([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
+```mermaid flowchart LR 2([library]) --> 4([vector]) 1([tool]) --> 2([library])
+3([file]) --> 5([packager]) 2([library]) --> 3([file]) 0([import]) --> 2(
+[library]) 0([import]) --> 3([file]) 2([library]) --> 5([packager]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 1 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generaltool` | |:------------------|:----------------| | *No
@@ -23,20 +23,20 @@
 ***** Information *****
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -----------------------------------------------|:------------------------------
 -----------------|:----------------------|:------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------|:----------------|:------
---| | [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.1]
-(https://pypi.org/project/generaltool/) | 2023-06-02 23:27 CEST | [3.8](https:/
+--| | [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.2]
+(https://pypi.org/project/generaltool/) | 2023-06-05 11:30 CEST | [3.8](https:/
 /www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/
 downloads/release/python-390/), [3.10](https://www.python.org/downloads/
 release/python-3100/), [3.11](https://www.python.org/downloads/release/python-
 3110/) | Windows, Ubuntu | 99.1 % |
 ***** Attributes *****
 Module:_generaltool
 ââ Function:_enforce_literals
 
 ***** Contributions *****
 Issue-creation, discussions and pull requests are most welcome!  Generated
-2023-06-02 23:27 CEST for commit master.
+2023-06-05 11:30 CEST for commit master.
```

### Comparing `generaltool-0.1.1/generaltool/enforce_literal.py` & `generaltool-0.1.2/generaltool/enforce_literal.py`

 * *Files identical despite different names*

### Comparing `generaltool-0.1.1/generaltool/test/test_literal.py` & `generaltool-0.1.2/generaltool/test/test_literal.py`

 * *Files identical despite different names*

### Comparing `generaltool-0.1.1/generaltool.egg-info/PKG-INFO` & `generaltool-0.1.2/generaltool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generaltool
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library code with no dependencies.
 Home-page: https://github.com/ManderaGeneral/generaltool
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,21 +36,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 1 fill:#482
@@ -68,15 +68,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                      | Ver                                            | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:-------------------------------------------------------------|:-----------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.1](https://pypi.org/project/generaltool/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 99.1 %  |
+| [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.2](https://pypi.org/project/generaltool/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 99.1 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
@@ -92,11 +92,11 @@
 
 Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generaltool/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generaltool/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: generaltool Version: 0.1.1 Summary: Library code
+Metadata-Version: 2.1 Name: generaltool Version: 0.1.2 Summary: Library code
 with no dependencies. Home-page: https://github.com/ManderaGeneral/generaltool
 Author: Rickard "Mandera" Abraham Author-email: rickard.abraham@gmail.com
 License: mit Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
@@ -14,17 +14,17 @@
 ââ Dependency_Diagram_for_ManderaGeneral
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
-[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
-([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
+```mermaid flowchart LR 2([library]) --> 4([vector]) 1([tool]) --> 2([library])
+3([file]) --> 5([packager]) 2([library]) --> 3([file]) 0([import]) --> 2(
+[library]) 0([import]) --> 3([file]) 2([library]) --> 5([packager]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 1 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generaltool` | |:------------------|:----------------| | *No
@@ -32,20 +32,20 @@
 ***** Information *****
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -----------------------------------------------|:------------------------------
 -----------------|:----------------------|:------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------|:----------------|:------
---| | [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.1]
-(https://pypi.org/project/generaltool/) | 2023-06-02 23:27 CEST | [3.8](https:/
+--| | [generaltool](https://github.com/ManderaGeneral/generaltool) | [0.1.2]
+(https://pypi.org/project/generaltool/) | 2023-06-05 11:30 CEST | [3.8](https:/
 /www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/
 downloads/release/python-390/), [3.10](https://www.python.org/downloads/
 release/python-3100/), [3.11](https://www.python.org/downloads/release/python-
 3110/) | Windows, Ubuntu | 99.1 % |
 ***** Attributes *****
 Module:_generaltool
 ââ Function:_enforce_literals
 
 ***** Contributions *****
 Issue-creation, discussions and pull requests are most welcome!  Generated
-2023-06-02 23:27 CEST for commit master.
+2023-06-05 11:30 CEST for commit master.
```

### Comparing `generaltool-0.1.1/setup.py` & `generaltool-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 except FileNotFoundError:
     long_description = 'Readme missing'
 
 setup(
     name="generaltool",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="0.1.1",
+    version="0.1.2",
     description="Library code with no dependencies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/ManderaGeneral/generaltool",
     license="mit",
     packages=find_namespace_packages(exclude=("build*", "dist*")),
```

