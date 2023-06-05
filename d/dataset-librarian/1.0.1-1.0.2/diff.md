# Comparing `tmp/dataset_librarian-1.0.1.tar.gz` & `tmp/dataset_librarian-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_librarian-1.0.1.tar", last modified: Mon Jun  5 18:31:42 2023, max compression
+gzip compressed data, was "dataset_librarian-1.0.2.tar", last modified: Mon Jun  5 19:36:02 2023, max compression
```

## Comparing `dataset_librarian-1.0.1.tar` & `dataset_librarian-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.023649 dataset_librarian-1.0.1/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3974 2023-06-05 18:31:42.023649 dataset_librarian-1.0.1/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3424 2023-06-05 18:22:53.000000 dataset_librarian-1.0.1/README.md
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      804 2023-06-05 18:31:32.000000 dataset_librarian-1.0.1/pyproject.toml
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-06-05 18:31:42.023649 dataset_librarian-1.0.1/setup.cfg
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.019649 dataset_librarian-1.0.1/src/
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.019649 dataset_librarian-1.0.1/src/dataset_librarian/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.1/src/dataset_librarian/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3944 2023-05-23 13:31:26.000000 dataset_librarian-1.0.1/src/dataset_librarian/dataset.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.019649 dataset_librarian-1.0.1/src/dataset_librarian/dataset_api/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.1/src/dataset_librarian/dataset_api/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2302 2023-05-18 18:37:10.000000 dataset_librarian-1.0.1/src/dataset_librarian/dataset_api/download.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3484 2023-05-18 18:37:04.000000 dataset_librarian-1.0.1/src/dataset_librarian/dataset_api/preprocess.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2425 2023-05-18 18:00:22.000000 dataset_librarian-1.0.1/src/dataset_librarian/datasets_urls.json
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.019649 dataset_librarian-1.0.1/src/dataset_librarian/scripts/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.1/src/dataset_librarian/scripts/__init__.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.023649 dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     7804 2023-06-05 18:23:21.000000 dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/create_data_split.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     8135 2023-06-01 04:54:09.000000 dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/prepare_nlp_data.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    10700 2023-05-18 18:00:22.000000 dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/prepare_vision_data.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.023649 dataset_librarian-1.0.1/src/dataset_librarian/scripts/mvtec-ad/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-18 18:00:22.000000 dataset_librarian-1.0.1/src/dataset_librarian/scripts/mvtec-ad/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2746 2023-05-18 18:00:22.000000 dataset_librarian-1.0.1/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1928 2023-05-18 18:00:22.000000 dataset_librarian-1.0.1/src/dataset_librarian/terms_and_conditions.txt
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 18:31:42.019649 dataset_librarian-1.0.1/src/dataset_librarian.egg-info/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3974 2023-06-05 18:31:41.000000 dataset_librarian-1.0.1/src/dataset_librarian.egg-info/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      939 2023-06-05 18:31:42.000000 dataset_librarian-1.0.1/src/dataset_librarian.egg-info/SOURCES.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-06-05 18:31:41.000000 dataset_librarian-1.0.1/src/dataset_librarian.egg-info/dependency_links.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       77 2023-06-05 18:31:41.000000 dataset_librarian-1.0.1/src/dataset_librarian.egg-info/requires.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       18 2023-06-05 18:31:41.000000 dataset_librarian-1.0.1/src/dataset_librarian.egg-info/top_level.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)   102383 2023-06-05 18:22:53.000000 dataset_librarian-1.0.1/third-party-programs.txt
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3975 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3424 2023-06-05 18:22:53.000000 dataset_librarian-1.0.2/README.md
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      805 2023-06-05 19:35:51.000000 dataset_librarian-1.0.2/pyproject.toml
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/setup.cfg
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/dataset_librarian/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3944 2023-05-23 13:31:26.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2302 2023-05-18 18:37:10.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/download.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3484 2023-05-18 18:37:04.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/preprocess.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2425 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/datasets_urls.json
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/src/dataset_librarian/scripts/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/__init__.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     7804 2023-06-05 18:23:21.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/create_data_split.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     8135 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_nlp_data.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    10700 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_vision_data.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2746 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1928 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/terms_and_conditions.txt
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3975 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      939 2023-06-05 19:36:02.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/SOURCES.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/dependency_links.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       77 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/requires.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       18 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/top_level.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)   102383 2023-06-05 18:22:53.000000 dataset_librarian-1.0.2/third-party-programs.txt
```

### Comparing `dataset_librarian-1.0.1/PKG-INFO` & `dataset_librarian-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dataset_librarian
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets
 Author-email: IntelAI <IntelAI@intel.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 
 # Dataset Librarian
 
 ## Installation Process
```

### Comparing `dataset_librarian-1.0.1/README.md` & `dataset_librarian-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/pyproject.toml` & `dataset_librarian-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset_librarian"
-version = "1.0.1"
+version = "1.0.2"
 requires-python = ">=3.9,<3.11"
 authors = [
     { name="IntelAI", email="IntelAI@intel.com"}
 ]
 description = "Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pandas",
     "tqdm",
     "docx2txt",
     "openpyxl",
```

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/__init__.py` & `dataset_librarian-1.0.2/src/dataset_librarian/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/dataset.py` & `dataset_librarian-1.0.2/src/dataset_librarian/dataset.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/dataset_api/__init__.py` & `dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/dataset_api/download.py` & `dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/download.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/dataset_api/preprocess.py` & `dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/preprocess.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/datasets_urls.json` & `dataset_librarian-1.0.2/src/dataset_librarian/datasets_urls.json`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/scripts/__init__.py` & `dataset_librarian-1.0.2/src/dataset_librarian/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/__init__.py` & `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/create_data_split.py` & `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/create_data_split.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/prepare_nlp_data.py` & `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_nlp_data.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/scripts/brca/prepare_vision_data.py` & `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_vision_data.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/scripts/mvtec-ad/__init__.py` & `dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py` & `dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian/terms_and_conditions.txt` & `dataset_librarian-1.0.2/src/dataset_librarian/terms_and_conditions.txt`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian.egg-info/PKG-INFO` & `dataset_librarian-1.0.2/src/dataset_librarian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dataset-librarian
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets
 Author-email: IntelAI <IntelAI@intel.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 
 # Dataset Librarian
 
 ## Installation Process
```

### Comparing `dataset_librarian-1.0.1/src/dataset_librarian.egg-info/SOURCES.txt` & `dataset_librarian-1.0.2/src/dataset_librarian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.1/third-party-programs.txt` & `dataset_librarian-1.0.2/third-party-programs.txt`

 * *Files identical despite different names*

