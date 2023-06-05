# Comparing `tmp/nemo_library-1.0.7.tar.gz` & `tmp/nemo_library-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_library-1.0.7.tar", last modified: Mon Jun  5 20:58:58 2023, max compression
+gzip compressed data, was "nemo_library-1.0.8.tar", last modified: Mon Jun  5 21:33:22 2023, max compression
```

## Comparing `nemo_library-1.0.7.tar` & `nemo_library-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 20:58:58.109400 nemo_library-1.0.7/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-05 20:58:58.109049 nemo_library-1.0.7/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)     1887 2023-06-03 19:14:26.000000 nemo_library-1.0.7/README.md
--rw-r--r--   0 schuglocal   (503) staff       (20)     1971 2023-06-05 20:58:57.000000 nemo_library-1.0.7/README.rst
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 20:58:58.105550 nemo_library-1.0.7/nemo_library/
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.7/nemo_library/__init__.py
--rw-r--r--   0 schuglocal   (503) staff       (20)    11883 2023-06-05 20:58:00.000000 nemo_library-1.0.7/nemo_library/nemo_library.py
--rw-r--r--   0 schuglocal   (503) staff       (20)      680 2023-06-05 20:55:34.000000 nemo_library-1.0.7/nemo_library/symbols.py
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 20:58:58.108231 nemo_library-1.0.7/nemo_library.egg-info/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/SOURCES.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/dependency_links.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/requires.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/top_level.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-05 20:58:58.109463 nemo_library-1.0.7/setup.cfg
--rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-05 20:52:25.000000 nemo_library-1.0.7/setup.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 21:33:22.879614 nemo_library-1.0.8/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2871 2023-06-05 21:33:22.879381 nemo_library-1.0.8/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2361 2023-06-05 21:33:06.000000 nemo_library-1.0.8/README.md
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2577 2023-06-05 21:33:22.000000 nemo_library-1.0.8/README.rst
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 21:33:22.877235 nemo_library-1.0.8/nemo_library/
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.8/nemo_library/__init__.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)    11883 2023-06-05 20:58:00.000000 nemo_library-1.0.8/nemo_library/nemo_library.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)      680 2023-06-05 20:55:34.000000 nemo_library-1.0.8/nemo_library/symbols.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 21:33:22.879020 nemo_library-1.0.8/nemo_library.egg-info/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2871 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/SOURCES.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/dependency_links.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/requires.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/top_level.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-05 21:33:22.879679 nemo_library-1.0.8/setup.cfg
+-rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-05 21:33:14.000000 nemo_library-1.0.8/setup.py
```

### Comparing `nemo_library-1.0.7/PKG-INFO` & `nemo_library-1.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: nemo_library
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
 ============
 
 This library helps you with access to NEMO APIs
 
 Installation
 ============
 
-pip install nemo_library
+::
+
+   pip install nemo_library
 
 Sources
 =======
 
 please find all sources on github:
 https://github.com/H3rm1nat0r/nemo_library
 
@@ -30,31 +32,31 @@
 
 ::
 
    [nemo_library]
    nemo_url = https://enter.nemo-ai.com
    userid = <your userid>
    password = <your password>
+   environment = [prod|dev|demo]
 
-usage
-=====
+Methods
+=======
+
+LoadReport method
+-----------------
+
+Load a report from NEMO and return this as pandas dataframe
 
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
-   nl.UploadFile(filename="test.csv")
    df = nl.LoadReport(report_guid="b82cfed8-81a7-44e0-b3da-c76454540697")
 
-LoadReport method
------------------
-
-Load a report from NEMO and return this as pandas dataframe
-
 report_guid
 ~~~~~~~~~~~
 
 This methode takes 1 mandatory parameter, the report_guid. You can find
 “your” guid in NEMO meta data. Just open the definition of the report in
 meta data and copy the GUID from your browser URL.
 
@@ -67,14 +69,48 @@
 max_pages
 ~~~~~~~~~
 
 By default all pages from the report are loaded. You can optionally
 restrict the amount of data by providing max_pages parameter and you’ll
 get not more than this number of pages (usually 1 page holds 20 records)
 
+UploadFile method
+-----------------
+
+(Re-)Upload a CSV file into an existing project
+
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
+
+ProjectProperty method
+----------------------
+
+Get a project property
+
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   val = nl.ProjectProperty(propertyname="ExpDateTo")
+
+.. _projectproperty-method-1:
+
+ProjectProperty method
+----------------------
+
+.. _projectproperty-method-2:
+
+ProjectProperty method
+----------------------
+
 Contributions
 =============
 
 Contributions are welcome! If you would like to suggest improvements or
 have found a bug, please open an issue or submit a pull request.
 
 License
```

### Comparing `nemo_library-1.0.7/README.md` & `nemo_library-1.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,82 @@
 # NEMO Library
 
 This library helps you with access to NEMO APIs
 
 # Installation
 
+```
 pip install nemo_library
+```
 
 # Sources
 
 please find all sources on github: https://github.com/H3rm1nat0r/nemo_library
 
 # configuration
 
 please create a file "config.ini". This is an example for the content:
 ```
 [nemo_library]
 nemo_url = https://enter.nemo-ai.com
 userid = <your userid>
 password = <your password>
+environment = [prod|dev|demo]
 ```
 
-# usage
+# Methods
+
+
+## LoadReport method
+
+Load a report from NEMO and return this as pandas dataframe
 
 ```python
 from nemo_library import NemoLibrary
 
 nl = NemoLibrary()
-nl.UploadFile(filename="test.csv")
 df = nl.LoadReport(report_guid="b82cfed8-81a7-44e0-b3da-c76454540697")
 ```
 
-## LoadReport method
-
-Load a report from NEMO and return this as pandas dataframe
-
 ### report_guid
 
 This methode takes 1 mandatory parameter, the report_guid. You can find "your" guid in NEMO meta data. Just open the definition of the report in meta data and copy the GUID from your browser URL.
 
 The report "(SAMPLE) Replenishment Time Analysis Purchased Parts" for example has this URL: https://enter.nemo-ai.com/nemo/metadata/report/b82cfed8-81a7-44e0-b3da-c76454540697 and thus the GUID you need is then "b82cfed8-81a7-44e0-b3da-c76454540697"
 
 ### max_pages
 
 By default all pages from the report are loaded. You can optionally restrict the amount of data by providing max_pages parameter and you'll get not more than this number of pages (usually 1 page holds 20 records)
 
+## UploadFile method
+
+(Re-)Upload a CSV file into an existing project
+
+```python
+from nemo_library import NemoLibrary
+
+nl = NemoLibrary()
+nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
+````
+
+## ProjectProperty method
+
+Get a project property
+
+```python
+from nemo_library import NemoLibrary
+
+nl = NemoLibrary()
+val = nl.ProjectProperty(propertyname="ExpDateTo")
+````
+
+
+## ProjectProperty method
+## ProjectProperty method
+
 # Contributions
 
 Contributions are welcome! If you would like to suggest improvements or have found a bug, please open an issue or submit a pull request.
 
 # License
 
 This project is released under the Unlicense. You can find the full text of the Unlicense in the [UNLICENSE](UNLICENSE) file. This means that the code is released into the public domain, and you are free to use, modify, distribute, and do whatever you want with it, without any restrictions or requirements.
```

### Comparing `nemo_library-1.0.7/README.rst` & `nemo_library-1.0.8/nemo_library.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+Metadata-Version: 2.1
+Name: nemo-library
+Version: 1.0.8
+Summary: A library for uploading data to and downloading reports from NEMO cloud solution
+Author: Gunnar Schug
+Author-email: GunnarSchug81@gmail.com
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
+
 NEMO Library
 ============
 
 This library helps you with access to NEMO APIs
 
 Installation
 ============
 
-pip install nemo_library
+::
+
+   pip install nemo_library
 
 Sources
 =======
 
 please find all sources on github:
 https://github.com/H3rm1nat0r/nemo_library
 
@@ -21,31 +32,31 @@
 
 ::
 
    [nemo_library]
    nemo_url = https://enter.nemo-ai.com
    userid = <your userid>
    password = <your password>
+   environment = [prod|dev|demo]
+
+Methods
+=======
 
-usage
-=====
+LoadReport method
+-----------------
+
+Load a report from NEMO and return this as pandas dataframe
 
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
-   nl.UploadFile(filename="test.csv")
    df = nl.LoadReport(report_guid="b82cfed8-81a7-44e0-b3da-c76454540697")
 
-LoadReport method
------------------
-
-Load a report from NEMO and return this as pandas dataframe
-
 report_guid
 ~~~~~~~~~~~
 
 This methode takes 1 mandatory parameter, the report_guid. You can find
 “your” guid in NEMO meta data. Just open the definition of the report in
 meta data and copy the GUID from your browser URL.
 
@@ -58,14 +69,48 @@
 max_pages
 ~~~~~~~~~
 
 By default all pages from the report are loaded. You can optionally
 restrict the amount of data by providing max_pages parameter and you’ll
 get not more than this number of pages (usually 1 page holds 20 records)
 
+UploadFile method
+-----------------
+
+(Re-)Upload a CSV file into an existing project
+
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
+
+ProjectProperty method
+----------------------
+
+Get a project property
+
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   val = nl.ProjectProperty(propertyname="ExpDateTo")
+
+.. _projectproperty-method-1:
+
+ProjectProperty method
+----------------------
+
+.. _projectproperty-method-2:
+
+ProjectProperty method
+----------------------
+
 Contributions
 =============
 
 Contributions are welcome! If you would like to suggest improvements or
 have found a bug, please open an issue or submit a pull request.
 
 License
```

### Comparing `nemo_library-1.0.7/nemo_library/nemo_library.py` & `nemo_library-1.0.8/nemo_library/nemo_library.py`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.7/nemo_library/symbols.py` & `nemo_library-1.0.8/nemo_library/symbols.py`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.7/nemo_library.egg-info/PKG-INFO` & `nemo_library-1.0.8/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-Metadata-Version: 2.1
-Name: nemo-library
-Version: 1.0.7
-Summary: A library for uploading data to and downloading reports from NEMO cloud solution
-Author: Gunnar Schug
-Author-email: GunnarSchug81@gmail.com
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/x-rst
-
 NEMO Library
 ============
 
 This library helps you with access to NEMO APIs
 
 Installation
 ============
 
-pip install nemo_library
+::
+
+   pip install nemo_library
 
 Sources
 =======
 
 please find all sources on github:
 https://github.com/H3rm1nat0r/nemo_library
 
@@ -30,31 +23,31 @@
 
 ::
 
    [nemo_library]
    nemo_url = https://enter.nemo-ai.com
    userid = <your userid>
    password = <your password>
+   environment = [prod|dev|demo]
+
+Methods
+=======
 
-usage
-=====
+LoadReport method
+-----------------
+
+Load a report from NEMO and return this as pandas dataframe
 
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
-   nl.UploadFile(filename="test.csv")
    df = nl.LoadReport(report_guid="b82cfed8-81a7-44e0-b3da-c76454540697")
 
-LoadReport method
------------------
-
-Load a report from NEMO and return this as pandas dataframe
-
 report_guid
 ~~~~~~~~~~~
 
 This methode takes 1 mandatory parameter, the report_guid. You can find
 “your” guid in NEMO meta data. Just open the definition of the report in
 meta data and copy the GUID from your browser URL.
 
@@ -67,14 +60,48 @@
 max_pages
 ~~~~~~~~~
 
 By default all pages from the report are loaded. You can optionally
 restrict the amount of data by providing max_pages parameter and you’ll
 get not more than this number of pages (usually 1 page holds 20 records)
 
+UploadFile method
+-----------------
+
+(Re-)Upload a CSV file into an existing project
+
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
+
+ProjectProperty method
+----------------------
+
+Get a project property
+
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   val = nl.ProjectProperty(propertyname="ExpDateTo")
+
+.. _projectproperty-method-1:
+
+ProjectProperty method
+----------------------
+
+.. _projectproperty-method-2:
+
+ProjectProperty method
+----------------------
+
 Contributions
 =============
 
 Contributions are welcome! If you would like to suggest improvements or
 have found a bug, please open an issue or submit a pull request.
 
 License
```

### Comparing `nemo_library-1.0.7/setup.py` & `nemo_library-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nemo_library',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     install_requires=[
         'requests','pandas'
     ],
     author='Gunnar Schug',
     author_email='GunnarSchug81@gmail.com',
     description='A library for uploading data to and downloading reports from NEMO cloud solution',
```

