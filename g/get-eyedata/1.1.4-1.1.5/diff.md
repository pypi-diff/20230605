# Comparing `tmp/get_eyedata-1.1.4.tar.gz` & `tmp/get_eyedata-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_eyedata-1.1.4.tar", last modified: Sun Jun  4 09:16:50 2023, max compression
+gzip compressed data, was "get_eyedata-1.1.5.tar", last modified: Mon Jun  5 08:32:44 2023, max compression
```

## Comparing `get_eyedata-1.1.4.tar` & `get_eyedata-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 09:16:50.527707 get_eyedata-1.1.4/
--rw-rw-rw-   0        0        0     1091 2023-04-27 05:56:35.000000 get_eyedata-1.1.4/LICENCE
--rw-rw-rw-   0        0        0     1930 2023-06-04 09:16:50.526708 get_eyedata-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1407 2023-05-13 00:34:57.000000 get_eyedata-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 09:16:50.503704 get_eyedata-1.1.4/get_eyedata/
--rw-rw-rw-   0        0        0        6 2023-06-04 09:16:22.000000 get_eyedata-1.1.4/get_eyedata/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-06-04 07:07:15.000000 get_eyedata-1.1.4/get_eyedata/frame_utils.py
--rw-rw-rw-   0        0        0        0 2023-05-13 00:34:57.000000 get_eyedata-1.1.4/get_eyedata/ow2.py
--rw-rw-rw-   0        0        0     3258 2023-06-04 08:53:03.000000 get_eyedata-1.1.4/get_eyedata/valo.py
-drwxrwxrwx   0        0        0        0 2023-06-04 09:16:50.521702 get_eyedata-1.1.4/get_eyedata.egg-info/
--rw-rw-rw-   0        0        0     1930 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 09:16:50.527707 get_eyedata-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1492 2023-06-04 09:16:38.000000 get_eyedata-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:32:44.402189 get_eyedata-1.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-27 05:56:35.000000 get_eyedata-1.1.5/LICENCE
+-rw-rw-rw-   0        0        0     1431 2023-06-05 08:32:44.401189 get_eyedata-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-06-05 08:24:05.000000 get_eyedata-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 08:32:44.369487 get_eyedata-1.1.5/get_eyedata/
+-rw-rw-rw-   0        0        0        6 2023-06-05 08:24:05.000000 get_eyedata-1.1.5/get_eyedata/__init__.py
+-rw-rw-rw-   0        0        0     1581 2023-06-05 08:24:48.000000 get_eyedata-1.1.5/get_eyedata/frame_utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 08:24:05.000000 get_eyedata-1.1.5/get_eyedata/ow2.py
+-rw-rw-rw-   0        0        0     3258 2023-06-05 08:24:05.000000 get_eyedata-1.1.5/get_eyedata/valo.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:32:44.395679 get_eyedata-1.1.5/get_eyedata.egg-info/
+-rw-rw-rw-   0        0        0     1431 2023-06-05 08:32:44.000000 get_eyedata-1.1.5/get_eyedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-05 08:32:44.000000 get_eyedata-1.1.5/get_eyedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:32:44.000000 get_eyedata-1.1.5/get_eyedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2023-06-05 08:32:44.000000 get_eyedata-1.1.5/get_eyedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-05 08:32:44.000000 get_eyedata-1.1.5/get_eyedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 08:32:44.402189 get_eyedata-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1492 2023-06-05 08:32:40.000000 get_eyedata-1.1.5/setup.py
```

### Comparing `get_eyedata-1.1.4/LICENCE` & `get_eyedata-1.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `get_eyedata-1.1.4/PKG-INFO` & `get_eyedata-1.1.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_eyedata
-Version: 1.1.4
+Version: 1.1.5
 Summary: gat gaze data form record.
 Home-page: https://github.com/ikrfun/get_eyedata
 Download-URL: https://github.com/ikrfun/get_eyedata
 Author: ikrfun
 Author-email: t.nobuto130625@gmail.com
 Maintainer: ikrfun
 Maintainer-email: t.nobuto130625@gmail.com
@@ -13,31 +13,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Get-eyedata
 
-this softwere is an application that allows you to track objects in a video file and save the tracking data to a CSV file.
+this library is an application that allows you to track objects in a video file and save the tracking data to a CSV file.
 
 ## Installation
-
 ---
-
-1. Clone the repository to your local machine using the following command:
-
+you can use pip to install get-eyedata.
 ```bash
-git clone https://github.com/ikrfun/get_eyedata.git
-cd get_eyedata
-```
-
-2. Install the required packages using the following command:
-
-```bash
-pip install -r requirements.txt
+pip install get-eyedata
 ```
 
 ---
 
 ## Usage
 
 ### Preparing Recorded Data
@@ -50,30 +40,17 @@
 
 ---
 
 ### When creating a dataset of actual facial images and their corresponding gaze coordinates 
 
 To use mekeing eye dataset, run the following command in your terminal
 
-```bash
-python make_eyedataset.py -f <video-file-path> 
-```
+```python
+from get_eyedata import valo
 
-`<video-file-path>`: The path to the video file 
-then you can find dataset on 'data' dir
-
----
-
-###  When creating a dataset consisting of Valorant screen data and corresponding gaze information
-
-```bash
-python make_valodataset.py -f <video-file-path> 
+# valo_df is pandas dataframe
+valo_df = valo.make_dataset('{video-file-path}')
 ```
-
-`<video-file-path>`: The path to the video file 
-then you can find dataset on 'data' dir
-
 ---
-
 ## License
 
 This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `get_eyedata-1.1.4/README.md` & `get_eyedata-1.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 # Get-eyedata
 
-this softwere is an application that allows you to track objects in a video file and save the tracking data to a CSV file.
+this library is an application that allows you to track objects in a video file and save the tracking data to a CSV file.
 
 ## Installation
-
 ---
-
-1. Clone the repository to your local machine using the following command:
-
+you can use pip to install get-eyedata.
 ```bash
-git clone https://github.com/ikrfun/get_eyedata.git
-cd get_eyedata
-```
-
-2. Install the required packages using the following command:
-
-```bash
-pip install -r requirements.txt
+pip install get-eyedata
 ```
 
 ---
 
 ## Usage
 
 ### Preparing Recorded Data
@@ -33,30 +23,17 @@
 
 ---
 
 ### When creating a dataset of actual facial images and their corresponding gaze coordinates 
 
 To use mekeing eye dataset, run the following command in your terminal
 
-```bash
-python make_eyedataset.py -f <video-file-path> 
-```
+```python
+from get_eyedata import valo
 
-`<video-file-path>`: The path to the video file 
-then you can find dataset on 'data' dir
-
----
-
-###  When creating a dataset consisting of Valorant screen data and corresponding gaze information
-
-```bash
-python make_valodataset.py -f <video-file-path> 
+# valo_df is pandas dataframe
+valo_df = valo.make_dataset('{video-file-path}')
 ```
-
-`<video-file-path>`: The path to the video file 
-then you can find dataset on 'data' dir
-
 ---
-
 ## License
 
 This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `get_eyedata-1.1.4/get_eyedata/frame_utils.py` & `get_eyedata-1.1.5/get_eyedata/frame_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,32 +7,36 @@
     _, binary = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
     binary_array = np.where(binary == 0, 0, 1)
     return binary_array
 
 def cog(binary_img):
     '''
     Center of Gravity
-    重心を座標として出力する
+    重心を座標として出力する（左下を0,0とする座標系）
     '''
-    #ラベリング処理
+    # ラベリング処理
     nlabels, labels, stats, center = cv2.connectedComponentsWithStats(binary_img)
-    #背景のオブジェクト情報の削除
+    
+    # 背景のオブジェクト情報の削除
     nlabels = nlabels - 1
     stats = np.delete(stats, 0, 0)
     center = np.delete(center, 0, 0)
-    #面積が最大のオブジェクトのラベル番号を取得
+    
+    # 面積が最大のオブジェクトのラベル番号を取得
     try:
-        max_index = np.argmax(stats[:,4])
+        max_index = np.argmax(stats[:, 4])
         center_x = int(center[max_index][0])
-        center_y = int(center[max_index][1])
+        center_y = binary_img.shape[0] - int(center[max_index][1])  # y座標を変更
     except ValueError:
         center_x = np.nan
         center_y = np.nan
+    
     return center_x, center_y
 
+
 def sep_y(image,corrd:int = None):
     '''
     frameを回しているfor文の中での利用を前提とする
     '''
     if corrd:
         # 動画を上下で半分に分割
         top_half = image[:corrd, :]
```

### Comparing `get_eyedata-1.1.4/get_eyedata/valo.py` & `get_eyedata-1.1.5/get_eyedata/valo.py`

 * *Files identical despite different names*

### Comparing `get_eyedata-1.1.4/get_eyedata.egg-info/PKG-INFO` & `get_eyedata-1.1.5/get_eyedata.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-eyedata
-Version: 1.1.4
+Version: 1.1.5
 Summary: gat gaze data form record.
 Home-page: https://github.com/ikrfun/get_eyedata
 Download-URL: https://github.com/ikrfun/get_eyedata
 Author: ikrfun
 Author-email: t.nobuto130625@gmail.com
 Maintainer: ikrfun
 Maintainer-email: t.nobuto130625@gmail.com
@@ -13,31 +13,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Get-eyedata
 
-this softwere is an application that allows you to track objects in a video file and save the tracking data to a CSV file.
+this library is an application that allows you to track objects in a video file and save the tracking data to a CSV file.
 
 ## Installation
-
 ---
-
-1. Clone the repository to your local machine using the following command:
-
+you can use pip to install get-eyedata.
 ```bash
-git clone https://github.com/ikrfun/get_eyedata.git
-cd get_eyedata
-```
-
-2. Install the required packages using the following command:
-
-```bash
-pip install -r requirements.txt
+pip install get-eyedata
 ```
 
 ---
 
 ## Usage
 
 ### Preparing Recorded Data
@@ -50,30 +40,17 @@
 
 ---
 
 ### When creating a dataset of actual facial images and their corresponding gaze coordinates 
 
 To use mekeing eye dataset, run the following command in your terminal
 
-```bash
-python make_eyedataset.py -f <video-file-path> 
-```
+```python
+from get_eyedata import valo
 
-`<video-file-path>`: The path to the video file 
-then you can find dataset on 'data' dir
-
----
-
-###  When creating a dataset consisting of Valorant screen data and corresponding gaze information
-
-```bash
-python make_valodataset.py -f <video-file-path> 
+# valo_df is pandas dataframe
+valo_df = valo.make_dataset('{video-file-path}')
 ```
-
-`<video-file-path>`: The path to the video file 
-then you can find dataset on 'data' dir
-
 ---
-
 ## License
 
 This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `get_eyedata-1.1.4/setup.py` & `get_eyedata-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = 'gat gaze data form record.'
 NAME = 'get_eyedata'
 AUTHOR = 'ikrfun'
 AUTHOR_EMAIL = 't.nobuto130625@gmail.com'
 URL = 'https://github.com/ikrfun/get_eyedata'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 PYTHON_REQUIRES = '>=3.10'
 INSTALL_REQUIRES = [
     'matplotlib>=3.7.1',
     'moviepy>=1.0.3',
     'numpy>=1.24.3',
     'opencv_contrib_python>=4.6.0.66',
     'opencv_python>=4.7.0.72',
```

