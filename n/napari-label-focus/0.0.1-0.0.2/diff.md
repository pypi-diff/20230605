# Comparing `tmp/napari-label-focus-0.0.1.tar.gz` & `tmp/napari-label-focus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-label-focus-0.0.1.tar", last modified: Mon Jun  5 08:55:16 2023, max compression
+gzip compressed data, was "napari-label-focus-0.0.2.tar", last modified: Mon Jun  5 10:07:14 2023, max compression
```

## Comparing `napari-label-focus-0.0.1.tar` & `napari-label-focus-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 08:55:16.837332 napari-label-focus-0.0.1/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1490 2023-05-24 09:58:04.000000 napari-label-focus-0.0.1/LICENSE
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       96 2023-05-24 09:58:04.000000 napari-label-focus-0.0.1/MANIFEST.in
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-05 08:55:16.837332 napari-label-focus-0.0.1/PKG-INFO
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1702 2023-06-01 14:15:18.000000 napari-label-focus-0.0.1/README.md
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      178 2023-06-01 14:12:18.000000 napari-label-focus-0.0.1/pyproject.toml
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1457 2023-06-05 08:55:16.837332 napari-label-focus-0.0.1/setup.cfg
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 08:55:16.837332 napari-label-focus-0.0.1/src/
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 08:55:16.837332 napari-label-focus-0.0.1/src/napari_label_focus/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       89 2023-05-25 16:10:58.000000 napari-label-focus-0.0.1/src/napari_label_focus/__init__.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     3785 2023-05-25 17:08:22.000000 napari-label-focus-0.0.1/src/napari_label_focus/_table.py
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 08:55:16.837332 napari-label-focus-0.0.1/src/napari_label_focus/_tests/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-05-24 09:58:04.000000 napari-label-focus-0.0.1/src/napari_label_focus/_tests/__init__.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      352 2023-06-01 14:10:17.000000 napari-label-focus-0.0.1/src/napari_label_focus/_tests/test_widget.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1812 2023-05-25 17:06:37.000000 napari-label-focus-0.0.1/src/napari_label_focus/_widget.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      276 2023-05-25 16:11:06.000000 napari-label-focus-0.0.1/src/napari_label_focus/napari.yaml
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 08:55:16.837332 napari-label-focus-0.0.1/src/napari_label_focus.egg-info/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-05 08:55:16.000000 napari-label-focus-0.0.1/src/napari_label_focus.egg-info/PKG-INFO
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      556 2023-06-05 08:55:16.000000 napari-label-focus-0.0.1/src/napari_label_focus.egg-info/SOURCES.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        1 2023-06-05 08:55:16.000000 napari-label-focus-0.0.1/src/napari_label_focus.egg-info/dependency_links.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       70 2023-06-05 08:55:16.000000 napari-label-focus-0.0.1/src/napari_label_focus.egg-info/entry_points.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      114 2023-06-05 08:55:16.000000 napari-label-focus-0.0.1/src/napari_label_focus.egg-info/requires.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       19 2023-06-05 08:55:16.000000 napari-label-focus-0.0.1/src/napari_label_focus.egg-info/top_level.txt
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1490 2023-05-24 09:58:04.000000 napari-label-focus-0.0.2/LICENSE
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       96 2023-05-24 09:58:04.000000 napari-label-focus-0.0.2/MANIFEST.in
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/PKG-INFO
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1702 2023-06-01 14:15:18.000000 napari-label-focus-0.0.2/README.md
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      178 2023-06-01 14:12:18.000000 napari-label-focus-0.0.2/pyproject.toml
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1457 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/setup.cfg
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/napari_label_focus/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       89 2023-05-25 16:10:58.000000 napari-label-focus-0.0.2/src/napari_label_focus/__init__.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     3889 2023-06-05 09:59:24.000000 napari-label-focus-0.0.2/src/napari_label_focus/_table.py
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/napari_label_focus/_tests/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-05-24 09:58:04.000000 napari-label-focus-0.0.2/src/napari_label_focus/_tests/__init__.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      352 2023-06-01 14:10:17.000000 napari-label-focus-0.0.2/src/napari_label_focus/_tests/test_widget.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1908 2023-06-05 09:53:47.000000 napari-label-focus-0.0.2/src/napari_label_focus/_widget.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      276 2023-05-25 16:11:06.000000 napari-label-focus-0.0.2/src/napari_label_focus/napari.yaml
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/PKG-INFO
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      556 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/SOURCES.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        1 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/dependency_links.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       70 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/entry_points.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      114 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/requires.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       19 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/top_level.txt
```

### Comparing `napari-label-focus-0.0.1/LICENSE` & `napari-label-focus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-label-focus-0.0.1/PKG-INFO` & `napari-label-focus-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-label-focus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Easily focus the view on selected elements form a Labels layer.
 Home-page: https://github.com/MalloryWittwer/napari-label-focus.git
 Author: Mallory Wittwer
 Author-email: mallory.wittwer@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-label-focus-0.0.1/README.md` & `napari-label-focus-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-label-focus-0.0.1/setup.cfg` & `napari-label-focus-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-label-focus
-version = 0.0.1
+version = 0.0.2
 description = Easily focus the view on selected elements form a Labels layer.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MalloryWittwer/napari-label-focus.git
 author = Mallory Wittwer
 author_email = mallory.wittwer@epfl.ch
 license = BSD-3-Clause
```

### Comparing `napari-label-focus-0.0.1/src/napari_label_focus/_table.py` & `napari-label-focus-0.0.2/src/napari_label_focus/_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,23 +85,26 @@
             self._view.setHorizontalHeaderItem(1, QTableWidgetItem('volume'))
             return
 
         labels = self._layer.data
         if labels.sum() == 0:
             return
         
+        if len(labels.shape) == 2:
+            labels = labels[None]  # Add an extra dimension
+        
         properties = skimage.measure.regionprops_table(labels, properties=["label", "area", "bbox"])
         df = pd.DataFrame.from_dict(properties)
         df.rename(columns={"area": "volume"}, inplace=True)
         df.sort_values(by="volume", ascending=False, inplace=True)
         self.set_content(df)
 
     def set_content(self, df: pd.DataFrame):
         self._table = df
         self._view.clear()
         self._view.setRowCount(len(self._table))
         self._view.setHorizontalHeaderItem(0, QTableWidgetItem('label'))
         self._view.setHorizontalHeaderItem(1, QTableWidgetItem('volume'))
 
         for i, (lab, vol) in self._table[['label', 'volume']].iterrows():
-            self._view.setItem(0, i, QTableWidgetItem(str(lab)))
-            self._view.setItem(1, i, QTableWidgetItem(str(vol)))
+            self._view.setItem(i, 0, QTableWidgetItem(str(lab)))
+            self._view.setItem(i, 1, QTableWidgetItem(str(vol)))
```

### Comparing `napari-label-focus-0.0.1/src/napari_label_focus/_widget.py` & `napari-label-focus-0.0.2/src/napari_label_focus/_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self.viewer.layers.events.removed.connect(self._on_layer_change)
         self.viewer.layers.events.removed.connect(self._on_layer_remove)
         self._on_layer_change(None)
 
     def _add_rename_event(self, e):
         source_layer = e.value
         source_layer.events.name.connect(lambda _: self._on_layer_change(None))
+        source_layer.events.set_data.connect(lambda _: self.table.update_content(source_layer))
 
     def _on_layer_change(self, e):
         self.cb.clear()
         for x in self.viewer.layers:
             if isinstance(x, napari.layers.Labels):
                 self.cb.addItem(x.name, x.data)
```

### Comparing `napari-label-focus-0.0.1/src/napari_label_focus.egg-info/PKG-INFO` & `napari-label-focus-0.0.2/src/napari_label_focus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-label-focus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Easily focus the view on selected elements form a Labels layer.
 Home-page: https://github.com/MalloryWittwer/napari-label-focus.git
 Author: Mallory Wittwer
 Author-email: mallory.wittwer@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-label-focus-0.0.1/src/napari_label_focus.egg-info/SOURCES.txt` & `napari-label-focus-0.0.2/src/napari_label_focus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

