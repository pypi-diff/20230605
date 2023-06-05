# Comparing `tmp/languagemodels-0.1.1.tar.gz` & `tmp/languagemodels-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.1.1.tar", last modified: Mon Jun  5 16:53:37 2023, max compression
+gzip compressed data, was "languagemodels-0.1.2.tar", last modified: Mon Jun  5 17:01:32 2023, max compression
```

## Comparing `languagemodels-0.1.1.tar` & `languagemodels-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 16:53:37.975765 languagemodels-0.1.1/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 16:53:37.975765 languagemodels-0.1.1/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 16:53:37.971765 languagemodels-0.1.1/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8050 2023-06-05 16:38:46.000000 languagemodels-0.1.1/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:26:20.000000 languagemodels-0.1.1/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     5984 2023-06-05 16:26:20.000000 languagemodels-0.1.1/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 16:53:37.971765 languagemodels-0.1.1/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 16:53:37.000000 languagemodels-0.1.1/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-05 16:53:37.000000 languagemodels-0.1.1/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-05 16:53:37.000000 languagemodels-0.1.1/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-05 16:53:37.000000 languagemodels-0.1.1/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-05 16:53:37.000000 languagemodels-0.1.1/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-05 16:53:37.975765 languagemodels-0.1.1/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-05 16:53:07.000000 languagemodels-0.1.1/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 17:01:32.532605 languagemodels-0.1.2/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 17:01:32.532605 languagemodels-0.1.2/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 17:01:32.528605 languagemodels-0.1.2/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8050 2023-06-05 16:58:20.000000 languagemodels-0.1.2/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:58:20.000000 languagemodels-0.1.2/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6128 2023-06-05 16:58:20.000000 languagemodels-0.1.2/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 17:01:32.532605 languagemodels-0.1.2/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-05 17:01:32.532605 languagemodels-0.1.2/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-05 17:01:21.000000 languagemodels-0.1.2/setup.py
```

### Comparing `languagemodels-0.1.1/PKG-INFO` & `languagemodels-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
```

### Comparing `languagemodels-0.1.1/languagemodels/__init__.py` & `languagemodels-0.1.2/languagemodels/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     'positive'
     >>> classify("That movie was terrible.","positive","negative") #doctest: +SKIP
     'negative'
     >>> classify("The submarine is diving", "ocean", "space") #doctest: +SKIP
     'ocean'
     """
 
-    return generate_instruct(f'Classify as {label1} or {label2}: {doc}', max_tokens=5)
+    return generate_instruct(f"Classify as {label1} or {label2}: {doc}", max_tokens=5)
 
 
 def store_doc(doc: str) -> None:
     """Store document for later retrieval
 
     :param doc: A plain text document to store.
```

### Comparing `languagemodels-0.1.1/languagemodels/embeddings.py` & `languagemodels-0.1.2/languagemodels/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def store(self, doc):
         writer = self.index.writer()
         writer.add_document(content=doc)
         writer.commit()
 
     def get_match(self, query):
         with self.index.searcher() as searcher:
-            query = re.sub(r'[,\.\?\!\:\;]', ' ', query)
+            query = re.sub(r"[,\.\?\!\:\;]", " ", query)
             qp = QueryParser("content", self.index.schema, group=OrGroup)
             query = qp.parse(query)
             results = searcher.search(query)
 
             try:
                 return results[0]["content"]
             except IndexError:
```

### Comparing `languagemodels-0.1.1/languagemodels/inference.py` & `languagemodels-0.1.2/languagemodels/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,20 @@
 
     if os.environ.get("oa_key"):
         return generate_oa("text-babbage-001", prompt, max_tokens)
 
     tokenizer, model = get_model("jncraton/LaMini-Flan-T5-248M-ct2-int8")
 
     input_tokens = tokenizer.EncodeAsPieces(prompt) + ["</s>"]
-    results = model.translate_batch([input_tokens])
+    results = model.translate_batch(
+        [input_tokens],
+        repetition_penalty=repetition_penalty,
+        max_decoding_length=max_tokens,
+        sampling_temperature=temperature,
+    )
 
     output_tokens = results[0].hypotheses[0]
 
     return tokenizer.DecodePieces(output_tokens)
 
 
 def convert_chat(prompt):
```

### Comparing `languagemodels-0.1.1/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.1.2/languagemodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
```

### Comparing `languagemodels-0.1.1/setup.py` & `languagemodels-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.1.1",
+    version="0.1.2",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```

