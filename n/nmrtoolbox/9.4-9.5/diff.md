# Comparing `tmp/nmrtoolbox-9.4.tar.gz` & `tmp/nmrtoolbox-9.5.tar.gz`

## Comparing `nmrtoolbox-9.4.tar` & `nmrtoolbox-9.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/src/nmrtoolbox/__init__.py
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/src/nmrtoolbox/mask.py
--rw-r--r--   0        0        0    29234 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/src/nmrtoolbox/peak.py
--rw-r--r--   0        0        0    21611 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/src/nmrtoolbox/roc.py
--rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/src/nmrtoolbox/util.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/LICENSE
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/README.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/pyproject.toml
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 nmrtoolbox-9.4/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/src/nmrtoolbox/__init__.py
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/src/nmrtoolbox/mask.py
+-rw-r--r--   0        0        0    31740 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/src/nmrtoolbox/peak.py
+-rw-r--r--   0        0        0    21611 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/src/nmrtoolbox/roc.py
+-rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/src/nmrtoolbox/util.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/LICENSE
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/README.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/pyproject.toml
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 nmrtoolbox-9.5/PKG-INFO
```

### Comparing `nmrtoolbox-9.4/src/nmrtoolbox/mask.py` & `nmrtoolbox-9.5/src/nmrtoolbox/mask.py`

 * *Files identical despite different names*

### Comparing `nmrtoolbox-9.4/src/nmrtoolbox/peak.py` & `nmrtoolbox-9.5/src/nmrtoolbox/peak.py`

 * *Files 4% similar despite different names*

```diff
@@ -477,14 +477,16 @@
 class PeakTablePipe(PeakTable):
     def __init__(self, file, **kwargs):
         """
         This class has subclasses for peak tables coming from INJECTED and RECOVERED peak tables; use those subclasses.
         You probably don't want to create a PeakTablePipe object - it is just a super-class to provide common tasks.
         """
         # pre
+        self.REMARK = []
+        self.DATA = []
         self.VARS = None
         self.FORMAT = None
 
         try:
             super().__init__(file, **kwargs)
         except ParsePeakTableError as e:
             # raise ParsePeakTableError(e)
@@ -525,23 +527,24 @@
                         self.REMARK.append(line)
                         continue
                     else:
                         mode = 'data'
 
                 if mode == 'genSimTab':
                     if line.startswith('#'):
-                        self.genSimTab.append(line.strip().lstrip('#').rstrip('\\').strip())
+                        self.genSimTab_raw_list.append(line.strip().lstrip('#').rstrip('\\').strip())
                         continue
                     else:
                         mode = 'data'
 
                 if mode == 'data':
                     if line.startswith('DATA'):
                         # axis properties are described like this
                         # example: DATA  X_AXIS HN           1   659   10.297ppm    5.798ppm
+                        self.DATA.append(line)
                         info = line.split()
                         try:
                             if info[1] == 'CLUSTER':
                                 # some filtered peak tables include CLUSTER info - ignore these lines
                                 # example: DATA  CLUSTER X_AXIS +/- 7
                                 continue
                             elif info[1].endswith('_AXIS'):
@@ -595,20 +598,78 @@
                     else:
                         self.peaks.append(Peak(
                             prop_list=self.VARS,
                             val_list=line.split(),
                             axis_property=self.axis,
                         ))
 
+    def _build_genSimTab_comment(self):
+        """
+        convert list of genSimTab lines into a single comment string that can be written into header of peak table
+        :return:
+        """
+        try:
+            join_str = ' \\\n#' + ' ' * 15
+            return '# ' + join_str.join(self.genSimTab_raw_list)
+        except AttributeError:
+            raise AttributeError
+
+    def write(self, file):
+        """
+        write a peak table to file.  include (if available) genSimTab, REMARK, DATA, VARS, FORMAT, and peak table
+        :param file:
+        :return:
+        """
+        try:
+            with open(file, 'w') as f_out:
+                try:
+                    f_out.write(self._build_genSimTab_comment())
+                    f_out.write('\n\n')
+                except AttributeError:
+                    pass
+
+                if self.REMARK:
+                    for line in self.REMARK:
+                        f_out.write(line + '\n')
+                    f_out.write('\n')
+
+                if self.DATA:
+                    for line in self.DATA:
+                        f_out.write(line + '\n')
+                    f_out.write('\n')
+
+                # build the FORMAT and VARS lines in the same style as NMRPipe tables
+                vars_out   = 'VARS   '
+                format_out = 'FORMAT '
+                for vars_current, format_current in zip(self.VARS, self.FORMAT):
+                    width = max(len(vars_current), len(format_current))
+                    vars_out += f' {vars_current:<{width}}'
+                    format_out += f' {format_current:<{width}}'
+                f_out.write(vars_out + '\n')
+                f_out.write(format_out+ '\n')
+                f_out.write('\n')
+
+                for p in self.peaks:
+                    out = []
+                    for vars_name, format_spec in zip(self.VARS, self.FORMAT):
+                        val = p.get_par(par=vars_name)
+                        out.append(f'{val:{format_spec.lstrip("%")}}')
+                    f_out.write(' ' + ' '.join(out) + '\n')
+        except FileNotFoundError:
+            raise FileNotFoundError(f'bad file: {file}')
+        except PermissionError:
+            raise PermissionError(f'bad file: {file}')
+        except Exception as e:
+            raise Exception(e)
+
 
 class PeakTablePipeRec(PeakTablePipe):
     """This subclass is for capturing the peaks "recovered" from an experiment by the NMRPipe peak picker"""
     def __init__(self, file, **kwargs):
         # pre
-        self.REMARK = []
 
         try:
             super().__init__(file, **kwargs)
         except:
             raise ParsePeakTableError(f'failed to read peak table as type: PeakTablePipeRec\n{file}')
 
         # post
@@ -671,23 +732,24 @@
         """
 
         # could get carrier_frequency from kwargs input, but it wouldn't be a required input or autocomplete
         # want to put carrier_frequency back into kwargs, so that kwargs can be passed up to super
         kwargs['carrier_frequency'] = carrier_frequency
 
         # pre
-        self.genSimTab = []
+        # capture the lines of genSimTab command as they are formatted so they can be written to file if needed
+        self.genSimTab_raw_list = []
 
         try:
             super().__init__(file, **kwargs)
         except (ParsePeakTableError, Exception) as e:
             raise ParsePeakTableError(f'failed to read peak table as type: PeakTablePipeInj\n  table = {file}\n  error = {e}')
 
         # post
-        self.genSimTab = ' '.join(self.genSimTab)
+        self.genSimTab = ' '.join(self.genSimTab_raw_list)
         self._set_maxLW()
         self._post()
 
     def _set_maxLW(self):
         """
         #1. read LW params from genSimTab command (indirect)
         #2. compute LW from injected peak table using X1/X3 (in pts) and converting to hz
```

### Comparing `nmrtoolbox-9.4/src/nmrtoolbox/roc.py` & `nmrtoolbox-9.5/src/nmrtoolbox/roc.py`

 * *Files identical despite different names*

### Comparing `nmrtoolbox-9.4/src/nmrtoolbox/util.py` & `nmrtoolbox-9.5/src/nmrtoolbox/util.py`

 * *Files identical despite different names*

### Comparing `nmrtoolbox-9.4/LICENSE` & `nmrtoolbox-9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nmrtoolbox-9.4/README.md` & `nmrtoolbox-9.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 
 ## Changelog
 v9
 - change in internal data model for storing metadata in Peak, PeakTable, Mask, ROC, and ROI classes
 - allow roc class to accept Mask object (not just mask file)
 - approximate maximum LW for injected peaks from X1/X3, etc. parameters in the injected peak table
+- function to write NMRPipe peak table to file
 
 v8
 - change to MIT license
 - box_radius for mask filtering is multidimensional
 - improved input options for setting carrier frequency
 - axis labels used to verify compatibility of Peak, Mask, ROI, and ROC objects
```

### Comparing `nmrtoolbox-9.4/pyproject.toml` & `nmrtoolbox-9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nmrtoolbox-9.4/PKG-INFO` & `nmrtoolbox-9.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmrtoolbox
-Version: 9.4
+Version: 9.5
 Summary: simple utility for parsing and working with NMR peak tables, including ROC analysis
 Project-URL: Homepage, https://nmrbox.nmrhub.org/
 Author-email: Adam Schuyler <schuyler@uchc.edu>, D Levi Craft <darcraft@uchc.edu>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,14 +64,15 @@
 
 
 ## Changelog
 v9
 - change in internal data model for storing metadata in Peak, PeakTable, Mask, ROC, and ROI classes
 - allow roc class to accept Mask object (not just mask file)
 - approximate maximum LW for injected peaks from X1/X3, etc. parameters in the injected peak table
+- function to write NMRPipe peak table to file
 
 v8
 - change to MIT license
 - box_radius for mask filtering is multidimensional
 - improved input options for setting carrier frequency
 - axis labels used to verify compatibility of Peak, Mask, ROI, and ROC objects
```

