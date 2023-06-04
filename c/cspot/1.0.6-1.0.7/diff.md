# Comparing `tmp/cspot-1.0.6.tar.gz` & `tmp/cspot-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspot-1.0.6.tar", max compression
+gzip compressed data, was "cspot-1.0.7.tar", max compression
```

## Comparing `cspot-1.0.6.tar` & `cspot-1.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      113 2023-06-02 23:46:02.832679 cspot-1.0.6/README.md
--rw-r--r--   0        0        0     8196 2023-06-03 14:50:07.931359 cspot-1.0.6/cspot/.DS_Store
--rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 cspot-1.0.6/cspot/UNet.py
--rw-r--r--   0        0        0      567 2023-06-03 00:49:31.038091 cspot-1.0.6/cspot/__init__.py
--rw-r--r--   0        0        0     6447 2023-06-04 14:04:52.928156 cspot-1.0.6/cspot/addPredictions.py
--rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.000000 cspot-1.0.6/cspot/archives/UNet-02032023.py
--rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 cspot-1.0.6/cspot/archives/gator-01272023.py
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/PartitionOfImage.py
--rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/PartitionOfImageOM.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/ftools.py
--rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/imtools.py
--rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.000000 cspot-1.0.6/cspot/archives/toolbox-02032023/toolbox.py
--rw-r--r--   0        0        0     9983 2023-06-03 23:29:17.205882 cspot-1.0.6/cspot/cloneFolder.py
--rw-r--r--   0        0        0     5425 2023-06-04 14:03:34.502069 cspot-1.0.6/cspot/csExport.py
--rw-r--r--   0        0        0    12214 2023-06-04 01:49:29.376512 cspot-1.0.6/cspot/csObject.py
--rw-r--r--   0        0        0    21466 2023-06-04 13:57:25.098445 cspot-1.0.6/cspot/csPhenotype.py
--rw-r--r--   0        0        0    17791 2023-06-04 00:09:38.907372 cspot-1.0.6/cspot/csPipeline.py
--rw-r--r--   0        0        0    12655 2023-06-04 01:03:32.130826 cspot-1.0.6/cspot/csPredict.py
--rw-r--r--   0        0        0    11491 2023-06-03 23:36:08.727326 cspot-1.0.6/cspot/csTrain.py
--rw-r--r--   0        0        0    41377 2023-06-04 01:56:09.635845 cspot-1.0.6/cspot/cspot.py
--rw-r--r--   0        0        0     7236 2023-06-04 01:37:29.786489 cspot-1.0.6/cspot/generateCSScore.py
--rw-r--r--   0        0        0    26724 2023-06-03 23:25:34.169745 cspot-1.0.6/cspot/generateThumbnails.py
--rw-r--r--   0        0        0    13523 2023-06-03 23:32:52.946563 cspot-1.0.6/cspot/generateTrainTestSplit.py
--rw-r--r--   0        0        0     8633 2023-06-04 02:03:45.337949 cspot-1.0.6/cspot/mergecsObject.py
--rw-r--r--   0        0        0    10237 2023-06-04 00:13:46.879038 cspot-1.0.6/cspot/scatterPlot.py
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.6/cspot/toolbox/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.6/cspot/toolbox/PartitionOfImage.py
--rw-r--r--   0        0        0      196 2023-03-10 02:36:16.000000 cspot-1.0.6/cspot/toolbox/__init__.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.6/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.6/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0      477 2023-03-10 02:39:18.000000 cspot-1.0.6/cspot/toolbox/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      711 2023-02-04 00:52:32.000000 cspot-1.0.6/cspot/toolbox/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.000000 cspot-1.0.6/cspot/toolbox/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0      361 2023-02-04 00:50:12.000000 cspot-1.0.6/cspot/toolbox/ftools.py
--rw-r--r--   0        0        0      671 2023-02-04 00:46:01.000000 cspot-1.0.6/cspot/toolbox/imtools.py
--rw-r--r--   0        0        0     1166 2023-06-04 14:40:07.691914 cspot-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 cspot-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1907 2023-06-04 22:13:27.495922 cspot-1.0.7/README.md
+-rw-r--r--   0        0        0     8196 2023-06-03 14:50:07.931359 cspot-1.0.7/cspot/.DS_Store
+-rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 cspot-1.0.7/cspot/UNet.py
+-rw-r--r--   0        0        0      567 2023-06-03 00:49:31.038091 cspot-1.0.7/cspot/__init__.py
+-rw-r--r--   0        0        0     6447 2023-06-04 14:04:52.928156 cspot-1.0.7/cspot/addPredictions.py
+-rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.000000 cspot-1.0.7/cspot/archives/UNet-02032023.py
+-rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 cspot-1.0.7/cspot/archives/gator-01272023.py
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/PartitionOfImage.py
+-rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/PartitionOfImageOM.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/ftools.py
+-rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/imtools.py
+-rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.000000 cspot-1.0.7/cspot/archives/toolbox-02032023/toolbox.py
+-rw-r--r--   0        0        0     9983 2023-06-03 23:29:17.205882 cspot-1.0.7/cspot/cloneFolder.py
+-rw-r--r--   0        0        0     5425 2023-06-04 14:03:34.502069 cspot-1.0.7/cspot/csExport.py
+-rw-r--r--   0        0        0    12214 2023-06-04 01:49:29.376512 cspot-1.0.7/cspot/csObject.py
+-rw-r--r--   0        0        0    21466 2023-06-04 13:57:25.098445 cspot-1.0.7/cspot/csPhenotype.py
+-rw-r--r--   0        0        0    17791 2023-06-04 00:09:38.907372 cspot-1.0.7/cspot/csPipeline.py
+-rw-r--r--   0        0        0    12655 2023-06-04 01:03:32.130826 cspot-1.0.7/cspot/csPredict.py
+-rw-r--r--   0        0        0    11491 2023-06-03 23:36:08.727326 cspot-1.0.7/cspot/csTrain.py
+-rw-r--r--   0        0        0    41377 2023-06-04 01:56:09.635845 cspot-1.0.7/cspot/cspot.py
+-rw-r--r--   0        0        0     7236 2023-06-04 01:37:29.786489 cspot-1.0.7/cspot/generateCSScore.py
+-rw-r--r--   0        0        0    26724 2023-06-03 23:25:34.169745 cspot-1.0.7/cspot/generateThumbnails.py
+-rw-r--r--   0        0        0    13523 2023-06-03 23:32:52.946563 cspot-1.0.7/cspot/generateTrainTestSplit.py
+-rw-r--r--   0        0        0     8633 2023-06-04 02:03:45.337949 cspot-1.0.7/cspot/mergecsObject.py
+-rw-r--r--   0        0        0    10237 2023-06-04 00:13:46.879038 cspot-1.0.7/cspot/scatterPlot.py
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.7/cspot/toolbox/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.7/cspot/toolbox/PartitionOfImage.py
+-rw-r--r--   0        0        0      196 2023-03-10 02:36:16.000000 cspot-1.0.7/cspot/toolbox/__init__.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.7/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.7/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0      477 2023-03-10 02:39:18.000000 cspot-1.0.7/cspot/toolbox/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      711 2023-02-04 00:52:32.000000 cspot-1.0.7/cspot/toolbox/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.000000 cspot-1.0.7/cspot/toolbox/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0      361 2023-02-04 00:50:12.000000 cspot-1.0.7/cspot/toolbox/ftools.py
+-rw-r--r--   0        0        0      671 2023-02-04 00:46:01.000000 cspot-1.0.7/cspot/toolbox/imtools.py
+-rw-r--r--   0        0        0     1166 2023-06-04 22:42:50.115102 cspot-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 cspot-1.0.7/PKG-INFO
```

### Comparing `cspot-1.0.6/cspot/.DS_Store` & `cspot-1.0.7/cspot/.DS_Store`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/UNet.py` & `cspot-1.0.7/cspot/UNet.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/__init__.py` & `cspot-1.0.7/cspot/__init__.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/addPredictions.py` & `cspot-1.0.7/cspot/addPredictions.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/UNet-02032023.py` & `cspot-1.0.7/cspot/archives/UNet-02032023.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/gator-01272023.py` & `cspot-1.0.7/cspot/archives/gator-01272023.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/GPUselect.py` & `cspot-1.0.7/cspot/archives/toolbox-02032023/GPUselect.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/PartitionOfImage.py` & `cspot-1.0.7/cspot/archives/toolbox-02032023/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/PartitionOfImageOM.py` & `cspot-1.0.7/cspot/archives/toolbox-02032023/PartitionOfImageOM.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc` & `cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc` & `cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc` & `cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc` & `cspot-1.0.7/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/ftools.py` & `cspot-1.0.7/cspot/archives/toolbox-02032023/ftools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/imtools.py` & `cspot-1.0.7/cspot/archives/toolbox-02032023/imtools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/archives/toolbox-02032023/toolbox.py` & `cspot-1.0.7/cspot/archives/toolbox-02032023/toolbox.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/cloneFolder.py` & `cspot-1.0.7/cspot/cloneFolder.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/csExport.py` & `cspot-1.0.7/cspot/csExport.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/csObject.py` & `cspot-1.0.7/cspot/csObject.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/csPhenotype.py` & `cspot-1.0.7/cspot/csPhenotype.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/csPipeline.py` & `cspot-1.0.7/cspot/csPipeline.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/csPredict.py` & `cspot-1.0.7/cspot/csPredict.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/csTrain.py` & `cspot-1.0.7/cspot/csTrain.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/cspot.py` & `cspot-1.0.7/cspot/cspot.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/generateCSScore.py` & `cspot-1.0.7/cspot/generateCSScore.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/generateThumbnails.py` & `cspot-1.0.7/cspot/generateThumbnails.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/generateTrainTestSplit.py` & `cspot-1.0.7/cspot/generateTrainTestSplit.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/mergecsObject.py` & `cspot-1.0.7/cspot/mergecsObject.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/scatterPlot.py` & `cspot-1.0.7/cspot/scatterPlot.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/toolbox/GPUselect.py` & `cspot-1.0.7/cspot/toolbox/GPUselect.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/toolbox/PartitionOfImage.py` & `cspot-1.0.7/cspot/toolbox/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc` & `cspot-1.0.7/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc` & `cspot-1.0.7/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/toolbox/__pycache__/ftools.cpython-39.pyc` & `cspot-1.0.7/cspot/toolbox/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/toolbox/__pycache__/imtools.cpython-39.pyc` & `cspot-1.0.7/cspot/toolbox/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/cspot/toolbox/imtools.py` & `cspot-1.0.7/cspot/toolbox/imtools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.6/pyproject.toml` & `cspot-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cspot"
-version = "1.0.6"
+version = "1.0.7"
 description = "CELL SPOTTER (CSPOT): A scalable framework for automated processing of highly multiplexed tissue images"
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 readme = "README.md"
 
 keywords = ["image analysis","multiplex imaging","single cell analysis"]
 
 homepage = "https://pypi.org/project/cspot/"
@@ -24,15 +24,15 @@
 python = ">=3.8,<3.12"
 numpy = "^1.23.2"
 pandas = "^1.4.4"
 tifffile = "^2022.8.12"
 pathlib = "^1.0.1"
 dask = "^2022.8.1"
 zarr = "^2.12.0"
-tensorflow = "2.13.0rc1"
+tensorflow = "2.13.0rc0"
 opencv-python = "^4.6.0.66"
 anndata = "^0.8.0"
 scikit-learn = "^1.2.1"
 argparse = "^1.4.0"
 scikit-image = "^0.19.3"
 Brotli = "^1.0.9"
 matplotlib = "^3.7.1"
```

