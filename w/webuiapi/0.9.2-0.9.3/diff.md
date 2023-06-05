# Comparing `tmp/webuiapi-0.9.2-py3-none-any.whl.zip` & `tmp/webuiapi-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12658 bytes, number of entries: 7
--rw-r--r--  2.0 unx      532 b- defN 23-Jun-01 06:33 webuiapi/__init__.py
--rw-r--r--  2.0 unx    34658 b- defN 23-Jun-01 06:33 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13529 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/RECORD
-7 files, 50444 bytes uncompressed, 11696 bytes compressed:  76.8%
+Zip file size: 12771 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      532 b- defN 23-Jun-05 08:45 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    34866 b- defN 23-Jun-05 08:45 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13529 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/RECORD
+7 files, 50652 bytes uncompressed, 11809 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.9.2.dist-info/LICENSE
+Filename: webuiapi-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.9.2.dist-info/METADATA
+Filename: webuiapi-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.9.2.dist-info/WHEEL
+Filename: webuiapi-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.9.2.dist-info/top_level.txt
+Filename: webuiapi-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.9.2.dist-info/RECORD
+Filename: webuiapi-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -8,15 +8,15 @@
     ModelKeywordResult,
     ModelKeywordInterface,
     InstructPix2PixInterface,
     ControlNetInterface,
     ControlNetUnit,
 )
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
```

## webuiapi/webuiapi.py

```diff
@@ -1,12 +1,12 @@
 import json
 import requests
 import io
 import base64
-from PIL import Image
+from PIL import Image, PngImagePlugin
 from dataclasses import dataclass
 from enum import Enum
 from typing import List, Dict, Any
 
 
 class Upscaler(str, Enum):
     none = "None"
@@ -106,29 +106,31 @@
             "guidance_start": self.guidance_start,
             "guidance_end": self.guidance_end,
             "control_mode": self.control_mode,
             "pixel_perfect": self.pixel_perfect,
         }
 
 
-def b64_img(image: Image):
-    buffered = io.BytesIO()
-    image.save(buffered, format="PNG")
-    img_base64 = "data:image/png;base64," + str(
-        base64.b64encode(buffered.getvalue()), "utf-8"
-    )
-    return img_base64
+def b64_img(image: Image) -> str:
+    return  "data:image/png;base64," + raw_b64_img(image)
 
-
-def raw_b64_img(image: Image):
+def raw_b64_img(image: Image) -> str:
     # XXX controlnet only accepts RAW base64 without headers
-    buffered = io.BytesIO()
-    image.save(buffered, format="PNG")
-    img_base64 = str(base64.b64encode(buffered.getvalue()), "utf-8")
-    return img_base64
+    with io.BytesIO() as output_bytes:
+        metadata = None
+        for key, value in image.info.items():
+            if isinstance(key, str) and isinstance(value, str):
+                if metadata is None:
+                    metadata = PngImagePlugin.PngInfo()
+                metadata.add_text(key, value)
+        image.save(output_bytes, format="PNG", pnginfo=metadata)
+
+        bytes_data = output_bytes.getvalue()
+
+    return str(base64.b64encode(bytes_data), "utf-8")
 
 
 class WebUIApi:
     has_controlnet = False
 
     def __init__(
         self,
```

## Comparing `webuiapi-0.9.2.dist-info/LICENSE` & `webuiapi-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.9.2.dist-info/METADATA` & `webuiapi-0.9.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
 Platform: UNKNOWN
```

