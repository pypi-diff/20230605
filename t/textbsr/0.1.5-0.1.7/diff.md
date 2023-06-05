# Comparing `tmp/textbsr-0.1.5.tar.gz` & `tmp/textbsr-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbsr-0.1.5.tar", last modified: Mon Jun  5 12:35:59 2023, max compression
+gzip compressed data, was "textbsr-0.1.7.tar", last modified: Mon Jun  5 12:51:40 2023, max compression
```

## Comparing `textbsr-0.1.5.tar` & `textbsr-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:35:59.000000 textbsr-0.1.5/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:35:59.000000 textbsr-0.1.5/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     3225 2023-06-05 12:13:56.000000 textbsr-0.1.5/README.md
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-06-05 12:35:59.000000 textbsr-0.1.5/setup.cfg
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     1165 2023-06-05 12:35:50.000000 textbsr-0.1.5/setup.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.5/textbsr/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr/checkpoints/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.5/textbsr/checkpoints/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr/models/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     9774 2023-06-05 11:52:46.000000 textbsr-0.1.5/textbsr/models/TextEnhancement.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.5/textbsr/models/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     6879 2023-06-05 12:19:06.000000 textbsr-0.1.5/textbsr/textbsr.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr/utils/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.5/textbsr/utils/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2636 2023-06-05 06:38:59.000000 textbsr-0.1.5/textbsr/utils/utils_image.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr.egg-info/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr.egg-info/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      393 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr.egg-info/SOURCES.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr.egg-info/dependency_links.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       53 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr.egg-info/entry_points.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       47 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr.egg-info/requires.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-06-05 12:35:59.000000 textbsr-0.1.5/textbsr.egg-info/top_level.txt
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:51:40.000000 textbsr-0.1.7/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:51:40.000000 textbsr-0.1.7/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     3225 2023-06-05 12:13:56.000000 textbsr-0.1.7/README.md
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-06-05 12:51:40.000000 textbsr-0.1.7/setup.cfg
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     1165 2023-06-05 12:47:49.000000 textbsr-0.1.7/setup.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.7/textbsr/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr/checkpoints/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.7/textbsr/checkpoints/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr/models/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     9774 2023-06-05 11:52:46.000000 textbsr-0.1.7/textbsr/models/TextEnhancement.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.7/textbsr/models/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     6627 2023-06-05 12:51:24.000000 textbsr-0.1.7/textbsr/textbsr.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr/utils/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.7/textbsr/utils/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     2636 2023-06-05 06:38:59.000000 textbsr-0.1.7/textbsr/utils/utils_image.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr.egg-info/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr.egg-info/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      393 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       53 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr.egg-info/entry_points.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       47 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr.egg-info/requires.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-06-05 12:51:40.000000 textbsr-0.1.7/textbsr.egg-info/top_level.txt
```

### Comparing `textbsr-0.1.5/PKG-INFO` & `textbsr-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textbsr
-Version: 0.1.5
+Version: 0.1.7
 Summary: a simple version for blind text image super-resolution (current version is only for English and Chinese)
 Home-page: https://github.com/csxmli2016/MARCONet
 Author: Xiaoming Li
 Author-email: csxmli@gmail.com
 License: S-Lab License 1.0
 Description: 
         # Update v0.1.2
```

### Comparing `textbsr-0.1.5/README.md` & `textbsr-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `textbsr-0.1.5/setup.py` & `textbsr-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         requires = [line.replace('\n', '') for line in f.readlines()]
     return requires
 
 def read(fname):
 	return codecs.open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(name='textbsr',
-      version='0.1.5',
+      version='0.1.7',
       description='a simple version for blind text image super-resolution (current version is only for English and Chinese)',
       author='Xiaoming Li',
       author_email='csxmli@gmail.com',
       long_description=read("README.md"),
       long_description_content_type="text/markdown",
       packages=find_packages(),  #
       #
```

### Comparing `textbsr-0.1.5/textbsr/models/TextEnhancement.py` & `textbsr-0.1.7/textbsr/models/TextEnhancement.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.1.5/textbsr/textbsr.py` & `textbsr-0.1.7/textbsr/textbsr.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,16 @@
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
-
 
 def load_file_from_url(url, model_dir=None, progress=True, file_name=None):
     if model_dir is None:  # use the pytorch hub_dir
         hub_dir = get_dir()
         model_dir = os.path.join(hub_dir, 'checkpoints')
 
     os.makedirs(model_dir, exist_ok=True)
@@ -59,15 +57,14 @@
     if device == None or device == 'gpu':
         use_cuda = torch.cuda.is_available()
     if device == 'cpu':
         use_cuda = False
     device = torch.device('cuda' if use_cuda else 'cpu')
     weight_path = load_file_from_url(pretrain_model_url['x4'])
 
-    weight_path = '/mnt/lustre/xmli/MARCONetESRGAN/experiments/train_sr/models/net_g_ema_279000.pth'
     TextModel = TextRestoration(ModelName='RRDB', TextModelPath=weight_path, device=device)
 
     print('{:>25s} : {:s}'.format('Model Name', 'BSRGAN'))
     if use_cuda:
         print('{:>25s} : {:<d}'.format('GPU ID', torch.cuda.current_device()))
     else:
         print('{:>25s} : {:s}'.format('GPU ID', 'No GPU is available. Use CPU instead.'))
@@ -121,15 +118,15 @@
             if width_S == 0 or height_S == 0:
                 width_S = (width_L * scale_factor)
                 height_S = (height_L * scale_factor)
             SQ = cv2.resize(SQ.astype(np.float32), (width_S, height_S), interpolation=cv2.INTER_AREA)
             cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), SQ[:,:,::-1])
         else:
             cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), en_texts[0][:,:,::-1])
-        cv2.imwrite(os.path.join(E_path, img_name +'_Input.png'), img_E[:,:,::-1])
+
         ####################################
         #####(3) Save Cropped Results
         ####################################
         if save_text and not aligned:
             for m, (et, ot) in enumerate(zip(en_texts, ori_texts)): ##save each face region
                 w, h, c = et.shape
                 ot = cv2.resize(ot, (h, w))
```

### Comparing `textbsr-0.1.5/textbsr/utils/utils_image.py` & `textbsr-0.1.7/textbsr/utils/utils_image.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.1.5/textbsr.egg-info/PKG-INFO` & `textbsr-0.1.7/textbsr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textbsr
-Version: 0.1.5
+Version: 0.1.7
 Summary: a simple version for blind text image super-resolution (current version is only for English and Chinese)
 Home-page: https://github.com/csxmli2016/MARCONet
 Author: Xiaoming Li
 Author-email: csxmli@gmail.com
 License: S-Lab License 1.0
 Description: 
         # Update v0.1.2
```

