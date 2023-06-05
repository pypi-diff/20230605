# Comparing `tmp/keypoint-moseq-0.1.3.tar.gz` & `tmp/keypoint-moseq-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.1.3.tar", last modified: Fri May 19 14:10:19 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.1.4.tar", last modified: Mon Jun  5 19:18:44 2023, max compression
```

## Comparing `keypoint-moseq-0.1.3.tar` & `keypoint-moseq-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-19 14:10:19.455508 keypoint-moseq-0.1.3/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.3/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.3/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-19 14:10:19.455619 keypoint-moseq-0.1.3/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.3/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-19 14:10:19.456438 keypoint-moseq-0.1.3/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-19 14:10:19.456518 keypoint-moseq-0.1.3/keypoint_moseq/_version.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.3/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17318 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.3/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    41843 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.3/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    27401 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    68264 2023-05-19 14:06:57.000000 keypoint-moseq-0.1.3/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-19 14:10:19.455263 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-05-19 14:10:19.456155 keypoint-moseq-0.1.3/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.3/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-05 19:18:44.252938 keypoint-moseq-0.1.4/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.4/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.4/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-05 19:18:44.253141 keypoint-moseq-0.1.4/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.4/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-05 19:18:44.254788 keypoint-moseq-0.1.4/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-06-05 19:18:44.254916 keypoint-moseq-0.1.4/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17701 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17249 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    46339 2023-06-05 19:18:09.000000 keypoint-moseq-0.1.4/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    27260 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    68264 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-05 19:18:44.252365 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-06-05 19:18:44.254352 keypoint-moseq-0.1.4/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.4/versioneer.py
```

### Comparing `keypoint-moseq-0.1.3/LICENSE.md` & `keypoint-moseq-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.3/NOTICE.md` & `keypoint-moseq-0.1.4/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.3/README.md` & `keypoint-moseq-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.3/keypoint_moseq/__init__.py` & `keypoint-moseq-0.1.4/keypoint_moseq/__init__.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.3/keypoint_moseq/analysis.py` & `keypoint-moseq-0.1.4/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.3/keypoint_moseq/calibration.py` & `keypoint-moseq-0.1.4/keypoint_moseq/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,54 +251,56 @@
             toolbar=None, default_tools=[], 
             xlabel='log10(confidence)', ylabel='log10(error)')
 
 
     def update_img(crop_size, sample_ix, x, y):
         
         key,frame,bodypart = sample_key = sample_keys[sample_ix]
+        image = sample_images[sample_key]
+        h,w = image.shape[:2]
+
         keypoint_ix = bodyparts.index(bodypart)
-        xys = coordinates[key][frame]
+        xys = coordinates[key][frame].copy()
+        xys[:,1] = h-xys[:,1]
         masked_nodes = np.nonzero(~np.isnan(xys).any(1))[0]
         confs = confidences[key][frame]
         
         if x and y:
-            annotations_stream.annotations.update({sample_key:(x,y)})
+            annotations_stream.annotations.update({sample_key:(x,h-y)})
             annotations_stream.event()
 
         if sample_key in annotations_stream.annotations: 
             point = np.array(annotations_stream.annotations[sample_key])
+            point[1] = h-point[1]
         else: point = xys[keypoint_ix]
           
         colorvals = np.linspace(0,1,len(bodyparts))
         pt_data = np.append(point,colorvals[keypoint_ix])[None]
         hv_point = hv.Points(pt_data, vdims=['bodypart']).opts(
             color='bodypart', cmap='autumn', size=15, framewise=True, marker='x', line_width=3)
         
         label = f'{bodypart}, confidence = {confs[keypoint_ix]:.5f}'
-        h,w = sample_images[sample_key].shape[:2]
-        rgb = hv.RGB(sample_images[sample_key], bounds=(0,2*h,w,h), label=label).opts(
+        rgb = hv.RGB(image, bounds=(0,0,w,h), label=label).opts(
             framewise=True, xaxis='bare', yaxis='bare', frame_width=250)
 
         xlim = (xys[keypoint_ix,0]-crop_size/2,xys[keypoint_ix,0]+crop_size/2)
         ylim = (xys[keypoint_ix,1]-crop_size/2,xys[keypoint_ix,1]+crop_size/2)
          
         edge_data = ((),(),())
         if len(edges)>0: 
             masked_edges = edges[np.isin(edges,masked_nodes).all(1)]
             if len(masked_edges)>0:
                 edge_data = (*masked_edges.T, colorvals[masked_edges[:,0]])
 
-                    
         sizes = np.where(np.arange(len(xys))==keypoint_ix, 10, 6)[masked_nodes]
         masked_bodyparts = [bodyparts[i] for i in masked_nodes]
         nodes = hv.Nodes((*xys[masked_nodes].T, masked_nodes, masked_bodyparts, sizes), vdims=['name','size'])        
         graph = hv.Graph((edge_data, nodes), vdims='ecolor').opts(
             node_color='name', node_cmap=keypoint_colormap, tools=[],
-            edge_color='ecolor', edge_cmap=keypoint_colormap, 
-            node_size='size',  invert_yaxis=True)
+            edge_color='ecolor', edge_cmap=keypoint_colormap, node_size='size')
 
         return (rgb*graph*hv_point).opts(data_aspect=1, xlim=xlim, ylim=ylim, toolbar=None)
     
     
     def update_estimator_text(*, slope, intercept, conf_threshold):
         lines = [f'slope: {slope:.6f}',
                  f'intercept: {intercept:.6f}',
```

### Comparing `keypoint-moseq-0.1.3/keypoint_moseq/fitting.py` & `keypoint-moseq-0.1.4/keypoint_moseq/fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import joblib
 import os
 import numpy as np
 import tqdm
 import jax
 import warnings
 from textwrap import fill
 from datetime import datetime
 
 from keypoint_moseq.viz import plot_progress
 from keypoint_moseq.io import save_checkpoint, format_data, save_hdf5
-from keypoint_moseq.util import get_durations, get_frequencies, pad_along_axis, reindex_by_frequency
+from keypoint_moseq.util import reindex_by_frequency
 from jax_moseq.models.keypoint_slds import estimate_coordinates, resample_model, init_model
-from jax_moseq.utils import check_for_nans, batch, unbatch
+from jax_moseq.utils import check_for_nans, unbatch
 
 class StopResampling(Exception):
     pass
 
 def _update_history(history, iteration, model, include_states=True): 
     
     model_snapshot = {
```

### Comparing `keypoint-moseq-0.1.3/keypoint_moseq/io.py` & `keypoint-moseq-0.1.4/keypoint_moseq/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 import numpy as np
 import warnings
 import h5py
 import joblib
 import tqdm
 import yaml
 import os
-import cv2
 import re
 import pandas as pd
 from datetime import datetime
 from textwrap import fill
-from vidio.read import OpenCVReader
 import matplotlib.pyplot as plt
 import tabulate
 
 
 from jax_moseq.utils import batch
 from keypoint_moseq.util import (
     reindex_by_bodyparts, 
@@ -859,37 +857,61 @@
                  '{}% of frames:\n - {}\n\n'.format(warning_threshold*100, '\n - '.join(bps)))
             warnings.warn(
                 'This may cause problems during modeling. See '
                 'https://keypoint-moseq.readthedocs.io/en/latest/FAQs.html#high-proportion-of-nans'
                 ' for additional information.')
 
 
-
-def load_deeplabcut_results(filepath_pattern, recursive=True, path_sep='-',
-                            path_in_name=False, remove_extension=True):
+def load_keypoints(filepath_pattern, format, recursive=True, path_sep='-',
+                   path_in_name=False, remove_extension=True):
     """
-    Load tracking results from deeplabcut csv or hdf5 files.
+    Load keypoint tracking results from one or more files. Several file
+    formats are supported:
 
-    For single-animal tracking, each file yields a single key/value 
-    pair in the returned `coordinates` and `confidences` dictionaries. For
-    multi-animal tracking, a key/vaue pair will be generated for each
-    tracked individual. For example a single file called `two_mice.h5`
-    with individuals "mouseA" and "mouseB" will yield the pair of
-    keys `'two_mice_mouseA', 'two_mice_mouseB'`. 
+    - deeplabcut
+        .csv and .h5/.hdf5 files generated by deeplabcut. For single-animal
+        tracking, each file yields a single key/value pair in the returned 
+        `coordinates` and `confidences` dictionaries. For multi-animal tracking, 
+        a key/vaue pair will be generated for each tracked individual. For 
+        example the file `two_mice.h5` with individuals "mouseA" and "mouseB" 
+        will yield the pair of keys `'two_mice_mouseA', 'two_mice_mouseB'`. 
+
+    - sleap
+        .h5/.hdf5 files generated by sleap. For single-animal tracking, each
+        file yields a single key/value pair in the returned `coordinates` and
+        `confidences` dictionaries. For multi-animal tracking, a key/vaue pair 
+        will be generated for each track. For example a single file called 
+        `two_mice.h5` will yield the pair of keys `'two_mice_track0', 
+        'two_mice_track1'`.   
+
+    - anipose
+        .csv files generated by anipose. Each file should contain five columns
+        per keypoint (x,y,z,error,score), plus a last column with the frame number.
+        The `score` column is used as the keypoint confidence. 
+
+    - anipose-sleap
+        .h5/.hdf5 files generated by anipose-sleap. Each file should contain 
+        a dataset called `'tracks'` with shape (n_frames, 1, n_keypoints, 3).
+        If there is also a `'point_scores'` dataset, it will be used as the
+        keypoint confidence. Otherwise, the confidence will be set to 1.
 
     Parameters
     ----------
     filepath_pattern: str or list of str
         Filepath pattern for a set of deeplabcut csv or hdf5 files, 
         or a list of such patterns. Filepath patterns can be:
 
-            - single file (e.g. `/path/to/file.csv`) 
-            - single directory (e.g. `/path/to/dir/`)
-            - set of files (e.g. `/path/to/fileprefix*`)
-            - set of directories (e.g. `/path/to/dirprefix*`)
+        - single file (e.g. `/path/to/file.csv`) 
+        - single directory (e.g. `/path/to/dir/`)
+        - set of files (e.g. `/path/to/fileprefix*`)
+        - set of directories (e.g. `/path/to/dirprefix*`)
+
+    format: str
+        Format of the files to load. Must be one of `'deeplabcut'`, 
+        `'sleap'`, `'anipose'`, or `'anipose-sleap'`.
 
     recursive: bool, default=True
         Whether to search recursively for deeplabcut csv or hdf5 files.
 
     path_in_name: bool, default=False
         Whether to name the tracking results from each file by the path
         to the file (True) or just the filename (False). If True, the
@@ -899,59 +921,179 @@
         Separator to use when `path_in_name` is True. For example,
         if `path_sep` is `'-'`, then the tracking results from the
         file `/path/to/file.csv` will be named `path-to-file`. Using
         `'/'` as the separator is discouraged, as it will cause problems
         saving/loading the modeling results to/from hdf5 files.
 
     remove_extension: bool, default=True
-        Whether to remove the file extension from the name of the tracking
-        results.
+        Whether to remove the file extension when naming the tracking
+        results from each file.
 
     Returns
     -------
     coordinates: dict
         Dictionary mapping filenames to keypoint coordinates as ndarrays
-        of shape (n_frames, n_bodyparts, 2)
+        of shape (n_frames, n_bodyparts, 2[or 3])
 
     confidences: dict
         Dictionary mapping filenames to `likelihood` scores as ndarrays
         of shape (n_frames, n_bodyparts)
 
     bodyparts: list of str
         List of bodypart names. The order of the names matches the order
         of the bodyparts in `coordinates` and `confidences`.
     """
+    formats = ['deeplabcut', 'sleap', 'anipose', 'anipose-sleap']
+    assert format in formats, fill(
+        f'Unrecognized format {format}. Must be one of {formats}')
+    
+    extensions = {
+        'deeplabcut': ['.csv','.h5','.hdf5'],
+        'sleap': ['.h5','.hdf5'],
+        'anipose': ['.csv'],
+        'anipose-sleap': ['.h5','.hdf5']
+    }[format]
+
+    loader = {
+        'deeplabcut': _deeplabcut_loader,
+        'sleap': _sleap_loader,
+        'anipose': _anipose_loader,
+        'anipose-sleap': _anipose_sleap_loader
+    }[format]
+
+    filepaths = list_files_with_exts(
+        filepath_pattern, extensions, recursive=recursive)
+    assert len(filepaths)>0, fill(
+        f'No files with extensions {extensions} found for {filepath_pattern}')
+    
+    coordinates,confidences = {},{}
+    for filepath in tqdm.tqdm(filepaths, desc=f'Loading keypoints'):
+        try:
+            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
+            new_coordinates,new_confidences,bodyparts = loader(filepath, name)
+            coordinates.update(new_coordinates)
+            confidences.update(new_confidences)
+        except Exception as e:
+            print(fill(f'Error loading {filepath}: {e}'))
+
+    if len(coordinates) > 0:
+        check_nan_proportions(coordinates, bodyparts)
+    return coordinates,confidences,bodyparts
+
+
+def _deeplabcut_loader(filepath, name):
+    """Load tracking results from deeplabcut csv or hdf5 files."""
+    ext = os.path.splitext(filepath)[1]
+    if ext=='.h5': df = pd.read_hdf(filepath)
+    if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
+
+    coordinates,confidences = {},{}
+    bodyparts = df.columns.get_level_values('bodyparts').unique().tolist()
+    if 'individuals' in df.columns.names:
+        for ind in df.columns.get_level_values('individuals').unique():
+            ind_df = df.xs(ind, axis=1, level='individuals')
+            arr = ind_df.to_numpy().reshape(len(ind_df), -1, 3)
+            coordinates[f'{name}_{ind}'] = arr[:,:,:-1]
+            confidences[f'{name}_{ind}'] = arr[:,:,-1]
+    else:
+        arr = df.to_numpy().reshape(len(df), -1, 3)
+        coordinates[name] = arr[:,:,:-1]
+        confidences[name] = arr[:,:,-1]
+
+    return coordinates,confidences,bodyparts
+
+
+def _sleap_loader(filepath, name):
+    """Load keypoints from sleap hdf5 files."""
+    with h5py.File(filepath, 'r') as f:
+        coords = f['tracks'][()]
+        confs = f['point_scores'][()]
+        bodyparts = [name.decode('utf-8') for name in f['node_names']]
+        if coords.shape[0] == 1: 
+            coordinates = {name: coords[0].T}
+            confidences = {name: confs[0].T}
+        else:
+            coordinates = {f'{name}_track{i}': coords[i].T for i in range(coords.shape[0])}
+            confidences = {f'{name}_track{i}': confs[i].T for i in range(coords.shape[0])}
+    return coordinates,confidences,bodyparts
+
+
+def _anipose_loader(filepath, name):
+    """Load keypoints from anipose csv files."""
+    df = pd.read_csv(filepath,)
+    bodyparts = [n.split('_x')[0] for n in df.columns[:-1][::5]] 
+    arr = df.to_numpy()[:,:-1].reshape(len(df), len(bodyparts), 5)
+    coordinates = {name: arr[:,:,:3]}
+    confidences = {name: arr[:,:,4]}
+    return coordinates,confidences,bodyparts
+
+
+def _anipose_sleap_loader(filepath, name):
+    """Load keypoints from anipose-sleap hdf5 files."""
+    with h5py.File(filepath, 'r') as f:
+        coords = f['tracks'][()]
+        if 'point_scores' in f.keys():
+            confs = f['point_scores'][()]
+        else:
+            confs = np.ones_like(coords[...,0])
+        bodyparts = ['bodypart{}'.format(i) for i in range(coords.shape[2])]
+        coordinates = {name: coords[0].T}
+        confidences = {name: confs[0].T}
+    return coordinates,confidences,bodyparts
+
+
+
+def load_deeplabcut_results(filepath_pattern, recursive=True, path_sep='-',
+                            path_in_name=False, remove_extension=True):
+    """
+    Load tracking results from deeplabcut csv or hdf5 files.
+
+    For single-animal tracking, each file yields a single key/value 
+    pair in the returned `coordinates` and `confidences` dictionaries. For
+    multi-animal tracking, a key/vaue pair will be generated for each
+    tracked individual. For example a single file called `two_mice.h5`
+    with individuals "mouseA" and "mouseB" will yield the pair of
+    keys `'two_mice_mouseA', 'two_mice_mouseB'`. 
+
+    See :py:func:`keypoint_moseq.io.load_keypoints` for a description of 
+    the parameters and return values.
+    """
+    warnings.warn(
+        'WARNING: This `load_deeplabcut_results` is being deprecated. '
+        ' Use `load_keypoints` instead.\n\n')
+    
     filepaths = list_files_with_exts(
         filepath_pattern, ['.csv','.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No deeplabcut csv or hdf5 files found for {filepath_pattern}')
 
     coordinates,confidences = {},{}
     for filepath in tqdm.tqdm(filepaths, desc='Loading from deeplabcut'):
+        
+        try:
+            ext = os.path.splitext(filepath)[1]
+            if ext=='.h5': df = pd.read_hdf(filepath)
+            if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
+            
+            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
+            bodyparts = df.columns.get_level_values('bodyparts').unique().tolist()   
+            
+            if 'individuals' in df.columns.names:
+                for ind in df.columns.get_level_values('individuals').unique():
+                    ind_df = df.xs(ind, axis=1, level='individuals')
+                    arr = ind_df.to_numpy().reshape(len(ind_df), -1, 3)
+                    coordinates[f'{name}_{ind}'] = arr[:,:,:-1]
+                    confidences[f'{name}_{ind}'] = arr[:,:,-1]
+            else:
+                arr = df.to_numpy().reshape(len(df), -1, 3)
+                coordinates[name] = arr[:,:,:-1]
+                confidences[name] = arr[:,:,-1]
 
-        ext = os.path.splitext(filepath)[1]
-        if ext=='.h5': df = pd.read_hdf(filepath)
-        if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
-        
-        name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
-        bodyparts = df.columns.get_level_values('bodyparts').unique().tolist()   
-        
-        if 'individuals' in df.columns.names:
-            for ind in df.columns.get_level_values('individuals').unique():
-                ind_df = df.xs(ind, axis=1, level='individuals')
-                arr = ind_df.to_numpy().reshape(len(ind_df), -1, 3)
-                coordinates[f'{name}_{ind}'] = arr[:,:,:-1]
-                confidences[f'{name}_{ind}'] = arr[:,:,-1]
-        else:
-            arr = df.to_numpy().reshape(len(df), -1, 3)
-            coordinates[name] = arr[:,:,:-1]
-            confidences[name] = arr[:,:,-1]
-
-        # except Exception as e: 
-        #     print(fill(f'Error loading {filepath}: {e}'))
+        except Exception as e: 
+            print(fill(f'Error loading {filepath}: {e}'))
     
     if len(coordinates) > 0:
         check_nan_proportions(coordinates, bodyparts)
 
     return coordinates,confidences,bodyparts
 
 
@@ -963,58 +1105,21 @@
 
     For single-animal tracking, each file yields a single key/value 
     pair in the returned `coordinates` and `confidences` dictionaries. For
     multi-animal tracking, a key/vaue pair will be generated for each track.
     For example a single file called `two_mice.h5` will yield the pair of
     keys `'two_mice_track0', 'two_mice_track1'`.
 
-    Parameters
-    ----------
-    filepath_pattern: str, default=None
-        Filepath pattern for a set of sleap hdf5 files, or a list of 
-        such patterns. Filepath patterns can be:
-
-            - single file (e.g. `/path/to/file.csv`) 
-            - single directory (e.g. `/path/to/dir/`)
-            - set of files (e.g. `/path/to/fileprefix*`)
-            - set of directories (e.g. `/path/to/dirprefix*`)
-
-    recursive: bool, default=True
-        Whether to search recursively for sleap hdf5 files.
-
-    path_in_name: bool, default=False
-        Whether to name the tracking results from each file by the path
-        to the file (True) or just the filename (False). If True, the
-        `path_sep` argument is used to separate the path components.
-        
-    path_sep: str, default='-'
-        Separator to use when `path_in_name` is True. For example,
-        if `path_sep` is `'-'`, then the tracking results from the
-        file `/path/to/file.csv` will be named `path-to-file`. Using
-        `'/'` as the separator is discouraged, as it will cause problems
-        saving/loading the modeling results to/from hdf5 files.
-
-    remove_extension: bool, default=True
-        Whether to remove the file extension from the name of the tracking
-        results.
-
-    Returns
-    -------
-    coordinates: dict
-        Dictionary mapping filenames to keypoint coordinates as ndarrays
-        of shape (n_frames, n_bodyparts, 2)
-
-    confidences: dict
-        Dictionary mapping filenames to `likelihood` scores as ndarrays
-        of shape (n_frames, n_bodyparts)
-
-    bodyparts: list of str
-        List of bodypart names. The order of the names matches the order
-        of the bodyparts in `coordinates` and `confidences`.
+    See :py:func:`keypoint_moseq.io.load_keypoints` for a description of 
+    the parameters and return values.
     """
+    warnings.warn(
+        'WARNING: This `load_sleap_results` is being deprecated. '
+        ' Use `load_keypoints` instead.\n\n')
+    
     filepaths = list_files_with_exts(
         filepath_pattern, ['.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No sleap hdf5 files found for {filepath_pattern}.')
 
     coordinates,confidences = {},{}
     for filepath in tqdm.tqdm(filepaths, desc='Loading from sleap'):
@@ -1035,17 +1140,25 @@
             print(fill(f'Error loading {filepath}: {e}'))
 
     if len(coordinates) > 0:
         check_nan_proportions(coordinates, bodyparts)
 
     return coordinates,confidences,bodyparts
 
+
+
+
+
+
+
+
+
+
 # hdf5 save/load routines modified from
 # https://gist.github.com/nirum/b119bbbd32d22facee3071210e08ecdf
-
 def save_hdf5(filepath, save_dict):
     """
     Save a dict of pytrees to an hdf5 file.
     
     Parameters
     ----------
     filepath: str
```

### Comparing `keypoint-moseq-0.1.3/keypoint_moseq/util.py` & `keypoint-moseq-0.1.4/keypoint_moseq/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import numpy as np
 import os
 import glob
 import tqdm
 import warnings
 from textwrap import fill
-import jax, jax.numpy as jnp, jax.random as jr
-from jax.tree_util import tree_map
+import jax, jax.numpy as jnp
 from itertools import groupby
-from functools import partial
 from scipy.ndimage import median_filter, convolve1d
 from sklearn.decomposition import PCA
 from sklearn.neighbors import NearestNeighbors
-from jaxlib.xla_extension import DeviceArray as jax_array
 from jax_moseq.models.keypoint_slds import inverse_rigid_transform
 na = jnp.newaxis
 
 
 def np_io(fn): 
     """
     Converts a function involving jax arrays to one that inputs and
```

### Comparing `keypoint-moseq-0.1.3/keypoint_moseq/viz.py` & `keypoint-moseq-0.1.4/keypoint_moseq/viz.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.3/setup.cfg` & `keypoint-moseq-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.3/versioneer.py` & `keypoint-moseq-0.1.4/versioneer.py`

 * *Files identical despite different names*

