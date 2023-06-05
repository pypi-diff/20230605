# Comparing `tmp/textbsr-0.0.24.tar.gz` & `tmp/textbsr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbsr-0.0.24.tar", last modified: Fri May 26 09:02:25 2023, max compression
+gzip compressed data, was "textbsr-0.1.0.tar", last modified: Mon Jun  5 11:35:31 2023, max compression
```

## Comparing `textbsr-0.0.24.tar` & `textbsr-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-26 09:02:25.000000 textbsr-0.0.24/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     3868 2023-05-26 09:02:25.000000 textbsr-0.0.24/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2747 2023-05-26 08:09:49.000000 textbsr-0.0.24/README.md
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-26 09:02:25.000000 textbsr-0.0.24/setup.cfg
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     1491 2023-05-26 09:02:13.000000 textbsr-0.0.24/setup.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-26 09:02:25.000000 textbsr-0.0.24/textbsr/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-05-26 07:57:27.000000 textbsr-0.0.24/textbsr/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-26 09:02:25.000000 textbsr-0.0.24/textbsr/checkpoints/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.24/textbsr/checkpoints/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-26 09:02:25.000000 textbsr-0.0.24/textbsr/models/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     9096 2023-05-26 08:08:30.000000 textbsr-0.0.24/textbsr/models/TextEnhancement.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-05-26 07:57:07.000000 textbsr-0.0.24/textbsr/models/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     6477 2023-05-26 09:02:03.000000 textbsr-0.0.24/textbsr/textbsr.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-26 09:02:25.000000 textbsr-0.0.24/textbsr/utils/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.24/textbsr/utils/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.24/textbsr/utils/utils_image.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-26 09:02:25.000000 textbsr-0.0.24/textbsr.egg-info/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     3868 2023-05-26 09:02:24.000000 textbsr-0.0.24/textbsr.egg-info/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      393 2023-05-26 09:02:25.000000 textbsr-0.0.24/textbsr.egg-info/SOURCES.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-26 09:02:24.000000 textbsr-0.0.24/textbsr.egg-info/dependency_links.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       53 2023-05-26 09:02:24.000000 textbsr-0.0.24/textbsr.egg-info/entry_points.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       56 2023-05-26 09:02:24.000000 textbsr-0.0.24/textbsr.egg-info/requires.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-26 09:02:25.000000 textbsr-0.0.24/textbsr.egg-info/top_level.txt
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 11:35:31.000000 textbsr-0.1.0/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     4434 2023-06-05 11:35:31.000000 textbsr-0.1.0/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     3226 2023-06-05 11:29:48.000000 textbsr-0.1.0/README.md
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-06-05 11:35:31.000000 textbsr-0.1.0/setup.cfg
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     1165 2023-06-05 11:34:10.000000 textbsr-0.1.0/setup.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.0/textbsr/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr/checkpoints/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.0/textbsr/checkpoints/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr/models/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     9774 2023-06-05 11:25:46.000000 textbsr-0.1.0/textbsr/models/TextEnhancement.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.0/textbsr/models/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     6519 2023-06-05 11:35:19.000000 textbsr-0.1.0/textbsr/textbsr.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr/utils/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.0/textbsr/utils/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     2636 2023-06-05 06:38:59.000000 textbsr-0.1.0/textbsr/utils/utils_image.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr.egg-info/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     4434 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr.egg-info/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      393 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       53 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr.egg-info/entry_points.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       42 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr.egg-info/requires.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-06-05 11:35:31.000000 textbsr-0.1.0/textbsr.egg-info/top_level.txt
```

### Comparing `textbsr-0.0.24/PKG-INFO` & `textbsr-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: textbsr
-Version: 0.0.24
+Version: 0.1.0
 Summary: a simple version for blind text image super-resolution (current version is only for English and Chinese)
 Home-page: https://github.com/csxmli2016/MARCONet
 Author: Xiaoming Li
 Author-email: csxmli@gmail.com
 License: S-Lab License 1.0
-Description: ## This is a simple text image super-resolution package.
+Description: 
+        # Update v0.25.0
         
+        - Support text region with different angle.
+        - Higher resolution. min(height, width) of output is 256 (128 in v0.24.0)
+        
+        See our project page for more details: https://github.com/csxmli2016/textbsr
+        
+        -----------
+        
+        ## This is a simple text image super-resolution package.
         More details can be found in our Project Page: https://github.com/csxmli2016/textbsr
-        > It can post-process the text region with a simple commond, i.e.,
-        ``` 
+        
+        This package can post-process the text region with a simple command, i.e., 
+        ```
         textbsr -i [LR_TEXT_PATH] -b [BACKGROUND_SR_PATH]
         ```
         
+        > - [LR_TEXT_PATH] is the LR image path.
+        > - [BACKGROUND_SR_PATH] stores the results from any blind image super-resolution methods.
+        > - If the text image is degraded severely, this method may still fail to obtain a plausible result.
         
-        ## Quick Start
         ### Dependencies and Installation
         - numpy
-        - opencv-python
+        - cnstd
         - torch>=1.8.1
         - torchvision>=0.9
         
         ``` 
         # Install with pip
         pip install textbsr
         ```
@@ -41,53 +53,52 @@
         textbsr.bsr(input_path='./testsets/LQs')
         ```
         
         Parameter details:
         
         | parameter name | default | description  |
         | :-----  | :-----:  | :-----  |
-        | <span style="white-space:nowrap">-i, --input_path </span>| - | The lr text image path. It can be a full image or a text region only |
-        | <span style="white-space:nowrap">-b, --bg_path</span> | None | The background sr path from other methods. If None, we only super-resolve the text region.|
-        | <span style="white-space:nowrap">-o, --output_path</span> | None | The save path for text sr result. If None, we save the results on the same path with [input_path]_TIMESTAMP|
-        | <span style="white-space:nowrap">-a, --aligned </span>| False | action='store_true'. If True, the input text image contains only text region. If False, we use CnSTD to detect and restore the text region.|
+        | <span style="white-space:nowrap">-i, --input_path </span>| - | The lr text image path. It can store full images or text layouts only. |
+        | <span style="white-space:nowrap">-b, --bg_path</span> | None | The background sr path from other methods. If None, we only restore the text region detected by cnstd.|
+        | <span style="white-space:nowrap">-o, --output_path</span> | None | The save path for text sr result. If None, we save the results on the same path with the format of [input_path]\_TIMESTAMP.|
+        | <span style="white-space:nowrap">-a, --aligned </span>| False | action='store_true'. If True, the input text image contains only text region. If False, we use CnSTD to detect text regions and then restore them.|
         | <span style="white-space:nowrap">-s, --save_text </span>| False | action='store_true'. If True, save the LR and SR text layout.|
         | <span style="white-space:nowrap">-d, --device</span> | None | Device, use 'gpu' or 'cpu'. If None, we use torch.cuda.is_available to select the device. |
         
-        
         ### Example for post-processing the text region
         ```
         # On the terminal command
         textbsr -i [LR_TEXT_PATH] -b [BACKGROUND_SR_PATH] -s
         ```
         or
         ```
         # On the python environment
         from textbsr import textbsr
         textbsr.bsr(input_path='./testsets/LQs', bg_path='./testsets/RealESRGANResults', save_text=True)
         ```
-        > When [BACKGROUND_SR_PATH] is None, we only restore the text region and paste back to the LR input, with the background region unchanged.
+        > When [BACKGROUND_SR_PATH] is None, we only restore the text region and paste it back to the LR input, with the background region unchanged.
         
         
         ---
         
-        ### Example for super-resolving the aligned text region
+        ### Example for restoring the aligned text region
         ```
         # On the terminal command
         textbsr -i [LR_TEXT_PATH] -a
         ```
         or
         ```
         # On the python environment
         from textbsr import textbsr
         textbsr.bsr(input_path='./testsets/LQs', aligned=True)
         ```
         
         
         
-        > If you find this package helpful, please kindly consider to cite our paper:
+        > If you find this package helpful, please kindly consider citing our paper:
         ```
         @InProceedings{li2023marconet,
         author = {Li, Xiaoming and Zuo, Wangmeng and Loy, Chen Change},
         title = {Learning Generative Structure Prior for Blind Text Image Super-resolution},
         booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
         year = {2023}
         }
```

### Comparing `textbsr-0.0.24/README.md` & `textbsr-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,32 @@
-## This is a simple text image super-resolution package.
 
+# Update v0.25.0
+
+- Support text region with different angle.
+- Higher resolution. min(height, width) of output is 256 (128 in v0.24.0)
+
+See our project page for more details: https://github.com/csxmli2016/textbsr
+
+-----------
+
+## This is a simple text image super-resolution package.
 More details can be found in our Project Page: https://github.com/csxmli2016/textbsr
-> It can post-process the text region with a simple commond, i.e.,
-``` 
+
+This package can post-process the text region with a simple command, i.e., 
+```
 textbsr -i [LR_TEXT_PATH] -b [BACKGROUND_SR_PATH]
 ```
 
+> - [LR_TEXT_PATH] is the LR image path.
+> - [BACKGROUND_SR_PATH] stores the results from any blind image super-resolution methods.
+> - If the text image is degraded severely, this method may still fail to obtain a plausible result.
 
-## Quick Start
 ### Dependencies and Installation
 - numpy
-- opencv-python
+- cnstd
 - torch>=1.8.1
 - torchvision>=0.9
 
 ``` 
 # Install with pip
 pip install textbsr
 ```
@@ -33,53 +45,52 @@
 textbsr.bsr(input_path='./testsets/LQs')
 ```
 
 Parameter details:
 
 | parameter name | default | description  |
 | :-----  | :-----:  | :-----  |
-| <span style="white-space:nowrap">-i, --input_path </span>| - | The lr text image path. It can be a full image or a text region only |
-| <span style="white-space:nowrap">-b, --bg_path</span> | None | The background sr path from other methods. If None, we only super-resolve the text region.|
-| <span style="white-space:nowrap">-o, --output_path</span> | None | The save path for text sr result. If None, we save the results on the same path with [input_path]_TIMESTAMP|
-| <span style="white-space:nowrap">-a, --aligned </span>| False | action='store_true'. If True, the input text image contains only text region. If False, we use CnSTD to detect and restore the text region.|
+| <span style="white-space:nowrap">-i, --input_path </span>| - | The lr text image path. It can store full images or text layouts only. |
+| <span style="white-space:nowrap">-b, --bg_path</span> | None | The background sr path from other methods. If None, we only restore the text region detected by cnstd.|
+| <span style="white-space:nowrap">-o, --output_path</span> | None | The save path for text sr result. If None, we save the results on the same path with the format of [input_path]\_TIMESTAMP.|
+| <span style="white-space:nowrap">-a, --aligned </span>| False | action='store_true'. If True, the input text image contains only text region. If False, we use CnSTD to detect text regions and then restore them.|
 | <span style="white-space:nowrap">-s, --save_text </span>| False | action='store_true'. If True, save the LR and SR text layout.|
 | <span style="white-space:nowrap">-d, --device</span> | None | Device, use 'gpu' or 'cpu'. If None, we use torch.cuda.is_available to select the device. |
 
-
 ### Example for post-processing the text region
 ```
 # On the terminal command
 textbsr -i [LR_TEXT_PATH] -b [BACKGROUND_SR_PATH] -s
 ```
 or
 ```
 # On the python environment
 from textbsr import textbsr
 textbsr.bsr(input_path='./testsets/LQs', bg_path='./testsets/RealESRGANResults', save_text=True)
 ```
-> When [BACKGROUND_SR_PATH] is None, we only restore the text region and paste back to the LR input, with the background region unchanged.
+> When [BACKGROUND_SR_PATH] is None, we only restore the text region and paste it back to the LR input, with the background region unchanged.
 
 
 ---
 
-### Example for super-resolving the aligned text region
+### Example for restoring the aligned text region
 ```
 # On the terminal command
 textbsr -i [LR_TEXT_PATH] -a
 ```
 or
 ```
 # On the python environment
 from textbsr import textbsr
 textbsr.bsr(input_path='./testsets/LQs', aligned=True)
 ```
 
 
 
-> If you find this package helpful, please kindly consider to cite our paper:
+> If you find this package helpful, please kindly consider citing our paper:
 ```
 @InProceedings{li2023marconet,
 author = {Li, Xiaoming and Zuo, Wangmeng and Loy, Chen Change},
 title = {Learning Generative Structure Prior for Blind Text Image Super-resolution},
 booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
 year = {2023}
 }
```

### Comparing `textbsr-0.0.24/textbsr/textbsr.py` & `textbsr-0.1.0/textbsr/textbsr.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import torch.nn.functional as F
 import time
 import argparse
 import os.path as osp
 from urllib.parse import urlparse
 
 pretrain_model_url = {
-    'x4': 'https://github.com/macuper/tmppp/releases/download/v1/bsrgan_text.pth',
+    'x4': 'https://github.com/csxmli2016/textbsr/releases/download/0.2.0/bsrgan_text_256.pth',
 }
-# https://github.com/csxmli2016/textbsr/releases/download/0.1.0/bsrgan_text.pth
 
 
 def load_file_from_url(url, model_dir=None, progress=True, file_name=None):
     if model_dir is None:  # use the pytorch hub_dir
         hub_dir = get_dir()
         model_dir = os.path.join(hub_dir, 'checkpoints')
 
@@ -36,14 +35,16 @@
     return cached_file
 
 def bsr(input_path=None, bg_path=None, output_path=None, aligned=False, save_text=False, device=None):
     if input_path is None:
         exit('input image path is none. Please see our document')
     if output_path is None:
         TIMESTAMP = time.strftime("%m-%d_%H-%M", time.localtime())
+        if input_path[-1] == '/' or input_path[-1] == '\\':
+            input_path = input_path[:-1]
         output_path = osp.join(input_path+'_'+TIMESTAMP+'_BSRGAN-Text')
     os.makedirs(output_path, exist_ok=True)
 
     lq_imgs = []
     sq_imgs = []
     lq_imgs = util.get_image_paths(input_path)
     if len(lq_imgs) ==0:
@@ -87,16 +88,16 @@
         #####(1) Read Image
         ####################################
         idx += 1
         img_name, ext = os.path.splitext(os.path.basename(img))
         print('{:>20s} {:04d} : x{:<d} --> {:<s}'.format('Restoring ', idx, scale_factor, img_name+ext))
 
         img_L = util.imread_uint(img, n_channels=3) #RGB 0~255
-        width_L = img_L.shape[1]
-        height_L = img_L.shape[0]
+        height_L, width_L = img_L.shape[:2]
+
 
         width_S, height_S = 0, 0
         
 
         if len(sq_imgs) > 0:
             sq_img = sq_imgs[idx-1]
             img_E = util.imread_uint(sq_img, n_channels=3)
@@ -115,23 +116,24 @@
         if not aligned:
             if width_S == 0 or height_S == 0:
                 width_S = (width_L * scale_factor)
                 height_S = (height_L * scale_factor)
             SQ = cv2.resize(SQ.astype(np.float32), (width_S, height_S), interpolation=cv2.INTER_AREA)
             cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), SQ[:,:,::-1])
         else:
-            cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), en_texts[0])
+            cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), en_texts[0][:,:,::-1])
+
         ####################################
         #####(3) Save Cropped Results
         ####################################
         if save_text and not aligned:
             for m, (et, ot) in enumerate(zip(en_texts, ori_texts)): ##save each face region
                 w, h, c = et.shape
                 ot = cv2.resize(ot, (h, w))
-                cv2.imwrite(os.path.join(E_path, img_name +'_patch_{}.png'.format(m)), np.hstack((ot, et)))
+                cv2.imwrite(os.path.join(E_path, img_name +'_patch_{}.png'.format(m)), np.hstack((ot[:,:,::-1], et[:,:,::-1])))
 
 
 def textbsr():
     parser = argparse.ArgumentParser()
     parser.add_argument('-i', '--input_path', type=str, default='./testsets/LQ', help='The lr text image path')
     parser.add_argument('-b', '--bg_path', type=str, default=None, help='The background sr path, default:None')
     parser.add_argument('-o', '--output_path', type=str, default=None, help='The save path for text sr result')
```

### Comparing `textbsr-0.0.24/textbsr/utils/utils_image.py` & `textbsr-0.1.0/textbsr/utils/utils_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import os
-import math
-import random
 import numpy as np
 import torch
 import cv2
-# from torchvision.utils import make_grid
-# from datetime import datetime
-# import matplotlib.pyplot as plt
-# from mpl_toolkits.mplot3d import Axes3D
+
 os.environ["KMP_DUPLICATE_LIB_OK"]="TRUE"
 
 
 IMG_EXTENSIONS = ['.jpg', '.JPG', '.jpeg', '.JPEG', '.png', '.PNG', '.ppm', '.PPM', '.bmp', '.BMP', '.tif']
 
 def is_image_file(filename):
     return any(filename.endswith(extension) for extension in IMG_EXTENSIONS)
@@ -54,14 +49,18 @@
     #  input: path
     # output: HxWx3(RGB or GGG), or HxWx1 (G)
     if n_channels == 1:
         img = cv2.imread(path, 0)  # cv2.IMREAD_GRAYSCALE
         img = np.expand_dims(img, axis=2)  # HxWx1
     elif n_channels == 3:
         img = cv2.imread(path, cv2.IMREAD_UNCHANGED)  # BGR or G
+        if img is None:
+            import PIL
+            img = np.array(PIL.Image.open(path).convert('RGB'))
+            return img
         if img.ndim == 2:
             img = cv2.cvtColor(img, cv2.COLOR_GRAY2RGB)  # GGG
         else:
             img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)  # RGB
     return img
 
 def imsave(img, img_path):
```

### Comparing `textbsr-0.0.24/textbsr.egg-info/PKG-INFO` & `textbsr-0.1.0/textbsr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: textbsr
-Version: 0.0.24
+Version: 0.1.0
 Summary: a simple version for blind text image super-resolution (current version is only for English and Chinese)
 Home-page: https://github.com/csxmli2016/MARCONet
 Author: Xiaoming Li
 Author-email: csxmli@gmail.com
 License: S-Lab License 1.0
-Description: ## This is a simple text image super-resolution package.
+Description: 
+        # Update v0.25.0
         
+        - Support text region with different angle.
+        - Higher resolution. min(height, width) of output is 256 (128 in v0.24.0)
+        
+        See our project page for more details: https://github.com/csxmli2016/textbsr
+        
+        -----------
+        
+        ## This is a simple text image super-resolution package.
         More details can be found in our Project Page: https://github.com/csxmli2016/textbsr
-        > It can post-process the text region with a simple commond, i.e.,
-        ``` 
+        
+        This package can post-process the text region with a simple command, i.e., 
+        ```
         textbsr -i [LR_TEXT_PATH] -b [BACKGROUND_SR_PATH]
         ```
         
+        > - [LR_TEXT_PATH] is the LR image path.
+        > - [BACKGROUND_SR_PATH] stores the results from any blind image super-resolution methods.
+        > - If the text image is degraded severely, this method may still fail to obtain a plausible result.
         
-        ## Quick Start
         ### Dependencies and Installation
         - numpy
-        - opencv-python
+        - cnstd
         - torch>=1.8.1
         - torchvision>=0.9
         
         ``` 
         # Install with pip
         pip install textbsr
         ```
@@ -41,53 +53,52 @@
         textbsr.bsr(input_path='./testsets/LQs')
         ```
         
         Parameter details:
         
         | parameter name | default | description  |
         | :-----  | :-----:  | :-----  |
-        | <span style="white-space:nowrap">-i, --input_path </span>| - | The lr text image path. It can be a full image or a text region only |
-        | <span style="white-space:nowrap">-b, --bg_path</span> | None | The background sr path from other methods. If None, we only super-resolve the text region.|
-        | <span style="white-space:nowrap">-o, --output_path</span> | None | The save path for text sr result. If None, we save the results on the same path with [input_path]_TIMESTAMP|
-        | <span style="white-space:nowrap">-a, --aligned </span>| False | action='store_true'. If True, the input text image contains only text region. If False, we use CnSTD to detect and restore the text region.|
+        | <span style="white-space:nowrap">-i, --input_path </span>| - | The lr text image path. It can store full images or text layouts only. |
+        | <span style="white-space:nowrap">-b, --bg_path</span> | None | The background sr path from other methods. If None, we only restore the text region detected by cnstd.|
+        | <span style="white-space:nowrap">-o, --output_path</span> | None | The save path for text sr result. If None, we save the results on the same path with the format of [input_path]\_TIMESTAMP.|
+        | <span style="white-space:nowrap">-a, --aligned </span>| False | action='store_true'. If True, the input text image contains only text region. If False, we use CnSTD to detect text regions and then restore them.|
         | <span style="white-space:nowrap">-s, --save_text </span>| False | action='store_true'. If True, save the LR and SR text layout.|
         | <span style="white-space:nowrap">-d, --device</span> | None | Device, use 'gpu' or 'cpu'. If None, we use torch.cuda.is_available to select the device. |
         
-        
         ### Example for post-processing the text region
         ```
         # On the terminal command
         textbsr -i [LR_TEXT_PATH] -b [BACKGROUND_SR_PATH] -s
         ```
         or
         ```
         # On the python environment
         from textbsr import textbsr
         textbsr.bsr(input_path='./testsets/LQs', bg_path='./testsets/RealESRGANResults', save_text=True)
         ```
-        > When [BACKGROUND_SR_PATH] is None, we only restore the text region and paste back to the LR input, with the background region unchanged.
+        > When [BACKGROUND_SR_PATH] is None, we only restore the text region and paste it back to the LR input, with the background region unchanged.
         
         
         ---
         
-        ### Example for super-resolving the aligned text region
+        ### Example for restoring the aligned text region
         ```
         # On the terminal command
         textbsr -i [LR_TEXT_PATH] -a
         ```
         or
         ```
         # On the python environment
         from textbsr import textbsr
         textbsr.bsr(input_path='./testsets/LQs', aligned=True)
         ```
         
         
         
-        > If you find this package helpful, please kindly consider to cite our paper:
+        > If you find this package helpful, please kindly consider citing our paper:
         ```
         @InProceedings{li2023marconet,
         author = {Li, Xiaoming and Zuo, Wangmeng and Loy, Chen Change},
         title = {Learning Generative Structure Prior for Blind Text Image Super-resolution},
         booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
         year = {2023}
         }
```

