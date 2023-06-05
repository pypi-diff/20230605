# Comparing `tmp/aisdc-1.0.4.tar.gz` & `tmp/aisdc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisdc-1.0.4.tar", last modified: Fri May  5 14:05:25 2023, max compression
+gzip compressed data, was "aisdc-1.0.5.tar", last modified: Mon Jun  5 20:43:21 2023, max compression
```

## Comparing `aisdc-1.0.4.tar` & `aisdc-1.0.5.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.4/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-05 14:05:25.694556 aisdc-1.0.4/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-02 15:24:23.000000 aisdc-1.0.4/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/attacks/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/attacks/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      395 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/attacks/attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/attacks/attribute_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2167 2023-05-02 10:18:16.000000 aisdc-1.0.4/aisdc/attacks/dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22027 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/attacks/likelihood_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12090 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/attacks/report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22656 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/attacks/worst_case_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10042 2023-05-02 15:24:23.000000 aisdc-1.0.4/aisdc/generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-02 15:32:15.000000 aisdc-1.0.4/aisdc/metrics.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/preprocessing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/preprocessing/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/preprocessing/loaders.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/safemodel/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc/safemodel/classifiers/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/dp_svc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7595 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/new_model_template.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7149 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safekeras.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6322 2023-05-05 14:05:12.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/classifiers/safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/reporting.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.4/aisdc/safemodel/rules.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    30719 2023-05-02 15:16:25.000000 aisdc-1.0.4/aisdc/safemodel/safemodel.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/aisdc.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1435 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      170 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-05-05 14:05:25.000000 aisdc-1.0.4/aisdc.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-05-05 14:05:25.694556 aisdc-1.0.4/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1857 2023-05-05 14:05:12.000000 aisdc-1.0.4/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-05 14:05:25.694556 aisdc-1.0.4/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-05-02 15:16:25.000000 aisdc-1.0.4/tests/test_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_attacks_dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_attacks_via_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_attribute_inference_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_data_interface.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6065 2023-05-02 15:24:23.000000 aisdc-1.0.4/tests/test_generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3661 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_lira_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_loaders.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.4/tests/test_metrics.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safekeras2.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15852 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11863 2023-05-05 14:05:12.000000 aisdc-1.0.4/tests/test_saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.4/tests/test_safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11146 2023-05-02 10:18:16.000000 aisdc-1.0.4/tests/test_worst_case_attack.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.089487 aisdc-1.0.5/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.5/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-06-05 20:43:21.089487 aisdc-1.0.5/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-17 12:52:16.000000 aisdc-1.0.5/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/attacks/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/attacks/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      977 2023-06-05 19:25:56.000000 aisdc-1.0.5/aisdc/attacks/attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/attacks/attribute_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2166 2023-05-17 12:52:16.000000 aisdc-1.0.5/aisdc/attacks/dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3616 2023-05-17 12:52:16.000000 aisdc-1.0.5/aisdc/attacks/failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    26233 2023-06-05 19:25:56.000000 aisdc-1.0.5/aisdc/attacks/likelihood_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12913 2023-05-19 21:41:45.000000 aisdc-1.0.5/aisdc/attacks/report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    30917 2023-06-05 19:25:56.000000 aisdc-1.0.5/aisdc/attacks/worst_case_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10176 2023-05-19 21:41:45.000000 aisdc-1.0.5/aisdc/generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-17 12:52:16.000000 aisdc-1.0.5/aisdc/metrics.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/preprocessing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/preprocessing/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/preprocessing/loaders.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/safemodel/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/safemodel/classifiers/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/dp_svc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7620 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/new_model_template.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7221 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-05-02 15:16:25.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safekeras.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6347 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-05-11 14:01:54.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/reporting.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/rules.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    30820 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/safemodel.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1484 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      181 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-06-05 20:43:21.089487 aisdc-1.0.5/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1879 2023-06-05 20:27:42.000000 aisdc-1.0.5/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.089487 aisdc-1.0.5/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-05-02 15:16:25.000000 aisdc-1.0.5/tests/test_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_attacks_dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_attacks_via_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_attribute_inference_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_data_interface.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5595 2023-05-17 12:52:16.000000 aisdc-1.0.5/tests/test_failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6782 2023-05-19 21:41:45.000000 aisdc-1.0.5/tests/test_generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8107 2023-06-05 19:25:56.000000 aisdc-1.0.5/tests/test_lira_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_loaders.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.5/tests/test_metrics.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safekeras2.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16955 2023-05-23 09:33:17.000000 aisdc-1.0.5/tests/test_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11863 2023-05-17 12:52:16.000000 aisdc-1.0.5/tests/test_saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13595 2023-05-25 09:59:37.000000 aisdc-1.0.5/tests/test_worst_case_attack.py
```

### Comparing `aisdc-1.0.4/LICENSE` & `aisdc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/PKG-INFO` & `aisdc-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.4/README.md` & `aisdc-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/attacks/attribute_attack.py` & `aisdc-1.0.5/aisdc/attacks/attribute_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/attacks/dataset.py` & `aisdc-1.0.5/aisdc/attacks/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         y_test: np.ndarray,
     ) -> None:
         """Add a processed and split dataset"""
         self.x_train = x_train
         self.y_train = np.array(y_train, int)
         self.x_test = x_test
         self.y_test = np.array(y_test, int)
-        self.n_samples = len(x_train) + len(y_train)
+        self.n_samples = len(x_train) + len(x_test)
 
     def add_feature(self, name: str, indices: list[int], encoding: str) -> None:
         """Add a feature description to the data dictionary."""
         index: int = len(self.features)
         self.features[index] = {
             "name": name,
             "indices": indices,
```

### Comparing `aisdc-1.0.4/aisdc/attacks/likelihood_attack.py` & `aisdc-1.0.5/aisdc/attacks/likelihood_attack.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 
 from __future__ import annotations
 
 import argparse
 import importlib
 import json
 import logging
+import uuid
 from collections.abc import Hashable, Iterable
+from datetime import datetime
 from typing import Any
 
 import numpy as np
 import sklearn
 from scipy.stats import norm
 from sklearn.datasets import load_breast_cancer
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 
 from aisdc import metrics
 from aisdc.attacks import report
-from aisdc.attacks.attack import Attack
+from aisdc.attacks.attack import Attack, ConfigFile
 from aisdc.attacks.dataset import Data
 
 logging.basicConfig(level=logging.INFO)
 
 N_SHADOW_MODELS = 100  # Number of shadow models that should be trained
 EPS = 1e-16  # Used to avoid numerical issues in logit function
 P_THRESH = 0.05  # default significance threshold
@@ -70,18 +72,31 @@
 
 
 class LIRAAttackArgs:
     """LIRA Attack arguments"""
 
     def __init__(self, **kwargs):
         self.__dict__["n_shadow_models"] = N_SHADOW_MODELS
+        self.__dict__["n_shadow_rows_confidences_min"] = 10
         self.__dict__["p_thresh"] = 0.05
         self.__dict__["report_name"] = None
-        self.__dict__["json_file"] = "config.json"
+        self.__dict__["training_data_filename"] = None
+        self.__dict__["test_data_filename"] = None
+        self.__dict__["training_preds_filename"] = None
+        self.__dict__["test_preds_filename"] = None
+        self.__dict__["target_model"] = None
+        self.__dict__["target_model_hyp"] = None
+        self.__dict__["attack_config_json_file_name"] = None
+        self.__dict__["shadow_models_fail_fast"] = False
         self.__dict__.update(kwargs)
+        if self.__dict__["attack_config_json_file_name"] is not None:
+            configfile_obj = ConfigFile(self.__dict__["attack_config_json_file_name"])
+            configfile_obj.load_config_file_into_dict(self.__dict__)
+        # deleted for not enabling to appear in the output file
+        del self.__dict__["attack_config_json_file_name"]
 
     def __str__(self):
         return ",".join(
             [f"{str(key)}: {str(value)}" for key, value in self.__dict__.items()]
         )
 
     def set_param(self, key: Hashable, value: Any) -> None:
@@ -94,14 +109,15 @@
 
 
 class LIRAAttack(Attack):
     """The main LIRA Attack class"""
 
     def __init__(self, args: LIRAAttackArgs = LIRAAttackArgs()) -> None:
         self.attack_metrics = None
+        self.attack_failfast_shadow_models_trained = None
         self.dummy_attack_metrics = None
         self.metadata = None
         self.args = args
 
     def __str__(self):
         return "LIRA Attack"
 
@@ -110,15 +126,15 @@
         Runs a LIRA attack from a dataset object and a target model
 
         Parameters
         ----------
         dataset: attacks.dataset.Data
             Dataset as an instance of the Data class. Needs to have x_train, x_test, y_train
             and y_test set.
-        target_mode: sklearn.base.BaseEstimator
+        target_model: sklearn.base.BaseEstimator
             Trained target model. Any class that implements the sklearn.base.BaseEstimator
             interface (i.e. has fit, predict and predict_proba methods)
         """
 
         shadow_clf = sklearn.base.clone(target_model)
 
         dataset = self._check_and_update_dataset(dataset, target_model)
@@ -131,44 +147,47 @@
             dataset.x_test,
             dataset.y_test,
             target_model.predict_proba(dataset.x_test),
         )
 
     def _check_and_update_dataset(
         self, dataset: Data, target_model: sklearn.base.BaseEstimator
-    ) -> tuple[np.ndarray, np.ndarray]:
+    ) -> Data:
         """Makes sure that it is ok to use the class variables to index the prediction
         arrays. This has two steps:
         1. Replacing the values in y_train with their position in target_model.classes (will
            normally result in no change)
         2. Removing from the test set any rows corresponding to classes that are not in the
            training set.
         """
-
+        logger = logging.getLogger("_check_and_update_dataset")
         y_train_new = []
         classes = list(target_model.classes_)  # pylint: disable = protected-access
         for y in dataset.y_train:
             y_train_new.append(classes.index(y))
 
         dataset.y_train = np.array(y_train_new, int)
-        print(
-            f"new ytrain has values and counts: {np.unique(dataset.y_train,return_counts=True)}"
+
+        logger.info(
+            "new ytrain has values and counts: %s",
+            f"{np.unique(dataset.y_train,return_counts=True)}",
         )
         ok_pos = []
         y_test_new = []
         for i, y in enumerate(dataset.y_test):
             if y in classes:
                 ok_pos.append(i)
                 y_test_new.append(classes.index(y))
 
         if len(y_test_new) != len(dataset.x_test):
             dataset.x_test = dataset.x_test[ok_pos, :]
         dataset.y_test = np.array(y_test_new, int)
-        print(
-            f"new ytest has values and counts: {np.unique(dataset.y_test,return_counts=True)}"
+        logger.info(
+            "new ytest has values and counts: %s",
+            f"{np.unique(dataset.y_test,return_counts=True)}",
         )
 
         return dataset
 
     def run_scenario_from_preds(  # pylint: disable = too-many-statements, too-many-arguments, too-many-locals
         self,
         shadow_clf: sklearn.base.BaseEstimator,
@@ -292,14 +311,31 @@
                         shadow_row_to_confidence[i].append(
                             _logit(shadow_confidences[i, cl_pos])
                         )
                     else:  # pragma: no cover
                         # catch-all
                         shadow_row_to_confidence[i].append(_logit(0))
 
+            # Compute number of confidences for each row
+            lengths_shadow_row_to_confidence = {
+                key: len(value) for key, value in shadow_row_to_confidence.items()
+            }
+            n_shadow_confidences = self.args.n_shadow_rows_confidences_min
+            # Stop training of shadow models when shadow_model_fail_fast is True
+            # and a minimum number of confidences specified by parameter
+            # (n_shadow_rows_confidences_min) are computed for each row
+            if (
+                not any(
+                    value < n_shadow_confidences
+                    for value in lengths_shadow_row_to_confidence.values()
+                )
+                and self.args.shadow_models_fail_fast
+            ):
+                break
+        self.attack_failfast_shadow_models_trained = model_idx + 1
         # Do the test described in the paper in each case
         mia_scores = []
         mia_labels = []
         logger.info("Computing scores for train rows")
         for i in range(n_train_rows):
             true_score = _logit(target_train_preds[i, y_target_train[i]])
             null_scores = np.array(train_row_to_confidence[i])
@@ -379,15 +415,15 @@
         )
         self.metadata["global_metrics"]["AUC_sig"] = (
             f"Significant at p={self.args.p_thresh}"
             if auc_p <= self.args.p_thresh
             else f"Not significant at p={self.args.p_thresh}"
         )
         self.metadata["global_metrics"][
-            "AUC NULL 3sd range"
+            "null_auc_3sd_range"
         ] = f"{0.5 - 3 * auc_std} -> {0.5 + 3 * auc_std}"
 
         self.metadata["attack"] = str(self)
 
     def make_report(self) -> dict:
         """Create the report
 
@@ -397,30 +433,47 @@
         Returns
         -------
 
         output: Dict
             Dictionary containing all attack output
         """
         logger = logging.getLogger("reporting")
-        output = {}
         logger.info("Starting report, report_name = %s", self.args.report_name)
-        output["attack_metrics"] = self.attack_metrics
+        output = {}
+        output["log_id"] = str(uuid.uuid4())
+        output["log_time"] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
         self._construct_metadata()
         output["metadata"] = self.metadata
+        output["attack_experiment_logger"] = self._get_attack_metrics_instances()
+
         if self.args.report_name is not None:
             json_report = report.create_json_report(output)
             with open(f"{self.args.report_name}.json", "w", encoding="utf-8") as f:
                 f.write(json_report)
             logger.info("Wrote report to %s", f"{self.args.report_name}.json")
 
-            pdf = report.create_lr_report(output)
-            pdf.output(f"{self.args.report_name}.pdf", "F")
+            pdf_report = report.create_lr_report(output)
+            pdf_report.output(f"{self.args.report_name}.pdf", "F")
             logger.info("Wrote pdf report to %s", f"{self.args.report_name}.pdf")
         return output
 
+    def _get_attack_metrics_instances(self) -> dict:
+        """Constructs the metadata object, after attacks"""
+        attack_metrics_experiment = {}
+        attack_metrics_instances = {}
+
+        for rep, _ in enumerate(self.attack_metrics):
+            self.attack_metrics[rep][
+                "n_shadow_models_trained"
+            ] = self.attack_failfast_shadow_models_trained
+            attack_metrics_instances["instance_" + str(rep)] = self.attack_metrics[rep]
+
+        attack_metrics_experiment["attack_instance_logger"] = attack_metrics_instances
+        return attack_metrics_experiment
+
     def setup_example_data(self) -> None:
         """Method to create example data and save (including config). Intended to allow users
         to see how they would need to setup their own data.
 
         Generates train and test data .csv files, train and test predictions .csv files and
         a config.json file that can be used to run the attack from the command line.
         """
@@ -438,56 +491,56 @@
 
         train_preds = rf.predict_proba(train_X)
         test_preds = rf.predict_proba(test_X)
         np.savetxt("train_preds.csv", train_preds, delimiter=",")
         np.savetxt("test_preds.csv", test_preds, delimiter=",")
 
         config = {
-            "training_data_file": "train_data.csv",
-            "testing_data_file": "test_data.csv",
-            "training_preds_file": "train_preds.csv",
-            "testing_preds_file": "test_preds.csv",
+            "training_data_filename": "train_data.csv",
+            "test_data_filename": "test_data.csv",
+            "training_preds_filename": "train_preds.csv",
+            "test_preds_filename": "test_preds.csv",
             "target_model": ["sklearn.ensemble", "RandomForestClassifier"],
-            "target_hyppars": {"min_samples_split": 2, "min_samples_leaf": 1},
+            "target_model_hyp": {"min_samples_split": 2, "min_samples_leaf": 1},
         }
 
         with open("config.json", "w", encoding="utf-8") as f:
             f.write(json.dumps(config))
 
     def attack_from_config(self) -> None:  # pylint: disable = too-many-locals
         """Runs an attack based on the args parsed from the command line"""
         logger = logging.getLogger("run-attack")
-        logger.info("Reading config from %s", self.args.json_file)
-        with open(self.args.json_file, encoding="utf-8") as f:
-            config = json.loads(f.read())
-
-        logger.info("Loading training data csv from %s", config["training_data_file"])
-        training_data = np.loadtxt(config["training_data_file"], delimiter=",")
+        logger.info(
+            "Loading training data csv from %s", self.args.training_data_filename
+        )
+        training_data = np.loadtxt(self.args.training_data_filename, delimiter=",")
         train_X = training_data[:, :-1]
         train_y = training_data[:, -1].flatten().astype(int)
         logger.info("Loaded %d rows", len(train_X))
 
-        logger.info("Loading test data csv from %s", config["testing_data_file"])
-        test_data = np.loadtxt(config["testing_data_file"], delimiter=",")
+        logger.info("Loading test data csv from %s", self.args.test_data_filename)
+        test_data = np.loadtxt(self.args.test_data_filename, delimiter=",")
         test_X = test_data[:, :-1]
         test_y = test_data[:, -1].flatten().astype(int)
         logger.info("Loaded %d rows", len(test_X))
 
-        logger.info("Loading train predictions form %s", config["training_preds_file"])
-        train_preds = np.loadtxt(config["training_preds_file"], delimiter=",")
+        logger.info(
+            "Loading train predictions form %s", self.args.training_preds_filename
+        )
+        train_preds = np.loadtxt(self.args.training_preds_filename, delimiter=",")
         assert len(train_preds) == len(train_X)
 
-        logger.info("Loading test predictions form %s", config["testing_preds_file"])
-        test_preds = np.loadtxt(config["testing_preds_file"], delimiter=",")
+        logger.info("Loading test predictions form %s", self.args.test_preds_filename)
+        test_preds = np.loadtxt(self.args.test_preds_filename, delimiter=",")
         assert len(test_preds) == len(test_X)
 
-        clf_module_name, clf_class_name = config["target_model"]
+        clf_module_name, clf_class_name = self.args.target_model
         module = importlib.import_module(clf_module_name)
         clf_class = getattr(module, clf_class_name)
-        clf_params = config["target_hyppars"]
+        clf_params = self.args.target_model_hyp
         clf = clf_class(**clf_params)
         logger.info("Created model: %s", str(clf))
         self.run_scenario_from_preds(
             clf, train_X, train_y, train_preds, test_X, test_y, test_preds
         )
         logger.info("Computing metrics")
 
@@ -512,27 +565,51 @@
     """Run a command line attack based on saved files described in .json file"""
     lira_args = LIRAAttackArgs(**args.__dict__)
     attack_obj = LIRAAttack(lira_args)
     attack_obj.attack_from_config()
     attack_obj.make_report()
 
 
+def _run_attack_from_configfile(args):
+    """Run a command line attack based on saved files described in .json file"""
+    lira_args = LIRAAttackArgs(
+        attack_config_json_file_name=str(args.attack_config_json_file_name),
+    )
+    attack_obj = LIRAAttack(lira_args)
+    attack_obj.attack_from_config()
+    attack_obj.make_report()
+
+
 def main():
     """Main method to parse args and invoke relevant code"""
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument(
         "-s",
         "--n-shadow-models",
         type=int,
         required=False,
         default=N_SHADOW_MODELS,
         action="store",
         dest="n_shadow_models",
         help=("The number of shadow models to train (default = %(default)d)"),
     )
+
+    parser.add_argument(
+        "--n-shadow-rows-confidences-min",
+        type=int,
+        action="store",
+        dest="n_shadow_rows_confidences_min",
+        default=10,
+        required=False,
+        help=(
+            """Number of confidences against rows in shadow data from the shadow models
+            and works when --shadow-models-fail-fast = True. Default = %(default)d"""
+        ),
+    )
+
     parser.add_argument(
         "--report-name",
         type=str,
         action="store",
         dest="report_name",
         required=False,
         default="lr_report",
@@ -544,32 +621,61 @@
         type=float,
         action="store",
         dest="p_thresh",
         required=False,
         default=P_THRESH,
         help=("Significance threshold for p-value comparisons. Default = %(default)f"),
     )
+
+    parser.add_argument(
+        "--shadow-models-fail-fast",
+        action="store_true",
+        required=False,
+        dest="shadow_models_fail_fast",
+        help=(
+            """To stop training shadow models early based on minimum number of
+            confidences across all rows (--n-shadow-rows-confidences-min)
+            in the shadow data. Default = %(default)s"""
+        ),
+    )
+
     subparsers = parser.add_subparsers()
     example_parser = subparsers.add_parser("run-example", parents=[parser])
     example_parser.set_defaults(func=_example)
 
     attack_parser = subparsers.add_parser("run-attack", parents=[parser])
     attack_parser.add_argument(
         "-j",
-        "--json-file",
+        "--attack-config-json-file-name",
         action="store",
         required=True,
-        dest="json_file",
+        dest="attack_config_json_file_name",
         type=str,
         help=(
             "Name of the .json file containing details for the run. Default = %(default)s"
         ),
     )
     attack_parser.set_defaults(func=_run_attack)
 
+    attack_parser_config = subparsers.add_parser("run-attack-from-configfile")
+    attack_parser_config.add_argument(
+        "-j",
+        "--attack-config-json-file-name",
+        action="store",
+        required=True,
+        dest="attack_config_json_file_name",
+        type=str,
+        default="config_lira_cmd.json",
+        help=(
+            "Name of the .json file containing details for the run. Default = %(default)s"
+        ),
+    )
+
+    attack_parser_config.set_defaults(func=_run_attack_from_configfile)
+
     example_data_parser = subparsers.add_parser("setup-example-data")
     example_data_parser.set_defaults(func=_setup_example_data)
 
     args = parser.parse_args()
     try:
         args.func(args)
     except AttributeError as e:  # pragma:no cover
```

### Comparing `aisdc-1.0.4/aisdc/attacks/report.py` & `aisdc-1.0.5/aisdc/attacks/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,25 +196,25 @@
 
 def create_mia_report(attack_output: dict) -> FPDF:
     """make a worst case membership inference report
 
     Parameters
     ----------
 
-    metadata: dict
-        dictionary of metadata
+    attack_output: dict
+        dictionary with following items
 
-    mia_metrics: list
-        list of metrics dictionaries
+            metadata: dict
+                dictionary of metadata
 
-    dummy_metrics: list
-        list of metrics dictionaries
+            attack_experiment_logger: dict
+                list of metrics as dictionary items for an experiment
 
-    dummy_metadata: dict
-        metadata for dummy experiments
+            dummy_attack_experiment_logger: dict
+                list of metrics as dictionary items across dummy experiments
 
     Returns
     -------
 
     pdf: fpdf.FPDF
         fpdf document object
 
@@ -306,17 +306,44 @@
 
 def create_json_report(output):
     """Create a report in json format for injestion by other tools"""
     # Initial work, just dump mia_metrics and dummy_metrics into a json structure
     return json.dumps(output, cls=NumpyArrayEncoder)
 
 
-def create_lr_report(output):
-    """TODO"""
-    mia_metrics = output["attack_metrics"][0]
+def create_lr_report(output: dict) -> FPDF:
+    """make a lira membership inference report
+
+    Parameters
+    ----------
+
+    output: dict
+        dictionary with following items
+
+        metadata: dict
+                dictionary of metadata
+
+        attack_experiment_logger: dict
+            list of metrics as dictionary items for an experiments
+            In case of LIRA attack scenario, this will have dictionary
+            items of attack_instance_logger that
+            will have a single metrics dictionary
+
+    Returns
+    -------
+
+    pdf: fpdf.FPDF
+        fpdf document object
+
+    """
+    mia_metrics = [
+        v
+        for _, v in output["attack_experiment_logger"]["attack_instance_logger"].items()
+    ][0]
+    # mia_metrics = output["attack_metrics"][0]
     metadata = output["metadata"]
     _roc_plot_single(mia_metrics, "log_roc.png")
     pdf = FPDF()
     pdf.add_page()
     pdf.set_xy(0, 0)
     title(pdf, "Likelihood Ratio Attack Report")
     subtitle(pdf, "Introduction")
```

### Comparing `aisdc-1.0.4/aisdc/attacks/worst_case_attack.py` & `aisdc-1.0.5/aisdc/attacks/worst_case_attack.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 import sklearn
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import train_test_split
 
 from aisdc import metrics
 from aisdc.attacks import report
-from aisdc.attacks.attack import Attack
+from aisdc.attacks.attack import Attack, ConfigFile
 from aisdc.attacks.dataset import Data
+from aisdc.attacks.failfast import FailFast
 
 logging.basicConfig(level=logging.INFO)
 
 P_THRESH = 0.05
 
 
 class WorstCaseAttackArgs:
@@ -37,26 +38,38 @@
         self.__dict__["p_thresh"] = 0.05
         self.__dict__["n_dummy_reps"] = 1
         self.__dict__["train_beta"] = 2
         self.__dict__["test_beta"] = 2
         self.__dict__["test_prop"] = 0.3
         self.__dict__["n_rows_in"] = 1000
         self.__dict__["n_rows_out"] = 1000
-        self.__dict__["in_sample_filename"] = None
-        self.__dict__["out_sample_filename"] = None
+        self.__dict__["training_preds_filename"] = None
+        self.__dict__["test_preds_filename"] = None
         self.__dict__["report_name"] = None
         self.__dict__["include_model_correct_feature"] = False
         self.__dict__["sort_probs"] = True
         self.__dict__["mia_attack_model"] = RandomForestClassifier
         self.__dict__["mia_attack_model_hyp"] = {
             "min_samples_split": 20,
             "min_samples_leaf": 10,
             "max_depth": 5,
         }
+        self.__dict__["attack_metric_success_name"] = "P_HIGHER_AUC"
+        self.__dict__["attack_metric_success_thresh"] = 0.05
+        self.__dict__["attack_metric_success_comp_type"] = "lte"
+        self.__dict__["attack_metric_success_count_thresh"] = 5
+        self.__dict__["attack_fail_fast"] = False
+        self.__dict__["attack_config_json_file_name"] = None
         self.__dict__.update(kwargs)
+        # Reading parameters from a json file
+        if self.__dict__["attack_config_json_file_name"] is not None:
+            configfile_obj = ConfigFile(self.__dict__["attack_config_json_file_name"])
+            configfile_obj.load_config_file_into_dict(self.__dict__)
+        # deleted for not enabling to appear in the output file
+        del self.__dict__["attack_config_json_file_name"]
 
     def __str__(self):
         return ",".join(
             [f"{str(key)}: {str(value)}" for key, value in self.__dict__.items()]
         )
 
     def set_param(self, key: Hashable, value: Any) -> None:
@@ -69,15 +82,17 @@
 
 
 class WorstCaseAttack(Attack):
     """Class to wrap the worst case attack code"""
 
     def __init__(self, args: WorstCaseAttackArgs = WorstCaseAttackArgs()):
         self.attack_metrics = None
+        self.attack_metric_failfast_summary = None
         self.dummy_attack_metrics = None
+        self.dummy_attack_metric_failfast_summary = None
         self.metadata = None
         self.args = args
 
     def __str__(self):
         return "WorstCase attack"
 
     def attack(self, dataset: Data, target_model: sklearn.base.BaseEstimator) -> None:
@@ -113,16 +128,16 @@
         """Start an attack from saved prediction files
 
         To be used when only saved predictions are available.
 
         Filenames for the saved prediction files to be specified in the arguments provided
         in the constructor
         """
-        train_preds = np.loadtxt(self.args.in_sample_filename, delimiter=",")
-        test_preds = np.loadtxt(self.args.out_sample_filename, delimiter=",")
+        train_preds = np.loadtxt(self.args.training_preds_filename, delimiter=",")
+        test_preds = np.loadtxt(self.args.test_preds_filename, delimiter=",")
         self.attack_from_preds(train_preds, test_preds)
 
     def attack_from_preds(  # pylint: disable=too-many-locals
         self,
         train_preds: np.ndarray,
         test_preds: np.ndarray,
         train_correct: np.ndarray = None,
@@ -139,32 +154,48 @@
             Array of train predictions. One row per example, one column per class (i.e. 2)
         test_preds:  np.ndarray
             Array of test predictions. One row per example, one column per class (i.e. 2)
 
         """
         logger = logging.getLogger("attack-from-preds")
         logger.info("Running main attack repetitions")
-        self.attack_metrics = self.run_attack_reps(
+        attack_metric_dict = self.run_attack_reps(
             train_preds,
             test_preds,
             train_correct=train_correct,
             test_correct=test_correct,
         )
+        self.attack_metrics = attack_metric_dict["mia_metrics"]
+        self.attack_metric_failfast_summary = attack_metric_dict[
+            "failfast_metric_summary"
+        ]
 
         self.dummy_attack_metrics = []
+        self.dummy_attack_metric_failfast_summary = []
         if self.args.n_dummy_reps > 0:
             logger.info("Running dummy attack reps")
             n_train_rows = len(train_preds)
             n_test_rows = len(test_preds)
             for _ in range(self.args.n_dummy_reps):
                 d_train_preds, d_test_preds = self.generate_arrays(
                     n_train_rows, n_test_rows, self.args.train_beta, self.args.test_beta
                 )
-                temp_metrics = self.run_attack_reps(d_train_preds, d_test_preds)
-                self.dummy_attack_metrics += temp_metrics
+                temp_attack_metric_dict = self.run_attack_reps(
+                    d_train_preds, d_test_preds
+                )
+                temp_metrics = temp_attack_metric_dict["mia_metrics"]
+                temp_metric_failfast_summary = temp_attack_metric_dict[
+                    "failfast_metric_summary"
+                ]
+
+                self.dummy_attack_metrics.append(temp_metrics)
+                self.dummy_attack_metric_failfast_summary.append(
+                    temp_metric_failfast_summary
+                )
+
         logger.info("Finished running attacks")
 
     def _prepare_attack_data(
         self,
         train_preds: np.ndarray,
         test_preds: np.ndarray,
         train_correct: np.ndarray = None,
@@ -193,40 +224,46 @@
 
     def run_attack_reps(  # pylint: disable = too-many-locals
         self,
         train_preds: np.ndarray,
         test_preds: np.ndarray,
         train_correct: np.ndarray = None,
         test_correct: np.ndarray = None,
-    ) -> list:
+    ) -> dict:
         """
         Run actual attack reps from train and test predictions
 
         Parameters
         ----------
         train_preds: np.ndarray
             predictions from the model on training (in-sample) data
         test_preds: np.ndarray
             predictions from the model on testing (out-of-sample) data
 
         Returns
         -------
-        mia_metrics: List
-            List of attack metrics dictionaries, one for each repetition
+        mia_metrics_dict: dict
+            a dictionary with two items including mia_metrics
+            (a list of metric across repetitions) and failfast_metric_summary object
+            (an object of FailFast class) to maintain summary of
+            fail/success of attacks for a given metric of failfast option
         """
         self.args.set_param("n_rows_in", len(train_preds))
         self.args.set_param("n_rows_out", len(test_preds))
         logger = logging.getLogger("attack-reps")
         mi_x, mi_y = self._prepare_attack_data(
             train_preds, test_preds, train_correct, test_correct
         )
 
         mia_metrics = []
+
+        failfast_metric_summary = FailFast(self.args)
+
         for rep in range(self.args.n_reps):
-            logger.info("Rep %d of %d", rep, self.args.n_reps)
+            logger.info("Rep %d of %d", rep + 1, self.args.n_reps)
             mi_train_x, mi_test_x, mi_train_y, mi_test_y = train_test_split(
                 mi_x, mi_y, test_size=self.args.test_prop, stratify=mi_y
             )
             attack_classifier = self.args.mia_attack_model(
                 **self.args.mia_attack_model_hyp
             )
             attack_classifier.fit(mi_train_x, mi_train_y)
@@ -242,17 +279,29 @@
                 tn, fp, fn, tp = confusion_matrix(mi_test_y, yeom_preds).ravel()
                 mia_metrics[-1]["yeom_tpr"] = tp / (tp + fn)
                 mia_metrics[-1]["yeom_fpr"] = fp / (fp + tn)
                 mia_metrics[-1]["yeom_advantage"] = (
                     mia_metrics[-1]["yeom_tpr"] - mia_metrics[-1]["yeom_fpr"]
                 )
 
+            failfast_metric_summary.check_attack_success(mia_metrics[rep])
+
+            if (
+                failfast_metric_summary.check_overall_attack_success(self.args)
+                and self.args.attack_fail_fast
+            ):
+                break
+
         logger.info("Finished simulating attacks")
 
-        return mia_metrics
+        mia_metrics_dict = {}
+        mia_metrics_dict["mia_metrics"] = mia_metrics
+        mia_metrics_dict["failfast_metric_summary"] = failfast_metric_summary
+
+        return mia_metrics_dict
 
     def _get_global_metrics(self, attack_metrics: list) -> dict:
         """Summarise metrics from a metric list
 
         Arguments
         ---------
         attack_metrics: List
@@ -407,16 +456,16 @@
         train_preds, test_preds = self.generate_arrays(
             self.args.n_rows_in,
             self.args.n_rows_out,
             train_beta=self.args.train_beta,
             test_beta=self.args.test_beta,
         )
         logger.info("Saving files")
-        np.savetxt(self.args.in_sample_filename, train_preds, delimiter=",")
-        np.savetxt(self.args.out_sample_filename, test_preds, delimiter=",")
+        np.savetxt(self.args.training_preds_filename, train_preds, delimiter=",")
+        np.savetxt(self.args.test_preds_filename, test_preds, delimiter=",")
 
     def _construct_metadata(self):
         """Constructs the metadata object, after attacks"""
         self.metadata = {}
         # Store all args
         self.metadata["experiment_details"] = {}
         self.metadata["experiment_details"].update(self.args.__dict__)
@@ -424,67 +473,125 @@
             del self.metadata["experiment_details"]["func"]
 
         self.metadata["attack"] = str(self)
 
         # Global metrics
         self.metadata["global_metrics"] = self._get_global_metrics(self.attack_metrics)
         self.metadata["baseline_global_metrics"] = self._get_global_metrics(
-            self.dummy_attack_metrics
+            self._unpack_dummy_attack_metrics_experiments_instances()
         )
 
+    def _unpack_dummy_attack_metrics_experiments_instances(self) -> list:
+        """Constructs the metadata object, after attacks"""
+        dummy_attack_metrics_instances = []
+
+        for exp_rep, _ in enumerate(self.dummy_attack_metrics):
+            temp_dummy_attack_metrics = self.dummy_attack_metrics[exp_rep]
+            dummy_attack_metrics_instances += temp_dummy_attack_metrics
+
+        return dummy_attack_metrics_instances
+
     def _get_attack_metrics_instances(self) -> dict:
         """Constructs the metadata object, after attacks"""
         attack_metrics_experiment = {}
         attack_metrics_instances = {}
 
         for rep, _ in enumerate(self.attack_metrics):
-            attack_metrics_instances["instance_" + str(rep + 1)] = self.attack_metrics[
-                rep
-            ]
+            attack_metrics_instances["instance_" + str(rep)] = self.attack_metrics[rep]
 
         attack_metrics_experiment["attack_instance_logger"] = attack_metrics_instances
+        attack_metrics_experiment[
+            "attack_metric_failfast_summary"
+        ] = self.attack_metric_failfast_summary.get_attack_summary()
+
         return attack_metrics_experiment
 
+    def _get_dummy_attack_metrics_experiments_instances(self) -> dict:
+        """Constructs the metadata object, after attacks"""
+        dummy_attack_metrics_experiments = {}
+
+        for exp_rep, _ in enumerate(self.dummy_attack_metrics):
+            temp_dummy_attack_metrics = self.dummy_attack_metrics[exp_rep]
+            dummy_attack_metric_instances = {}
+            for rep, _ in enumerate(temp_dummy_attack_metrics):
+                dummy_attack_metric_instances[
+                    "instance_" + str(rep)
+                ] = temp_dummy_attack_metrics[rep]
+            temp = {}
+            temp["attack_instance_logger"] = dummy_attack_metric_instances
+            temp[
+                "attack_metric_failfast_summary"
+            ] = self.dummy_attack_metric_failfast_summary[exp_rep].get_attack_summary()
+            dummy_attack_metrics_experiments[
+                "dummy_attack_metrics_experiment_" + str(exp_rep)
+            ] = temp
+
+        return dummy_attack_metrics_experiments
+
     def make_report(self) -> dict:
         """Creates output dictionary structure"""
         output = {}
         output["log_id"] = str(uuid.uuid4())
         output["log_time"] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
 
         self._construct_metadata()
         output["metadata"] = self.metadata
 
         output["attack_experiment_logger"] = self._get_attack_metrics_instances()
+        output[
+            "dummy_attack_experiments_logger"
+        ] = self._get_dummy_attack_metrics_experiments_instances()
+
+        # output_for_pdf = {}
+        # output_for_pdf["attack_metrics"] = self.attack_metrics
+        # output_for_pdf[
+        #     "dummy_attack_metrics"
+        # ] = self._unpack_dummy_attack_metrics_experiments_instances()
+        # output_for_pdf["metadata"] = self.metadata
 
         if self.args.report_name is not None:
             json_report = report.create_json_report(output)
             with open(f"{self.args.report_name}.json", "w", encoding="utf-8") as f:
                 f.write(json_report)
+
+            # pdf_report = report.create_mia_report(output_for_pdf)
             pdf_report = report.create_mia_report(output)
             pdf_report.output(f"{self.args.report_name}.pdf", "F")
+
         return output
 
 
 def _make_dummy_data(args):
     """Initialise class and run dummy data creation"""
     wc_args = WorstCaseAttackArgs(**args.__dict__)
-    wc_args.set_param("in_sample_filename", "train_preds.csv")
-    wc_args.set_param("out_sample_filename", "test_preds.csv")
+    wc_args.set_param("training_preds_filename", "train_preds.csv")
+    wc_args.set_param("test_preds_filename", "test_preds.csv")
     attack_obj = WorstCaseAttack(wc_args)
     attack_obj.make_dummy_data()
 
 
 def _run_attack(args):
     """Initialise class and run attack from prediction files"""
     wc_args = WorstCaseAttackArgs(**args.__dict__)
     attack_obj = WorstCaseAttack(wc_args)
     attack_obj.attack_from_prediction_files()
     _ = attack_obj.make_report()
 
 
+def _run_attack_from_configfile(args):
+    """Initialise class and run attack from prediction files
+    using config file"""
+    wc_args = WorstCaseAttackArgs(
+        attack_config_json_file_name=str(args.attack_config_json_file_name),
+    )
+    attack_obj = WorstCaseAttack(wc_args)
+    attack_obj.attack_from_prediction_files()
+    _ = attack_obj.make_report()
+
+
 def main():
     """main method to parse arguments and invoke relevant method"""
     logger = logging.getLogger("main")
     parser = argparse.ArgumentParser(
         description=("Perform a worst case attack from saved model predictions")
     )
 
@@ -542,31 +649,31 @@
     )
 
     dummy_parser.set_defaults(func=_make_dummy_data)
 
     attack_parser = subparsers.add_parser("run-attack")
     attack_parser.add_argument(
         "-i",
-        "--in-sample-preds",
+        "--training-preds-filename",
         action="store",
-        dest="in_sample_filename",
+        dest="training_preds_filename",
         required=False,
         type=str,
         default="train_preds.csv",
         help=(
             "csv file containing the predictive probabilities (one column per class) for the "
             "training data (one row per training example). Default = %(default)s"
         ),
     )
 
     attack_parser.add_argument(
         "-o",
-        "--out-of-sample-preds",
+        "--test-preds-filename",
         action="store",
-        dest="out_sample_filename",
+        dest="test_preds_filename",
         required=False,
         type=str,
         default="test_preds.csv",
         help=(
             "csv file containing the predictive probabilities (one column per class) for the "
             "non-training data (one row per training example). Default = %(default)s"
         ),
@@ -631,14 +738,43 @@
         type=float,
         default=P_THRESH,
         required=False,
         dest="p_thresh",
         help=("P-value threshold for significance testing. Default = %(default)f"),
     )
 
+    attack_parser.add_argument(
+        "--train-beta",
+        action="store",
+        type=float,
+        required=False,
+        default=5,
+        dest="train_beta",
+        help=(
+            "Value of b parameter for beta distribution used to sample the in-sample "
+            "probabilities. "
+            "High values will give more extreme probabilities. Set this value higher than "
+            "--test-beta to see successful attacks. Default = %(default)f"
+        ),
+    )
+
+    attack_parser.add_argument(
+        "--test-beta",
+        action="store",
+        type=float,
+        required=False,
+        default=2,
+        dest="test_beta",
+        help=(
+            "Value of b parameter for beta distribution used to sample the out-of-sample "
+            "probabilities. High values will give more extreme probabilities. Set this value "
+            "lower than --train-beta to see successful attacks. Default = %(default)f"
+        ),
+    )
+
     # Not currently possible from the command line as we cannot compute the correctness
     # of predictions. Possibly to be added in the future
     # attack_parser.add_argument(
     #     "--include-correct",
     #     action="store",
     #     type=bool,
     #     required=False,
@@ -659,16 +795,98 @@
         dest="sort_probs",
         help=(
             "Whether or not to sort the output probabilities (per row) before "
             "using them to train the attack model. Default = %(default)f"
         ),
     )
 
+    attack_parser.add_argument(
+        "--attack-metric-success-name",
+        action="store",
+        type=str,
+        default="P_HIGHER_AUC",
+        required=False,
+        dest="attack_metric_success_name",
+        help=(
+            """for computing attack success/failure based on
+            --attack-metric-success-thresh option. Default = %(default)s"""
+        ),
+    )
+
+    attack_parser.add_argument(
+        "--attack-metric-success-thresh",
+        action="store",
+        type=float,
+        default=0.05,
+        required=False,
+        dest="attack_metric_success_thresh",
+        help=(
+            """for defining threshold value to measure attack success
+            for the metric defined by argument --fail-metric-name option. Default = %(default)f"""
+        ),
+    )
+
+    attack_parser.add_argument(
+        "--attack-metric-success-comp-type",
+        action="store",
+        type=str,
+        default="lte",
+        required=False,
+        dest="attack_metric_success_comp_type",
+        help=(
+            """for computing attack success/failure based on
+            --attack-metric-success-thresh option. Default = %(default)s"""
+        ),
+    )
+
+    attack_parser.add_argument(
+        "--attack-metric-success-count-thresh",
+        action="store",
+        type=int,
+        default=2,
+        required=False,
+        dest="attack_metric_success_count_thresh",
+        help=(
+            """for setting counter limit to stop further repetitions
+            given the attack is successful and the
+            --attack-fail-fast is true. Default = %(default)d"""
+        ),
+    )
+
+    attack_parser.add_argument(
+        "--attack-fail-fast",
+        action="store_true",
+        required=False,
+        dest="attack_fail_fast",
+        help=(
+            """to stop further repetitions when the given metric has fulfilled
+            a criteria for a specified number of times (--attack-metric-success-count-thresh)
+            and this has a true status.
+            Default = %(default)s"""
+        ),
+    )
+
     attack_parser.set_defaults(func=_run_attack)
 
+    attack_parser_config = subparsers.add_parser("run-attack-from-configfile")
+    attack_parser_config.add_argument(
+        "-j",
+        "--attack-config-json-file-name",
+        action="store",
+        required=True,
+        dest="attack_config_json_file_name",
+        type=str,
+        default="config_worstcase_cmd.json",
+        help=(
+            "Name of the .json file containing details for the run. Default = %(default)s"
+        ),
+    )
+
+    attack_parser_config.set_defaults(func=_run_attack_from_configfile)
+
     args = parser.parse_args()
 
     try:
         args.func(args)
     except AttributeError as e:  # pragma:no cover
         logger.error("Invalid command. Try --help to get more details")
         logger.error(e)
```

### Comparing `aisdc-1.0.4/aisdc/generate_report.py` & `aisdc-1.0.5/aisdc/generate_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
 
 class SummariseFDIFPvalsModule(SummariseAUCPvalsModule):
     """Summarise the number of significant FDIF p-values"""
 
     # TODO do we want to parameterise which FDIF (01, 001, etc)?
     def get_metric_list(self, input_dict: dict) -> list[float]:
+        """Get metrics_list from attack_instance_logger within JSON file"""
         metric_list = []
         for _, iteration_value in input_dict["attack_instance_logger"].items():
             metric_list.append(iteration_value["PDIF01"])
         metric_list = [np.exp(-m) for m in metric_list]
         return metric_list
 
     def __str__(self):
@@ -286,14 +287,17 @@
     return returned_string
 
 
 def process_json(input_filename: str, output_filename: str):
     """
     Function that takes an input JSON filename and outputs a neat text file summarising results
     """
+
+    output_filename = output_filename.replace(" ", "_")
+
     with open(input_filename) as f:
         json_report = json.loads(f.read())
 
     modules = [
         FinalRecommendationModule(json_report),
     ]
```

### Comparing `aisdc-1.0.4/aisdc/metrics.py` & `aisdc-1.0.5/aisdc/metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/preprocessing/loaders.py` & `aisdc-1.0.5/aisdc/preprocessing/loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/safemodel/classifiers/dp_svc.py` & `aisdc-1.0.5/aisdc/safemodel/classifiers/dp_svc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/safemodel/classifiers/new_model_template.py` & `aisdc-1.0.5/aisdc/safemodel/classifiers/new_model_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         ModelToMakeSafer.__init__(self, **the_kwds)
         self.model_type: str = "ModelToMakeSafer"
         super().preliminary_check(apply_constraints=True, verbose=True)
         self.ignore_items = [
             "model_save_file",
             "ignore_items",
             "base_estimator_",
+            "timestamp",
         ]
         self.examine_seperately_items = ["base_estimator", "estimators_"]
 
     def additional_checks(  # pylint: disable=too-many-nested-blocks,too-many-branches
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
         """ModelToMakeSafer specific checks
```

### Comparing `aisdc-1.0.4/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py` & `aisdc-1.0.5/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,20 @@
         the_kwds = {}
         for key, val in kwargs.items():
             if key in self.basemodel_paramnames:
                 the_kwds[key] = val
         DecisionTreeClassifier.__init__(self, **the_kwds)
         self.model_type: str = "DecisionTreeClassifier"
         super().preliminary_check(apply_constraints=True, verbose=True)
-        self.ignore_items = ["model_save_file", "basemodel_paramnames", "ignore_items"]
+        self.ignore_items = [
+            "model_save_file",
+            "basemodel_paramnames",
+            "ignore_items",
+            "timestamp",
+        ]
         self.examine_seperately_items = ["tree_"]
         self.k_anonymity = 0
 
     def additional_checks(
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
         """Decision Tree-specific checks"""
```

### Comparing `aisdc-1.0.4/aisdc/safemodel/classifiers/safekeras.py` & `aisdc-1.0.5/aisdc/safemodel/classifiers/safekeras.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/safemodel/classifiers/saferandomforestclassifier.py` & `aisdc-1.0.5/aisdc/safemodel/classifiers/saferandomforestclassifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         RandomForestClassifier.__init__(self, **the_kwds)
         self.model_type: str = "RandomForestClassifier"
         super().preliminary_check(apply_constraints=True, verbose=True)
         self.ignore_items = [
             "model_save_file",
             "ignore_items",
             "base_estimator_",  # this is an object
+            "timestamp",
         ]
         self.examine_seperately_items = ["estimators_", "base_estimator"]
         self.k_anonymity = 0
 
     def additional_checks(  # pylint: disable=too-many-nested-blocks,too-many-branches
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
```

### Comparing `aisdc-1.0.4/aisdc/safemodel/classifiers/safesvc.py` & `aisdc-1.0.5/aisdc/safemodel/classifiers/safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/safemodel/classifiers/safetf.py` & `aisdc-1.0.5/aisdc/safemodel/classifiers/safetf.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/safemodel/reporting.py` & `aisdc-1.0.5/aisdc/safemodel/reporting.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/safemodel/rules.json` & `aisdc-1.0.5/aisdc/safemodel/rules.json`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/aisdc/safemodel/safemodel.py` & `aisdc-1.0.5/aisdc/safemodel/safemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,15 @@
         self.model_load_file: str = "None"
         self.model_save_file: str = "None"
         self.ignore_items: list[str] = []
         self.examine_seperately_items: list[str] = []
         self.basemodel_paramnames = []
         self.filename: str = "None"
         self.researcher: str = "None"
+        self.timestamp: str = "None"
         try:
             self.researcher = getpass.getuser()
         except (ImportError, KeyError, OSError):  # pragma: no cover
             self.researcher = "unknown"
 
     def get_params(self, deep=True):
         """gets dictionary of parameter values
@@ -736,15 +737,15 @@
          2. If data_obj is not null, then worst case MIA and attribute inference
          attacks are called via run_attack.
          Outputs from the attacks will be stored in filebase_attack_res.json
 
 
 
         """
-        if filename == "undefined":
+        if filename == "undefined":  # pragma: no cover
             print("You must provide the name of the file you want to save your model")
             print("For security reasons, this will overwrite previous versions")
         else:
             self.save(filename)
             msg_prel, disclosive_prel = self.preliminary_check(verbose=False)
             msg_post, disclosive_post = self.posthoc_check()
 
@@ -776,15 +777,16 @@
                     output[f"{attack_name}_results"] = self.run_attack(
                         data_obj,
                         attack_name,
                         f"{os.path.splitext(filename)[0]}_{attack_name}_res",
                     )
 
             now = datetime.datetime.now()
-            output["timestamp"] = str(now.strftime("%Y-%m-%d %H:%M:%S"))
+            self.timestamp = str(now.strftime("%Y-%m-%d %H:%M:%S"))
+            output["timestamp"] = self.timestamp
 
             outputfilename = self.researcher + "_checkfile.json"
             data = [output]
             # load existing results
             if os.path.isfile(outputfilename):
                 with open(outputfilename, newline="", encoding="utf-8") as file:
                     try:
```

### Comparing `aisdc-1.0.4/aisdc.egg-info/PKG-INFO` & `aisdc-1.0.5/aisdc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.4/aisdc.egg-info/SOURCES.txt` & `aisdc-1.0.5/aisdc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 aisdc.egg-info/dependency_links.txt
 aisdc.egg-info/requires.txt
 aisdc.egg-info/top_level.txt
 aisdc/attacks/__init__.py
 aisdc/attacks/attack.py
 aisdc/attacks/attribute_attack.py
 aisdc/attacks/dataset.py
+aisdc/attacks/failfast.py
 aisdc/attacks/likelihood_attack.py
 aisdc/attacks/report.py
 aisdc/attacks/worst_case_attack.py
 aisdc/preprocessing/__init__.py
 aisdc/preprocessing/loaders.py
 aisdc/safemodel/__init__.py
 aisdc/safemodel/reporting.py
@@ -31,14 +32,15 @@
 aisdc/safemodel/classifiers/safesvc.py
 aisdc/safemodel/classifiers/safetf.py
 tests/test_attacks.py
 tests/test_attacks_dataset.py
 tests/test_attacks_via_safemodel.py
 tests/test_attribute_inference_attack.py
 tests/test_data_interface.py
+tests/test_failfast.py
 tests/test_generate_report.py
 tests/test_lira_attack.py
 tests/test_loaders.py
 tests/test_metrics.py
 tests/test_safedecisiontreeclassifier.py
 tests/test_safekeras2.py
 tests/test_safemodel.py
```

### Comparing `aisdc-1.0.4/setup.py` & `aisdc-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="aisdc",
-    version="1.0.4",
+    version="1.0.5",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="Tools for the statistical disclosure control of machine learning models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/AI-SDC",
@@ -27,14 +27,15 @@
         "multiprocess~=0.70.12.2",
         "numpy~=1.21",
         "pandas~=1.5.0",
         "scikit_learn~=1.1.2",
         "scipy~=1.7",
         "tensorflow~=2.10.0",
         "tensorflow_privacy~=0.8.7",
+        "uuid~=1.30",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `aisdc-1.0.4/tests/test_attacks.py` & `aisdc-1.0.5/tests/test_attacks.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_attacks_dataset.py` & `aisdc-1.0.5/tests/test_attacks_dataset.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_attacks_via_safemodel.py` & `aisdc-1.0.5/tests/test_attacks_via_safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_attribute_inference_attack.py` & `aisdc-1.0.5/tests/test_attribute_inference_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_data_interface.py` & `aisdc-1.0.5/tests/test_data_interface.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_generate_report.py` & `aisdc-1.0.5/tests/test_generate_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,14 +74,29 @@
         a = AnalysisModule()
         with pytest.raises(NotImplementedError):
             a.process_dict()
 
         with pytest.raises(NotImplementedError):
             str(a)
 
+    def test_whitespace_in_filenames(self):
+        """test to make sure whitespace is removed from the output file when creating the report"""
+        json_formatted = self.get_test_report()
+
+        filename = "test.json"
+        output_filename = "filename should be changed.txt"
+
+        with open(filename, "w", encoding="utf-8") as f:
+            json.dump(json_formatted, f)
+
+        process_json(filename, output_filename)
+
+        assert os.path.exists("filename should be changed.txt") is False
+        assert os.path.exists("filename_should_be_changed.txt") is True
+
     def test_svm(self):
         """test the process_json function when the target model is an SVM"""
         json_formatted = self.get_test_report()
 
         f = FinalRecommendationModule(json_formatted)
         returned = f.process_dict()
 
@@ -174,10 +189,16 @@
     def test_complete_runthrough(self):
         """test the full process_json file end-to-end when valid parameters are passed"""
         json_formatted = self.get_test_report()
         _ = self.process_json_from_file(json_formatted)
 
     def test_cleanup(self):
         """gets rid of files created during tests"""
-        names = ["test.json", "results.txt", "1024-WorstCase attack.png"]
+        names = [
+            "test.json",
+            "results.txt",
+            "1024-WorstCase attack.png",
+            "filename should be changed.txt",
+            "filename_should_be_changed.txt",
+        ]
         for name in names:
             self.clean_up(name)
```

### Comparing `aisdc-1.0.4/tests/test_loaders.py` & `aisdc-1.0.5/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_metrics.py` & `aisdc-1.0.5/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_safedecisiontreeclassifier.py` & `aisdc-1.0.5/tests/test_safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_safekeras2.py` & `aisdc-1.0.5/tests/test_safekeras2.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_safemodel.py` & `aisdc-1.0.5/tests/test_safemodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ tests for fnctionality in super class"""
 import copy
+import json
 import os
 import pickle
 
 import joblib
 import numpy as np
 from sklearn import datasets
 
@@ -63,15 +64,20 @@
         )
         the_kwds = {}
         for key, val in kwargs.items():
             if key in self.basemodel_paramnames:
                 the_kwds[key] = val
         DummyClassifier.__init__(self, **the_kwds)
         self.model_type: str = "DummyClassifier"
-        self.ignore_items = ["model_save_file", "basemodel_paramnames", "ignore_items"]
+        self.ignore_items = [
+            "model_save_file",
+            "basemodel_paramnames",
+            "ignore_items",
+            "timestamp",
+        ]
         # create an item to test additional_checks()
         self.examine_seperately_items = ["newthing"]
         self.newthing = ["myStringKey", "aString", "myIntKey", "42"]
 
     def set_params(self, **kwargs):  # pragma: no cover
         """sets params"""
         for key, val in kwargs.items():  # pylint:disable=unused-variable
@@ -502,17 +508,45 @@
         f"{model.newthing}\n"
         f'{model.saved_model["newthing"]}'
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
     assert disclosive is True
 
 
-def test_request_release():
-    """checks requestrelease code works"""
+def test_request_release_without_attcks():
+    """checks requestrelease code works and check the content of the json file"""
     model = SafeDummyClassifier()
     x, y = get_data()
     model.fit(x, y)
     # give it k_anonymity
     model.k_anonymity = 5  # pylint: disable=attribute-defined-outside-init
 
     # no file provided, has k_anonymity
-    model.request_release()
+
+    filename = "test.pkl"
+    json_filename = model.researcher + "_checkfile.json"
+    model.request_release(filename)
+
+    # check that pikle and the json files have been created
+    assert os.path.isfile(filename)
+    assert os.path.isfile(json_filename)
+
+    # check the content of the json file
+    with open(f"./{json_filename}", encoding="utf-8") as file:
+        json_data = json.load(file)
+
+        details, _ = model.preliminary_check(verbose=False)
+        msg_post, _ = model.posthoc_check()
+        k_anonymity = f"{model.k_anonymity}"
+        recommendation = "Do not allow release"
+        reason = details + msg_post
+
+        assert {
+            "researcher": model.researcher,
+            "model_type": model.model_type,
+            "model_save_file": filename,
+            "details": details,
+            "k_anonymity": k_anonymity,
+            "recommendation": recommendation,
+            "reason": reason,
+            "timestamp": model.timestamp,
+        } in json_data
```

### Comparing `aisdc-1.0.4/tests/test_saferandomforestclassifier.py` & `aisdc-1.0.5/tests/test_saferandomforestclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_safesvc.py` & `aisdc-1.0.5/tests/test_safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.4/tests/test_worst_case_attack.py` & `aisdc-1.0.5/tests/test_worst_case_attack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """test_worst_case_attack.py
 Copyright (C) Jim Smith 2022 <james.smith@uwe.ac.uk>
 """
+import json
 import os
 import sys
 from unittest.mock import patch
 
 import numpy as np
 import pytest
 from sklearn.datasets import load_breast_cancer
@@ -16,14 +17,75 @@
 
 def clean_up(name):
     """removes unwanted files or directory"""
     if os.path.exists(name) and os.path.isfile(name):
         os.remove(name)
 
 
+def test_config_file_arguments_parsin():
+    """tests reading parameters from the configuration file"""
+    config = {
+        "n_reps": 12,
+        "n_dummy_reps": 2,
+        "p_thresh": 0.06,
+        "test_prop": 0.4,
+        "report_name": "programmatically_worstcase_report_test",
+    }
+    with open("config_worstcase_test.json", "w", encoding="utf-8") as f:
+        f.write(json.dumps(config))
+    args = worst_case_attack.WorstCaseAttackArgs(
+        attack_config_json_file_name="config_worstcase_test.json",
+    )
+    assert args.__dict__["n_reps"] == config["n_reps"]
+    assert args.__dict__["n_dummy_reps"] == config["n_dummy_reps"]
+    assert args.__dict__["p_thresh"] == config["p_thresh"]
+    assert args.__dict__["test_prop"] == config["test_prop"]
+    assert args.__dict__["report_name"] == config["report_name"]
+    os.remove("config_worstcase_test.json")
+
+
+def test_attack_from_predictions_cmd():
+    """Running attack using configuration file and prediction files"""
+    X, y = load_breast_cancer(return_X_y=True, as_frame=False)
+    train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
+    dataset_obj = dataset.Data()
+    dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
+
+    target_model = SVC(gamma=0.1, probability=True)
+    target_model.fit(train_X, train_y)
+    ytr_pred = target_model.predict_proba(train_X)
+    yte_pred = target_model.predict_proba(test_X)
+    np.savetxt("ypred_train.csv", ytr_pred, delimiter=",")
+    np.savetxt("ypred_test.csv", yte_pred, delimiter=",")
+
+    config = {
+        "n_reps": 30,
+        "n_dummy_reps": 2,
+        "p_thresh": 0.05,
+        "test_prop": 0.5,
+        "training_preds_filename": "ypred_train.csv",
+        "test_preds_filename": "ypred_test.csv",
+        "attack_metric_success_name": "P_HIGHER_AUC",
+        "attack_metric_success_thresh": 0.05,
+        "attack_metric_success_comp_type": "lte",
+        "attack_metric_success_count_thresh": 2,
+        "attack_fail_fast": True,
+    }
+
+    with open("config_worstcase_cmd.json", "w", encoding="utf-8") as f:
+        f.write(json.dumps(config))
+    os.system(
+        f"{sys.executable} -m aisdc.attacks.worst_case_attack run-attack-from-configfile "
+        "--attack-config-json-file-name config_worstcase_cmd.json "
+    )
+    os.remove("config_worstcase_cmd.json")
+    os.remove("ypred_train.csv")
+    os.remove("ypred_test.csv")
+
+
 def test_report_worstcase():
     """tests worst case attack directly"""
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
     dataset_obj = dataset.Data()
     dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
 
@@ -34,16 +96,16 @@
 
     args = worst_case_attack.WorstCaseAttackArgs(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=1,
         p_thresh=0.05,
-        in_sample_filename=None,
-        out_sample_filename=None,
+        training_preds_filename=None,
+        test_preds_filename=None,
         test_prop=0.5,
         report_name="test-10reps",
     )
 
     # with multiple reps
     attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.attack(dataset_obj, target_model)
@@ -51,16 +113,16 @@
     _ = attack_obj.make_report()
 
     # with one rep
     args = worst_case_attack.WorstCaseAttackArgs(
         n_reps=1,
         n_dummy_reps=1,
         p_thresh=0.05,
-        in_sample_filename=None,
-        out_sample_filename=None,
+        training_preds_filename=None,
+        test_preds_filename=None,
         test_prop=0.5,
         report_name="test-1rep",
     )
 
     attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.attack(dataset_obj, target_model)
     _ = attack_obj.make_report()
@@ -78,16 +140,16 @@
 
     args = worst_case_attack.WorstCaseAttackArgs(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=1,
         n_dummy_reps=1,
         p_thresh=0.05,
-        in_sample_filename=None,
-        out_sample_filename=None,
+        training_preds_filename=None,
+        test_preds_filename=None,
         test_prop=0.5,
         report_name="test-1rep",
         include_model_correct_feature=True,
     )
 
     # with multiple reps
     attack_obj = worst_case_attack.WorstCaseAttack(args)
@@ -116,21 +178,21 @@
 
     args = worst_case_attack.WorstCaseAttackArgs(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=1,
         p_thresh=0.05,
-        in_sample_filename="ypred_train.csv",
-        out_sample_filename="ypred_test.csv",
+        training_preds_filename="ypred_train.csv",
+        test_preds_filename="ypred_test.csv",
         test_prop=0.5,
         report_name="test-10reps",
     )
 
-    assert args.get_args()["in_sample_filename"] == "ypred_train.csv"
+    assert args.get_args()["training_preds_filename"] == "ypred_train.csv"
     print(args)
 
     # with multiple reps
     attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.attack_from_prediction_files()
 
 
@@ -151,21 +213,21 @@
 
     args = worst_case_attack.WorstCaseAttackArgs(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=0,
         p_thresh=0.05,
-        in_sample_filename="ypred_train.csv",
-        out_sample_filename="ypred_test.csv",
+        training_preds_filename="ypred_train.csv",
+        test_preds_filename="ypred_test.csv",
         test_prop=0.5,
         report_name="test-10reps",
     )
 
-    assert args.get_args()["in_sample_filename"] == "ypred_train.csv"
+    assert args.get_args()["training_preds_filename"] == "ypred_train.csv"
     print(args)
 
     # with multiple reps
     attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.attack_from_prediction_files()
 
 
@@ -173,16 +235,16 @@
     """test functionality around creating dummy data"""
     args = worst_case_attack.WorstCaseAttackArgs(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=1,
         p_thresh=0.05,
-        in_sample_filename="ypred_train.csv",
-        out_sample_filename="ypred_test.csv",
+        training_preds_filename="ypred_train.csv",
+        test_preds_filename="ypred_test.csv",
         test_prop=0.5,
         report_name="test-10reps",
     )
 
     attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.make_dummy_data()
```

