# Comparing `tmp/easyai-sdwebui-api-0.1.2.tar.gz` & `tmp/easyai-sdwebui-api-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyai-sdwebui-api-0.1.2.tar", last modified: Tue Apr 25 06:53:38 2023, max compression
+gzip compressed data, was "easyai-sdwebui-api-0.1.3rc1.tar", last modified: Mon Jun  5 08:19:34 2023, max compression
```

## Comparing `easyai-sdwebui-api-0.1.2.tar` & `easyai-sdwebui-api-0.1.3rc1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      193 2023-04-25 06:32:35.338110 easyai-sdwebui-api-0.1.2/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2023-04-25 06:32:35.338580 easyai-sdwebui-api-0.1.2/.coveragerc
--rw-r--r--   0        0        0      386 2023-04-25 06:32:35.338983 easyai-sdwebui-api-0.1.2/.editorconfig
--rw-r--r--   0        0        0     6362 2023-04-25 06:32:37.032590 easyai-sdwebui-api-0.1.2/.gitignore
--rw-r--r--   0        0        0       53 2023-04-25 06:32:35.339976 easyai-sdwebui-api-0.1.2/.isort.cfg
--rw-r--r--   0        0        0      907 2023-04-25 06:32:35.340381 easyai-sdwebui-api-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-04-25 06:32:35.340772 easyai-sdwebui-api-0.1.2/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.2/LICENSE
--rw-r--r--   0        0        0     1265 2023-04-25 06:32:35.367759 easyai-sdwebui-api-0.1.2/Makefile
--rw-r--r--   0        0        0    10631 2023-04-25 06:51:06.189079 easyai-sdwebui-api-0.1.2/README.md
--rw-r--r--   0        0        0      496 2023-04-25 06:51:27.190518 easyai-sdwebui-api-0.1.2/easyai/__init__.py
--rw-r--r--   0        0        0     6537 2023-04-25 06:32:35.370102 easyai-sdwebui-api-0.1.2/easyai/base.py
--rw-r--r--   0        0        0     1349 2023-04-25 06:32:35.370543 easyai-sdwebui-api-0.1.2/easyai/image.py
--rw-r--r--   0        0        0    10790 2023-04-25 06:32:35.371024 easyai-sdwebui-api-0.1.2/easyai/interfaces.py
--rw-r--r--   0        0        0    11501 2023-04-25 06:32:35.371492 easyai-sdwebui-api-0.1.2/easyai/main.py
--rw-r--r--   0        0        0      183 2023-04-25 06:32:35.371921 easyai-sdwebui-api-0.1.2/easyai/result.py
--rw-r--r--   0        0        0  1660611 2023-04-25 06:48:34.939090 easyai-sdwebui-api-0.1.2/easyai_demo.ipynb
--rw-r--r--   0        0        0     1656 2023-04-25 06:53:36.087051 easyai-sdwebui-api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2506 2023-04-25 06:49:32.224267 easyai-sdwebui-api-0.1.2/setup.cfg
--rw-r--r--   0        0        0    12555 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.2/PKG-INFO
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

### Comparing `easyai-sdwebui-api-0.1.2/.gitignore` & `easyai-sdwebui-api-0.1.3rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.2/.pre-commit-config.yaml` & `easyai-sdwebui-api-0.1.3rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.2/LICENSE` & `easyai-sdwebui-api-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.2/Makefile` & `easyai-sdwebui-api-0.1.3rc1/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 clean: ## Removing cached python compiled files
 	find . -name \*pyc  | xargs  rm -rfv
 	find . -name \*pyo | xargs  rm -fv
 	find . -name \*~  | xargs  rm -fv
 	find . -name __pycache__  | xargs  rm -rfv
 
 install: ## Install dependencies
+	pip install flit
 	make clean
 	flit install --deps develop --symlink
 	pre-commit install
 
 lint: ## Run code linters
 	autoflake --remove-all-unused-imports --remove-unused-variables  --ignore-init-module-imports -r easyai
 	black --check easyai tests
 	isort --check easyai tests
 	flake8
-	mypy easy
+	mypy easyai
 
 fmt format: ## Run code formatters
 	autoflake --in-place --remove-all-unused-imports --remove-unused-variables --ignore-init-module-imports  -r easyai
 	isort easyai
 	black easyai
 
 test: ## Run tests
```

### Comparing `easyai-sdwebui-api-0.1.2/README.md` & `easyai-sdwebui-api-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.2/easyai/base.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import io
 import json
 
 import requests
 from PIL import Image
 
 from .image import b64_img
-from .result import ApiResult
+from .result import APIResult
 
 
 class WebUIAPIBase:
+    has_controlnet = False
+
     def __init__(
         self,
         host="127.0.0.1",
         port=7860,
         baseurl=None,
         sampler="Euler a",
         steps=20,
@@ -27,14 +29,23 @@
 
         self.baseurl = baseurl
         self.default_sampler = sampler
         self.default_steps = steps
 
         self.session = requests.Session()
 
+        self.check_controlnet()
+
+    def check_controlnet(self):
+        try:
+            scripts = self.get_scripts()
+            self.has_controlnet = "controlnet m2m" in scripts["txt2img"]
+        except:  # NOQA
+            pass
+
     def set_auth(self, username, password):
         self.session.auth = (username, password)
 
     def _to_api_result(self, response):
         if response.status_code != 200:
             raise RuntimeError(response.status_code, response.text)
 
@@ -56,15 +67,15 @@
         elif "caption" in r.keys():
             info = r["caption"]
 
         parameters = ""
         if "parameters" in r.keys():
             parameters = r["parameters"]
 
-        return ApiResult(images, parameters, info)
+        return APIResult(images, parameters, info)
 
     # XXX 500 error (2022/12/26)
     def png_info(self, image):
         payload = {
             "image": b64_img(image),
         }
 
@@ -76,30 +87,38 @@
         payload = {
             "image": b64_img(image),
         }
 
         response = self.session.post(url=f"{self.baseurl}/interrogate", json=payload)
         return self._to_api_result(response)
 
+    def interrupt(self):
+        response = self.session.post(url=f"{self.baseurl}/interrupt")
+        return response.json()
+
+    def skip(self):
+        response = self.session.post(url=f"{self.baseurl}/skip")
+        return response.json()
+
     def get_options(self):
         response = self.session.get(url=f"{self.baseurl}/options")
         return response.json()
 
     def set_options(self, options):
         response = self.session.post(url=f"{self.baseurl}/options", json=options)
         return response.json()
 
-    def get_progress(self):
-        response = self.session.get(url=f"{self.baseurl}/progress")
-        return response.json()
-
     def get_cmd_flags(self):
         response = self.session.get(url=f"{self.baseurl}/cmd-flags")
         return response.json()
 
+    def get_progress(self):
+        response = self.session.get(url=f"{self.baseurl}/progress")
+        return response.json()
+
     def get_samplers(self):
         response = self.session.get(url=f"{self.baseurl}/samplers")
         return response.json()
 
     def get_upscalers(self):
         response = self.session.get(url=f"{self.baseurl}/upscalers")
         return response.json()
@@ -120,26 +139,38 @@
         response = self.session.get(url=f"{self.baseurl}/realesrgan-models")
         return response.json()
 
     def get_prompt_styles(self):
         response = self.session.get(url=f"{self.baseurl}/prompt-styles")
         return response.json()
 
-    def get_artist_categories(self):
+    def get_artist_categories(self):  # deprecated ?
         response = self.session.get(url=f"{self.baseurl}/artist-categories")
         return response.json()
 
-    def get_artists(self):
+    def get_artists(self):  # deprecated ?
         response = self.session.get(url=f"{self.baseurl}/artists")
         return response.json()
 
     def refresh_checkpoints(self):
         response = self.session.post(url=f"{self.baseurl}/refresh-checkpoints")
         return response.json()
 
+    def get_scripts(self):
+        response = self.session.get(url=f"{self.baseurl}/scripts")
+        return response.json()
+
+    def get_embeddings(self):
+        response = self.session.get(url=f"{self.baseurl}/embeddings")
+        return response.json()
+
+    def get_memory(self):
+        response = self.session.get(url=f"{self.baseurl}/memory")
+        return response.json()
+
     def get_endpoint(self, endpoint, baseurl):
         if baseurl:
             return f"{self.baseurl}/{endpoint}"
         else:
             from urllib.parse import urlparse, urlunparse
 
             parsed_url = urlparse(self.baseurl)
@@ -153,14 +184,40 @@
         return response.json()
 
     def custom_post(self, endpoint, payload={}, baseurl=False):
         url = self.get_endpoint(endpoint, baseurl)
         response = self.session.post(url=url, json=payload)
         return self._to_api_result(response)
 
+    def controlnet_version(self):
+        r = self.custom_get("controlnet/version")
+        return r["version"]
+
+    def controlnet_model_list(self):
+        r = self.custom_get("controlnet/model_list")
+        return r["model_list"]
+
+    def controlnet_module_list(self):
+        r = self.custom_get("controlnet/module_list")
+        return r["module_list"]
+
+    def controlnet_detect(
+        self, images, module="none", processor_res=512, threshold_a=64, threshold_b=64
+    ):
+        input_images = [b64_img(x) for x in images]
+        payload = {
+            "controlnet_module": module,
+            "controlnet_input_images": input_images,
+            "controlnet_processor_res": processor_res,
+            "controlnet_threshold_a": threshold_a,
+            "controlnet_threshold_b": threshold_b,
+        }
+        r = self.custom_post("controlnet/detect", payload=payload)
+        return r
+
     def util_get_model_names(self):
         return sorted([x["title"] for x in self.get_sd_models()])
 
     def util_set_model(self, name, find_closest=True):
         if find_closest:
             name = name.lower()
         models = self.util_get_model_names()
```

### Comparing `easyai-sdwebui-api-0.1.2/easyai/interfaces.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/interfaces.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 """Interface for extensions"""
 from dataclasses import dataclass
 from typing import Any, Dict
 
-from PIL import Image
-
 from .image import b64_img, raw_b64_img
 
-# https://github.com/mix1009/model-keyword
-
 
 @dataclass
 class ModelKeywordResult:
     keywords: list
     model: str
     oldhash: str
     match_source: str
 
 
 class ModelKeywordInterface:
+    """https://github.com/mix1009/model-keyword"""
+
     def __init__(self, easyai):
         self.api = easyai
 
     def get_keywords(self):
         result = self.api.custom_get("model_keyword/get_keywords")
         keywords = result["keywords"]
         model = result["model"]
         oldhash = result["hash"]
         match_source = result["match_source"]
         return ModelKeywordResult(keywords, model, oldhash, match_source)
 
 
-# https://github.com/Klace/stable-diffusion-webui-instruct-pix2pix
-
-
 class InstructPix2PixInterface:
+    """https://github.com/Klace/stable-diffusion-webui-instruct-pix2pix"""
+
     def __init__(self, easyai):
         self.api = easyai
 
     def img2img(
         self,
         images=[],
         prompt: str = "",
@@ -66,67 +63,14 @@
             "image_cfg": image_cfg,
             "randomize_cfg": randomize_cfg,
             "output_image_width": output_image_width,
         }
         return self.api.custom_post("instruct-pix2pix/img2img", payload=payload)
 
 
-# https://github.com/Mikubill/sd-webui-controlnet
-class ControlNetUnit:
-    def __init__(
-        self,
-        input_image: Image = None,
-        mask: Image = None,
-        module: str = "none",
-        model: str = "None",
-        weight: float = 1.0,
-        resize_mode: str = "Scale to Fit (Inner Fit)",
-        lowvram: bool = False,
-        processor_res: int = 64,
-        threshold_a: float = 64,
-        threshold_b: float = 64,
-        guidance: float = 1.0,
-        guidance_start: float = 0.0,
-        guidance_end: float = 1.0,
-        guessmode: bool = False,
-    ):
-        self.input_image = input_image
-        self.mask = mask
-        self.module = module
-        self.model = model
-        self.weight = weight
-        self.resize_mode = resize_mode
-        self.lowvram = lowvram
-        self.processor_res = processor_res
-        self.threshold_a = threshold_a
-        self.threshold_b = threshold_b
-        self.guidance = guidance
-        self.guidance_start = guidance_start
-        self.guidance_end = guidance_end
-        self.guessmode = guessmode
-
-    def to_dict(self):
-        return {
-            "input_image": raw_b64_img(self.input_image) if self.input_image else "",
-            "mask": raw_b64_img(self.mask) if self.mask else "",
-            "module": self.module,
-            "model": self.model,
-            "weight": self.weight,
-            "resize_mode": self.resize_mode,
-            "lowvram": self.lowvram,
-            "processor_res": self.processor_res,
-            "threshold_a": self.threshold_a,
-            "threshold_b": self.threshold_b,
-            "guidance": self.guidance,
-            "guidance_start": self.guidance_start,
-            "guidance_end": self.guidance_end,
-            "guessmode": self.guessmode,
-        }
-
-
 class ControlNetInterface:
     def __init__(self, easyai, show_deprecation_warning=True):
         self.api = easyai
         self.show_deprecation_warning = show_deprecation_warning
 
     def print_deprecation_warning(self):
         print(
```

### Comparing `easyai-sdwebui-api-0.1.2/easyai/main.py` & `easyai-sdwebui-api-0.1.3rc1/easyai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List
 
 from .base import WebUIAPIBase
-from .image import HiResUpscaler, b64_img
-from .interfaces import ControlNetUnit
+from .controlnet import ControlNetUnit
+from .image import b64_img
+from .upscaler import HiResUpscaler
 
 
 class EasyAPI(WebUIAPIBase):
     def txt2img(
         self,
         enable_hr=False,
         denoising_strength=0.7,
@@ -109,14 +110,18 @@
             return self.custom_post("controlnet/txt2img", payload=payload)
 
         if controlnet_units and len(controlnet_units) > 0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
 
+        elif self.has_controlnet:
+            # workaround : if not passed, webui will use previous args!
+            payload["alwayson_scripts"]["ControlNet"] = {"args": []}
+
         response = self.session.post(url=f"{self.baseurl}/txt2img", json=payload)
         return self._to_api_result(response)
 
     def img2img(
         self,
         images=[],  # list of PIL Image
         resize_mode=0,
@@ -226,14 +231,17 @@
             payload["controlnet_units"] = [x.to_dict() for x in controlnet_units]
             return self.custom_post("controlnet/img2img", payload=payload)
 
         if controlnet_units and len(controlnet_units) > 0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
+        elif self.has_controlnet:
+            payload["alwayson_scripts"]["ControlNet"] = {"args": []}
+
         response = self.session.post(url=f"{self.baseurl}/img2img", json=payload)
         return self._to_api_result(response)
 
     def extra_single_image(
         self,
         image,  # PIL Image
         resize_mode=0,
```

### Comparing `easyai-sdwebui-api-0.1.2/easyai_demo.ipynb` & `easyai-sdwebui-api-0.1.3rc1/easyai_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'cells'": "{insert: [(2, OrderedDict([('cell_type', 'markdown'), ('source', []), ('metadata', "*

 * *            "OrderedDict([('collapsed', False)]))]))]}"}*

```diff
@@ -36,14 +36,21 @@
                 "# list all controlnet models\n",
                 "control_net = easyai.ControlNetInterface(api)\n",
                 "control_net.model_list()"
             ]
         },
         {
             "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": []
+        },
+        {
+            "cell_type": "markdown",
             "id": "2f613b8c-d5ad-4572-8b04-e929a6b11421",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
             },
             "source": [
                 "# Create a test image"
```

### Comparing `easyai-sdwebui-api-0.1.2/pyproject.toml` & `easyai-sdwebui-api-0.1.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.2/setup.cfg` & `easyai-sdwebui-api-0.1.3rc1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -21,22 +21,14 @@
     E203,
     E501,
     C901
 per-file-ignores =
     # F401: imported but unused
     # F403: import * used; unable to detect undefined names
     __init__.py: F401,F403
-    # F405: XXX may be undefined, or defined from star imports
-    api_ci.py: F405
-    api_dev.py: F405
-    api_stag.py: F405
-    api_test.py: F405
-    prod.py: F405
-    local.py: F405, E121
-    local-default.py: F405
 
 exclude =
     .tox,
     */migrations/*,
     */static/CACHE/*,
     docs,
     node_modules,
```

### Comparing `easyai-sdwebui-api-0.1.2/PKG-INFO` & `easyai-sdwebui-api-0.1.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyai-sdwebui-api
-Version: 0.1.2
+Version: 0.1.3rc1
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

