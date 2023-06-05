# Comparing `tmp/Pulse3D-0.33.6.tar.gz` & `tmp/Pulse3D-0.33.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.6.tar", last modified: Tue May 23 20:06:15 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.7.tar", last modified: Mon Jun  5 19:32:56 2023, max compression
```

## Comparing `Pulse3D-0.33.6.tar` & `Pulse3D-0.33.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.644726 Pulse3D-0.33.6/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.644726 Pulse3D-0.33.6/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.648726 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.644726 Pulse3D-0.33.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 20:06:15.000000 Pulse3D-0.33.6/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 20:06:15.000000 Pulse3D-0.33.6/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:05:57.000000 Pulse3D-0.33.6/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.648726 Pulse3D-0.33.6/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/nb_peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-05 19:31:36.000000 Pulse3D-0.33.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.071508 Pulse3D-0.33.7/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.067508 Pulse3D-0.33.7/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.071508 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-05 19:31:41.000000 Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.067508 Pulse3D-0.33.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-05 19:32:55.000000 Pulse3D-0.33.7/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-05 19:32:56.000000 Pulse3D-0.33.7/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:32:37.000000 Pulse3D-0.33.7/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.071508 Pulse3D-0.33.7/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-05 19:32:07.000000 Pulse3D-0.33.7/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:32:56.075508 Pulse3D-0.33.7/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33794 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-05 19:31:37.000000 Pulse3D-0.33.7/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.6/LICENSE` & `Pulse3D-0.33.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/PKG-INFO` & `Pulse3D-0.33.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.6
+Version: 0.33.7
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.6/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.7/mantarray-magnet-finding/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 """Setup configuration."""
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name="mantarray_magnet_finding",
-    version="0.5.1",
+    version="0.5.2",
     description="Magnet Finding",
     url="https://github.com/CuriBio/mantarray-magnet-finding",
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
         "nptyping==1.4.4",
         "numpy==1.23.4",  # Tanner (12/3/21): pinned for numba compatibility
         "scipy==1.9.3",
-        "numba==0.56.4",
+        "numba==0.57.0",
         "stdlib_utils>=0.4.4",
         "labware-domain-models>=0.3.1",
         "h5py>=3.7.0",
         "immutabledict>=2.2.1",
     ],
     zip_safe=False,
     include_package_data=True,
@@ -31,13 +31,14 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

### Comparing `Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.7/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/setup.py` & `Pulse3D-0.33.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.6",
+    version="0.33.7",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.6/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.7/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.6
+Version: 0.33.7
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.6/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.7/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.7/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.7/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.7/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/constants.py` & `Pulse3D-0.33.7/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.7/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/exceptions.py` & `Pulse3D-0.33.7/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.7/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/metrics.py` & `Pulse3D-0.33.7/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/nb_peak_detection.py` & `Pulse3D-0.33.7/src/pulse3D/nb_peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.7/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.7/src/pulse3D/plate_recording.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
                 zf = zipfile.ZipFile(path)
                 zf.extractall(path=tmpdir)
 
                 if glob.glob(os.path.join(tmpdir, "**", "*.h5"), recursive=True):
                     self.wells, calibration_recordings = load_files(
                         tmpdir, stiffness_factor, inverted_post_magnet_wells
                     )
-                elif xlsx_files := glob.glob(os.path.join(tmpdir, "*.xlsx"), recursive=True):
+                elif xlsx_files := glob.glob(os.path.join(tmpdir, "**", "*.xlsx"), recursive=True):
                     self._load_optical_well_files(xlsx_files, stiffness_factor)
         elif self.path.endswith(".xlsx"):  # optical file
             self._load_optical_well_files([self.path], stiffness_factor)
         else:  # .h5 files
             self.wells, calibration_recordings = load_files(
                 self.path, stiffness_factor, inverted_post_magnet_wells
             )
@@ -486,15 +486,15 @@
             stim_protocol = json.loads(wf[STIMULATION_PROTOCOL_UUID])
 
             try:
                 stim_sessions_waveforms = create_stim_session_waveforms(
                     stim_protocol["subprotocols"], wf[STIMULATION_READINGS], start_time_us, end_time_us
                 )
             except SubprotocolFormatIncompatibleWithInterpolationError:
-                log.info("Subprotocol format not supported by intperpolation")
+                log.exception("Subprotocol format not supported by interpolation")
                 return
 
             is_voltage = stim_protocol["stimulation_type"] == "V"
             charge_conversion_factor = 1 if is_voltage else MILLI_TO_BASE_CONVERSION
 
             for waveform in stim_sessions_waveforms:
                 if not waveform.shape[-1]:
@@ -516,14 +516,15 @@
         except KeyError:
             stim_timepoints = None
 
         for wf in self.wells:
             well_name = wf[WELL_NAME_UUID]
             raw_force_amplitudes = df[f"{well_name}__raw"]
             wf.force = np.vstack((force_timepoints, raw_force_amplitudes)).astype(np.float64)
+            wf.force = wf.force[:, ~np.isnan(raw_force_amplitudes)]
 
             if stim_timepoints is None:
                 continue
 
             stim_col_titles = sorted([col for col in df if f"{well_name}__stim" in col])
 
             for col_title in stim_col_titles:
```

### Comparing `Pulse3D-0.33.6/src/pulse3D/plotting.py` & `Pulse3D-0.33.7/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/stimulation.py` & `Pulse3D-0.33.7/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/transforms.py` & `Pulse3D-0.33.7/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.6/src/pulse3D/utils.py` & `Pulse3D-0.33.7/src/pulse3D/utils.py`

 * *Files identical despite different names*

