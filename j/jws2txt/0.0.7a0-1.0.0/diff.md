# Comparing `tmp/jws2txt-0.0.7a0.tar.gz` & `tmp/jws2txt-1.0.0.tar.gz`

## Comparing `jws2txt-0.0.7a0.tar` & `jws2txt-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/requirements.txt
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/.github/workflows/jws2txt_actions.yaml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/.vscode/settings.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/jws2txt/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/jws2txt/jws2txt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/jws2txt/helpers/__init.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/jws2txt/helpers/helpers.py
--rw-r--r--   0        0        0    21504 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/temp/001Hg.jws
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/temp/14.jws
--rw-r--r--   0        0        0    54784 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/temp/BGR20190312[5294].jws
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/temp/sample_fluorescence_3.jws
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/temp/smth.jws
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/temp/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/tests/__init__.py
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/tests/test_helpers.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/tests/test_main.py
--rw-r--r--   0        0        0    21504 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/tests/files/001Hg.jws
--rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/tests/files/2022_05_14-1.jwb
--rw-r--r--   0        0        0    25088 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/tests/files/sample_CD_HT_Abs.jws
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/tests/files/sample_fluorescence.jws
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/pyproject.toml
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jws2txt-0.0.7a0/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 jws2txt-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 jws2txt-1.0.0/.github/workflows/jws2txt_actions.yaml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jws2txt-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jws2txt-1.0.0/jws2txt/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jws2txt-1.0.0/jws2txt/jws2txt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jws2txt-1.0.0/jws2txt/helpers/__init.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 jws2txt-1.0.0/jws2txt/helpers/helpers.py
+-rw-r--r--   0        0        0    21504 2020-02-02 00:00:00.000000 jws2txt-1.0.0/temp/001Hg.jws
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 jws2txt-1.0.0/temp/14.jws
+-rw-r--r--   0        0        0    54784 2020-02-02 00:00:00.000000 jws2txt-1.0.0/temp/BGR20190312[5294].jws
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 jws2txt-1.0.0/temp/sample_fluorescence_3.jws
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 jws2txt-1.0.0/temp/smth.jws
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jws2txt-1.0.0/temp/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jws2txt-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 jws2txt-1.0.0/tests/test_helpers.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jws2txt-1.0.0/tests/test_main.py
+-rw-r--r--   0        0        0    21504 2020-02-02 00:00:00.000000 jws2txt-1.0.0/tests/files/001Hg.jws
+-rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 jws2txt-1.0.0/tests/files/2022_05_14-1.jwb
+-rw-r--r--   0        0        0    25088 2020-02-02 00:00:00.000000 jws2txt-1.0.0/tests/files/sample_CD_HT_Abs.jws
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 jws2txt-1.0.0/tests/files/sample_fluorescence.jws
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jws2txt-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jws2txt-1.0.0/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 jws2txt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jws2txt-1.0.0/PKG-INFO
```

### Comparing `jws2txt-0.0.7a0/.github/workflows/jws2txt_actions.yaml` & `jws2txt-1.0.0/.github/workflows/jws2txt_actions.yaml`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/jws2txt/jws2txt.py` & `jws2txt-1.0.0/jws2txt/jws2txt.py`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/jws2txt/helpers/helpers.py` & `jws2txt-1.0.0/jws2txt/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/temp/001Hg.jws` & `jws2txt-1.0.0/temp/001Hg.jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/temp/14.jws` & `jws2txt-1.0.0/temp/14.jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/temp/BGR20190312[5294].jws` & `jws2txt-1.0.0/temp/BGR20190312[5294].jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/temp/sample_fluorescence_3.jws` & `jws2txt-1.0.0/temp/sample_fluorescence_3.jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/temp/smth.jws` & `jws2txt-1.0.0/temp/smth.jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/temp/test.py` & `jws2txt-1.0.0/temp/test.py`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/tests/test_helpers.py` & `jws2txt-1.0.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/tests/files/001Hg.jws` & `jws2txt-1.0.0/tests/files/001Hg.jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/tests/files/2022_05_14-1.jwb` & `jws2txt-1.0.0/tests/files/2022_05_14-1.jwb`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/tests/files/sample_CD_HT_Abs.jws` & `jws2txt-1.0.0/tests/files/sample_CD_HT_Abs.jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/tests/files/sample_fluorescence.jws` & `jws2txt-1.0.0/tests/files/sample_fluorescence.jws`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/README.md` & `jws2txt-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `jws2txt-0.0.7a0/pyproject.toml` & `jws2txt-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "jws2txt"
-version = "0.0.7a"
+version = "1.0.0"
 authors = [
   { name="Józef Tran", email="jozeftran@gmail.com" },
 ]
 description = "A JASCO file (*.jws and *.jwb) to text file converter."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `jws2txt-0.0.7a0/PKG-INFO` & `jws2txt-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: jws2txt
-Version: 0.0.7a0
+Version: 1.0.0
 Summary: A JASCO file (*.jws and *.jwb) to text file converter.
 Project-URL: Homepage, https://github.com/jzftran/jws2txt
 Project-URL: Bug Tracker, https://github.com/jzftran/jws2txt/issues
 Author-email: Józef Tran <jozeftran@gmail.com>
+License-File: LICENSE.txt
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

