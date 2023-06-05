# Comparing `tmp/scCAMEL-0.26b0.tar.gz` & `tmp/scCAMEL-0.27b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCAMEL-0.26b0.tar", last modified: Tue May 23 10:53:45 2023, max compression
+gzip compressed data, was "scCAMEL-0.27b0.tar", last modified: Mon Jun  5 09:28:00 2023, max compression
```

## Comparing `scCAMEL-0.26b0.tar` & `scCAMEL-0.27b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:45.178655 scCAMEL-0.26b0/
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    34870 2023-05-23 10:09:37.000000 scCAMEL-0.26b0/LICENSE.txt
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:53:45.170656 scCAMEL-0.26b0/PKG-INFO
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      298 2022-11-01 09:55:19.000000 scCAMEL-0.26b0/README.md
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       86 2022-07-05 13:12:44.000000 scCAMEL-0.26b0/pyproject.toml
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       38 2023-05-23 10:53:45.181654 scCAMEL-0.26b0/setup.cfg
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      952 2023-05-23 10:53:19.000000 scCAMEL-0.26b0/setup.py
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:44.369352 scCAMEL-0.26b0/src/
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:44.830355 scCAMEL-0.26b0/src/scCAMEL/
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    62722 2023-04-18 10:06:59.000000 scCAMEL-0.26b0/src/scCAMEL/CamelEvo.py
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    56615 2023-04-18 09:44:23.000000 scCAMEL-0.26b0/src/scCAMEL/CamelPrefiltering.py
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)   121678 2023-05-23 10:32:37.000000 scCAMEL-0.26b0/src/scCAMEL/CamelSwapline.py
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      125 2022-10-31 11:06:46.000000 scCAMEL-0.26b0/src/scCAMEL/__init__.py
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:45.098357 scCAMEL-0.26b0/src/scCAMEL.egg-info/
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:53:43.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/PKG-INFO
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      295 2023-05-23 10:53:44.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/SOURCES.txt
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        1 2023-05-23 10:53:43.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/dependency_links.txt
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        8 2023-05-23 10:53:43.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/top_level.txt
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-06-05 09:28:00.203387 scCAMEL-0.27b0/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    34870 2023-05-23 10:09:37.000000 scCAMEL-0.27b0/LICENSE.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-06-05 09:28:00.194387 scCAMEL-0.27b0/PKG-INFO
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      298 2022-11-01 09:55:19.000000 scCAMEL-0.27b0/README.md
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       86 2022-07-05 13:12:44.000000 scCAMEL-0.27b0/pyproject.toml
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       38 2023-06-05 09:28:00.205387 scCAMEL-0.27b0/setup.cfg
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      952 2023-06-05 09:25:28.000000 scCAMEL-0.27b0/setup.py
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-06-05 09:27:59.378380 scCAMEL-0.27b0/src/
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-06-05 09:27:59.845384 scCAMEL-0.27b0/src/scCAMEL/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    62722 2023-04-18 10:06:59.000000 scCAMEL-0.27b0/src/scCAMEL/CamelEvo.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    56615 2023-06-05 09:13:51.000000 scCAMEL-0.27b0/src/scCAMEL/CamelPrefiltering.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)   121678 2023-05-23 10:32:37.000000 scCAMEL-0.27b0/src/scCAMEL/CamelSwapline.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      125 2022-10-31 11:06:46.000000 scCAMEL-0.27b0/src/scCAMEL/__init__.py
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-06-05 09:28:00.120386 scCAMEL-0.27b0/src/scCAMEL.egg-info/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-06-05 09:27:58.000000 scCAMEL-0.27b0/src/scCAMEL.egg-info/PKG-INFO
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      295 2023-06-05 09:27:59.000000 scCAMEL-0.27b0/src/scCAMEL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        1 2023-06-05 09:27:58.000000 scCAMEL-0.27b0/src/scCAMEL.egg-info/dependency_links.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        8 2023-06-05 09:27:58.000000 scCAMEL-0.27b0/src/scCAMEL.egg-info/top_level.txt
```

### Comparing `scCAMEL-0.26b0/LICENSE.txt` & `scCAMEL-0.27b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scCAMEL-0.26b0/PKG-INFO` & `scCAMEL-0.27b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCAMEL
-Version: 0.26b0
+Version: 0.27b0
 Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
 Home-page: https://sccamel.readthedocs.io/
 Author: Yizhou Hu
 Author-email: yizhou.hu@ki.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scCAMEL-0.26b0/setup.py` & `scCAMEL-0.27b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scCAMEL",
-    version="0.26b",
+    version="0.27b",
     author="Yizhou Hu",
     author_email="yizhou.hu@ki.se",
     description="scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sccamel.readthedocs.io/",
     classifiers=[
```

### Comparing `scCAMEL-0.26b0/src/scCAMEL/CamelEvo.py` & `scCAMEL-0.27b0/src/scCAMEL/CamelEvo.py`

 * *Files identical despite different names*

### Comparing `scCAMEL-0.26b0/src/scCAMEL/CamelPrefiltering.py` & `scCAMEL-0.27b0/src/scCAMEL/CamelPrefiltering.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,18 +683,18 @@
             sharedMVgenes = list(set(list_genes + tflist))
         else:
             df_dev_rev = dfpfc.iloc[np.argsort(score)[::-1], :].iloc[max(min(-thrs, -2000), -5000):, :]
             sharedMVgenes = list(set(list_genes + tflist) - set(df_dev_rev.index))
         if np.sum(TPTT) != 0:
             dfpfc = (dfpfc / dfpfc.sum()).multiply(TPTT, axis=0).fillna(0)
         if std_scaling == True:
-            scalepfc = dfpfc.div(dfpfc.std(1), axis=0).dropna(0)
-        scalepfc = dfpfc.astype(float).dropna(0)
+            scalepfc = dfpfc.div(dfpfc.std(1), axis=0).fillna(0)
+        scalepfc = dfpfc.astype(float).fillna(0)
         scalepfc = dfpfc.div(dfpfc.std(1), axis=0)
-        scalepfc = scalepfc.dropna(0)
+        scalepfc = scalepfc.fillna(0)
         dfpfc_dev = scalepfc.loc[set(scalepfc.index) & set(sharedMVgenes)].dropna()
         dfpfc_dev_log = np.log2(dfpfc_dev + 1)
         dfpfc_dev_all = dfpfc_dev_log.T.join(dfpfcclus.T, how="inner").dropna()
         bool1 = mprotogruop != "nan"
         mclasses_names, mclasses_index = np.unique(mprotogruop[bool1], return_inverse=True, return_counts=False)
         mtrain_index = mclasses_index
         mdf_train_set = dfpfc_dev_log.loc[:, bool1].copy()
```

### Comparing `scCAMEL-0.26b0/src/scCAMEL/CamelSwapline.py` & `scCAMEL-0.27b0/src/scCAMEL/CamelSwapline.py`

 * *Files identical despite different names*

### Comparing `scCAMEL-0.26b0/src/scCAMEL.egg-info/PKG-INFO` & `scCAMEL-0.27b0/src/scCAMEL.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCAMEL
-Version: 0.26b0
+Version: 0.27b0
 Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
 Home-page: https://sccamel.readthedocs.io/
 Author: Yizhou Hu
 Author-email: yizhou.hu@ki.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

