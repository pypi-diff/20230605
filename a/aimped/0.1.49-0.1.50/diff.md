# Comparing `tmp/aimped-0.1.49.tar.gz` & `tmp/aimped-0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.49.tar", last modified: Thu Jun  1 18:37:11 2023, max compression
+gzip compressed data, was "aimped-0.1.50.tar", last modified: Mon Jun  5 11:26:51 2023, max compression
```

## Comparing `aimped-0.1.49.tar` & `aimped-0.1.50.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:37:11.910787 aimped-0.1.49/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.49/LICENSE
--rw-rw-rw-   0        0        0     1778 2023-06-01 18:37:11.910787 aimped-0.1.49/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.49/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 18:37:11.861785 aimped-0.1.49/aimped/
--rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.49/aimped/__init__.py
--rw-rw-rw-   0        0        0    12497 2023-06-01 18:37:07.000000 aimped-0.1.49/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:37:11.872787 aimped-0.1.49/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/model/load.py
--rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:37:11.874788 aimped-0.1.49/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:37:11.895783 aimped-0.1.49/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.49/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.49/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.49/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:37:11.909783 aimped-0.1.49/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.49/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-06-01 18:35:47.000000 aimped-0.1.49/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:37:11.870785 aimped-0.1.49/aimped.egg-info/
--rw-rw-rw-   0        0        0     1778 2023-06-01 18:37:11.000000 aimped-0.1.49/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-01 18:37:11.000000 aimped-0.1.49/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:37:11.000000 aimped-0.1.49/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-01 18:37:11.000000 aimped-0.1.49/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 18:37:11.000000 aimped-0.1.49/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-01 18:37:11.912786 aimped-0.1.49/setup.cfg
--rw-rw-rw-   0        0        0     1163 2023-06-01 18:35:42.000000 aimped-0.1.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.685443 aimped-0.1.50/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.50/LICENSE
+-rw-rw-rw-   0        0        0     1778 2023-06-05 11:26:51.685443 aimped-0.1.50/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.50/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.628433 aimped-0.1.50/aimped/
+-rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.50/aimped/__init__.py
+-rw-rw-rw-   0        0        0    12747 2023-06-05 11:24:08.000000 aimped-0.1.50/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.641434 aimped-0.1.50/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/model/load.py
+-rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.642436 aimped-0.1.50/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.664437 aimped-0.1.50/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.50/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.50/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.50/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.683446 aimped-0.1.50/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2060 2023-06-05 10:53:19.000000 aimped-0.1.50/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-06-05 11:24:43.000000 aimped-0.1.50/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.637441 aimped-0.1.50/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1778 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-05 11:26:51.688445 aimped-0.1.50/setup.cfg
+-rw-rw-rw-   0        0        0     1163 2023-06-05 11:24:27.000000 aimped-0.1.50/setup.py
```

### Comparing `aimped-0.1.49/LICENSE` & `aimped-0.1.50/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/PKG-INFO` & `aimped-0.1.50/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.49
+Version: 0.1.50
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.aimped.ai/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **aimped**
 ![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
 
 **Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**
```

### Comparing `aimped-0.1.49/README.md` & `aimped-0.1.50/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/io_tasks.py` & `aimped-0.1.50/aimped/io_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 ################ Task: Name Entity Recognition ################
 
 class NameEntityRecognitionInput(BaseModel):
     """Input data for name entity recognition task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for NER."])
     entity: List[Any] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
 
+    class Config:
+        extra = Extra.allow
+
 
 class NameEntityRecognitionOutput(BaseModel):
     """Output data for name entity recognition task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
         default={"data_json": {"result": None}},
@@ -102,14 +105,17 @@
 ######################### Task: Deidentification #########################
 
 class DeidentificationInput(BaseModel):
     """Input data for deidentification task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for deidentification."])
     entity: List[str] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
 
+    class Config:
+        extra = Extra.allow
+
 class DeidentificationOutput(BaseModel):
     """Output data for deidentification task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
                                     default={"data_json": {"result": None}},
                                     description="Output dictionary",
@@ -145,14 +151,17 @@
                                                     {"role": "assistant", "content": "I am Chat Bot. Who are you?"},
                                                     {"role": "user", "content": "I am Joseph."}
                                                     ])
     stream: bool = False
     max_tokens: int = 256
     temperature: float = 0.7
 
+    class Config:
+        extra = Extra.allow
+
 class ChatbotOutput(BaseModel):
     """Output data for chatbot task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json", "data_audio"],
                                  description="List of data types",
                                  enum=data_types)
     # data_json: Dict[str, Any] = Field(default=None, description="Text API Output in dictionary", repr=False, exclude=True,)
@@ -203,14 +212,17 @@
 
 
 class OcrInput(BaseModel):
     """Input data for OCR task"""
     file_type: str = Field(..., description="File type image or pdf", example="image/png")
     file: str = Field(..., description="File in base64 format", example="data:image/png;base64,//tQxA-image-base64-format-string")
 
+    class Config:
+        extra = Extra.allow
+
 class OcrOutput(BaseModel):
     """Output data for OCR task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_image"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
                                     default={},
                                     description="Output dictionary",
@@ -236,14 +248,17 @@
 
 class TranslationInput(BaseModel):
     """Input data for translation task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for translation."])
     source_language: str = Field(..., description="Source language", example="en")
     output_language: str = Field(..., description="Output language", example="de")
 
+    class Config:
+        extra = Extra.allow
+
 
 class TranslationOutput(BaseModel):
     """Output data for translation task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types one or more item of data_types", enum=data_types)
     output: Dict[str, Any] = Field(
                                     default={"data_json": {"result": {'output_language':None, 'translated_text':None}}},
```

### Comparing `aimped-0.1.49/aimped/model/load.py` & `aimped-0.1.50/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/assertion.py` & `aimped-0.1.50/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/chunker.py` & `aimped-0.1.50/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/deid.py` & `aimped-0.1.50/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/ner.py` & `aimped-0.1.50/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/ner_cls_report.py` & `aimped-0.1.50/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/pipeline.py` & `aimped-0.1.50/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/regex_parser.py` & `aimped-0.1.50/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/relation.py` & `aimped-0.1.50/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/relation_visualizer.py` & `aimped-0.1.50/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/tokenizer.py` & `aimped-0.1.50/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/tools.py` & `aimped-0.1.50/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/nlp/translation.py` & `aimped-0.1.50/aimped/nlp/translation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_assertion.py` & `aimped-0.1.50/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_chunk_merger.py` & `aimped-0.1.50/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_deid_pipeline.py` & `aimped-0.1.50/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_ner_results.py` & `aimped-0.1.50/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_regex_parser.py` & `aimped-0.1.50/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_relation_pipeline.py` & `aimped-0.1.50/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_tokenizer.py` & `aimped-0.1.50/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/test/test_translation_pipeline.py` & `aimped-0.1.50/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/aimped/utils.py` & `aimped-0.1.50/aimped/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     logger.setLevel(log_level)
     logger.addHandler(f_handler)
 
     return logger
 
 def cuda_info():
     """Returns the cuda information if cuda is available."""
-    import torch
     try:
+        import torch
         if torch.cuda.is_available():
             cuda_info = {"cuda is available": torch.cuda.is_available(),
                          "device count": torch.cuda.device_count(),
                          "current device": torch.cuda.current_device(),
                          "device name": torch.cuda.get_device_name(0),
                          "Memory Usage": {"Allocated": round(torch.cuda.memory_allocated(0)/1024**3,1),
                                           "Cached": round(torch.cuda.memory_reserved(0)/1024**3,1)}}
```

### Comparing `aimped-0.1.49/aimped.egg-info/PKG-INFO` & `aimped-0.1.50/aimped.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.49
+Version: 0.1.50
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.aimped.ai/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **aimped**
 ![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
 
 **Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**
```

### Comparing `aimped-0.1.49/aimped.egg-info/SOURCES.txt` & `aimped-0.1.50/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.49/setup.py` & `aimped-0.1.50/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,10 +28,10 @@
     url="https://dev.aimped.ai/", 
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
 )
```

