# Comparing `tmp/proteinflow-1.3.5.tar.gz` & `tmp/proteinflow-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.3.5.tar", last modified: Fri May 26 11:32:45 2023, max compression
+gzip compressed data, was "proteinflow-1.3.6.tar", last modified: Mon Jun  5 12:59:15 2023, max compression
```

## Comparing `proteinflow-1.3.5.tar` & `proteinflow-1.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 11:32:30.000000 proteinflow-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-26 11:32:45.960125 proteinflow-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-26 11:32:30.000000 proteinflow-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.956125 proteinflow-1.3.5/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)   100459 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-26 11:32:30.000000 proteinflow-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:32:45.960125 proteinflow-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-26 11:32:30.000000 proteinflow-1.3.5/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-26 11:32:30.000000 proteinflow-1.3.5/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 11:32:30.000000 proteinflow-1.3.5/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.711494 proteinflow-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 12:59:03.000000 proteinflow-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-06-05 12:59:15.711494 proteinflow-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-06-05 12:59:03.000000 proteinflow-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.703494 proteinflow-1.3.6/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   101608 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.707494 proteinflow-1.3.6/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.707494 proteinflow-1.3.6/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.707494 proteinflow-1.3.6/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-05 12:59:03.000000 proteinflow-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:59:15.711494 proteinflow-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.711494 proteinflow-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-05 12:59:03.000000 proteinflow-1.3.6/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-05 12:59:03.000000 proteinflow-1.3.6/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-05 12:59:03.000000 proteinflow-1.3.6/tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.5/LICENSE` & `proteinflow-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/PKG-INFO` & `proteinflow-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.5
+Version: 1.3.6
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.5 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.6 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.5/README.md` & `proteinflow-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/__init__.py` & `proteinflow-1.3.6/proteinflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
 
         Returns
         -------
         chain_M : torch.Tensor
             a `(B, L)` shaped binary tensor where 1 denotes the part that needs to be predicted and
             0 is everything else
         """
-        
+
         if "cdr" in batch and "cdr_id" in batch:
             chain_M = torch.zeros_like(batch["cdr"])
             for i, cdr_arr in enumerate(batch["cdr"]):
                 if self.mask_all_cdrs:
                     chain_M[i] = cdr_arr != CDR["-"]
                 else:
                     chain_M[i] = cdr_arr == batch["cdr_id"][i]
@@ -1658,14 +1658,15 @@
         debug=False,
         interpolate="none",
         node_features_type="zeros",
         debug_file_path=None,
         entry_type="biounit",  # biounit, chain, pair
         classes_to_exclude=None,  # heteromers, homomers, single_chains
         shuffle_clusters=True,
+        min_cdr_length=None,
         feature_functions=None,
     ):
         """
         Parameters
         ----------
         dataset_folder : str
             the path to the folder with proteinflow format input files (assumes that files are named {biounit_id}.pickle)
@@ -1692,14 +1693,16 @@
         entry_type : {"biounit", "chain", "pair"}
             the type of entries to generate (`"biounit"` for biounit-level complexes, `"chain"` for chain-level, `"pair"`
             for chain-chain pairs (all pairs that are seen in the same biounit and have intersecting coordinate clouds))
         classes_to_exclude : list of str, optional
             a list of classes to exclude from the dataset (select from `"single_chains"`, `"heteromers"`, `"homomers"`)
         shuffle_clusters : bool, default True
             if `True`, a new representative is randomly selected for each cluster at each epoch (if `clustering_dict_path` is given)
+        min_cdr_length : int, optional
+            for SAbDab datasets, biounits with CDRs shorter than `min_cdr_length` will be excluded
         feature_functions : dict, optional
             a dictionary of functions to compute additional features (keys are the names of the features, values are the functions)
         """
 
         alphabet = ALPHABET
         self.alphabet_dict = defaultdict(lambda: 0)
         for i, letter in enumerate(alphabet):
@@ -1759,23 +1762,27 @@
         if clustering_dict_path is not None and use_fraction < 1:
             with open(clustering_dict_path, "rb") as f:
                 clusters = pickle.load(f)
             keys = sorted(clusters.keys())[: int(len(clusters) * use_fraction)]
             to_process = set()
             for key in keys:
                 to_process.update([x[0] for x in clusters[key]])
-            to_process = [x for x in to_process if x in os.listdir(dataset_folder)]
+
+            file_set = set(os.listdir(dataset_folder))
+            to_process = [x for x in to_process if x in file_set]
         if debug:
             to_process = to_process[:1000]
         if self.entry_type == "pair":
             print(
                 "Please note that the pair entry type takes longer to process than the other two. The progress bar is not linear because of the varying number of chains per file."
             )
         output_tuples_list = p_map(
-            lambda x: self._process(x, rewrite=rewrite, max_length=max_length),
+            lambda x: self._process(
+                x, rewrite=rewrite, max_length=max_length, min_cdr_length=min_cdr_length
+            ),
             to_process,
         )
         # save the file names
         for output_tuples in output_tuples_list:
             for id, filename, chain_set in output_tuples:
                 for chain in chain_set:
                     self.files[id][chain].append(filename)
@@ -1980,15 +1987,15 @@
         """
         Sidechain coordinates
         """
 
         crd_sc = chain_dict["crd_sc"]
         return crd_sc
 
-    def _process(self, filename, rewrite=False, max_length=None):
+    def _process(self, filename, rewrite=False, max_length=None, min_cdr_length=None):
         """
         Process a proteinflow file and save it as ProteinMPNN features
         """
 
         input_file = os.path.join(self.dataset_folder, filename)
         no_extension_name = filename.split(".")[0]
         with open(input_file, "rb") as f:
@@ -2012,14 +2019,22 @@
             pass_set = False
             add_name = True
             if os.path.exists(output_file) and not rewrite:
                 pass_set = True
                 if max_length is not None:
                     if sum([len(data[x]["seq"]) for x in chain_set]) > max_length:
                         add_name = False
+                if min_cdr_length is not None:
+                    for chain in chain_set:
+                        if "cdr" not in data[chain]:
+                            continue
+                        u = np.unique(data[chain]["cdr"])
+                        for cdr_ in u:
+                            if (data[chain]["cdr"] == cdr_).sum() < min_cdr_length:
+                                add_name = False
             else:
                 X = []
                 S = []
                 mask = []
                 mask_original = []
                 chain_encoding_all = []
                 residue_idx = []
@@ -2028,14 +2043,23 @@
                 last_idx = 0
                 chain_dict = {}
 
                 if max_length is not None:
                     if sum([len(data[x]["seq"]) for x in chain_set]) > max_length:
                         pass_set = True
                         add_name = False
+                if min_cdr_length is not None:
+                    for chain in chain_set:
+                        if "cdr" not in data[chain]:
+                            continue
+                        u = np.unique(data[chain]["cdr"])
+                        for cdr_ in u:
+                            if (data[chain]["cdr"] == cdr_).sum() < min_cdr_length:
+                                add_name = False
+                                pass_set = True
 
                 if self.entry_type == "pair":
                     # intersect = []
                     X1 = data[chain_set[0]]["crd_bb"][
                         data[chain_set[0]]["msk"].astype(bool)
                     ]
                     X2 = data[chain_set[1]]["crd_bb"][
```

### Comparing `proteinflow-1.3.5/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.3.6/proteinflow/scripts/proteinflow_cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/async_download.py` & `proteinflow-1.3.6/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/biotite_sse.py` & `proteinflow-1.3.6/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/build_pdb.py` & `proteinflow-1.3.6/proteinflow/utils/build_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.3.6/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/filter_database.py` & `proteinflow-1.3.6/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.3.6/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/process_pdb.py` & `proteinflow-1.3.6/proteinflow/utils/process_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow/utils/split_dataset.py` & `proteinflow-1.3.6/proteinflow/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.3.6/proteinflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.5
+Version: 1.3.6
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.5 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.6 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.5/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.3.6/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/pyproject.toml` & `proteinflow-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.3.5"
+version = "1.3.6"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-1.3.5/tests/test_download.py` & `proteinflow-1.3.6/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/tests/test_generate.py` & `proteinflow-1.3.6/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.5/tests/test_sabdab.py` & `proteinflow-1.3.6/tests/test_sabdab.py`

 * *Files identical despite different names*

