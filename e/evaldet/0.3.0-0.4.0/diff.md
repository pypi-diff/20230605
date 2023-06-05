# Comparing `tmp/evaldet-0.3.0.tar.gz` & `tmp/evaldet-0.4.0.tar.gz`

## Comparing `evaldet-0.3.0.tar` & `evaldet-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,36 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 evaldet-0.3.0/.flake8
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 evaldet-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 evaldet-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 evaldet-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 evaldet-0.3.0/Makefile
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 evaldet-0.3.0/env.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/dist.py
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/metrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/py.typed
--rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/tracks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/mot_metrics/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/mot_metrics/alta.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/mot_metrics/base.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/mot_metrics/clearmot.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/mot_metrics/hota.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/mot_metrics/identity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/utils/__init__.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/utils/preprocess.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/utils/sparse.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 evaldet-0.3.0/src/evaldet/utils/timer.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 evaldet-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 evaldet-0.3.0/LICENSE
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 evaldet-0.3.0/README.md
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 evaldet-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 evaldet-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 evaldet-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 evaldet-0.4.0/Makefile
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 evaldet-0.4.0/env.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/Makefile
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/make.bat
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/requirements.txt
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/conf.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/index.rst
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/start.rst
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/guide/index.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/reference/dist.rst
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/reference/index.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/reference/metrics.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 evaldet-0.4.0/old_docs/source/reference/tracks.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/__init__.py
+-rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/detections.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/dist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/py.typed
+-rw-r--r--   0        0        0    35064 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/tracks.py
+-rw-r--r--   0        0        0    21022 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/det/coco.py
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/det/utils.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/mot/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/mot/alta.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/mot/clearmot.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/mot/hota.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/mot/identity.py
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/mot/motmetrics.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/mot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/utils/__init__.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/utils/prec_recall.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 evaldet-0.4.0/src/evaldet/utils/timer.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 evaldet-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 evaldet-0.4.0/LICENSE
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 evaldet-0.4.0/README.md
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 evaldet-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 evaldet-0.4.0/PKG-INFO
```

### Comparing `evaldet-0.3.0/CHANGELOG.md` & `evaldet-0.4.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## 0.4.0 - 2023-06-06
+
+* Drop support for Python 3.8, add support for Python 3.11 (#36)
+* Add module for computing COCO object detection metrics (#36)
+* Add Detections class to represent object detections, and load from and save to COCO and parquet formats (#36)
+* Refactor the individual MOT metrics from classes to functions (#36)
+
 ## [0.3.0] - 2022-12-02
 
 ### Added
 
 * Support for reading/writing to parquet formats ([#30](https://github.com/tadejsv/EvalDeT/pull/30))
 
 ### Changed
```

### Comparing `evaldet-0.3.0/src/evaldet/metrics.py` & `evaldet-0.4.0/src/evaldet/mot/motmetrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import logging
 import typing as t
 
 import numpy as np
+import numpy.typing as npt
 
-from .dist import iou_dist
-from .mot_metrics.clearmot import CLEARMOTMetrics, CLEARMOTResults
-from .mot_metrics.hota import HOTAMetrics, HOTAResults
-from .mot_metrics.identity import IDMetrics, IDResults
-from .tracks import Tracks
-from .utils import timer
+from evaldet.dist import iou_dist
+from evaldet.tracks import Tracks
+from evaldet.utils import timer
+
+from .clearmot import CLEARMOTResults, calculate_clearmot_metrics
+from .hota import HOTAResults, calculate_hota_metrics
+from .identity import IDResults, calculate_id_metrics
 
 
 class MOTMetricsResults(t.TypedDict):
     """The result of the MOT metric computtion."""
 
     clearmot: t.Optional[CLEARMOTResults]
     id: t.Optional[IDResults]
     hota: t.Optional[HOTAResults]
 
 
-class MOTMetrics(CLEARMOTMetrics, IDMetrics, HOTAMetrics):
+class MOTMetrics:
     """The class for computing MOT metrics.
 
     To compute the metrics, use the ``compute`` method of this class, it will compute
     all the required MOT metrics.
 
     The reason for a single entrypoint for MOT computation is so that metrics can
     efficiently share pre-computed IoU distances.
     """
 
-    _ious: t.List[np.ndarray]
-    _ious_dict: t.Dict[int, int]
+    _ious_dict: dict[int, npt.NDArray[np.float32]]
 
     def __init__(
         self, clearmot_dist_threshold: float = 0.5, id_dist_threshold: float = 0.5
     ) -> None:
         """Initialize the object.
 
         Args:
@@ -46,30 +47,14 @@
                 ID metrics - used to determine whether to match two objects.
         """
         self._clearmot_dist_threshold = clearmot_dist_threshold
         self._id_dist_threshold = id_dist_threshold
 
         self._logger = logging.getLogger(self.__class__.__name__)
 
-    def _precompute_iou(self, ground_truth: Tracks, hypotheses: Tracks) -> None:
-        all_frames = sorted(set(ground_truth.frames).intersection(hypotheses.frames))
-
-        self._ious = []
-        self._ious_dict = {}
-        for ind, frame in enumerate(all_frames):
-            ious_f = iou_dist(
-                ground_truth[frame].detections, hypotheses[frame].detections
-            )
-            self._ious.append(ious_f)
-            self._ious_dict[frame] = ind
-
-    def _get_iou_frame(self, frame: int) -> np.ndarray:
-        """Get the IoU matrix for a fame."""
-        return self._ious[self._ious_dict[frame]]
-
     def compute(
         self,
         ground_truth: Tracks,
         hypotheses: Tracks,
         clearmot_metrics: bool = False,
         id_metrics: bool = False,
         hota_metrics: bool = True,
@@ -94,15 +79,15 @@
                 - IDFP (ID false positives)
                 - IDFN (ID false negatives)
                 - IDTP (ID true positives)
 
             - HOTA metrics (both average and individual alpha values). Note that I use
             the matching algorithm from the paper, which differs from what the official
             repository (TrackEval) is using - see
-            `this issue <https://github.com/JonathonLuiten/TrackEval/issues/22>`__
+            [this issue](https://github.com/JonathonLuiten/TrackEval/issues/22)
             for more details
 
                 - HOTA
                 - AssA
                 - DetA
                 - LocA
 
@@ -111,49 +96,66 @@
             hypotheses: Hypotheses tracks.
             clearmot_metrics: Whether to compute the CLEARMOT metrics.
             id_metrics: Whether to compute the ID metrics.
             hota_metrics: Whether to compute the HOTA metrics.
 
         Returns:
             A dictionary of computed metrics. Metrics are saved under the key of their
-            metric family (``"clearmot"``, ``"id"``, ``"hota"``).
+            metric family (`"clearmot"`, `"id"`, `"hota"`).
         """
         if not (clearmot_metrics or id_metrics or hota_metrics):
             raise ValueError("You must select some metrics to compute.")
 
         if not len(ground_truth):
             raise ValueError("No objects in ``ground_truths``, nothing to compute.")
 
         with timer.timer(self._logger, "Precompute IoU"):
-            self._precompute_iou(ground_truth, hypotheses)
+            self._ious_dict = _compute_ious(ground_truth, hypotheses)
 
         if clearmot_metrics:
             with timer.timer(self._logger, "Compute CLEARMOT Metrics"):
-                clrmt_metrics = self._calculate_clearmot_metrics(
-                    ground_truth, hypotheses, self._clearmot_dist_threshold
+                clrmt_metrics = calculate_clearmot_metrics(
+                    ground_truth,
+                    hypotheses,
+                    self._ious_dict,
+                    self._clearmot_dist_threshold,
                 )
         else:
             clrmt_metrics = None
 
         if id_metrics:
             with timer.timer(self._logger, "Compute ID Metrics"):
-                id_metrics_res = self._calculate_id_metrics(
-                    ground_truth, hypotheses, self._id_dist_threshold
+                id_metrics_res = calculate_id_metrics(
+                    ground_truth, hypotheses, self._ious_dict, self._id_dist_threshold
                 )
         else:
             id_metrics_res = None
 
         if hota_metrics:
             with timer.timer(self._logger, "Compute HOTA Metrics"):
-                hota_metrics_res = self._calculate_hota_metrics(
-                    ground_truth, hypotheses
+                hota_metrics_res = calculate_hota_metrics(
+                    ground_truth,
+                    hypotheses,
+                    self._ious_dict,
                 )
         else:
             hota_metrics_res = None
 
         # Remove IoU matrix to release memory
-        del self._ious
         del self._ious_dict
 
         return MOTMetricsResults(
             clearmot=clrmt_metrics, id=id_metrics_res, hota=hota_metrics_res
         )
+
+
+def _compute_ious(
+    tracks_1: Tracks, tracks_2: Tracks
+) -> dict[int, npt.NDArray[np.float32]]:
+    all_frames = sorted(set(tracks_1.frames).intersection(tracks_2.frames))
+
+    ious: dict[int, npt.NDArray[np.float32]] = {}
+    for frame in all_frames:
+        ious_f = iou_dist(tracks_1[frame].bboxes, tracks_2[frame].bboxes)
+        ious[frame] = ious_f
+
+    return ious
```

### Comparing `evaldet-0.3.0/src/evaldet/tracks.py` & `evaldet-0.4.0/src/evaldet/tracks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections as co
 import csv
 import datetime as dt
 import pathlib
 import typing as t
-import xml.etree.ElementTree as ET
+import xml.etree.ElementTree as ET  # noqa
 
 import numpy as np
 import numpy.typing as npt
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 _ID_KEY = "id"
@@ -17,82 +17,82 @@
 _XMIN_KEY = "xmin"
 _YMIN_KEY = "ymin"
 _WIDTH_KEY = "width"
 _HEIGHT_KEY = "height"
 
 
 class FrameTracks(t.NamedTuple):
-    detections: np.ndarray
-    ids: np.ndarray
-    classes: np.ndarray
-    confs: np.ndarray
+    bboxes: npt.NDArray[np.float32]
+    ids: npt.NDArray[np.int32]
+    classes: npt.NDArray[np.int32]
+    confs: npt.NDArray[np.float32]
 
 
 TracksType = t.TypeVar("TracksType", bound="Tracks")
 
 
 class Tracks:
     """A class representing objects' tracks in a MOT setting.
 
     It can read the following MOT file formats
 
-    - MOT format (as described `here <https://motchallenge.net/instructions/>`__)
-    - MOT ground truth format (as described `here <https://arxiv.org/abs/1603.00831>`__)
-    - CVAT's version of the MOT format (as described `here <https://openvinotoolkit.github.io/cvat/docs/manual/advanced/formats/format-mot/>`__)
-    - CVAT for Video format (as described `here <https://openvinotoolkit.github.io/cvat/docs/manual/advanced/xml_format/>`__)
-    - UA-DETRAC XML format (you can download an example `here <https://detrac-db.rit.albany.edu/Tracking>`__)
+    - MOT format (as described [here](https://motchallenge.net/instructions/))
+    - MOT ground truth format (as described [here](https://arxiv.org/abs/1603.00831))
+    - CVAT's version of the MOT format (as described [here](https://openvinotoolkit.github.io/cvat/docs/manual/advanced/formats/format-mot/))
+    - CVAT for Video format (as described [here](https://openvinotoolkit.github.io/cvat/docs/manual/advanced/xml_format/))
+    - UA-DETRAC XML format (you can download an example [here](https://detrac-db.rit.albany.edu/Tracking))
 
     Internally, all the attributes are saved as a single numpy array, and sorted by
     frame numbers. This enables easy access, as well as easy conversion to/from formats
     that to not store detections by frames (but by tracks).
 
     The frame numbers will be zero-indexed internally, so for the MOT files 1 will be
     subtracted from all frame numbers.
     """
 
     _frame_nums: npt.NDArray[np.int32]
     _ids: npt.NDArray[np.int32]
-    _detections: npt.NDArray[np.float32]
+    _bboxes: npt.NDArray[np.float32]
     _classes: npt.NDArray[np.int32]
     _confs: npt.NDArray[np.float32]
-    _frame_ind_dict: t.Dict[int, t.Tuple[int, int]]
+    _frame_ind_dict: dict[int, tuple[int, int]]
 
     @classmethod
     def from_csv(
         cls: t.Type[TracksType],
         csv_file: t.Union[str, pathlib.Path],
-        fieldnames: t.List[str],
+        fieldnames: t.Sequence[str],
         zero_indexed: bool = True,
     ) -> TracksType:
         """Get detections from a CSV file.
 
         The CSV file should have a normal comma (,) as a separator, and should not
         include a header.
 
         Args:
             csv_file: path to the CSV file
             filednames: The names of the fields. This will be passed to
-                ``csv.DictReader``. It should contain the names of the fields, in order
+                `csv.DictReader`. It should contain the names of the fields, in order
                 that they appear. The following names will be used (others will be
                 disregarded):
-                - ``xmin``
-                - ``ymin``
-                - ``height``
-                - ``width``
-                - ``conf``: for the confidence of the item
-                - ``class``: for the class label of the item
-                - ``id``: for the id of the item
-                - ``frame``: for the frame number
+                - `xmin`
+                - `ymin`
+                - `height`
+                - `width`
+                - `conf`: for the confidence of the item
+                - `class`: for the class label of the item
+                - `id`: for the id of the item
+                - `frame`: for the frame number
             zero_indexed: If the frame numbers are zero indexed. Otherwise they are
                 assumed to be 1 indexed, and 1 will be subtracted from all frame numbers
                 to make them zero indexed.
         """
         with open(csv_file, newline="") as file:
             csv_reader = csv.DictReader(file, fieldnames=fieldnames, dialect="unix")
-            accumulator: t.Dict[str, t.List] = co.defaultdict(list)
+            accumulator: dict[str, list] = co.defaultdict(list)
 
             for line_num, line in enumerate(csv_reader):
                 try:
                     cls._add_to_tracks_accumulator(accumulator, line)
 
                 except ValueError as e:
                     raise ValueError(
@@ -106,20 +106,22 @@
 
     @classmethod
     def from_mot(
         cls: t.Type[TracksType], file_path: t.Union[pathlib.Path, str]
     ) -> TracksType:
         """Creates a Tracks object from detections file in the MOT format.
 
-        The format should look like this::
+        The format should look like this
 
-            <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <conf>, <x>, <y>, <z>
+        ```
+        <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <conf>, <x>, <y>, <z>
+        ```
 
         Note that all values above are expected to be **numeric** - string values will
-        cause an error. The values for ``x``, ``y`` and ``z`` will be ignored.
+        cause an error. The values for `x`, `y` and `z` will be ignored.
 
         The frame numbers will be zero-indexed internally, so 1 will be subtracted from
         all frame numbers.
 
         Args:
             file_path: Path where the detections file is located. The file should be
                 in the format described above, and should not have a header.
@@ -138,23 +140,25 @@
 
         return cls.from_csv(file_path, fieldnames, zero_indexed=False)
 
     @classmethod
     def from_mot_gt(
         cls: t.Type[TracksType], file_path: t.Union[pathlib.Path, str]
     ) -> TracksType:
-        """Creates a Tracks object from detections file in the MOT ground truth format.
-        This format has some more information compared to the normal
-
-        The format should look like this::
+        """
+        Creates a Tracks object from detections file in the MOT ground truth format.
+        This format has some more information compared to the normal.
 
-            <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <conf>, <class>, <visibility>
+        The format should look like this
+        ```
+        <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <conf>, <class>, <visibility>
+        ```
 
         Note that all values above are expected to be **numeric** - string values will
-        cause an error. The value for ``visibility`` will be ignored.
+        cause an error. The value for `visibility` will be ignored.
 
         The frame numbers will be zero-indexed internally, so 1 will be subtracted from
         all frame numbers.
 
         Args:
             file_path: Path where the detections file is located. The file should be
                 in the format described above, and should not have a header.
@@ -178,19 +182,21 @@
     def from_mot_cvat(
         cls: t.Type[TracksType], file_path: t.Union[pathlib.Path, str]
     ) -> "Tracks":
         """Creates a Tracks object from detections file in the CVAT's MOT format.
 
         The format should look like this::
 
-            <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <not ignored>, <class>, <visibility>, <skipped>
+        ```
+        <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <not ignored>, <class>, <visibility>, <skipped>
+        ```
 
         Note that all values above are expected to be **numeric** - string values will
-        cause an error. The last two elements (``visibility`` and ``skipped``) are
-        optional. The values for ``not ignored``, ``visibility`` and ``skipped`` will be
+        cause an error. The last two elements (`visibility` and `skipped`) are
+        optional. The values for `not ignored`, `visibility` and `skipped` will be
         ignored.
 
         The frame numbers will be zero-indexed internally, so 1 will be subtracted from
         all frame numbers.
 
         Args:
             file_path: Path where the detections file is located. The file should be
@@ -211,94 +217,94 @@
         return cls.from_csv(file_path, fieldnames, zero_indexed=False)
 
     @classmethod
     def from_ua_detrac(
         cls: t.Type[TracksType],
         file_path: t.Union[pathlib.Path, str],
         classes_attr_name: t.Optional[str] = None,
-        classes_list: t.Optional[t.List[str]] = None,
+        classes_list: t.Optional[t.Sequence[str]] = None,
     ) -> TracksType:
         """Creates a Tracks object from detections file in the UA-DETRAC XML format.
 
         Here's how this file might look like:
 
-        .. code-block:: xml
+        ```
+        <sequence name="MVI_20033">
+            <sequence_attribute camera_state="unstable" sence_weather="sunny"/>
+            <ignored_region>
+                <box height="53.75" left="458.75" top="0.5" width="159.5"/>
+            </ignored_region>
+            <frame density="4" num="1">
+                <target_list>
+                    <target id="1">
+                        <box height="71.46" left="256.88" top="201.1" width="67.06"/>
+                        <attribute color="Multi" orientation="315" speed="1.0394" trajectory_length="91" truncation_ratio="0" vehicle_type="Taxi"/>
+                    </target>
+                </target_list>
+            </frame>
+            <frame density="2" num="2">
+                <target_list>
+                    <target id="2">
+                        <box height="32.44999999999999" left="329.27" top="96.65" width="56.53000000000003"/>
+                        <attribute color="Multi" orientation="315" speed="1.0394" trajectory_length="3" truncation_ratio="0" vehicle_type="Car"/>
+                    </target>
+                    <target id="4">
+                        <box height="122.67000000000002" left="0.0" top="356.7" width="76.6"/>
+                        <attribute color="Multi" orientation="315" speed="1.0394" trajectory_length="1" truncation_ratio="0" vehicle_type="Car"/>
+                    </target>
+                </target_list>
+            </frame>
+        </sequence>
+        ```
 
-            <sequence name="MVI_20033">
-                <sequence_attribute camera_state="unstable" sence_weather="sunny"/>
-                <ignored_region>
-                    <box height="53.75" left="458.75" top="0.5" width="159.5"/>
-                </ignored_region>
-                <frame density="4" num="1">
-                    <target_list>
-                        <target id="1">
-                            <box height="71.46" left="256.88" top="201.1" width="67.06"/>
-                            <attribute color="Multi" orientation="315" speed="1.0394" trajectory_length="91" truncation_ratio="0" vehicle_type="Taxi"/>
-                        </target>
-                    </target_list>
-                </frame>
-                <frame density="2" num="2">
-                    <target_list>
-                        <target id="2">
-                            <box height="32.44999999999999" left="329.27" top="96.65" width="56.53000000000003"/>
-                            <attribute color="Multi" orientation="315" speed="1.0394" trajectory_length="3" truncation_ratio="0" vehicle_type="Car"/>
-                        </target>
-                        <target id="4">
-                            <box height="122.67000000000002" left="0.0" top="356.7" width="76.6"/>
-                            <attribute color="Multi" orientation="315" speed="1.0394" trajectory_length="1" truncation_ratio="0" vehicle_type="Car"/>
-                        </target>
-                    </target_list>
-                </frame>
-            </sequence>
-
-        The ``ignored_region`` node will not be taken into account - if you want
+        The `ignored_region` node will not be taken into account - if you want
         some detections to be ignored, you need to filter them prior to the creation
         of the file.
 
         All attributes of each detection will be ignored, except for the one designated
-        by ``classes_attr_name`` (for example, in original UA-DETRAC this could be
-        ``"vehicle_type"``). This would then give values for ``classes`` attribute.
+        by `classes_attr_name` (for example, in original UA-DETRAC this could be
+        `"vehicle_type"`). This would then give values for `classes` attribute.
         As this attribute usually contains string values, you also need to provide
-        ``classes_list`` - a list of all possible class values. The class attribute will
+        `classes_list` - a list of all possible class values. The class attribute will
         then be replaced by the index of the label in this list.
 
         Args:
             file_path: Path where the detections file is located
-            classes_attr_name: The name of the attribute to be used for the ``classes``
-                attribute. If provided, ``classes_list`` must be provided as well.
+            classes_attr_name: The name of the attribute to be used for the `classes`
+                attribute. If provided, `classes_list` must be provided as well.
             classes_list: The list of all possible class values - must be provided if
-                ``classes_attr_name`` is provided. The values from that attribute in the
+                `classes_attr_name` is provided. The values from that attribute in the
                 file will then be replaced by the index of that value in this list.
         """
 
         if classes_attr_name and not classes_list:
             raise ValueError(
                 "If you provide `classes_attr_name`,"
                 " you must also provide `classes_list`"
             )
 
         xml_tree = ET.parse(file_path)
         root = xml_tree.getroot()
 
-        accumulator: t.Dict[str, t.List] = co.defaultdict(list)
+        accumulator: dict[str, list] = co.defaultdict(list)
 
-        frames = root.findall(_FRAME_KEY)
+        frames = root.findall("frame")
         for frame in frames:
             tracks_f = frame.find("target_list").findall("target")  # type: ignore
 
             current_frame = frame.attrib["num"]
             for track in tracks_f:
                 box = track.find("box")
                 assert box is not None
 
                 det_item = {
-                    _ID_KEY: track.attrib[_ID_KEY],
+                    _ID_KEY: track.attrib["id"],
                     _FRAME_KEY: current_frame,
-                    _HEIGHT_KEY: box.attrib[_HEIGHT_KEY],
-                    _WIDTH_KEY: box.attrib[_WIDTH_KEY],
+                    _HEIGHT_KEY: box.attrib["height"],
+                    _WIDTH_KEY: box.attrib["width"],
                     _XMIN_KEY: box.attrib["left"],
                     _YMIN_KEY: box.attrib["top"],
                 }
 
                 if classes_attr_name:
                     attrs = track.find("attribute")
                     class_val = attrs.attrib[classes_attr_name]  # type: ignore
@@ -308,77 +314,77 @@
 
         return cls(**accumulator, zero_indexed=True)
 
     @classmethod
     def from_cvat_video(
         cls: t.Type[TracksType],
         file_path: t.Union[pathlib.Path, str],
-        classes_list: t.List[str],
+        classes_list: t.Sequence[str],
     ) -> TracksType:
-        """Creates a Tracks object from detections file in the CVAT for Video XML
-        format.
+        """
+        Creates a Tracks object from detections file in the CVAT for Video XML format.
 
         Here's how this file might look like:
 
-        .. code-block:: xml
-
-            <annotations>
-                <version>1.1</version>
-                <meta>
-                    <!-- lots of non-relevant metadata -->
-                </meta>
-                <track id="0" label="Car" source="manual">
-                    <box frame="659" outside="0" occluded="0" keyframe="1" xtl="323.83" ytl="104.06" xbr="367.60" ybr="139.49" z_order="-1"> </box>
-                    <box frame="660" outside="0" occluded="0" keyframe="1" xtl="320.98" ytl="105.24" xbr="365.65" ybr="140.95" z_order="0"> </box>
-                </track>
-                <track id="1" label="Car" source="manual">
-                    <box frame="659" outside="0" occluded="0" keyframe="1" xtl="273.10" ytl="88.77" xbr="328.69" ybr="113.09" z_order="1"> </box>
-                    <box frame="660" outside="0" occluded="0" keyframe="1" xtl="273.10" ytl="88.88" xbr="328.80" ybr="113.40" z_order="0"> </box>
-                </track>
-                <track id="2" label="Car" source="manual">
-                    <box frame="659" outside="0" occluded="0" keyframe="1" xtl="375.24" ytl="80.43" xbr="401.65" ybr="102.67" z_order="0"> </box>
-                    <box frame="660" outside="0" occluded="0" keyframe="1" xtl="374.69" ytl="80.78" xbr="401.09" ybr="103.01" z_order="0"> </box>
-                </track>
-                <track id="3" label="Car" source="manual">
-                    <box frame="699" outside="0" occluded="0" keyframe="1" xtl="381.50" ytl="79.04" xbr="405.12" ybr="99.19" z_order="0"> </box>
-                    <box frame="700" outside="0" occluded="0" keyframe="1" xtl="380.94" ytl="79.60" xbr="404.56" ybr="99.75" z_order="0"> </box>
-                </track>
-            </annotations>
+        ```xml
+        <annotations>
+            <version>1.1</version>
+            <meta>
+                <!-- lots of non-relevant metadata -->
+            </meta>
+            <track id="0" label="Car" source="manual">
+                <box frame="659" outside="0" occluded="0" keyframe="1" xtl="323.83" ytl="104.06" xbr="367.60" ybr="139.49" z_order="-1"> </box>
+                <box frame="660" outside="0" occluded="0" keyframe="1" xtl="320.98" ytl="105.24" xbr="365.65" ybr="140.95" z_order="0"> </box>
+            </track>
+            <track id="1" label="Car" source="manual">
+                <box frame="659" outside="0" occluded="0" keyframe="1" xtl="273.10" ytl="88.77" xbr="328.69" ybr="113.09" z_order="1"> </box>
+                <box frame="660" outside="0" occluded="0" keyframe="1" xtl="273.10" ytl="88.88" xbr="328.80" ybr="113.40" z_order="0"> </box>
+            </track>
+            <track id="2" label="Car" source="manual">
+                <box frame="659" outside="0" occluded="0" keyframe="1" xtl="375.24" ytl="80.43" xbr="401.65" ybr="102.67" z_order="0"> </box>
+                <box frame="660" outside="0" occluded="0" keyframe="1" xtl="374.69" ytl="80.78" xbr="401.09" ybr="103.01" z_order="0"> </box>
+            </track>
+            <track id="3" label="Car" source="manual">
+                <box frame="699" outside="0" occluded="0" keyframe="1" xtl="381.50" ytl="79.04" xbr="405.12" ybr="99.19" z_order="0"> </box>
+                <box frame="700" outside="0" occluded="0" keyframe="1" xtl="380.94" ytl="79.60" xbr="404.56" ybr="99.75" z_order="0"> </box>
+            </track>
+        </annotations>
+        ```
 
-        All attributes of each detection will be ignored, except for ``label`` (in the
-        ``track`` object), which will be used for the ``class`` values. As this
+        All attributes of each detection will be ignored, except for `label` (in the
+        `track` object), which will be used for the `class` values. As this
         attribute usually contains string values, you also need to provide
-        ``classes_list`` - a list of all possible class values. The class attribute will
+        `classes_list` - a list of all possible class values. The class attribute will
         then be replaced by the index of the label in this list.
 
-        Elements with "outside=1" will be ignored.
+        Elements with `"outside=1"` will be ignored.
 
         Args:
             file_path: Path where the detections file is located
             classes_list: The list of all possible class values. The values from that
                 attribute in the file will then be replaced by the index of that value
                 in this list.
         """
 
         xml_tree = ET.parse(file_path)
         root = xml_tree.getroot()
-        accumulator: t.Dict[str, t.List] = co.defaultdict(list)
+        accumulator: dict[str, list] = co.defaultdict(list)
 
         tracks_cvat = root.findall("track")
         for track_cvat in tracks_cvat:
-            track_id = track_cvat.attrib[_ID_KEY]
+            track_id = track_cvat.attrib["id"]
             track_class = classes_list.index(track_cvat.attrib["label"])
 
             for box in track_cvat.findall("box"):
                 if int(box.attrib["outside"]) == 1:
                     continue
 
                 det_item = {
                     _ID_KEY: track_id,
-                    _FRAME_KEY: box.attrib[_FRAME_KEY],
+                    _FRAME_KEY: box.attrib["frame"],
                     _HEIGHT_KEY: float(box.attrib["ybr"]) - float(box.attrib["ytl"]),
                     _WIDTH_KEY: float(box.attrib["xbr"]) - float(box.attrib["xtl"]),
                     _XMIN_KEY: box.attrib["xtl"],
                     _YMIN_KEY: box.attrib["ytl"],
                     _CLASS_KEY: track_class,
                 }
 
@@ -389,26 +395,29 @@
     @classmethod
     def from_parquet(
         cls: t.Type[TracksType], file_path: t.Union[pathlib.Path, str]
     ) -> TracksType:
         """Read the tracks from a parquet file.
 
         The file should have the following columns:
-           <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <conf>, <class>
+
+        ```
+        <frame>, <id>, <xmin>, <ymin>, <width>, <height>, <conf>, <class>
+        ```
 
         Args:
             file_path: Path where the detections file is located
         """
 
         table = pq.read_table(file_path)
         table_cols = table.column_names
         tracks = cls(
             ids=table[_ID_KEY].to_numpy(),
             frame_nums=table[_FRAME_KEY].to_numpy(),
-            detections=np.stack(
+            bboxes=np.stack(
                 (
                     table[_XMIN_KEY].to_numpy(),
                     table[_YMIN_KEY].to_numpy(),
                     table[_WIDTH_KEY].to_numpy(),
                     table[_HEIGHT_KEY].to_numpy(),
                 ),
                 axis=-1,
@@ -423,112 +432,109 @@
         frame_num, track_id = int(new_obj[_FRAME_KEY]), int(float(new_obj[_ID_KEY]))
 
         xmin, ymin = float(new_obj[_XMIN_KEY]), float(new_obj[_YMIN_KEY])
         width, height = float(new_obj[_WIDTH_KEY]), float(new_obj[_HEIGHT_KEY])
 
         accumulator["frame_nums"].append(frame_num)
         accumulator["ids"].append(track_id)
-        accumulator["detections"].append(
+        accumulator["bboxes"].append(
             np.array([xmin, ymin, width, height], dtype=np.float32)
         )
 
         if _CONF_KEY in new_obj:
             conf = float(new_obj[_CONF_KEY])
             accumulator["confs"].append(conf)
         if _CLASS_KEY in new_obj:
             class_id = int(new_obj[_CLASS_KEY])
             accumulator["classes"].append(class_id)
 
     def __init__(
         self,
-        ids: t.Union[t.List[int], npt.NDArray[np.int32]],
-        frame_nums: t.Union[t.List[int], npt.NDArray[np.int32]],
-        detections: t.Union[t.List[npt.NDArray[np.float32]], npt.NDArray[np.float32]],
-        classes: t.Optional[t.Union[t.List[int], npt.NDArray[np.int32]]] = None,
-        confs: t.Optional[t.Union[t.List[float], npt.NDArray[np.float32]]] = None,
+        ids: t.Union[t.Sequence[int], npt.NDArray[np.int32]],
+        frame_nums: t.Union[t.Sequence[int], npt.NDArray[np.int32]],
+        bboxes: t.Union[t.Sequence[npt.NDArray[np.float32]], npt.NDArray[np.float32]],
+        classes: t.Optional[t.Union[t.Sequence[int], npt.NDArray[np.int32]]] = None,
+        confs: t.Optional[t.Union[t.Sequence[float], npt.NDArray[np.float32]]] = None,
         zero_indexed: bool = True,
     ) -> None:
         """
-        Create a ``Tracks`` instance.
+        Create a `Tracks` instance.
 
         Args:
-            ids: A list or array of track ids, which should be of type int32.
-            frame_nums: A list or array of frame numbers, which should be of type int32.
-            detections: A list or array of detection bounding boxes, which should be
-                in the format `x, y, w, h`, using a top-left-origin coordinate system.
-                The detections should be of `float32` dtype.
-            classes: A list or array of classes (labels), which should be of dtype
-                int32. It can not be provided, or be provided as an empty list - in this
-                case internally all detections will have a class of ``0``.
-            confs: A list or array of confidences (scores), which should be of dtype
-                float32. It can not be provided, or be provided as an empty list - in
+            ids: A list or array of track ids.
+            frame_nums: A list or array of frame numbers.
+            bboxes: A list or array of detection bounding boxes, which should be
+                in the format `xywh`, using a top-left-origin coordinate system.
+            classes: A list or array of classes (labels). It can not be provided, in
+                this case internally all detections will have a class of ``0``.
+            confs: A list or array of confidences (scores). It can not be provided, in
                 this case internally all detections will have a confidence of ``1``.
             zero_indexed: If the frame numbers are zero indexed. If not, it is assumed
                 that they are 1-indexed - that is, they start with 1, and will be
                 transformed to 0-indexed internally, by subtracting 1 from them.
         """
-        if len(ids) != len(detections):
+        if len(ids) != len(bboxes):
             raise ValueError(
-                "`detections` and `ids` should contain the same number of items."
+                "`bboxes` and `ids` should contain the same number of items."
             )
 
         if len(ids) != len(frame_nums):
             raise ValueError(
                 "`ids` and `frame_nums` should contain the same number of items."
             )
 
-        if classes is not None and (len(classes) != len(ids) and len(classes) > 0):
+        if classes is not None and len(classes) != len(ids):
             raise ValueError(
                 "If `classes` is given, it should contain the same number of items"
                 " as `ids`."
             )
 
-        if confs is not None and (len(confs) != len(ids) and len(confs) > 0):
+        if confs is not None and len(confs) != len(ids):
             raise ValueError(
                 "If `confs` is given, it should contain the same number of items"
                 " as `ids`."
             )
 
-        if len(detections) > 0 and detections[0].shape != (4,):
+        if len(bboxes) > 0 and bboxes[0].shape != (4,):
             raise ValueError(
-                "Each row of `detections` should be an 4-item array, but got"
-                f" shape {detections[0].shape}"
+                "Each row of `bboxes` should be an 4-item array, but got"
+                f" shape {bboxes[0].shape}"
             )
 
         if len(ids) == 0:
             self._frame_nums = np.zeros((0,), dtype=np.int32)
             self._ids = np.zeros((0,), dtype=np.int32)
-            self._detections = np.zeros((0, 4), dtype=np.float32)
+            self._bboxes = np.zeros((0, 4), dtype=np.float32)
             self._classes = np.zeros((0,), dtype=np.int32)
             self._confs = np.zeros((0,), dtype=np.float32)
 
         else:
             frame_nums = np.array(frame_nums)
             sort_inds = np.argsort(frame_nums)
 
             self._frame_nums = np.array(
                 frame_nums[sort_inds], copy=True, dtype=np.int32
             )
 
             self._ids = np.array(np.array(ids)[sort_inds], dtype=np.int32, copy=True)
-            self._detections = np.array(
-                np.array(detections)[sort_inds], dtype=np.float32, copy=True
+            self._bboxes = np.array(
+                np.array(bboxes)[sort_inds], dtype=np.float32, copy=True
             )
 
             if zero_indexed is False:
                 self._frame_nums -= 1
 
-            if classes is None or len(classes) == 0:
+            if classes is None:
                 self._classes = np.zeros((len(ids),), dtype=np.int32)
             else:
                 self._classes = np.array(
                     np.array(classes)[sort_inds], dtype=np.int32, copy=True
                 )
 
-            if confs is None or len(confs) == 0:
+            if confs is None:
                 self._confs = np.ones((len(ids),), dtype=np.float32)
             else:
                 self._confs = np.array(
                     np.array(confs)[sort_inds], dtype=np.float32, copy=True
                 )
 
         self._create_frame_ind_dict()
@@ -541,49 +547,54 @@
         u_frame_nums, start_inds = np.unique(self._frame_nums, return_index=True)
         frame_start_inds = start_inds.tolist()
         frame_end_inds = start_inds[1:].tolist() + [len(self._frame_nums)]
 
         frame_start_end_inds = zip(frame_start_inds, frame_end_inds)
         self._frame_ind_dict = dict(zip(u_frame_nums.tolist(), frame_start_end_inds))
 
-    def filter(self, filter: np.ndarray) -> None:
+    def filter(self, filter: np.ndarray) -> "Tracks":
         """Filter the tracks using a boolean mask.
 
         This method will filter all attributes according to the mask provided.
 
         Args:
             filter: A boolean array, should be the same length as ids and other
                 attributes.
+
+        Return:
+            The filtered tracks
         """
 
         if filter.shape != self.ids.shape:
             raise ValueError(
                 "Shape of the filter should equal the shape of ids, got"
                 f" {filter.shape}"
             )
 
-        self._ids = self._ids[filter]
-        self._frame_nums = self._frame_nums[filter]
-        self._classes = self._classes[filter]
-        self._confs = self._confs[filter]
-        self._detections = self._detections[filter]
+        filtered_tracks = Tracks(
+            ids=self._ids[filter],
+            frame_nums=self._frame_nums[filter],
+            bboxes=self._bboxes[filter],
+            classes=self._classes[filter],
+            confs=self._confs[filter],
+        )
 
-        self._create_frame_ind_dict()
+        return filtered_tracks
 
     @property
     def ids(self) -> npt.NDArray[np.int32]:
         return self._ids
 
     @property
     def frame_nums(self) -> npt.NDArray[np.int32]:
         return self._frame_nums
 
     @property
-    def detections(self) -> npt.NDArray[np.float32]:
-        return self._detections
+    def bboxes(self) -> npt.NDArray[np.float32]:
+        return self._bboxes
 
     @property
     def classes(self) -> npt.NDArray[np.int32]:
         return self._classes
 
     @property
     def confs(self) -> npt.NDArray[np.float32]:
@@ -610,45 +621,44 @@
         """Get an ordered list of all frame numbers in the collection."""
         return set(self._frame_ind_dict.keys())
 
     def __len__(self) -> int:
         return len(self._ids)
 
     def __contains__(self, idx: int) -> bool:
-        """Whether the frame ``idx`` is present in the collection."""
+        """Whether the frame `idx` is present in the collection."""
         return idx in self._frame_ind_dict
 
     @t.overload
     def __getitem__(self, idx: int) -> FrameTracks:
-        """Get the frame with number ``idx``.
+        """Get the frame with number `idx`.
 
         Note that indexing with negative values is not supported.
         """
 
     @t.overload
     def __getitem__(self, idx: slice) -> "Tracks":
         """Select only a subset of frames, as defined by the slice.
 
-        Note that the ``step`` argument is not supported and will result in an error
+        Note that the `step` argument is not supported and will result in an error
         being raised if it is supplied. Negative indices for start or stop argument are
         similarly not supported.
         """
 
     def __getitem__(self, idx: t.Union[int, slice]) -> t.Union[FrameTracks, "Tracks"]:
-
         if isinstance(idx, int):
             if idx < 0:
                 raise ValueError("Indexing with negative values is not supported.")
             if idx not in self:
                 raise KeyError(f"The frame {idx} does not exist.")
 
             start, end = self._frame_ind_dict[idx]
             return FrameTracks(
                 ids=self._ids[start:end],
-                detections=self._detections[start:end],
+                bboxes=self._bboxes[start:end],
                 classes=self._classes[start:end],
                 confs=self._confs[start:end],
             )
 
         elif isinstance(idx, slice):
             start, stop, step = idx.start, idx.stop, idx.step
             if step is not None:
@@ -662,39 +672,40 @@
 
             start = self._frame_ind_dict[min(keep_frames)][0]
             end = self._frame_ind_dict[max(keep_frames)][1]
 
             new_tracks = type(self)(
                 ids=self._ids[start:end],
                 frame_nums=self._frame_nums[start:end],
-                detections=self._detections[start:end],
+                bboxes=self._bboxes[start:end],
                 classes=self._classes[start:end],
                 confs=self._confs[start:end],
             )
 
             return new_tracks
         else:
             raise ValueError("Unrecognized index type")
 
     def to_cvat_video(
         self,
         filename: t.Union[pathlib.Path, str],
         labels: t.Sequence[str],
-        image_size: t.Tuple[int, int] = (1, 1),
+        image_size: tuple[int, int] = (1, 1),
     ) -> None:
         """Export detections to CVAT for Video 1.1 format.
 
-        More information on the format can be found `here <https://opencv.github.io/cvat/docs/manual/advanced/xml_format/>`_.
+        More information on the format can be found
+        [here](https://opencv.github.io/cvat/docs/manual/advanced/xml_format/).
 
         Args:
-            filename: The name of the file to save to - should have an ``.xml`` suffix.
+            filename: The name of the file to save to - should have an `.xml` suffix.
             labels: A list/tuple of label names. The length should be at least the
                 maximum label index - 1 (the first label corresponds to label at the
                 0-th index).
-            image_size: The size of the image in the ``[w, h]`` format, in pixels.
+            image_size: The size of the image in the `[w, h]` format, in pixels.
         """
 
         if len(self._ids) == 0:
             max_label_ind = 1
         else:
             max_label_ind = max(self.all_classes) + 1
         if len(labels) < max_label_ind:
@@ -776,15 +787,15 @@
                 "track",
                 id=str(track_id),
                 label=labels[label],
                 source=type(self).__name__,
             )
 
             for i, (ind, frame_num) in enumerate(zip(id_inds, track_frames)):
-                bbox = self.detections[ind]
+                bbox = self.bboxes[ind]
                 ET.SubElement(
                     track_el,
                     "box",
                     frame=str(frame_num),
                     xtl=f"{bbox[0]:.2f}",
                     ytl=f"{bbox[1]:.2f}",
                     xbr=f"{bbox[0] + bbox[2]:.2f}",
@@ -815,22 +826,23 @@
         )
 
     def to_csv(
         self,
         dirname: t.Union[pathlib.Path, str],
         labels: t.Sequence[str],
     ) -> None:
-        """Export detections to a simple CSV format. The format comprises of two files:
-        ``dets.csv``, containing the detections, and ``labels.txt``, which contains
-        the names of the labels (corresponding to label indices in ``dets.csv``). The
-        rows in ``dets.csv`` have the following format:
+        """
+        Export detections to a simple CSV format. The format comprises of two files:
+        `dets.csv`, containing the detections, and `labels.txt`, which contains
+        the names of the labels (corresponding to label indices in `dets.csv`). The
+        rows in `dets.csv` have the following format:
 
             <frame>, <id>, <x_min>, <y_min>, <width>, <height>, <class>, <conf>
 
-        Note that ``frame`` and ``class`` are both 0 indexed.
+        Note that `frame` and `class` are both 0 indexed.
 
         Args:
             dirname: The name of the directory to save to - will be created if it
                 doesn't already exist.
             labels: A list/tuple of label names. The length should be at least the
                 maximum label index - 1 (the first label corresponds to label at the
                 0-th index).
@@ -863,41 +875,41 @@
             "class_id",
             "conf",
         ]
         with open(pathlib.Path(dirname) / "dets.csv", "w", newline="") as f:
             writer = csv.DictWriter(f, fieldnames=fieldnames)
 
             for ind in range(len(self.ids)):
-                item: t.Dict[str, t.Union[str, int, float]] = {
+                item: dict[str, t.Union[str, int, float]] = {
                     "frame_id": self.frame_nums[ind],
                     "track_id": self.ids[ind],
                     "conf": self.confs[ind],
                     "class_id": self.classes[ind],
-                    "x_min": f"{self.detections[ind][0]:.2f}",
-                    "y_min": f"{self.detections[ind][1]:.2f}",
-                    "w": f"{self.detections[ind][2]:.2f}",
-                    "h": f"{self.detections[ind][3]:.2f}",
+                    "x_min": f"{self.bboxes[ind][0]:.2f}",
+                    "y_min": f"{self.bboxes[ind][1]:.2f}",
+                    "w": f"{self.bboxes[ind][2]:.2f}",
+                    "h": f"{self.bboxes[ind][3]:.2f}",
                 }
                 writer.writerow(item)
 
     def to_parquet(self, file_path: t.Union[pathlib.Path, str]) -> None:
         """Export detections to parquet format.
 
         Args:
             file_name: Relative or absolute file name to save to.
         """
 
         table = pa.Table.from_arrays(
             [
                 pa.array(self._ids),
                 pa.array(self._frame_nums),
-                pa.array(self._detections[:, 0]),
-                pa.array(self._detections[:, 1]),
-                pa.array(self._detections[:, 2]),
-                pa.array(self._detections[:, 3]),
+                pa.array(self._bboxes[:, 0]),
+                pa.array(self._bboxes[:, 1]),
+                pa.array(self._bboxes[:, 2]),
+                pa.array(self._bboxes[:, 3]),
                 pa.array(self._confs),
                 pa.array(self._classes),
             ],
             [
                 _ID_KEY,
                 _FRAME_KEY,
                 _XMIN_KEY,
```

### Comparing `evaldet-0.3.0/src/evaldet/mot_metrics/clearmot.py` & `evaldet-0.4.0/src/evaldet/mot/clearmot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,129 @@
 import logging
 import typing as t
 
 import numpy as np
+import numpy.typing as npt
 from scipy.optimize import linear_sum_assignment
 
-from ..tracks import Tracks
-from .base import MOTMetricBase
+from evaldet.tracks import Tracks
 
 logger = logging.getLogger(__name__)
 
 
 class CLEARMOTResults(t.TypedDict):
     MOTP: float
     MOTA: float
     FP_CLEAR: float
     FN_CLEAR: float
     IDSW: float
 
 
-class CLEARMOTMetrics(MOTMetricBase):
-    def _calculate_clearmot_metrics(
-        self, ground_truth: Tracks, hypotheses: Tracks, dist_threshold: float = 0.5
-    ) -> CLEARMOTResults:
-
-        all_frames = sorted(ground_truth.frames.union(hypotheses.frames))
-
-        false_negatives = 0
-        false_positives = 0
-        mismatches = 0
-        ground_truths = 0
-
-        matches_dist = []
-        matching: t.Dict[int, int] = {}
-
-        # This is the persistent matching dictionary, used to check for mismatches
-        # when a previously matched hypothesis is re-matched with a ground truth
-        matching_persist: t.Dict[int, int] = {}
-
-        for frame in all_frames:
-            if frame not in ground_truth:
-                matching = {}
-                false_positives += len(hypotheses[frame].ids)
-            elif frame not in hypotheses:
-                matching = {}
-                false_negatives += len(ground_truth[frame].ids)
-                ground_truths += len(ground_truth[frame].ids)
-            else:
-                hyp, gt = hypotheses[frame], ground_truth[frame]
-                ground_truths += len(gt.ids)
-
-                # Delete from matching missing gts/detections
-                for key in list(matching.keys()):
-                    if matching[key] not in hyp.ids or key not in gt.ids:
-                        del matching[key]
-
-                ious = self._get_iou_frame(frame)
-                id_ind_dict_gt = {_id: ind for ind, _id in enumerate(gt.ids)}
-                id_ind_dict_hyp = {_id: ind for ind, _id in enumerate(hyp.ids)}
-
-                for gt_id, hyp_id in tuple(matching.items()):
-                    dist_match = ious[id_ind_dict_gt[gt_id], id_ind_dict_hyp[hyp_id]]
-                    if dist_match > dist_threshold:
-                        del matching[gt_id]
-                    else:
-                        matches_dist.append(dist_match)
-
-                # For remaining (non-matching) gts/detections, compute matching as a LAP
-                match_gt_ids = tuple(matching.keys())
-                match_hyp_ids = tuple(matching.values())
-                inds_nm_gt = np.where(np.isin(gt.ids, match_gt_ids, invert=True))[0]
-                inds_nm_hyp = np.where(np.isin(hyp.ids, match_hyp_ids, invert=True))[0]
-                dist_matrix = ious[np.ix_(inds_nm_gt, inds_nm_hyp)]
-
-                for row_ind, col_ind in zip(*linear_sum_assignment(dist_matrix)):
-                    if dist_matrix[row_ind, col_ind] < dist_threshold:
-                        matching[gt.ids[inds_nm_gt[row_ind]]] = hyp.ids[
-                            inds_nm_hyp[col_ind]
-                        ]
-                        matches_dist.append(dist_matrix[row_ind, col_ind])
-
-                # Check if mismatches have occured
-                for key in matching:
-                    if (
-                        key in matching_persist
-                        and matching[key] != matching_persist[key]
-                    ):
-                        mismatches += 1
-
-                # Compute false positives and false negatices
-                false_negatives += len(gt.ids) - len(matching)
-                false_positives += len(hyp.ids) - len(matching)
-                matching_persist.update(matching)
-
-        if not matches_dist:
-            logger.warning("No matches were made, MOPT will be np.nan")
-            motp = np.nan
+def calculate_clearmot_metrics(
+    ground_truth: Tracks,
+    hypotheses: Tracks,
+    ious: dict[int, npt.NDArray[np.float32]],
+    dist_threshold: float = 0.5,
+) -> CLEARMOTResults:
+    """Calculate CLEARMOT metrics.
+
+    Args:
+        ground_truth: Ground truth tracks.
+        hypotheses: Hypotheses tracks.
+        ious_threshold: A dictionary where keys are frame numbers (indices), and values
+            are numpy matrices of IOU distances between detection in ground truth and
+            hypotheses for that frame. IOUs must be present for all frames that are
+            present in both ground truth and hypotheses.
+        dist_threshold: The distance threshold for the computation of metrics, used to
+            determine whether a matching between two tracks persist, and whether to
+            start a matching based on distance between two detections.
+
+    Returns:
+        A dictionary containing CLEARMOT metrics:
+
+            - MOTA (MOT Accuracy)
+            - MOTP (MOT Precision)
+            - FP (false positives)
+            - FN (false negatives)
+            - IDS (identity switches/mismatches)
+    """
+    all_frames = sorted(ground_truth.frames.union(hypotheses.frames))
+
+    false_negatives = 0
+    false_positives = 0
+    mismatches = 0
+    ground_truths = 0
+
+    matches_dist = []
+    matching: dict[int, int] = {}
+
+    # This is the persistent matching dictionary, used to check for mismatches
+    # when a previously matched hypothesis is re-matched with a ground truth
+    matching_persist: dict[int, int] = {}
+
+    for frame in all_frames:
+        if frame not in ground_truth:
+            matching = {}
+            false_positives += len(hypotheses[frame].ids)
+        elif frame not in hypotheses:
+            matching = {}
+            false_negatives += len(ground_truth[frame].ids)
+            ground_truths += len(ground_truth[frame].ids)
         else:
-            motp = sum(matches_dist) / len(matches_dist)
+            hyp, gt = hypotheses[frame], ground_truth[frame]
+            ground_truths += len(gt.ids)
 
-        mota = 1 - (false_negatives + false_positives + mismatches) / ground_truths
-
-        return {
-            "MOTP": motp,
-            "MOTA": mota,
-            "FP_CLEAR": false_positives,
-            "FN_CLEAR": false_negatives,
-            "IDSW": mismatches,
-        }
+            # Delete from matching missing gts/detections
+            for key in list(matching.keys()):
+                if matching[key] not in hyp.ids or key not in gt.ids:
+                    del matching[key]
+
+            iou_frame = ious[frame]
+            id_ind_dict_gt = {_id: ind for ind, _id in enumerate(gt.ids)}
+            id_ind_dict_hyp = {_id: ind for ind, _id in enumerate(hyp.ids)}
+
+            for gt_id, hyp_id in tuple(matching.items()):
+                dist_match = iou_frame[id_ind_dict_gt[gt_id], id_ind_dict_hyp[hyp_id]]
+                if dist_match > dist_threshold:
+                    del matching[gt_id]
+                else:
+                    matches_dist.append(dist_match)
+
+            # For remaining (non-matching) gts/detections, compute matching as a LAP
+            match_gt_ids = tuple(matching.keys())
+            match_hyp_ids = tuple(matching.values())
+            inds_nm_gt = np.where(np.isin(gt.ids, match_gt_ids, invert=True))[0]
+            inds_nm_hyp = np.where(np.isin(hyp.ids, match_hyp_ids, invert=True))[0]
+            dist_matrix = iou_frame[np.ix_(inds_nm_gt, inds_nm_hyp)]
+
+            for row_ind, col_ind in zip(*linear_sum_assignment(dist_matrix)):
+                if dist_matrix[row_ind, col_ind] < dist_threshold:
+                    matching[gt.ids[inds_nm_gt[row_ind]]] = hyp.ids[
+                        inds_nm_hyp[col_ind]
+                    ]
+                    matches_dist.append(dist_matrix[row_ind, col_ind])
+
+            # Check if mismatches have occured
+            for key in matching:
+                if key in matching_persist and matching[key] != matching_persist[key]:
+                    mismatches += 1
+
+            # Compute false positives and false negatices
+            false_negatives += len(gt.ids) - len(matching)
+            false_positives += len(hyp.ids) - len(matching)
+            matching_persist.update(matching)
+
+    if not matches_dist:
+        logger.warning("No matches were made, MOPT will be np.nan")
+        motp = np.nan
+    else:
+        motp = sum(matches_dist) / len(matches_dist)
+
+    mota = 1 - (false_negatives + false_positives + mismatches) / ground_truths
+
+    return {
+        "MOTP": motp,
+        "MOTA": mota,
+        "FP_CLEAR": false_positives,
+        "FN_CLEAR": false_negatives,
+        "IDSW": mismatches,
+    }
```

### Comparing `evaldet-0.3.0/src/evaldet/mot_metrics/hota.py` & `evaldet-0.4.0/src/evaldet/mot/hota.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import collections as co
 import typing as t
 
 import numpy as np
+import numpy.typing as npt
 from scipy.optimize import linear_sum_assignment
 
-from ..tracks import Tracks
-from ..utils import sparse
-from .base import MOTMetricBase
+from evaldet.tracks import Tracks
+
+from .utils import create_coo_array
 
 _EPS = 1 / 1000
 
 
 class HOTAResults(t.TypedDict):
     HOTA: float
     DetA: float
@@ -19,105 +20,122 @@
     alphas_HOTA: np.ndarray
     HOTA_alpha: np.ndarray
     DetA_alpha: np.ndarray
     AssA_alpha: np.ndarray
     LocA_alpha: np.ndarray
 
 
-class HOTAMetrics(MOTMetricBase):
-    def _calculate_hota_metrics(
-        self, ground_truth: Tracks, hypotheses: Tracks
-    ) -> HOTAResults:
-
-        alphas = np.arange(0.05, 0.96, 0.05)  # from 0.05 to 0.95 inclusive
-        all_frames = sorted(set(ground_truth.frames).intersection(hypotheses.frames))
-
-        gts = tuple(ground_truth.ids_count.keys())
-        gts_counts = tuple(ground_truth.ids_count.values())
-        gts_id_ind_dict = {_id: ind for ind, _id in enumerate(gts)}
-
-        hyps = tuple(hypotheses.ids_count.keys())
-        hyps_counts = tuple(hypotheses.ids_count.values())
-        hyps_id_ind_dict = {_id: ind for ind, _id in enumerate(hyps)}
-
-        n_gt, n_hyp = len(gts), len(hyps)
-        FP, FN = sum(hyps_counts), sum(gts_counts)
-
-        DetAs = np.zeros_like(alphas)
-        AssAs = np.zeros_like(alphas)
-        LocAs = np.zeros_like(alphas)
-
-        for a_ind, alpha in enumerate(alphas):
-            # The arrays should all have the shape [n_gt, n_hyp]
-            FPA_max = np.tile(hyps_counts, (n_gt, 1))
-            FNA_max = np.tile(gts_counts, (n_hyp, 1)).T
-            TPA_max_vals: t.Dict[t.Tuple[int, int], int] = co.defaultdict(int)
-
-            FPA, FNA = FPA_max.copy(), FNA_max.copy()
-            locs = 0.0  # Accumulator of similarities
-
-            # Do the optimisitc matching - allow multiple matches per gt/hyp in the
-            # same frame
-            for frame in all_frames:
-                dist_matrix = self._get_iou_frame(frame)
-
-                gt_frame_inds = [
-                    gts_id_ind_dict[_id] for _id in ground_truth[frame].ids
-                ]
-                hyp_frame_inds = [
-                    hyps_id_ind_dict[_id] for _id in hypotheses[frame].ids
-                ]
-
-                for row_ind, col_ind in np.argwhere(dist_matrix < alpha):
-                    TPA_max_vals[(gt_frame_inds[row_ind], hyp_frame_inds[col_ind])] += 1
-
-            TPA_max = sparse.create_coo_array(TPA_max_vals, (n_gt, n_hyp)).toarray()
-
-            # Compute optimistic A_max, to be used for actual matching
-            A_max = TPA_max / (FNA_max + FPA_max - TPA_max)
-
-            # Do the actual matching
-            TPA_vals: t.Dict[t.Tuple[int, int], int] = co.defaultdict(int)
-            for frame in all_frames:
-                dist_matrix = self._get_iou_frame(frame)
-                dist_cost = (1 - dist_matrix) * _EPS
-
-                gt_ids_f = ground_truth[frame].ids
-                hyp_ids_f = hypotheses[frame].ids
-                gt_frame_inds = [gts_id_ind_dict[_id] for _id in gt_ids_f]
-                hyp_frame_inds = [hyps_id_ind_dict[_id] for _id in hyp_ids_f]
-
-                opt_matrix = ((dist_matrix < alpha) / _EPS).astype(np.float64)
-                opt_matrix += A_max[np.ix_(gt_frame_inds, hyp_frame_inds)]
-                opt_matrix += dist_cost
-
-                # Calculate matching as a LAP
-                matching_inds = linear_sum_assignment(opt_matrix, maximize=True)
-                for row_ind, col_ind in zip(*matching_inds):
-                    if dist_matrix[row_ind, col_ind] < alpha:
-                        TPA_vals[(gt_frame_inds[row_ind], hyp_frame_inds[col_ind])] += 1
-                        locs += 1 - dist_matrix[row_ind, col_ind]
-
-            TPA = sparse.create_coo_array(TPA_vals, (n_gt, n_hyp)).toarray()
-
-            # Compute proper scores
-            TP = TPA.sum()
-            A = TPA / (FNA + FPA - TPA)
-            DetAs[a_ind] = TP / (FN + FP - TP)
-            AssAs[a_ind] = (TPA * A).sum() / max(TP, 1)
-
-            # If no matches -> full similarity [strange default]
-            LocAs[a_ind] = np.maximum(locs, 1e-10) / np.maximum(TP, 1e-10)
-
-        HOTAs = np.sqrt(DetAs * AssAs)
-
-        return {
-            "HOTA": HOTAs.mean(),
-            "DetA": DetAs.mean(),
-            "AssA": AssAs.mean(),
-            "LocA": LocAs.mean(),
-            "alphas_HOTA": alphas,
-            "HOTA_alpha": HOTAs,
-            "DetA_alpha": DetAs,
-            "AssA_alpha": AssAs,
-            "LocA_alpha": LocAs,
-        }
+def calculate_hota_metrics(
+    ground_truth: Tracks, hypotheses: Tracks, ious: dict[int, npt.NDArray[np.float32]]
+) -> HOTAResults:
+    """Calculate HOTA metrics.
+
+    Args:
+        ground_truth: Ground truth tracks.
+        hypotheses: Hypotheses tracks.
+        ious_threshold: A dictionary where keys are frame numbers (indices), and values
+            are numpy matrices of IOU distances between detection in ground truth and
+            hypotheses for that frame. IOUs must be present for all frames that are
+            present in both ground truth and hypotheses.
+
+    Returns:
+        A dictionary containing HOTA metrics (both average and individual alpha values).
+        Note that I use the matching algorithm from the paper, which differs from what
+        the official repository (TrackEval) is using - see
+        [this issue](https://github.com/JonathonLuiten/TrackEval/issues/22) for more
+        details. The metrics returned are:
+
+            - HOTA
+            - AssA
+            - DetA
+            - LocA
+    """
+
+    alphas = np.arange(0.05, 0.96, 0.05)  # from 0.05 to 0.95 inclusive
+    all_frames = sorted(set(ground_truth.frames).intersection(hypotheses.frames))
+
+    gts = tuple(ground_truth.ids_count.keys())
+    gts_counts = tuple(ground_truth.ids_count.values())
+    gts_id_ind_dict = {_id: ind for ind, _id in enumerate(gts)}
+
+    hyps = tuple(hypotheses.ids_count.keys())
+    hyps_counts = tuple(hypotheses.ids_count.values())
+    hyps_id_ind_dict = {_id: ind for ind, _id in enumerate(hyps)}
+
+    n_gt, n_hyp = len(gts), len(hyps)
+    FP, FN = sum(hyps_counts), sum(gts_counts)
+
+    DetAs = np.zeros_like(alphas)
+    AssAs = np.zeros_like(alphas)
+    LocAs = np.zeros_like(alphas)
+
+    for a_ind, alpha in enumerate(alphas):
+        # The arrays should all have the shape [n_gt, n_hyp]
+        FPA_max = np.tile(hyps_counts, (n_gt, 1))
+        FNA_max = np.tile(gts_counts, (n_hyp, 1)).T
+        TPA_max_vals: dict[tuple[int, int], int] = co.defaultdict(int)
+
+        FPA, FNA = FPA_max.copy(), FNA_max.copy()
+        locs = 0.0  # Accumulator of similarities
+
+        # Do the optimisitc matching - allow multiple matches per gt/hyp in the
+        # same frame
+        for frame in all_frames:
+            dist_matrix = ious[frame]
+
+            gt_frame_inds = [gts_id_ind_dict[_id] for _id in ground_truth[frame].ids]
+            hyp_frame_inds = [hyps_id_ind_dict[_id] for _id in hypotheses[frame].ids]
+
+            for row_ind, col_ind in np.argwhere(dist_matrix < alpha):
+                TPA_max_vals[(gt_frame_inds[row_ind], hyp_frame_inds[col_ind])] += 1
+
+        TPA_max = create_coo_array(TPA_max_vals, (n_gt, n_hyp)).toarray()
+
+        # Compute optimistic A_max, to be used for actual matching
+        A_max = TPA_max / (FNA_max + FPA_max - TPA_max)
+
+        # Do the actual matching
+        TPA_vals: dict[tuple[int, int], int] = co.defaultdict(int)
+        for frame in all_frames:
+            dist_matrix = ious[frame]
+            dist_cost = (1 - dist_matrix) * _EPS
+
+            gt_ids_f = ground_truth[frame].ids
+            hyp_ids_f = hypotheses[frame].ids
+            gt_frame_inds = [gts_id_ind_dict[_id] for _id in gt_ids_f]
+            hyp_frame_inds = [hyps_id_ind_dict[_id] for _id in hyp_ids_f]
+
+            opt_matrix = ((dist_matrix < alpha) / _EPS).astype(np.float64)
+            opt_matrix += A_max[np.ix_(gt_frame_inds, hyp_frame_inds)]
+            opt_matrix += dist_cost
+
+            # Calculate matching as a LAP
+            matching_inds = linear_sum_assignment(opt_matrix, maximize=True)
+            for row_ind, col_ind in zip(*matching_inds):
+                if dist_matrix[row_ind, col_ind] < alpha:
+                    TPA_vals[(gt_frame_inds[row_ind], hyp_frame_inds[col_ind])] += 1
+                    locs += 1 - dist_matrix[row_ind, col_ind]
+
+        TPA = create_coo_array(TPA_vals, (n_gt, n_hyp)).toarray()
+
+        # Compute proper scores
+        TP = TPA.sum()
+        A = TPA / (FNA + FPA - TPA)
+        DetAs[a_ind] = TP / (FN + FP - TP)
+        AssAs[a_ind] = (TPA * A).sum() / max(TP, 1)
+
+        # If no matches -> full similarity [strange default]
+        LocAs[a_ind] = np.maximum(locs, 1e-10) / np.maximum(TP, 1e-10)
+
+    HOTAs = np.sqrt(DetAs * AssAs)
+
+    return {
+        "HOTA": HOTAs.mean(),
+        "DetA": DetAs.mean(),
+        "AssA": AssAs.mean(),
+        "LocA": LocAs.mean(),
+        "alphas_HOTA": alphas,
+        "HOTA_alpha": HOTAs,
+        "DetA_alpha": DetAs,
+        "AssA_alpha": AssAs,
+        "LocA_alpha": LocAs,
+    }
```

### Comparing `evaldet-0.3.0/.gitignore` & `evaldet-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `evaldet-0.3.0/LICENSE` & `evaldet-0.4.0/LICENSE`

 * *Files identical despite different names*

