# Comparing `tmp/pydoxtools-0.6.3.tar.gz` & `tmp/pydoxtools-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoxtools-0.6.3.tar", max compression
+gzip compressed data, was "pydoxtools-0.6.4.tar", max compression
```

## Comparing `pydoxtools-0.6.3.tar` & `pydoxtools-0.6.4.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0     1072 2023-03-29 07:08:59.780129 pydoxtools-0.6.3/LICENSE
--rw-r--r--   0        0        0     8260 2023-05-25 18:58:37.513803 pydoxtools-0.6.3/README.md
--rw-r--r--   0        0        0      261 2023-05-29 20:02:49.181016 pydoxtools-0.6.3/pydoxtools/__init__.py
--rw-r--r--   0        0        0    12096 2023-05-29 21:07:28.688538 pydoxtools-0.6.3/pydoxtools/agent.py
--rw-r--r--   0        0        0     2508 2022-02-03 10:08:19.000000 pydoxtools-0.6.3/pydoxtools/class_utils.py
--rwxr-xr-x   0        0        0    30541 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/classifier.py
--rw-r--r--   0        0        0    29431 2022-09-09 18:06:03.434226 pydoxtools-0.6.3/pydoxtools/cluster_utils.py
--rw-r--r--   0        0        0     6047 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/dask_operators.py
--rw-r--r--   0        0        0    54044 2023-05-29 18:22:59.945511 pydoxtools-0.6.3/pydoxtools/document.py
--rw-r--r--   0        0        0    35071 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/document_base.py
--rw-r--r--   0        0        0     1673 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_classes.py
--rw-r--r--   0        0        0     3978 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_filesystem.py
--rw-r--r--   0        0        0    13329 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_html.py
--rw-r--r--   0        0        0    12566 2023-05-27 05:02:18.158595 pydoxtools-0.6.3/pydoxtools/extract_index.py
--rw-r--r--   0        0        0     5965 2023-05-29 18:22:59.945511 pydoxtools-0.6.3/pydoxtools/extract_nlpchat.py
--rw-r--r--   0        0        0     2469 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_objects.py
--rw-r--r--   0        0        0     1656 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_ocr.py
--rw-r--r--   0        0        0     6469 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_pandoc.py
--rw-r--r--   0        0        0     5544 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_spacy.py
--rw-r--r--   0        0        0    43269 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_tables.py
--rw-r--r--   0        0        0     8139 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_textstructure.py
--rw-r--r--   0        0        0     1232 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/file_utils.py
--rwxr-xr-x   0        0        0     6143 2022-09-14 22:13:53.783991 pydoxtools-0.6.3/pydoxtools/html_utils.py
--rw-r--r--   0        0        0      150 2022-02-03 10:08:19.000000 pydoxtools-0.6.3/pydoxtools/initialize_library.py
--rw-r--r--   0        0        0     7077 2022-09-09 18:06:03.434226 pydoxtools-0.6.3/pydoxtools/labeling.py
--rw-r--r--   0        0        0     7364 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/list_utils.py
--rw-r--r--   0        0        0      371 2022-09-09 18:06:03.434226 pydoxtools-0.6.3/pydoxtools/math_utils.py
--rw-r--r--   0        0        0     2431 2022-09-13 15:47:40.161989 pydoxtools-0.6.3/pydoxtools/models.py
--rwxr-xr-x   0        0        0    18776 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/nlp_utils.py
--rw-r--r--   0        0        0     2502 2022-03-25 12:06:42.174796 pydoxtools-0.6.3/pydoxtools/ocr_language_mappings.py
--rw-r--r--   0        0        0     8897 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/operator_huggingface.py
--rw-r--r--   0        0        0     1134 2023-05-29 18:22:59.945511 pydoxtools-0.6.3/pydoxtools/operators.py
--rw-r--r--   0        0        0     7856 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/operators_base.py
--rwxr-xr-x   0        0        0    12146 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/pdf_utils.py
--rw-r--r--   0        0        0    34126 2023-03-29 07:08:59.788125 pydoxtools-0.6.3/pydoxtools/random_data_generators.py
--rwxr-xr-x   0        0        0     1332 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/settings.py
--rw-r--r--   0        0        0    17693 2023-05-25 18:58:37.525804 pydoxtools-0.6.3/pydoxtools/training.py
--rw-r--r--   0        0        0     3898 2022-02-03 10:08:19.000000 pydoxtools-0.6.3/pydoxtools/visual_document_analysis.py
--rw-r--r--   0        0        0     3209 2023-03-29 07:08:59.788125 pydoxtools-0.6.3/pydoxtools/webdav_utils.py
--rw-r--r--   0        0        0     5930 2023-05-29 21:49:19.710912 pydoxtools-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    11084 1970-01-01 00:00:00.000000 pydoxtools-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-29 07:08:59.780129 pydoxtools-0.6.4/LICENSE
+-rw-r--r--   0        0        0     8260 2023-05-25 18:58:37.513803 pydoxtools-0.6.4/README.md
+-rw-r--r--   0        0        0      353 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/__init__.py
+-rw-r--r--   0        0        0    12308 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/agent.py
+-rw-r--r--   0        0        0     2501 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/class_utils.py
+-rwxr-xr-x   0        0        0    30464 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/classifier.py
+-rw-r--r--   0        0        0    29499 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/cluster_utils.py
+-rw-r--r--   0        0        0     6139 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/dask_operators.py
+-rw-r--r--   0        0        0    54128 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/document.py
+-rw-r--r--   0        0        0    35236 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/document_base.py
+-rw-r--r--   0        0        0     1765 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_classes.py
+-rw-r--r--   0        0        0     4065 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_filesystem.py
+-rw-r--r--   0        0        0    13396 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_html.py
+-rw-r--r--   0        0        0    12658 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_index.py
+-rw-r--r--   0        0        0     6069 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_nlpchat.py
+-rw-r--r--   0        0        0     2561 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_objects.py
+-rw-r--r--   0        0        0     1750 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_ocr.py
+-rw-r--r--   0        0        0     6561 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_pandoc.py
+-rw-r--r--   0        0        0     5570 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_spacy.py
+-rw-r--r--   0        0        0    43343 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_tables.py
+-rw-r--r--   0        0        0     8231 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_textstructure.py
+-rw-r--r--   0        0        0     1324 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/file_utils.py
+-rwxr-xr-x   0        0        0     6187 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/html_utils.py
+-rw-r--r--   0        0        0     7167 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/labeling.py
+-rw-r--r--   0        0        0     7327 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/list_utils.py
+-rw-r--r--   0        0        0      466 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/math_utils.py
+-rw-r--r--   0        0        0     2499 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/models.py
+-rwxr-xr-x   0        0        0    18805 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/nlp_utils.py
+-rw-r--r--   0        0        0     2504 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/ocr_language_mappings.py
+-rw-r--r--   0        0        0     8965 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/operator_huggingface.py
+-rw-r--r--   0        0        0     1134 2023-06-04 22:57:01.069614 pydoxtools-0.6.4/pydoxtools/operators.py
+-rw-r--r--   0        0        0     7947 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/operators_base.py
+-rwxr-xr-x   0        0        0    12182 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/pdf_utils.py
+-rw-r--r--   0        0        0    34121 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/random_data_generators.py
+-rwxr-xr-x   0        0        0     1400 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/settings.py
+-rw-r--r--   0        0        0    17775 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/training.py
+-rw-r--r--   0        0        0     3990 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/visual_document_analysis.py
+-rw-r--r--   0        0        0     3301 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/webdav_utils.py
+-rw-r--r--   0        0        0     5988 2023-06-05 05:55:24.817152 pydoxtools-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    11246 1970-01-01 00:00:00.000000 pydoxtools-0.6.4/PKG-INFO
```

### Comparing `pydoxtools-0.6.3/LICENSE` & `pydoxtools-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.3/README.md` & `pydoxtools-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.3/pydoxtools/agent.py` & `pydoxtools-0.6.4/pydoxtools/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import logging
 import uuid
 
 import chromadb
 import dask.diagnostics
 import numpy as np
@@ -81,14 +83,15 @@
         self._data_source: pdx.DocumentBag | None = data_source
         # we need to delete all previously stored "dynamic" information generated
         # by the agent in most cases to make our information
         # search more efficient and deduplicate information
         # TODO: make agents reuse information in the future!
         if startfresh:
             self.chromadb_collection.delete(where=self._context_where_all)
+            self.chromadb_client.persist()
 
     @property
     def collection_name(self):
         return "pdx_agent_index"
 
     def reload_vector_store(self):
         """sometimes we need to reload the vector store. For example if we have added nwe data from
@@ -183,17 +186,18 @@
             context_size: int = 5,
             previous_task_size=0,
             max_tokens=256,
             formatting="yaml",
             save_task=False
     ):
         if context_size:
-            context = self.get_context(task,
-                                       where_clause=self._context_where_info,
-                                       n_results=context_size)[0]
+            context = self.get_context(
+                task,
+                where_clause=self._context_where_info,
+                n_results=context_size)[0]
         else:
             context = ""
         # TODO: if we had this exact task in an earlier iteration..
         #       evaluate if we have to do it again or already have our answer...
         if previous_task_size:
             previous_tasks = self.get_context(
                 task, where_clause=self._context_where_tasks,
@@ -254,14 +258,15 @@
         #       only a single word...
         #       also, try this "local" strategy to answer questions...
         # anslist = pd.DataFrame(Document(txt).answers(question)[0])
         # if not anslist.empty:
         #    ans = anslist.groupby(0).sum().sort_values(by=1, ascending=False).index[0]
         # else:
         # TODO: should we save the question?
+        """If you don't know the answer, just say that you don't know, don't try to make up an answer."""
         res = self.execute_task(task=f"answer the following question: '{question}' "
                                      f"using this text as input: {txt}", formatting="txt")
         ans = res
         # TODO: ask questions like "is this correct?" or can you provide the name?
         # ans_parsed = yaml.unsafe_load(ans)
         self.add_question(question, ans)
         return ans
```

### Comparing `pydoxtools-0.6.3/pydoxtools/class_utils.py` & `pydoxtools-0.6.4/pydoxtools/class_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from abc import get_cache_token
-from collections import namedtuple
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 # import types, weakref  # Deferred to single_dispatch()
-from reprlib import recursive_repr
 from _thread import RLock
 
 # TODO: remove the following function if we update our python requirements to be
 #       >= 3.8 (cached_property is supportd natively onwards from that...)
 
 # TODO: convert this class into a class with "reactive" properties
 #       which can build a property hierarchy on an observer-like pattern
 #       where a decorated property automatically gets updated once
 #       one of its underlying functions gets updated...
 _NOT_FOUND = object()
+
+
 class cached_property:
     def __init__(self, func):
         self.func = func
         self.attrname = None
         self.__doc__ = func.__doc__
         self.lock = RLock()
 
@@ -53,8 +54,8 @@
                         cache[self.attrname] = val
                     except TypeError:
                         msg = (
                             f"The '__dict__' attribute on {type(instance).__name__!r} instance "
                             f"does not support item assignment for caching {self.attrname!r} property."
                         )
                         raise TypeError(msg) from None
-        return val
+        return val
```

### Comparing `pydoxtools-0.6.3/pydoxtools/classifier.py` & `pydoxtools-0.6.4/pydoxtools/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """
 Created on Mon Apr  6 22:01:10 2020
 TODO write file description
 """
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
 
 import abc
 import functools
 import logging
 import pathlib
 import typing
 import urllib
@@ -59,15 +59,15 @@
 class string_vectorizer(torch.nn.Module):
     """
     This module takes a webpage and finds an embedding using
     a pre-generated look-up table.56
     """
 
     def __init__(self):
-        super(string_vectorizer, self).__init__()
+        super().__init__()
         self.model_name = settings.PDXT_STANDARD_TOKENIZER  # name of model used for initialization
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         embedding_num, embedding_dim = 119547, 768  # size of multilingual BERT vocabulary
         self.embedding = torch.nn.Embedding(embedding_num, embedding_dim)
 
     def forward(self, strlist):
         # TODO: we might be able to us "diskcache" here in order to cache some layers!!!
@@ -143,15 +143,15 @@
             "classes": [self.classmap_[i.item()] for i in x],
             "probabilities": probs
         }
 
 
 class lightning_training_procedures(pytorch_lightning.LightningModule):
     def __init__(self):
-        super(lightning_training_procedures, self).__init__()
+        super().__init__()
         self.histograms = True
         self._hp_metric = None
 
     def add_standard_metrics(self, num_classes, hist_params=None):
         # TODO: get rid of this function in all child classes and somehow
         #       calculate "num_classes" automatically during initialization
         # define sensors for training/testing
@@ -296,15 +296,15 @@
             fft_pooling=True,
             ngram_size=2,  # size of ngrams to calculate for features
             topk_ngrams=5,  # number of top frequency ngrams to include in metadata
             meanmax_pooling=True,
             hp_metric=None,
             embeddings_mode=None
     ):
-        super(txt_block_classifier, self).__init__()
+        super().__init__()
 
         # we are saving all hyperparameters from above in the model checkpoint this way...
         self.save_hyperparameters()
         self.classmap_ = self.hparams.classmap
         self.classmapinv_ = {v: k for k, v in classmap.items()}
         self.classes_ = list(classmap.values())
         num_classes = len(classmap)
@@ -430,15 +430,15 @@
             # create n-grams and count their frequency. Add frequency of top-5 n-grams to
             # metadata. The hope is that we can recognize repetitiveness more easily this way.
             *get_topk_ngrams(s, k=self.hparams.topk_ngrams, ngram_size=self.hparams.ngram_size)
         ) for s in str_list], dtype=torch.float32).unsqueeze(1).to(device=self.device).squeeze()
         # normalize meta data on string length
         counts_norm = counts / (str_lens + 0.0001)  # adding 0.0001 to prevent div errors
         # len(s) / 2000,  # normalize size with 2000 (approx 1 pages = 1.0)
-        meta = torch.cat([counts_norm, str_lens/2000], 1)
+        meta = torch.cat([counts_norm, str_lens / 2000], 1)
 
         if self.hparams.embeddings_dim:
             # TODO: add optional str.strip here... (deactivated during training to improve speed)
             ids = self.tokenizer(
                 list(str_list),  # convert trlist into an actual list (e.g. if it is a pandas dataframe)
                 padding='max_length', truncation=True,
                 max_length=500,  # approx. half an A4 page of text
@@ -497,15 +497,15 @@
     TODO: right now the model can only cope with batches of size: 1, it would
           be preferrable to have larger batches.
 
     TODO: make urlClassifier a descendent of txtClassifier
     """
 
     def __init__(self, classes):
-        super(urlClassifier, self).__init__()
+        super().__init__()
         self.save_hyperparameters()
         self.classes_ = list(classes)
         self.classmap_ = dict(enumerate(classes))
         num_classes = len(classes)
 
         # define network layers
         self.string_vectorizer = string_vectorizer()
@@ -538,15 +538,15 @@
     TODO: make the clasifier itself check if it got the right "vectorization"
           for classification (in the case of pre-generated vectorizations from
           a database)
     """
     __version__ = "CCXv2002007"
 
     def __init__(self, classmap, scaling):
-        super(pageClassifier, self).__init__()
+        super().__init__()
         self.save_hyperparameters()
         self.classmap_ = classmap
         self.classmapinv_ = {v: k for k, v in classmap.items()}
         self.classes_ = list(classmap.values())
         self.scaling = torch.tensor(scaling)
         num_classes = len(classmap)
         self.testing = False
@@ -617,15 +617,15 @@
 
     TODO: turn this into a document classifier...
     TODO: move this into the document class itself...
     """
     __version__ = "txt20200807"
 
     def __init__(self, classmap):
-        super(pdfClassifier, self).__init__()
+        super().__init__()
         self.save_hyperparameters()  # save classmap
         self.cached = False
         self.classmap_ = classmap
         self.classmapinv_ = {v: k for k, v in classmap.items()}
         self.classes_ = list(classmap.values())
         num_classes = len(classmap)
         self.testing = False
@@ -697,15 +697,15 @@
             except:
                 logger.exception("failed vectorization...")
                 raise FailedVectorization(f"converting {pdf} did not work")
 
         return torch.stack(x)
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_classifier(name):
     logger.info(f"loading classifier: {name}")
     if name == "text_block":
         net = txt_block_classifier.load_from_checkpoint(settings.MODEL_STORE(name))
     elif name == "url":
         net = urlClassifier.load_from_checkpoint(settings.MODEL_STORE(name))
     elif name == "page":
@@ -713,15 +713,15 @@
     elif name == "pdf":
         net = pdfClassifier.load_from_checkpoint(settings.MODEL_STORE(name))
 
     net.freeze()
     return net
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def gen_meta_info(url, htmlstr) -> torch.tensor:
     """
     Generates some meta-info mainly based
     on the structure of a page:
 
     This is a stand-alone function in order to be able to cache it...
```

### Comparing `pydoxtools-0.6.3/pydoxtools/cluster_utils.py` & `pydoxtools-0.6.4/pydoxtools/cluster_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# -*- coding: utf-8 -*-
 """
 Potentially cython-optimizable code for geometric calculations should go here.
 """
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import difflib
 import functools
 import typing
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
@@ -658,19 +659,20 @@
     :param bbs: list of boundary boxes to search
     :param bbox: search in this area
     :param tol: search tolerance (with respect to a single dimension)
     :return: list of boundary boxes extracted from bbs which are in the search area *bbox*
     """
     # valid_areas.loc[valid_areas.x0>bbox[0]].loc[valid_areas.x1<bbox[2]]
     # in order to increase the speed we filter with several .loc operations
-    indices =  bbs.loc[bbs.y1 > (bbox[1] - tol)].loc[bbs.y0 < (bbox[3] + tol)] \
+    indices = bbs.loc[bbs.y1 > (bbox[1] - tol)].loc[bbs.y0 < (bbox[3] + tol)] \
         .loc[bbs.x1 > (bbox[0] - tol)].loc[bbs.x0 < (bbox[2] + tol)].index
 
     return indices
 
+
 # TODO: check in different location whether it makes sense that
 #       we use a custom distance function in order to improve clustering
 # TODO: directly hand over the distance matrix for clarity?...
 def distance_cluster(data: np.ndarray = None,
                      distance_threshold: float = 0.0,
                      distance_func=None,
                      pairwise_distance_func=None,
```

### Comparing `pydoxtools-0.6.3/pydoxtools/dask_operators.py` & `pydoxtools-0.6.4/pydoxtools/dask_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import copy
 from typing import Any
 from typing import Callable
 
 import dask.bag
 from dask import dataframe
 from dask.bag import Bag
```

### Comparing `pydoxtools-0.6.3/pydoxtools/document.py` & `pydoxtools-0.6.4/pydoxtools/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import functools
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import io
 import json
 import logging
 import mimetypes
 import re
 from functools import cached_property
@@ -305,15 +306,15 @@
             FunctionOperator(lambda article: article.top_image)
             .pipe(article="goose_article").out("main_image").cache(),
             Alias(full_text="main_content"),
             FunctionOperator(lambda x: pd.DataFrame(get_text_only_blocks(x), columns=["text"])).cache()
             .pipe(x="raw_content").out("text_box_elements"),
             FunctionOperator(lambda t, s: [t, s])
             .pipe(t="title", s="short_title").out("titles").cache(),
-            FunctionOperator(lambda x: set(w.strip() for w in x.split(",")))
+            FunctionOperator(lambda x: {w.strip() for w in x.split(",")})
             .pipe(x="html_keywords_str").out("html_keywords").cache(),
 
             ########### AGGREGATION ##############
             FunctionOperator(lambda **kwargs: set(list_utils.flatten(kwargs.values())))
             .pipe("html_keywords", "textrank_keywords").out("keywords").cache(),
         ],
         # docx
@@ -649,15 +650,15 @@
     ):
         """Initialize a Document instance.
 
         Either fobj or source are required. They can both be given. If either of them
         isn't specified the other one is inferred automatically.
 
         document_type, page_number and max_pages are also not required, but can be used to override
-        the default behaviour. specifically document_type can be used manually specify
+        the default behaviour. specifically document_tgiype can be used manually specify
         the pipeline that should be used.
 
         Args:
             fobj:
                 The file object or data to load. Depending on the type of object passed:
                 - If a string or bytes object: the object itself is the document. IN case of a bytes
                      object, the source helps in determining the filetype through file endings.
@@ -724,15 +725,15 @@
                 #       fileloader and this here to download urls
                 if is_url(fobj):
                     response = requests.get(fobj)
                     self._fobj = response.content
             except:
                 pass
 
-    @functools.cache
+    @functools.lru_cache
     def _key(self):
         return (self.__class__.__name__, str(self._configuration), self._fobj, self._source,
                 self._document_type, self._page_numbers, self._max_pages)
 
     @cached_property
     def fobj(self) -> bytes | str | Path | IO | dict | list | set:
         if self._fobj:
@@ -771,27 +772,27 @@
         if self._document_type != "auto":
             return self._document_type
         else:
             doc_type, _, _ = self.document_type_detection()
             return doc_type
 
     @staticmethod
-    @functools.cache  # make sure we only run it once..
+    @functools.lru_cache  # make sure we only run it once..
     def magic_library_available():
         try:
             import magic
         except ImportError:
             logger.warning("libmagic was not found on your system! falling back"
                            "to filetype detection by file-ending only. In order"
                            "to have a more robust file type detection it would be"
                            "advisable to install this library.")
             magic = False
         return magic
 
-    # @functools.cache
+    @functools.lru_cache
     def document_type_detection(self):
         """
         This one here is actually important as it detects the
         type of data that we are going to use for out pipeline.
         That is also why this is implemented as a member function and can
         not be pushed in the pipeline itself, because in needs to be run
         in order to select which pipline we are going to use.
@@ -895,15 +896,15 @@
             return "*"
 
     def __repr__(self):
         """
         Returns:
             str: A string representation of the instance.
         """
-        if isinstance(self._source, str | bytes):
+        if isinstance(self._source, (str,bytes)):
             return f"{self.__module__}.{self.__class__.__name__}(source={self.source[:10]})"
         else:
             return f"{self.__module__}.{self.__class__.__name__}(source={self.source})"
 
     """
     @property
     def final_url(self) -> list[str]:
```

### Comparing `pydoxtools-0.6.3/pydoxtools/document_base.py` & `pydoxtools-0.6.4/pydoxtools/document_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,55 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import json
 import logging
 import pathlib
 import pickle
+import sys
 import uuid
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from time import time
-from typing import List, Any, get_type_hints
+from typing import Any, get_type_hints
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import spacy.tokens
 import yaml
 from diskcache import Cache
 
 from .list_utils import deep_str_convert
 from .operators_base import Operator, Configuration, OperatorException, OperatorOutputException
 from .settings import settings
 
 logger = logging.getLogger(__name__)
 
+if sys.version_info.minor < 10:
+    slot_args = dict()
+else:
+    slot_args = dict(slots=True)
+
 
-@dataclass(eq=True, frozen=True, slots=True)
+@dataclass(eq=True, frozen=True, **slot_args)
 class Font:
     name: str
     size: float
     color: str
 
 
 class ElementType(Enum):
     Graphic = 1
     Text = 2
     Image = 3
 
 
-@dataclass(slots=True)
+@dataclass(**slot_args)
 class DocumentElement:
     type: ElementType
     p_num: int | None = None
     x0: float | None = None
     y0: float | None = None
     x1: float | None = None
     y1: float | None = None
@@ -59,15 +67,15 @@
     stroke: bool | None = None
     fill: bool | None = None
     evenodd: int | None = None
     level: int = 0
 
 
 class TokenCollection:
-    def __init__(self, tokens: List[spacy.tokens.Token]):
+    def __init__(self, tokens: list[spacy.tokens.Token]):
         self._tokens = tokens
 
     @cached_property
     def vector(self):
         return np.mean([t.vector for t in self._tokens], 0)
 
     @cached_property
@@ -110,15 +118,15 @@
     #       decouple etc...
 
     # in theory, we could add additional arguments to this function which we could
     # pass in our documentbase class
     def __new__(cls, clsname, bases, attrs):
         start_time = time()
         # construct our class
-        new_class: Pipeline.__class__ = super(MetaPipelineClassConfiguration, cls).__new__(
+        new_class: Pipeline.__class__ = super().__new__(
             cls, clsname, bases, attrs)
 
         if hasattr(new_class, "_operators"):
             if new_class._operators:
                 # TODO: add checks to make sure we don't have any name-collisions
                 # configure class
                 logger.info(f"configure {new_class} class...")
@@ -359,15 +367,15 @@
         """
 
         properties = {a: getattr(self, a) for a in args}
         properties.update({v: getattr(self, k) for k, v in kwargs.items()})
 
         return deep_str_convert(properties)
 
-    @functools.cache
+    @functools.lru_cache
     def to_dataframe(self, *args, **kwargs):
         dictlist = self.to_dict(*args, **kwargs)
         df = pd.DataFrame(dictlist)
         return df
 
     def to_yaml(self, *args, **kwargs):
         """
@@ -462,17 +470,17 @@
                  operation name, usage, return type, and supported pipelines.
         """
         output_infos = cls.pipeline_docs()
 
         node_docs = []
         for k, v in output_infos.items():
             return_types = " | ".join(sorted(str(i) for i in v['output_types']))
-            return_types = return_types.replace(">", "\>")
+            return_types = return_types.replace(">", r"\>")
             pipeline_flows = ", ".join(sorted(v['pipe_types']))
-            pipeline_flows = pipeline_flows.replace(">", "\>")
+            pipeline_flows = pipeline_flows.replace(">", r"\>")
 
             single_node_doc = f"""### {k}
             
 {v['description']}
 
 Can be called using:
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_classes.py` & `pydoxtools-0.6.4/pydoxtools/extract_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import logging
 
 import langdetect
 import pandas as pd
 from transformers import AutoModelForSequenceClassification, pipeline, AutoTokenizer
 
 from pydoxtools.operators_base import Operator
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_filesystem.py` & `pydoxtools-0.6.4/pydoxtools/extract_filesystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import pathlib
 import typing
 from pathlib import Path
 
 import chardet
 
@@ -19,15 +21,15 @@
     else:
         return txt
 
 
 def load_raw_file_content(fobj: bytes | str | Path | typing.IO) -> bytes | str:
     if isinstance(fobj, pathlib.Path):
         try:
-            with open(fobj, "r") as file:
+            with open(fobj) as file:
                 txt = file.read()
         except:
             with open(fobj, "rb") as file:
                 txt = file.read()
     elif isinstance(fobj, str | bytes):
         txt = fobj
     else:
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_html.py` & `pydoxtools-0.6.4/pydoxtools/extract_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
 
 import base64
 import html
 import logging
 from io import BytesIO
 from typing import List
 from urllib.parse import urlsplit
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_index.py` & `pydoxtools-0.6.4/pydoxtools/extract_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import logging
 import uuid
 from typing import Callable
 
 import dask.bag
 import hnswlib
 import networkx as nx
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_nlpchat.py` & `pydoxtools-0.6.4/pydoxtools/extract_nlpchat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 from typing import Callable
 
 import yaml
 from diskcache import Cache
 
 from .operators_base import Operator
@@ -46,29 +48,29 @@
     completion = openai_chat_completion_with_diskcache(
         model_id=model_id, temperature=0.0, messages=msgs, max_tokens=max_tokens
     )
     result = completion.choices[0].message
     return result
 
 
-@functools.cache
+@functools.lru_cache
 def get_gpt4model(model_id):
     from gpt4all import GPT4All
     # gptj = GPT4All("ggml-gpt4all-j-v1.3-groovy")
     gptj = GPT4All(model_id)
     return gptj
 
 
-@functools.cache
+@functools.lru_cache
 def gpt4_models():
     from gpt4all import GPT4All
     return [m["filename"].strip('.bin') for m in GPT4All.list_models()]
 
 
-@cache.memoize()
+@functools.lru_cache
 def gpt4allchat(messages, model_id="ggml-mpt-7b-instruct", max_tokens=256, *args, **kwargs):
     gptj = get_gpt4model(model_id)
     res = gptj.chat_completion(messages, default_prompt_footer=False, default_prompt_header=False)
     return res
 
 
 class LLMChat(Operator):
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_objects.py` & `pydoxtools-0.6.4/pydoxtools/extract_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 from typing import Any
 
 import pandas as pd
 from urlextract import URLExtract
 
 from pydoxtools.operators_base import Operator
 from pydoxtools.settings import settings
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_ocr.py` & `pydoxtools-0.6.4/pydoxtools/extract_ocr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import io
 import logging
 
 import langdetect
 import pytesseract
 from PIL import Image
 from pdfminer.high_level import extract_text
@@ -32,15 +34,15 @@
         if ocr_lang == "auto":
             pdf = pytesseract.image_to_pdf_or_hocr(file, extension='pdf', lang=None)
             text = extract_text(io.BytesIO(pdf))
             try:
                 lang = langdetect.detect(text)
             except langdetect.lang_detect_exception.LangDetectException as err:
                 if err.args[0] == 'No features in text.':
-                    lang = "en" #simply use english as a language
+                    lang = "en"  # simply use english as a language
                 else:
                     raise OCRException("could not detect language !!!")
             # get the corresponding language for tesseract
             lang = ocr_language_mappings.langdetect2tesseract.get(lang, None)
             file.seek(0)  # we are scanning th same file now with the correct language
         else:
             lang = ocr_lang
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_pandoc.py` & `pydoxtools-0.6.4/pydoxtools/extract_pandoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import logging
 import mimetypes
 
 import pandas as pd
 from packaging import version
 
 import pydoxtools.operators_base
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_spacy.py` & `pydoxtools-0.6.4/pydoxtools/extract_spacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 import logging
 import subprocess
+import typing
 from typing import Optional, Any
 
 import numpy as np
 import spacy
 from spacy import Language
 from spacy.tokens import Doc, Token, Span
 
@@ -16,15 +17,15 @@
 
 def download_model(model_id: str):
     # python -m spacy download en_core_web_sm
     return subprocess.call(['python', '-m', 'spacy', 'download', model_id])
     # spacy.load("en_core_web_sm")
 
 
-def extract_noun_chunks(spacy_doc) -> list[TokenCollection]:
+def extract_noun_chunks(spacy_doc) -> typing.List[TokenCollection]:
     token_list = []
     for nc in spacy_doc.noun_chunks:
         tc = TokenCollection([t for t in nc if t.pos_ not in ["DET", "SPACE", "PRON"]])
         if len(tc) > 0:
             token_list.append(tc)
     # filter = ["DET"]
     return token_list
@@ -57,15 +58,15 @@
                             'nl', 'fi', 'el', 'ko', 'lt', 'mk', 'nb', 'pl', 'pt',
                             'ro', 'ru', 'sv', 'uk']:
         return f'{model_language}_core_news_{size}'
     else:
         return f'xx_sent_ud_sm'
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_cached_spacy_model(model_id: str) -> Language:
     """
     load spacy nlp model and in case of a transformer model add custom vector pipeline...
 
     we also make sure to cache the model for batch operations on documens.
     """
     try:
@@ -148,15 +149,15 @@
 class SpacyOperator(Operator):
     def __call__(
             self,
             full_text: str,
             language: str,
             spacy_model: str,
             model_size: str
-    ) -> dict[str, Any]:
+    ) -> typing.Dict[str, Any]:
         """Load a document using spacy"""
         if spacy_model == "auto":
             nlp_modelid = get_spacy_model_id(language, model_size)
         else:
             nlp_modelid = spacy_model
 
         spacy_nlp = load_cached_spacy_model(nlp_modelid)
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_tables.py` & `pydoxtools-0.6.4/pydoxtools/extract_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import hashlib
 import logging
 import re
 import typing
 from functools import cached_property
 
@@ -12,17 +14,17 @@
 from sklearn.neighbors import KernelDensity
 
 import pydoxtools
 import pydoxtools.document_base
 import pydoxtools.operators_base
 from pydoxtools import cluster_utils as gu
 from pydoxtools.cluster_utils import pairwise_txtbox_dist, box_cols, y1, x0, x1, boundarybox_intersection_query
-from pydoxtools.operators_base import Operator
 from pydoxtools.extract_html import extract_lists, extract_tables
 from pydoxtools.extract_textstructure import _line2txt
+from pydoxtools.operators_base import Operator
 
 logger = logging.getLogger(__name__)
 
 idx = pd.IndexSlice
 
 
 class TableExtractionParameters(pydantic.BaseModel):
@@ -321,15 +323,15 @@
     @cached_property
     def bbox(self):
         # find the exact bounding box of our table...
         ge_bb = np.array([self.df_ge.x0.min(), self.df_ge.y0.min(), self.df_ge.x1.max(), self.df_ge.y1.max()])
         le_bb = np.array([self.df_le.x0.min(), self.df_le.y0.min(), self.df_le.x1.max(), self.df_le.y1.max()])
         return np.array([*np.vstack([ge_bb[:2], le_bb[:2]]).min(0), *np.vstack([ge_bb[2:], le_bb[2:]]).max(0)])
 
-    @functools.lru_cache()
+    @functools.lru_cache
     def detect_cells(self, steps=None) -> pd.DataFrame:
         """
         This algorithm works by slowly scanning through a table bottom-to-top first
         and left-to-right for each row.
 
         On the way we detect rows by alternating between text lines and graphical lines.
         We can detect a cell border by going from the bottom of a text-line-box to the botom
@@ -468,30 +470,30 @@
             h_row_elem = h_row_elem.loc[
                 h_row_elem.w > min_cell_width]  # .reorder_levels([2, 3, 0, 1], axis=0).sort_index()
             # and extract horizontal lines from them
             h_lines = pd.concat([
                 h_row_elem.loc[y0_h_elem - elem_scan_tol:y0_h_elem + max_v_line_thickness,
                 ["x0", "x1", "y0"]].rename(columns={"y0": "y"}),
                 h_row_elem.loc[idx[:, y0_h_elem - elem_scan_tol:y0_h_elem + max_v_line_thickness],
-                               ["x0", "x1", "y1"]].rename(columns={"y1": "y"})
+                ["x0", "x1", "y1"]].rename(columns={"y1": "y"})
             ]).droplevel(["y0", "y1"]).sort_index().drop_duplicates(["x0", "x1"])
 
             new_cells, still_open = _close_open_cells(
                 open_cells, h_lines, le, elem_scan_tol, text_line_tol, y0_h_elem)
             open_cells = still_open
             cells.extend(new_cells)
 
         if steps:  # return additional debug information
             self._debug["open_cells"] = pd.DataFrame(open_cells)
             self._debug["open_cells"]['y1'] = self.bbox[y1]
             return pd.DataFrame(cells)
         else:
             return pd.DataFrame(cells)
 
-    @functools.lru_cache()
+    @functools.lru_cache
     def convert_cells_to_df(self) -> typing.Tuple[pd.DataFrame, typing.Tuple]:
         """
         TODO: make the algorithm work with non-graphical tables as well by searching for rows/columns/cells
               using textboxes only.
 
         TODO: enhance function by also taking textboxes into account. (for large table cells)
         """
@@ -553,15 +555,15 @@
         in order to label pdf tables for parametr optimization"""
         table, (hlines, vlines, cells) = self.convert_cells_to_df()
         # TODO: over time calculate better metrics by goind
         #       through our table extractions and check wrong classifications
 
         # remove some special characters and normalize whitespace
         # to get a good md5 sum for these tables...
-        tokentable = table.replace({'<.?s>': '', '\s+': ' '}, regex=True)
+        tokentable = table.replace({'<.?s>': '', r'\s+': ' '}, regex=True)
         tablestr = str(tokentable.values.tolist())
         md5 = hashlib.md5(tablestr.encode('utf-8')).hexdigest()
 
         metrics = dict(
             area_detection_method=self.tbe.extraction_method,
             table_area=self.bbox,
             md5=md5,
```

### Comparing `pydoxtools-0.6.3/pydoxtools/extract_textstructure.py` & `pydoxtools-0.6.4/pydoxtools/extract_textstructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import operator
 import typing
 from dataclasses import asdict
 
 import pandas as pd
 import pdfminer
 from pdfminer.layout import LTChar, LTTextLineVertical
```

### Comparing `pydoxtools-0.6.3/pydoxtools/file_utils.py` & `pydoxtools-0.6.4/pydoxtools/file_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import hashlib
 import typing
 from pathlib import Path
 from urllib.parse import urlparse
 
 
 def generate_unique_pdf_filename_from_url(source_url: str) -> str:
```

### Comparing `pydoxtools-0.6.3/pydoxtools/html_utils.py` & `pydoxtools-0.6.4/pydoxtools/html_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
+# !/usr/bin/env python3
 """
 Created on Mon Apr  6 21:57:32 2020
 # TODO write file description
 # TODO split up file in "cleaning" and "extraction" functions
 """
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
 
 import logging
 import os
 import re
 import tempfile
 import urllib
 import webbrowser
-from typing import List
 from urllib.parse import urlparse
 
 import pandas as pd
 from bs4 import BeautifulSoup
 from lxml.html.clean import Cleaner
 
 logger = logging.getLogger(__name__)
@@ -101,20 +100,20 @@
 
 
 def url_join(url1, url2):
     """
     joins two urls while removing double-slashes
     """
     # TODO: remove double slashes from URL with http
-    url1, url2 = [url.replace("//", "/") if url[:4] != "http"
-                  else url[:7] + url[7:].replace("//", "/") for url in [url1, url2]]
+    url1, url2 = (url.replace("//", "/") if url[:4] != "http"
+                  else url[:7] + url[7:].replace("//", "/") for url in [url1, url2])
     return urllib.parse.urljoin(url1, url2)
 
 
-def get_pdf_links(html) -> List[str]:
+def get_pdf_links(html) -> list[str]:
     linklist = []
     soup = BeautifulSoup(html, 'lxml')
     for link in soup.find_all('a', href=True):
         if link['href'].lower().endswith(".pdf"):
             linklist.append(link['href'])
     return linklist
```

### Comparing `pydoxtools-0.6.3/pydoxtools/labeling.py` & `pydoxtools-0.6.4/pydoxtools/labeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 This file gathers functions that are used multiple times
 in our jupyter notebooks...  They are not intended for production
 use.
 """
 
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import concurrent.futures
 import concurrent.futures
 import functools
 import itertools
 import logging
 
 import numpy as np
@@ -93,15 +95,15 @@
     tables.file = tables.file.str.split("/").str[-1]
     return tables.reset_index().drop(columns='index')
 
 
 md5_cols = ["md5", "page", "file"]
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_tables_from_csv():
     """TODO: move this into an extractor!!"""
     table_data = settings.TRAINING_DATA_DIR / "pdfs/tabledata.csv"
 
     # match labeled tables with calculated data
     tables_csv = pd.read_csv(table_data)
     # remove intermediate header rows...
```

### Comparing `pydoxtools-0.6.3/pydoxtools/list_utils.py` & `pydoxtools-0.6.4/pydoxtools/list_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """
 Created on Thu Apr  9 22:12:25 2020
 # TODO write file description
 """
 from __future__ import annotations
 
 import collections
 import datetime
 import logging
 import math
 import numbers
 from collections.abc import Iterable, Mapping, MutableMapping
 from itertools import groupby
 from operator import itemgetter
-from typing import List, Tuple, Any, Dict
+from typing import Any, Dict
 
 import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
 def iterablefyer(property):
@@ -88,18 +87,18 @@
 
 
 def flatten_unique(x):
     return set(flatten(x))
 
 
 def flatten_dict(
-        dct: Dict[str, Any],
+        dct: dict[str, Any],
         prefix: str = '',
         separator: str = '.'
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Flattens a nested dictionary structure into a single-level dictionary.
 
     This function recursively traverses through the input dictionary structure and creates new keys
     for nested dictionaries using dot notation. The traversal stops at the specified maximum depth.
 
     Args:
@@ -181,15 +180,15 @@
         logger.debug(f"can not process object of kind: {type(obj)}"
                      f",\nthe object: {obj}")
         res = str(obj)
 
     return res
 
 
-def group_by(data: List[Tuple[str, Any]]) -> Dict[str, Any]:
+def group_by(data: list[tuple[str, Any]]) -> dict[str, Any]:
     """group data given as a list of tuples where the first element of the tuple
     specfies the group key.
     """
     groups = {}
     for k, group in groupby(sorted(data, key=itemgetter(0)), lambda x: x[0]):
         groups[k] = [g[1:] for g in group]
```

### Comparing `pydoxtools-0.6.3/pydoxtools/models.py` & `pydoxtools-0.6.4/pydoxtools/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 @author: Thomas Meschede
 
 This file implements common models used "all over the place" by componardo/comcharax.
 
 "internal" models based on "pydantic" have an "underscore" as suffix:
 
@@ -20,14 +19,16 @@
 - or an underscore at the end
 
 properties (calculated & stored) are indicated by lower letters
 
 
 """
 
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import datetime
 import gzip
 import logging
 from typing import List, Any
 
 from pydantic import BaseModel, Field, AnyHttpUrl
```

### Comparing `pydoxtools-0.6.3/pydoxtools/nlp_utils.py` & `pydoxtools-0.6.4/pydoxtools/nlp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """
 Created on Mon Mar 30 15:29:52 2020
 
 @author: Thomas.Meschede@soprasteria.com
 
 we accumulate most of our NLP functions here for the rest of the library
 as we need to keep models in memory for other functions to use
@@ -14,25 +13,26 @@
 TODO: refactor this... there are a lot of functions and it would
       be great if we could somehow organize them a little better...
 
 TODO: think about how to disribute functions between nlp_utils and
       classifier
 """
 
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import logging
 from difflib import SequenceMatcher
 from typing import Any
 
 import numpy as np
 import pandas as pd
 import sklearn as sk
 import sklearn.linear_model
 import torch
-from pydantic import BaseModel
 from scipy.spatial.distance import pdist, squareform
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModel, AutoModelForQuestionAnswering
 
 from pydoxtools.settings import settings
 
 logger = logging.getLogger(__name__)
@@ -57,15 +57,15 @@
 @functools.lru_cache(maxsize=32)
 def load_tokenizer(model_id):
     logger.info("load_tokenizer")
     tokenizer = AutoTokenizer.from_pretrained(model_id)
     return tokenizer
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_model(model_id: str) -> Any:
     logger.info(f"load model {model_id} on device: {device}")
     # model = AutoModelForQuestionAnswering.from_pretrained(model_id, output_hidden_states=True)
     model = AutoModel.from_pretrained(model_id, output_hidden_states=True)
     model.to(device)
     model.eval()
     return model
@@ -316,15 +316,15 @@
     load_tokenizer.cache_clear()
 
 
 def vecseq_similarity(vs, search_vec):
     return cos_compare(vs, [search_vec])
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def get_vocabulary(model_id: str):
     """make sure the vocabulary only gets loaded once
     TODO: implement more vocabularies"""
     logger.info(f"loading vocabulary from {model_id}")
     model = load_model(model_id)
     # return and transform embeddings into numpy array
     return model.embeddings.word_embeddings.weight.detach().numpy()
@@ -450,22 +450,22 @@
 
 def convert_ids_to_string(model_id: str, ids):
     tokenizer = load_tokenizer(model_id=model_id)
     a = tokenizer.convert_ids_to_tokens(ids)
     return tokenizer.convert_tokens_to_string(a)
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_pipeline(pipeline_type: str, model_id: str):
     from transformers import pipeline
     pipeline_instance = pipeline(pipeline_type, model=model_id)
     return pipeline_instance
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_qa_models(model_id: str):
     # TODO: only load model "id" and use that id
     #        with transformers AutoModel etc...
     logger.info(f"loading Q & A model and tokenizer {model_id}")
     # model, tokenizer = load_models(model_id)
     # TODO: use load_tokenizer function for this
     tokenizer = load_tokenizer(model_id)
```

### Comparing `pydoxtools-0.6.3/pydoxtools/ocr_language_mappings.py` & `pydoxtools-0.6.4/pydoxtools/ocr_language_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,8 @@
     "uzb": None,
     "uzb_cyrl": None,
     "vie": "vi",
     "yid": None,
     "yor": None,
 }
 
-langdetect2tesseract = {v:k for k, v in tesseract2langdetect.items() if v}
+langdetect2tesseract = {v: k for k, v in tesseract2langdetect.items() if v}
```

### Comparing `pydoxtools-0.6.3/pydoxtools/operator_huggingface.py` & `pydoxtools-0.6.4/pydoxtools/operator_huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """
 Huggingface related code
 
 Enables loading of mdoels from huggingface for all kinds of purposes
 """
 
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import logging
 from typing import Dict, List, Tuple, Callable
 
 import torch
 
 from pydoxtools import nlp_utils
-from pydoxtools.operators_base import Operator
 from pydoxtools.list_utils import iterablefyer
 from pydoxtools.nlp_utils import tokenize_windows
+from pydoxtools.operators_base import Operator
 
 logger = logging.getLogger(__name__)
 
 
 def answer_questions_on_long_text(questions, text, model_id) -> Dict[str, List[Tuple[str, float]]]:
     all_answers = {}
     for q in questions:
```

### Comparing `pydoxtools-0.6.3/pydoxtools/operators.py` & `pydoxtools-0.6.4/pydoxtools/operators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.3/pydoxtools/operators_base.py` & `pydoxtools-0.6.4/pydoxtools/operators_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 The pydoxtools.operators module defines
 a set of generic pipeline operators that can
 be used inside of a pipeline class definition
 to create your own pipelines.
 """
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import abc
 import typing
 from abc import ABC
-
 from typing import Callable, Iterable, Any
 
 
 class Operator(ABC):
     """Base class to build extraction logic for information extraction from
     unstructured documents and loading files
```

### Comparing `pydoxtools-0.6.3/pydoxtools/pdf_utils.py` & `pydoxtools-0.6.4/pydoxtools/pdf_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# -*- coding: utf-8 -*-
 """
 Created on Mon Dec 16 12:07:52 2019
 
 @author: Thomas Meschede
 """
 
 # alternatives to camelot:
 # https://github.com/tabulapdf/tabula for "stream-tables"
 # 
 
 
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import io
 import logging
 from pathlib import Path
 
 import pandas as pd
 # TODO: evaluate tabula as an additional table-read mechanism
@@ -25,15 +26,14 @@
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LAParams
 from pdfminer.layout import LTChar, LTCurve, LTFigure, LTTextLine
 from pdfminer.layout import LTTextContainer
 from pdfminer.pdfinterp import resolve1
 from pdfminer.pdfparser import PDFParser
 
-import pydoxtools.document_base
 import pydoxtools.operators_base
 from pydoxtools import document_base, list_utils
 
 logger = logging.getLogger(__name__)
 
 try:
     from functools import cached_property
```

### Comparing `pydoxtools-0.6.3/pydoxtools/random_data_generators.py` & `pydoxtools-0.6.4/pydoxtools/random_data_generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from itertools import islice
 from random import randint
 
 import torch
 
 from .settings import settings
 
-_asciichars = ''.join(sorted(set(chr(i) for i in range(32, 128)).union(string.printable)))
+_asciichars = ''.join(sorted({chr(i) for i in range(32, 128)}.union(string.printable)))
 
 
 def rand_chars(char_dict: dict) -> typing.Callable[[], str]:
     """create a random function which randomly selects characters from
     a list. function Argument is a dictionary with weights on how often
     characters should be chosen:
 
@@ -124,15 +124,15 @@
     """TODO: convert this into  Faker provider?"""
 
     def __init__(self, type="address", rand_str_perc=0.3, osm_perc=0.5, fieldname_prob=0.05):
         # function which returns some random separation characters
         self._rand_str_perc = rand_str_perc  # probability to use radom strings in certain areas
         self._osm_perc = osm_perc  # probability to use openstreetmap data
         self._fieldname_prob = fieldname_prob  # probability to use a fieldname in front of an address line
-        self._f: "faker.Faker" | None = None
+        self._f: faker.Faker | None = None
         self._type: str = type
 
     @cached_property
     def random_sep_func(self):
         return rand_chars({"\n": 48, ", ": 12, "; ": 6, " | ": 3, "|": 3, "·": 1, " · ": 1})
 
     @cached_property
```

### Comparing `pydoxtools-0.6.3/pydoxtools/settings.py` & `pydoxtools-0.6.4/pydoxtools/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """
 Created on Tue Apr 28 21:55:35 2020
 
 @author: tom
 """
 
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import logging
 import os
 from pathlib import Path
 
 import appdirs
 # TODO: remove joblib as a dependency from here ...
 from pydantic import BaseSettings
```

### Comparing `pydoxtools-0.6.3/pydoxtools/training.py` & `pydoxtools-0.6.4/pydoxtools/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import datetime
 import functools
 import logging
 import pickle
 from pathlib import Path
 
 import numpy as np
@@ -15,15 +17,15 @@
     pageClassifier, txt_block_classifier
 from pydoxtools.random_data_generators import TextBlockGenerator
 from pydoxtools.settings import settings
 
 logger = logging.getLogger(__name__)
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_labeled_webpages():
     trainingfiles = file_utils.get_nested_paths(settings.TRAINING_DATA_DIR, "trainingitem*.parquet")
 
     df = pd.read_parquet(trainingfiles[0])
     df['file'] = trainingfiles[0]
     for tf in trainingfiles[1:]:
         df2 = pd.read_parquet(tf)
@@ -49,15 +51,15 @@
             if not pt in allowed_types:
                 df.loc[df.page_type == pt, 'page_type'] = 'unknown'
 
     df.page_type = df.page_type.astype("category")
     return df
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def load_labeled_pdf_files(label_subset=None) -> pd.DataFrame:
     """
     This function loads the pdfs from the training data and
     labels them according to the folder they were found in...
 
     TODO: use the label_subset
     """
@@ -99,15 +101,15 @@
         vector = self.vectors[i]
         return vector, self.labels[i]
 
     def __len__(self):
         return len(self.labels)
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def prepare_pdf_training():
     """
     loads textblock data, enriches it with addresses and
     other classes in order to train
 
     :return: pytorch dataloaders
     """
@@ -148,15 +150,15 @@
         batch_size=500,
         num_workers=5
         # sampler=weighted_sampler
     )
     return train_loader, test_loader, model
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def prepare_page_training():
     """
     Prepares training data, loaders and model parameters
 
     TODO: use the same function for generating the features here and
           in the classifier.
 
@@ -322,15 +324,15 @@
         callbacks=kwargs.get('callbacks', []),
         default_root_dir=settings.MODEL_STORE("text_block").parent
     )
 
     return train_loader, validation_loader, model, trainer
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def prepare_url_training():
     # TODO:  use our textblock classifier for this!
     df = load_labeled_webpages()
     # TODO make a classmap here instead of classes for added safety, that
     #      categorical encoding stay the same...
     classes = df.page_type.cat.categories.tolist()
     X = df.url
```

### Comparing `pydoxtools-0.6.3/pydoxtools/visual_document_analysis.py` & `pydoxtools-0.6.4/pydoxtools/visual_document_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import functools
 import hashlib
 import typing
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pydantic
```

### Comparing `pydoxtools-0.6.3/pydoxtools/webdav_utils.py` & `pydoxtools-0.6.4/pydoxtools/webdav_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # this is so, that we can use python3.10 annotations..
+
 import logging
 import subprocess
 import time
 
 import requests
 from webdav3.client import Client
```

### Comparing `pydoxtools-0.6.3/pyproject.toml` & `pydoxtools-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pydoxtools"
-version = "0.6.3"
+version = "0.6.4"
 description = "This library contains a set of tools in order to extract and synthesize structured information from documents"
 authors = ["thomas meschede <yeusblender@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pydoxtools.xyntopia.com"
 repository = "https://github.com/xyntopia/pydoxtools"
 documentation = "https://pydoxtools.xyntopia.com"
 keywords = ["AI", "document-analysis", "LLM", "NLP", "ML"]
 
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0" # python version constraints are caused by scipy
+python = ">=3.8,<4.0" # python version constraints are caused by scipy
 goose3 = { optional = true, version = ">=3.1.6" }
 # we are using this version of readability as the other version has a little bug...
 readability-lxml = { optional = true, version = ">=0.8.1" }
 appdirs = ">=1.4.4"
 langdetect = { optional = true, version = ">=1.0.8" }
 transformers = { optional = true, version = ">=4.17.0" }
 # TODO: get rid of this library, can be replace by custom function
@@ -54,25 +54,26 @@
 torch = { version = ">=1.12.1", optional = true }
 pytesseract = {version = "^0.3.10", optional = true}
 pyyaml = "^6.0"
 dask = {extras = ["complete"], version = "^2023.4.1", optional = true}
 diskcache = "^5.6.1"
 chardet = "^5.1.0"
 chromadb = {version = "^0.3.23", optional = true}
+gpt4all = {version = "^0.2.3", optional = true}
 
 [tool.poetry.extras]
 # extraction-transformation-load facilities
 etl = ["goose3", "langdetect", "tldextract", "spacy", "pdfminer.six",
     "extruct", "urlextract", "quantulum3", "stemming",
     "quantities", "readability-lxml", "pandas", "beautifulsoup4", "hnswlib",
     "networkx", "openai", "textract", "pandoc", "python-pptx", "dask", "pytesseract"
 ]
 # TODO: rename & regroups extras (e.g. light, medium average or something like that...)
 inference = ["transformers", "scikit-learn", "tqdm", "torch", "pytorch-lightning", "spacy",
-    "beautifulsoup4", "pandas", "urlextract", "hnswlib", "chromadb"]
+    "beautifulsoup4", "pandas", "urlextract", "hnswlib", "chromadb", "gpt4all"]
 
 [tool.poetry.group.colab]
 optional = true
 
 [tool.poetry.group.colab.dependencies]
 pytest = ">=6.0.1"
 yattag = ">=1.13.2" #for html text coloring
```

### Comparing `pydoxtools-0.6.3/PKG-INFO` & `pydoxtools-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: pydoxtools
-Version: 0.6.3
+Version: 0.6.4
 Summary: This library contains a set of tools in order to extract and synthesize structured information from documents
 Home-page: https://pydoxtools.xyntopia.com
 License: MIT
 Keywords: AI,document-analysis,LLM,NLP,ML
 Author: thomas meschede
 Author-email: yeusblender@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: etl
 Provides-Extra: inference
 Requires-Dist: Pint (>=0.16.1)
 Requires-Dist: Shapely (>=1.8.0,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4)
 Requires-Dist: beautifulsoup4 (>=4.8.0) ; extra == "etl" or extra == "inference"
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: chromadb (>=0.3.23,<0.4.0) ; extra == "inference"
 Requires-Dist: dask[complete] (>=2023.4.1,<2024.0.0) ; extra == "etl"
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: extruct (>=0.9.0) ; extra == "etl"
 Requires-Dist: goose3 (>=3.1.6) ; extra == "etl"
+Requires-Dist: gpt4all (>=0.2.3,<0.3.0) ; extra == "inference"
 Requires-Dist: hnswlib (>=0.6.2) ; extra == "etl" or extra == "inference"
 Requires-Dist: langdetect (>=1.0.8) ; extra == "etl"
 Requires-Dist: lxml (>=4.6.2)
 Requires-Dist: networkx (>=2.8.6,<3.0.0) ; extra == "etl"
 Requires-Dist: openai (>=0.27.4,<0.28.0) ; extra == "etl"
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0) ; extra == "etl" or extra == "inference"
```

