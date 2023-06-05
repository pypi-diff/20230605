# Comparing `tmp/abmatrix-0.3.2.tar.gz` & `tmp/abmatrix-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.3.2.tar", last modified: Mon Jun  5 18:06:07 2023, max compression
+gzip compressed data, was "abmatrix-0.3.3.tar", last modified: Mon Jun  5 18:16:57 2023, max compression
```

## Comparing `abmatrix-0.3.2.tar` & `abmatrix-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-05 18:06:07.766970 abmatrix-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-05 18:05:57.000000 abmatrix-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:05:57.000000 abmatrix-0.3.2/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-05 18:05:57.000000 abmatrix-0.3.2/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 18:05:57.000000 abmatrix-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 18:06:07.766970 abmatrix-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-05 18:05:57.000000 abmatrix-0.3.2/tests/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-05 18:05:57.000000 abmatrix-0.3.2/tests/test_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:16:57.861435 abmatrix-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-05 18:16:57.861435 abmatrix-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-05 18:16:47.000000 abmatrix-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:16:57.857435 abmatrix-0.3.3/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:16:47.000000 abmatrix-0.3.3/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-05 18:16:47.000000 abmatrix-0.3.3/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:16:57.861435 abmatrix-0.3.3/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-05 18:16:57.000000 abmatrix-0.3.3/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 18:16:57.000000 abmatrix-0.3.3/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:16:57.000000 abmatrix-0.3.3/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 18:16:57.000000 abmatrix-0.3.3/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 18:16:47.000000 abmatrix-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 18:16:57.861435 abmatrix-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:16:57.861435 abmatrix-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-05 18:16:47.000000 abmatrix-0.3.3/tests/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-05 18:16:47.000000 abmatrix-0.3.3/tests/test_subset.py
```

### Comparing `abmatrix-0.3.2/PKG-INFO` & `abmatrix-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abmatrix
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python module to read and parse AB Matrix files
 Author-email: Daniel Garrigan <popgendad@proton.me>
 Project-URL: Homepage, https://github.com/wisdomhealth-inc/abmatrix
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `abmatrix-0.3.2/README.md` & `abmatrix-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `abmatrix-0.3.2/abmatrix/abmatrix.py` & `abmatrix-0.3.3/abmatrix/abmatrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,16 +110,16 @@
                 if self.iszip:
                     line = line.decode("utf-8")
                 locus_array = line.rstrip("\n").split("\t")
                 _ = locus_array.pop(0)
                 for sample_id in sample_list:
                     try:
                         pos = self.sample_index[sample_id]
-                    except KeyError as e:
-                        raise e
+                    except KeyError:
+                        locus_dict[sample_id] = "--"
                     else:
                         locus_dict[sample_id] = locus_array[pos]
             finally:
                 output_list.append(locus_dict)
         return output_list
 
     def close(self):
```

### Comparing `abmatrix-0.3.2/abmatrix.egg-info/PKG-INFO` & `abmatrix-0.3.3/abmatrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abmatrix
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python module to read and parse AB Matrix files
 Author-email: Daniel Garrigan <popgendad@proton.me>
 Project-URL: Homepage, https://github.com/wisdomhealth-inc/abmatrix
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `abmatrix-0.3.2/tests/test_feature_extraction.py` & `abmatrix-0.3.3/tests/test_feature_extraction.py`

 * *Files identical despite different names*

