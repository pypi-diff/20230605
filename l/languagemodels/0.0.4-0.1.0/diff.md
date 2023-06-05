# Comparing `tmp/languagemodels-0.0.4.tar.gz` & `tmp/languagemodels-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.0.4.tar", last modified: Mon May 15 18:09:36 2023, max compression
+gzip compressed data, was "languagemodels-0.1.0.tar", last modified: Mon Jun  5 16:27:38 2023, max compression
```

## Comparing `languagemodels-0.0.4.tar` & `languagemodels-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-15 18:09:36.367425 languagemodels-0.0.4/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3925 2023-05-15 18:09:36.367425 languagemodels-0.0.4/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-15 18:09:36.367425 languagemodels-0.0.4/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7513 2023-05-15 17:19:44.000000 languagemodels-0.0.4/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2265 2023-05-09 19:09:44.000000 languagemodels-0.0.4/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3639 2023-05-15 17:19:44.000000 languagemodels-0.0.4/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-15 18:09:36.367425 languagemodels-0.0.4/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3925 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       52 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-05-15 18:09:36.367425 languagemodels-0.0.4/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-05-15 18:09:27.000000 languagemodels-0.0.4/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 16:27:38.733426 languagemodels-0.1.0/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 16:27:38.729426 languagemodels-0.1.0/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 16:27:38.729426 languagemodels-0.1.0/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8043 2023-06-05 16:26:20.000000 languagemodels-0.1.0/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:26:20.000000 languagemodels-0.1.0/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     5984 2023-06-05 16:26:20.000000 languagemodels-0.1.0/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 16:27:38.729426 languagemodels-0.1.0/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 16:27:38.000000 languagemodels-0.1.0/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-05 16:27:38.000000 languagemodels-0.1.0/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-05 16:27:38.000000 languagemodels-0.1.0/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-05 16:27:38.000000 languagemodels-0.1.0/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-05 16:27:38.000000 languagemodels-0.1.0/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-05 16:27:38.733426 languagemodels-0.1.0/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-05 16:27:22.000000 languagemodels-0.1.0/setup.py
```

### Comparing `languagemodels-0.0.4/languagemodels/__init__.py` & `languagemodels-0.1.0/languagemodels/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,47 @@
 import requests
 import datetime
 import json
 
-from languagemodels.inference import generate_instruct, get_pipeline, convert_chat
+from languagemodels.inference import generate_instruct, convert_chat, list_tokens
 from languagemodels.embeddings import RetrievalContext
 
 docs = RetrievalContext()
 
 
+def print_tokens(prompt: str) -> None:
+    """Prints a list of tokens in a prompt
+
+    This function is provided for exploratory purposes only. It may return
+    different tokens than the underlying model and may not match the
+    tokenization of any backend API being used.
+
+    :param prompt: Prompt to use as input to tokenizer
+    :return: Nothing
+
+    Examples:
+
+    >>> print_tokens("Hello world")
+    ' Hello' (token 8774)
+    ' world' (token 296)
+
+    >>> print_tokens("Hola mundo")
+    ' Hol' (token 5838)
+    'a' (token 9)
+    ' mun' (token 13844)
+    'd' (token 26)
+    'o' (token 32)
+    """
+
+    tokens = list_tokens(prompt)
+
+    for token in tokens:
+        print(f"'{token[0].replace('▁',' ')}' (token {token[1]})")
+
+
 def complete(prompt: str) -> str:
     """Provide one completion for a given open-ended prompt
 
     :param prompt: Prompt to use as input to the model
     :return: Completion returned from the language model
 
     Examples:
@@ -32,25 +62,22 @@
     """Follow a single-turn instructional prompt
 
     :param prompt: Instructional prompt to follow
     :return: Completion returned from the language model
 
     Examples:
 
-    >>> do("Translate to Spanish: Hello, world!")
-    'Hola, mundo!'
+    >>> do("Translate Spanish to English: Hola mundo!")
+    'Hello world!'
 
     >>> do("Pick the sport: baseball, texas, chemistry")
-    'baseball'
+    'Baseball.'
 
     >>> do("Is the following positive or negative: I love Star Trek.")
-    'positive'
-
-    >>> do("Does this make sense: The course is jumping well.")
-    'no'
+    'Positive.'
     """
     return generate_instruct(prompt, max_tokens=200)
 
 
 def chat(prompt: str) -> str:
     """Get new message from chat-optimized language model
 
@@ -73,21 +100,21 @@
     <|assistant|>The capital of Germany is Berlin.<|endoftext|>
     <|prompter|>How many people live there?<|endoftext|>
     <|assistant|>
     ```
 
     The completion from the language model is returned.
 
-    :param message: List of message as (role, content) tuples
+    :param message: Prompt using formatting described above
     :return: Completion returned from the language model
 
     >>> chat("<|system|>It is 5:15pm. Assistant is helpful<|endoftext|>" \\
-    ...      "<|prompter|>Do you know what time it is?<|endoftext|>" \\
+    ...      "<|prompter|>What time is it?<|endoftext|>" \\
     ...      "<|assistant|>")
-    'It is 5:15pm.'
+    '5:15pm.'
     """
 
     prompt = convert_chat(prompt)
 
     return generate_instruct(prompt, max_tokens=200)
 
 
@@ -98,53 +125,44 @@
     It may not always be a correct or meaningful answer, but it will never be
     an arbitrary hallucination.
 
     :param question: A question to answer using knowledge from context
     :param context: Knowledge used to answer the question
     :return: Answer to the question.
 
-    >>> extract_answer("What color is the ball?", "There is a green ball and a red box")
+    >>> context = "There is a green ball and a red box"
+    >>> extract_answer("What color is the ball?", context) #doctest: +SKIP
     'green'
-    >>> extract_answer("Who created Python?", fetch_wiki('Python'))
+    >>> extract_answer("Who created Python?", fetch_wiki('Python')) #doctest: +SKIP
     'Guido van Rossum'
     """
 
-    qa = get_pipeline("question-answering", "distilbert-base-cased-distilled-squad")
-
-    return qa(question, context)["answer"]
+    return generate_instruct(f"{context}\n\n{question}")
 
 
 def classify(doc: str, label1: str, label2: str) -> str:
     """Performs binary classification on an input
 
     :param doc: A plain text input document to classify
     :param label1: The first label to classify against
     :param label2: The second label to classify against
     :return: The closest matching class. The return value will always be
     `label1` or `label2`
 
-    >>> classify("I love you!","positive","negative")
+    >>> classify("I love you!","positive","negative") #doctest: +SKIP
     'positive'
-    >>> classify("That book was fine.","positive","negative")
+    >>> classify("That book was fine.","positive","negative") #doctest: +SKIP
     'positive'
-    >>> classify("That movie was terrible.","positive","negative")
+    >>> classify("That movie was terrible.","positive","negative") #doctest: +SKIP
     'negative'
-    >>> classify("The submarine is diving", "ocean", "space")
+    >>> classify("The submarine is diving", "ocean", "space") #doctest: +SKIP
     'ocean'
     """
 
-    classifier = get_pipeline(
-        "zero-shot-classification", "valhalla/distilbart-mnli-12-1"
-    )
-
-    result = classifier(doc, [label1, label2])
-
-    top = max(zip(result["scores"], result["labels"]), key=lambda r: r[0])
-
-    return top[1]
+    return generate_instruct(f'{doc}\n\nClassify as "{label1}" or "{label2}":')
 
 
 def store_doc(doc: str) -> None:
     """Store document for later retrieval
 
     :param doc: A plain text document to store.
 
@@ -157,16 +175,16 @@
     """Load a matching document
 
     A single document that best matches `query` will be returned.
 
     :param query: Query to compare to stored documents
     :return: Content of the closest matching document
 
-    >>> store_doc("The sky is blue.")
     >>> store_doc("Paris is in France.")
+    >>> store_doc("The sky is blue.")
     >>> load_doc("Where is Paris?")
     'Paris is in France.'
     """
     return docs.get_match(query)
 
 
 def fetch_wiki(topic: str) -> str:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

