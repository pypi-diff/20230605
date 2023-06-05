# Comparing `tmp/onnx_clip-2.3.0.tar.gz` & `tmp/onnx_clip-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx_clip-2.3.0.tar", max compression
+gzip compressed data, was "onnx_clip-3.0.0.tar", max compression
```

## Comparing `onnx_clip-2.3.0.tar` & `onnx_clip-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-02-06 16:20:44.660387 onnx_clip-2.3.0/LICENSE
--rw-r--r--   0        0        0     3521 2023-02-08 12:52:08.334182 onnx_clip-2.3.0/README.md
--rw-r--r--   0        0        0      393 2023-05-02 08:27:40.190660 onnx_clip-2.3.0/onnx_clip/__init__.py
--rw-r--r--   0        0        0       43 2023-02-06 16:20:44.660994 onnx_clip-2.3.0/onnx_clip/data/.gitattributes
--rw-r--r--   0        0        0   252444 2023-02-06 16:20:44.662626 onnx_clip-2.3.0/onnx_clip/data/CLIP.png
--rw-r--r--   0        0        0  1356917 2023-02-06 16:20:44.664095 onnx_clip-2.3.0/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0        0        0   602240 2023-02-06 16:20:44.666081 onnx_clip-2.3.0/onnx_clip/data/expected_preprocessed_image.npy
--rw-r--r--   0        0        0    80530 2023-02-06 16:20:44.666325 onnx_clip-2.3.0/onnx_clip/data/franz-kafka.jpg
--rw-r--r--   0        0        0    10104 2023-04-25 08:59:00.089438 onnx_clip-2.3.0/onnx_clip/model.py
--rw-r--r--   0        0        0     6898 2023-02-08 12:52:08.334682 onnx_clip-2.3.0/onnx_clip/preprocessor.py
--rw-r--r--   0        0        0     7659 2023-02-08 12:52:08.335075 onnx_clip-2.3.0/onnx_clip/tokenizer.py
--rw-r--r--   0        0        0      737 2023-05-02 08:26:53.371378 onnx_clip-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 onnx_clip-2.3.0/setup.py
--rw-r--r--   0        0        0     4516 1970-01-01 00:00:00.000000 onnx_clip-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-26 14:28:02.956223 onnx_clip-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3521 2023-05-26 14:28:02.956375 onnx_clip-3.0.0/README.md
+-rw-r--r--   0        0        0      393 2023-06-05 07:29:34.069013 onnx_clip-3.0.0/onnx_clip/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-26 14:28:02.956934 onnx_clip-3.0.0/onnx_clip/data/.gitattributes
+-rw-r--r--   0        0        0   252444 2023-05-26 14:28:02.958500 onnx_clip-3.0.0/onnx_clip/data/CLIP.png
+-rw-r--r--   0        0        0  1356917 2023-05-26 14:28:02.960272 onnx_clip-3.0.0/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0   602240 2023-05-26 14:28:02.962273 onnx_clip-3.0.0/onnx_clip/data/expected_preprocessed_image.npy
+-rw-r--r--   0        0        0    80530 2023-05-26 14:28:02.962532 onnx_clip-3.0.0/onnx_clip/data/franz-kafka.jpg
+-rw-r--r--   0        0        0    10985 2023-06-05 07:29:10.831158 onnx_clip-3.0.0/onnx_clip/model.py
+-rw-r--r--   0        0        0     6955 2023-06-05 07:29:10.831843 onnx_clip-3.0.0/onnx_clip/preprocessor.py
+-rw-r--r--   0        0        0     7659 2023-05-26 14:28:02.962928 onnx_clip-3.0.0/onnx_clip/tokenizer.py
+-rw-r--r--   0        0        0      737 2023-06-05 07:29:10.832260 onnx_clip-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 onnx_clip-3.0.0/PKG-INFO
```

### Comparing `onnx_clip-2.3.0/LICENSE` & `onnx_clip-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.3.0/README.md` & `onnx_clip-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.3.0/onnx_clip/data/CLIP.png` & `onnx_clip-3.0.0/onnx_clip/data/CLIP.png`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.3.0/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz` & `onnx_clip-3.0.0/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.3.0/onnx_clip/data/expected_preprocessed_image.npy` & `onnx_clip-3.0.0/onnx_clip/data/expected_preprocessed_image.npy`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.3.0/onnx_clip/data/franz-kafka.jpg` & `onnx_clip-3.0.0/onnx_clip/data/franz-kafka.jpg`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.3.0/onnx_clip/model.py` & `onnx_clip-3.0.0/onnx_clip/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,50 +101,69 @@
     This class can be utilised to predict the most relevant text snippet, given
     an image, without directly optimizing for the task, similarly to the
     zero-shot capabilities of GPT-2 and 3. The difference between this class
     and [CLIP](https://github.com/openai/CLIP) is that here we don't depend on
     `torch` or `torchvision`.
     """
 
-    # The length of each embedding array
-    EMBEDDING_SIZE = 512
 
     def __init__(
-        self, batch_size: Optional[int] = None, silent_download: bool = False
+        self, model: str = "ViT-B/32", batch_size: Optional[int] = None, silent_download: bool = False
     ):
         """
         Instantiates the model and required encoding classes.
 
         Args:
+            model: The model to utilise. Currently ViT-B/32 and RN50 are
+                allowed.
             batch_size: If set, splits the lists in `get_image_embeddings`
                 and `get_text_embeddings` into batches of this size before
                 passing them to the model. The embeddings are then concatenated
                 back together before being returned. This is necessary when
                 passing large amounts of data (perhaps ~100 or more).
             silent_download: If True, the function won't show a warning in
                 case when the models need to be downloaded from the S3 bucket.
         """
-        self.image_model, self.text_model = self._load_models(silent_download)
+        allowed_models = ["ViT-B/32", "RN50"]
+        if model not in allowed_models:
+            raise ValueError(f"`model` must be in {allowed_models}. Got {model}.")
+        if model == "ViT-B/32":
+            self.embedding_size = 512
+        elif model == "RN50":
+            self.embedding_size = 1024
+        self.image_model, self.text_model = self._load_models(model, silent_download)
         self._tokenizer = Tokenizer()
         self._preprocessor = Preprocessor()
         self._batch_size = batch_size
+    
+    @property
+    def EMBEDDING_SIZE(self):
+        raise RuntimeError("OnnxModel.EMBEDDING_SIZE is no longer supported, please use the instance attribute: onnx_model.embedding_size")
+
 
     @staticmethod
     def _load_models(
+        model: str,
         silent: bool,
     ) -> Tuple[ort.InferenceSession, ort.InferenceSession]:
         """
-        Grabs the ONNX implementation of CLIP's ViT-B/32 :
+        Grabs the ONNX implementation of CLIP's model :
         https://github.com/openai/CLIP/blob/main/clip/model.py
 
         We have exported it to ONNX to remove the dependency on `torch` and
         `torchvision`.
         """
-        IMAGE_MODEL_FILE = "clip_image_model_vitb32.onnx"
-        TEXT_MODEL_FILE = "clip_text_model_vitb32.onnx"
+        if model == "ViT-B/32":
+            IMAGE_MODEL_FILE = "clip_image_model_vitb32.onnx"
+            TEXT_MODEL_FILE = "clip_text_model_vitb32.onnx"
+        elif model == "RN50":
+            IMAGE_MODEL_FILE = "clip_image_model_rn50.onnx"
+            TEXT_MODEL_FILE = "clip_text_model_rn50.onnx"
+        else:
+            raise ValueError(f"Unexpected model {model}. No `.onnx` file found.")
         base_dir = os.path.dirname(os.path.abspath(__file__))
 
         models = []
         for model_file in [IMAGE_MODEL_FILE, TEXT_MODEL_FILE]:
             path = os.path.join(base_dir, "data", model_file)
             models.append(OnnxClip._load_model(path, silent))
 
@@ -194,15 +213,15 @@
             images: A list of images to run on. Each image must be a 3-channel
                 (RGB) image. Can be any size, as the preprocessing step will
                 resize each image to size (224, 224).
             with_batching: Whether to use batching - see the `batch_size` param
                 in `__init__()`
 
         Returns:
-            An array of embeddings of shape (len(images), 512).
+            An array of embeddings of shape (len(images), embedding_size).
         """
         if not with_batching or self._batch_size is None:
             # Preprocess images
             images = [
                 self._preprocessor.encode_image(image) for image in images
             ]
             if not images:
@@ -232,15 +251,15 @@
         Args:
             texts: A list of texts to run on. Each entry can be at most
                 77 characters.
             with_batching: Whether to use batching - see the `batch_size` param
                 in `__init__()`
 
         Returns:
-            An array of embeddings of shape (len(texts), 512).
+            An array of embeddings of shape (len(texts), embedding_size).
         """
         if not with_batching or self._batch_size is None:
             text = self._tokenizer.encode_text(texts)
             if len(text) == 0:
                 return self._get_empty_embedding()
 
             return self.text_model.run(None, {"TEXT": text})[0]
@@ -253,15 +272,15 @@
 
             if not embeddings:
                 return self._get_empty_embedding()
 
             return np.concatenate(embeddings)
 
     def _get_empty_embedding(self):
-        return np.empty((0, OnnxClip.EMBEDDING_SIZE), dtype=np.float32)
+        return np.empty((0, self.embedding_size), dtype=np.float32)
 
 
 T = TypeVar("T")
 
 
 def to_batches(items: Iterable[T], size: int) -> Iterator[List[T]]:
     """
```

### Comparing `onnx_clip-2.3.0/onnx_clip/preprocessor.py` & `onnx_clip-3.0.0/onnx_clip/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import cv2 as cv
 import numpy as np
 from PIL import Image
 
 
 class Preprocessor:
     """
-    A rough approximation to the CLIP `preprocess` neural net.
+    Our approach to the CLIP `preprocess` neural net that does not rely on PyTorch.
+    The two approaches fully match.
     """
 
     # Fixed variables that ensure the correct output shapes and values for the `Model` class.
     CLIP_INPUT_SIZE = 224
     # Normalization constants taken from original CLIP:
     # https://github.com/openai/CLIP/blob/3702849800aa56e2223035bccd1c6ef91c704ca8/clip/clip.py#L85
     NORM_MEAN = np.array([0.48145466, 0.4578275, 0.40821073]).reshape(
```

### Comparing `onnx_clip-2.3.0/onnx_clip/tokenizer.py` & `onnx_clip-3.0.0/onnx_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.3.0/pyproject.toml` & `onnx_clip-3.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "onnx_clip"
-version = "2.3.0"
+version = "3.0.0"
 description = "CLIP with ONNX Runtime and without PyTorch dependencies."
 readme = "README.md"
 authors = ["Lakera AI <dev@lakera.ai>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `onnx_clip-2.3.0/PKG-INFO` & `onnx_clip-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: onnx-clip
-Version: 2.3.0
+Version: 3.0.0
 Summary: CLIP with ONNX Runtime and without PyTorch dependencies.
 Author: Lakera AI
 Author-email: dev@lakera.ai
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: boto3 (>=1.23.10,<2.0.0)
 Requires-Dist: ftfy (>=6.0.3,<7.0.0)
 Requires-Dist: importlib_metadata (>=4.8)
 Requires-Dist: numpy (>=1.18.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.4.0)
 Requires-Dist: opencv-python-headless (>=4.0.1,<5.0.0)
 Requires-Dist: pillow (>=8.4.0,<9.0.0)
```

