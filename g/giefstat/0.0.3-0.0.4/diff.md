# Comparing `tmp/giefstat-0.0.3.tar.gz` & `tmp/giefstat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giefstat-0.0.3.tar", last modified: Mon Jun  5 09:47:49 2023, max compression
+gzip compressed data, was "giefstat-0.0.4.tar", last modified: Mon Jun  5 15:08:44 2023, max compression
```

## Comparing `giefstat-0.0.3.tar` & `giefstat-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.588308 giefstat-0.0.3/
--rw-rw-rw-   0        0        0     4294 2023-06-05 09:47:49.587312 giefstat-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3169 2023-06-05 09:47:24.000000 giefstat-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.506529 giefstat-0.0.3/estimate/
--rw-rw-rw-   0        0        0     3953 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/__init__.py
--rw-rw-rw-   0        0        0     5258 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/_univar_encoding.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.508524 giefstat-0.0.3/estimate/gief/
--rw-rw-rw-   0        0        0      414 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.513509 giefstat-0.0.3/estimate/gief/entropy/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/entropy/__init__.py
--rw-rw-rw-   0        0        0      915 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/entropy/cond_entropy.py
--rw-rw-rw-   0        0        0     2602 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/entropy/marg_entropy.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.525477 giefstat-0.0.3/estimate/gief/mutual_info/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/__init__.py
--rw-rw-rw-   0        0        0    11405 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/_kraskov.py
--rw-rw-rw-   0        0        0     2767 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/_ross.py
--rw-rw-rw-   0        0        0     2651 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/cmi.py
--rw-rw-rw-   0        0        0     1931 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/gief/mutual_info/mi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.529467 giefstat-0.0.3/estimate/kde/
--rw-rw-rw-   0        0        0       89 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/kde/__init__.py
--rw-rw-rw-   0        0        0     3015 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/kde/kde.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.535451 giefstat-0.0.3/estimate/mic/
--rw-rw-rw-   0        0        0      194 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/mic/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/mic/_mic_rmic.py
--rw-rw-rw-   0        0        0     2802 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/mic/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.539441 giefstat-0.0.3/estimate/model_based/
--rw-rw-rw-   0        0        0      260 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/model_based/__init__.py
--rw-rw-rw-   0        0        0     4099 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/model_based/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.543429 giefstat-0.0.3/estimate/other/
--rw-rw-rw-   0        0        0      289 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/other/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-26 06:57:38.000000 giefstat-0.0.3/estimate/other/coefficient.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.550411 giefstat-0.0.3/estimate/quant_based/
--rw-rw-rw-   0        0        0      281 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/quant_based/__init__.py
--rw-rw-rw-   0        0        0     7282 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/quant_based/_quant_darbellay.py
--rw-rw-rw-   0        0        0     2111 2023-04-27 08:37:39.000000 giefstat-0.0.3/estimate/quant_based/mi_classic.py
--rw-rw-rw-   0        0        0     1700 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/quant_based/mi_darbellay.py
--rw-rw-rw-   0        0        0       90 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/setting.py
--rw-rw-rw-   0        0        0     3447 2023-04-26 05:55:04.000000 giefstat-0.0.3/estimate/util.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.560384 giefstat-0.0.3/giefstat.egg-info/
--rw-rw-rw-   0        0        0     4294 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1292 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-05 09:47:49.000000 giefstat-0.0.3/giefstat.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.562379 giefstat-0.0.3/mod/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.566367 giefstat-0.0.3/mod/config/
--rw-rw-rw-   0        0        0      181 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/config/__init__.py
--rw-rw-rw-   0        0        0     4929 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/config/config_loader.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.570358 giefstat-0.0.3/mod/data_encoding/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_encoding/__init__.py
--rw-rw-rw-   0        0        0     5410 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_encoding/univar_encoding.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.576341 giefstat-0.0.3/mod/data_process/
--rw-rw-rw-   0        0        0      847 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_process/__init__.py
--rw-rw-rw-   0        0        0    13764 2023-04-26 05:55:04.000000 giefstat-0.0.3/mod/data_process/numpy.py
--rw-rw-rw-   0        0        0       42 2023-06-05 09:47:49.588308 giefstat-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-06-05 09:47:31.000000 giefstat-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:47:49.585317 giefstat-0.0.3/statistical_tools/
--rw-rw-rw-   0        0        0      498 2023-06-05 07:37:56.000000 giefstat-0.0.3/statistical_tools/__init__.py
--rw-rw-rw-   0        0        0     3142 2023-06-05 08:29:21.000000 giefstat-0.0.3/statistical_tools/surrog_indep_test.py
--rw-rw-rw-   0        0        0     2692 2023-06-05 08:41:34.000000 giefstat-0.0.3/statistical_tools/time_delayed_association.py
--rw-rw-rw-   0        0        0     1068 2023-06-05 07:46:14.000000 giefstat-0.0.3/statistical_tools/util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:08:44.304700 giefstat-0.0.4/
+-rw-rw-rw-   0        0        0     3561 2023-06-05 15:08:44.303702 giefstat-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3170 2023-06-05 14:19:49.000000 giefstat-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 15:08:44.302706 giefstat-0.0.4/giefstat.egg-info/
+-rw-rw-rw-   0        0        0     3561 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:08:44.304700 giefstat-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-06-05 15:06:31.000000 giefstat-0.0.4/setup.py
```

### Comparing `giefstat-0.0.3/PKG-INFO` & `giefstat-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,103 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
-Description: ### general-information-estimation-framework
-        
-        ### TODOs
-        
-        1. ~~script/独立性检验/statistical_power_test.py~~
-        2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
-        3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
-        
-        ### Project Purpose
-        
-        This project aims for:
-        1. computing higher-order information interactions between differen types (discrete & continuous) of variables
-        2. uncovering complex associations and causal relationships in high-dimensional data
-        
-        ### Project Structure
-        
-        ```
-        |-- general-information-estimation-framework
-            |-- estimate            # information estimation base on KNN, KDE, etc.
-                |-- __init__.py     
-                |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
-                |-- util.py
-                |-- _univar_encoding.py     # encoding one-dimensional variable data
-                |-- gief            # general information estimation
-                    __init__.py
-                    |-- entropy     # marginal and conditional entropies
-                        |-- __init__.py
-                        |-- cond_entropy.py
-                        |-- marg_entropy.py
-                    |-- mutual_info
-                        |-- __init__.py
-                        |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
-                        |-- _ross.py    # proposed by Ross
-                        |-- mi.py       # mutual information estimation
-                        |-- cmi.py      # conditional mutual information estimation
-        
-            |-- statistical_tools
-                |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
-                |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
-                |-- time_delayed_association.py         # time delayed association detection
-        
-            |-- script
-                |-- 独立性检验
-                    |-- indep_test.py               # independence test
-                    |-- statistical_power_test.py   # statistical power test
-                |-- 条件独立性检验
-                    |-- cond_indep_test.py          # conditional independence test
-                |-- 时延关联检测
-        
-        ```
-        
-        file dependency plot：
-        
-        ```mermaid
-        flowchart LR
-        
-        subgraph estimate
-            subgraph gief
-                H-G & MI-G & CMI-G
-            end
-        
-            subgraph kde
-                MI-KDE
-            end
-        
-            subgraph other
-                coefficient --> PearsonCorr & SpearmanCorr & DistCorr
-            end
-        
-            subgraph quant_based
-                MI-Classic --> MI-cut & MI-qcut
-                MI-Darbellay
-            end
-        end
-        
-        subgraph statistical_tools
-            cal_general_assoc --> surrog_indep_test
-            surrog_indep_test --> time_delayed_assocication
-        end
-        
-        estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
-        ```
-        
-        ### References
-        
-        1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
-        2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
-        3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
-        4. https://github.com/dizcza/entropy-estimators
-        5. https://github.com/danielhomola/mifs
-        
-        
 Keywords: python,information estimation
-Platform: UNKNOWN
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+
+### general-information-estimation-framework
+
+### TODOs
+
+1. ~~script/独立性检验/statistical_power_test.py~~
+2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
+3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
+
+### Project Purpose
+
+This project aims for:
+1. computing higher-order information interactions between different types (discrete & continuous) of variables
+2. uncovering complex associations and causal relationships in high-dimensional data
+
+### Project Structure
+
+```
+|-- general-information-estimation-framework
+    |-- estimate            # information estimation base on KNN, KDE, etc.
+        |-- __init__.py     
+        |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
+        |-- util.py
+        |-- _univar_encoding.py     # encoding one-dimensional variable data
+        |-- gief            # general information estimation
+            __init__.py
+            |-- entropy     # marginal and conditional entropies
+                |-- __init__.py
+                |-- cond_entropy.py
+                |-- marg_entropy.py
+            |-- mutual_info
+                |-- __init__.py
+                |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
+                |-- _ross.py    # proposed by Ross
+                |-- mi.py       # mutual information estimation
+                |-- cmi.py      # conditional mutual information estimation
+
+    |-- statistical_tools
+        |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
+        |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
+        |-- time_delayed_association.py         # time delayed association detection
+
+    |-- script
+        |-- 独立性检验
+            |-- indep_test.py               # independence test
+            |-- statistical_power_test.py   # statistical power test
+        |-- 条件独立性检验
+            |-- cond_indep_test.py          # conditional independence test
+        |-- 时延关联检测
+
+```
+
+file dependency plot：
+
+```mermaid
+flowchart LR
+
+subgraph estimate
+    subgraph gief
+        H-G & MI-G & CMI-G
+    end
+
+    subgraph kde
+        MI-KDE
+    end
+
+    subgraph other
+        coefficient --> PearsonCorr & SpearmanCorr & DistCorr
+    end
+
+    subgraph quant_based
+        MI-Classic --> MI-cut & MI-qcut
+        MI-Darbellay
+    end
+end
+
+subgraph statistical_tools
+    cal_general_assoc --> surrog_indep_test
+    surrog_indep_test --> time_delayed_assocication
+end
+
+estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
+```
+
+### References
+
+1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+4. https://github.com/dizcza/entropy-estimators
+5. https://github.com/danielhomola/mifs
+
```

### Comparing `giefstat-0.0.3/README.md` & `giefstat-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 1. ~~script/独立性检验/statistical_power_test.py~~
 2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
 3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
 
 ### Project Purpose
 
 This project aims for:
-1. computing higher-order information interactions between differen types (discrete & continuous) of variables
+1. computing higher-order information interactions between different types (discrete & continuous) of variables
 2. uncovering complex associations and causal relationships in high-dimensional data
 
 ### Project Structure
 
 ```
 |-- general-information-estimation-framework
     |-- estimate            # information estimation base on KNN, KDE, etc.
```

### Comparing `giefstat-0.0.3/giefstat.egg-info/PKG-INFO` & `giefstat-0.0.4/giefstat.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,103 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
-Description: ### general-information-estimation-framework
-        
-        ### TODOs
-        
-        1. ~~script/独立性检验/statistical_power_test.py~~
-        2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
-        3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
-        
-        ### Project Purpose
-        
-        This project aims for:
-        1. computing higher-order information interactions between differen types (discrete & continuous) of variables
-        2. uncovering complex associations and causal relationships in high-dimensional data
-        
-        ### Project Structure
-        
-        ```
-        |-- general-information-estimation-framework
-            |-- estimate            # information estimation base on KNN, KDE, etc.
-                |-- __init__.py     
-                |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
-                |-- util.py
-                |-- _univar_encoding.py     # encoding one-dimensional variable data
-                |-- gief            # general information estimation
-                    __init__.py
-                    |-- entropy     # marginal and conditional entropies
-                        |-- __init__.py
-                        |-- cond_entropy.py
-                        |-- marg_entropy.py
-                    |-- mutual_info
-                        |-- __init__.py
-                        |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
-                        |-- _ross.py    # proposed by Ross
-                        |-- mi.py       # mutual information estimation
-                        |-- cmi.py      # conditional mutual information estimation
-        
-            |-- statistical_tools
-                |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
-                |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
-                |-- time_delayed_association.py         # time delayed association detection
-        
-            |-- script
-                |-- 独立性检验
-                    |-- indep_test.py               # independence test
-                    |-- statistical_power_test.py   # statistical power test
-                |-- 条件独立性检验
-                    |-- cond_indep_test.py          # conditional independence test
-                |-- 时延关联检测
-        
-        ```
-        
-        file dependency plot：
-        
-        ```mermaid
-        flowchart LR
-        
-        subgraph estimate
-            subgraph gief
-                H-G & MI-G & CMI-G
-            end
-        
-            subgraph kde
-                MI-KDE
-            end
-        
-            subgraph other
-                coefficient --> PearsonCorr & SpearmanCorr & DistCorr
-            end
-        
-            subgraph quant_based
-                MI-Classic --> MI-cut & MI-qcut
-                MI-Darbellay
-            end
-        end
-        
-        subgraph statistical_tools
-            cal_general_assoc --> surrog_indep_test
-            surrog_indep_test --> time_delayed_assocication
-        end
-        
-        estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
-        ```
-        
-        ### References
-        
-        1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
-        2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
-        3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
-        4. https://github.com/dizcza/entropy-estimators
-        5. https://github.com/danielhomola/mifs
-        
-        
 Keywords: python,information estimation
-Platform: UNKNOWN
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+
+### general-information-estimation-framework
+
+### TODOs
+
+1. ~~script/独立性检验/statistical_power_test.py~~
+2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
+3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
+
+### Project Purpose
+
+This project aims for:
+1. computing higher-order information interactions between different types (discrete & continuous) of variables
+2. uncovering complex associations and causal relationships in high-dimensional data
+
+### Project Structure
+
+```
+|-- general-information-estimation-framework
+    |-- estimate            # information estimation base on KNN, KDE, etc.
+        |-- __init__.py     
+        |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
+        |-- util.py
+        |-- _univar_encoding.py     # encoding one-dimensional variable data
+        |-- gief            # general information estimation
+            __init__.py
+            |-- entropy     # marginal and conditional entropies
+                |-- __init__.py
+                |-- cond_entropy.py
+                |-- marg_entropy.py
+            |-- mutual_info
+                |-- __init__.py
+                |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
+                |-- _ross.py    # proposed by Ross
+                |-- mi.py       # mutual information estimation
+                |-- cmi.py      # conditional mutual information estimation
+
+    |-- statistical_tools
+        |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
+        |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
+        |-- time_delayed_association.py         # time delayed association detection
+
+    |-- script
+        |-- 独立性检验
+            |-- indep_test.py               # independence test
+            |-- statistical_power_test.py   # statistical power test
+        |-- 条件独立性检验
+            |-- cond_indep_test.py          # conditional independence test
+        |-- 时延关联检测
+
+```
+
+file dependency plot：
+
+```mermaid
+flowchart LR
+
+subgraph estimate
+    subgraph gief
+        H-G & MI-G & CMI-G
+    end
+
+    subgraph kde
+        MI-KDE
+    end
+
+    subgraph other
+        coefficient --> PearsonCorr & SpearmanCorr & DistCorr
+    end
+
+    subgraph quant_based
+        MI-Classic --> MI-cut & MI-qcut
+        MI-Darbellay
+    end
+end
+
+subgraph statistical_tools
+    cal_general_assoc --> surrog_indep_test
+    surrog_indep_test --> time_delayed_assocication
+end
+
+estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
+```
+
+### References
+
+1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+4. https://github.com/dizcza/entropy-estimators
+5. https://github.com/danielhomola/mifs
+
```

### Comparing `giefstat-0.0.3/setup.py` & `giefstat-0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 import os
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Package for information estimation, independence test, etc."
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text(encoding="utf-8")
 
 setup(
     name="giefstat",
     version=VERSION,
     author="Dreisteine",
     author_email="dreisteine@163.com",
     description=DESCRIPTION,
-    packages=find_packages(),
+    packages=find_packages(include=["gief"]),
     install_requires=["scikit-learn==0.24.0", "minepy==1.2.6"],
     keywords=["python", "information estimation"],
+    python_requires=">=3.8.0",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ulti-Dreisteine/general-information-estimation-framework",
 )
```

