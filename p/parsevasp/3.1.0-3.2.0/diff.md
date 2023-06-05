# Comparing `tmp/parsevasp-3.1.0.tar.gz` & `tmp/parsevasp-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsevasp-3.1.0.tar", last modified: Fri May 27 11:37:32 2022, max compression
+gzip compressed data, was "parsevasp-3.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `parsevasp-3.1.0.tar` & `parsevasp-3.2.0.tar`

### file list

```diff
@@ -1,42 +1,20 @@
-drwxrwxr-x   0 espenfl   (1000) espenfl   (1000)        0 2022-05-27 11:37:32.087306 parsevasp-3.1.0/
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)       76 2022-05-27 10:31:16.000000 parsevasp-3.1.0/MANIFEST.in
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     1528 2022-05-27 11:37:32.087306 parsevasp-3.1.0/PKG-INFO
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)      536 2022-05-27 10:31:16.000000 parsevasp-3.1.0/README.rst
-drwxrwxr-x   0 espenfl   (1000) espenfl   (1000)        0 2022-05-27 11:37:32.085306 parsevasp-3.1.0/parsevasp/
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)      194 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/__init__.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     5985 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/base.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     4588 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/chgcar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     1943 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/constants.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    10894 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/doscar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     5742 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/eigenval.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    20536 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/incar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    78855 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/incar.yml
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    34220 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/kpoints.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    17776 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/outcar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    36890 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/poscar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    12992 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/stream.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     4756 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/stream.yml
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     9403 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/utils.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)   136240 2022-05-27 10:31:16.000000 parsevasp-3.1.0/parsevasp/vasprun.py
-drwxrwxr-x   0 espenfl   (1000) espenfl   (1000)        0 2022-05-27 11:37:32.086305 parsevasp-3.1.0/parsevasp.egg-info/
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     1528 2022-05-27 11:37:32.000000 parsevasp-3.1.0/parsevasp.egg-info/PKG-INFO
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)      775 2022-05-27 11:37:32.000000 parsevasp-3.1.0/parsevasp.egg-info/SOURCES.txt
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)        1 2022-05-27 11:37:32.000000 parsevasp-3.1.0/parsevasp.egg-info/dependency_links.txt
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)      164 2022-05-27 11:37:32.000000 parsevasp-3.1.0/parsevasp.egg-info/requires.txt
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)       16 2022-05-27 11:37:32.000000 parsevasp-3.1.0/parsevasp.egg-info/top_level.txt
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)      112 2022-05-27 11:37:32.087306 parsevasp-3.1.0/setup.cfg
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     1235 2022-05-27 10:31:16.000000 parsevasp-3.1.0/setup.json
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)      704 2022-05-27 10:31:16.000000 parsevasp-3.1.0/setup.py
-drwxrwxr-x   0 espenfl   (1000) espenfl   (1000)        0 2022-05-27 11:37:32.087306 parsevasp-3.1.0/tests/
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)        0 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/__init__.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     3266 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_chgcar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     9626 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_doscar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     1838 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_eigenval.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     5584 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_incar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    15578 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_kpoints.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    12495 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_outcar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    17449 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_poscar.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)     1998 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_stream.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    38386 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_xml_event.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)    41588 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/test_xml_regular.py
--rw-rw-r--   0 espenfl   (1000) espenfl   (1000)      116 2022-05-27 10:31:16.000000 parsevasp-3.1.0/tests/utils.py
+-rw-r--r--   0        0        0     1075 2023-03-30 11:01:36.486379 parsevasp-3.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      536 2023-03-30 11:01:36.486379 parsevasp-3.2.0/README.rst
+-rw-r--r--   0        0        0      194 2023-06-05 13:14:19.435740 parsevasp-3.2.0/parsevasp/__init__.py
+-rw-r--r--   0        0        0     5985 2023-03-30 11:01:36.486379 parsevasp-3.2.0/parsevasp/base.py
+-rw-r--r--   0        0        0     4588 2023-03-30 11:01:36.486379 parsevasp-3.2.0/parsevasp/chgcar.py
+-rw-r--r--   0        0        0     1943 2023-03-30 11:01:36.486379 parsevasp-3.2.0/parsevasp/constants.py
+-rw-r--r--   0        0        0    10926 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/doscar.py
+-rw-r--r--   0        0        0     5742 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/eigenval.py
+-rw-r--r--   0        0        0    20388 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/incar.py
+-rw-r--r--   0        0        0    78855 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/incar.yml
+-rw-r--r--   0        0        0    37215 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/kpoints.py
+-rw-r--r--   0        0        0    17776 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/outcar.py
+-rw-r--r--   0        0        0    36808 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/poscar.py
+-rw-r--r--   0        0        0     7046 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/potcar.py
+-rw-r--r--   0        0        0    15910 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/stream.py
+-rw-r--r--   0        0        0     5076 2023-06-05 13:14:19.442407 parsevasp-3.2.0/parsevasp/stream.yml
+-rw-r--r--   0        0        0     9403 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/utils.py
+-rw-r--r--   0        0        0   136794 2023-06-05 13:14:19.442407 parsevasp-3.2.0/parsevasp/vasprun.py
+-rw-r--r--   0        0        0     3106 2023-06-05 13:14:19.442407 parsevasp-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 parsevasp-3.2.0/PKG-INFO
```

### Comparing `parsevasp-3.1.0/PKG-INFO` & `parsevasp-3.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 Metadata-Version: 2.1
 Name: parsevasp
-Version: 3.1.0
+Version: 3.2.0
 Summary: A general parser for VASP
-Home-page: https://github.com/aiida-vasp/parsevasp
-Author: Espen Flage-Larsen
-Author-email: espen.flage-larsen@sintef.no
-License: MIT
-Description: =============================
-        Parsevasp - a parser for VASP
-        =============================
-        
-        .. image:: https://img.shields.io/pypi/v/parsevasp
-        
-        .. image:: https://img.shields.io/pypi/pyversions/parsevasp
-        
-        .. image:: https://github.com/aiida-vasp/parsevasp/workflows/parsevasp/badge.svg
-          :target: https://github.com/aiida-vasp/parsevasp/actions
-        
-        .. image:: https://codecov.io/gh/espenfl/aiida-vasp/branch/develop/graph/badge.svg
-          :target: https://codecov.io/gh/espenfl/aiida-vasp
-        
-        
-        A parser for VASP using lxml or fallback elementTree.
-        
-Keywords: VASP,parser,python,xml
-Platform: UNKNOWN
+Keywords: vasp,parser
+Author-email: Espen Flage-Larsen	 <espen.flage-larsen@sigma2.no>
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.7
+Requires-Dist: numpy
+Requires-Dist: lxml
+Requires-Dist: pyyaml
+Requires-Dist: tox>=3.23.0 ; extra == "pre-commit"
+Requires-Dist: virtualenv>20 ; extra == "pre-commit"
+Requires-Dist: pre-commit~=2.2 ; extra == "pre-commit"
+Requires-Dist: pylint~=2.15.0 ; extra == "pre-commit"
+Requires-Dist: tox>=3.23.0 ; extra == "tests"
+Requires-Dist: virtualenv>20 ; extra == "tests"
+Requires-Dist: pytest~=7.0 ; extra == "tests"
+Requires-Dist: pytest-cov~=2.7,<2.11 ; extra == "tests"
+Requires-Dist: coverage~=6.0 ; extra == "tests"
+Project-URL: Source, https://github.com/aiida-vasp/parsevasp
 Provides-Extra: pre-commit
 Provides-Extra: tests
+
+=============================
+Parsevasp - a parser for VASP
+=============================
+
+.. image:: https://img.shields.io/pypi/v/parsevasp
+
+.. image:: https://img.shields.io/pypi/pyversions/parsevasp
+
+.. image:: https://github.com/aiida-vasp/parsevasp/workflows/parsevasp/badge.svg
+  :target: https://github.com/aiida-vasp/parsevasp/actions
+
+.. image:: https://codecov.io/gh/espenfl/aiida-vasp/branch/develop/graph/badge.svg
+  :target: https://codecov.io/gh/espenfl/aiida-vasp
+
+
+A parser for VASP using lxml or fallback elementTree.
+
```

### Comparing `parsevasp-3.1.0/README.rst` & `parsevasp-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/base.py` & `parsevasp-3.2.0/parsevasp/base.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/chgcar.py` & `parsevasp-3.2.0/parsevasp/chgcar.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/constants.py` & `parsevasp-3.2.0/parsevasp/constants.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/doscar.py` & `parsevasp-3.2.0/parsevasp/doscar.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,17 +214,18 @@
             else:
                 dos[name] = dos_data[:, i + 1:i + 1 + num_spin]
 
         # Partial density of states
         pdos_items = []
         pdos = np.array([])  # Partial dos is empty by default
         if line_2 in data:
+            start = data.index(line_2) + 1
             for _ in range(num_ions):
-                start = data.index(line_2) + 1
                 pdos_items += [data[start:start + ndos]]
+                start += (ndos + 1)
 
             # Get the number of columns for the pdos section.
             count = len(pdos_items[-1][-1])
             pdos_data = np.array(pdos_items)
 
             # Adjust the spin according to the column definitions
             num_spin = _get_num_spin(count, self._non_collinear)
```

### Comparing `parsevasp-3.1.0/parsevasp/eigenval.py` & `parsevasp-3.2.0/parsevasp/eigenval.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/incar.py` & `parsevasp-3.2.0/parsevasp/incar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Handle INCAR."""
 # pylint: disable=consider-using-f-string
 import io
 import logging
 import sys
 
-from past.builtins import basestring
-
 from parsevasp import constants, utils
 from parsevasp.base import BaseParser
 
 
 class Incar(BaseParser):
     """Class to handle INCAR."""
 
@@ -237,15 +235,15 @@
             clean_tag = entry.get_tag()
             if clean_tag in incar_dict:
                 self._logger.info(f'Tag {entry.get_tag()} already found in the INCAR dictionary, overwriting it.')
             incar_dict[clean_tag] = entry
 
         return incar_dict
 
-    def _convert_value_to_string(self, value):  # pylint: disable=R0201
+    def _convert_value_to_string(self, value):
         """
         Converts a value for an INCAR entry to a string that
         is compatible with VASP.
 
         Parameters
         ----------
         value : string
@@ -536,17 +534,16 @@
         # 1.0 - float
         # 1.0 2.0 3.0 - set of floats
         # 10*1.0 etc., interpreted as strings here
 
         # However, let us also open for the fact that users might
         # give a value what they would in INCAR
 
-        # Make sure we keep compatibility between Python 2 and 3
-        if isinstance(value, basestring):
-            if clean_tag in ('system', 'magmom'):
+        if isinstance(value, str):
+            if clean_tag in ('system', 'magmom', 'm_constr'):
                 # If value is SYSTEM or MAGMOM (can contain asterix), treat it a bit special and
                 # leave its string intact but remove grub
                 clean_value = value.strip()
                 return clean_tag, clean_value, None
 
             # Values is a string, so we have read an INCAR or the user
             # tries to assign an entry with just a string
@@ -597,15 +594,15 @@
         if comment is not None:
             clean_comment = comment.strip()
         else:
             clean_comment = None
 
         return clean_tag, clean_value, clean_comment
 
-    def _test_string_for_bool(self, string):  # pylint: disable=R0201
+    def _test_string_for_bool(self, string):
         """
         Detects if string contains Fortran bool.
 
         Parameters
         ----------
         string : string
             A string containing what is to be tested.
```

### Comparing `parsevasp-3.1.0/parsevasp/incar.yml` & `parsevasp-3.2.0/parsevasp/incar.yml`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/kpoints.py` & `parsevasp-3.2.0/parsevasp/kpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Handle KPOINTS."""
-# pylint: disable=consider-using-f-string
+# pylint: disable=consider-using-f-string, disable=too-many-lines
 import io
 import sys
 
 import numpy as np
 
 from parsevasp import utils
 from parsevasp.base import BaseParser
@@ -168,14 +168,15 @@
         in order to be able to keep the input methods as clean as posible.
 
         """
 
         comment = kpoints[0].replace('#', '').strip()
         num_kpoints = int(kpoints[1].split()[0])
         divisions = None
+        generating_vectors = None
         shifts = None
         tetra = None
         tetra_vol = None
         points = None
         automatic = False
         line_mode = False
         centering = None
@@ -232,14 +233,20 @@
                 if third_line_char == 'g':
                     centering = 'Gamma'
                 else:
                     centering = 'Monkhorst-Pack'
                 divisions = [int(element) for element in kpoints[3].split()]
                 if len(kpoints) == 5:
                     shifts = [float(element) for element in kpoints[4].split()]
+            elif third_line_char == 'r':
+                centering = 'Reciprocal'
+                generating_vectors = []
+                for line_no in range(3, 6):
+                    generating_vectors.append([float(element) for element in kpoints[line_no].split()])
+                shifts = [float(element) for element in kpoints[6].split()]
             elif third_line_char in ('d', 'c'):
                 self._logger.error(self.ERROR_MESSAGES[self.ERROR_NO_EXPERT])
                 sys.exit(self.ERROR_NO_EXPERT)
         if line_mode:
             direct = False
             points = []
             reference = kpoints[3].split()[0][0].lower()
@@ -261,14 +268,15 @@
             mode = 'automatic'
         if line_mode:
             mode = 'line'
         # Add to dictionary
         kpoints_dict = {}
         kpoints_dict['comment'] = comment
         kpoints_dict['divisions'] = divisions
+        kpoints_dict['generating_vectors'] = generating_vectors
         kpoints_dict['shifts'] = shifts
         kpoints_dict['points'] = points
         kpoints_dict['tetra'] = tetra
         kpoints_dict['tetra_volume'] = tetra_vol
         kpoints_dict['mode'] = mode
         kpoints_dict['centering'] = centering
         kpoints_dict['num_kpoints'] = num_kpoints
@@ -318,14 +326,16 @@
                         point = self._to_direct(point)
                         self._logger.error(self.ERROR_MESSAGES[self.ERROR_CONVERSION])
                         sys.exit(self.ERROR_CONVERSION)
             if entry == 'comment':
                 self._check_comment(comment=value)
             if entry == 'divisions':
                 self._check_divisions(divisions=value)
+            if entry == 'generating_vectors':
+                self._check_generating_vectors(generating_vectors=value)
             if entry == 'shifts':
                 self._check_shifts(shifts=value)
             if entry == 'tetra':
                 self._check_tetra(tetra=value)
             if entry == 'tetra_volume':
                 self._check_tetra_volume(volume=value)
             if entry == 'centering':
@@ -377,16 +387,16 @@
             _ = self.entries
         except AttributeError:
             self._logger.error(self.ERROR_MESSAGES[self.ERROR_NO_ENTRIES])
             sys.exit(self.ERROR_NO_ENTRIES)
 
         # Check that at least divisions or points are set
         # to something else than None
-        if (self.entries['divisions'] is None) \
-           and (self.entries['points'] is None):
+        if ((self.entries['divisions'] is None) and (self.entries['points'] is None) and
+            (self.entries['generating_vectors'] is None)):
             self._logger.error(self.ERROR_MESSAGES[self.ERROR_DIVISIONS])
             sys.exit(self.ERROR_DIVISIONS)
 
     def _check_allowed_entries(self, entry):
         """
         Check the allowed values of entry.
 
@@ -588,14 +598,55 @@
                     if not isinstance(element, int):
                         self._logger.error(
                             f'{self.ERROR_MESSAGES[self.ERROR_KEY_INVALID_TYPE]} '
                             "The elements in the key 'divisions' should be integers."
                         )
                         sys.exit(self.ERROR_KEY_INVALID_TYPE)
 
+    def _check_generating_vectors(self, generating_vectors=None):
+        """
+        Check that the generating_vectors are either None or a list of three lists of three floats.
+
+        Parameters
+        ----------
+        generating_vectors : list of lists, optional
+            The reciprocal mode of generating lattice vectors to be checked.
+
+        """
+
+        if generating_vectors is None:
+            try:
+                generating_vectors = self.entries['generating_vectors']
+            except KeyError:
+                self._logger.error(
+                    f"{self.ERROR_MESSAGES[self.ERROR_NO_KEY]} The key in question is 'generating_vectors'."
+                )
+                sys.exit(self.ERROR_NO_KEY)
+        if generating_vectors is not None:
+            if not isinstance(generating_vectors, list):
+                self._logger.error(
+                    f"{self.ERROR_MESSAGES[self.ERROR_KEY_INVALID_TYPE]} The key 'generating_vectors' should be a list."
+                )
+                sys.exit(self.ERROR_KEY_INVALID_TYPE)
+            else:
+                for vec in generating_vectors:
+                    if not isinstance(vec, list):
+                        self._logger.error(
+                            f'{self.ERROR_MESSAGES[self.ERROR_KEY_INVALID_TYPE]} '
+                            "The key 'generating_vectors' should be a list of lists."
+                        )
+                        sys.exit(self.ERROR_KEY_INVALID_TYPE)
+                    for element in vec:
+                        if not isinstance(element, float):
+                            self._logger.error(
+                                f'{self.ERROR_MESSAGES[self.ERROR_KEY_INVALID_TYPE]} '
+                                "The elements in the key 'generating_vectors' should be floats."
+                            )
+                            sys.exit(self.ERROR_KEY_INVALID_TYPE)
+
     def _check_tetra(self, tetra=None):
         """
         Check that tetra are either None or a list of four integers.
 
         Parameters
         ----------
         tetra : list, optional
@@ -651,15 +702,15 @@
             try:
                 centering = self.entries['centering']
             except KeyError:
                 self._logger.error(f"{self.ERROR_MESSAGES[self.ERROR_NO_KEY]} The key in question is 'centering'.")
                 sys.exit(self.ERROR_NO_KEY)
         if centering is not None:
             # allow None
-            if not centering in ('Gamma', 'Monkhorst-Pack'):
+            if not centering in ('Gamma', 'Monkhorst-Pack', 'Reciprocal'):
                 self._logger.error(self.ERROR_MESSAGES[self.ERROR_INVALID_CENTERING])
                 sys.exit(self.ERROR_INVALID_CENTERING)
 
     def _check_num_kpoints(self, num_kpoints=None):
         """
         Check that num_kpoints is valid.
 
@@ -706,31 +757,31 @@
                 self._logger.error(self.ERROR_MESSAGES[self.ERROR_INVALID_MODE])
                 sys.exit(self.ERROR_INVALID_MODE)
 
     def _validate(self):
         """Validate the content of entries
 
         """
-
         self._check_dict()
         self._check_comment()
         self._check_points()
         self._check_centering()
         self._check_divisions()
+        self._check_generating_vectors()
         self._check_shifts()
         self._check_mode()
         self._check_num_kpoints()
         self._check_tetra()
         self._check_tetra_volume()
 
-    def _to_direct(self, point):  # pylint: disable=R0201
+    def _to_direct(self, point):
 
         return point
 
-    def _to_cart(self, point):  # pylint: disable=R0201
+    def _to_cart(self, point):
 
         return point
 
     def get(self, tag):
         """
         Return the value and comment of the entry with tag.
 
@@ -865,19 +916,27 @@
                             width=self._width
                         )
                     )
         if mode == 'automatic':
             file_handler.write('0\n')
             file_handler.write(entries['centering'] + '\n')
             divisions = entries['divisions']
-            file_handler.write(
-                '{:{width}d} {:{width}d} {:{width}d}\n'.format(
-                    divisions[0], divisions[1], divisions[2], width=self._width
+            if divisions is not None:
+                file_handler.write(
+                    '{:{width}d} {:{width}d} {:{width}d}\n'.format(
+                        divisions[0], divisions[1], divisions[2], width=self._width
+                    )
                 )
-            )
+            generating_vectors = entries['generating_vectors']
+            if generating_vectors is not None:
+                for vec in generating_vectors:
+                    file_handler.write(
+                        '{:{width}.{prec}f} {:{width}.{prec}f} '
+                        '{:{width}.{prec}f}\n'.format(vec[0], vec[1], vec[2], prec=self._prec, width=self._width)
+                    )
             shifts = entries['shifts']
             if shifts is not None:
                 file_handler.write(
                     '{:{width}.{prec}f} {:{width}.{prec}f} '
                     '{:{width}.{prec}f}\n'.format(shifts[0], shifts[1], shifts[2], prec=self._prec, width=self._width)
                 )
             else:
```

### Comparing `parsevasp-3.1.0/parsevasp/outcar.py` & `parsevasp-3.2.0/parsevasp/outcar.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/poscar.py` & `parsevasp-3.2.0/parsevasp/poscar.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,16 +219,16 @@
             unitcell[1] = [float(x) for x in poscar[3].split()]
             unitcell[2] = [float(x) for x in poscar[4].split()]
             unitcell = np.asarray(unitcell)
             # Apply scaling factor
             unitcell = scaling * unitcell
             spec = poscar[5].split()
             atoms = [int(x) for x in poscar[6].split()]
-            for i, _ in enumerate(atoms):
-                nions = nions + atoms[i]
+            for num_ions in atoms:
+                nions = nions + num_ions
             if poscar[7][0].lower() == 's':
                 selective = True
                 loopmax = 9
                 if not poscar[8][0].lower() == 'd':
                     direct = False
             if not selective:
                 if not poscar[7][0].lower() == 'd':
@@ -674,20 +674,20 @@
             if species_concat and species_concat[-1] == specie:
                 num_species[-1] = num_species[-1] + 1
             else:
                 species_concat.append(specie)
                 num_species.append(1)
         return sites, species_concat, num_species, selective, velocities, predictors
 
-    def _get_key(self, item):  # pylint: disable=R0201
+    def _get_key(self, item):
         """Key fetcher for the sorted function."""
 
         return item[0]
 
-    def _to_direct(self, position_cart, unitcell):  # pylint: disable=R0201
+    def _to_direct(self, position_cart, unitcell):
         """
         Transforms the position from cartesian to direct
         coordinates.
 
         Parameters
         ----------
         position_cart : ndarray
@@ -706,15 +706,15 @@
 
         """
 
         position = utils.cart_to_dir(position_cart, unitcell)
 
         return position
 
-    def _to_cart(self, position_dir, unitcell):  # pylint: disable=R0201
+    def _to_cart(self, position_dir, unitcell):
         """
         Transforms the position from direct to cartesian
         coordinates.
 
         Parameters
         ----------
         position : ndarray
```

### Comparing `parsevasp-3.1.0/parsevasp/stream.py` & `parsevasp-3.2.0/parsevasp/stream.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
         super().__init__(file_path=file_path, file_handler=file_handler, logger=logger)
 
         self._file_path = file_path
         self._file_handler = file_handler
         self._history = history
         self._streams = []
+        self._inverse_streams = []
         self._config = config
 
         # Check that at least file path or file handler is supplied
         if self._file_path is None and self._file_handler is None:
             self._logger.error(self.ERROR_MESSAGES[self.ERROR_USE_ONE_ARGUMENT])
             sys.exit(self.ERROR_USE_ONE_ARGUMENT)
 
@@ -61,19 +62,22 @@
         self._stream_config = self._load_config()
 
         # Now investigate the kinds of streams present in the config
         self._stream_kinds = self._set_streams()
 
         # Build list of error and warning objects and store the these as stream triggers on which
         # we will react if detected in the stream.
-        self._stream_triggers = self._build_stream_triggers()
+        self._stream_triggers, self._inverse_stream_triggers = self._build_stream_triggers()
 
         # Parse parse parse
         self._parse()
 
+        # Add inverse triggers not detected during parsing
+        self._add_inverse_triggers()
+
     def __repr__(self):
         """Define representation to list number of streams found."""
         return f'StreamScanner found {len(self._streams)} streams'
 
     def __str__(self):
         """Define a string representation for the class which can be used for reporting purposes."""
         return f"We detected {self.number_of_entries} unique {', '.join(self._stream_kinds)}'s"
@@ -114,15 +118,15 @@
         stream_config = self._load_config_from_file()
         # Then override or add new entries with the supplied entries.
         if self._config is not None:
             stream_config.update(self._config)
 
         return stream_config
 
-    def _load_config_from_file(self):  # pylint: disable=R0201
+    def _load_config_from_file(self):
         """Read the configuration of the errors and warnings from a yaml file and save it as the class method."""
 
         stream_config = None
         fname = Path(__file__).parent / 'stream.yml'
         # Read the config file
         with open(fname, 'r', encoding='utf8') as file_handler:
             stream_config = yaml.safe_load(file_handler)
@@ -143,23 +147,33 @@
         return stream_kinds
 
     def _build_stream_triggers(self):
         """Here we use the stream configs to initialize the triggers"""
 
         # Define container for the triggers
         triggers = {}
+        inverse_triggers = {}
         for stream in self._stream_kinds:
             triggers[''.join([stream.lower(), 's'])] = []
+            inverse_triggers[''.join([stream.lower(), 's'])] = []
 
         for stream in self._stream_kinds:
             for shortname, config in self._stream_config.items():
                 if config['kind'] == stream:
-                    triggers[''.join([stream.lower(), 's'])].append(VaspStream(shortname=shortname, **config))
+                    try:
+                        inverse = config['inverse']
+                    except KeyError:
+                        inverse = False
+                    if not inverse:
+                        triggers[''.join([stream.lower(), 's'])].append(VaspStream(shortname=shortname, **config))
+                    else:
+                        inverse_triggers[''.join([stream.lower(),
+                                                  's'])].append(VaspStream(shortname=shortname, **config))
 
-        return triggers
+        return triggers, inverse_triggers
 
     def _parse(self):
         """Perform the actual parsing."""
 
         if self._file_path is None and self._file_handler is None:
             return
 
@@ -180,38 +194,79 @@
 
         Parameters
         ----------
         stream : list
             A list of strings containing each line in the standard stream.
 
         """
-        # Copy the dictionary as we will use pop when we do not want history to
-        # remove items as we go
-        stream_triggers = dict(self._stream_triggers)
-        for _, line in enumerate(stream):
+        # Make sure we access all triggers
+        stream_triggers = {}
+        for kind in self._stream_kinds:
+            key = ''.join([kind.lower(), 's'])
+            stream_triggers[key] = self._stream_triggers[key]
+            stream_triggers[key].extend(self._inverse_stream_triggers[key])
+
+        # Ignore list to avoid multiple occurrences if not requested (default)
+        ignore = {}
+        for kind, _ in stream_triggers.items():
+            ignore[kind] = []
+        for _, line in enumerate(stream):  # pylint: disable=too-many-nested-blocks
             # Go though all entries in the stream triggers
-            for triggers in stream_triggers.values():
+            for kind, triggers in stream_triggers.items():
                 # Not check all the triggers of the given kind
                 for index, trigger in enumerate(triggers):
-                    trigger_record = trigger.check_line(line)
-                    if trigger_record:
-                        self._streams.append(trigger_record)
-                        if not self._history:
-                            # Pop stream trigger if we do not want the
-                            # full history of streams (e.g. multiple stream occurrences recorded)
-                            triggers.pop(index)
+                    if index not in ignore[kind]:
+                        trigger_record = trigger.check_line(line)
+                        if trigger_record is not None:
+                            if not trigger_record.inverse:
+                                # Store the streams that we trigger on and want to store.
+                                self._streams.append(trigger_record)
+                            else:
+                                # Keep track of streams detected that we trigger on, but do not want stored.
+                                self._inverse_streams.append(trigger_record.shortname)
+                            if not self._history:
+                                # Add index to avoid storing same trigger multiple times if we do not want the
+                                # full history of streams (e.g. multiple stream occurrences recorded)
+                                ignore[kind].append(index)
+
+    def _add_inverse_triggers(self):
+        """Adds the triggers that are marked as inverse and are not detected, meaning they should be
+        included in the returned streams.
+
+        """
+
+        for _, triggers in self._inverse_stream_triggers.items():
+            for trigger in triggers:
+                if trigger.shortname not in self._inverse_streams:
+                    # Only add inverse triggers if they was not detected during parsing.
+                    self._streams.append(
+                        VaspStream(
+                            trigger.shortname, trigger.kind, trigger.regex, trigger.message, trigger.suggestion,
+                            trigger.location, trigger.recover, trigger.inverse
+                        )
+                    )
 
 
 class VaspStream:  # pylint: disable=R0902
     """Class representing stream elements given by VASP that we want to trigger on."""
 
     _ALLOWED_STREAMS = ['ERROR', 'WARNING']
     _ALLOWED_LOCATIONS = ['STDOUT', 'STDERR']
 
-    def __init__(self, shortname, kind, regex, message, suggestion=None, location='STDOUT', recover=False):  # pylint: disable=too-many-arguments
+    def __init__(
+        self,
+        shortname,
+        kind,
+        regex,
+        message,
+        suggestion=None,
+        location='STDOUT',
+        recover=False,
+        inverse=False
+    ):  # pylint: disable=too-many-arguments
         """
         Initialise a VaspStream object.
 
         Paramters
         ---------
         shortname : string
             A short and unique string that identifies the stream
@@ -223,30 +278,36 @@
             Message to the user.
         suggestion : string, optional
             String containing a suggestion on how to address the stream message. Defaults to None.
         location : string, optional
             The location of the stream (typically STDOUT or STDERR). Defaults to STDOUT.
         recover : bool, optional
             True if the stream indicates that we are able to recover using some measures. Defaults to False.
+        inverse : bool, optional
+            If True, the stream should only be triggered on if we do not detect it.
 
         """
         self.shortname = shortname
         self.kind = kind
         if isinstance(regex, str):
             self.regex = re.compile(regex)
         else:
             self.regex = regex
         self.message = message
         self.suggestion = suggestion
         self.location = location
         self.recover = recover
+        self.inverse = inverse
 
     def __repr__(self):
         """Set the representation."""
-        return f'VaspStream(kind={self.kind}, re={self.regex}, message={self.message}, recover={self.recover})'
+        return (
+            f'VaspStream(kind={self.kind}, re={self.regex}, message={self.message}, '
+            f'recover={self.recover}, inverse={self.inverse})'
+        )
 
     def __str__(self):
         """Set string representation of the stream entry that can be used in a human readable report."""
         return f'({self.kind}) {self.shortname}: {self.message}'
 
     @property
     def shortname(self):
@@ -312,52 +373,63 @@
 
     @suggestion.setter
     def suggestion(self, sug):
         """Setter for the suggestion which validated if it is a string."""
         if sug is not None:
             # Allow None
             if not isinstance(sug, str):
-                raise ValueError(f'The suggestion entry for {self._shortname} is not of type string.')
+                raise ValueError(f'The suggestion entry {sug} is not of type string.')
         self._suggestion = sug
 
     @property
     def location(self):
         """Return the location of the stream."""
         return self._location
 
     @location.setter
     def location(self, loc):
         """Setter for the location that validates if it is an allowed value."""
         if not loc in self._ALLOWED_LOCATIONS:
-            raise ValueError(
-                f'The location entry for {self._shortname} is not one o fthe allowed values {self._ALLOWED_LOCATIONS}'
-            )
+            raise ValueError(f'The location entry {loc} is not one of the allowed values {self._ALLOWED_LOCATIONS}')
         self._location = loc
 
     @property
     def recover(self):
         """Return the recover status."""
         return self._recover
 
     @recover.setter
     def recover(self, rec):
         """Setter for the recover that validates if it is a boolean."""
         if not isinstance(rec, bool):
-            raise ValueError('The recover entry for {self._shortname is not of type string.}')
+            raise ValueError(f'The recover entry {rec} is not of type bool.')
         self._recover = rec
 
     @property
     def recoverable(self):
         """True if the stream is marked as recoverable."""
         return self._recover
 
+    @property
+    def inverse(self):
+        """Return the inverse status."""
+        return self._inverse
+
+    @inverse.setter
+    def inverse(self, inv):
+        """Setter for the inverse that validates if it is a boolean."""
+        if not isinstance(inv, bool):
+            raise ValueError(f'The recover entry {inv} is not of type bool.')
+        self._inverse = inv
+
     def check_line(self, line):
         """Check the stream in a line, return True the stream is found"""
         mch = self.regex.search(line)
         if mch:
             # Make a new instance for this particular error (in case we want
             # to save each and every error)
             return VaspStream(
-                self.shortname, self.kind, self.regex, self.message, self.suggestion, self.location, self.recover
+                self.shortname, self.kind, self.regex, self.message, self.suggestion, self.location, self.recover,
+                self.inverse
             )
 
         return None
```

### Comparing `parsevasp-3.1.0/parsevasp/stream.yml` & `parsevasp-3.2.0/parsevasp/stream.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,186 +1,195 @@
 # File containing the definition of different streams that VASP generate.
 # Each key is an unique short name of the error
 # kind: What kind of stream is it (ERROR/WARNING)
-# regex: The string printed by VASP (what we search for when we parse the stream)
+# regex: The string printed by VASP (what we search for when we parse the stream line by line)
 # message: A human readable interpretation of the regex
 # suggestion: A human readable suggestion on how to act
 # location: Can be found in which stream (STDOUT/STDERR)
 # recover: If False, always break when this error appears, there is no point in recovering
 
+# This is a special one we use to detect if VASP have not been started
+nostart:
+  kind: ERROR
+  location: STDOUT
+  message: "VASP has not been started."
+  recover: false
+  regex: "vasp."
+  inverse: True
+  suggestion: ""
 # There can be multiple IBZKPT errors, some are actually warnings but all printed as "internal error...."
-# Here I let recover=True since if it is the fatal ones VASP do stop execution.
+# Here we let recover=True since if it is the fatal ones VASP do stop execution.
 ibzkpt:
   kind: ERROR
   location: STDOUT
-  message: Error with the k-points
+  message: "Error with the k-points."
   recover: true
-  regex: internal error in subroutine IBZKPT
-  suggestion: ''
+  regex: "internal error in subroutine IBZKPT"
+  suggestion: ""
 brmix:
   kind: ERROR
   location: STDOUT
-  message: Error in BRMIX
+  message: "Error in BRMIX."
   recover: false
-  regex: 'BRMIX: very serious problems'
-  suggestion: ''
+  regex: "BRMIX: very serious problems"
+  suggestion: ""
 cnormn:
   kind: ERROR
   location: STDOUT
-  message: Error in CNORMN
+  message: "Error in CNORMN."
   recover: false
-  regex: 'WARNING: CNORMN'
-  suggestion: ''
+  regex: "WARNING: CNORMN"
+  suggestion: ""
 denmp:
   kind: ERROR
   location: STDOUT
-  message: Error in DENMP
+  message: "Error in DENMP."
   recover: false
-  regex: 'WARNING: DENMP: can''t reach specified precision'
-  suggestion: ''
+  regex: "WARNING: DENMP: can't reach specified precision"
+  suggestion: ""
 dentet:
   kind: ERROR
   location: STDOUT
-  message: Error with DENTET
+  message: "Error with DENTET."
   recover: false
-  regex: 'WARNING: DENTET'
-  suggestion: ''
+  regex: "WARNING: DENTET"
+  suggestion: ""
 edddav_zhegv:
   kind: ERROR
   location: STDOUT
-  message: Error in ZHEGV from EDDAV
+  message: "Error in ZHEGV from EDDAV."
   recover: false
-  regex: 'Error EDDDAV: Call to ZHEGV failed'
-  suggestion: ''
+  regex: "Error EDDDAV: Call to ZHEGV failed"
+  suggestion: ""
 eddrmm_zhegv:
   kind: ERROR
   location: STDOUT
-  message: Error in EDDRMM
+  message: "Error in EDDRMM."
   recover: false
-  regex: 'WARNING in EDDRMM: call to ZHEGV failed'
-  suggestion: ''
+  regex: "WARNING in EDDRMM: call to ZHEGV failed"
+  suggestion: ""
 edwav:
   kind: ERROR
   location: STDOUT
-  message: Error in EDWAV
+  message: "Error in EDWAV."
   recover: false
-  regex: 'EDWAV: internal error'
-  suggestion: ''
+  regex: "EDWAV: internal error"
+  suggestion: ""
 fexcp:
   kind: ERROR
   location: STDOUT
-  message: Error in FEXCP
+  message: "Error in FEXCP."
   recover: false
-  regex: 'ERROR FEXCP: supplied Exchange'
-  suggestion: ''
+  regex: "ERROR FEXCP: supplied Exchange"
+  suggestion: ""
 fock_acc:
   kind: ERROR
   location: STDERR
-  message: Error in FOCK_ACC
+  message: "Error in FOCK_ACC."
   recover: false
-  regex: internal error in FOCK_ACC
-  suggestion: ''
+  regex: "internal error in FOCK_ACC"
+  suggestion: ""
 invgrp:
   kind: ERROR
   location: STDOUT
-  message: Error in INVGRP
+  message: "Error in INVGRP."
   recover: false
-  regex: internal error in subroutine INVGRP
-  suggestion: ''
+  regex: "internal error in subroutine INVGRP"
+  suggestion: ""
 kpoints_trans:
   kind: ERROR
   location: STDERR
-  message: Error in GENERATE_KPOINTS_TRANS
+  message: "Error in GENERATE_KPOINTS_TRANS."
   recover: false
-  regex: internal error in GENERATE_KPOINTS_TRANS
-  suggestion: ''
+  regex: "internal error in GENERATE_KPOINTS_TRANS"
+  suggestion: ""
 non_collinear:
   kind: ERROR
   location: STDOUT
-  message: Using a collinear spin executable for a non-colinear calculation
+  message: "Using a collinear spin executable for a non-colinear calculation."
   recover: false
-  regex: 'ERROR: non collinear calculations require'
+  regex: "ERROR: non collinear calculations require"
   suggestion: Please make sure to use the VASP executable that has been compiled with the non-colinear functionality (ncl flavor, consult build instructions)
 not_hermitian:
   kind: ERROR
   location: STDOUT
-  message: Sub-space matrix not Hermitian in DAV
+  message: "Sub-space matrix not Hermitian in DAV."
   recover: false
-  regex: not Hermitian in DAV
-  suggestion: ''
+  regex: "not Hermitian in DAV"
+  suggestion: ""
 psmaxn:
   kind: ERROR
   location: STDOUT
-  message: Error in PSMAXN
+  message: "Error in PSMAXN."
   recover: false
-  regex: PSMAXN for non-local potential too small
-  suggestion: ''
+  regex: "PSMAXN for non-local potential too small"
+  suggestion: ""
 pssyevx:
   kind: ERROR
   location: STDOUT
-  message: Error in PSSYEVX
+  message: "Error in PSSYEVX."
   recover: false
-  regex: Error in subspace rotation PSSYEVX
-  suggestion: ''
+  regex: "Error in subspace rotation PSSYEVX"
+  suggestion: ""
 pzstein:
   kind: ERROR
   location: STDOUT
-  message: Error in PZSETIN
+  message: "Error in PZSETIN"
   recover: false
-  regex: PZSTEIN parameter number had an illegal value
-  suggestion: ''
+  regex: "PZSTEIN parameter number had an illegal value"
+  suggestion: ""
 real_optlay:
   kind: ERROR
   location: STDOUT
-  message: Error in REAL_OPTLAY
+  message: "Error in REAL_OPTLAY."
   recover: false
-  regex: 'REAL_OPTLAY: internal error'
-  suggestion: ''
+  regex: "REAL_OPTLAY: internal error"
+  suggestion: ""
 rhosyg:
   kind: ERROR
   location: STDOUT
-  message: Error in RHOSYG
+  message: "Error in RHOSYG"
   recover: false
-  regex: 'RHOSYG: internal error'
-  suggestion: ''
+  regex: "RHOSYG: internal error"
+  suggestion: ""
 rspher:
   kind: ERROR
   location: STDOUT
   message: Error in RSPHER
   recover: false
-  regex: Internal ERROR RSPHER
-  suggestion: ''
+  regex: "Internal ERROR RSPHER."
+  suggestion: ""
 set_indpw_full:
   kind: ERROR
   location: STDOUT
-  message: 'Error in INDPW: insufficient memory'
+  message: "Error in INDPW: insufficient memory."
   recover: false
-  regex: 'internal error in SET_INDPW_FULL: insufficient'
-  suggestion: ''
+  regex: "internal error in SET_INDPW_FULL: insufficient"
+  suggestion: ""
 sgrcon:
   kind: ERROR
   location: STDOUT
-  message: Error in SGRCON
+  message: "Error in SGRCON"
   recover: false
-  regex: internal error in subroutine SGRCON
-  suggestion: ''
+  regex: "internal error in subroutine SGRCON"
+  suggestion: ""
 no_potim:
   kind: ERROR
   location: STDOUT
-  message: NSW specified, but no POTIM or IBRION set
+  message: "NSW specified, but no POTIM or IBRION set."
   recover: false
-  regex: 'Fatal error! IBRION=0, but no entry for POTIM on file INCAR. MUST be specified!!'
-  suggestion: ''
+  regex: "Fatal error! IBRION=0, but no entry for POTIM on file INCAR. MUST be specified!!"
+  suggestion: ""
 magmom:
   kind: ERROR
   location: STDOUT
-  message: MAGMON is specified, but ISPIN is set to one
+  message: "MAGMON is specified, but ISPIN is set to one."
   recover: false
   regex: "Error reading item 'MAGMOM' from file INCAR"
-  suggestion: ''
+  suggestion: ""
 bandocc:
   kind: ERROR
   location: STDOUT
-  message: The topmost band is occupied.
+  message: "The topmost band is occupied."
   recover: false
   regex: "TOO FEW BANDS"
-  suggestion: ''
+  suggestion: ""
```

### Comparing `parsevasp-3.1.0/parsevasp/utils.py` & `parsevasp-3.2.0/parsevasp/utils.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.1.0/parsevasp/vasprun.py` & `parsevasp-3.2.0/parsevasp/vasprun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1137,15 +1137,16 @@
 
         Notes
         -----
         Used when detecting symmetry.
 
         """
 
-        entry = self._find(xml, './/parameters/separator[@name="symmetry"]/' 'i[@name="SYMPREC"]')
+        entry = self._find(xml, './/parameters/separator[@name="symmetry"]/'
+                           'i[@name="SYMPREC"]')
 
         if entry is None:
             return None
 
         symprec = self._convert_f(entry)
 
         return symprec
@@ -1233,15 +1234,16 @@
 
         Notes
         -----
         Maximum number of eletronic steps. This is needed for checking ionic convergence.
 
         """
 
-        entry = self._find(xml, './/parameters/separator[@name="ionic"]/' 'i[@name="NSW"]')
+        entry = self._find(xml, './/parameters/separator[@name="ionic"]/'
+                           'i[@name="NSW"]')
 
         if entry is None:
             return None
 
         nsw = self._convert_i(entry)
 
         return nsw
@@ -1327,15 +1329,16 @@
 
         Notes
         -----
         The number of bands used in the calculation.
 
         """
 
-        entry = self._find(xml, './/parameters/separator[@name="electronic"]/' 'i[@name="NBANDS"]')
+        entry = self._find(xml, './/parameters/separator[@name="electronic"]/'
+                           'i[@name="NBANDS"]')
         if entry is None:
             return None
 
         nbands = self._convert_i(entry)
 
         return nbands
 
@@ -1355,15 +1358,16 @@
 
         Notes
         -----
         The number of electrons used in the calculation.
 
         """
 
-        entry = self._find(xml, './/parameters/separator[@name="electronic"]/' 'i[@name="NELECT"]')
+        entry = self._find(xml, './/parameters/separator[@name="electronic"]/'
+                           'i[@name="NELECT"]')
 
         if entry is None:
             return None
 
         nelect = self._convert_f(entry)
 
         return nelect
@@ -1384,15 +1388,16 @@
 
         Notes
         -----
         A comment that can be specified in the INCAR file.
 
         """
 
-        entry = self._find(xml, './/parameters/separator[@name="general"]/' 'i[@name="SYSTEM"]')
+        entry = self._find(xml, './/parameters/separator[@name="general"]/'
+                           'i[@name="SYSTEM"]')
 
         if entry is None:
             return None
 
         system = entry.text
 
         return system
@@ -1410,15 +1415,16 @@
         -------
         born : ndarray
             A ndarray containing the born effective charge
             tensor for each atom.
 
         """
 
-        entry = self._findall(xml, './/calculation/array[@name="born_charges"]/' 'set/v')
+        entry = self._findall(xml, './/calculation/array[@name="born_charges"]/'
+                              'set/v')
 
         if entry is None:
             return None
 
         num_atoms = 0
         species = self._lattice['species']
         if species is None:
@@ -1619,15 +1625,16 @@
         -------
         spec : ndarray
             An array containing the atomic species as a number.
             Organized in the same order as the atomic positions.
 
         """
 
-        entry = self._findall(xml, './/atominfo/' 'array[@name="atoms"]/set/rc/c')
+        entry = self._findall(xml, './/atominfo/'
+                              'array[@name="atoms"]/set/rc/c')
 
         if entry is None:
             return None
 
         spec = self._convert_species(entry[::2])
 
         return spec
@@ -1644,15 +1651,16 @@
         Returns
         -------
         hessian : ndarray
             An array containing the Hessian matrix.
 
         """
 
-        entry = self._findall(xml, './/calculation/dynmat/' 'varray[@name="hessian"]/v')
+        entry = self._findall(xml, './/calculation/dynmat/'
+                              'varray[@name="hessian"]/v')
 
         if entry is None:
             return None
 
         species = self._lattice['species']
         if species is None:
             # Try to fetch species again, if still none, we cannot parse it
@@ -1678,15 +1686,16 @@
         Returns
         -------
         dynmat : dict
             An dict containing the eigenvalues and eigenvectors.
 
         """
 
-        entry = self._find(xml, './/calculation/dynmat/' 'v[@name="eigenvalues"]')
+        entry = self._find(xml, './/calculation/dynmat/'
+                           'v[@name="eigenvalues"]')
 
         if entry is None:
             return None
 
         species = self._lattice['species']
         if species is None:
             # Try to fetch species again, if still none, we cannot parse it
@@ -1694,15 +1703,16 @@
             species = self._fetch_speciesw(xml)
             if species is None:
                 return None
         num_atoms = species.shape[0]
 
         eigenvalues = self._convert_array_f(entry)
 
-        entry = self._find(xml, './/calculation/dynmat/' 'varray[@name="eigenvectors"]')
+        entry = self._find(xml, './/calculation/dynmat/'
+                           'varray[@name="eigenvectors"]')
 
         if entry is None:
             return None
 
         eigenvectors = self._convert_array2D_f(entry, num_atoms * 3)
 
         dynmat = {'eigenvalues': eigenvalues, 'eigenvectors': eigenvectors}
@@ -1805,18 +1815,20 @@
             An tupple of dicts containing ndarrays containing the
             eigenvalues and occupancies for each spin, band and
             kpoint index.
 
         """
 
         # Spin 1
-        entry_ispin1 = self._findall(xml, './/calculation/eigenvalues/array/set/' 'set[@comment="spin 1"]/set/r')
+        entry_ispin1 = self._findall(xml, './/calculation/eigenvalues/array/set/'
+                                     'set[@comment="spin 1"]/set/r')
 
         # Spin 2
-        entry_ispin2 = self._findall(xml, './/calculation/eigenvalues/array/set/' 'set[@comment="spin 2"]/set/r')
+        entry_ispin2 = self._findall(xml, './/calculation/eigenvalues/array/set/'
+                                     'set[@comment="spin 2"]/set/r')
 
         # If we do not find spin 1 entries return right away
         if entry_ispin1 is None:
             return None, None
 
         eigenvalues, occupancies = self._extract_eigenvalues(entry_ispin1, entry_ispin2, len(self._lattice['kpoints']))
 
@@ -1939,18 +1951,20 @@
         projectors : dict
             An dict containing ndarrays of the projectors
             for each atomic, spin, band and kpoint index.
 
         """
 
         # Projectors spin 1
-        entry_ispin1 = self._findall(xml, './/calculation/projected/array/set/' 'set[@comment="spin1"]/set/set/r')
+        entry_ispin1 = self._findall(xml, './/calculation/projected/array/set/'
+                                     'set[@comment="spin1"]/set/set/r')
 
         # Projectors spin 2
-        entry_ispin2 = self._findall(xml, './/calculation/projected/array/set/' 'set[@comment="spin2"]/set/set/r')
+        entry_ispin2 = self._findall(xml, './/calculation/projected/array/set/'
+                                     'set[@comment="spin2"]/set/set/r')
 
         # If we do not find spin 1 entries return right away
         if entry_ispin1 is None:
             return None
 
         projectors = self._extract_projectors(entry_ispin1, entry_ispin2)
         return projectors
@@ -3152,20 +3166,20 @@
 
     def get_energies(self, status, etype=None, nosc=True):
         """
         Return the total energies.
 
         Paramaeters
         -----------
-        status : {'all', 'initial', 'final'}
+        status : {'all', 'initial', 'last'}
             A string containing which positions to return. For `all`, positionss for all ionic steps
-            are returned. For `initial` and `final`, the positions for the first and last ionic step
+            are returned. For `initial` and `last`, the positions for the first and last ionic step
             is returned, respectively.
-        etype : {'energy_extrapolated', 'energy_free', 'energy_no_entropy'}
-            The type of total energy to return. The `energy_extrapolated`, `energy_free` and
+        etype : list
+            A list containing the type of total energies to return. The `energy_extrapolated`, `energy_free` and
             `energy_no_entropy` transfers to `e_0_energy`, `e_fr_energy` and `energy_no_entropy`
             as printed in the XML file.
         nosc : bool
             If `True` we do not return the total energies of all the electronic steps, only the last,
             otherwise if `False`.
 
         Returns
@@ -3189,17 +3203,22 @@
         `etype` and `etype_final` not to be the same, even though no corrections
         have been applied. This has been fixed in VASP 6.
 
         """
 
         if etype is None:
             etype = ['energy_extrapolated']
+
+        if not isinstance(etype, list):
+            # The supplied etype is not a list
+            raise ValueError(f'The supplied etype: {etype} is not a list.')
+
         # Check if the supplied etype is in the support list
         for item in etype:
-            if item not in _SUPPORTED_TOTAL_ENERGIES.keys():
+            if item not in _SUPPORTED_TOTAL_ENERGIES.keys():  # pylint: disable=consider-iterating-dictionary
                 raise ValueError(f'The supplied total energy type: {item} is not supported.')
 
         return self._get_energies(status, etype, nosc)
 
     def _get_energies(self, status, etype, nosc):
         """
         Driver for the `get_energies`.
@@ -3531,15 +3550,15 @@
             self._logger.error(
                 f'{self.ERROR_MESSAGES[self.ERROR_UNSUPPORTED_STATUS]} '
                 'Please use any of the following values '
                 f'{str(allowed_entries)}'
             )
             sys.exit(self.ERROR_UNSUPPORTED_STATUS)
 
-    def _find(self, xml, locator):  # pylint: disable=R0201
+    def _find(self, xml, locator):
         """Wrapper to check if the request returns something.
 
         Parameters
         ----------
         xml : object
             An ElementTree object to be used for parsing.
         locator : string
@@ -3555,15 +3574,15 @@
 
         entry = xml.find(locator)
 
         if entry is None:
             return None
         return entry
 
-    def _findall(self, xml, locator):  # pylint: disable=R0201
+    def _findall(self, xml, locator):
         """Wrapper to check if the request returns something.
 
         Parameters
         ----------
         xml : object
             An ElementTree object to be used for parsing.
         locator : string
```

