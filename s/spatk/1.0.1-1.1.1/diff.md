# Comparing `tmp/spatk-1.0.1.tar.gz` & `tmp/spatk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatk-1.0.1.tar", last modified: Fri May 19 11:40:12 2023, max compression
+gzip compressed data, was "spatk-1.1.1.tar", last modified: Mon Jun  5 14:01:21 2023, max compression
```

## Comparing `spatk-1.0.1.tar` & `spatk-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-05-19 11:40:12.074137 spatk-1.0.1/
--rw-r--r--   0 christoph  (1000) christoph  (1000)    35149 2017-09-30 07:16:26.000000 spatk-1.0.1/LICENSE
--rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-05-19 11:40:12.074137 spatk-1.0.1/PKG-INFO
--rw-r--r--   0 christoph  (1000) christoph  (1000)      564 2023-05-19 11:37:54.000000 spatk-1.0.1/README.md
--rw-r--r--   0 christoph  (1000) christoph  (1000)      713 2023-05-19 11:39:39.000000 spatk-1.0.1/pyproject.toml
--rw-r--r--   0 christoph  (1000) christoph  (1000)       38 2023-05-19 11:40:12.074137 spatk-1.0.1/setup.cfg
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-05-19 11:40:12.074137 spatk-1.0.1/spatk/
--rw-r--r--   0 christoph  (1000) christoph  (1000)      840 2023-05-19 09:26:30.000000 spatk-1.0.1/spatk/__init__.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     9492 2023-05-19 10:25:03.000000 spatk-1.0.1/spatk/circuit.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     2657 2023-05-19 09:26:49.000000 spatk-1.0.1/spatk/elements.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     6019 2023-05-19 10:23:26.000000 spatk-1.0.1/spatk/genelems.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)    13866 2023-05-19 08:47:55.000000 spatk-1.0.1/spatk/helems.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     9667 2023-04-12 18:59:09.000000 spatk-1.0.1/spatk/helpers.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)    13772 2023-05-19 09:34:24.000000 spatk-1.0.1/spatk/ngelems.py
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-05-19 11:40:12.074137 spatk-1.0.1/spatk.egg-info/
--rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-05-19 11:40:12.000000 spatk-1.0.1/spatk.egg-info/PKG-INFO
--rw-r--r--   0 christoph  (1000) christoph  (1000)      317 2023-05-19 11:40:12.000000 spatk-1.0.1/spatk.egg-info/SOURCES.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)        1 2023-05-19 11:40:12.000000 spatk-1.0.1/spatk.egg-info/dependency_links.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)       14 2023-05-19 11:40:12.000000 spatk-1.0.1/spatk.egg-info/requires.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)        6 2023-05-19 11:40:12.000000 spatk-1.0.1/spatk.egg-info/top_level.txt
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-05-19 11:40:12.074137 spatk-1.0.1/tests/
--rw-r--r--   0 christoph  (1000) christoph  (1000)    24272 2023-05-19 10:33:40.000000 spatk-1.0.1/tests/test_spatk.py
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.309777 spatk-1.1.1/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    35149 2017-09-30 07:16:26.000000 spatk-1.1.1/LICENSE
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-06-05 14:01:21.309777 spatk-1.1.1/PKG-INFO
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      564 2023-05-19 11:37:54.000000 spatk-1.1.1/README.md
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      713 2023-06-05 14:00:25.000000 spatk-1.1.1/pyproject.toml
+-rw-r--r--   0 christoph  (1000) christoph  (1000)       38 2023-06-05 14:01:21.309777 spatk-1.1.1/setup.cfg
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.305777 spatk-1.1.1/spatk/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      840 2023-05-19 09:26:30.000000 spatk-1.1.1/spatk/__init__.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     9645 2023-06-05 13:59:05.000000 spatk-1.1.1/spatk/circuit.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     2663 2023-06-05 13:59:05.000000 spatk-1.1.1/spatk/elements.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     6019 2023-05-19 10:23:26.000000 spatk-1.1.1/spatk/genelems.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    13866 2023-05-19 08:47:55.000000 spatk-1.1.1/spatk/helems.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     9667 2023-04-12 18:59:09.000000 spatk-1.1.1/spatk/helpers.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    15389 2023-06-05 13:59:05.000000 spatk-1.1.1/spatk/ngelems.py
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.309777 spatk-1.1.1/spatk.egg-info/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/PKG-INFO
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      317 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/SOURCES.txt
+-rw-r--r--   0 christoph  (1000) christoph  (1000)        1 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/dependency_links.txt
+-rw-r--r--   0 christoph  (1000) christoph  (1000)       14 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/requires.txt
+-rw-r--r--   0 christoph  (1000) christoph  (1000)        6 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/top_level.txt
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.309777 spatk-1.1.1/tests/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    24543 2023-06-05 13:59:05.000000 spatk-1.1.1/tests/test_spatk.py
```

### Comparing `spatk-1.0.1/LICENSE` & `spatk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spatk-1.0.1/PKG-INFO` & `spatk-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatk
-Version: 1.0.1
+Version: 1.1.1
 Summary: Module for handling and analyzing spice netlists
 Author: Christoph Weiser
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `spatk-1.0.1/README.md` & `spatk-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spatk-1.0.1/pyproject.toml` & `spatk-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spatk"
-version = "1.0.1"
+version = "1.1.1"
 description = "Module for handling and analyzing spice netlists"
 readme = "README.md"
 authors = [{ name = "Christoph Weiser"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `spatk-1.0.1/spatk/__init__.py` & `spatk-1.1.1/spatk/__init__.py`

 * *Files identical despite different names*

### Comparing `spatk-1.0.1/spatk/circuit.py` & `spatk-1.1.1/spatk/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,17 @@
         else:
             self.name = "Netlist"
             self._netlist = []
 
         self.parsed_circuit = self.parse(self._netlist)
         self.circuit = copy.deepcopy(self.parsed_circuit)
         self._synthesize()
+        self._asign_attributes()
 
+    def _asign_attributes(self):
         for elem in elementmap.values():
             if elem:
                 elemname = (elem.__name__).lower()
                 setattr(self, "{}s".format(elemname), self._attr(elem))
 
 
     def __str__(self):
@@ -212,24 +214,26 @@
     def append(self, line):
         """ Append an element to the Circuit.
 
         Required inputs:
         ----------------
         line (str):     SPICE netlist line.
         """
+        line = clean_netlist(line)
         parsed = self.parse(line)
         last = list(self.circuit.keys())[-1]
         if last:
             n = self.circuit[last].n + 1
         else:
             n = 0
         for i, uid_parsed in enumerate(parsed):
-            uid = get_uid(line, i)
+            uid = get_uid(parsed[uid_parsed].line, i)
             parsed[uid_parsed].n = n + i
             self.circuit[uid] = parsed[uid_parsed]
+        self._asign_attributes()
 
 
     def write(self, filename):
         """ Write the netlist to file
 
         Optional inputs:
         ----------------
```

### Comparing `spatk-1.0.1/spatk/elements.py` & `spatk-1.1.1/spatk/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                             Comment)
 
 if SYNTAX == "ngspice":
 
     from spatk.ngelems import elementmap
     from spatk.ngelems import process_statement, identify_linetype
     from spatk.ngelems import (Model, Include, Library,
-                               Option, Function, Param,
+                               Option, Function, Temp, Param,
                                Global, Xspice, Behavioral_source,
                                Capacitor, Diode, Vcvs, Cccs,
                                Vccs, Ccvs, Isource, Jfet,
                                Inductor, Mosfet, Numerical_device_gss,
                                Lossy_transmission_line, Bjt,
                                Resistor, Vcsw, Lossless_transmission_line,
                                Uniformely_distributed_rc_line,
```

### Comparing `spatk-1.0.1/spatk/genelems.py` & `spatk-1.1.1/spatk/genelems.py`

 * *Files identical despite different names*

### Comparing `spatk-1.0.1/spatk/helems.py` & `spatk-1.1.1/spatk/helems.py`

 * *Files identical despite different names*

### Comparing `spatk-1.0.1/spatk/helpers.py` & `spatk-1.1.1/spatk/helpers.py`

 * *Files identical despite different names*

### Comparing `spatk-1.0.1/spatk/ngelems.py` & `spatk-1.1.1/spatk/ngelems.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,27 @@
 
 class Function(Statement):
     """ .func Statement. """
     def __init__(self, *args):
         super(Function, self).__init__(*args)
 
 
+class Temp(Statement):
+    """ .temp Statement. """
+    def __init__(self, *args):
+        super(Temp, self).__init__(*args)
+
+    @property
+    def value(self):
+        return self.elements[1]
+
+    @value.setter
+    def value(self, arg):
+        self.elements[1] = str(arg)
+
 class Param(Statement):
     """ .param Statement. """
     def __init__(self, *args):
         super(Param, self).__init__(*args)
 
     @property
     def value(self):
@@ -248,14 +261,31 @@
         self.argsdata = arg
 
 class Isource(Component_2T):
     """ I - Current Source. """
     def __init__(self, *args):
         super(Isource, self).__init__(*args)
 
+    def parse(self, elements):
+        if len(elements) == 4:
+            super(Isource, self).parse(elements)
+        else:
+            var_source = False
+            types = ["dc", "ac", "pulse", "exp", "pwl", 
+                     "sffm", "am", "trnoise", "trrandom"] 
+            for t in types:
+                if t in elements[3]:
+                    var_source = True
+            if var_source:
+                self.ports = self._assign_ports(elements[1:3])
+                self.value = " ".join(elements[3:])
+                self.argsdata = None
+            else:
+                super(Isource, self).parse(elements)
+
     @property
     def current(self):
         return self.value
 
     @current.setter
     def current(self, arg):
         self.value = arg
@@ -391,14 +421,31 @@
 
 
 class Vsource(Component_2T):
     """ V - Voltage Source. """
     def __init__(self, *args):
         super(Vsource, self).__init__(*args)
 
+    def parse(self, elements):
+        if len(elements) == 4:
+            super(Vsource, self).parse(elements)
+        else:
+            var_source = False
+            types = ["dc", "ac", "pulse", "exp", "pwl", 
+                     "sffm", "am", "trnoise", "trrandom"] 
+            for t in types:
+                if t in elements[3]:
+                    var_source = True
+            if var_source:
+                self.ports = self._assign_ports(elements[1:3])
+                self.value = " ".join(elements[3:])
+                self.argsdata = None
+            else:
+                super(Vsource, self).parse(elements)
+
     @property
     def voltage(self):
         return self.value
 
     @voltage.setter
     def voltage(self, arg):
         self.value = arg
@@ -442,14 +489,15 @@
 elementmap = {"*":          Comment,
               ".":          Statement,
               "model":      Model,
               "include":    Include,
               "library":    Library,
               "option":     Option,
               "function":   Function,
+              "temp":       Temp,
               "param":      Param,
               "global":     Global,
               "A":          Xspice,
               "B":          Behavioral_source,
               "C":          Capacitor,
               "D":          Diode,
               "E":          Vcvs,
@@ -503,14 +551,16 @@
         return "model"
     elif identifier in [".option"]:
         return "option"
     elif identifier in [".func", ".function"]:
         return "function"
     elif identifier in [".global"]:
         return "global"
+    elif identifier in [".temp"]:
+        return "temp"
     elif identifier in [".par", ".param"]:
         return "param"
     else:
         return "."
 
 
 def identify_linetype(line):
```

### Comparing `spatk-1.0.1/spatk.egg-info/PKG-INFO` & `spatk-1.1.1/spatk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatk
-Version: 1.0.1
+Version: 1.1.1
 Summary: Module for handling and analyzing spice netlists
 Author: Christoph Weiser
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `spatk-1.0.1/tests/test_spatk.py` & `spatk-1.1.1/tests/test_spatk.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,14 +174,27 @@
     "uid"       : "testuid",
     "mod"       : spe.Function,
     "instance"  : None,
     "type"      : "function",
     "value"     : None,
     "ports"     : dict(),
 },
+"temp":
+{
+    "line"      : ".temp 20",
+    "loc"       : "root",
+    "lib"       : None,
+    "n"         : 1,
+    "uid"       : "testuid",
+    "mod"       : spe.Temp,
+    "instance"  : None,
+    "type"      : "temp",
+    "value"     : "20",
+    "ports"     : dict(),
+},
 "param":
 {
     "line"      : ".param mypar='value'",
     "loc"       : "root",
     "lib"       : None,
     "n"         : 1,
     "uid"       : "testuid",
```

