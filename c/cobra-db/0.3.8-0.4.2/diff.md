# Comparing `tmp/cobra_db-0.3.8.tar.gz` & `tmp/cobra_db-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobra_db-0.3.8.tar", max compression
+gzip compressed data, was "cobra_db-0.4.2.tar", max compression
```

## Comparing `cobra_db-0.3.8.tar` & `cobra_db-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0      609 2022-08-25 09:24:06.242378 cobra_db-0.3.8/LICENSE
--rw-r--r--   0        0        0     3540 2023-05-23 08:22:03.656463 cobra_db-0.3.8/README.md
--rw-r--r--   0        0        0     1846 2023-05-28 10:55:15.766056 cobra_db-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      332 2022-08-26 14:33:49.499529 cobra_db-0.3.8/src/cobra_db/__init__.py
--rw-r--r--   0        0        0     2160 2022-08-25 10:25:47.249683 cobra_db-0.3.8/src/cobra_db/dataset_mod.py
--rw-r--r--   0        0        0     4849 2023-05-27 06:45:18.857910 cobra_db-0.3.8/src/cobra_db/deid.py
--rw-r--r--   0        0        0    19064 2023-05-27 06:45:18.858208 cobra_db-0.3.8/src/cobra_db/deid_recipe.txt
--rw-r--r--   0        0        0     2382 2023-02-09 15:28:28.969845 cobra_db-0.3.8/src/cobra_db/deid_recipe_mr.txt
--rw-r--r--   0        0        0     4423 2023-05-23 08:22:03.657525 cobra_db-0.3.8/src/cobra_db/encrypt.py
--rw-r--r--   0        0        0     4603 2022-09-22 19:04:29.847121 cobra_db-0.3.8/src/cobra_db/enums.py
--rw-r--r--   0        0        0     2266 2023-02-16 16:28:15.413447 cobra_db-0.3.8/src/cobra_db/filesystem.py
--rw-r--r--   0        0        0    17338 2023-05-23 08:22:03.658032 cobra_db-0.3.8/src/cobra_db/model.py
--rw-r--r--   0        0        0    19451 2023-05-23 08:22:03.658390 cobra_db-0.3.8/src/cobra_db/mongo_dao.py
--rw-r--r--   0        0        0        0 2022-09-20 13:32:34.744297 cobra_db-0.3.8/src/cobra_db/scripts/__init__.py
--rw-r--r--   0        0        0    10333 2023-05-23 09:13:53.676827 cobra_db-0.3.8/src/cobra_db/scripts/pseudonymize_image_metadata.py
--rw-r--r--   0        0        0    13064 2022-11-15 12:38:50.520888 cobra_db-0.3.8/src/cobra_db/scripts/stage_1_ingest_images.py
--rw-r--r--   0        0        0     2508 2022-09-22 11:58:01.231405 cobra_db-0.3.8/src/cobra_db/scripts/stage_2.py
--rw-r--r--   0        0        0     2397 2022-09-22 11:38:28.493491 cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_patients.py
--rw-r--r--   0        0        0     4709 2022-09-21 16:52:48.434815 cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_series.py
--rw-r--r--   0        0        0     5058 2023-05-23 08:22:03.658713 cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_studies.py
--rw-r--r--   0        0        0     1042 2022-09-20 13:32:34.746137 cobra_db-0.3.8/src/cobra_db/scripts/utils.py
--rw-r--r--   0        0        0      535 2022-08-25 10:25:47.234583 cobra_db-0.3.8/src/cobra_db/types.py
--rw-r--r--   0        0        0     4635 2022-10-20 08:57:54.475224 cobra_db-0.3.8/src/cobra_db/utils.py
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.3.8/PKG-INFO
+-rwxr-xr-x   0        0        0      609 2022-08-25 09:24:06.242378 cobra_db-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3540 2023-05-23 08:22:03.656463 cobra_db-0.4.2/README.md
+-rw-r--r--   0        0        0     1846 2023-06-05 12:07:47.703589 cobra_db-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      332 2022-08-26 14:33:49.499529 cobra_db-0.4.2/src/cobra_db/__init__.py
+-rw-r--r--   0        0        0     2160 2022-08-25 10:25:47.249683 cobra_db-0.4.2/src/cobra_db/dataset_mod.py
+-rw-r--r--   0        0        0     4899 2023-06-05 12:04:44.309815 cobra_db-0.4.2/src/cobra_db/deid.py
+-rw-r--r--   0        0        0    19064 2023-05-27 06:45:18.858208 cobra_db-0.4.2/src/cobra_db/deid_recipe.txt
+-rw-r--r--   0        0        0     2382 2023-02-09 15:28:28.969845 cobra_db-0.4.2/src/cobra_db/deid_recipe_mr.txt
+-rw-r--r--   0        0        0     4423 2023-05-23 08:22:03.657525 cobra_db-0.4.2/src/cobra_db/encrypt.py
+-rw-r--r--   0        0        0     4603 2022-09-22 19:04:29.847121 cobra_db-0.4.2/src/cobra_db/enums.py
+-rw-r--r--   0        0        0     2266 2023-02-16 16:28:15.413447 cobra_db-0.4.2/src/cobra_db/filesystem.py
+-rw-r--r--   0        0        0    18282 2023-06-05 12:04:44.310223 cobra_db-0.4.2/src/cobra_db/model.py
+-rw-r--r--   0        0        0    19451 2023-05-23 08:22:03.658390 cobra_db-0.4.2/src/cobra_db/mongo_dao.py
+-rw-r--r--   0        0        0        0 2022-09-20 13:32:34.744297 cobra_db-0.4.2/src/cobra_db/scripts/__init__.py
+-rw-r--r--   0        0        0    10338 2023-06-05 12:04:44.310757 cobra_db-0.4.2/src/cobra_db/scripts/pseudonymize_image_metadata.py
+-rw-r--r--   0        0        0    13064 2022-11-15 12:38:50.520888 cobra_db-0.4.2/src/cobra_db/scripts/stage_1_ingest_images.py
+-rw-r--r--   0        0        0     2508 2022-09-22 11:58:01.231405 cobra_db-0.4.2/src/cobra_db/scripts/stage_2.py
+-rw-r--r--   0        0        0     2397 2022-09-22 11:38:28.493491 cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_patients.py
+-rw-r--r--   0        0        0     4709 2022-09-21 16:52:48.434815 cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_series.py
+-rw-r--r--   0        0        0     5058 2023-05-23 08:22:03.658713 cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_studies.py
+-rw-r--r--   0        0        0     1042 2022-09-20 13:32:34.746137 cobra_db-0.4.2/src/cobra_db/scripts/utils.py
+-rw-r--r--   0        0        0      535 2022-08-25 10:25:47.234583 cobra_db-0.4.2/src/cobra_db/types.py
+-rw-r--r--   0        0        0     4635 2022-10-20 08:57:54.475224 cobra_db-0.4.2/src/cobra_db/utils.py
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.4.2/PKG-INFO
```

### Comparing `cobra_db-0.3.8/LICENSE` & `cobra_db-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/README.md` & `cobra_db-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/pyproject.toml` & `cobra_db-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cobra_db"
-version = "0.3.8"
+version = "0.4.2"
 description = "COnsolidated BReast cancer Analysis DataBase"
 authors = ["Fernando Cossio", "Apostolia Tsirikoglou", "Haiko Schurz", "Hui Li", "Fredrik Strand"]
 license = "Apache License 2.0"
 readme = "README.md"
 include = ["src/cobra_db/deid_recipe.txt"]
 
 [tool.poetry.dependencies]
```

### Comparing `cobra_db-0.3.8/src/cobra_db/dataset_mod.py` & `cobra_db-0.4.2/src/cobra_db/dataset_mod.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/deid.py` & `cobra_db-0.4.2/src/cobra_db/deid.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,23 +94,24 @@
         return interval * round(value / interval)
 
     @staticmethod
     def _round_AS_to_nearest_5y(item, value, field, dicom):
         """Rounds age(AS) field to 5 year intervals in the deid framework"""
         value = field.element.value
         # if age is empty, try to calculate it from the StudyDate and PatientBirthDate
-        if value == '' or value == None:
+        if value == "" or value is None:
             try:
-                study_date = dicom.get('StudyDate')
-                study_date = parse_DA_TM_as_datetime(DA=study_date, TM='000000')
-                birth_date = dicom.get('PatientBirthDate')
-                birth_date = parse_DA_TM_as_datetime(DA=birth_date, TM='000000')
-                age = (study_date - birth_date).days/365
-            except:
-                return ''
+                study_date = dicom.get("StudyDate")
+                study_date = parse_DA_TM_as_datetime(DA=study_date, TM="000000")
+                birth_date = dicom.get("PatientBirthDate")
+                birth_date = parse_DA_TM_as_datetime(DA=birth_date, TM="000000")
+                age = (study_date - birth_date).days / 365
+            except Exception as e:
+                logging.error(e)
+                return ""
         else:
             age = parse_AS_as_int(field.element.value)
         return f"{Deider._round_to_nearest(age, 5):03d}Y"
 
     @staticmethod
     def _round_DS_to_nearest_5(item, value, field, dicom):
         """Rounds age(AS) field to 5 year intervals in the deid framework"""
```

### Comparing `cobra_db-0.3.8/src/cobra_db/deid_recipe.txt` & `cobra_db-0.4.2/src/cobra_db/deid_recipe.txt`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/deid_recipe_mr.txt` & `cobra_db-0.4.2/src/cobra_db/deid_recipe_mr.txt`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/encrypt.py` & `cobra_db-0.4.2/src/cobra_db/encrypt.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/enums.py` & `cobra_db-0.4.2/src/cobra_db/enums.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/filesystem.py` & `cobra_db-0.4.2/src/cobra_db/filesystem.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/model.py` & `cobra_db-0.4.2/src/cobra_db/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from copy import copy
 from dataclasses import dataclass, fields, is_dataclass
 from datetime import datetime, timezone
-from typing import Callable, List, Tuple, Type, Union
+from typing import Callable, List, Literal, Tuple, Type, Union
 
 import numpy as np
 import pydicom
 from bson import ObjectId
 from pydicom.dataset import Dataset
 
 from cobra_db import __version__
@@ -482,7 +482,39 @@
     def get_file_size(self, mount_paths) -> int:
         """Get the size in bytes of the file"""
         filepath = self.get_local_filepath(mount_paths)
         return os.path.getsize(filepath)
 
     def __repr__(self):
         return super().__repr__()
+
+
+@dataclass
+class Annotation(Entity):
+    """
+    Abstract class for any annotation that is stored in cobra_db. Should be subclassed
+    """
+
+    annotation_type: List[
+        Literal["text", "semantic_segmentation", "binary", "categorical"]
+    ]
+    annotator_email: str
+    date: datetime  # annotation date
+    possible_labels: List[
+        str
+    ]  # List of all possible labels example [mass, non-mass, ...]
+    file_format: str  # Name of the extension of the file. jpeg, png, npz, etc.
+    aggregation_level: Literal["patient", "study", "series", "image"]
+    # For example the SOPInstanceUID of the image, StudyInstanceID of the study, etc.
+    referenced_entity_uid: str
+    patient_anon_id: str
+    study_date: datetime
+    file_source: FileSource  # file/folder of the annotation
+    project_name: str
+
+
+@dataclass
+class Annotator(Entity):
+    email: str
+    specialization: str
+    first_name: str
+    last_name: str
```

### Comparing `cobra_db-0.3.8/src/cobra_db/mongo_dao.py` & `cobra_db-0.4.2/src/cobra_db/mongo_dao.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/scripts/pseudonymize_image_metadata.py` & `cobra_db-0.4.2/src/cobra_db/scripts/pseudonymize_image_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import os
 import sys
 from argparse import ArgumentParser, Namespace
 from multiprocessing import Pool
+from time import sleep
 from typing import List, Union
 
 import pydicom
 from bson import ObjectId
 from pyaml_env import parse_config
 from pydicom.errors import BytesLengthException
 from pymongo.errors import DuplicateKeyError
@@ -15,16 +16,14 @@
 from cobra_db.dataset_mod import DatasetMod
 from cobra_db.deid import Deider, base_recipe_path, mr_recipe_path
 from cobra_db.filesystem import get_instance_path
 from cobra_db.model import FileSource, ImageMetadata
 from cobra_db.mongo_dao import Connector, ImageMetadataDao
 from cobra_db.scripts.utils import add_args_to_iterable, batcher
 
-from time import sleep
-
 
 def parse_arguments(raw_args: List[str]) -> str:
     """Parse the arguments for the pseudonymization process
 
     :param raw_args: arguments from sys.argv[1:]
     :return: a namespace with the required cfg
     """
@@ -167,15 +166,15 @@
         pydicom.write_file(dst_filepath, deid_ds)
     except ValueError as e:
         logging.error(f"{e}")
     except OSError as e:
         print(f"{e} - {dst_filepath}")
         if retries > 0:
             sleep(2)
-            print(f"Retrying now, {r} retries left - {dst_filepath}")
+            print(f"Retrying now, {retries} retries left - {dst_filepath}")
             r = retries - 1
             return process_im_meta(im_meta_dict, cfg, src_im_dao, dst_im_dao, r)
         print(
             f"Unknown OS error, could not fix by retrying, will not write - {dst_filepath}"
         )
 
     # the _id of the dataset is stored with the same database _id so that a super user
```

### Comparing `cobra_db-0.3.8/src/cobra_db/scripts/stage_1_ingest_images.py` & `cobra_db-0.4.2/src/cobra_db/scripts/stage_1_ingest_images.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/scripts/stage_2.py` & `cobra_db-0.4.2/src/cobra_db/scripts/stage_2.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_patients.py` & `cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_patients.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_series.py` & `cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_series.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_studies.py` & `cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_studies.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/scripts/utils.py` & `cobra_db-0.4.2/src/cobra_db/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/types.py` & `cobra_db-0.4.2/src/cobra_db/types.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/src/cobra_db/utils.py` & `cobra_db-0.4.2/src/cobra_db/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.3.8/PKG-INFO` & `cobra_db-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobra-db
-Version: 0.3.8
+Version: 0.4.2
 Summary: COnsolidated BReast cancer Analysis DataBase
 License: Apache-2.0
 Author: Fernando Cossio
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

