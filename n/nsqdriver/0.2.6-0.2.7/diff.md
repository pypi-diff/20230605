# Comparing `tmp/nsqdriver-0.2.6.tar.gz` & `tmp/nsqdriver-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsqdriver-0.2.6.tar", last modified: Wed May 17 07:10:58 2023, max compression
+gzip compressed data, was "nsqdriver-0.2.7.tar", last modified: Mon Jun  5 04:24:03 2023, max compression
```

## Comparing `nsqdriver-0.2.6.tar` & `nsqdriver-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.085828 nsqdriver-0.2.6/nsqdriver/
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/NS_CST.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/NS_MCI.py
--rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/NS_QSYNC.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/nsqdriver/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/wrapper/AWG_ADC.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/wrapper/ND_NSMCI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/nsqdriver/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/nsqdriver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 07:10:58.000000 nsqdriver-0.2.6/nsqdriver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:10:58.089828 nsqdriver-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_cy_gen_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_demod_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_driver_info_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_init_device.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_mixer_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_param_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_rfskit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-17 07:10:51.000000 nsqdriver-0.2.6/tests/test_rpc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.766407 nsqdriver-0.2.7/nsqdriver/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/NS_CST.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/NS_MCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/NS_QSYNC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/nsqdriver/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/AWG_ADC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/BD_NSMCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/ND_NSMCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/nsqdriver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_cy_gen_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_demod_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_driver_info_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_init_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_mixer_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_param_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_rfskit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_rpc_parser.py
```

### Comparing `nsqdriver-0.2.6/PKG-INFO` & `nsqdriver-0.2.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsqdriver
-Version: 0.2.6
+Version: 0.2.7
 Summary: Naishu Q series quantum measurement and control equipment driver interface
 Home-page: https://g2hoyqcmh4.feishu.cn/wiki/wikcnzvyMd82DLZUe2NsI6HxsFc
 Author: Naishu Technology
 Author-email: jilianyi@naishu.tech
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nsqdriver-0.2.6/README.md` & `nsqdriver-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/nsqdriver/NS_CST.py` & `nsqdriver-0.2.7/nsqdriver/NS_CST.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/nsqdriver/NS_MCI.py` & `nsqdriver-0.2.7/nsqdriver/NS_MCI.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/nsqdriver/NS_QSYNC.py` & `nsqdriver-0.2.7/nsqdriver/NS_QSYNC.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/nsqdriver/wrapper/AWG_ADC.py` & `nsqdriver-0.2.7/nsqdriver/wrapper/AWG_ADC.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/nsqdriver/wrapper/ND_NSMCI.py` & `nsqdriver-0.2.7/nsqdriver/wrapper/ND_NSMCI.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/nsqdriver.egg-info/PKG-INFO` & `nsqdriver-0.2.7/nsqdriver.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsqdriver
-Version: 0.2.6
+Version: 0.2.7
 Summary: Naishu Q series quantum measurement and control equipment driver interface
 Home-page: https://g2hoyqcmh4.feishu.cn/wiki/wikcnzvyMd82DLZUe2NsI6HxsFc
 Author: Naishu Technology
 Author-email: jilianyi@naishu.tech
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nsqdriver-0.2.6/nsqdriver.egg-info/SOURCES.txt` & `nsqdriver-0.2.7/nsqdriver.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 nsqdriver/setup.py
 nsqdriver.egg-info/PKG-INFO
 nsqdriver.egg-info/SOURCES.txt
 nsqdriver.egg-info/dependency_links.txt
 nsqdriver.egg-info/requires.txt
 nsqdriver.egg-info/top_level.txt
 nsqdriver/wrapper/AWG_ADC.py
+nsqdriver/wrapper/BD_NSMCI.py
 nsqdriver/wrapper/ND_NSMCI.py
 nsqdriver/wrapper/__init__.py
 tests/test_cy_gen_wave.py
 tests/test_demod_speed.py
 tests/test_driver_info_memory.py
 tests/test_init_device.py
 tests/test_mixer_simulator.py
```

### Comparing `nsqdriver-0.2.6/setup.py` & `nsqdriver-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/tests/test_cy_gen_wave.py` & `nsqdriver-0.2.7/tests/test_cy_gen_wave.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/tests/test_demod_speed.py` & `nsqdriver-0.2.7/tests/test_demod_speed.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/tests/test_driver_info_memory.py` & `nsqdriver-0.2.7/tests/test_driver_info_memory.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/tests/test_param_memory.py` & `nsqdriver-0.2.7/tests/test_param_memory.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/tests/test_rfskit_base.py` & `nsqdriver-0.2.7/tests/test_rfskit_base.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.6/tests/test_rpc_parser.py` & `nsqdriver-0.2.7/tests/test_rpc_parser.py`

 * *Files identical despite different names*

