# Comparing `tmp/quivr-0.4.1.tar.gz` & `tmp/quivr-0.4.2.tar.gz`

## Comparing `quivr-0.4.1.tar` & `quivr-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/__version__.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/attributes.py
--rw-r--r--   0        0        0    27573 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/columns.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/concat.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/defragment.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/errors.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/schemagraph.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/streaming.py
--rw-r--r--   0        0        0    27596 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/tables.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.1/LICENSE
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.1/README.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/__version__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/attributes.py
+-rw-r--r--   0        0        0    27573 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/columns.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/concat.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/defragment.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/errors.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/schemagraph.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/streaming.py
+-rw-r--r--   0        0        0    27707 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/tables.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.2/LICENSE
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.2/README.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.2/PKG-INFO
```

### Comparing `quivr-0.4.1/quivr/__init__.py` & `quivr-0.4.2/quivr/__init__.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/quivr/attributes.py` & `quivr-0.4.2/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/quivr/columns.py` & `quivr-0.4.2/quivr/columns.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/quivr/concat.py` & `quivr-0.4.2/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/quivr/indexing.py` & `quivr-0.4.2/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/quivr/matrix.py` & `quivr-0.4.2/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/quivr/schemagraph.py` & `quivr-0.4.2/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/quivr/tables.py` & `quivr-0.4.2/quivr/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,16 @@
                 arrays.append(value.to_structarray())
             elif isinstance(value, pa.Array):
                 arrays.append(value)
             elif isinstance(value, np.ndarray):
                 arrays.append(pa.array(value, type=field.type))
             elif isinstance(value, list):
                 arrays.append(pa.array(value, type=field.type))
+            elif isinstance(value, pd.Series):
+                arrays.append(pa.array(value, type=field.type))
             else:
                 raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
 
         if size is None:
             raise ValueError("No data provided")
 
         for idx in empty_columns:
```

### Comparing `quivr-0.4.1/quivr/validators.py` & `quivr-0.4.2/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/LICENSE` & `quivr-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/README.md` & `quivr-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/pyproject.toml` & `quivr-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.4.1/PKG-INFO` & `quivr-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.4.1
+Version: 0.4.2
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

