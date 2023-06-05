# Comparing `tmp/giefstat-0.0.2.tar.gz` & `tmp/giefstat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giefstat-0.0.2.tar", last modified: Mon Jun  5 09:36:30 2023, max compression
+gzip compressed data, was "giefstat-0.0.3.tar", last modified: Mon Jun  5 09:47:49 2023, max compression
```

## Comparing `giefstat-0.0.2.tar` & `giefstat-0.0.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.837090 giefstat-0.0.2/
--rw-rw-rw-   0        0        0     3665 2023-06-05 09:36:30.836092 giefstat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-06-05 09:28:09.000000 giefstat-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.761294 giefstat-0.0.2/estimate/
--rw-rw-rw-   0        0        0     3953 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/__init__.py
--rw-rw-rw-   0        0        0     5258 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/_univar_encoding.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.763288 giefstat-0.0.2/estimate/gief/
--rw-rw-rw-   0        0        0      414 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.768274 giefstat-0.0.2/estimate/gief/entropy/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/entropy/__init__.py
--rw-rw-rw-   0        0        0      915 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/entropy/cond_entropy.py
--rw-rw-rw-   0        0        0     2602 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/entropy/marg_entropy.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.777252 giefstat-0.0.2/estimate/gief/mutual_info/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/mutual_info/__init__.py
--rw-rw-rw-   0        0        0    11405 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/mutual_info/_kraskov.py
--rw-rw-rw-   0        0        0     2767 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/mutual_info/_ross.py
--rw-rw-rw-   0        0        0     2651 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/mutual_info/cmi.py
--rw-rw-rw-   0        0        0     1931 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/gief/mutual_info/mi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.780242 giefstat-0.0.2/estimate/kde/
--rw-rw-rw-   0        0        0       89 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/kde/__init__.py
--rw-rw-rw-   0        0        0     3015 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/kde/kde.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.786227 giefstat-0.0.2/estimate/mic/
--rw-rw-rw-   0        0        0      194 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/mic/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/mic/_mic_rmic.py
--rw-rw-rw-   0        0        0     2802 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/mic/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.789219 giefstat-0.0.2/estimate/model_based/
--rw-rw-rw-   0        0        0      260 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/model_based/__init__.py
--rw-rw-rw-   0        0        0     4099 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/model_based/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.793208 giefstat-0.0.2/estimate/other/
--rw-rw-rw-   0        0        0      289 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/other/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-26 06:57:38.000000 giefstat-0.0.2/estimate/other/coefficient.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.800190 giefstat-0.0.2/estimate/quant_based/
--rw-rw-rw-   0        0        0      281 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/quant_based/__init__.py
--rw-rw-rw-   0        0        0     7282 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/quant_based/_quant_darbellay.py
--rw-rw-rw-   0        0        0     2111 2023-04-27 08:37:39.000000 giefstat-0.0.2/estimate/quant_based/mi_classic.py
--rw-rw-rw-   0        0        0     1700 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/quant_based/mi_darbellay.py
--rw-rw-rw-   0        0        0       90 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/setting.py
--rw-rw-rw-   0        0        0     3447 2023-04-26 05:55:04.000000 giefstat-0.0.2/estimate/util.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.811161 giefstat-0.0.2/giefstat.egg-info/
--rw-rw-rw-   0        0        0     3665 2023-06-05 09:36:30.000000 giefstat-0.0.2/giefstat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1292 2023-06-05 09:36:30.000000 giefstat-0.0.2/giefstat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:36:30.000000 giefstat-0.0.2/giefstat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-05 09:36:30.000000 giefstat-0.0.2/giefstat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-05 09:36:30.000000 giefstat-0.0.2/giefstat.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.814154 giefstat-0.0.2/mod/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.2/mod/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.818142 giefstat-0.0.2/mod/config/
--rw-rw-rw-   0        0        0      181 2023-04-26 05:55:04.000000 giefstat-0.0.2/mod/config/__init__.py
--rw-rw-rw-   0        0        0     4929 2023-04-26 05:55:04.000000 giefstat-0.0.2/mod/config/config_loader.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.821135 giefstat-0.0.2/mod/data_encoding/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.2/mod/data_encoding/__init__.py
--rw-rw-rw-   0        0        0     5410 2023-04-26 05:55:04.000000 giefstat-0.0.2/mod/data_encoding/univar_encoding.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.826120 giefstat-0.0.2/mod/data_process/
--rw-rw-rw-   0        0        0      847 2023-04-26 05:55:04.000000 giefstat-0.0.2/mod/data_process/__init__.py
--rw-rw-rw-   0        0        0    13764 2023-04-26 05:55:04.000000 giefstat-0.0.2/mod/data_process/numpy.py
--rw-rw-rw-   0        0        0       42 2023-06-05 09:36:30.837090 giefstat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-06-05 09:36:25.000000 giefstat-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:36:30.834098 giefstat-0.0.2/statistical_tools/
--rw-rw-rw-   0        0        0      498 2023-06-05 07:37:56.000000 giefstat-0.0.2/statistical_tools/__init__.py
--rw-rw-rw-   0        0        0     3142 2023-06-05 08:29:21.000000 giefstat-0.0.2/statistical_tools/surrog_indep_test.py
--rw-rw-rw-   0        0        0     2692 2023-06-05 08:41:34.000000 giefstat-0.0.2/statistical_tools/time_delayed_association.py
--rw-rw-rw-   0        0        0     1068 2023-06-05 07:46:14.000000 giefstat-0.0.2/statistical_tools/util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.588308 giefstat-0.0.3/
+-rw-rw-rw-   0        0        0     4294 2023-06-05 09:47:49.587312 giefstat-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3169 2023-06-05 09:47:24.000000 giefstat-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.506529 giefstat-0.0.3/estimate/
+-rw-rw-rw-   0        0        0     3953 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/__init__.py
+-rw-rw-rw-   0        0        0     5258 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/_univar_encoding.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.508524 giefstat-0.0.3/estimate/gief/
+-rw-rw-rw-   0        0        0      414 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.513509 giefstat-0.0.3/estimate/gief/entropy/
+-rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/entropy/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/entropy/cond_entropy.py
+-rw-rw-rw-   0        0        0     2602 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/entropy/marg_entropy.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.525477 giefstat-0.0.3/estimate/gief/mutual_info/
+-rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/__init__.py
+-rw-rw-rw-   0        0        0    11405 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/_kraskov.py
+-rw-rw-rw-   0        0        0     2767 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/_ross.py
+-rw-rw-rw-   0        0        0     2651 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/cmi.py
+-rw-rw-rw-   0        0        0     1931 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/mi.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.529467 giefstat-0.0.3/estimate/kde/
+-rw-rw-rw-   0        0        0       89 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/kde/__init__.py
+-rw-rw-rw-   0        0        0     3015 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/kde/kde.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.535451 giefstat-0.0.3/estimate/mic/
+-rw-rw-rw-   0        0        0      194 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/mic/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/mic/_mic_rmic.py
+-rw-rw-rw-   0        0        0     2802 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/mic/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.539441 giefstat-0.0.3/estimate/model_based/
+-rw-rw-rw-   0        0        0      260 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/model_based/__init__.py
+-rw-rw-rw-   0        0        0     4099 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/model_based/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.543429 giefstat-0.0.3/estimate/other/
+-rw-rw-rw-   0        0        0      289 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/other/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-26 06:57:38.000000 giefstat-0.0.3/estimate/other/coefficient.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.550411 giefstat-0.0.3/estimate/quant_based/
+-rw-rw-rw-   0        0        0      281 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/quant_based/__init__.py
+-rw-rw-rw-   0        0        0     7282 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/quant_based/_quant_darbellay.py
+-rw-rw-rw-   0        0        0     2111 2023-04-27 08:37:39.000000 giefstat-0.0.3/estimate/quant_based/mi_classic.py
+-rw-rw-rw-   0        0        0     1700 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/quant_based/mi_darbellay.py
+-rw-rw-rw-   0        0        0       90 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/setting.py
+-rw-rw-rw-   0        0        0     3447 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.560384 giefstat-0.0.3/giefstat.egg-info/
+-rw-rw-rw-   0        0        0     4294 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1292 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.562379 giefstat-0.0.3/mod/
+-rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.566367 giefstat-0.0.3/mod/config/
+-rw-rw-rw-   0        0        0      181 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/config/__init__.py
+-rw-rw-rw-   0        0        0     4929 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/config/config_loader.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.570358 giefstat-0.0.3/mod/data_encoding/
+-rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_encoding/__init__.py
+-rw-rw-rw-   0        0        0     5410 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_encoding/univar_encoding.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.576341 giefstat-0.0.3/mod/data_process/
+-rw-rw-rw-   0        0        0      847 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_process/__init__.py
+-rw-rw-rw-   0        0        0    13764 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_process/numpy.py
+-rw-rw-rw-   0        0        0       42 2023-06-05 09:47:49.588308 giefstat-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-06-05 09:47:31.000000 giefstat-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.585317 giefstat-0.0.3/statistical_tools/
+-rw-rw-rw-   0        0        0      498 2023-06-05 07:37:56.000000 giefstat-0.0.3/statistical_tools/__init__.py
+-rw-rw-rw-   0        0        0     3142 2023-06-05 08:29:21.000000 giefstat-0.0.3/statistical_tools/surrog_indep_test.py
+-rw-rw-rw-   0        0        0     2692 2023-06-05 08:41:34.000000 giefstat-0.0.3/statistical_tools/time_delayed_association.py
+-rw-rw-rw-   0        0        0     1068 2023-06-05 07:46:14.000000 giefstat-0.0.3/statistical_tools/util.py
```

### Comparing `giefstat-0.0.2/PKG-INFO` & `giefstat-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Description: ### general-information-estimation-framework
         
@@ -12,17 +12,19 @@
         
         1. ~~script/独立性检验/statistical_power_test.py~~
         2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
         3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
         
         ### Project Purpose
         
-        For computing higher-order information interractions between arbitrary types of variables
+        This project aims for:
+        1. computing higher-order information interactions between differen types (discrete & continuous) of variables
+        2. uncovering complex associations and causal relationships in high-dimensional data
         
-        ### 项目结构
+        ### Project Structure
         
         ```
         |-- general-information-estimation-framework
             |-- estimate            # information estimation base on KNN, KDE, etc.
                 |-- __init__.py     
                 |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
                 |-- util.py
@@ -83,11 +85,19 @@
             cal_general_assoc --> surrog_indep_test
             surrog_indep_test --> time_delayed_assocication
         end
         
         estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
         ```
         
+        ### References
+        
+        1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+        2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+        3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+        4. https://github.com/dizcza/entropy-estimators
+        5. https://github.com/danielhomola/mifs
+        
         
 Keywords: python,information estimation
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `giefstat-0.0.2/README.md` & `giefstat-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 1. ~~script/独立性检验/statistical_power_test.py~~
 2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
 3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
 
 ### Project Purpose
 
-For computing higher-order information interractions between arbitrary types of variables
+This project aims for:
+1. computing higher-order information interactions between differen types (discrete & continuous) of variables
+2. uncovering complex associations and causal relationships in high-dimensional data
 
-### 项目结构
+### Project Structure
 
 ```
 |-- general-information-estimation-framework
     |-- estimate            # information estimation base on KNN, KDE, etc.
         |-- __init__.py     
         |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
         |-- util.py
@@ -75,7 +77,15 @@
     cal_general_assoc --> surrog_indep_test
     surrog_indep_test --> time_delayed_assocication
 end
 
 estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
 ```
 
+### References
+
+1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+4. https://github.com/dizcza/entropy-estimators
+5. https://github.com/danielhomola/mifs
+
```

### Comparing `giefstat-0.0.2/estimate/__init__.py` & `giefstat-0.0.3/estimate/__init__.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/_univar_encoding.py` & `giefstat-0.0.3/estimate/_univar_encoding.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/gief/entropy/cond_entropy.py` & `giefstat-0.0.3/estimate/gief/entropy/cond_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/gief/entropy/marg_entropy.py` & `giefstat-0.0.3/estimate/gief/entropy/marg_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/gief/mutual_info/_kraskov.py` & `giefstat-0.0.3/estimate/gief/mutual_info/_kraskov.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/gief/mutual_info/_ross.py` & `giefstat-0.0.3/estimate/gief/mutual_info/_ross.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/gief/mutual_info/cmi.py` & `giefstat-0.0.3/estimate/gief/mutual_info/cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/gief/mutual_info/mi.py` & `giefstat-0.0.3/estimate/gief/mutual_info/mi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/kde/kde.py` & `giefstat-0.0.3/estimate/kde/kde.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/mic/_mic_rmic.py` & `giefstat-0.0.3/estimate/mic/_mic_rmic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/mic/mi_cmi.py` & `giefstat-0.0.3/estimate/mic/mi_cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/model_based/mi_cmi.py` & `giefstat-0.0.3/estimate/model_based/mi_cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/other/coefficient.py` & `giefstat-0.0.3/estimate/other/coefficient.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/quant_based/_quant_darbellay.py` & `giefstat-0.0.3/estimate/quant_based/_quant_darbellay.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/quant_based/mi_classic.py` & `giefstat-0.0.3/estimate/quant_based/mi_classic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/quant_based/mi_darbellay.py` & `giefstat-0.0.3/estimate/quant_based/mi_darbellay.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/estimate/util.py` & `giefstat-0.0.3/estimate/util.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/giefstat.egg-info/PKG-INFO` & `giefstat-0.0.3/giefstat.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Description: ### general-information-estimation-framework
         
@@ -12,17 +12,19 @@
         
         1. ~~script/独立性检验/statistical_power_test.py~~
         2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
         3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
         
         ### Project Purpose
         
-        For computing higher-order information interractions between arbitrary types of variables
+        This project aims for:
+        1. computing higher-order information interactions between differen types (discrete & continuous) of variables
+        2. uncovering complex associations and causal relationships in high-dimensional data
         
-        ### 项目结构
+        ### Project Structure
         
         ```
         |-- general-information-estimation-framework
             |-- estimate            # information estimation base on KNN, KDE, etc.
                 |-- __init__.py     
                 |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
                 |-- util.py
@@ -83,11 +85,19 @@
             cal_general_assoc --> surrog_indep_test
             surrog_indep_test --> time_delayed_assocication
         end
         
         estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
         ```
         
+        ### References
+        
+        1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+        2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+        3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+        4. https://github.com/dizcza/entropy-estimators
+        5. https://github.com/danielhomola/mifs
+        
         
 Keywords: python,information estimation
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `giefstat-0.0.2/giefstat.egg-info/SOURCES.txt` & `giefstat-0.0.3/giefstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/mod/config/config_loader.py` & `giefstat-0.0.3/mod/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/mod/data_encoding/univar_encoding.py` & `giefstat-0.0.3/mod/data_encoding/univar_encoding.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/mod/data_process/__init__.py` & `giefstat-0.0.3/mod/data_process/__init__.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/mod/data_process/numpy.py` & `giefstat-0.0.3/mod/data_process/numpy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/setup.py` & `giefstat-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 import os
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Package for information estimation, independence test, etc."
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text(encoding="utf-8")
 
 setup(
     name="giefstat",
     version=VERSION,
```

### Comparing `giefstat-0.0.2/statistical_tools/surrog_indep_test.py` & `giefstat-0.0.3/statistical_tools/surrog_indep_test.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/statistical_tools/time_delayed_association.py` & `giefstat-0.0.3/statistical_tools/time_delayed_association.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.2/statistical_tools/util.py` & `giefstat-0.0.3/statistical_tools/util.py`

 * *Files identical despite different names*

