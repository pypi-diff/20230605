# Comparing `tmp/esa-1.3.4.tar.gz` & `tmp/esa-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esa-1.3.4.tar", last modified: Sat Dec 10 04:23:47 2022, max compression
+gzip compressed data, was "esa-1.3.5.tar", last modified: Mon Jun  5 21:17:23 2023, max compression
```

## Comparing `esa-1.3.4.tar` & `esa-1.3.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-12-10 04:23:47.149555 esa-1.3.4/
--rw-rw-rw-   0        0        0    11571 2022-12-09 19:45:24.000000 esa-1.3.4/LICENSE
--rw-rw-rw-   0        0        0       88 2022-12-09 19:45:24.000000 esa-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5596 2022-12-10 04:23:47.149555 esa-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4090 2022-12-10 04:22:34.000000 esa-1.3.4/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-10 04:23:47.123664 esa-1.3.4/docs/
-drwxrwxrwx   0        0        0        0 2022-12-10 04:23:47.123664 esa-1.3.4/docs/rst/
-drwxrwxrwx   0        0        0        0 2022-12-10 04:23:47.129644 esa-1.3.4/docs/rst/welcome/
--rw-rw-rw-   0        0        0     6378 2022-12-10 04:22:34.000000 esa-1.3.4/docs/rst/welcome/changelog.rst
-drwxrwxrwx   0        0        0        0 2022-12-10 04:23:47.138604 esa-1.3.4/esa/
--rw-rw-rw-   0        0        0      543 2022-12-10 04:23:47.000000 esa-1.3.4/esa/__about__.py
--rw-rw-rw-   0        0        0      834 2022-12-10 04:23:47.000000 esa-1.3.4/esa/__init__.py
--rw-rw-rw-   0        0        0     1106 2022-12-09 19:45:25.000000 esa-1.3.4/esa/_performance.py
--rw-rw-rw-   0        0        0     1296 2022-12-10 04:22:34.000000 esa-1.3.4/esa/_performance_jit.py
--rw-rw-rw-   0        0        0   208384 2022-12-09 19:45:25.000000 esa-1.3.4/esa/performance310.pyd
--rw-rw-rw-   0        0        0   218624 2022-12-09 19:45:25.000000 esa-1.3.4/esa/performance37.pyd
--rw-rw-rw-   0        0        0   194560 2022-12-09 19:45:25.000000 esa-1.3.4/esa/performance38.pyd
--rw-rw-rw-   0        0        0   194560 2022-12-09 19:45:25.000000 esa-1.3.4/esa/performance39.pyd
--rw-rw-rw-   0        0        0   155132 2022-12-10 04:22:34.000000 esa-1.3.4/esa/saw.py
-drwxrwxrwx   0        0        0        0 2022-12-10 04:23:47.144586 esa-1.3.4/esa.egg-info/
--rw-rw-rw-   0        0        0     5596 2022-12-10 04:23:47.000000 esa-1.3.4/esa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2022-12-10 04:23:47.000000 esa-1.3.4/esa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-10 04:23:47.000000 esa-1.3.4/esa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-09 19:45:59.000000 esa-1.3.4/esa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      171 2022-12-10 04:23:47.000000 esa-1.3.4/esa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-10 04:23:47.000000 esa-1.3.4/esa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-10 04:23:47.150551 esa-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     3394 2022-12-10 04:22:34.000000 esa-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-10 04:23:47.148560 esa-1.3.4/tests/
--rw-rw-rw-   0        0        0        0 2022-12-09 19:45:25.000000 esa-1.3.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1608 2022-12-09 19:45:25.000000 esa-1.3.4/tests/constants.py
--rw-rw-rw-   0        0        0     4248 2022-12-09 19:45:25.000000 esa-1.3.4/tests/run_tests_for_all_python_versions.py
--rw-rw-rw-   0        0        0   107496 2022-12-10 04:22:34.000000 esa-1.3.4/tests/test_saw.py
--rw-rw-rw-   0        0        0     2664 2022-12-09 19:45:25.000000 esa-1.3.4/tests/test_snippets.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:17:23.375020 esa-1.3.5/
+-rw-rw-rw-   0        0        0    11571 2023-05-31 12:10:49.000000 esa-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-05-31 12:10:49.000000 esa-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5731 2023-06-05 21:17:23.374024 esa-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4248 2023-06-05 21:15:21.000000 esa-1.3.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 21:17:23.310745 esa-1.3.5/docs/
+drwxrwxrwx   0        0        0        0 2023-06-05 21:17:23.310745 esa-1.3.5/docs/rst/
+drwxrwxrwx   0        0        0        0 2023-06-05 21:17:23.322331 esa-1.3.5/docs/rst/welcome/
+-rw-rw-rw-   0        0        0     6916 2023-06-05 21:15:21.000000 esa-1.3.5/docs/rst/welcome/changelog.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 21:17:23.350135 esa-1.3.5/esa/
+-rw-rw-rw-   0        0        0      543 2023-06-05 21:17:23.000000 esa-1.3.5/esa/__about__.py
+-rw-rw-rw-   0        0        0      834 2023-06-05 21:17:23.000000 esa-1.3.5/esa/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-05-31 12:10:50.000000 esa-1.3.5/esa/_performance.py
+-rw-rw-rw-   0        0        0     1296 2023-05-31 12:10:50.000000 esa-1.3.5/esa/_performance_jit.py
+-rw-rw-rw-   0        0        0   208384 2023-05-31 12:10:50.000000 esa-1.3.5/esa/performance310.pyd
+-rw-rw-rw-   0        0        0   218624 2023-05-31 12:10:50.000000 esa-1.3.5/esa/performance37.pyd
+-rw-rw-rw-   0        0        0   194560 2023-05-31 12:10:50.000000 esa-1.3.5/esa/performance38.pyd
+-rw-rw-rw-   0        0        0   194560 2023-05-31 12:10:50.000000 esa-1.3.5/esa/performance39.pyd
+-rw-rw-rw-   0        0        0   157978 2023-06-05 21:15:21.000000 esa-1.3.5/esa/saw.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:17:23.362084 esa-1.3.5/esa.egg-info/
+-rw-rw-rw-   0        0        0     5731 2023-06-05 21:17:23.000000 esa-1.3.5/esa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-06-05 21:17:23.000000 esa-1.3.5/esa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 21:17:23.000000 esa-1.3.5/esa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 13:05:31.000000 esa-1.3.5/esa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      171 2023-06-05 21:17:23.000000 esa-1.3.5/esa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 21:17:23.000000 esa-1.3.5/esa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 21:17:23.375020 esa-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     3394 2023-05-31 12:10:50.000000 esa-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:17:23.373027 esa-1.3.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:10:50.000000 esa-1.3.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     1608 2023-05-31 12:10:50.000000 esa-1.3.5/tests/constants.py
+-rw-rw-rw-   0        0        0     4248 2023-05-31 12:10:50.000000 esa-1.3.5/tests/run_tests_for_all_python_versions.py
+-rw-rw-rw-   0        0        0   108983 2023-06-05 21:15:21.000000 esa-1.3.5/tests/test_saw.py
+-rw-rw-rw-   0        0        0     2664 2023-05-31 12:10:50.000000 esa-1.3.5/tests/test_snippets.py
```

### Comparing `esa-1.3.4/LICENSE` & `esa-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `esa-1.3.4/PKG-INFO` & `esa-1.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: esa
-Version: 1.3.4
+Version: 1.3.5
 Summary: Easy SimAuto (ESA): An easy-to-use Python connector to PowerWorld Simulator Automation Server (SimAuto).
 Home-page: https://github.com/mzy2240/ESA
 Author: Zeyu Mao, Brandon Thayer, Yijing Liu
 Author-email: zeyumao2@tamu.edu, blthayer@tamu.edu, yiji21@tamu.edu
 License: Apache License 2.0
 Keywords: Python,PowerWorld,PowerWorld Simulator,Simulator,PowerWorld Simulation Automation Server,SimAuto,Automation,Power Systems,Electric Power,Power,Easy SimAuto,ESA,Smart Grid,Numpy,Pandas
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -33,14 +32,16 @@
 
 Easy SimAuto (ESA)
 ==================
 .. image:: https://img.shields.io/pypi/v/esa.svg
    :target: https://pypi.org/project/esa/
 .. image:: https://img.shields.io/pypi/pyversions/esa.svg
    :target: https://pypi.org/project/esa/
+.. image:: https://img.shields.io/discord/1114563747651006524
+   :target: https://discord.gg/V9v8NRCT
 .. image:: https://joss.theoj.org/papers/10.21105/joss.02289/status.svg
    :target: https://doi.org/10.21105/joss.02289
 .. image:: https://img.shields.io/pypi/l/esa.svg
    :target: https://github.com/mzy2240/ESA/blob/master/LICENSE
 .. image:: https://pepy.tech/badge/esa/month
    :target: https://pepy.tech/project/esa
 .. image:: https://img.shields.io/badge/coverage-100%25-brightgreen
@@ -105,37 +106,35 @@
 Currently ESA supports PW Simulator V17, V18, V19, V20, V21, V22 and V23.
 
 
 Testing Coverage
 ----------------
 
 The ESA team works hard to ensure ESA is well tested, and we strive for
-100% testing coverage. The table below shows the most up-to-date
+100% testing coverage (sometimes we cannot due to lack of specific add-ons). The table below shows the most up-to-date
 testing coverage data for ESA, using `coverage
 <https://pypi.org/project/coverage/>`__.
 
-.. table:: ESA's testing coverage as of 2022-12-09 (Git commit: 9bf6a24)
+.. table:: ESA's testing coverage as of 2023-05-31 (Git commit: 7180cc9)
     :widths: auto
     :align: left
 
     +-----------------+-------------------+-----------------+-----------------+--------------------+
     | Name            |   Num. Statements |   Missing Lines |   Covered Lines |   Percent Coverage |
     +=================+===================+=================+=================+====================+
-    | esa/__init__.py |                 2 |               0 |               2 |                100 |
+    | esa/__init__.py |                 2 |               0 |               2 |           100      |
     +-----------------+-------------------+-----------------+-----------------+--------------------+
-    | esa/saw.py      |              1196 |               0 |            1196 |                100 |
+    | esa/saw.py      |              1206 |               2 |            1204 |            99.8342 |
     +-----------------+-------------------+-----------------+-----------------+--------------------+
 
 License
 -------
 
 `Apache License 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`__
 
 Contributing
 ------------
 
 We welcome contributions! Please read ``contributing.md``.
 
 .. _documentation: https://mzy2240.github.io/ESA/
 .. _documented: https://mzy2240.github.io/ESA/
-
-
```

### Comparing `esa-1.3.4/README.rst` & `esa-1.3.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Easy SimAuto (ESA)
 ==================
 .. image:: https://img.shields.io/pypi/v/esa.svg
    :target: https://pypi.org/project/esa/
 .. image:: https://img.shields.io/pypi/pyversions/esa.svg
    :target: https://pypi.org/project/esa/
+.. image:: https://img.shields.io/discord/1114563747651006524
+   :target: https://discord.gg/V9v8NRCT
 .. image:: https://joss.theoj.org/papers/10.21105/joss.02289/status.svg
    :target: https://doi.org/10.21105/joss.02289
 .. image:: https://img.shields.io/pypi/l/esa.svg
    :target: https://github.com/mzy2240/ESA/blob/master/LICENSE
 .. image:: https://pepy.tech/badge/esa/month
    :target: https://pepy.tech/project/esa
 .. image:: https://img.shields.io/badge/coverage-100%25-brightgreen
@@ -72,28 +74,28 @@
 Currently ESA supports PW Simulator V17, V18, V19, V20, V21, V22 and V23.
 
 
 Testing Coverage
 ----------------
 
 The ESA team works hard to ensure ESA is well tested, and we strive for
-100% testing coverage. The table below shows the most up-to-date
+100% testing coverage (sometimes we cannot due to lack of specific add-ons). The table below shows the most up-to-date
 testing coverage data for ESA, using `coverage
 <https://pypi.org/project/coverage/>`__.
 
-.. table:: ESA's testing coverage as of 2022-12-09 (Git commit: 9bf6a24)
+.. table:: ESA's testing coverage as of 2023-05-31 (Git commit: 7180cc9)
     :widths: auto
     :align: left
 
     +-----------------+-------------------+-----------------+-----------------+--------------------+
     | Name            |   Num. Statements |   Missing Lines |   Covered Lines |   Percent Coverage |
     +=================+===================+=================+=================+====================+
-    | esa/__init__.py |                 2 |               0 |               2 |                100 |
+    | esa/__init__.py |                 2 |               0 |               2 |           100      |
     +-----------------+-------------------+-----------------+-----------------+--------------------+
-    | esa/saw.py      |              1196 |               0 |            1196 |                100 |
+    | esa/saw.py      |              1206 |               2 |            1204 |            99.8342 |
     +-----------------+-------------------+-----------------+-----------------+--------------------+
 
 License
 -------
 
 `Apache License 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`__
```

### Comparing `esa-1.3.4/docs/rst/welcome/changelog.rst` & `esa-1.3.5/docs/rst/welcome/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 Changes made with each ESA release are listed here. Please note that
 versions prior to 1.0.0 are not listed here, but are still available on
 `PyPi <https://pypi.org/project/esa/#history>`__.
 
-Version 1.3.3
+Version 1.3.5
+^^^^^^^^^^^^^
+
+* Fix bug in `get_lodf_matrix` that causes mismatched column names and column values
+* Add new parameter ignore_new_branch to `get_lodf_matrix` to ensure the returned matrix is square
+* Fix bug associated with filename format in `DetermineBranchesThatCreateIslands`
+* Fix bug associated with filename format in `DetermineShortestPath`
+* Fix bug in test of `ListOfDevices` associated with dataframe index data type
+* Fix bug in test of `clean_df_or_series` associated with dataframe index data type
+
+Version 1.3.4
 ^^^^^^^^^^^^^
 
 * Add `DetermineBranchesThatCreateIslands`
 * Add `DeterminePathDistance`
 * Add `DetermineShortestPath`
 * Add `RunScriptCommand2`
 * Add `ProgramInformation` property
```

### Comparing `esa-1.3.4/esa/__about__.py` & `esa-1.3.5/esa/__about__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 __github__ = "https://github.com/mzy2240/ESA"
 __docs__ = "https://mzy2240.github.io/ESA"
 __tracker__ = "https://github.com/mzy2240/ESA/issues"
 __pypi__ = "https://pypi.org/project/esa/"
 __email__ = "me@zeyumao.com"
 __license__ = "Apache License 2.0"
 __copyright__ = "Copyright 2022 - Zeyu Mao"
-__version__ = "1.3.4"
+__version__ = "1.3.5"
```

### Comparing `esa-1.3.4/esa/__init__.py` & `esa-1.3.5/esa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
     via SAW helper methods like
     ``change_and_confirm_params_multiple_element``
 *   __version__: ESA's version.
 """
 # Please keep the docstring above up to date with all the imports.
 from .saw import SAW, PowerWorldError, COMError, CommandNotRespectedError,\
     Error
-__version__ = "1.3.4"
+__version__ = "1.3.5"
```

### Comparing `esa-1.3.4/esa/_performance.py` & `esa-1.3.5/esa/_performance.py`

 * *Files identical despite different names*

### Comparing `esa-1.3.4/esa/_performance_jit.py` & `esa-1.3.5/esa/_performance_jit.py`

 * *Files identical despite different names*

### Comparing `esa-1.3.4/esa/saw.py` & `esa-1.3.5/esa/saw.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
     # set_simauto_property method.
     SIMAUTO_PROPERTIES = {'CreateIfNotFound': bool, 'CurrentDir': str,
                           'UIVisible': bool}
 
     def __init__(self, FileName, early_bind=False, UIVisible=False,
                  object_field_lookup=('bus', 'gen', 'load', 'shunt',
                                       'branch'),
-                 CreateIfNotFound=False, pw_order=False):
+                 CreateIfNotFound:bool=False, UseDefinedNamesInVariables:bool=False,
+                 pw_order=False):
         """Initialize SimAuto wrapper. The case will be opened, and
         object fields given in object_field_lookup will be retrieved.
 
         :param FileName: Full file path to .pwb file to open. This will
             be passed to the SimAuto function OpenCase.
         :param early_bind: Whether (True) or not (False) to connect to
             SimAuto via early binding.
@@ -139,14 +140,16 @@
             Objects that already exist will be updated.
             Set CreateIfNotFound = False to not create new objects
             and only update existing ones.
         :param object_field_lookup: Listing of PowerWorld objects to
             initially look up available fields for. Objects not
             specified for lookup here will be looked up later as
             necessary.
+        :param UseDefinedNamesInVariables: Set UseDefinedNamesInVariables to True
+            if you want to have custom field with custom header. Default is False.
         :param pw_order: Set pw_order = True if you want to have exact
             same order as shown in PW Simulator. Default is False, which
             generally sorts the data in a bus ascending order.
 
         Note that
         `Microsoft recommends
         <https://docs.microsoft.com/en-us/office/troubleshoot/office-developer/binding-type-available-to-automation-clients>`__
@@ -208,14 +211,23 @@
         # Open the case.
         self.OpenCase(FileName=FileName)
 
         # Get the version number and the build date
         version_string, self.build_date = self.get_version_and_builddate()
         self.version = int(re.search(r'\d+', version_string)[0])
 
+        # Set the UseDefinedNamesInVariables property.
+        if UseDefinedNamesInVariables:
+            self.exec_aux("""
+                CaseInfo_Options_Value (Option,Value)
+                    {
+                        "UseDefinedNamesInVariables"    "YES"
+                    }
+            """)
+
         # Sensitivity-related initialization
         self.lodf = None
 
         # Look up and cache field listing and key fields for the given
         # object types in object_field_lookup.
         self._object_fields = {}
         self._object_key_fields = {}
@@ -231,14 +243,31 @@
             # Get the key fields for this object. This will store the
             # results in self._object_key_fields[o]
             self.get_key_fields_for_object_type(ObjectType=o)
 
     ####################################################################
     # Helper Functions
     ####################################################################
+    def exec_aux(self, aux: str, use_double_quotes:bool = False):
+        """Helper function to execute auxiliary script directly. Skip the
+        hassle to save the aux script to a file and then execute it.
+
+        :param aux: Auxiliary script (including data section) to execute.
+        :param use_double_quotes: Whether to use double quotes or single
+            quotes. Default is False. Change to True will replace all the
+            single quotes with double quotes.
+        """
+        if use_double_quotes:
+            aux = aux.replace("'", '"')
+        file = tempfile.NamedTemporaryFile(mode='wt', suffix='.aux', delete=False)
+        file.write(aux)
+        file.close()
+        self.ProcessAuxFile(file.name)
+        os.unlink(file.name)
+
     def change_and_confirm_params_multiple_element(self, ObjectType: str,
                                                    command_df: pd.DataFrame) \
             -> None:
         """Change parameters for multiple objects of the same type, and
         confirm that the change was respected by PowerWorld.
 
         :param ObjectType: The type of objects you are changing
@@ -888,15 +917,15 @@
                 nx.set_node_attributes(graph, node_attr_reformat)
             except ValueError as e:
                 raise e
         self.pw_order = original
         return graph
 
     def DeterminePathDistance(self, start: str, BranchDistMeas: str = "X", BranchFilter: str = "ALL",
-                              BusField="CustomFloat:1"):
+                              BusField="CustomFloat:1") -> pd.DataFrame:
         """
         Powerworld's built-in function to calculate a distance measure at each bus in the entire model.
         The distance measure will represent how far each bus is from the starting group specified. The distance
         measure can be related to impedance, geographical distance, or simply the number of nodes.
 
         :param start: The starting location. String only. Follow the powerworld auxilliary file document.
         :param BranchDistMeas: is either X, Z, Length, Nodes, or a field variable name for a branch.
@@ -913,34 +942,36 @@
         df = self.GetParametersMultipleElement("Bus", key + [BusField])
         df.rename(columns={BusField: BranchDistMeas}, inplace=True)
         df["BusNum"] = df["BusNum"].astype(int)
         df[BranchDistMeas] = df[BranchDistMeas].astype(float)
         self.pw_order = original
         return df
 
-    def DetermineBranchesThatCreateIslands(self, Filter: str = "ALL", StoreBuses: str = "YES", SetSelectedOnLines: str = "NO"):
+    def DetermineBranchesThatCreateIslands(self, Filter: str = "ALL", StoreBuses: str = "YES", SetSelectedOnLines: str = "NO") -> pd.DataFrame:
         """
         Powerworld's built-in function to determine the branches whose outage results in island formation. Note that
         setting the Selected field will overwrite the Selected fields.
 
         :param Filter: This parameter is used to specify which branches are checked
         :param StoreBuses: YES to store the buses in the island
         :param SetSelectedOnLines: Yes to set the SELECTED field to YES for branches that create islands
 
         :returns: A dataframe that contains the branch and the island information
         """
         file = tempfile.NamedTemporaryFile()
         filename = Path(file.name).as_posix()
         file.close()
-        statement = f"DetermineBranchesThatCreateIslands({Filter},{StoreBuses},{filename},{SetSelectedOnLines},CSV);"
+        statement = f"DetermineBranchesThatCreateIslands({Filter},{StoreBuses},\"{filename}\",{SetSelectedOnLines}," \
+                    f"CSV);"
+        print(statement)
         self.RunScriptCommand(statement)
         df = pd.read_csv(filename, header=0)
         return df
 
-    def DetermineShortestPath(self, start: str, end: str, BranchDistanceMeasure: str = "X", BranchFilter: str = "ALL"):
+    def DetermineShortestPath(self, start: str, end: str, BranchDistanceMeasure: str = "X", BranchFilter: str = "ALL") -> pd.DataFrame:
         """
         Powerworld's built-in function to calculate the shortest path between a starting group and an ending group. The
         first bus listed in the dataframe will be in the end grouping and the last bus listed will be the start grouping.
         The dataframe will have a line for each bus passed.
 
         :param start: same as the starting place for the DeterminePathDistance function
         :param end: same as the starting place for the DeterminePathDistance function
@@ -948,28 +979,33 @@
         :param BranchFilter: same as for the DeterminePathDistance function
 
         :returns: A dataframe with number, distance, and name
         """
         file = tempfile.NamedTemporaryFile()
         filename = Path(file.name).as_posix()
         file.close()
-        statement = f"DetermineShortestPath({start}, {end}, {BranchDistanceMeasure}, {BranchFilter}, {filename});"
+        statement = f"DetermineShortestPath({start}, {end}, {BranchDistanceMeasure}, {BranchFilter}, \"{filename}\");"
         self.RunScriptCommand(statement)
         df = pd.read_csv(filename, header=None, delim_whitespace=True, names=["BusNum", BranchDistanceMeasure, "BusName"])
         df["BusNum"] = df["BusNum"].astype(int)
         return df
 
-    def get_lodf_matrix(self, precision: int = 3, method: str = 'DC', post: bool = True,
-                        raw: bool = False):
+    def get_lodf_matrix(self, precision: int = 3, ignore_open_branch: bool = True, method: str = 'DC',
+                        post: bool = True, raw: bool = False):
         """Obtain LODF matrix in numpy array or scipy sparse matrix.
         By default, it obtains the lodf matrix directly from PW. If size
         is larger than 1000, then precision will be applied to filter out
         small values and the result will be returned in scipy sparse matrix.
+        The line (lines) in "OPEN" status are removed from the returned 
+        results, which is aligned with PW GUI. Make sure the line in 
+        interest is in "CLOSED" status, or calculate LCDF value instead.
 
         :param precision:  number of decimal to keep.
+        :param ignore_open_branch: Ignore branches are open or not. Set to True to monitor only those branches that
+            are closed. Set to False to monitor branches regardless of their status. Default is True.
         :param method: The linear method to be used for the LODF calculation. Default is DC.
             Change to DCPS would take phase shifter into account. Note: AC is NOT an option for the
             LODF calculation.
         :param post: Set to True to calculate any line closure sensitivies relative to
             post-closure flow on the line being closed. This is known as the LCDF value. Set to
             False to calculate any line closure sensitivities based on calculating the flow on the
             line being closed from pre-closure voltages and angles. This is known as the MLCDF value.
@@ -977,46 +1013,56 @@
             table shown in the PW GUI. Default is False.
 
         :returns: The LODF matrix and a boolean vector to indicate which lines would cause
             islanding.
         """
         original = self.pw_order
         self.pw_order = True
-        count = self.ListOfDevices('branch').shape[0]
+        # count = self.ListOfDevices('branch').shape[0]
+        # Changed on 03/18/2023. Fixed issue of shifted column & rows when there is at least one line in outage.
+        branch_key_fields = self.get_key_field_list('Branch')
+        params = branch_key_fields + ['Status']
+        branches_data = self.GetParametersMultipleElement(ObjectType='Branch', ParamList=params)
+        count = branches_data[branches_data['Status'] == 'Closed'].shape[0] if ignore_open_branch else \
+            branches_data.shape[0]
+        ignore_str = 'YES' if ignore_open_branch else 'NO'
         if post:
             self.RunScriptCommand(
-                f"CalculateLODFMatrix(OUTAGES,ALL,ALL,YES,{method},ALL,YES)")
+                f"CalculateLODFMatrix(OUTAGES,ALL,ALL,{ignore_str},{method},ALL,YES)")
         else:
             self.RunScriptCommand(
-                f"CalculateLODFMatrix(OUTAGES,ALL,ALL,YES,{method},ALL,NO)")
+                f"CalculateLODFMatrix(OUTAGES,ALL,ALL,{ignore_str},{method},ALL,NO)")
         array = [f"LODFMult:{x}" for x in range(count)]
         if raw:
             array = ['BusNum', 'BusNum:1', 'LineCircuit', 'LineMW'] + array
             container = []
             for batch in partition_all(500, array):
                 df = self.GetParametersMultipleElement('branch', batch)
                 temp = df.apply(pd.to_numeric, errors='coerce')
                 container.append(temp)
             self.lodf = pd.concat(container, axis=1, copy=False)
             df_array = self.lodf.to_numpy(dtype=float) / 100
             self.isl = np.any(df_array >= 10, axis=1)
         else:
             if count <= 1000:
-                self._extracted_from_get_lodf_matrix_9(array)
+                self._extracted_from_get_lodf_matrix_9(array, ignore_open_branch)
             else:
-                self._extracted_from_get_lodf_matrix_16(array, precision)
+                self._extracted_from_get_lodf_matrix_16(array, precision, ignore_open_branch)
         self.pw_order = original
         return self.lodf, self.isl
 
     # TODO Rename this here and in `get_lodf_matrix`
-    def _extracted_from_get_lodf_matrix_16(self, array, precision):
+    def _extracted_from_get_lodf_matrix_16(self, array, precision, ignore_open_branch):
         container = []
         isl = None
         for batch in partition_all(20, array):
             df = self.GetParametersMultipleElement('branch', batch)
+            if ignore_open_branch:
+                df.dropna(axis=0, inplace=True)
+                df.reset_index(inplace=True, drop=True)
             temp = df.to_numpy(dtype=float) / 100
             temp = temp.round(precision)
             isl = np.any(temp >= 10, axis=1) if isl is None else np.logical_or(
                 isl, np.any(temp >= 10, axis=1))
 
             temp[isl, :] = 0
             temp = coo_matrix(temp)
@@ -1027,16 +1073,19 @@
         temp[isl, isl] = -1
         temp = temp.tocsr()
         temp.eliminate_zeros()
         self.lodf = temp
         self.isl = isl
 
     # TODO Rename this here and in `get_lodf_matrix`
-    def _extracted_from_get_lodf_matrix_9(self, array):
+    def _extracted_from_get_lodf_matrix_9(self, array, ignore_open_branch):
         df = self.GetParametersMultipleElement('branch', array)
+        if ignore_open_branch:
+            df.dropna(axis=0, inplace=True)
+            df.reset_index(inplace=True, drop=True)
         temp = df.to_numpy(dtype=float) / 100
         self.isl = np.any(temp >= 10, axis=1)
         temp[self.isl, :] = 0
         temp[self.isl, self.isl] = -1
         self.lodf = temp
 
     def get_incidence_matrix(self):
@@ -1693,15 +1742,15 @@
                 flows = f + lodf[i, :] * f[i]
                 qq = abs(flows) / lim
                 violating_lines = abs(flows) > lim
                 num_of_violations = np.sum(violating_lines)
                 margins = np.maximum(margins, qq)
                 if num_of_violations:
                     ctg[i] = 1
-                    violations[violating_lines] += 1
+                    violations[np.ravel(violating_lines)] += 1
         print(f"The size of N-1 islanding set is {np.sum(c1_isl)}")
         print(
             f"Fast N-1 analysis was performed, {np.sum(ctg)} dangerous N-1 contigencies were found, "
             f"{np.sum(violations > 0)} lines are violated")
         if np.sum(ctg):
             print(
                 "Grid is not N-1 secure. Invoke n1_protect function to automatically increasing limits through lines.")
@@ -2830,15 +2879,14 @@
             the type will not be changed). In addition to the integer
             labeled columns which match the "meta" rows, the "data"
             DataFrame additionally has a "time" column which corresponds
             to the timestamp (in seconds).
         """
         out = self._call_simauto('TSGetContingencyResults', CtgName,
                                  ObjFieldList, str(StartTime), str(StopTime))
-
         # We get (None, (None,)) if the contingency does not exist.
         if out == (None, (None,)):
             return None, None
 
         # Length should always be 2.
         assert len(out) == 2, 'Unexpected return format from PowerWorld.'
 
@@ -2846,15 +2894,16 @@
         meta = pd.DataFrame(
             out[0], columns=['ObjectType', 'PrimaryKey', 'SecondaryKey',
                              'Label', 'VariableName', 'ColHeader'])
 
         # Remove extraneous white space in the strings.
         # https://stackoverflow.com/a/40950485/11052174
         meta = meta.apply(lambda x: x.str.strip(), axis=0)
-
+        # print(out[0])
+        # print(out[1])
         # Extract the data.
         data = pd.DataFrame(out[1])
 
         # Decrement all the columns by 1 so that they line up with the
         # 'meta' frame.
         data.rename(columns=lambda x: x - 1, inplace=True)
 
@@ -3100,15 +3149,14 @@
         # Call the function.
         try:
             output = f(*args)
         except Exception as e:
             m = f'An error occurred when trying to call {func} with {args}'
             self.log.exception(m)
             raise COMError(m) from e
-
         # handle errors
         if output == ('',):
             # If we just get a tuple with the empty string in it,
             # there's nothing to return.
             return None
 
         # There's one inconsistent method, GetFieldMaxNum, which
```

### Comparing `esa-1.3.4/esa.egg-info/PKG-INFO` & `esa-1.3.5/esa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: esa
-Version: 1.3.4
+Version: 1.3.5
 Summary: Easy SimAuto (ESA): An easy-to-use Python connector to PowerWorld Simulator Automation Server (SimAuto).
 Home-page: https://github.com/mzy2240/ESA
 Author: Zeyu Mao, Brandon Thayer, Yijing Liu
 Author-email: zeyumao2@tamu.edu, blthayer@tamu.edu, yiji21@tamu.edu
 License: Apache License 2.0
 Keywords: Python,PowerWorld,PowerWorld Simulator,Simulator,PowerWorld Simulation Automation Server,SimAuto,Automation,Power Systems,Electric Power,Power,Easy SimAuto,ESA,Smart Grid,Numpy,Pandas
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -33,14 +32,16 @@
 
 Easy SimAuto (ESA)
 ==================
 .. image:: https://img.shields.io/pypi/v/esa.svg
    :target: https://pypi.org/project/esa/
 .. image:: https://img.shields.io/pypi/pyversions/esa.svg
    :target: https://pypi.org/project/esa/
+.. image:: https://img.shields.io/discord/1114563747651006524
+   :target: https://discord.gg/V9v8NRCT
 .. image:: https://joss.theoj.org/papers/10.21105/joss.02289/status.svg
    :target: https://doi.org/10.21105/joss.02289
 .. image:: https://img.shields.io/pypi/l/esa.svg
    :target: https://github.com/mzy2240/ESA/blob/master/LICENSE
 .. image:: https://pepy.tech/badge/esa/month
    :target: https://pepy.tech/project/esa
 .. image:: https://img.shields.io/badge/coverage-100%25-brightgreen
@@ -105,37 +106,35 @@
 Currently ESA supports PW Simulator V17, V18, V19, V20, V21, V22 and V23.
 
 
 Testing Coverage
 ----------------
 
 The ESA team works hard to ensure ESA is well tested, and we strive for
-100% testing coverage. The table below shows the most up-to-date
+100% testing coverage (sometimes we cannot due to lack of specific add-ons). The table below shows the most up-to-date
 testing coverage data for ESA, using `coverage
 <https://pypi.org/project/coverage/>`__.
 
-.. table:: ESA's testing coverage as of 2022-12-09 (Git commit: 9bf6a24)
+.. table:: ESA's testing coverage as of 2023-05-31 (Git commit: 7180cc9)
     :widths: auto
     :align: left
 
     +-----------------+-------------------+-----------------+-----------------+--------------------+
     | Name            |   Num. Statements |   Missing Lines |   Covered Lines |   Percent Coverage |
     +=================+===================+=================+=================+====================+
-    | esa/__init__.py |                 2 |               0 |               2 |                100 |
+    | esa/__init__.py |                 2 |               0 |               2 |           100      |
     +-----------------+-------------------+-----------------+-----------------+--------------------+
-    | esa/saw.py      |              1196 |               0 |            1196 |                100 |
+    | esa/saw.py      |              1206 |               2 |            1204 |            99.8342 |
     +-----------------+-------------------+-----------------+-----------------+--------------------+
 
 License
 -------
 
 `Apache License 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`__
 
 Contributing
 ------------
 
 We welcome contributions! Please read ``contributing.md``.
 
 .. _documentation: https://mzy2240.github.io/ESA/
 .. _documented: https://mzy2240.github.io/ESA/
-
-
```

### Comparing `esa-1.3.4/esa.egg-info/SOURCES.txt` & `esa-1.3.5/esa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esa-1.3.4/setup.py` & `esa-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `esa-1.3.4/tests/constants.py` & `esa-1.3.5/tests/constants.py`

 * *Files identical despite different names*

### Comparing `esa-1.3.4/tests/run_tests_for_all_python_versions.py` & `esa-1.3.5/tests/run_tests_for_all_python_versions.py`

 * *Files identical despite different names*

### Comparing `esa-1.3.4/tests/test_saw.py` & `esa-1.3.5/tests/test_saw.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
         df_in = pd.DataFrame([[' 6    ', '7.2234 ', ' yes '],
                               [' 3', '11', '   no ']],
                              columns=['BusNum', 'GenMW', 'GenAGCAble'])
         df_expected = pd.DataFrame([[3, 11.0, 'no'], [6, 7.2234, 'yes']],
                                    columns=['BusNum', 'GenMW', 'GenAGCAble'])
 
         df_actual = saw_14.clean_df_or_series(obj=df_in, ObjectType='gen')
-
+        df_expected.index = df_expected.index.astype('int32')
         pd.testing.assert_frame_equal(df_actual, df_expected)
 
     def test_bad_type(self):
         """Ensure a TypeError is raised if 'obj' is a bad type."""
         with self.assertRaisesRegex(TypeError, 'The given object is not a Da'):
             # noinspection PyTypeChecker
             saw_14.clean_df_or_series(obj=42, ObjectType='shunt')
@@ -685,16 +685,19 @@
         """
         self.assertIsInstance(self.saw.get_ybus(True), np.ndarray)
 
     def test_get_ybus_external(self):
         """
         Test get_ybus function with external ybus file.
         """
-        self.assertIsInstance(self.saw.get_ybus(file="data/ybus.mat"),
-                              csr_matrix)
+        try:
+            ybus = self.saw.get_ybus(file="data/ybus.mat")
+        except FileNotFoundError:
+            ybus = self.saw.get_ybus(file="tests/data/ybus.mat")
+        self.assertIsInstance(ybus,csr_matrix)
 
 
 class GetAdmittanceTestCase(unittest.TestCase):
     """Test get_branch_admittance and get_shunt_admittance function."""
 
     @classmethod
     def setUpClass(cls) -> None:
@@ -882,14 +885,33 @@
         self.assertIsInstance(lodf, sp.sparse.csr.csr_matrix)
 
     def test_get_lodf_matrix_raw(self):
         """Should return a dataframe and a boolean vector
         """
         lodf, isl = self.saw.get_lodf_matrix(raw=True)
         self.assertIsInstance(lodf, pd.DataFrame)
+        
+    def test_get_lodf_matrix_outage(self):
+        """When param ignore_open_branch is set to True, the program should return an (N-x)*(N-x) square matrix and
+        a boolean vector if there is x branch in outage in the case.
+        When param ignore is set to False, the program should return an N*N square matrix and a boolean
+        vector no matter how many branches are in open status.
+        """
+        branch_kf = self.saw.get_key_field_list('Branch')
+        lines_dataPrev = self.saw.GetParametersMultipleElement(ObjectType='Branch', ParamList=branch_kf + [
+            'LineStatus'])
+        lines_dataPrev.loc[lines_dataPrev['BusNum'].isin([1]), 'LineStatus'] = ['Open', 'Open']
+        self.saw.change_and_confirm_params_multiple_element('Branch', lines_dataPrev)
+        lines_data = self.saw.GetParametersMultipleElement(ObjectType='Branch', ParamList=branch_kf + ['LineStatus'])
+        x = lines_data[lines_data['LineStatus'] == 'Open'].shape[0]
+        N = lines_data.shape[0]
+        lodf, isl = self.saw.get_lodf_matrix(ignore_open_branch=True)
+        self.assertEqual(lodf.shape, (N-x, N-x))
+        lodf, isl = self.saw.get_lodf_matrix(ignore_open_branch=False)
+        self.assertEqual(lodf.shape, (N, N))
 
     def test_get_incidence_matrix(self):
         """ Should return an N*M matrix
         """
         b = self.saw.get_incidence_matrix()
         self.assertNotEqual(b.shape[0], b.shape[1])
 
@@ -1841,15 +1863,15 @@
         # Query.
         result = saw_14.ListOfDevices(ObjType='Gen')
         # The 14 bus case has 5 generators at buses 1, 2, 3, 6, and 8.
         # Since there's only one generator at each bus, they have an
         # ID of 1. However, ID is a string field.
         expected = pd.DataFrame([[1, '1'], [2, '1'], [3, '1'], [6, '1'],
                                  [8, '1']], columns=['BusNum', 'GenID'])
-
+        expected.index = expected.index.astype('int32')
         pd.testing.assert_frame_equal(expected, result)
 
     def test_shunts(self):
         """There are no shunts in th 14 bus model."""
         result = saw_14.ListOfDevices(ObjType="Shunt")
         self.assertIsNone(result)
```

### Comparing `esa-1.3.4/tests/test_snippets.py` & `esa-1.3.5/tests/test_snippets.py`

 * *Files identical despite different names*

