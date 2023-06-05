# Comparing `tmp/abmatrix-0.3.1.tar.gz` & `tmp/abmatrix-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.3.1.tar", last modified: Mon Jun  5 05:32:06 2023, max compression
+gzip compressed data, was "abmatrix-0.3.2.tar", last modified: Mon Jun  5 18:06:07 2023, max compression
```

## Comparing `abmatrix-0.3.1.tar` & `abmatrix-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 05:32:06.242778 abmatrix-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-05 05:31:53.000000 abmatrix-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:31:53.000000 abmatrix-0.3.1/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-05 05:31:53.000000 abmatrix-0.3.1/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 05:31:53.000000 abmatrix-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 05:32:06.242778 abmatrix-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-05 05:31:53.000000 abmatrix-0.3.1/tests/test_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-05 18:06:07.766970 abmatrix-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-05 18:05:57.000000 abmatrix-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:05:57.000000 abmatrix-0.3.2/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-05 18:05:57.000000 abmatrix-0.3.2/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 18:06:07.000000 abmatrix-0.3.2/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 18:05:57.000000 abmatrix-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 18:06:07.766970 abmatrix-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:07.766970 abmatrix-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-05 18:05:57.000000 abmatrix-0.3.2/tests/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-05 18:05:57.000000 abmatrix-0.3.2/tests/test_subset.py
```

### Comparing `abmatrix-0.3.1/abmatrix/abmatrix.py` & `abmatrix-0.3.2/abmatrix/abmatrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,32 +94,33 @@
         if "samples" in kwargs:
             sample_list = kwargs["samples"]
         else:
             sample_list = list(self.sample_index.keys())
         if type(locus_list) != list:
             raise Exception("reduce needs list of locus identifiers")
         for locus in locus_list:
+            locus_dict = {"id": locus}
             try:
                 offset = self.index[locus]
-            except KeyError as e:
-                raise e
+            except KeyError:
+                for sample_id in sample_list:
+                    locus_dict[sample_id] = "--"
             else:
-                locus_dict = {}
                 self.fstream.seek(offset)
                 line = self.fstream.readline()
                 if self.iszip:
                     line = line.decode("utf-8")
                 locus_array = line.rstrip("\n").split("\t")
-                locus_id = locus_array.pop(0)
-                locus_dict["id"] = locus_id
+                _ = locus_array.pop(0)
                 for sample_id in sample_list:
                     try:
                         pos = self.sample_index[sample_id]
                     except KeyError as e:
                         raise e
                     else:
                         locus_dict[sample_id] = locus_array[pos]
+            finally:
                 output_list.append(locus_dict)
         return output_list
 
     def close(self):
         self.fstream.close()
```

