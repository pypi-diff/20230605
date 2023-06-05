# Comparing `tmp/pdr-0.7.5.tar.gz` & `tmp/pdr-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-0.7.5.tar", last modified: Thu Mar 16 00:44:53 2023, max compression
+gzip compressed data, was "pdr-1.0.0.tar", last modified: Mon Jun  5 15:59:17 2023, max compression
```

## Comparing `pdr-0.7.5.tar` & `pdr-1.0.0.tar`

### file list

```diff
@@ -1,46 +1,61 @@
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-03-16 18:45:51.892622 pdr-0.7.5/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1524 2022-10-26 20:37:15.000000 pdr-0.7.5/LICENSE
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    10715 2023-03-16 18:45:51.892622 pdr-0.7.5/PKG-INFO
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    10137 2022-10-31 22:45:51.000000 pdr-0.7.5/README.md
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-03-16 18:45:50.821980 pdr-0.7.5/pdr/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      552 2023-03-16 18:40:21.000000 pdr-0.7.5/pdr/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5289 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/bit_handling.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    11531 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/browsify.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     7121 2023-03-16 18:40:21.000000 pdr-0.7.5/pdr/datatypes.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-03-16 18:45:51.703567 pdr-0.7.5/pdr/formats/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      572 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/formats/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     4527 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/formats/cassini.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      812 2023-01-18 16:32:19.000000 pdr-0.7.5/pdr/formats/clementine.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    18250 2023-03-16 18:40:21.000000 pdr-0.7.5/pdr/formats/core.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      869 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/formats/diviner.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      590 2022-10-26 20:37:15.000000 pdr-0.7.5/pdr/formats/galileo.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1322 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/formats/juno.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      371 2022-10-26 20:37:15.000000 pdr-0.7.5/pdr/formats/lroc.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1202 2022-12-29 21:12:41.000000 pdr-0.7.5/pdr/formats/m3.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      259 2022-12-28 18:49:22.000000 pdr-0.7.5/pdr/formats/messenger.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      415 2023-01-18 16:32:19.000000 pdr-0.7.5/pdr/formats/mex_marsis.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     2368 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/formats/mgn.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      321 2023-03-16 18:40:21.000000 pdr-0.7.5/pdr/formats/mgs.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      247 2022-10-26 20:37:15.000000 pdr-0.7.5/pdr/formats/msl_apxs.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      304 2022-10-26 20:37:15.000000 pdr-0.7.5/pdr/formats/msl_ccam.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1199 2022-10-31 22:45:51.000000 pdr-0.7.5/pdr/formats/msl_cmn.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      427 2022-10-31 22:45:51.000000 pdr-0.7.5/pdr/formats/rosetta.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3337 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/np_utils.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-03-16 18:45:51.861276 pdr-0.7.5/pdr/parselabel/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-10-26 20:37:15.000000 pdr-0.7.5/pdr/parselabel/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    11010 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/parselabel/pds3.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1395 2022-10-31 22:45:51.000000 pdr-0.7.5/pdr/parselabel/pds4.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      731 2023-03-16 18:40:21.000000 pdr-0.7.5/pdr/parselabel/utils.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     7247 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/pd_utils.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    62412 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/pdr.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      490 2022-10-26 20:37:15.000000 pdr-0.7.5/pdr/pvl_utils.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1280 2022-10-26 20:37:15.000000 pdr-0.7.5/pdr/rasterio_utils.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5691 2023-03-13 20:38:40.000000 pdr-0.7.5/pdr/utils.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-03-16 18:45:50.947105 pdr-0.7.5/pdr.egg-info/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    10715 2023-03-16 18:45:50.000000 pdr-0.7.5/pdr.egg-info/PKG-INFO
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      801 2023-03-16 18:45:50.000000 pdr-0.7.5/pdr.egg-info/SOURCES.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        1 2023-03-16 18:45:50.000000 pdr-0.7.5/pdr.egg-info/dependency_links.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      177 2023-03-16 18:45:50.000000 pdr-0.7.5/pdr.egg-info/requires.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        4 2023-03-16 18:45:50.000000 pdr-0.7.5/pdr.egg-info/top_level.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       38 2023-03-16 18:45:51.892622 pdr-0.7.5/setup.cfg
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1076 2023-03-16 18:40:21.000000 pdr-0.7.5/setup.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.171064 pdr-1.0.0/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-02 18:30:59.000000 pdr-1.0.0/LICENSE
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-05 15:59:17.171064 pdr-1.0.0/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10315 2023-06-05 15:54:39.000000 pdr-1.0.0/README.md
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.167063 pdr-1.0.0/pdr/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      560 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3956 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/_scaling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5212 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/bit_handling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11544 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/browsify.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7128 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/datatypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       97 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/errors.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.167063 pdr-1.0.0/pdr/formats/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      602 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3846 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/cassini.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    12685 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/checkers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      940 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/clementine.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      650 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/diviner.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      993 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/galileo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      884 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/juno.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1940 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/lro.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      125 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/lroc.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      335 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/mex_marsis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/mgn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      420 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/mgs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      214 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/msl_apxs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      210 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/msl_ccam.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      518 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/msl_cmn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      530 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/pvo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      221 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/rosetta.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1053 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/themis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5457 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/func.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.171064 pdr-1.0.0/pdr/loaders/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/_helpers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4623 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/datawrap.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4398 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/dispatch.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2767 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/handlers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5219 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/image.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    17607 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/queries.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6429 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/table.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2473 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/text.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1516 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/utility.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3493 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/np_utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.171064 pdr-1.0.0/pdr/parselabel/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.0/pdr/parselabel/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11104 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/parselabel/pds3.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1397 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/parselabel/pds4.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      731 2023-05-02 18:30:59.000000 pdr-1.0.0/pdr/parselabel/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7294 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/pd_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    26437 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/pdr.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      208 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/pdrtypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      490 2023-05-02 18:30:59.000000 pdr-1.0.0/pdr/pvl_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6652 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.167063 pdr-1.0.0/pdr.egg-info/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1086 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/SOURCES.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/dependency_links.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      177 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/requires.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/top_level.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-06-05 15:59:17.171064 pdr-1.0.0/setup.cfg
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1076 2023-06-05 15:54:44.000000 pdr-1.0.0/setup.py
```

### Comparing `pdr-0.7.5/LICENSE` & `pdr-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdr-0.7.5/PKG-INFO` & `pdr-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 0.7.5
+Version: 1.0.0
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -24,14 +24,17 @@
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
 (under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](supported_datasets.md) 
 
 If the software fails while attempting to read from datasets that we have listed as supported, please submit an issue with a link to the file and information about the error (if applicable). There might also be datasets that work but are not listed. We would like to hear about those too. If a dataset is not yet supported that you would like us to consider prioritizing, [please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
 
+### Attribution
+If you use _pdr_ in your work, please cite us using our Zenodo DOI: [![DOI](https://zenodo.org/badge/266449940.svg)](https://zenodo.org/badge/latestdoi/266449940)
+
 ### Installation
 _pdr_ is now on `conda` and `pip`. We recommend (and only officially support) installation into a `conda` environment.
 You can do this like so: 
 
 ```
 conda create --name pdrenv
 conda activate pdrenv
@@ -52,15 +55,15 @@
   - `pillow`: adds support for TIFF files and browse image rendering
   - `matplotlib`: allows usage of `save_sparklines`, an experimental browse function
 
 ### Usage
 
 (You can check out our example Notebook on Binder for a 
 quick interactive demo of functionality: 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/master))
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/main))
 
 Just open and python shell and run `import pdr` and then `pdr.read(filename)`, 
 where _filename_ is the full path to a data file _or_ a metadata / label file 
 (extensions .LBL, .lbl, or .xml). `read()` will look for corresponding data 
 or metadata files in the same path, or read metadata directly from the data file 
 if it has an attached label.
```

### Comparing `pdr-0.7.5/README.md` & `pdr-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
 (under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](supported_datasets.md) 
 
 If the software fails while attempting to read from datasets that we have listed as supported, please submit an issue with a link to the file and information about the error (if applicable). There might also be datasets that work but are not listed. We would like to hear about those too. If a dataset is not yet supported that you would like us to consider prioritizing, [please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
 
+### Attribution
+If you use _pdr_ in your work, please cite us using our Zenodo DOI: [![DOI](https://zenodo.org/badge/266449940.svg)](https://zenodo.org/badge/latestdoi/266449940)
+
 ### Installation
 _pdr_ is now on `conda` and `pip`. We recommend (and only officially support) installation into a `conda` environment.
 You can do this like so: 
 
 ```
 conda create --name pdrenv
 conda activate pdrenv
@@ -32,15 +35,15 @@
   - `pillow`: adds support for TIFF files and browse image rendering
   - `matplotlib`: allows usage of `save_sparklines`, an experimental browse function
 
 ### Usage
 
 (You can check out our example Notebook on Binder for a 
 quick interactive demo of functionality: 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/master))
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/main))
 
 Just open and python shell and run `import pdr` and then `pdr.read(filename)`, 
 where _filename_ is the full path to a data file _or_ a metadata / label file 
 (extensions .LBL, .lbl, or .xml). `read()` will look for corresponding data 
 or metadata files in the same path, or read metadata directly from the data file 
 if it has an attached label.
```

### Comparing `pdr-0.7.5/pdr/__init__.py` & `pdr-1.0.0/pdr/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path as _osp
 
-from pdr.pdr import Data, Metadata
-from pdr.utils import check_cases
-
-__version__ = "0.7.5"
+__version__ = "1.0.0"
 
 pkg_dir = _osp.abspath(_osp.dirname(__file__))
 
 
 def read(fp, **kwargs):
+    from pdr.pdr import Data, Metadata
+    from pdr.utils import check_cases
+
     try:
         return Data(fp, **kwargs)
     except FileNotFoundError:
-        if any(val in str(fp) for val in ['http', 'www.', 'ftp:']):
+        if any(val in str(fp) for val in ["http", "www.", "ftp:"]):
             raise ValueError(
                 "Support for read from url is not currently implemented."
             )
         return Data(check_cases(fp), **kwargs)
 
 
 def open(fp, **kwargs):
```

### Comparing `pdr-0.7.5/pdr/bit_handling.py` & `pdr-1.0.0/pdr/bit_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """utilities for parsing BIT_COLUMN objects in tables."""
 from functools import partial, reduce
 from operator import add
 
 import numpy as np
 import pandas as pd
 from pdr.datatypes import determine_byte_order, sample_types
-from pdr.formats import check_special_bit_column_case, check_special_bit_start_case
+from pdr.formats import (
+    check_special_bit_column_case, check_special_bit_start_case
+)
 import warnings
 
 
 def expand_bit_strings(table, fmtdef):
     if "start_bit_list" not in fmtdef.columns:
         return table
     table = convert_to_full_bit_string(table, fmtdef)
@@ -27,15 +29,15 @@
             table[fmtdef.NAME[column]] = bit_str_column
     return table
 
 
 def factor_to_dtype(field_length, byte_order):
     lengths = [1, 2, 4, 8]
     if field_length in lengths:
-        return np.dtype([('0', f"{byte_order}u{field_length}")])
+        return np.dtype([("0", f"{byte_order}u{field_length}")])
     dtype, remaining_length = [], field_length
     n = 0
     while remaining_length > 0:
         if remaining_length - lengths[-1] < 0:
             lengths.pop()
             continue
         dtype.append((str(n), f"{byte_order}u{lengths[-1]}"))
@@ -67,76 +69,81 @@
         if isinstance(fmtdef.start_bit_list[column], list):
             bit_column = table[fmtdef.NAME[column]]
             start_bit_list = [
                 val - 1 for val in fmtdef.start_bit_list[column]
             ]  # python zero indexing
             bit_size_list = fmtdef.bit_size_list[column]
             bit_list_column = bit_column.map(
-                partial(split_bits, start_bit_list=start_bit_list, bit_size_list=bit_size_list)
+                partial(
+                    split_bits,
+                    start_bit_list=start_bit_list,
+                    bit_size_list=bit_size_list,
+                )
             )
             table[fmtdef.NAME[column]] = bit_list_column
     return table
 
 
 def split_bits(bit_string, start_bit_list, bit_size_list):
-    end_bit_list = [start + size
-                    for start, size in zip(start_bit_list, bit_size_list)]
+    end_bit_list = [
+        start + size for start, size in zip(start_bit_list, bit_size_list)
+    ]
     return [
         bit_string[start:end]
         for start, end in zip(start_bit_list, end_bit_list)
     ]
 
 
-def set_bit_string_data_type(obj, data):
-    is_special, special_dtype = check_special_bit_column_case(data)
+def set_bit_string_data_type(obj, identifiers):
+    is_special, special_dtype = check_special_bit_column_case(identifiers)
     if is_special is False:
         try:
-            byteorder = sample_types(obj["BIT_COLUMN"]["BIT_DATA_TYPE"], 1, True)[0]
+            byteorder = sample_types(
+                obj["BIT_COLUMN"]["BIT_DATA_TYPE"], 1, True
+            )[0]
         except (KeyError, ValueError):
             raise ValueError("Incompatible data type for bit columns.")
         if byteorder == ">":
-            warnings.warn(f"Data type {obj['DATA_TYPE']} incompatible for bit column. "
-                          f"Changing to MSB_BIT_STRING.")
+            warnings.warn(
+                f"Data type {obj['DATA_TYPE']} incompatible for bit column. "
+                f"Changing to MSB_BIT_STRING."
+            )
             obj["DATA_TYPE"] = "MSB_BIT_STRING"
         elif byteorder == "<":
-            warnings.warn(f"Data type {obj['DATA_TYPE']} incompatible for bit column. "
-                          f"Changing to LSB_BIT_STRING.")
+            warnings.warn(
+                f"Data type {obj['DATA_TYPE']} incompatible for bit column. "
+                f"Changing to LSB_BIT_STRING."
+            )
             obj["DATA_TYPE"] = "LSB_BIT_STRING"
     else:
         obj["DATA_TYPE"] = special_dtype
     return obj
 
 
-def get_bit_start_and_size(obj, definition, data):
+def get_bit_start_and_size(obj, definition, identifiers):
     start_bit_list = []
     bit_size_list = []
     list_of_pvl_objects_for_bit_columns = definition.getall("BIT_COLUMN")
     for pvl_obj in list_of_pvl_objects_for_bit_columns:
         if pvl_obj.get("ITEMS"):
             items = pvl_obj.get("ITEMS")
             item_bits = pvl_obj.get("ITEM_BITS")
             first_item_start_bit = pvl_obj.get("START_BIT")
             for item_index in range(items):
-                start_bit = first_item_start_bit + item_index*item_bits
+                start_bit = first_item_start_bit + item_index * item_bits
                 start_bit_list.append(start_bit)
                 bit_size_list.append(item_bits)
         else:
             start_bit = pvl_obj.get("START_BIT")
             bit_size = pvl_obj.get("BITS")
             start_bit_list.append(start_bit)
             bit_size_list.append(bit_size)
-    is_also_special, special_start_bit_list = \
-        check_special_bit_start_case(data, list_of_pvl_objects_for_bit_columns, start_bit_list)
+    is_also_special, special_start_bit_list = check_special_bit_start_case(
+        identifiers, list_of_pvl_objects_for_bit_columns, start_bit_list
+    )
     if is_also_special:
         obj["start_bit_list"] = special_start_bit_list
     else:
         obj["start_bit_list"] = start_bit_list
     obj["bit_size_list"] = bit_size_list
     return obj
 
-
-def add_bit_column_info(obj, definition, data):
-    if "BIT_COLUMN" in obj.keys():
-        if "BIT_STRING" not in obj["DATA_TYPE"]:
-            obj = set_bit_string_data_type(obj, data)
-        obj = get_bit_start_and_size(obj, definition, data)
-    return obj
```

### Comparing `pdr-0.7.5/pdr/browsify.py` & `pdr-1.0.0/pdr/browsify.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,22 +79,22 @@
         if inplace is True:
             image = np.clip(image, minimum, maximum, out=image)
         else:
             image = np.clip(image, minimum, maximum)
     if inplace is True:
         # perform the operation in-place
         image -= minimum
-        image *= (range_max - range_min)
-        if image.dtype.char in np.typecodes['AllInteger']:
+        image *= range_max - range_min
+        if image.dtype.char in np.typecodes["AllInteger"]:
             # this loss of precision is probably better than
             # automatically typecasting it.
             # TODO: detect rollover cases, etc.
-            image //= (maximum - minimum)
+            image //= maximum - minimum
         else:
-            image /= (maximum - minimum)
+            image /= maximum - minimum
         image += range_min
         return image
     return (image - minimum) * (range_max - range_min) / (
         maximum - minimum
     ) + range_min
 
 
@@ -191,15 +191,15 @@
     purge: bool = False,
     image_clip: Union[float, tuple[float, float]] = (1, 1),
     mask_color: Optional[tuple[int, int, int]] = (0, 255, 255),
     band_ix: Optional[int] = None,
     save: bool = True,
     override_rgba: bool = False,
     image_format: str = "jpg",
-    **_
+    **_,
 ):
     """
     attempt to save array as one or more images
     """
     if len(obj.shape) == 3:
         obj = _format_multiband_image(obj, band_ix, override_rgba)
     if not isinstance(obj, tuple):
@@ -211,25 +211,25 @@
         result = _render_and_save(
             band,
             f"{outbase}_{ix}",
             purge,
             image_clip,
             mask_color,
             save,
-            image_format
+            image_format,
         )
         results.append(result)
     return results
 
 
 def _render_and_save(
     obj, outbase, purge, image_clip, mask_color, save, image_format
 ):
     # upcast integer data types < 32-bit to prevent unhelpful wraparound
-    if (obj.dtype.char in np.typecodes['AllInteger']) and (obj.itemsize <= 2):
+    if (obj.dtype.char in np.typecodes["AllInteger"]) and (obj.itemsize <= 2):
         obj = obj.astype(np.int32)
     # convert to unsigned eight-bit integer to make it easy to write
     obj = eightbit(obj, image_clip, purge)
     # unless color_fill is set to None, fill masked elements -- probably
     # special constants -- with RGB value defined by mask_color
     if isinstance(obj, np.ma.MaskedArray) and (mask_color is not None):
         obj = colorfill_maskedarray(obj, mask_color)
@@ -301,27 +301,29 @@
         )
         return obj[middle_ix]
 
 
 def save_sparklines(
     df: pd.DataFrame,
     outbase,
-    sparkline_column_key = lambda c: 'spectrum' in c.lower(),
-    orientation = 'rows'
+    sparkline_column_key=lambda c: "spectrum" in c.lower(),
+    orientation="rows",
 ):
     from matplotlib import pyplot as plt
 
-    sparkframe = df[
-        [c for c in df.columns if sparkline_column_key(c)]
-    ].copy().reset_index(drop=True)
+    sparkframe = (
+        df[[c for c in df.columns if sparkline_column_key(c)]]
+        .copy()
+        .reset_index(drop=True)
+    )
 
     fig, ax = plt.subplots()
-    if orientation == 'rows':
+    if orientation == "rows":
         height = (sparkframe.max(axis=1) - sparkframe.min(axis=1)).iloc[0]
         for ix, row in sparkframe.iterrows():
             ax.plot(row.values + height * ix)
     else:
         height = (sparkframe.max(axis=0) - sparkframe.min(axis=0)).iloc[0]
         for ix, colvals in enumerate(sparkframe.iteritems()):
             ax.plot(colvals[1].values + height * ix)
     fig.savefig(outbase + "_sparklines.jpg")
-    plt.close('all')
+    plt.close("all")
```

### Comparing `pdr-0.7.5/pdr/datatypes.py` & `pdr-1.0.0/pdr/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,32 +51,32 @@
         signed = "UNSIGNED" not in sample_type
         return integer_bytes(endian, signed, sample_bytes, for_numpy)
     void = "V" if for_numpy is True else "s"
     _float = "d" if sample_bytes == 8 else "f"
     return {
         "IEEE_REAL": f">{_float}",
         "PC_REAL": f"<{_float}",
-        "FLOAT":  f">{_float}",
-        "REAL":  f">{_float}",
-        "MAC_REAL":  f">{_float}",
-        "SUN_REAL":  f">{_float}",
+        "FLOAT": f">{_float}",
+        "REAL": f">{_float}",
+        "MAC_REAL": f">{_float}",
+        "SUN_REAL": f">{_float}",
         "MSB_BIT_STRING": f"{void}{sample_bytes}",
         "LSB_BIT_STRING": f"{void}{sample_bytes}",
         # "Character string representing a real number"
         "ASCII_REAL": f"S{sample_bytes}",
         # ASCII character string representing an integer
         "ASCII_INTEGER": f"S{sample_bytes}",
         # "ASCII character string representing a date in PDS standard format"
         # (e.g. 1990-08-01T23:59:59)
         "DATE": f"S{sample_bytes}",
         "CHARACTER": f"S{sample_bytes}",  # ASCII character string
         "TIME": f"S{sample_bytes}",
         "VOID": f"{void}{sample_bytes}",
         "BCD": f"{void}{sample_bytes}",
-        "BINARY_CODED_DECIMAL": f"{void}{sample_bytes}"
+        "BINARY_CODED_DECIMAL": f"{void}{sample_bytes}",
     }[sample_type]
 
 
 # "basic" PDS3 special constants
 PDS3_CONSTANT_NAMES = (
     "INVALID_CONSTANT",
     "MISSING_CONSTANT",
@@ -87,17 +87,17 @@
 )
 # some (all?) of these are derived from ISIS properties; these are names they
 # take on when they are made explicit in a PDS3 label
 PDS3_ISIS_CONSTANT_NAMES = tuple(
     [
         f"{category}{direction}{entity}{prop}"
         for category, direction, entity, prop in product(
-            ("CORE_", "BAND_SUFFIX_", "SAMPLE_SUFFIX", "LINE_SUFFIX", ""),
-            ("HIGH_", "LOW_"),
-            ("INST_", "REPR_"),
+            ("CORE_", "BAND_SUFFIX_", "SAMPLE_SUFFIX_", "LINE_SUFFIX_", ""),
+            ("HIGH_", "LOW_", ""),
+            ("INST_", "REPR_", ""),
             ("NULL", "SATURATION", "SAT"),
         )
     ]
 )
 # noinspection PyTypeChecker
 PDS3_CONSTANT_NAMES = tuple(PDS3_ISIS_CONSTANT_NAMES + PDS3_CONSTANT_NAMES)
 # this dictionary contains common "implicit" (not specified in the label)
```

### Comparing `pdr-0.7.5/pdr/formats/__init__.py` & `pdr-1.0.0/pdr/formats/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from .core import *
+from .checkers import *
 import pdr.formats.cassini as cassini
 import pdr.formats.clementine as clementine
 import pdr.formats.diviner as diviner
 import pdr.formats.galileo as galileo
 import pdr.formats.juno as juno
 import pdr.formats.lroc as lroc
-import pdr.formats.m3 as m3
-import pdr.formats.messenger as messenger
+import pdr.formats.lro as lro
 import pdr.formats.mex_marsis as mex_marsis
 import pdr.formats.mgn as mgn
 import pdr.formats.mgs as mgs
 import pdr.formats.msl_apxs as msl_apxs
 import pdr.formats.msl_cmn as msl_cmn
 import pdr.formats.msl_ccam as msl_ccam
+import pdr.formats.pvo as pvo
 import pdr.formats.rosetta as rosetta
+import pdr.formats.themis as themis
```

### Comparing `pdr-0.7.5/pdr/formats/clementine.py` & `pdr-1.0.0/pdr/formats/clementine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import re
-import pandas as pd
-from pdr.pd_utils import insert_sample_types_into_df
+
+import pdr.loaders.queries
 
 
 def get_offset(data, pointer):
-    start_row = int(re.split(r',|[(|)]', data.metadata[f'^{pointer}'])[2])
-    return True, (start_row - 1) * data.metadata['RECORD_BYTES']
+    start_row = int(re.split(r",|[(|)]", data.metadata[f"^{pointer}"])[2])
+    return True, (start_row - 1) * data.metadata["RECORD_BYTES"]
 
 
 def get_fn(data, object_name):
-    target = re.split(r',|[(|)]', data.metadata[f'^{object_name}'])[1]
+    target = re.split(r",|[(|)]", data.metadata[f"^{object_name}"])[1]
     return True, target
 
 
-def get_structure(pointer, data):
-    fmtdef = data.read_table_structure(pointer)
+def get_structure(block, name, filename, data, identifiers):
+    fmtdef = pdr.loaders.queries.read_table_structure(
+        block, name, filename, data, identifiers
+    )
+    import pandas as pd
+
     fmtdef = pd.concat([fmtdef, fmtdef], ignore_index=True)
-    fmtdef['NAME'] = fmtdef['NAME'].str.split('_', expand=True)[0]
-    fmtdef['NAME'] = fmtdef['NAME'].str.cat(map(str, fmtdef.index), sep='_')
+    fmtdef["NAME"] = fmtdef["NAME"].str.split("_", expand=True)[0]
+    fmtdef["NAME"] = fmtdef["NAME"].str.cat(map(str, fmtdef.index), sep="_")
     fmtdef.ITEM_OFFSET = 8
     fmtdef.ITEM_BYTES = 8
-    fmtdef, dt = insert_sample_types_into_df(fmtdef, data)
-    return True, fmtdef, dt
+    from pdr.pd_utils import insert_sample_types_into_df
+
+    fmtdef, dt = insert_sample_types_into_df(fmtdef, identifiers)
+    return fmtdef, dt
```

### Comparing `pdr-0.7.5/pdr/formats/mgn.py` & `pdr-1.0.0/pdr/formats/mgn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 from io import StringIO
+
 from pdr.utils import head_file
-from pdr.pd_utils import compute_offsets
-import pandas as pd
 
 
-def geom_table_loader(data, pointer):
+def geom_table_loader(filename, fmtdef_dt):
     """
     The Magellan radar system geometry tables include null bytes between rows.
     """
-    def load_mgn_geom_table(*_, **__):
-        import pandas as pd
-        from pdr.utils import head_file
-
-        fmtdef, dt = data.parse_table_structure(pointer)
-        with head_file(data.file_mapping[pointer]) as buf:
-            bytes_ = buf.read().replace(b"\x00", b"")
-        string_buffer = StringIO(bytes_.decode())
-        string_buffer.seek(0)
-        table = pd.read_csv(string_buffer, header=None)
-        assert len(table.columns) == len(fmtdef.NAME.tolist())
-        string_buffer.close()
-        table.columns = fmtdef.NAME.tolist()
-        return table
-    return load_mgn_geom_table
+    import pandas as pd
+    from pdr.utils import head_file
+
+    fmtdef, dt = fmtdef_dt
+    with head_file(filename) as buf:
+        bytes_ = buf.read().replace(b"\x00", b"")
+    string_buffer = StringIO(bytes_.decode())
+    string_buffer.seek(0)
+    table = pd.read_csv(string_buffer, header=None)
+    assert len(table.columns) == len(fmtdef.NAME.tolist())
+    string_buffer.close()
+    table.columns = fmtdef.NAME.tolist()
+    return table
 
 
-def orbit_table_in_img_loader(data, pointer):
-    return data.trivial
+def orbit_table_in_img_loader():
+    return True
 
 
 def get_fn(data):
     target = data.filename
     return True, target
 
 
-def occultation_loader(data, pointer):
-    def load_occult_table(*_, **__):
-        fmtdef, dt = data.parse_table_structure(pointer)
-        record_length = data.metablock_(pointer)['ROW_BYTES']
-
-        # Checks end of each row for newline character. If missing, removes extraneous
-        # newline from middle of the row and adjusts for the extra byte.
-        with head_file(data.file_mapping[pointer]) as f:
-            processed = bytearray()
-            for row in range(0, data.metadata["FILE_RECORDS"]):
-                bytes_ = f.read(record_length)
-                if not bytes_.endswith(b'\n'):
-                    new_bytes_ = bytes_.replace(b'\n', b'') + f.read(1)
-                    processed += new_bytes_
-                else:
-                    processed += bytes_
-        string_buffer = StringIO(processed.decode())
-
-        # adapted from _interpret_as_ascii()
-        colspecs = []
-        position_records = compute_offsets(fmtdef).to_dict('records')
-        for record in position_records:
-            col_length = record['BYTES']
-            colspecs.append((record['OFFSET'], record['OFFSET'] + col_length))
-        string_buffer.seek(0)
-        table = pd.read_fwf(string_buffer, header=None, colspecs=colspecs)
-        string_buffer.close()
-
-        table.columns = fmtdef.NAME.tolist()
-        return table
-    return load_occult_table
+def occultation_loader(identifiers, fmtdef_dt, block, filename):
+    import pandas as pd
+
+    fmtdef, dt = fmtdef_dt
+    record_length = block["ROW_BYTES"]
+
+    # Checks end of each row for newline character. If missing, removes extraneous
+    # newline from middle of the row and adjusts for the extra byte.
+    with head_file(filename) as f:
+        processed = bytearray()
+        for row in range(0, identifiers["FILE_RECORDS"]):
+            bytes_ = f.read(record_length)
+            if not bytes_.endswith(b"\n"):
+                new_bytes_ = bytes_.replace(b"\n", b"") + f.read(1)
+                processed += new_bytes_
+            else:
+                processed += bytes_
+    string_buffer = StringIO(processed.decode())
+    # adapted from _interpret_as_ascii()
+    colspecs = []
+    from pdr.pd_utils import compute_offsets
+
+    position_records = compute_offsets(fmtdef).to_dict("records")
+    for record in position_records:
+        col_length = record["BYTES"]
+        colspecs.append((record["OFFSET"], record["OFFSET"] + col_length))
+    string_buffer.seek(0)
+    table = pd.read_fwf(string_buffer, header=None, colspecs=colspecs)
+    string_buffer.close()
+
+    table.columns = fmtdef.NAME.tolist()
+    return table
+
+
+def gvanf_sample_type():
+    return ">B"
```

### Comparing `pdr-0.7.5/pdr/np_utils.py` & `pdr-1.0.0/pdr/np_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,21 +69,27 @@
 # TODO: shake this out with a bunch of different compression type examples,
 #  including specific compressions on band/line/single-plane/etc. images,
 #  compressed binary tables, etc.
 def np_from_buffered_io(
     buffered_io: BufferedIOBase,
     dtype: Union[np.dtype, str],
     offset: Optional[int] = None,
-    count: Optional[int] = None
+    count: Optional[int] = None,
 ):
     """
     return a numpy array from a buffered IO object, first decompressing it in
     memory if it's a compressed buffer, and just using np.fromfile if it's not
     """
     if offset is not None:
         buffered_io.seek(offset)
     if isinstance(buffered_io, (BZ2File, ZipFile, GzipFile, BytesIO)):
         n_bytes = None if count is None else count * dtype.itemsize
         stream = BytesIO(buffered_io.read(n_bytes))
         return np.frombuffer(stream.getbuffer(), dtype=dtype)
     count = -1 if count is None else count
     return np.fromfile(buffered_io, dtype=dtype, count=count)
+
+
+def make_c_contiguous(arr: np.ndarray) -> np.ndarray:
+    if arr.flags["C_CONTIGUOUS"] is False:
+        return np.ascontiguousarray(arr)
+    return arr
```

### Comparing `pdr-0.7.5/pdr/parselabel/pds3.py` & `pdr-1.0.0/pdr/parselabel/pds3.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,16 @@
 
 def looks_pvl(filename):
     return Path(filename).suffix.lower() in (".lbl", ".fmt")
 
 
 def read_pvl(filename, deduplicate_pointers=True, max_size=DEFAULT_PVL_LIMIT):
     with decompress(filename) as stream:
-        errors = 'replace' if looks_pvl(filename) else 'strict'
-        label = trim_label(stream, max_size).decode('utf-8', errors=errors)
+        errors = "replace" if looks_pvl(filename) else "strict"
+        label = trim_label(stream, max_size).decode("utf-8", errors=errors)
     uncommented_label = re.sub(r"/\*.*?(\r|\n|/\*)", "", label)
     trimmed_lines = filter(
         None, map(lambda line: line.strip(), uncommented_label.split("\n"))
     )
     statements = chunk_statements(trimmed_lines)
     mapping, params = BlockParser().parse_statements(statements)
     if deduplicate_pointers:
@@ -222,14 +222,16 @@
             return literal_eval(obj)
     except (SyntaxError, ValueError):
         # note: this is very permissive, and handled downstream with a simple
         #  exception catch that should work for most cases.
         if ("<" in obj) and (">" in obj):
             return parse_pvl_quantity_statement(obj)
         return obj
+        # TODO, maybe: handle sequences/sets containing unquoted character
+        #  strings
 
 
 def literalize_pvl_block(block):
     literalized = multidict_dig_and_edit(
         block,
         None,
         predicate=lambda x, y: True,
```

### Comparing `pdr-0.7.5/pdr/parselabel/pds4.py` & `pdr-1.0.0/pdr/parselabel/pds4.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
 # noinspection PyTypeChecker
 def reformat_pds4_tools_label(label):
     result = dig_and_edit(
         label.to_dict(),
         constant(True),
         lambda _, v: unpack_if_mapping(v, (OrderedDict, MultiDict)),
-        mtypes=(OrderedDict, MultiDict)
+        mtypes=(OrderedDict, MultiDict),
     )
     params = []
     # collect all keys to populate pdr.Metadata's fieldcounts attribute
     dig_and_edit(
         result,
         constant(True),
         lambda k, v: log_and_pass(params, k, v),
-        mtypes=(MultiDict,)
+        mtypes=(MultiDict,),
     )
     return result, params
```

### Comparing `pdr-0.7.5/pdr/parselabel/utils.py` & `pdr-1.0.0/pdr/parselabel/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-0.7.5/pdr/pd_utils.py` & `pdr-1.0.0/pdr/pd_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,134 +39,134 @@
             name = f"RESERVED_{field_group['START_BYTE'].iloc[0]}"
         names = [f"{name}_{ix}" for ix in range(len(field_group))]
         df.loc[field_group.index, column] = names
     return df
 
 
 def _apply_item_offsets(fmtdef):
-    item_offsets = fmtdef['ITEM_BYTES'].copy()
+    item_offsets = fmtdef["ITEM_BYTES"].copy()
     if "ITEM_OFFSET" not in fmtdef.columns:
         return item_offsets
-    offset = fmtdef.loc[fmtdef['ITEM_OFFSET'].notna()]
-    if (offset['ITEM_OFFSET'] < offset['ITEM_BYTES']).any():
+    offset = fmtdef.loc[fmtdef["ITEM_OFFSET"].notna()]
+    if (offset["ITEM_OFFSET"] < offset["ITEM_BYTES"]).any():
         raise ValueError(
             "Don't know how to intepret a field narrower than its value."
         )
-    item_offsets.loc[offset.index] = offset['ITEM_OFFSET']
+    item_offsets.loc[offset.index] = offset["ITEM_OFFSET"]
     return item_offsets
 
 
 def compute_offsets(fmtdef):
     """
     given a DataFrame containing PDS3 binary table structure specifications,
     including a START_BYTE column, add an OFFSET column, unpacking objects
     if necessary
     """
     # START_BYTE is 1-indexed, but we're preparing these offsets for
     # numpy, which 0-indexes
-    fmtdef['OFFSET'] = fmtdef['START_BYTE'] - 1
-    if 'ROW_PREFIX_BYTES' in fmtdef.columns:
-        fmtdef['OFFSET'] += fmtdef['ROW_PREFIX_BYTES']
-    block_names = fmtdef['BLOCK_NAME'].unique()
+    fmtdef["OFFSET"] = fmtdef["START_BYTE"] - 1
+    if "ROW_PREFIX_BYTES" in fmtdef.columns:
+        fmtdef["OFFSET"] += fmtdef["ROW_PREFIX_BYTES"]
+    block_names = fmtdef["BLOCK_NAME"].unique()
     # calculate offsets for formats loaded in by reference
     for block_name in block_names[1:]:
-        fmt_block = fmtdef.loc[fmtdef['BLOCK_NAME'] == block_name]
+        fmt_block = fmtdef.loc[fmtdef["BLOCK_NAME"] == block_name]
         prior = fmtdef.loc[fmt_block.index[0] - 1]
-        fmtdef.loc[
-            fmt_block.index, 'OFFSET'
-        ] += prior['OFFSET'] + prior['BYTES']
+        fmtdef.loc[fmt_block.index, "OFFSET"] += (
+            prior["OFFSET"] + prior["BYTES"]
+        )
     # correctly compute offsets within columns w/multiple items
-    if 'ITEM_BYTES' in fmtdef:
-        fmtdef['ITEM_SIZE'] = _apply_item_offsets(fmtdef)
-        column_groups = fmtdef.loc[fmtdef['ITEM_SIZE'].notna()]
-        for _, group in column_groups.groupby('OFFSET'):
-            fmtdef.loc[group.index, 'OFFSET'] = (
-                group['OFFSET']
-                + int(group['ITEM_SIZE'].iloc[0])
-                * np.arange(len(group))
-            )
+    if "ITEM_BYTES" in fmtdef:
+        fmtdef["ITEM_SIZE"] = _apply_item_offsets(fmtdef)
+        column_groups = fmtdef.loc[fmtdef["ITEM_SIZE"].notna()]
+        for _, group in column_groups.groupby("OFFSET"):
+            fmtdef.loc[group.index, "OFFSET"] = group["OFFSET"] + int(
+                group["ITEM_SIZE"].iloc[0]
+            ) * np.arange(len(group))
     pad_length = 0
-    end_byte = fmtdef['OFFSET'].iloc[-1] + fmtdef['BYTES'].iloc[-1]
-    if 'ROW_BYTES' in fmtdef.columns:
-        pad_length += fmtdef['ROW_BYTES'].iloc[0] - end_byte
-    if 'ROW_SUFFIX_BYTES' in fmtdef.columns:
-        pad_length += fmtdef['ROW_SUFFIX_BYTES'].iloc[0]
+    end_byte = fmtdef["OFFSET"].iloc[-1] + fmtdef["BYTES"].iloc[-1]
+    if "ROW_BYTES" in fmtdef.columns:
+        pad_length += fmtdef["ROW_BYTES"].iloc[0] - end_byte
+    if "ROW_SUFFIX_BYTES" in fmtdef.columns:
+        pad_length += fmtdef["ROW_SUFFIX_BYTES"].iloc[0]
     if pad_length > 0:
         placeholder_rec = {
-            'NAME': 'PLACEHOLDER_0',
-            'DATA_TYPE': 'VOID',
-            'BYTES': pad_length,
-            'START_BYTE': end_byte,
-            'OFFSET': end_byte
+            "NAME": "PLACEHOLDER_0",
+            "DATA_TYPE": "VOID",
+            "BYTES": pad_length,
+            "START_BYTE": end_byte,
+            "OFFSET": end_byte,
         }
         fmtdef = pd.concat(
             [fmtdef, pd.DataFrame([placeholder_rec])]
         ).reset_index(drop=True)
     return fmtdef
 
 
 def _fill_empty_byte_rows(fmtdef):
-    nobytes = fmtdef['BYTES'].isna()
+    nobytes = fmtdef["BYTES"].isna()
     with warnings.catch_warnings():
         # we do not care that loc will set items inplace later. at all.
         warnings.simplefilter("ignore", category=FutureWarning)
-        fmtdef.loc[nobytes, 'BYTES'] = (
+        fmtdef.loc[nobytes, "BYTES"] = (
             # TODO, maybe: update with ITEM_OFFSET should we implement that
-            fmtdef.loc[nobytes, 'ITEMS'] * fmtdef.loc[nobytes, 'ITEM_BYTES']
+            fmtdef.loc[nobytes, "ITEMS"]
+            * fmtdef.loc[nobytes, "ITEM_BYTES"]
         )
-    fmtdef['BYTES'] = fmtdef['BYTES'].astype(int)
+    fmtdef["BYTES"] = fmtdef["BYTES"].astype(int)
     return fmtdef
 
 
-def insert_sample_types_into_df(fmtdef, data):
+def insert_sample_types_into_df(fmtdef, identifiers):
     """
     given a DataFrame containing PDS3 binary table structure specifications,
     insert numpy-compatible data type strings into that DataFrame;
     return that DataFrame along with a numpy dtype object generated from it.
     used in the Data.read_table pipeline.
     """
-    fmtdef['dt'] = None
-    if 'BYTES' not in fmtdef.columns:
-        fmtdef['BYTES'] = np.nan
-    if fmtdef['BYTES'].isna().any():
+    fmtdef["dt"] = None
+    if "BYTES" not in fmtdef.columns:
+        fmtdef["BYTES"] = np.nan
+    if fmtdef["BYTES"].isna().any():
         try:
             fmtdef = _fill_empty_byte_rows(fmtdef)
         except (KeyError, TypeError, IndexError):
             raise ValueError("This table's byte sizes are underspecified.")
-    if 'ITEM_BYTES' not in fmtdef.columns:
-        fmtdef['ITEM_BYTES'] = np.nan
-    if 'START_BYTE' in fmtdef.columns:
+    if "ITEM_BYTES" not in fmtdef.columns:
+        fmtdef["ITEM_BYTES"] = np.nan
+    if "START_BYTE" in fmtdef.columns:
         fmtdef = compute_offsets(fmtdef)
     data_types = tuple(
-        fmtdef.groupby(['DATA_TYPE', 'ITEM_BYTES', 'BYTES'], dropna=False)
+        fmtdef.groupby(["DATA_TYPE", "ITEM_BYTES", "BYTES"], dropna=False)
     )
     for data_type, group in data_types:
         dt, item_bytes, total_bytes = data_type
         sample_bytes = total_bytes if np.isnan(item_bytes) else item_bytes
         try:
+            samp_info = {"SAMPLE_TYPE": dt, "BYTES_PER_PIXEL": sample_bytes}
             is_special, special_type = check_special_sample_type(
-                data, dt, int(sample_bytes), for_numpy=True
+                identifiers, samp_info
             )
             if is_special:
-                fmtdef.loc[group.index, 'dt'] = special_type
+                fmtdef.loc[group.index, "dt"] = special_type
             else:
-                fmtdef.loc[group.index, 'dt'] = sample_types(
+                fmtdef.loc[group.index, "dt"] = sample_types(
                     dt, int(sample_bytes), for_numpy=True
                 )
         except KeyError:
             raise KeyError(
                 f"{data_type} is not a currently-supported data type."
             )
     dtype_spec = fmtdef[
-        [c for c in ('NAME', 'dt', 'OFFSET') if c in fmtdef.columns]
-    ].to_dict('list')
-    spec_keys = ('names', 'formats', 'offsets')[:len(dtype_spec)]
-    return(
+        [c for c in ("NAME", "dt", "OFFSET") if c in fmtdef.columns]
+    ].to_dict("list")
+    spec_keys = ("names", "formats", "offsets")[: len(dtype_spec)]
+    return (
         fmtdef,
-        np.dtype({k: v for k, v in zip(spec_keys, dtype_spec.values())})
+        np.dtype({k: v for k, v in zip(spec_keys, dtype_spec.values())}),
     )
 
 
 def booleanize_booleans(
     table: pd.DataFrame, fmtdef: pd.DataFrame
 ) -> pd.DataFrame:
     boolean_columns = fmtdef.loc[fmtdef["DATA_TYPE"] == "BOOLEAN", "NAME"]
```

### Comparing `pdr-0.7.5/pdr/utils.py` & `pdr-1.0.0/pdr/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 import bz2
 from io import BytesIO
 from itertools import chain
 from numbers import Number
 from pathlib import Path
 import struct
 import textwrap
-from typing import Union, Sequence, Mapping, MutableSequence, IO, Collection
+from typing import (
+    Union,
+    Sequence,
+    Mapping,
+    MutableSequence,
+    IO,
+    Collection,
+    Optional,
+)
 import warnings
 from zipfile import ZipFile
 
 from dustgoggles.structures import listify
 from multidict import MultiDict
 
-try:
-    from isal import igzip as gzip_lib
-except ImportError:
-    import gzip as gzip_lib
-
 
 def read_hex(hex_string: str, fmt: str = ">I") -> Number:
     """
     return the decimal representation of a hexadecimal number in a given
     number format (expressed as a struct-style format string, default is
     unsigned 32-bit integer)
     """
@@ -58,20 +61,20 @@
     lowercase = path.stem.lower()
     exts = tuple(map(str.lower, path.suffixes))
     if len(exts) == 0:
         return lowercase
     # don't remove compression suffix if it's the only suffix
     if (len(exts) == 1) or (exts[-1] in SUPPORTED_COMPRESSION_EXTENSIONS):
         return f"{lowercase}{exts[0]}"
-    return f"{lowercase}{''.join(exts)}"
+    return f"{lowercase}{exts[-1]}"
 
 
 def check_cases(
     filenames: Union[Collection[Union[Path, str]], Union[Path, str]],
-    skip: bool = False
+    skip: bool = False,
 ) -> str:
     """
     check for oddly-cased versions of a specified filename in local path --
     very common to have case mismatches between PDS3 labels and actual archive
     contents. similarly, check common compression extensions.
 
     the skip argument makes the function simply return filename.
@@ -120,17 +123,25 @@
         if repeat_count > 1:
             fields += [obj for _ in range(repeat_count)]
         else:
             fields.append(obj)
     return fields
 
 
+def import_best_gzip():
+    try:
+        from isal import igzip as gzip_lib
+    except ImportError:
+        import gzip as gzip_lib
+    return gzip_lib
+
+
 def decompress(filename):
     if filename.lower().endswith(".gz"):
-        f = gzip_lib.open(filename, "rb")
+        f = import_best_gzip().open(filename, "rb")
     elif filename.lower().endswith(".bz2"):
         f = bz2.BZ2File(filename, "rb")
     elif filename.lower().endswith(".zip"):
         f = ZipFile(filename, "r").open(
             ZipFile(filename, "r").infolist()[0].filename
         )
     else:
@@ -141,17 +152,17 @@
 def with_extension(fn: Union[str, Path], new_suffix: str) -> str:
     return str(Path(fn).with_suffix(new_suffix))
 
 
 def find_repository_root(absolute_path):
     parts = Path(absolute_path).parts
     data_indices = [
-        ix for ix, part in enumerate(parts) if part.lower() == 'data'
+        ix for ix, part in enumerate(parts) if part.lower() == "data"
     ]
-    return Path(*parts[:data_indices[-1]])
+    return Path(*parts[: data_indices[-1]])
 
 
 def prettify_multidict(multi, sep=" ", indent=0):
     indentation, output, first_line = "", "{", True
     for k, v in multi.items():
         if sep == "\n":
             indentation = " " * indent
@@ -174,7 +185,36 @@
         if sep != " ":
             continue
         if len(output) > 70:
             return prettify_multidict(multi, sep="\n", indent=indent + 1)
     if len(indentation) > 0:
         indentation = indentation[:-1]
     return output + indentation + "}"
+
+
+def associate_label_file(
+    data_filename: str,
+    label_filename: Optional[str] = None,
+    skip_check: bool = False,
+) -> Optional[str]:
+    from pdr.loaders.utility import LABEL_EXTENSIONS
+
+    if label_filename is not None:
+        return check_cases(Path(label_filename).absolute(), skip_check)
+    elif data_filename.lower().endswith(LABEL_EXTENSIONS):
+        return check_cases(data_filename)
+    for lext in LABEL_EXTENSIONS:
+        try:
+            return check_cases(with_extension(data_filename, lext))
+        except FileNotFoundError:
+            continue
+    return None
+
+
+def catch_return_default(debug: bool, return_default, exception: Exception):
+    """
+    if we are in debug mode, reraise an exception. otherwise, return
+    the default only.
+    """
+    if debug is True:
+        raise exception
+    return return_default
```

### Comparing `pdr-0.7.5/pdr.egg-info/PKG-INFO` & `pdr-1.0.0/pdr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 0.7.5
+Version: 1.0.0
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -24,14 +24,17 @@
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
 (under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](supported_datasets.md) 
 
 If the software fails while attempting to read from datasets that we have listed as supported, please submit an issue with a link to the file and information about the error (if applicable). There might also be datasets that work but are not listed. We would like to hear about those too. If a dataset is not yet supported that you would like us to consider prioritizing, [please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
 
+### Attribution
+If you use _pdr_ in your work, please cite us using our Zenodo DOI: [![DOI](https://zenodo.org/badge/266449940.svg)](https://zenodo.org/badge/latestdoi/266449940)
+
 ### Installation
 _pdr_ is now on `conda` and `pip`. We recommend (and only officially support) installation into a `conda` environment.
 You can do this like so: 
 
 ```
 conda create --name pdrenv
 conda activate pdrenv
@@ -52,15 +55,15 @@
   - `pillow`: adds support for TIFF files and browse image rendering
   - `matplotlib`: allows usage of `save_sparklines`, an experimental browse function
 
 ### Usage
 
 (You can check out our example Notebook on Binder for a 
 quick interactive demo of functionality: 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/master))
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/main))
 
 Just open and python shell and run `import pdr` and then `pdr.read(filename)`, 
 where _filename_ is the full path to a data file _or_ a metadata / label file 
 (extensions .LBL, .lbl, or .xml). `read()` will look for corresponding data 
 or metadata files in the same path, or read metadata directly from the data file 
 if it has an attached label.
```

### Comparing `pdr-0.7.5/pdr.egg-info/SOURCES.txt` & `pdr-1.0.0/pdr.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 LICENSE
 README.md
 setup.py
 pdr/__init__.py
+pdr/_scaling.py
 pdr/bit_handling.py
 pdr/browsify.py
 pdr/datatypes.py
+pdr/errors.py
+pdr/func.py
 pdr/np_utils.py
 pdr/pd_utils.py
 pdr/pdr.py
+pdr/pdrtypes.py
 pdr/pvl_utils.py
-pdr/rasterio_utils.py
 pdr/utils.py
 pdr.egg-info/PKG-INFO
 pdr.egg-info/SOURCES.txt
 pdr.egg-info/dependency_links.txt
 pdr.egg-info/requires.txt
 pdr.egg-info/top_level.txt
 pdr/formats/__init__.py
 pdr/formats/cassini.py
+pdr/formats/checkers.py
 pdr/formats/clementine.py
-pdr/formats/core.py
 pdr/formats/diviner.py
 pdr/formats/galileo.py
 pdr/formats/juno.py
+pdr/formats/lro.py
 pdr/formats/lroc.py
-pdr/formats/m3.py
-pdr/formats/messenger.py
 pdr/formats/mex_marsis.py
 pdr/formats/mgn.py
 pdr/formats/mgs.py
 pdr/formats/msl_apxs.py
 pdr/formats/msl_ccam.py
 pdr/formats/msl_cmn.py
+pdr/formats/pvo.py
 pdr/formats/rosetta.py
+pdr/formats/themis.py
+pdr/loaders/__init__.py
+pdr/loaders/_helpers.py
+pdr/loaders/datawrap.py
+pdr/loaders/dispatch.py
+pdr/loaders/handlers.py
+pdr/loaders/image.py
+pdr/loaders/queries.py
+pdr/loaders/table.py
+pdr/loaders/text.py
+pdr/loaders/utility.py
 pdr/parselabel/__init__.py
 pdr/parselabel/pds3.py
 pdr/parselabel/pds4.py
 pdr/parselabel/utils.py
```

### Comparing `pdr-0.7.5/setup.py` & `pdr-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdr",
-    version="0.7.5",
+    version="1.0.0",
     author="Chase Million",
     author_email="chase@millionconcepts.com",
     description="Planetary Data Reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MillionConcepts/pdr",
     packages=setuptools.find_packages(),
```

