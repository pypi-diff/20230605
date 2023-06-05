# Comparing `tmp/bareunpy-1.6.0.tar.gz` & `tmp/bareunpy-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareunpy-1.6.0.tar", max compression
+gzip compressed data, was "bareunpy-1.6.1.tar", max compression
```

## Comparing `bareunpy-1.6.0.tar` & `bareunpy-1.6.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1547 2023-01-31 05:55:04.322163 bareunpy-1.6.0/LICENSE
--rw-r--r--   0        0        0     4119 2023-02-03 10:49:16.423445 bareunpy-1.6.0/README.md
--rw-r--r--   0        0        0     1432 2023-02-16 05:54:33.395859 bareunpy-1.6.0/bareunpy/__init__.py
--rw-r--r--   0        0        0     7481 2023-02-03 05:03:48.308582 bareunpy-1.6.0/bareunpy/_custom_dict.py
--rw-r--r--   0        0        0     6006 2023-02-03 05:52:01.607848 bareunpy-1.6.0/bareunpy/_custom_dict_client.py
--rw-r--r--   0        0        0     3427 2023-02-03 05:48:12.726778 bareunpy-1.6.0/bareunpy/_lang_service_client.py
--rw-r--r--   0        0        0     8871 2023-02-16 05:56:41.736197 bareunpy-1.6.0/bareunpy/_tagger.py
--rw-r--r--   0        0        0     9633 2023-02-03 05:02:41.306079 bareunpy-1.6.0/bareunpy/_tokenizer.py
--rw-r--r--   0        0        0     1379 2023-02-16 05:57:26.083676 bareunpy-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 bareunpy-1.6.0/setup.py
--rw-r--r--   0        0        0     5903 1970-01-01 00:00:00.000000 bareunpy-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1547 2023-01-30 00:41:12.108840 bareunpy-1.6.1/LICENSE
+-rw-r--r--   0        0        0     4119 2023-03-24 00:58:50.777709 bareunpy-1.6.1/README.md
+-rw-r--r--   0        0        0     1432 2023-06-05 09:40:00.081909 bareunpy-1.6.1/bareunpy/__init__.py
+-rw-r--r--   0        0        0     7475 2023-06-05 09:39:16.952459 bareunpy-1.6.1/bareunpy/_custom_dict.py
+-rw-r--r--   0        0        0     6006 2023-06-05 09:39:16.952459 bareunpy-1.6.1/bareunpy/_custom_dict_client.py
+-rw-r--r--   0        0        0     3427 2023-03-24 00:58:50.781709 bareunpy-1.6.1/bareunpy/_lang_service_client.py
+-rw-r--r--   0        0        0     8871 2023-03-24 00:58:50.781709 bareunpy-1.6.1/bareunpy/_tagger.py
+-rw-r--r--   0        0        0     9633 2023-03-24 00:58:50.781709 bareunpy-1.6.1/bareunpy/_tokenizer.py
+-rw-r--r--   0        0        0     1379 2023-06-05 09:39:47.193476 bareunpy-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5903 1970-01-01 00:00:00.000000 bareunpy-1.6.1/PKG-INFO
```

### Comparing `bareunpy-1.6.0/LICENSE` & `bareunpy-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.0/README.md` & `bareunpy-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.0/bareunpy/__init__.py` & `bareunpy-1.6.1/bareunpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 
 from bareunpy._tagger import Tagger, Tagged
 from bareunpy._tokenizer import Tokenizer, Tokenized
 from bareunpy._custom_dict import CustomDict
 from bareunpy._custom_dict_client import CustomDictionaryServiceClient
 from bareunpy._lang_service_client import BareunLanguageServiceClient
 
-version = "1.6.0"
+version = "1.6.1"
 bareun_version = "1.8.0"
```

### Comparing `bareunpy-1.6.0/bareunpy/_custom_dict.py` & `bareunpy-1.6.1/bareunpy/_custom_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,24 +169,24 @@
         집합을 복합명사 분리 사전으로 지정합니다.
 
         Args:
             dict_set (set): 복합명사 분리 사전
         """
         self.cp_caret_set = dict_set
 
-    def copy_cp_vv_set(self, dict_set: set):
+    def copy_vv_set(self, dict_set: set):
         """
         집합을 동사 사전으로 지정합니다.
 
         Args:
             dict_set (set): 동사 사전
         """
         self.vv_set = dict_set
 
-    def copy_cp_va_set(self, dict_set: set):
+    def copy_va_set(self, dict_set: set):
         """
         집합을 형용사 사전으로 지정합니다.
 
         Args:
             dict_set (set): 형용사 사전
         """
         self.va_set = dict_set
```

### Comparing `bareunpy-1.6.0/bareunpy/_custom_dict_client.py` & `bareunpy-1.6.1/bareunpy/_custom_dict_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,16 @@
         req = pb.UpdateCustomDictionaryRequest()
         req.domain_name = domain
 
         req.dict.domain_name = domain
 
         req.dict.np_set.CopyFrom(build_dict_set(domain, 'np-set', np))
         req.dict.cp_set.CopyFrom(build_dict_set(domain, 'cp-set', cp))
-        req.dict.vv_set.CopyFrom(build_dict_set(domain, 'vv-set', cp))
-        req.dict.va_set.CopyFrom(build_dict_set(domain, 'va-set', cp))
+        req.dict.vv_set.CopyFrom(build_dict_set(domain, 'vv-set', vv))
+        req.dict.va_set.CopyFrom(build_dict_set(domain, 'va-set', va))
         req.dict.cp_caret_set.CopyFrom(
             build_dict_set(domain, 'cp-caret-set', cp_caret))
 
         try:
             res, c = self.stub.UpdateCustomDictionary.with_call(
                 request=req, metadata=self.metadata)
             return res.updated_domain_name == domain
```

### Comparing `bareunpy-1.6.0/bareunpy/_lang_service_client.py` & `bareunpy-1.6.1/bareunpy/_lang_service_client.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.0/bareunpy/_tagger.py` & `bareunpy-1.6.1/bareunpy/_tagger.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.0/bareunpy/_tokenizer.py` & `bareunpy-1.6.1/bareunpy/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.0/pyproject.toml` & `bareunpy-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bareunpy"
-version = "1.6.0"
+version = "1.6.1"
 description = "The bareun python library using grpc"
 authors = ["Gihyun YUN <gih2yun@baikal.ai>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://bareun.ai/"
 repository = "https://github.com/bareun-nlp/bareunpy"
 keywords = [ "NLP", "Korean", "Deep Learning", "POS tagger", "bareun"]
```

### Comparing `bareunpy-1.6.0/PKG-INFO` & `bareunpy-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareunpy
-Version: 1.6.0
+Version: 1.6.1
 Summary: The bareun python library using grpc
 Home-page: https://bareun.ai/
 License: BSD-3-Clause
 Keywords: NLP,Korean,Deep Learning,POS tagger,bareun
 Author: Gihyun YUN
 Author-email: gih2yun@baikal.ai
 Requires-Python: >=3.6,<4.0
```

