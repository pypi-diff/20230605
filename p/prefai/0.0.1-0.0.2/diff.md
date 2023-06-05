# Comparing `tmp/prefai-0.0.1.tar.gz` & `tmp/prefai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefai-0.0.1.tar", last modified: Wed May 31 05:29:15 2023, max compression
+gzip compressed data, was "prefai-0.0.2.tar", last modified: Mon Jun  5 21:22:20 2023, max compression
```

## Comparing `prefai-0.0.1.tar` & `prefai-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-05-31 05:29:15.813798 prefai-0.0.1/
--rw-r--r--   0 bjaros     (501) staff       (20)     1082 2023-05-31 04:10:37.000000 prefai-0.0.1/LICENSE.txt
--rw-r--r--   0 bjaros     (501) staff       (20)     1681 2023-05-31 05:29:15.813634 prefai-0.0.1/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)     1237 2023-05-31 04:45:13.000000 prefai-0.0.1/README.md
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-05-31 05:29:15.812638 prefai-0.0.1/prefai/
--rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.1/prefai/__init__.py
--rw-r--r--   0 bjaros     (501) staff       (20)     4456 2023-05-31 04:09:16.000000 prefai-0.0.1/prefai/client.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-05-31 05:29:15.813219 prefai-0.0.1/prefai.egg-info/
--rw-r--r--   0 bjaros     (501) staff       (20)     1681 2023-05-31 05:29:15.000000 prefai-0.0.1/prefai.egg-info/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-05-31 05:29:15.000000 prefai-0.0.1/prefai.egg-info/SOURCES.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-05-31 05:29:15.000000 prefai-0.0.1/prefai.egg-info/dependency_links.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-05-31 05:29:15.000000 prefai-0.0.1/prefai.egg-info/top_level.txt
--rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-05-31 05:29:15.813881 prefai-0.0.1/setup.cfg
--rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-05-31 05:28:10.000000 prefai-0.0.1/setup.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-05-31 05:29:15.813330 prefai-0.0.1/tests/
--rw-r--r--   0 bjaros     (501) staff       (20)     3195 2023-05-26 23:37:00.000000 prefai-0.0.1/tests/test_client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.503586 prefai-0.0.2/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1079 2023-06-01 06:14:59.000000 prefai-0.0.2/LICENSE.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-05 21:22:20.503379 prefai-0.0.2/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)     1238 2023-06-03 22:24:22.000000 prefai-0.0.2/README.md
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.502080 prefai-0.0.2/prefai/
+-rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.2/prefai/__init__.py
+-rw-r--r--   0 bjaros     (501) staff       (20)     4290 2023-06-05 21:09:53.000000 prefai-0.0.2/prefai/client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.502792 prefai-0.0.2/prefai.egg-info/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/SOURCES.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/dependency_links.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/top_level.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-06-05 21:22:20.503643 prefai-0.0.2/setup.cfg
+-rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-06-05 21:10:13.000000 prefai-0.0.2/setup.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.502915 prefai-0.0.2/tests/
+-rw-r--r--   0 bjaros     (501) staff       (20)     3204 2023-06-03 22:24:22.000000 prefai-0.0.2/tests/test_client.py
```

### Comparing `prefai-0.0.1/LICENSE.txt` & `prefai-0.0.2/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright (c) OpenAI (https://openai.com)
+Copyright (c) PrefAI (https://pref.ai)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `prefai-0.0.1/PKG-INFO` & `prefai-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.1
+Version: 0.0.2
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 The PrefAI Python Library enables applications coded in Python to interface with the PrefAI API.
 
 ## Installation
 
 Install with:
 
 ```bash
-npm install prefai
+pip install prefai
 ```
 
 ## Usage
 
 The library needs an API key, which you get on your [pref.ai developer account](https://pref.ai/dev/account/keys).
 
 ```bash
@@ -48,12 +48,12 @@
 
 prefai_client.api_key = os.getenv("PREFAI_API_KEY")
 test_user_email = os.getenv("PREFAI_TEST_USER_EMAIL")
 
 # Add record
 prefai_client.add_record(
     user_email = "test@pref.ai",
-    source_raw = "What's a spicy appetizer you'd recommend for a BBQ with 6 people?",
+    user_action = "What's a spicy appetizer you'd recommend for a BBQ with 6 people?",
 )
 ```
 
 For more information and next steps, read the [quickstart](https://pref.ai/dev/docs/quickstart).
```

### Comparing `prefai-0.0.1/README.md` & `prefai-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 The PrefAI Python Library enables applications coded in Python to interface with the PrefAI API.
 
 ## Installation
 
 Install with:
 
 ```bash
-npm install prefai
+pip install prefai
 ```
 
 ## Usage
 
 The library needs an API key, which you get on your [pref.ai developer account](https://pref.ai/dev/account/keys).
 
 ```bash
@@ -33,12 +33,12 @@
 
 prefai_client.api_key = os.getenv("PREFAI_API_KEY")
 test_user_email = os.getenv("PREFAI_TEST_USER_EMAIL")
 
 # Add record
 prefai_client.add_record(
     user_email = "test@pref.ai",
-    source_raw = "What's a spicy appetizer you'd recommend for a BBQ with 6 people?",
+    user_action = "What's a spicy appetizer you'd recommend for a BBQ with 6 people?",
 )
 ```
 
 For more information and next steps, read the [quickstart](https://pref.ai/dev/docs/quickstart).
```

### Comparing `prefai-0.0.1/prefai/client.py` & `prefai-0.0.2/prefai/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,33 +19,30 @@
         return f"Pref.ai request failed [{self.code}]: {self.detail}"
 
 
 class PrefaiTimeoutError(PrefaiError):
     pass
 
 class PrefaiClient:
-    # TODO TODO make production
-    # _api_base_url = 'https://api.pref.ai'
-    _api_base_url = 'http://127.0.0.1:8000'
+    _api_base_url = 'https://api.pref.ai'
 
     def __init__(self, api_key: str = None):
         if api_key:
             self.api_key = api_key
         else:
             self.api_key = os.getenv('PREFAI_API_KEY')
 
     def add_record(self,
-        source_raw: str,
+        user_action: str,
         context: Optional[str] = None,
         user_email: Optional[str] = None,
         user_id: Optional[str] = None,
-        source_summary: Optional[str] = None,
-        create_summary: Optional[bool] = False,
+        interaction_title: Optional[str] = None,
         observation: Optional[str] = None,
-        create_observation: Optional[bool] = False,
+        create_observation: Optional[bool] = True,
     ) -> Dict:
         """
         """
 
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
@@ -53,18 +50,17 @@
 
         try:
             response = requests.post(
                 f"{self._api_base_url}/v1/records/add",
                 json={
                     "user_email": user_email,
                     "user_id": user_id,
-                    "source_raw": source_raw,
+                    "user_action": user_action,
                     "context": context,
-                    "source_summary": source_summary,
-                    "create_summary": create_summary,
+                    "interaction_title": interaction_title,
                     "observation": observation,
                     "create_observation": create_observation,
                 },
                 headers=headers,
                 timeout=5
             )
 
@@ -93,15 +89,15 @@
                 code=http_err.response.status_code,
                 detail=detail,
                 headers=http_err.response.headers or {},
             )
 
 
     def retrieve_records(self,
-        source_raw: str,
+        user_action: str,
         context: Optional[str] = None,
         user_email: Optional[str] = None,
         user_id: Optional[str] = None,
         max_num_results: Optional[int] = 3,
         min_similarity: Optional[float] = None,
     ) -> Dict:
 
@@ -111,15 +107,15 @@
         }
 
         try:
             response = requests.post(
                 f"{self._api_base_url}/v1/records/retrieve",
                 json={
                     "context": context,
-                    "source_raw": source_raw,
+                    "user_action": user_action,
                     "user_email": user_email,
                     "user_id": user_id,
                     "max_num_results": max_num_results,
                     "min_similarity": min_similarity,
                 },
                 headers=headers,
                 timeout=5
```

### Comparing `prefai-0.0.1/prefai.egg-info/PKG-INFO` & `prefai-0.0.2/prefai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.1
+Version: 0.0.2
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 The PrefAI Python Library enables applications coded in Python to interface with the PrefAI API.
 
 ## Installation
 
 Install with:
 
 ```bash
-npm install prefai
+pip install prefai
 ```
 
 ## Usage
 
 The library needs an API key, which you get on your [pref.ai developer account](https://pref.ai/dev/account/keys).
 
 ```bash
@@ -48,12 +48,12 @@
 
 prefai_client.api_key = os.getenv("PREFAI_API_KEY")
 test_user_email = os.getenv("PREFAI_TEST_USER_EMAIL")
 
 # Add record
 prefai_client.add_record(
     user_email = "test@pref.ai",
-    source_raw = "What's a spicy appetizer you'd recommend for a BBQ with 6 people?",
+    user_action = "What's a spicy appetizer you'd recommend for a BBQ with 6 people?",
 )
 ```
 
 For more information and next steps, read the [quickstart](https://pref.ai/dev/docs/quickstart).
```

### Comparing `prefai-0.0.1/setup.py` & `prefai-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="prefai",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     author="Bobby Jaros",
     author_email="bobby@pref.ai",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="http://github.com/prefai/pythonclient",
```

### Comparing `prefai-0.0.1/tests/test_client.py` & `prefai-0.0.2/tests/test_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def test_add_record_bad_api_key():
     orig_api_key = prefai_client.api_key 
     prefai_client.api_key = "BAD KEY"
     success = False
     try:
         prefai_client.add_record(
             user_email = test_user_email,
-            source_raw = "Does this recipe have tree nuts? Can you modify if so?",
+            user_action = "Does this recipe have tree nuts? Can you modify if so?",
         )
         success = True
     except PrefaiError as e:
         assert e.code == 401
         assert e.detail == 'Invalid API key'
     assert not success
     prefai_client.api_key = orig_api_key
@@ -22,29 +22,29 @@
 def test_add_record_none_api_key():
     orig_api_key = prefai_client.api_key 
     prefai_client.api_key = None
     success = False
     try:
         prefai_client.add_record(
             user_email = test_user_email,
-            source_raw = "Does this recipe have tree nuts? Can you modify if so?",
+            user_action = "Does this recipe have tree nuts? Can you modify if so?",
         )
         success = True
     except PrefaiError as e:
         assert e.code == 401
         assert e.detail == 'Invalid API key'
     assert not success
     prefai_client.api_key = orig_api_key
 
 def test_add_record_missing_user():
     success = False
     try:
         prefai_client.add_record(
             # Missing user_email or user_id
-            source_raw = "Does this recipe have tree nuts? Can you modify if so?",
+            user_action = "Does this recipe have tree nuts? Can you modify if so?",
         )
         success = True
     except PrefaiError as e:
         assert e.code == 422
         assert e.detail == "Either user_email or user_id must be provided (but not both)"
     assert not success
 
@@ -53,50 +53,50 @@
     try:
         prefai_client.add_record(
             user_email = test_user_email,
             # Missing source
         )
         success = True
     except TypeError as e:
-        assert e.args[0] == "add_record() missing 1 required positional argument: 'source_raw'"
+        assert e.args[0] == "add_record() missing 1 required positional argument: 'user_action'"
     assert not success
 
 
 def test_add():
     res = prefai_client.add_record(
         user_email = test_user_email,
-        source_raw = "Does this recipe have tree nuts? Can you modify if so?",
+        user_action = "Does this recipe have tree nuts? Can you modify if so?",
     )
     assert res.get('success')
     assert 'record_id' in res
 
 def test_add_with_context():
     res = prefai_client.add_record(
         user_email = test_user_email,
         context = """User: How do I ask someone's name in French?
         
         AI: You would ask: "Comment vous appelez-vous?" """,
-        source_raw = "Is that a casual way to ask? I don't want to sound too formal.",
+        user_action = "Is that a casual way to ask? I don't want to sound too formal.",
     )
     assert res.get('success')
     assert 'record_id' in res
 
 def test_add_record_with_unknown_email():
     user_email = "unknown-email@pref.ai"
     res = prefai_client.add_record(
         user_email = user_email,
-        source_raw = "Does this recipe have tree nuts? Can you modify if so?",
+        user_action = "Does this recipe have tree nuts? Can you modify if so?",
     )
     assert res.get('success')
     assert 'record_id' in res
 
 def test_retrieve():
     res = prefai_client.retrieve_records(
         user_email = test_user_email,
         context = "User",
-        source_raw = "How do you say I love you in Spanish?",
+        user_action = "How do you say I love you in Spanish?",
         min_similarity = -1.0
     )
     assert res.get('success')
-    assert res['records'][0]['source_raw'].startswith('Is that a casual way to ask?')
+    assert res['records'][0]['user_action'].startswith('Is that a casual way to ask?')
     print(res['records'])
```

