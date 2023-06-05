# Comparing `tmp/acryl-datahub-classify-0.0.6.tar.gz` & `tmp/acryl-datahub-classify-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryl-datahub-classify-0.0.6.tar", last modified: Thu Mar  9 22:57:27 2023, max compression
+gzip compressed data, was "acryl-datahub-classify-0.0.7.tar", last modified: Mon Jun  5 19:21:29 2023, max compression
```

## Comparing `acryl-datahub-classify-0.0.6.tar` & `acryl-datahub-classify-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:57:27.587117 acryl-datahub-classify-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-03-09 22:57:27.587117 acryl-datahub-classify-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-09 22:57:27.587117 acryl-datahub-classify-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:57:27.579116 acryl-datahub-classify-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:57:27.583116 acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-03-09 22:57:27.000000 acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-09 22:57:27.000000 acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 22:57:27.000000 acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-09 22:57:27.000000 acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 22:57:27.000000 acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:57:27.587117 acryl-datahub-classify-0.0.6/src/datahub_classify/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-09 22:57:21.000000 acryl-datahub-classify-0.0.6/src/datahub_classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/src/datahub_classify/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/src/datahub_classify/helper_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26988 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/src/datahub_classify/infotype_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/src/datahub_classify/infotype_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/src/datahub_classify/infotype_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/src/datahub_classify/reference_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:57:27.587117 acryl-datahub-classify-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-03-09 22:19:33.000000 acryl-datahub-classify-0.0.6/tests/test_infotype_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/src/datahub_classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 19:21:22.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/helper_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28228 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/reference_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/tests/test_custom_infotype_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/tests/test_infotype_predictor.py
```

### Comparing `acryl-datahub-classify-0.0.6/PKG-INFO` & `acryl-datahub-classify-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-datahub-classify
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to predict info types for DataHub
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/
 Project-URL: Source, https://github.com/acryldata/datahub-classify
 Project-URL: Changelog, https://github.com/acryldata/datahub-classify/releases
 Classifier: Development Status :: 5 - Production/Stable
@@ -121,14 +121,15 @@
     'Values': 0.6,
     'Datatype': 0.3
 }
 ```
 
 ## Supported Infotypes
 
+Below Infotypes are supported out of the box.
 1. Age
 2. Gender
 3. Person Name / Full Name
 4. Email Address
 5. Phone Number
 6. Street Address
 7. Credit-Debit Card Number
@@ -136,14 +137,16 @@
 9. Vehicle Identification Number
 10. US Social Security Number
 11. Ipv4 Address
 12. Ipv6 Address
 13. Swift Code
 14. US Driving License Number
 
+Regex based custom infotypes are supported. Specify custom infotype configuration in format mentioned [here](#infotype-configuration).
+
 ## Assumptions
 
 - If value prediction factor weight is non-zero (indicating values should be used for infotype inspection) then a minimum 50 non-null column values should be present.
 
 ## Development
 
 ### Set up your Python environment
```

### Comparing `acryl-datahub-classify-0.0.6/README.md` & `acryl-datahub-classify-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     'Values': 0.6,
     'Datatype': 0.3
 }
 ```
 
 ## Supported Infotypes
 
+Below Infotypes are supported out of the box.
 1. Age
 2. Gender
 3. Person Name / Full Name
 4. Email Address
 5. Phone Number
 6. Street Address
 7. Credit-Debit Card Number
@@ -106,14 +107,16 @@
 9. Vehicle Identification Number
 10. US Social Security Number
 11. Ipv4 Address
 12. Ipv6 Address
 13. Swift Code
 14. US Driving License Number
 
+Regex based custom infotypes are supported. Specify custom infotype configuration in format mentioned [here](#infotype-configuration).
+
 ## Assumptions
 
 - If value prediction factor weight is non-zero (indicating values should be used for infotype inspection) then a minimum 50 non-null column values should be present.
 
 ## Development
 
 ### Set up your Python environment
```

### Comparing `acryl-datahub-classify-0.0.6/setup.cfg` & `acryl-datahub-classify-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.6/setup.py` & `acryl-datahub-classify-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/PKG-INFO` & `acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-datahub-classify
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to predict info types for DataHub
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/
 Project-URL: Source, https://github.com/acryldata/datahub-classify
 Project-URL: Changelog, https://github.com/acryldata/datahub-classify/releases
 Classifier: Development Status :: 5 - Production/Stable
@@ -121,14 +121,15 @@
     'Values': 0.6,
     'Datatype': 0.3
 }
 ```
 
 ## Supported Infotypes
 
+Below Infotypes are supported out of the box.
 1. Age
 2. Gender
 3. Person Name / Full Name
 4. Email Address
 5. Phone Number
 6. Street Address
 7. Credit-Debit Card Number
@@ -136,14 +137,16 @@
 9. Vehicle Identification Number
 10. US Social Security Number
 11. Ipv4 Address
 12. Ipv6 Address
 13. Swift Code
 14. US Driving License Number
 
+Regex based custom infotypes are supported. Specify custom infotype configuration in format mentioned [here](#infotype-configuration).
+
 ## Assumptions
 
 - If value prediction factor weight is non-zero (indicating values should be used for infotype inspection) then a minimum 50 non-null column values should be present.
 
 ## Development
 
 ### Set up your Python environment
```

### Comparing `acryl-datahub-classify-0.0.6/src/acryl_datahub_classify.egg-info/SOURCES.txt` & `acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 src/datahub_classify/__init__.py
 src/datahub_classify/constants.py
 src/datahub_classify/helper_classes.py
 src/datahub_classify/infotype_helper.py
 src/datahub_classify/infotype_predictor.py
 src/datahub_classify/infotype_utils.py
 src/datahub_classify/reference_input.py
+tests/test_custom_infotype_predictor.py
 tests/test_infotype_predictor.py
```

### Comparing `acryl-datahub-classify-0.0.6/src/datahub_classify/helper_classes.py` & `acryl-datahub-classify-0.0.7/src/datahub_classify/helper_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional
 
 
 @dataclass
+class DebugInfo:
+    name: Optional[float] = None
+    description: Optional[float] = None
+    datatype: Optional[float] = None
+    values: Optional[float] = None
+
+
+@dataclass
 class InfotypeProposal:
     infotype: str
     confidence_level: float
-    debug_info: Dict[str, Any]
+    debug_info: DebugInfo
 
 
 @dataclass
 class Metadata:
     meta_info: Dict[str, Any]
     name: str = field(init=False)
     description: str = field(init=False)
@@ -25,15 +33,7 @@
 
 
 @dataclass
 class ColumnInfo:
     metadata: Metadata
     values: List[Any]
     infotype_proposals: Optional[List[InfotypeProposal]] = None
-
-
-@dataclass
-class DebugInfo:
-    name: Optional[float] = None
-    description: Optional[float] = None
-    datatype: Optional[float] = None
-    values: Optional[float] = None
```

### Comparing `acryl-datahub-classify-0.0.6/src/datahub_classify/infotype_helper.py` & `acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,43 @@
         debug_info.values = values_score
 
     debug_info = compute_name_description_dtype_score(metadata, config, debug_info)
     confidence_level = compute_overall_confidence(debug_info, config)
     return confidence_level, debug_info
 
 
+def inspect_for_custom_infotype(
+    metadata: Metadata, values: List[Any], config: Dict[str, Dict]
+) -> Tuple[float, DebugInfo]:
+    prediction_factors_weights = config[PREDICTION_FACTORS_AND_WEIGHTS]
+    debug_info = DebugInfo()
+    # Value Logic
+    if prediction_factors_weights.get(VALUES, 0) > 0:
+        values_score = 0.0
+        try:
+            if config[VALUES][PREDICTION_TYPE] == "regex":
+                values_score = match_regex_for_values(values, config[VALUES][REGEX])
+            elif config[VALUES][PREDICTION_TYPE] == "library":
+                raise Exception(
+                    "Currently prediction type 'library' is not supported for custom infotype"
+                )
+            else:
+                raise Exception(
+                    f"Inappropriate Prediction type {config[VALUES][PREDICTION_TYPE]}"
+                )
+        except Exception as e:
+            logger.error(f"Column {metadata.name} failed due to {e}")
+        values_score = np.round(values_score, 2)
+        debug_info.values = values_score
+
+    debug_info = compute_name_description_dtype_score(metadata, config, debug_info)
+    confidence_level = compute_overall_confidence(debug_info, config)
+    return confidence_level, debug_info
+
+
 def inspect_for_street_address(
     metadata: Metadata, values: List[Any], config: Dict[str, Dict]
 ) -> Tuple[float, DebugInfo]:  # noqa: C901
     prediction_factors_weights = config[PREDICTION_FACTORS_AND_WEIGHTS]
     debug_info = DebugInfo()
 
     # Values logic
```

### Comparing `acryl-datahub-classify-0.0.6/src/datahub_classify/infotype_predictor.py` & `acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     if not infotypes:
         infotypes = list(global_config.keys())
     for infotype in infotypes:
         if infotype not in global_config.keys():
             logger.warning(f"Configuration is not available for infotype - {infotype}")
         else:
             fn_name = f"inspect_for_{infotype.lower()}"
-            infotype_function_map[infotype] = module_fn_dict[fn_name]
+            if fn_name in module_fn_dict:
+                infotype_function_map[infotype] = module_fn_dict[fn_name]
+            else:
+                fn_name = "inspect_for_custom_infotype"
+                infotype_function_map[infotype] = module_fn_dict[fn_name]
     return infotype_function_map
 
 
 def predict_infotypes(
     column_infos: List[ColumnInfo],
     confidence_level_threshold: float,
     global_config: Dict[str, Dict],
@@ -71,15 +75,15 @@
                 else:
                     basic_checks_failed_columns.append(
                         (column_info.metadata.name, column_info.metadata.dataset_name)
                     )
 
             except Exception as e:
                 # traceback.print_exc()
-                logger.warning(f"Failed to extract info type due to {e}")
+                logger.warning(f"Failed to extract info type {infotype} due to {e}")
         if len(proposal_list) > 0:
             num_cols_with_infotype_assigned += 1
         column_info.infotype_proposals = proposal_list
     if len(basic_checks_failed_columns) > 0:
         basic_checks_failed_columns_set = set(basic_checks_failed_columns)
         logger.warning(
             f"Infotype not extracted due to basic checks failure for {len(basic_checks_failed_columns_set)} out of {len(column_infos)} columns.Check DEBUG logs for details"
```

### Comparing `acryl-datahub-classify-0.0.6/src/datahub_classify/infotype_utils.py` & `acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_utils.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.6/src/datahub_classify/reference_input.py` & `acryl-datahub-classify-0.0.7/src/datahub_classify/reference_input.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.6/tests/test_infotype_predictor.py` & `acryl-datahub-classify-0.0.7/tests/test_infotype_predictor.py`

 * *Files identical despite different names*

