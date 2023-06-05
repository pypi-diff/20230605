# Comparing `tmp/PyArrShow-1.0.7.tar.gz` & `tmp/PyArrShow-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyArrShow-1.0.7.tar", last modified: Mon Jun  5 09:19:13 2023, max compression
+gzip compressed data, was "PyArrShow-1.0.8.tar", last modified: Mon Jun  5 10:24:07 2023, max compression
```

## Comparing `PyArrShow-1.0.7.tar` & `PyArrShow-1.0.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:19:13.939046 PyArrShow-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-06-05 09:19:13.841306 PyArrShow-1.0.7/.vscode/
--rw-rw-rw-   0        0        0      510 2023-06-02 11:52:15.000000 PyArrShow-1.0.7/.vscode/launch.json
--rw-rw-rw-   0        0        0     1088 2023-06-02 11:52:15.000000 PyArrShow-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1868 2023-06-05 09:19:13.938049 PyArrShow-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 09:19:13.851279 PyArrShow-1.0.7/PyArrShow.egg-info/
--rw-rw-rw-   0        0        0     1868 2023-06-05 09:19:13.000000 PyArrShow-1.0.7/PyArrShow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2023-06-05 09:19:13.000000 PyArrShow-1.0.7/PyArrShow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:19:13.000000 PyArrShow-1.0.7/PyArrShow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-05 09:19:13.000000 PyArrShow-1.0.7/PyArrShow.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-06-05 09:19:13.000000 PyArrShow-1.0.7/PyArrShow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-05 09:19:13.000000 PyArrShow-1.0.7/PyArrShow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1323 2023-06-05 09:11:30.000000 PyArrShow-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 09:19:13.853274 PyArrShow-1.0.7/__pycache__/
--rw-rw-rw-   0        0        0      219 2023-06-02 11:52:15.000000 PyArrShow-1.0.7/__pycache__/__init__.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-06-05 09:19:13.872223 PyArrShow-1.0.7/pyas/
--rw-rw-rw-   0        0        0     5088 2023-05-30 01:48:38.000000 PyArrShow-1.0.7/pyas/DataCursorFrame.py
--rw-rw-rw-   0        0        0     3605 2023-05-05 11:35:48.000000 PyArrShow-1.0.7/pyas/ImgDisplayFrame.py
--rw-rw-rw-   0        0        0    13988 2023-05-06 08:42:19.000000 PyArrShow-1.0.7/pyas/PilotFrame.py
--rw-rw-rw-   0        0        0      169 2023-06-05 04:06:31.000000 PyArrShow-1.0.7/pyas/__init__.py
--rw-rw-rw-   0        0        0     1055 2023-06-05 08:04:54.000000 PyArrShow-1.0.7/pyas/__main__.py
--rw-rw-rw-   0        0        0    19356 2023-06-05 04:06:27.000000 PyArrShow-1.0.7/pyas/controller.py
--rw-rw-rw-   0        0        0    47850 2023-06-05 02:12:58.000000 PyArrShow-1.0.7/pyas/main_backup.py
--rw-rw-rw-   0        0        0    17671 2023-06-05 02:06:47.000000 PyArrShow-1.0.7/pyas/model.py
--rw-rw-rw-   0        0        0    67984 2023-05-29 12:06:03.000000 PyArrShow-1.0.7/pyas/qrc_resources.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:19:13.937051 PyArrShow-1.0.7/pyas/resources/
--rw-rw-rw-   0        0        0    44264 2023-04-27 02:48:45.000000 PyArrShow-1.0.7/pyas/resources/About_logo.jpg
--rw-rw-rw-   0        0        0     5697 2023-04-28 09:46:12.000000 PyArrShow-1.0.7/pyas/resources/PyAs_main_window.svg
--rw-rw-rw-   0        0        0      893 2023-04-27 01:46:15.000000 PyArrShow-1.0.7/pyas/resources/figure_change_title.svg
--rw-rw-rw-   0        0        0     1082 2023-04-27 01:49:48.000000 PyArrShow-1.0.7/pyas/resources/figure_show_title_within_image.svg
--rw-rw-rw-   0        0        0     1013 2023-04-26 07:13:45.000000 PyArrShow-1.0.7/pyas/resources/file_exit.svg
--rw-rw-rw-   0        0        0      988 2023-04-26 07:08:47.000000 PyArrShow-1.0.7/pyas/resources/file_open.svg
--rw-rw-rw-   0        0        0      856 2023-04-26 07:09:25.000000 PyArrShow-1.0.7/pyas/resources/file_save.svg
--rw-rw-rw-   0        0        0     1806 2023-04-27 01:57:34.000000 PyArrShow-1.0.7/pyas/resources/help_about.svg
--rw-rw-rw-   0        0        0     1225 2023-04-26 03:29:10.000000 PyArrShow-1.0.7/pyas/resources/help_content.svg
--rw-rw-rw-   0        0        0     7336 2023-04-27 02:47:07.000000 PyArrShow-1.0.7/pyas/resources/main_window.jpg
--rw-rw-rw-   0        0        0    19019 2023-04-27 06:51:50.000000 PyArrShow-1.0.7/pyas/resources/main_window.png
--rw-rw-rw-   0        0        0    24034 2023-04-27 06:50:13.000000 PyArrShow-1.0.7/pyas/resources/main_window_v1.jpg
--rw-rw-rw-   0        0        0     4025 2023-04-26 09:13:00.000000 PyArrShow-1.0.7/pyas/resources/operation_FFT.svg
--rw-rw-rw-   0        0        0     4438 2023-04-27 01:40:25.000000 PyArrShow-1.0.7/pyas/resources/operation_FFTShift.svg
--rw-rw-rw-   0        0        0     2167 2023-04-26 08:19:11.000000 PyArrShow-1.0.7/pyas/resources/operation_Fourier_transform.svg
--rw-rw-rw-   0        0        0     2963 2023-04-26 07:31:28.000000 PyArrShow-1.0.7/pyas/resources/operation_anticlockwise_rotation_90.svg
--rw-rw-rw-   0        0        0     3068 2023-04-26 07:32:08.000000 PyArrShow-1.0.7/pyas/resources/operation_clockwise_rotation_90.svg
--rw-rw-rw-   0        0        0     1135 2023-05-05 03:27:32.000000 PyArrShow-1.0.7/pyas/resources/operation_conjugate.svg
--rw-rw-rw-   0        0        0      530 2023-04-26 07:59:11.000000 PyArrShow-1.0.7/pyas/resources/operation_flip_horizontal.svg
--rw-rw-rw-   0        0        0      536 2023-04-26 07:59:44.000000 PyArrShow-1.0.7/pyas/resources/operation_flip_vertical.svg
--rw-rw-rw-   0        0        0     6224 2023-04-26 09:13:12.000000 PyArrShow-1.0.7/pyas/resources/operation_iFFT.svg
--rw-rw-rw-   0        0        0     4422 2023-04-27 01:40:58.000000 PyArrShow-1.0.7/pyas/resources/operation_iFFTShift.svg
--rw-rw-rw-   0        0        0     1985 2023-05-05 03:46:53.000000 PyArrShow-1.0.7/pyas/resources/operation_permute.svg
--rw-rw-rw-   0        0        0     2527 2023-04-26 08:22:18.000000 PyArrShow-1.0.7/pyas/resources/operation_reset.svg
--rw-rw-rw-   0        0        0      690 2023-05-05 03:46:14.000000 PyArrShow-1.0.7/pyas/resources/operation_reshape.svg
--rw-rw-rw-   0        0        0      991 2023-05-05 03:43:28.000000 PyArrShow-1.0.7/pyas/resources/operation_squeeze.svg
--rw-rw-rw-   0        0        0     1100 2023-05-05 07:33:12.000000 PyArrShow-1.0.7/pyas/resources/view_playVideo.svg
--rw-rw-rw-   0        0        0     1864 2023-05-05 07:33:36.000000 PyArrShow-1.0.7/pyas/resources.qrc
--rw-rw-rw-   0        0        0     9960 2023-06-05 04:04:21.000000 PyArrShow-1.0.7/pyas/view.py
--rw-rw-rw-   0        0        0      723 2023-06-05 09:12:38.000000 PyArrShow-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 09:19:13.939046 PyArrShow-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 10:24:07.298277 PyArrShow-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-06-05 10:24:07.150791 PyArrShow-1.0.8/.vscode/
+-rw-rw-rw-   0        0        0      510 2023-06-02 11:52:15.000000 PyArrShow-1.0.8/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1088 2023-06-02 11:52:15.000000 PyArrShow-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1994 2023-06-05 10:24:07.296982 PyArrShow-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 10:24:07.172873 PyArrShow-1.0.8/PyArrShow.egg-info/
+-rw-rw-rw-   0        0        0     1994 2023-06-05 10:24:07.000000 PyArrShow-1.0.8/PyArrShow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-06-05 10:24:07.000000 PyArrShow-1.0.8/PyArrShow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 10:24:07.000000 PyArrShow-1.0.8/PyArrShow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-05 10:24:07.000000 PyArrShow-1.0.8/PyArrShow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 10:24:07.000000 PyArrShow-1.0.8/PyArrShow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-05 10:24:07.000000 PyArrShow-1.0.8/PyArrShow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1449 2023-06-05 10:20:47.000000 PyArrShow-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 10:24:07.176985 PyArrShow-1.0.8/__pycache__/
+-rw-rw-rw-   0        0        0      219 2023-06-02 11:52:15.000000 PyArrShow-1.0.8/__pycache__/__init__.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-06-05 10:24:07.211771 PyArrShow-1.0.8/pyas/
+-rw-rw-rw-   0        0        0     5088 2023-05-30 01:48:38.000000 PyArrShow-1.0.8/pyas/DataCursorFrame.py
+-rw-rw-rw-   0        0        0     3605 2023-05-05 11:35:48.000000 PyArrShow-1.0.8/pyas/ImgDisplayFrame.py
+-rw-rw-rw-   0        0        0    13988 2023-05-06 08:42:19.000000 PyArrShow-1.0.8/pyas/PilotFrame.py
+-rw-rw-rw-   0        0        0      169 2023-06-05 04:06:31.000000 PyArrShow-1.0.8/pyas/__init__.py
+-rw-rw-rw-   0        0        0     1055 2023-06-05 08:04:54.000000 PyArrShow-1.0.8/pyas/__main__.py
+-rw-rw-rw-   0        0        0    19356 2023-06-05 04:06:27.000000 PyArrShow-1.0.8/pyas/controller.py
+-rw-rw-rw-   0        0        0    47850 2023-06-05 02:12:58.000000 PyArrShow-1.0.8/pyas/main_backup.py
+-rw-rw-rw-   0        0        0    17671 2023-06-05 02:06:47.000000 PyArrShow-1.0.8/pyas/model.py
+-rw-rw-rw-   0        0        0    67984 2023-05-29 12:06:03.000000 PyArrShow-1.0.8/pyas/qrc_resources.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:24:07.294933 PyArrShow-1.0.8/pyas/resources/
+-rw-rw-rw-   0        0        0    44264 2023-04-27 02:48:45.000000 PyArrShow-1.0.8/pyas/resources/About_logo.jpg
+-rw-rw-rw-   0        0        0     5697 2023-04-28 09:46:12.000000 PyArrShow-1.0.8/pyas/resources/PyAs_main_window.svg
+-rw-rw-rw-   0        0        0      893 2023-04-27 01:46:15.000000 PyArrShow-1.0.8/pyas/resources/figure_change_title.svg
+-rw-rw-rw-   0        0        0     1082 2023-04-27 01:49:48.000000 PyArrShow-1.0.8/pyas/resources/figure_show_title_within_image.svg
+-rw-rw-rw-   0        0        0     1013 2023-04-26 07:13:45.000000 PyArrShow-1.0.8/pyas/resources/file_exit.svg
+-rw-rw-rw-   0        0        0      988 2023-04-26 07:08:47.000000 PyArrShow-1.0.8/pyas/resources/file_open.svg
+-rw-rw-rw-   0        0        0      856 2023-04-26 07:09:25.000000 PyArrShow-1.0.8/pyas/resources/file_save.svg
+-rw-rw-rw-   0        0        0     1806 2023-04-27 01:57:34.000000 PyArrShow-1.0.8/pyas/resources/help_about.svg
+-rw-rw-rw-   0        0        0     1225 2023-04-26 03:29:10.000000 PyArrShow-1.0.8/pyas/resources/help_content.svg
+-rw-rw-rw-   0        0        0     7336 2023-04-27 02:47:07.000000 PyArrShow-1.0.8/pyas/resources/main_window.jpg
+-rw-rw-rw-   0        0        0    19019 2023-04-27 06:51:50.000000 PyArrShow-1.0.8/pyas/resources/main_window.png
+-rw-rw-rw-   0        0        0    24034 2023-04-27 06:50:13.000000 PyArrShow-1.0.8/pyas/resources/main_window_v1.jpg
+-rw-rw-rw-   0        0        0     4025 2023-04-26 09:13:00.000000 PyArrShow-1.0.8/pyas/resources/operation_FFT.svg
+-rw-rw-rw-   0        0        0     4438 2023-04-27 01:40:25.000000 PyArrShow-1.0.8/pyas/resources/operation_FFTShift.svg
+-rw-rw-rw-   0        0        0     2167 2023-04-26 08:19:11.000000 PyArrShow-1.0.8/pyas/resources/operation_Fourier_transform.svg
+-rw-rw-rw-   0        0        0     2963 2023-04-26 07:31:28.000000 PyArrShow-1.0.8/pyas/resources/operation_anticlockwise_rotation_90.svg
+-rw-rw-rw-   0        0        0     3068 2023-04-26 07:32:08.000000 PyArrShow-1.0.8/pyas/resources/operation_clockwise_rotation_90.svg
+-rw-rw-rw-   0        0        0     1135 2023-05-05 03:27:32.000000 PyArrShow-1.0.8/pyas/resources/operation_conjugate.svg
+-rw-rw-rw-   0        0        0      530 2023-04-26 07:59:11.000000 PyArrShow-1.0.8/pyas/resources/operation_flip_horizontal.svg
+-rw-rw-rw-   0        0        0      536 2023-04-26 07:59:44.000000 PyArrShow-1.0.8/pyas/resources/operation_flip_vertical.svg
+-rw-rw-rw-   0        0        0     6224 2023-04-26 09:13:12.000000 PyArrShow-1.0.8/pyas/resources/operation_iFFT.svg
+-rw-rw-rw-   0        0        0     4422 2023-04-27 01:40:58.000000 PyArrShow-1.0.8/pyas/resources/operation_iFFTShift.svg
+-rw-rw-rw-   0        0        0     1985 2023-05-05 03:46:53.000000 PyArrShow-1.0.8/pyas/resources/operation_permute.svg
+-rw-rw-rw-   0        0        0     2527 2023-04-26 08:22:18.000000 PyArrShow-1.0.8/pyas/resources/operation_reset.svg
+-rw-rw-rw-   0        0        0      690 2023-05-05 03:46:14.000000 PyArrShow-1.0.8/pyas/resources/operation_reshape.svg
+-rw-rw-rw-   0        0        0      991 2023-05-05 03:43:28.000000 PyArrShow-1.0.8/pyas/resources/operation_squeeze.svg
+-rw-rw-rw-   0        0        0     1100 2023-05-05 07:33:12.000000 PyArrShow-1.0.8/pyas/resources/view_playVideo.svg
+-rw-rw-rw-   0        0        0     1864 2023-05-05 07:33:36.000000 PyArrShow-1.0.8/pyas/resources.qrc
+-rw-rw-rw-   0        0        0     9960 2023-06-05 04:04:21.000000 PyArrShow-1.0.8/pyas/view.py
+-rw-rw-rw-   0        0        0      723 2023-06-05 10:23:42.000000 PyArrShow-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 10:24:07.298922 PyArrShow-1.0.8/setup.cfg
```

### Comparing `PyArrShow-1.0.7/LICENSE` & `PyArrShow-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/PKG-INFO` & `PyArrShow-1.0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: PyArrShow
-Version: 1.0.7
-Summary: Python ArrayShow for MRI data visualization.
-Author-email: "Kaixuan,Zhao" <kaixuan_zhao@163.com>
-Project-URL: Homepage, https://github.com/15625148866/PyArrShow
-Project-URL: Bug Tracker, https://github.com/15625148866/PyArrShow/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyArrShow
 
 ## About
 
 Python is presently the leading language for MRI data processing and reconstruction, such as in fastMRI challenge, etc. Due to MRI data usually containing multiple dimensional aspects, such as width-height-slice-coil-dynamic-modalities(such as different b-values in DWI, and different TE images in multi-echo GRE/SE sequence), visualization of processed or reconstructed results requires checking MRI data along specific dimensions,  and this need can not be simply satisfied by standard matplotlib. Additionally, in the data preparation stage, visually checking multi-dimensional inputs and outputs is quite important and necessary.
 
 PyArrShow attempts to provide a Python tool with a similar functionality as the Matlab arrShow project. 
@@ -34,19 +20,21 @@
 
 ```
 pip install -e .
 ```
 
 ## Examples
 
-Here is an code example for PyArrShow
+Here is a code example for PyArrShow
 
 ```
-import  pyas 
+import pyas 
 import numpy as np
-5d_nparray = np.random.rand(256,344,10,5,8)
-pyas.PyArrShow().show(a)
+nparray_5d = np.random.rand(256,344,10,5,8)
+pyas.PyArrShow().show(nparray_5d)
+nparray_5d_c= np.random.rand(256,344,10,5,8) + 1j*np.random.rand(256,344,10,5,8)
+pyas.PyArrShow().show(nparray_5d_c)
 ```
 
 ## License
 
-PyArrShow is MIT licensed, as found in the LICENSE file.
+PyArrShow is MIT licensed, as found in the LICENSE file.
```

### Comparing `PyArrShow-1.0.7/PyArrShow.egg-info/SOURCES.txt` & `PyArrShow-1.0.8/PyArrShow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/DataCursorFrame.py` & `PyArrShow-1.0.8/pyas/DataCursorFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/ImgDisplayFrame.py` & `PyArrShow-1.0.8/pyas/ImgDisplayFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/PilotFrame.py` & `PyArrShow-1.0.8/pyas/PilotFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/__main__.py` & `PyArrShow-1.0.8/pyas/__main__.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/controller.py` & `PyArrShow-1.0.8/pyas/controller.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/main_backup.py` & `PyArrShow-1.0.8/pyas/main_backup.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/model.py` & `PyArrShow-1.0.8/pyas/model.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/qrc_resources.py` & `PyArrShow-1.0.8/pyas/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/About_logo.jpg` & `PyArrShow-1.0.8/pyas/resources/About_logo.jpg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/PyAs_main_window.svg` & `PyArrShow-1.0.8/pyas/resources/PyAs_main_window.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/figure_change_title.svg` & `PyArrShow-1.0.8/pyas/resources/figure_change_title.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/figure_show_title_within_image.svg` & `PyArrShow-1.0.8/pyas/resources/figure_show_title_within_image.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/file_exit.svg` & `PyArrShow-1.0.8/pyas/resources/file_exit.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/file_open.svg` & `PyArrShow-1.0.8/pyas/resources/file_open.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/file_save.svg` & `PyArrShow-1.0.8/pyas/resources/file_save.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/help_about.svg` & `PyArrShow-1.0.8/pyas/resources/help_about.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/help_content.svg` & `PyArrShow-1.0.8/pyas/resources/help_content.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/main_window.jpg` & `PyArrShow-1.0.8/pyas/resources/main_window.jpg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/main_window.png` & `PyArrShow-1.0.8/pyas/resources/main_window.png`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/main_window_v1.jpg` & `PyArrShow-1.0.8/pyas/resources/main_window_v1.jpg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_FFT.svg` & `PyArrShow-1.0.8/pyas/resources/operation_FFT.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_FFTShift.svg` & `PyArrShow-1.0.8/pyas/resources/operation_FFTShift.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_Fourier_transform.svg` & `PyArrShow-1.0.8/pyas/resources/operation_Fourier_transform.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_anticlockwise_rotation_90.svg` & `PyArrShow-1.0.8/pyas/resources/operation_anticlockwise_rotation_90.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_clockwise_rotation_90.svg` & `PyArrShow-1.0.8/pyas/resources/operation_clockwise_rotation_90.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_conjugate.svg` & `PyArrShow-1.0.8/pyas/resources/operation_conjugate.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_flip_horizontal.svg` & `PyArrShow-1.0.8/pyas/resources/operation_flip_horizontal.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_flip_vertical.svg` & `PyArrShow-1.0.8/pyas/resources/operation_flip_vertical.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_iFFT.svg` & `PyArrShow-1.0.8/pyas/resources/operation_iFFT.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_iFFTShift.svg` & `PyArrShow-1.0.8/pyas/resources/operation_iFFTShift.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_permute.svg` & `PyArrShow-1.0.8/pyas/resources/operation_permute.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_reset.svg` & `PyArrShow-1.0.8/pyas/resources/operation_reset.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_reshape.svg` & `PyArrShow-1.0.8/pyas/resources/operation_reshape.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/operation_squeeze.svg` & `PyArrShow-1.0.8/pyas/resources/operation_squeeze.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources/view_playVideo.svg` & `PyArrShow-1.0.8/pyas/resources/view_playVideo.svg`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/resources.qrc` & `PyArrShow-1.0.8/pyas/resources.qrc`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyas/view.py` & `PyArrShow-1.0.8/pyas/view.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.7/pyproject.toml` & `PyArrShow-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["setuptools","setuptools-scm"]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "PyArrShow"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Kaixuan,Zhao", email="kaixuan_zhao@163.com" },
 ]
 description = "Python ArrayShow for MRI data visualization."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

