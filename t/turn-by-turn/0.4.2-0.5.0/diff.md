# Comparing `tmp/turn_by_turn-0.4.2.tar.gz` & `tmp/turn_by_turn-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/turn_by_turn/turn_by_turn/dist/tmp2bb69l_c/turn_by_turn-0.4.2.tar", last modified: Wed Sep 21 12:36:20 2022, max compression
+gzip compressed data, was "turn_by_turn-0.5.0.tar", last modified: Mon Jun  5 13:57:43 2023, max compression
```

## Comparing `turn_by_turn-0.4.2.tar` & `turn_by_turn-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4205 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/turn_by_turn/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6411 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/ascii.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/esrf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5105 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/iota.py
--rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/lhc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7213 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/ptc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/sps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/trackone.py
--rw-r--r--   0 runner    (1001) docker     (121)     6334 2022-09-21 12:36:05.000000 turn_by_turn-0.4.2/turn_by_turn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/turn_by_turn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4205 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/turn_by_turn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/turn_by_turn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/turn_by_turn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/turn_by_turn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-21 12:36:20.000000 turn_by_turn-0.4.2/turn_by_turn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:43.341057 turn_by_turn-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-05 13:57:43.341057 turn_by_turn-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:57:43.341057 turn_by_turn-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:43.337057 turn_by_turn-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/tests/test_iota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/tests/test_lhc_and_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/tests/test_ptc_trackone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/tests/test_sps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:43.341057 turn_by_turn-0.5.0/turn_by_turn/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/esrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/iota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/lhc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/ptc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/sps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/trackone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-05 13:57:24.000000 turn_by_turn-0.5.0/turn_by_turn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:43.341057 turn_by_turn-0.5.0/turn_by_turn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-05 13:57:43.000000 turn_by_turn-0.5.0/turn_by_turn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 13:57:43.000000 turn_by_turn-0.5.0/turn_by_turn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:57:43.000000 turn_by_turn-0.5.0/turn_by_turn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-05 13:57:43.000000 turn_by_turn-0.5.0/turn_by_turn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 13:57:43.000000 turn_by_turn-0.5.0/turn_by_turn.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `turn_by_turn-0.4.2/LICENSE` & `turn_by_turn-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/PKG-INFO` & `turn_by_turn-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turn_by_turn
-Version: 0.4.2
+Version: 0.5.0
 Summary: Read and write turn-by-turn measurement files from different particle accelerator formats.
 Home-page: https://github.com/pylhc/turn_by_turn
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `turn_by_turn-0.4.2/README.md` & `turn_by_turn-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/setup.py` & `turn_by_turn-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/__init__.py` & `turn_by_turn-0.5.0/turn_by_turn/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Exposes TbtData, read_tbt and write_tbt directly in the package's namespace."""
 from .io import read_tbt, write_tbt
 from .structures import TbtData, TransverseData
 
 __title__ = "turn_by_turn"
 __description__ = "Read and write turn-by-turn measurement files from different particle accelerator formats."
 __url__ = "https://github.com/pylhc/turn_by_turn"
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 __author__ = "pylhc"
 __author_email__ = "pylhc@github.com"
 __license__ = "MIT"
 
 # aliases
 write = write_tbt
 read = read_tbt
```

### Comparing `turn_by_turn-0.4.2/turn_by_turn/ascii.py` & `turn_by_turn-0.5.0/turn_by_turn/ascii.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/errors.py` & `turn_by_turn-0.5.0/turn_by_turn/errors.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/esrf.py` & `turn_by_turn-0.5.0/turn_by_turn/esrf.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/io.py` & `turn_by_turn-0.5.0/turn_by_turn/io.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/iota.py` & `turn_by_turn-0.5.0/turn_by_turn/iota.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/lhc.py` & `turn_by_turn-0.5.0/turn_by_turn/lhc.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/ptc.py` & `turn_by_turn-0.5.0/turn_by_turn/ptc.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/sps.py` & `turn_by_turn-0.5.0/turn_by_turn/sps.py`

 * *Files identical despite different names*

### Comparing `turn_by_turn-0.4.2/turn_by_turn/structures.py` & `turn_by_turn-0.5.0/turn_by_turn/structures.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,46 +2,77 @@
 Structures
 ----------
 
 Data structures to be used in ``turn_by_turn`` to store turn-by-turn measurement data.
 """
 from dataclasses import dataclass, field, fields
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import List, Sequence, Union
 
 import pandas as pd
 from dateutil import tz
 
 
 @dataclass
 class TransverseData:
     """
     Object holding measured turn-by-turn data for both transverse planes in the form of pandas DataFrames.
     """
 
     X: pd.DataFrame  # horizontal data
     Y: pd.DataFrame  # vertical data
 
-    def fieldnames(self):
-        return (f.name for f in fields(self))
+    @classmethod
+    def fieldnames(self) -> List[str]:
+        """Return a list of the fields of this dataclass."""
+        return list(f.name for f in fields(self))
 
     def __getitem__(self, item):  # to access X and Y like one would with a dictionary
         if item not in self.fieldnames():
             raise KeyError(f"'{item}' is not in the fields of a {self.__class__.__name__} object.")
         return getattr(self, item)
 
 
 @dataclass
+class TrackingData:
+    """
+    Object holding multidimensional turn-by-turn simulation data in the form of pandas DataFrames.
+    """
+
+    X: pd.DataFrame  # horizontal data
+    PX: pd.DataFrame  # horizontal momentum data
+    Y: pd.DataFrame  # vertical data
+    PY: pd.DataFrame  # vertical momentum data
+    T: pd.DataFrame  # longitudinal data
+    PT: pd.DataFrame  # longitudinal momentum data
+    S: pd.DataFrame  # longitudinal position data
+    E: pd.DataFrame  # energy data
+
+    @classmethod
+    def fieldnames(self) -> List[str]:
+        """Return a list of the fields of this dataclass."""
+        return list(f.name for f in fields(self))
+
+    def __getitem__(self, item):  # to access fields like one would with a dictionary
+        if item not in self.fieldnames():
+            raise KeyError(f"'{item}' is not in the fields of a {self.__class__.__name__} object.")
+        return getattr(self, item)
+
+
+DataType = Union[TransverseData, TrackingData]
+
+
+@dataclass
 class TbtData:
     """
     Object holding a representation of a Turn-by-Turn data measurement. The date of the measurement,
     the transverse data, number of turns and bunches as well as the bunch IDs are encapsulated in this object.
     """
 
-    matrices: Sequence[TransverseData]  # each entry corresponds to a bunch
+    matrices: Sequence[DataType]  # each entry corresponds to a bunch
     date: datetime = None  # will default in post_init
     bunch_ids: List[int] = None  # will default in post_init
     nturns: int = None
     nbunches: int = field(init=False)
 
     def __post_init__(self):
         self.nbunches = len(self.matrices)
```

### Comparing `turn_by_turn-0.4.2/turn_by_turn/trackone.py` & `turn_by_turn-0.5.0/turn_by_turn/trackone.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,34 +9,42 @@
 """
 import logging
 from pathlib import Path
 from typing import Dict, Tuple, Union
 
 import numpy as np
 
-from turn_by_turn.structures import TbtData
+from turn_by_turn.structures import TbtData, TrackingData, TransverseData
 from turn_by_turn.utils import numpy_to_tbt
 
 LOGGER = logging.getLogger()
 
 
-def read_tbt(file_path: Union[str, Path]) -> TbtData:
+def read_tbt(file_path: Union[str, Path], is_tracking_data: bool = False) -> TbtData:
     """
     Reads turn-by-turn data from the ``MAD-X`` **trackone** format file.
 
     Args:
         file_path (Union[str, Path]): path to the turn-by-turn measurement file.
+        is_tracking_data (bool): if ``True``, all (``X``, ``PX``, ``Y``, ``PY``,
+            ``T``, ``PT``, ``S``, ``E``) fields are expected in the file as it
+            is considered a full tracking simulation output. Those are then read
+            into ``TrackingData`` objects. Defaults to ``False``.
 
     Returns:
         A ``TbTData`` object with the loaded data.
     """
     nturns, npart = get_trackone_stats(file_path)
     names, matrix = get_structure_from_trackone(nturns, npart, file_path)
-    # matrix[0, 2] contains just (x, y) samples.
-    return numpy_to_tbt(names, matrix[[0, 2]])
+    if is_tracking_data:
+        # Converts full tracking output to TbTData.
+        return numpy_to_tbt(names, matrix, datatype=TrackingData)
+    else:
+        # matrix[0, 2] contains just (x, y) samples.
+        return numpy_to_tbt(names, matrix[[0, 2]], datatype=TransverseData)
 
 
 def get_trackone_stats(file_path: Union[str, Path], write_out: bool = False) -> Tuple[int, int]:
     """
     Determines the number of particles and turns in the matrices from the provided ``MAD-X``
     **trackone** file.
```

### Comparing `turn_by_turn-0.4.2/turn_by_turn/utils.py` & `turn_by_turn-0.5.0/turn_by_turn/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Utils
 -----
 
 Utility functions for convenience operations on turn-by-turn data objects in this package.
 """
 import logging
-
-from typing import Dict, Sequence
+from typing import Sequence, Union
 
 import numpy as np
 import pandas as pd
 
-from turn_by_turn.constants import PLANES, PLANE_TO_NUM
+from turn_by_turn.constants import PLANE_TO_NUM, PLANES
 from turn_by_turn.errors import ExclusiveArgumentsError
-from turn_by_turn.structures import TbtData, TransverseData
+from turn_by_turn.structures import DataType, TbtData, TransverseData
 
 LOGGER = logging.getLogger(__name__)
 
 
 def generate_average_tbtdata(tbtdata: TbtData) -> TbtData:
     """
     Takes a ``TbtData`` object and returns another containing the averaged matrices over all
@@ -27,27 +26,26 @@
         tbtdata (TbtData): entry TbtData object from measurements.
 
     Returns:
         A new TbtData object with the averaged matrices.
     """
     data = tbtdata.matrices
     bpm_names = data[0].X.index
+    datatype = tbtdata.matrices[0].__class__
 
     new_matrices = [
-        TransverseData(
-            X=pd.DataFrame(
-                index=bpm_names,
-                data=get_averaged_data(bpm_names, data, "X", tbtdata.nturns),
-                dtype=float,
-            ),
-            Y=pd.DataFrame(
-                index=bpm_names,
-                data=get_averaged_data(bpm_names, data, "Y", tbtdata.nturns),
-                dtype=float,
-            ),
+        datatype(  # datatype is directly the class to load data into
+            **{  # for each field in the datatype, load the corresponding matrix
+                field: pd.DataFrame(
+                    index=bpm_names,
+                    data=get_averaged_data(bpm_names, data, field, tbtdata.nturns),
+                    dtype=float,
+                )
+                for field in datatype.fieldnames()
+            }
         )
     ]
     return TbtData(new_matrices, tbtdata.date, [1], tbtdata.nturns)
 
 
 def get_averaged_data(
     bpm_names: Sequence[str], matrices: Sequence[TransverseData], plane: str, turns: int
@@ -147,32 +145,38 @@
         ) for m in data.matrices],
         date=data.date,
         bunch_ids=data.bunch_ids,
         nturns=data.nturns,
     )
 
 
-def numpy_to_tbt(names: np.ndarray, matrix: np.ndarray) -> TbtData:
+def numpy_to_tbt(names: np.ndarray, matrix: np.ndarray, datatype: DataType = TransverseData) -> TbtData:
     """
     Converts turn by turn matrices and names into a ``TbTData`` object.
 
     Args:
         names (np.ndarray): Numpy array of BPM names.
         matrix (np.ndarray): 4D Numpy array [quantity, BPM, particle/bunch No., turn No.]
             quantities in order [x, y].
+        datatype (DataType): The type of data to be converted to in the matrices. Either
+            ``TransverseData`` (which implies reading ``X`` and ``Y`` fields) or
+            ``TrackingData`` (which implies reading all 8 fields). Defaults to 
+            ``TransverseData``.
 
     Returns:
         A ``TbtData`` object loaded with the matrices in the provided numpy arrays.
     """
     # get list of TbTFile from 4D matrix ...
     _, _, nbunches, nturns = matrix.shape
     matrices = []
     indices = []
-    for index in range(nbunches):
+    for idx_bunch in range(nbunches):
         matrices.append(
-            TransverseData(
-                X=pd.DataFrame(index=names, data=matrix[0, :, index, :]),
-                Y=pd.DataFrame(index=names, data=matrix[1, :, index, :]),
+            datatype(  # datatype is directly the class to load data into (TransverseData or TrackingData)
+                **{  # for each field in the datatype, load the corresponding matrix
+                    field: pd.DataFrame(index=names, data=matrix[idx_field, :, idx_bunch, :])
+                    for idx_field, field in enumerate(datatype.fieldnames())
+                }
             )
         )
-        indices.append(index)
+        indices.append(idx_bunch)
     return TbtData(matrices=matrices, bunch_ids=indices, nturns=nturns)
```

### Comparing `turn_by_turn-0.4.2/turn_by_turn.egg-info/PKG-INFO` & `turn_by_turn-0.5.0/turn_by_turn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turn-by-turn
-Version: 0.4.2
+Version: 0.5.0
 Summary: Read and write turn-by-turn measurement files from different particle accelerator formats.
 Home-page: https://github.com/pylhc/turn_by_turn
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

