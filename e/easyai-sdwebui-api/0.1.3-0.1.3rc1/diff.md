# Comparing `tmp/easyai-sdwebui-api-0.1.3.tar.gz` & `tmp/easyai-sdwebui-api-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyai-sdwebui-api-0.1.3.tar", last modified: Mon Jun  5 09:08:10 2023, max compression
+gzip compressed data, was "easyai-sdwebui-api-0.1.3rc1.tar", last modified: Mon Jun  5 08:19:34 2023, max compression
```

## Comparing `easyai-sdwebui-api-0.1.3.tar` & `easyai-sdwebui-api-0.1.3rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai-sdwebui-api-0.1.3/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai-sdwebui-api-0.1.3/.coveragerc
--rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai-sdwebui-api-0.1.3/.editorconfig
--rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai-sdwebui-api-0.1.3/.gitignore
--rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai-sdwebui-api-0.1.3/.isort.cfg
--rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai-sdwebui-api-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai-sdwebui-api-0.1.3/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.3/LICENSE
--rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai-sdwebui-api-0.1.3/Makefile
--rw-r--r--   0        0        0    10878 2023-06-05 09:07:31.290393 easyai-sdwebui-api-0.1.3/README.md
--rw-r--r--   0        0        0      712 2023-06-05 09:07:45.044970 easyai-sdwebui-api-0.1.3/easyai/__init__.py
--rw-r--r--   0        0        0     8356 2023-06-05 08:39:39.865831 easyai-sdwebui-api-0.1.3/easyai/base.py
--rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai-sdwebui-api-0.1.3/easyai/controlnet.py
--rw-r--r--   0        0        0      527 2023-06-05 08:39:39.869902 easyai-sdwebui-api-0.1.3/easyai/image.py
--rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai-sdwebui-api-0.1.3/easyai/interfaces.py
--rw-r--r--   0        0        0    11802 2023-06-05 08:39:39.873286 easyai-sdwebui-api-0.1.3/easyai/main.py
--rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai-sdwebui-api-0.1.3/easyai/result.py
--rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai-sdwebui-api-0.1.3/easyai/upscaler.py
--rw-r--r--   0        0        0     3706 2023-06-05 08:39:39.877521 easyai-sdwebui-api-0.1.3/easyai_demo.ipynb
--rw-r--r--   0        0        0     1656 2023-06-05 08:39:39.879019 easyai-sdwebui-api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai-sdwebui-api-0.1.3/setup.cfg
--rw-r--r--   0        0        0    12802 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-06-05 06:56:49.454552 easyai-sdwebui-api-0.1.3rc1/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2023-06-05 06:56:49.456491 easyai-sdwebui-api-0.1.3rc1/.coveragerc
+-rw-r--r--   0        0        0      386 2023-06-05 06:56:49.458187 easyai-sdwebui-api-0.1.3rc1/.editorconfig
+-rw-r--r--   0        0        0     6362 2023-06-05 06:56:49.461256 easyai-sdwebui-api-0.1.3rc1/.gitignore
+-rw-r--r--   0        0        0       53 2023-06-05 06:56:49.462526 easyai-sdwebui-api-0.1.3rc1/.isort.cfg
+-rw-r--r--   0        0        0      907 2023-06-05 06:56:49.463940 easyai-sdwebui-api-0.1.3rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      228 2023-06-05 06:56:49.466085 easyai-sdwebui-api-0.1.3rc1/.pylintrc
+-rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.3rc1/LICENSE
+-rw-r--r--   0        0        0     1285 2023-06-05 08:01:28.392840 easyai-sdwebui-api-0.1.3rc1/Makefile
+-rw-r--r--   0        0        0    10631 2023-06-05 06:56:49.470651 easyai-sdwebui-api-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      715 2023-06-05 08:18:50.739154 easyai-sdwebui-api-0.1.3rc1/easyai/__init__.py
+-rw-r--r--   0        0        0     8356 2023-06-05 07:57:14.930254 easyai-sdwebui-api-0.1.3rc1/easyai/base.py
+-rw-r--r--   0        0        0     2230 2023-05-26 05:21:20.240000 easyai-sdwebui-api-0.1.3rc1/easyai/controlnet.py
+-rw-r--r--   0        0        0      527 2023-05-20 01:50:59.511000 easyai-sdwebui-api-0.1.3rc1/easyai/image.py
+-rw-r--r--   0        0        0     8999 2023-05-20 01:50:59.560000 easyai-sdwebui-api-0.1.3rc1/easyai/interfaces.py
+-rw-r--r--   0        0        0    11802 2023-06-05 08:05:34.637572 easyai-sdwebui-api-0.1.3rc1/easyai/main.py
+-rw-r--r--   0        0        0      183 2023-05-20 01:50:59.560000 easyai-sdwebui-api-0.1.3rc1/easyai/result.py
+-rw-r--r--   0        0        0      822 2023-05-20 01:50:59.560000 easyai-sdwebui-api-0.1.3rc1/easyai/upscaler.py
+-rw-r--r--   0        0        0  1660710 2023-06-05 08:09:10.161477 easyai-sdwebui-api-0.1.3rc1/easyai_demo.ipynb
+-rw-r--r--   0        0        0     1656 2023-06-05 06:56:49.570893 easyai-sdwebui-api-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-05 07:00:43.510081 easyai-sdwebui-api-0.1.3rc1/setup.cfg
+-rw-r--r--   0        0        0    12558 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.3rc1/PKG-INFO
```

### Comparing `easyai-sdwebui-api-0.1.3/.gitignore` & `easyai-sdwebui-api-0.1.3rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/.pre-commit-config.yaml` & `easyai-sdwebui-api-0.1.3rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/LICENSE` & `easyai-sdwebui-api-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/Makefile` & `easyai-sdwebui-api-0.1.3rc1/Makefile`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/README.md` & `easyai-sdwebui-api-0.1.3rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easyai-sdwebui-api
+pip install easyai
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
@@ -35,22 +35,14 @@
 #api = easyai.EasyAPI(host='webui.example.com', port=443, use_https=True)
 
 # create API client with default sampler, steps.
 #api = easyai.EasyAPI(sampler='Euler a', steps=20)
 
 # optionally set username, password when --api-auth is set on webui.
 api.set_auth('username', 'password')
-
-# check controlnet version
-api.controlnet_version()
-
-# list all controlnet models
-# api.controlnet_module_list()
-# api.controlnet_model_list()
-
 ```
 
 ## txt2img
 ```
 result1 = api.txt2img(prompt="cute squirrel",
                     negative_prompt="ugly, out of frame",
                     seed=1003,
@@ -323,20 +315,16 @@
 r = api.img2img(prompt='sunset', images=[pil_img], cfg_scale=7.5, image_cfg_scale=1.5)
 r.image
 ```
 
 ### Extension support - ControlNet
 ```
 # https://github.com/Mikubill/sd-webui-controlnet
-# check controlnet version
-api.controlnet_version()
-
-# list all controlnet models
-# api.controlnet_module_list()
-# api.controlnet_model_list()
+cn = easyai.ControlNetInterface(api)
+cn.model_list()
 ```
 <pre>
 ['control_canny-fp16 [e3fe7712]',
  'control_depth-fp16 [400750f6]',
  'control_hed-fp16 [13fee50b]',
  'control_mlsd-fp16 [e3705cfa]',
  'control_normal-fp16 [63f96f7c]',
```

### Comparing `easyai-sdwebui-api-0.1.3/easyai/__init__.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             port=80,
             use_https=False,
         )
 
 
 easyai = EasyAI()
 
-__version__ = "0.1.3"
+__version__ = "0.1.3rc1"
 
 __all__ = [
     "easyai",
     "EasyAI",
     "EasyAPI",
     "ModelKeywordInterface",
     "InstructPix2PixInterface",
```

### Comparing `easyai-sdwebui-api-0.1.3/easyai/base.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/base.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/easyai/controlnet.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/controlnet.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/easyai/image.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/image.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/easyai/interfaces.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/interfaces.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/easyai/main.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/main.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/easyai/upscaler.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/upscaler.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/pyproject.toml` & `easyai-sdwebui-api-0.1.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/setup.cfg` & `easyai-sdwebui-api-0.1.3rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3/PKG-INFO` & `easyai-sdwebui-api-0.1.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyai-sdwebui-api
-Version: 0.1.3
+Version: 0.1.3rc1
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -55,15 +55,15 @@
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easyai-sdwebui-api
+pip install easyai
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
@@ -80,22 +80,14 @@
 #api = easyai.EasyAPI(host='webui.example.com', port=443, use_https=True)
 
 # create API client with default sampler, steps.
 #api = easyai.EasyAPI(sampler='Euler a', steps=20)
 
 # optionally set username, password when --api-auth is set on webui.
 api.set_auth('username', 'password')
-
-# check controlnet version
-api.controlnet_version()
-
-# list all controlnet models
-# api.controlnet_module_list()
-# api.controlnet_model_list()
-
 ```
 
 ## txt2img
 ```
 result1 = api.txt2img(prompt="cute squirrel",
                     negative_prompt="ugly, out of frame",
                     seed=1003,
@@ -368,20 +360,16 @@
 r = api.img2img(prompt='sunset', images=[pil_img], cfg_scale=7.5, image_cfg_scale=1.5)
 r.image
 ```
 
 ### Extension support - ControlNet
 ```
 # https://github.com/Mikubill/sd-webui-controlnet
-# check controlnet version
-api.controlnet_version()
-
-# list all controlnet models
-# api.controlnet_module_list()
-# api.controlnet_model_list()
+cn = easyai.ControlNetInterface(api)
+cn.model_list()
 ```
 <pre>
 ['control_canny-fp16 [e3fe7712]',
  'control_depth-fp16 [400750f6]',
  'control_hed-fp16 [13fee50b]',
  'control_mlsd-fp16 [e3705cfa]',
  'control_normal-fp16 [63f96f7c]',
```

