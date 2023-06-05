# Comparing `tmp/whitespace_correction-0.1.4-py2.py3-none-any.whl.zip` & `tmp/whitespace_correction-0.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22764 bytes, number of entries: 14
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-27 13:21 whitespace_correction/__init__.py
--rw-r--r--  2.0 unx     8128 b- defN 23-Feb-27 13:21 whitespace_correction/model.py
--rw-r--r--  2.0 unx       22 b- defN 23-Feb-27 13:21 whitespace_correction/version.py
--rw-r--r--  2.0 unx       68 b- defN 23-Feb-27 13:21 whitespace_correction/api/__init__.py
--rw-r--r--  2.0 unx     2175 b- defN 23-Feb-27 13:21 whitespace_correction/api/cli.py
--rw-r--r--  2.0 unx    20298 b- defN 23-Feb-27 13:21 whitespace_correction/api/corrector.py
--rw-r--r--  2.0 unx     4054 b- defN 23-Feb-27 13:21 whitespace_correction/api/server.py
--rw-r--r--  2.0 unx     1207 b- defN 23-Feb-27 13:21 whitespace_correction/api/train.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Feb-27 13:22 whitespace_correction-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    23129 b- defN 23-Feb-27 13:22 whitespace_correction-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-27 13:22 whitespace_correction-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Feb-27 13:22 whitespace_correction-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Feb-27 13:22 whitespace_correction-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1291 b- defN 23-Feb-27 13:22 whitespace_correction-0.1.4.dist-info/RECORD
-14 files, 72030 bytes uncompressed, 20570 bytes compressed:  71.4%
+Zip file size: 22861 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 10:17 whitespace_correction/__init__.py
+-rw-r--r--  2.0 unx     8128 b- defN 23-Jun-05 10:17 whitespace_correction/model.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 10:17 whitespace_correction/version.py
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 10:17 whitespace_correction/api/__init__.py
+-rw-r--r--  2.0 unx     1878 b- defN 23-Jun-05 10:17 whitespace_correction/api/cli.py
+-rw-r--r--  2.0 unx    20578 b- defN 23-Jun-05 10:17 whitespace_correction/api/corrector.py
+-rw-r--r--  2.0 unx     4556 b- defN 23-Jun-05 10:17 whitespace_correction/api/server.py
+-rw-r--r--  2.0 unx     1207 b- defN 23-Jun-05 10:17 whitespace_correction/api/train.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-05 10:18 whitespace_correction-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23131 b- defN 23-Jun-05 10:18 whitespace_correction-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 10:18 whitespace_correction-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 10:18 whitespace_correction-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 10:18 whitespace_correction-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1291 b- defN 23-Jun-05 10:18 whitespace_correction-0.1.5.dist-info/RECORD
+14 files, 72517 bytes uncompressed, 20667 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: whitespace_correction/api/server.py
 Comment: 
 
 Filename: whitespace_correction/api/train.py
 Comment: 
 
-Filename: whitespace_correction-0.1.4.dist-info/LICENSE
+Filename: whitespace_correction-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: whitespace_correction-0.1.4.dist-info/METADATA
+Filename: whitespace_correction-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: whitespace_correction-0.1.4.dist-info/WHEEL
+Filename: whitespace_correction-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: whitespace_correction-0.1.4.dist-info/entry_points.txt
+Filename: whitespace_correction-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: whitespace_correction-0.1.4.dist-info/top_level.txt
+Filename: whitespace_correction-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: whitespace_correction-0.1.4.dist-info/RECORD
+Filename: whitespace_correction-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## whitespace_correction/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

## whitespace_correction/api/cli.py

```diff
@@ -1,9 +1,9 @@
 from io import TextIOWrapper
-from typing import Any, Iterator, Optional, Union
+from typing import Iterator, Optional, Union
 
 from text_correction_utils.api.cli import TextCorrectionCli
 from text_correction_utils import data
 
 from whitespace_correction import version
 from whitespace_correction.api.corrector import WhitespaceCorrector
 from whitespace_correction.api.server import WhitespaceCorrectionServer
@@ -12,22 +12,14 @@
 class WhitespaceCorrectionCli(TextCorrectionCli):
     text_corrector_cls = WhitespaceCorrector
     text_correction_server_cls = WhitespaceCorrectionServer
 
     def version(self) -> str:
         return version.__version__
 
-    def format_output(self, pred: Any, ipt: data.InferenceData, lang: Optional[str]) -> str:
-        if self.args.output_format == "text":
-            return str(pred)
-        else:
-            assert lang is not None or ipt.language is not None
-            lang = lang if ipt.language is None else ipt.language
-            return f"{pred}\t{lang}"
-
     def correct_iter(
         self,
         corrector: WhitespaceCorrector,
         iter: Iterator[data.InferenceData]
     ) -> Iterator[data.InferenceData]:
         yield from corrector.correct_iter(
             ((data.text, data.language) for data in iter),
@@ -57,12 +49,14 @@
             not self.args.unsorted,
             self.args.num_threads,
             show_progress=self.args.progress
         )
 
 
 def main():
+    import warnings
+    warnings.filterwarnings("ignore")
     parser = WhitespaceCorrectionCli.parser(
         "Whitespace correction",
         "Correct missing or spurious whitespaces in text"
     )
     WhitespaceCorrectionCli(parser.parse_args()).run()
```

## whitespace_correction/api/corrector.py

```diff
@@ -2,15 +2,14 @@
 import math
 import os
 import sys
 from typing import Any, Dict, List, Tuple, Optional, Union, Iterator
 
 import torch
 from torch import nn
-from torch import autocast
 
 from whitespace_correction.model import model_from_config, EncoderDecoderWithHead
 
 from text_correction_utils import data, whitespace, tokenization
 from text_correction_utils.api.corrector import ModelInfo
 from text_correction_utils.api import corrector
 from text_correction_utils.api.utils import device_info, to
@@ -18,15 +17,15 @@
 
 _BASE_URL = "https://ad-publications.informatik.uni-freiburg.de/" \
     "ACL_whitespace_correction_transformer_BHW_2023.materials"
 _NAME_TO_ZIP = {
     "eo_large_char_v1": "eo_large_char_v1.zip",
     "eo_large_char": "eo_large_char_v2.zip",
     "eo_large_byte": "eo_large_byte_v2.zip",
-    "eo_huge_byte": "eo_huge_byte_v2.zip",
+    "eo_larger_byte": "eo_huge_byte_v2.zip",
     "eo_medium_char_v1": "eo_medium_char_v1.zip",
     "eo_medium_char": "eo_medium_char_v2.zip",
     "eo_medium_byte": "eo_medium_byte_v2.zip",
     "ed_large_char": "ed_large_v1.zip",
     "ed_medium_char": "ed_medium_v1.zip",
 }
 
@@ -35,30 +34,30 @@
     task = "whitespace correction"
 
     @classmethod
     def available_models(cls) -> List[ModelInfo]:
         return [
             ModelInfo(
                 name="eo_large_byte",
-                description="Byte-level model combining fast inference and good performance",
+                description="Byte-level model combining fast inference and good quality",
                 tags=["default", "lang::en", "arch::encoder-only", "input::byte"]
             ),
             ModelInfo(
                 name="eo_large_char",
-                description="Character-level model combining fast inference and good performance",
+                description="Character-level model combining fast inference and good quality",
                 tags=["lang::en", "arch::encoder-only", "input::char"]
             ),
             ModelInfo(
                 name="eo_large_char_v1",
-                description="Character-level model combining fast inference and good performance, "
+                description="Character-level model combining fast inference and good quality, "
                 "trained with a different loss than eo_large_char",
                 tags=["lang::en", "arch::encoder-only", "input::char"]
             ),
             ModelInfo(
-                name="eo_huge_byte",
+                name="eo_larger_byte",
                 description="Larger and slower than eo_large_byte, but also more accuracte",
                 tags=["lang::en", "arch::encoder-only", "input::byte"]
             ),
             ModelInfo(
                 name="eo_medium_byte",
                 description="Smaller and faster than eo_large_byte, but less accurate",
                 tags=["lang::en", "arch::encoder-only", "input::byte"]
@@ -71,15 +70,15 @@
             ModelInfo(
                 name="eo_medium_char_v1",
                 description="Smaller and faster than eo_large_char_v1, but less accurate",
                 tags=["lang::en", "arch::encoder-only", "input::char"]
             ),
             ModelInfo(
                 name="ed_large_char",
-                description="Similar to eo_large_byte in size and performance, but slower due to "
+                description="Similar to eo_large_byte in size and quality, but slower due to "
                 "its autoregressive decoder",
                 tags=["lang::en", "arch::encoder-decoder", "input::char", "output::char"]
             ),
             ModelInfo(
                 name="ed_medium_char",
                 description="Smaller and faster than ed_large, but less accurate",
                 tags=["lang::en", "arch::encoder-decoder", "input::char", "output::char"]
@@ -128,32 +127,33 @@
         if lang_cfg is None:
             return None
         else:
             return lang_cfg["languages"]
 
     def __init__(
         self,
-            model_dir: str,
-            device: Union[str, int]
+        model_dir: str,
+        device: Union[str, int]
     ) -> None:
         super().__init__(model_dir, device)
-        precision = self.cfg["train"].get("mixed_precision_dtype", "fp32")
-        self.set_precision(precision)
         self.logger.debug(f"loaded model config:\n{self.cfg['model']}")
         self.logger.info(f"running {self.name} whitespace corrector on device {device_info(self.device)}")
         self.input_tokenizer = tokenization.Tokenizer.from_config(self.cfg["input_tokenizer"])
         if "output_tokenizer" in self.cfg:
             self.output_tokenizer = tokenization.Tokenizer.from_config(self.cfg["output_tokenizer"])
         else:
             self.output_tokenizer = None
 
         self._encoder_only = self.cfg["model"]["type"].endswith("encoder_with_head")
         self._pfx = self.input_tokenizer.num_prefix_tokens()
         self._sfx = self.input_tokenizer.num_suffix_tokens()
 
+        precision = self.cfg["train"].get("mixed_precision_dtype", "fp32")
+        self.set_precision(precision)
+
     def _build_inference_loader_config(self) -> Dict[str, Any]:
         input_tokenizer = tokenization.Tokenizer.from_config(self.cfg["input_tokenizer"])
         pfx = input_tokenizer.num_prefix_tokens()
         sfx = input_tokenizer.num_suffix_tokens()
 
         # use the training max sequence length here, even though some models work with arbitrary long sequences
         # (e.g. LSTM), for better accuracy
@@ -489,14 +489,21 @@
             if output_file_is_str:
                 output_file.close()
 
         else:
             return (output.text for output in outputs)
 
     def set_precision(self, precision: str) -> None:
-        training_precision = self.cfg["train"].get("mixed_precision_dtype", "fp32")
-        if precision != "fp32" and precision != training_precision:
+        if self.device.type == "cpu" and self._encoder_only and precision != "fp32":
             self.logger.warning(
-                f"this model was trained with {training_precision} precision, "
-                "inference with {precision} might give unexpected results"
+                f"got {precision} precision, but "
+                "encoder-only models only support fp32 precision on CPU"
             )
+            precision = "fp32"
+        else:
+            training_precision = self.cfg["train"].get("mixed_precision_dtype", "fp32")
+            if precision != "fp32" and precision != training_precision:
+                self.logger.warning(
+                    f"this model was trained with {training_precision} precision, "
+                    f"inference with {precision} might give unexpected results"
+                )
         return super().set_precision(precision)
```

## whitespace_correction/api/server.py

```diff
@@ -11,14 +11,22 @@
 
 
 class WhitespaceCorrectionServer(TextCorrectionServer):
     text_corrector_cls = WhitespaceCorrector
 
     def __init__(self, config: Dict[str, Any]):
         super().__init__(config)
+        self.batch_size = int(self.config.get("batch_size", 16))
+        if "batch_max_tokens" in self.config:
+            self.batch_max_tokens = int(self.config["batch_max_tokens"])
+        else:
+            self.batch_max_tokens = None
+
+        for cor, _ in self.text_correctors.values():
+            cor.set_precision(self.precision)
 
         @self.server.route(f"{self.base_url}/correct", methods=["POST"])
         def _correct() -> Response:
             json = request.get_json()
             if json is None:
                 return abort(Response("request body must be json", status=400))
             elif "model" not in json:
@@ -32,15 +40,19 @@
                         return abort(cor.to_response())
                     assert isinstance(cor, WhitespaceCorrector)
                     start = time.perf_counter()
                     iter = ProgressIterator(
                         ((t, None) for t in json["text"]),
                         size_fn=lambda e: len(e[0].encode("utf8"))
                     )
-                    corrected = list(cor.correct_iter(iter))
+                    corrected = list(cor.correct_iter(
+                        iter,
+                        batch_size=self.batch_size,
+                        batch_max_tokens=self.batch_max_tokens,
+                    ))
                     end = time.perf_counter()
                     b = iter.total_size
                     s = end - start
             except Exception as error:
                 return abort(Response(f"request failed with unexpected error: {error}", status=500))
 
             return jsonify({
```

## Comparing `whitespace_correction-0.1.4.dist-info/LICENSE` & `whitespace_correction-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `whitespace_correction-0.1.4.dist-info/METADATA` & `whitespace_correction-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitespace-correction
-Version: 0.1.4
+Version: 0.1.5
 Summary: Correct missing or spurious whitespaces in text.
 Author-email: Sebastian Walter <swalter@cs.uni-freiburg.de>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,15 +212,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: text-correction-utils (>=0.1.4)
+Requires-Dist: text-correction-utils (==0.1.4)
 Requires-Dist: transformers (>=4.26.0)
 
 ## Whitespace correction using Transformers
 
 Correct missing or spurious whitespaces in text.
 
 ### Installation
@@ -383,15 +383,15 @@
 Download links:
 - [eo_large_char_v1](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_large_char_v1.zip)
 - [eo_large_char](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_large_char_v2.zip)
 - [eo_large_byte](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_large_byte_v2.zip)
 - [eo_medium_char_v1](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_medium_char_v1.zip)
 - [eo_medium_char](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_medium_char_v2.zip)
 - [eo_medium_byte](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_medium_byte_v2.zip)
-- [eo_huge_byte](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_huge_byte_v2.zip)
+- [eo_larger_byte](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/eo_huge_byte_v2.zip)
 - [ed_large_char](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/ed_large_v1.zip)
 - [ed_medium_char](https://ad-publications.informatik.uni-freiburg.de/ACL_whitespace_correction_transformer_BHW_2023.materials/ed_medium_v1.zip)
 
 #### Use own model
 
 Once you trained your own model you can use it in the following way.
```

