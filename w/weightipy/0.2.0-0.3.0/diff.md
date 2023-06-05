# Comparing `tmp/weightipy-0.2.0.tar.gz` & `tmp/weightipy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weightipy-0.2.0.tar", last modified: Sat Jun  3 20:46:39 2023, max compression
+gzip compressed data, was "weightipy-0.3.0.tar", last modified: Mon Jun  5 14:03:15 2023, max compression
```

## Comparing `weightipy-0.2.0.tar` & `weightipy-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:39.924743 weightipy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-03 20:46:28.000000 weightipy-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:28.000000 weightipy-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-03 20:46:39.924743 weightipy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-03 20:46:28.000000 weightipy-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 20:46:39.924743 weightipy-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-03 20:46:28.000000 weightipy-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:39.924743 weightipy-0.2.0/weightipy/
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26240 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/rim.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/weight_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:39.924743 weightipy-0.2.0/weightipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:15.310465 weightipy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-05 14:02:55.000000 weightipy-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:55.000000 weightipy-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-05 14:03:15.310465 weightipy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-05 14:02:55.000000 weightipy-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-05 14:03:15.310465 weightipy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-05 14:02:55.000000 weightipy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:15.310465 weightipy-0.3.0/weightipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-05 14:02:55.000000 weightipy-0.3.0/weightipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26766 2023-06-05 14:02:55.000000 weightipy-0.3.0/weightipy/rim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 14:02:55.000000 weightipy-0.3.0/weightipy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-05 14:02:55.000000 weightipy-0.3.0/weightipy/weight_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:15.310465 weightipy-0.3.0/weightipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-05 14:03:15.000000 weightipy-0.3.0/weightipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-05 14:03:15.000000 weightipy-0.3.0/weightipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:03:15.000000 weightipy-0.3.0/weightipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 14:03:15.000000 weightipy-0.3.0/weightipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 14:03:15.000000 weightipy-0.3.0/weightipy.egg-info/top_level.txt
```

### Comparing `weightipy-0.2.0/LICENSE.txt` & `weightipy-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weightipy-0.2.0/setup.py` & `weightipy-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             if lib in versions.keys() else lib
             for lib in libs]
 
 
 INSTALL_REQUIRES = version_libs(libs, precisions, versions)
 
 setup(name='weightipy',
-      version='0.2.0',
+      version='0.3.0',
       author='Remi Sebastian Kits',
       author_email='kaitumisuuringute.keskus@gmail.com',
       packages=find_packages(exclude=['tests']),
       include_package_data=True,
       install_requires=INSTALL_REQUIRES,
       long_description=long_description,
       long_description_content_type='text/markdown'
```

### Comparing `weightipy-0.2.0/weightipy/rim.py` & `weightipy-0.3.0/weightipy/rim.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,19 @@
                  name,
                  max_iterations=1000,
                  convcrit=0.01,
                  cap=0,
                  dropna=True,
                  impute_method="mean",
                  weight_column_name=None,
-                 total=0):
+                 total=0,
+                 verbose=False):
 
         # Default var init
+        self.verbose = verbose
         self.name = name
         self.type = "Rim"
         self.target_cols = []
         self.max_iterations = max_iterations
         self.convcrit = convcrit
         self.cap = cap
         self.weight_column_name = weight_column_name
@@ -173,15 +175,17 @@
             wdf[wgt] = 1
             rake = Rake(wdf,
                         self.groups[group][self._TARGETS],
                         self._weight_name(),
                         max_iterations = self.max_iterations,
                         _use_cap=self._use_cap(),
                         cap=self.cap,
-                        anesrake_cap_correction=self.anesrake_cap_correction)
+                        anesrake_cap_correction=self.anesrake_cap_correction,
+                        verbose=self.verbose
+            )
             self.groups[group][self._ITERATIONS_] = rake.start()
             self._df.loc[rake.dataframe.index, wgt] = rake.dataframe[wgt]
             self.groups[group][self._REPORT] = rake.report
         invalid_idx = []
         for group in self.groups:
             if self.groups[group][self._FILTER_DEF] is not None:
                 invalid_idx.extend(
@@ -265,16 +269,22 @@
                     print(m)
                     self._df[column].fillna(m, inplace=True)
                 elif method == "mode":
                     self._df[column].fillna(self._df[column].mode()[0], inplace=True)
 
     def report(self, group=None):
         """
-        TODO: Docstring
+        Returns the report for the specified group or all groups if no group is specified.
+
+        Requires verbose to be set to True on the Rim class. This is disabled by default
+        for performance reasons.
         """
+        if not self.verbose:
+            raise ValueError("Verbose must evaluate to True on the Rim class to generate a report."
+                             "This is disabled by default for performance reasons.")
         report = {}
         if group is None:
             for group in self.groups:
                 report[group] = self.groups[group][self._REPORT]
         else:
             report[group] = self.groups[group][self._REPORT]
         return report
```

### Comparing `weightipy-0.2.0/weightipy/weight_engine.py` & `weightipy-0.3.0/weightipy/weight_engine.py`

 * *Files identical despite different names*

