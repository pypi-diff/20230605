# Comparing `tmp/tokflow-1.1.0.tar.gz` & `tmp/tokflow-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokflow-1.1.0.tar", last modified: Sun Jun  4 09:55:50 2023, max compression
+gzip compressed data, was "tokflow-1.2.0.tar", last modified: Mon Jun  5 07:48:20 2023, max compression
```

## Comparing `tokflow-1.1.0.tar` & `tokflow-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.148610 tokflow-1.1.0/
--rw-rw-rw-   0        0        0    11364 2023-05-19 04:51:42.000000 tokflow-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     6114 2023-06-04 09:55:50.148610 tokflow-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5349 2023-06-04 09:53:45.000000 tokflow-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.111327 tokflow-1.1.0/TokFlow.egg-info/
--rw-rw-rw-   0        0        0     6114 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 09:55:50.148610 tokflow-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-06-04 09:54:55.000000 tokflow-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.128874 tokflow-1.1.0/tests/
--rw-rw-rw-   0        0        0     8777 2023-05-19 04:51:42.000000 tokflow-1.1.0/tests/test_refit_flow_worker.py
--rw-rw-rw-   0        0        0    12117 2023-05-19 04:51:42.000000 tokflow-1.1.0/tests/test_tokflow_01_IN_spot_OUT_spot.py
--rw-rw-rw-   0        0        0     1394 2023-06-04 07:54:15.000000 tokflow-1.1.0/tests/test_tokflow_02_IN_full_OUT_spot.py
--rw-rw-rw-   0        0        0    32891 2023-06-04 06:56:56.000000 tokflow-1.1.0/tests/test_tokflow_02_data.py
--rw-rw-rw-   0        0        0     1649 2023-06-04 09:37:08.000000 tokflow-1.1.0/tests/test_tokflow_03_IN_spot_OUT_full.py
--rw-rw-rw-   0        0        0     1229 2023-06-04 09:38:29.000000 tokflow-1.1.0/tests/test_tokflow_04_IN_full_OUT_full.py
-drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.146611 tokflow-1.1.0/tokflow/
--rw-rw-rw-   0        0        0       72 2023-05-19 05:04:54.000000 tokflow-1.1.0/tokflow/__init__.py
--rw-rw-rw-   0        0        0    11997 2023-06-04 09:35:11.000000 tokflow-1.1.0/tokflow/tok_flow.py
--rw-rw-rw-   0        0        0     9059 2023-05-19 04:51:42.000000 tokflow-1.1.0/tokflow/tok_flow_worker.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:48:20.339767 tokflow-1.2.0/
+-rw-rw-rw-   0        0        0    35148 2023-06-05 07:47:39.000000 tokflow-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     8716 2023-06-05 07:48:20.338768 tokflow-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7849 2023-06-05 07:47:39.000000 tokflow-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 07:48:20.309879 tokflow-1.2.0/TokFlow.egg-info/
+-rw-rw-rw-   0        0        0     8716 2023-06-05 07:48:20.000000 tokflow-1.2.0/TokFlow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-06-05 07:48:20.000000 tokflow-1.2.0/TokFlow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:48:20.000000 tokflow-1.2.0/TokFlow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 07:48:20.000000 tokflow-1.2.0/TokFlow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:48:20.339767 tokflow-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      949 2023-06-05 07:47:39.000000 tokflow-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:48:20.330766 tokflow-1.2.0/tests/
+-rw-rw-rw-   0        0        0     8852 2023-06-05 07:47:39.000000 tokflow-1.2.0/tests/test_refit_flow_worker.py
+-rw-rw-rw-   0        0        0     4326 2023-06-05 07:47:39.000000 tokflow-1.2.0/tests/test_sentence_stop.py
+-rw-rw-rw-   0        0        0     1726 2023-06-05 07:47:39.000000 tokflow-1.2.0/tests/test_sentence_stop_data.py
+-rw-rw-rw-   0        0        0     4086 2023-06-05 07:47:39.000000 tokflow-1.2.0/tests/test_sentence_stop_spot_mode.py
+-rw-rw-rw-   0        0        0    12117 2023-05-19 04:51:42.000000 tokflow-1.2.0/tests/test_tokflow_01_IN_spot_OUT_spot.py
+-rw-rw-rw-   0        0        0     1394 2023-06-04 07:54:15.000000 tokflow-1.2.0/tests/test_tokflow_02_IN_full_OUT_spot.py
+-rw-rw-rw-   0        0        0    32891 2023-06-04 06:56:56.000000 tokflow-1.2.0/tests/test_tokflow_02_data.py
+-rw-rw-rw-   0        0        0     1649 2023-06-04 09:37:08.000000 tokflow-1.2.0/tests/test_tokflow_03_IN_spot_OUT_full.py
+-rw-rw-rw-   0        0        0     1229 2023-06-04 09:38:29.000000 tokflow-1.2.0/tests/test_tokflow_04_IN_full_OUT_full.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:48:20.336765 tokflow-1.2.0/tokflow/
+-rw-rw-rw-   0        0        0      112 2023-06-05 07:47:39.000000 tokflow-1.2.0/tokflow/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-06-05 07:47:39.000000 tokflow-1.2.0/tokflow/sentence_stop.py
+-rw-rw-rw-   0        0        0    13942 2023-06-05 07:47:39.000000 tokflow-1.2.0/tokflow/tok_flow.py
+-rw-rw-rw-   0        0        0     9571 2023-06-05 07:47:39.000000 tokflow-1.2.0/tokflow/tok_flow_worker.py
```

### Comparing `tokflow-1.1.0/PKG-INFO` & `tokflow-1.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,180 @@
-Metadata-Version: 2.1
-Name: tokflow
-Version: 1.1.0
-Summary: LLM utility of streaming token realtime replacement processing
-Home-page: https://github.com/riversun/TokFlow
-Author: Tom Misawa
-Author-email: riversun.org@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TokFlow
-
-[&#26085;&#26412;&#35486;](https://github.com/riversun/TokFlow/blob/main/README_ja.md)
-
-
-
-Utility that outputs tokens generated by a large language model (LLM) with sequential replacement processing
-
-## How it works
-
-The tokens are entered one after the other as small pieces as shown below.
-
-```python
-["He","llo"," ","t","h","ere","!<","N","L>m","y ","nam","e"," ","is"," tokfl","ow.","<","N","L>N","ice"," to ","me","et you."]
-```
-
-The input tokens are output, with `<NL>` replaced by `\n` each time.
-
-
-![tokflow](https://github.com/riversun/TokFlow/assets/11747460/85f497bd-cf51-41d9-aaf5-ad5420f42b6a)
-
-
-You can specify any string to be replaced.
-Moreover, you can specify multiple replacement targets.
-
-## What is this library for?
-
-I developed this for the purpose of outputting special tokens with successive replacements in sequential sentence generation using a large-scale language model, which is a generative AI, but it may also be used for other string stream processing.
-
-# Install
-
-```
-pip install tokflow
-```
-
-# Usage
-
-```python
-import time
-from tokflow import TokFlow
-
-TOKEN_GENERATOR_MOCK = ["He", "llo", " ", "t", "h", "ere", "!<", "N", "L>m", "y ", "nam", "e", " ", "is", " tokfl", "ow.",
-                  "<", "N", "L>N", "ice", " to ", "me", "et you."]
-
-# replace "<NL>" with "\n". "<NL>" is called "search target string".
-# Multiple replacement conditions can be specified.
-tokf = TokFlow([("<NL>", "\n")])
-
-for input_token in TOKEN_GENERATOR_MOCK:
-
-    output_token = tokf.put(input_token)
-
-    # Input sequential tokens.
-    # If there is a possibility that the token is a "search target string",
-    # it is buffered for a while, so output_token may be empty for a while.
-    print(f"{output_token}", end="", flush=True)
-
-    # Included wait to show the sequential generation operation.
-    time.sleep(0.3)
-
-
-# Remember to output the remaining buffer at the very end. Buffers may be empty characters.
-print(f"{tokf.flush()}", end="", flush=True)
-
-```
-
-
-![tokflow](https://github.com/riversun/TokFlow/assets/11747460/85f497bd-cf51-41d9-aaf5-ad5420f42b6a)
-
-# Generation Options
-
-The `put` method can take an optional parameter `opts` like `put(text,opts)`.
-
-`opts` can specify the format of the input and output, like `{"in_type":"spot","out_type:"spot" }`.
-
-It behaves as follows:
-
-| in_type  | out_type | Description                                    |
-| :------- | :------- | :---------------------------------------------- |
-| spot     | spot     | A mode that incrementally sends tokens to the `put` method, and outputs generated segments each time. |
-| spot     | full     | A mode that incrementally sends tokens to the `put` method, but outputs the full sentence. |
-| full     | spot     | A mode that sends the full sentence to the `put` method at once, but outputs generated segments each time. |
-| full     | full     | A mode that sends the full sentence to the `put` method at once, and outputs the full sentence. |
-
-Notes:
-- All text strings need to be sent to the `put` method before calling the `flush` method. Especially in `full` mode, all input strings are sent at once.
-- If the output type (`out_type`) is `full`, the `flush` method must be called to obtain the final result.
-- It's important to appropriately combine the call pattern of the `put` method and the use of the `flush` method to maintain consistency in each mode.
-
-**Code Example**
-
-Specify rules like `condition = {"in_type": "full", "out_type": "full"}`, and use `condition` as an argument for `put` and `flush`.
-
-```python
-    tokf = TokFlow([("<NL>", "\n")])
-
-    condition = {"in_type": "full", "out_type": "full"}
-    prev_len = 0
-    for input_token_base in get_example_texts():
-        output_sentence = tokf.put(input_token_base, condition)
-
-        print(f"output_sentence:{output_sentence}")
-
-        if prev_len > len(output_sentence):
-            raise ValueError("Length error")
-
-        if "<NL>" in output_sentence:
-            raise Exception("Failure Must be converted str found.")
-
-        prev_len = len(output_sentence)
-
-    output_sentence = tokf.flush(condition)
-```
-
-# Processing
-
-## About Internal processing
-
-Tokens are sequentially read in real time.
-The token read is combined with the tokens read so far, referred to as the "token buffer".
-In this sequential process, when a pre-specified string (hereafter referred to
-as the "search target string") appears in the token buffer,
-this string is replaced with another string (hereafter referred to as the "replacement string").
-Since tokens are read sequentially, in the intermediate stage,
-a string that is unrelated to the search target string or part of the search target string accumulates
-in the token buffer. If the token buffer is composed in an order that cannot be a search target string,
-the token buffer is returned as the method's return value the moment such a determination is made.
-On the other hand, if the token buffer is composed in an order that could be a search target string,
-the return value remains an empty string until either the search target string appears or
-it is determined that it cannot be a search target string.
-In this way, by buffering until the appearance of the search target string,
-most sequential tokens can be displayed as they are, while replacement is delayed when necessary,
-enabling stream processing.
-
+# TokFlow
+
+[&#26085;&#26412;&#35486;](https://github.com/riversun/TokFlow/blob/main/README_ja.md)
+
+
+
+Utility that outputs tokens generated by a large language model (LLM) with sequential replacement processing
+
+## How it works
+
+The tokens are entered one after the other as small pieces as shown below.
+
+```python
+["He","llo"," ","t","h","ere","!<","N","L>m","y ","nam","e"," ","is"," tokfl","ow.","<","N","L>N","ice"," to ","me","et you."]
+```
+
+The input tokens are output, with `<NL>` replaced by `\n` each time.
+
+
+![tokflow](https://github.com/riversun/TokFlow/assets/11747460/85f497bd-cf51-41d9-aaf5-ad5420f42b6a)
+
+
+You can specify any string to be replaced.
+Moreover, you can specify multiple replacement targets.
+
+## What is this library for?
+
+I developed this for the purpose of outputting special tokens with successive replacements in sequential sentence generation using a large-scale language model, which is a generative AI, but it may also be used for other string stream processing.
+
+# Install
+
+```
+pip install tokflow
+```
+
+# Usage
+
+```python
+import time
+from tokflow import TokFlow
+
+TOKEN_GENERATOR_MOCK = ["He", "llo", " ", "t", "h", "ere", "!<", "N", "L>m", "y ", "nam", "e", " ", "is", " tokfl", "ow.",
+                  "<", "N", "L>N", "ice", " to ", "me", "et you."]
+
+# replace "<NL>" with "\n". "<NL>" is called "search target string".
+# Multiple replacement conditions can be specified.
+tokf = TokFlow([("<NL>", "\n")])
+
+for input_token in TOKEN_GENERATOR_MOCK:
+
+    output_token = tokf.put(input_token)
+
+    # Input sequential tokens.
+    # If there is a possibility that the token is a "search target string",
+    # it is buffered for a while, so output_token may be empty for a while.
+    print(f"{output_token}", end="", flush=True)
+
+    # Included wait to show the sequential generation operation.
+    time.sleep(0.3)
+
+
+# Remember to output the remaining buffer at the very end. Buffers may be empty characters.
+print(f"{tokf.flush()}", end="", flush=True)
+
+```
+
+
+![tokflow](https://github.com/riversun/TokFlow/assets/11747460/85f497bd-cf51-41d9-aaf5-ad5420f42b6a)
+
+# Generation Options
+
+The `put` method can take an optional parameter `opts` like `put(text,opts)`.
+
+`opts` can specify the format of the input and output, like `{"in_type":"spot","out_type:"spot" }`.
+
+It behaves as follows:
+
+| in_type  | out_type | Description                                    |
+| :------- | :------- | :---------------------------------------------- |
+| spot     | spot     | A mode that incrementally sends tokens to the `put` method, and outputs generated segments each time. |
+| spot     | full     | A mode that incrementally sends tokens to the `put` method, but outputs the full sentence. |
+| full     | spot     | A mode that sends the full sentence to the `put` method at once, but outputs generated segments each time. |
+| full     | full     | A mode that sends the full sentence to the `put` method at once, and outputs the full sentence. |
+
+Notes:
+- All text strings need to be sent to the `put` method before calling the `flush` method. Especially in `full` mode, all input strings are sent at once.
+- If the output type (`out_type`) is `full`, the `flush` method must be called to obtain the final result.
+- It's important to appropriately combine the call pattern of the `put` method and the use of the `flush` method to maintain consistency in each mode.
+
+**Code Example**
+
+Specify rules like `condition = {"in_type": "full", "out_type": "full"}`, and use `condition` as an argument for `put` and `flush`.
+
+```python
+    tokf = TokFlow([("<NL>", "\n")])
+
+    condition = {"in_type": "full", "out_type": "full"}
+    prev_len = 0
+    for input_token_base in get_example_texts():
+        output_sentence = tokf.put(input_token_base, condition)
+
+        print(f"output_sentence:{output_sentence}")
+
+        if prev_len > len(output_sentence):
+            raise ValueError("Length error")
+
+        if "<NL>" in output_sentence:
+            raise Exception("Failure Must be converted str found.")
+
+        prev_len = len(output_sentence)
+
+    output_sentence = tokf.flush(condition)
+```
+
+
+# SentenceStop Class
+
+The SentenceStop class is designed to detect specific keywords and stop text generation at the point where the keyword is found. It assumes a situation where text is input one character at a time.
+
+## Main Features
+
+- **Detection of specific keywords**: Detects specific keywords within the string. The detected keywords are treated as stop strings.
+- **Stop text generation**: Stops text generation at the position of the detected stop string. Specifically, it returns the text at the point where the stop string is detected.
+- **Real-time processing**: Assumes a situation where strings are input one character at a time, enabling real-time processing.
+
+## How to use
+
+Specify the keywords to stop at initialization. After that, input one character at a time with the `put` method, and if a stop string is found, it returns the text at that point. When all inputs are finished, use the `flush` method to perform the remaining processing.
+
+
+
+
+
+# Processing
+
+## About Internal processing
+
+Tokens are sequentially read in real time.
+The token read is combined with the tokens read so far, referred to as the "token buffer".
+In this sequential process, when a pre-specified string (hereafter referred to
+as the "search target string") appears in the token buffer,
+this string is replaced with another string (hereafter referred to as the "replacement string").
+Since tokens are read sequentially, in the intermediate stage,
+a string that is unrelated to the search target string or part of the search target string accumulates
+in the token buffer. If the token buffer is composed in an order that cannot be a search target string,
+the token buffer is returned as the method's return value the moment such a determination is made.
+On the other hand, if the token buffer is composed in an order that could be a search target string,
+the return value remains an empty string until either the search target string appears or
+it is determined that it cannot be a search target string.
+In this way, by buffering until the appearance of the search target string,
+most sequential tokens can be displayed as they are, while replacement is delayed when necessary,
+enabling stream processing.
+
+# TokFlow License
+
+## Open source license
+
+The open source license has been specifically designed to enable the development of open source and personal projects using TokFlow. The open source license associated with TokFlow is the [GNU General Public License version 3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.html). 
+The GPLv3 has many terms, yet perhaps the most crucial is its 'sticky' nature when you distribute your work publicly. 
+As outlined in the [GPL FAQ](https://www.gnu.org/licenses/gpl-faq.html):
+
+> "Upon releasing a modified version of your program to the public, the GPLv3 requires you to make the modified source code available to the users of your program, under the GPLv3."
+
+Publicly releasing your project that utilises TokFlow under the GPLv3, in turn, 
+requires your project to be licensed under the GPLv3. 
+If you're comfortable with this, you're more than welcome to use TokFlow under the GPLv3, 
+without the need to acquire a commercial license.
+
+However, if you wish to include this library in your tool and distribute it under a license other than the GPLv3, 
+or if you wish to distribute it for a fee, 
+or should you want to use it for commercial purposes, 
+obtaining a commercial license will be necessary. 
+Please don't hesitate to contact us for discussion.
+
+## Commercial OEM License
+
+If you want to include TokFlow as part of a commercial product, SDK, or toolkit, 
+choose the Commercial OEM license. 
+Commercial OEM licenses are customized for each customer. Contact `riversun.org@gmail.com`
+
```

### Comparing `tokflow-1.1.0/TokFlow.egg-info/SOURCES.txt` & `tokflow-1.2.0/TokFlow.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 README.md
 setup.py
 TokFlow.egg-info/PKG-INFO
 TokFlow.egg-info/SOURCES.txt
 TokFlow.egg-info/dependency_links.txt
 TokFlow.egg-info/top_level.txt
 tests/test_refit_flow_worker.py
+tests/test_sentence_stop.py
+tests/test_sentence_stop_data.py
+tests/test_sentence_stop_spot_mode.py
 tests/test_tokflow_01_IN_spot_OUT_spot.py
 tests/test_tokflow_02_IN_full_OUT_spot.py
 tests/test_tokflow_02_data.py
 tests/test_tokflow_03_IN_spot_OUT_full.py
 tests/test_tokflow_04_IN_full_OUT_full.py
 tokflow/__init__.py
+tokflow/sentence_stop.py
 tokflow/tok_flow.py
 tokflow/tok_flow_worker.py
 tokflow.egg-info/PKG-INFO
 tokflow.egg-info/SOURCES.txt
 tokflow.egg-info/dependency_links.txt
 tokflow.egg-info/top_level.txt
```

### Comparing `tokflow-1.1.0/setup.py` & `tokflow-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tokflow",
-    version="1.1.0",
+    version="1.2.0",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="LLM utility of streaming token realtime replacement processing",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/TokFlow",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
     tests_require=["pytest"],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
+    license="GPLv3 or Commercial",
     python_requires=">=3.8",
     install_requires=[
     ]
 )
```

### Comparing `tokflow-1.1.0/tests/test_tokflow_01_IN_spot_OUT_spot.py` & `tokflow-1.2.0/tests/test_tokflow_01_IN_spot_OUT_spot.py`

 * *Files identical despite different names*

### Comparing `tokflow-1.1.0/tests/test_tokflow_02_IN_full_OUT_spot.py` & `tokflow-1.2.0/tests/test_tokflow_02_IN_full_OUT_spot.py`

 * *Files identical despite different names*

### Comparing `tokflow-1.1.0/tests/test_tokflow_02_data.py` & `tokflow-1.2.0/tests/test_tokflow_02_data.py`

 * *Files identical despite different names*

### Comparing `tokflow-1.1.0/tests/test_tokflow_03_IN_spot_OUT_full.py` & `tokflow-1.2.0/tests/test_tokflow_03_IN_spot_OUT_full.py`

 * *Files identical despite different names*

### Comparing `tokflow-1.1.0/tests/test_tokflow_04_IN_full_OUT_full.py` & `tokflow-1.2.0/tests/test_tokflow_04_IN_full_OUT_full.py`

 * *Files identical despite different names*

### Comparing `tokflow-1.1.0/tokflow/tok_flow.py` & `tokflow-1.2.0/tokflow/tok_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,20 +32,39 @@
     一方、検索対象文字列になり得る順序でトークンバッファが構成されている場合、検索対象文字列が出現するか、
     検索対象文字列になりえないと判断されるまで、戻り値は空文字となる。
     このように、検索対象文字列が出現するまでバッファリングさせることで、
     逐次トークンのほとんどはそのまま逐次表示させ、置換が必要な場合には表示を遅らせる、というストリーム処理することができる。
     """
 
     def __init__(self, replacer_list):
+        self.is_matched = False  # 現在、マッチしている状態か否か
+        self.is_possible_str_started = False  # True: 現在、どれか1つ以上のワーカーが検索対象文字列の連なる可能性のある文字列をスキャンしている場合
+
+        self.matched_worker = None  # 最後に　検索対象文字列　がマッチしたワーカー(どのワーカーがマッチして終わったのか、を取得するため)
+        self.prev_output_full_sentence = None
+        self.prev_input_full_sentence = None
+        self.not_consumed_str = None
+        self.workers = None
         self.replacer_list = replacer_list
+        self.clear()
+
+    def clear(self):
+        """
+        TokFlowの状態を初期化する
+        """
         self.workers = []
         self.not_consumed_str = ""
         self.prev_input_full_sentence = ""
         self.prev_output_full_sentence = ""
-        for from_token, to_token in replacer_list:
+
+        self.is_matched = False  # True: 現在の処理で検索対象文字列にマッチした状態
+        self.is_possible_str_started = False  # True: 現在、どれか1つ以上のワーカーが検索対象文字列の連なる可能性のある文字列をスキャンしている場合
+        self.matched_worker = None
+
+        for from_token, to_token in self.replacer_list:
             self.workers.append(TokFlowWorker(from_token, to_token))
 
     def put(self, str, opts={}):
         in_type = opts.get("in_type", "spot")
         out_type = opts.get("out_type", "spot")
 
         if in_type == "spot":
@@ -56,15 +75,15 @@
                 return self.prev_output_full_sentence
             else:
                 raise ValueError(f'unknown out_type:"{out_type}"')
         elif in_type == "full":
             if out_type == "spot":
                 return self.put_sentence(str)
             elif out_type == "full":
-                self.prev_output_full_sentence+=self.put_sentence(str)
+                self.prev_output_full_sentence += self.put_sentence(str)
                 return self.prev_output_full_sentence
             else:
                 raise ValueError(f'unknown out_type:"{out_type}"')
 
         else:
             raise ValueError(f'unknown in_type:"{in_type}"')
 
@@ -97,44 +116,55 @@
         # ある一定の数のトークンを入力すると各ワーカーのトークンバッファ（トークン列＝トークンを結合したもの）が長くなるため
         # どれか１つのワーカーで検索対象文字列が存在した場合、そのワーカーからの出力を採用する。
         # このとき、ほかのワーカーはトークンバッファ内に検索対象文字列が発見できなかったことになる。
         # 発見できたワーカーはそのターンまでのマッチングタスクとしては役目を終えるので、クリアされ、次以降のトークン列の分析に再び使われる
         # 発見できなかったワーカーも発見できないという形でマッチングタスクは終えるので同様にクリアされ、次以降のトークン列の分析に再び使われる
         for worker in self.workers:
             # ワーカーにトークンを食わせる
-            # 前ターンに仮に検索対象文字列が発見された場合は、検索対象文字列以降は未処理文字列（未消費）となるので
-            # 未消費文字列＋新たなトークンを食わせる ことになる
+            # 前ターンに仮に検索対象文字列が発見された場合は、検索対象文字列以降は未処理文字列（未消費文字列）となるので
+            # 次ターンはワーカーに 未処理文字列（未消費文字列）＋新たなトークン を食わせる
             worker.eat(self.not_consumed_str + token_str)
 
         self.not_consumed_str = ""  # 未消費の文字列をクリアする
 
         potential = False  # True:どれか1つ以上のワーカーがマッチングのポテンシャルがある状態
         matched = False  # True: どれか1つのワーカーが検索対象文字列を発見した場合
-
+        self.is_matched = False
+        self.is_possible_str_started = False  # True: どれか1つ以上のワーカーが検索対象文字列の連なる可能性のある文字列をスキャンしている場合
         ttl_num_of_not_appearred = 0
 
         pending_str = ""
 
         for worker in self.workers:
+            # 各ワーカーを１つずつ確認し、現在の検索対象文字列発見状況を確認する
+
+            if worker.is_possible_str_started:
+                # どれか１つのワーカーが、検索対象文字列に連なる文字列の処理を開始していたらフラグをたてる
+                self.is_possible_str_started = True
 
             if worker.search_str_appeared:
-                # このワーカーが担当する検索文字列の出現が確認された
-                ret_val = worker.converted
+                # - このワーカーが担当する検索文字列の出現が確認されたとき
+
+                ret_val = worker.converted  #
                 self.not_consumed_str = worker.str_to_be_process_next
-                # 　1つ正解した
-                # ほかのすべてのマッチャーをクリアすべき
+
+                # 1つのワーカー(マッチャー)で正解したので、
+                # 次からまた新しい探索が始まるため、正解したワーカーも含め現在仕掛中の他のワーカーもクリアする
                 for _worker in self.workers:
                     _worker.clear()
 
                 matched = True
+                self.matched_worker = worker
+                self.is_matched = True
 
+                break
 
-            elif worker.str_matching_started:
+            elif worker.is_possible_str_started:
                 potential = True
-                pass
+
             elif worker.confirmed_not_to_appear:
                 # 本ワーカーが現在までトークン列を分析したところ、
                 # 本ワーカー対象の検索対象文字列が発見できないことが確定した場合
 
                 # すべてのワーカーが検索対象文字列を発見できなかったのか判定するためにカウンターを+1する
                 ttl_num_of_not_appearred = ttl_num_of_not_appearred + 1
 
@@ -144,44 +174,46 @@
                 # （どのワーカーからも同じものがでてくる)
                 pending_str = worker.buffer
                 worker.clear()  # ワーカーをクリアする（現在までの処理履歴に関する変数をクリア)その後ワーカーは再利用される
 
             else:
                 pass
 
+        # end for
+
         if ttl_num_of_not_appearred == len(self.workers):
             # すべてのワーカーが検索対象文字列を発見できないことが確定した場合、
             # トークンバッファはそのまま出力すればいいので、そのまま返す
             return pending_str
 
         if not potential and not matched:
             # 検索対象文字列の出現可能性がなく、かつ、検索対象文字列の出現もしていない場合
             # ワーカーの1つから、マッチしなかった文字列を戻り値とする
-            # 度のワーカーでも同じ unmatched_str を保持しているため、便宜的に0番目を返している
+            # どのワーカーでも同じ unmatched_str を保持しているため、便宜的に0番目を返している
             ret_val = self.workers[0].unmatched_str
             pass
 
         return ret_val
 
-    def flush(self,opts={}):
+    def flush(self, opts={}):
         """
         put処理が終了したあと、未消費のトークンバッファが残っている場合があるため、
         すべてのput処理が終了したあと、本メソッドを呼出し未消費のトークンバッファを取得する
         未消費のトークンバッファが存在すればそれも出力対象とする
         """
 
         in_type = opts.get("in_type", "spot")
         out_type = opts.get("out_type", "spot")
 
         if in_type == "spot":
             if out_type == "spot":
                 final_str = self.not_consumed_str
                 pass
             elif out_type == "full":
-                final_str = self.prev_output_full_sentence+self.not_consumed_str
+                final_str = self.prev_output_full_sentence + self.not_consumed_str
                 pass
             else:
                 raise ValueError(f'unknown out_type:"{out_type}"')
         elif in_type == "full":
             if out_type == "spot":
                 final_str = self.not_consumed_str
                 pass
@@ -192,12 +224,11 @@
                 raise ValueError(f'unknown out_type:"{out_type}"')
         else:
             raise ValueError(f'unknown in_type:"{in_type}"')
 
         self.prev_output_full_sentence = ""
         self.prev_input_full_sentence = ""
 
-
         return final_str
 
     def get_workers(self):
         return self.workers
```

### Comparing `tokflow-1.1.0/tokflow/tok_flow_worker.py` & `tokflow-1.2.0/tokflow/tok_flow_worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 class TokFlowWorker:
-    
+
     def __init__(self, target_str, replace_to_str):
         self.replace_to_str = replace_to_str
         self.search_str = target_str
-        self.search_str_appeared = False
-        self.str_matching_started = False  # True:検索文字列に一致しはじめた（ポテンシャルあり）
+        self.search_str_appeared = False  # True: 検索対象文字列が発見された
+        self.is_possible_str_started = False  # True:現在、走査しているトークンが検索文字列に一致しはじめた（ポテンシャルあり）状態
         self.buffer = ""  # トークンバッファ。処理に準じてトークンが加えられていく
         self.str_to_be_process_next = ""  # 次に処理していくときの残り
         self.converted = ""  # 無事に置換成功した出力対象
         self.str_expected_to_appear = ""
         self.confirmed_not_to_appear = False  # いっかい potential True になったものがダメになった場合 dispose にする
         self.unmatched_str = ""
 
     def clear(self):
+        """
+        これまでの処理を初期化する
+        """
         self.search_str_appeared = False
-        self.str_matching_started = False
+        self.is_possible_str_started = False
         self.buffer = ""
         self.str_to_be_process_next = ""
         self.converted = ""
         self.str_expected_to_appear = ""
         self.confirmed_not_to_appear = False
         self.unmatched_str = ""
 
     def eat(self, token):
 
         self.buffer += token
 
-        if not self.str_matching_started:
+        if not self.is_possible_str_started:
             # まだ「ポテンシャルあり」となっていない場合
             # （「ポテンシャルあり」とは、現在までのトークンバッファ（与えられたトークンを順に結合したもの）が
             # 今後成長していくと、検索対象文字列を含む可能性がある状態のこと。）
 
             if self.search_str in self.buffer:
-                # トークンバッファ内に、検索対象文字列がまるごと入っていた場合
+                # - トークンバッファ内に、検索対象文字列がまるごと入っていた場合
 
                 # 最後に self.search_str が登場する以降を取得
                 part_after_search_str = self.extract_after_last_nl(self.search_str, self.buffer)
 
                 # 最後に登場する self.search_str　までを取得
                 part_before_last_search_str = self.extract_until_last_nl(self.search_str, self.buffer)
 
@@ -45,68 +48,80 @@
 
                 # 検索対象文字列以降は、次ターンのトークン処理でつかうために申し送る
                 self.str_to_be_process_next = part_after_search_str
 
                 # 検索対象文字列　出現フラグを立てる
                 self.search_str_appeared = True
 
-                self.str_matching_started = True
+                self.is_possible_str_started = True
                 return
             else:
-                # トークンバッファ内に、検索対象文字列がまるごと入ってはいない場合
+                # - トークンバッファ内に、検索対象文字列がまるごと入ってはいない場合
 
                 len_search_str = len(self.search_str)
 
                 # 検索対象文字列の一部でも入っているか
                 is_at_least_piece_of_search_str_matched = False
                 # 一部でもはいっていないかどうか1文字ずつへらしていって確認する
                 for i in range(len_search_str - 1, 0, -1):
                     left_n_size_part_of_piece = self.search_str[:i]
+
                     str_to_expect_next = self.search_str[i:]
                     # 検索対象文字列が "<NL>" を例とすると、
                     # 例えば 現在のトークンバッファが "abc<N" のような状態であるとき、
                     # つまり今後与えられるトークンをトークンバッファに加えていくと "abc<NL>" のように
                     # 検索対象文字列が出現するとき、「ポテンシャルあり」とみなす。
+                    #
                     # 本処理では、 "abc<N" のように 検索対象文字列 "<NL>" の　”かけら”（left_n_size_part_of_piece） が
                     # トークンバッファの末尾に存在しないかどうかを確認していく。
                     # ポテンシャルありとなる、トークンバッファの末尾は、 "かけら"（left_n_size_part_of_piece） を順に短くしていき確認していく。
                     # STEP1."<NL"
                     # STEP2."<N"
                     # STEP3."<"
                     if self.buffer.endswith(left_n_size_part_of_piece):
+
                         # 検索文字列のかけらがトークンバッファの末尾に存在した場合
                         # is_at_least_piece_of_search_str_matched = True #
-                        self.str_matching_started = True  # ポテンシャルあり　にする
+                        self.is_possible_str_started = True  # ポテンシャルあり　にする
 
                         # かけら　が　"<NL"　の場合は ">" に出現してほしい
                         # かけら　が "<N" の場合は、 "L>" に出現してほしい
                         # かけら　が "<" の場合は、 "NL>" に出現してほしい
                         self.str_expected_to_appear = str_to_expect_next  # 次以降に出現してほしい文字列をセットする
                         break
 
-                if not self.str_matching_started:
+                if not self.is_possible_str_started:
                     # ポテンシャルがなかった場合
                     # (トークンバッファに小さな　"かけら" すらなかった場合)
                     self.unmatched_str = self.buffer
                     self.buffer = ""
 
                     pass
 
         else:
             # ポテンシャルあり となり、検索対象文字列のマッチングが開始している場合
 
-            if self.str_expected_to_appear in self.buffer:
-                # 出現待ちになっている文字列がまるごとトークンバッファに存在した場合
+            # このアプローチだと、検索対象が「<NLL>」で、「L>」をまってるときに、バッファが<NL>のときに
+            # バッファ「<NL>」に「L>」をみつけてしまうのでNG
+            #if self.str_expected_to_appear in self.buffer:
+
+            if self.search_str in self.buffer:
+                # - 出現待ちになっている文字列がまるごとトークンバッファに存在した場合
+                #
                 # (たとえば、前回ターンのトークンバッファが "abc<" で　今回ターンのトークンバッファが "NL>" のようになったタイミング)
+
                 self.str_to_be_process_next = self.extract_after_last_nl(self.search_str,
                                                                          self.buffer)  # 最後に self.search_str が登場する以降を取得
+
                 part_before_last_search_str = self.extract_until_last_nl(self.search_str,
                                                                          self.buffer)  # 最後に登場する self.search_str　までを取得
+
                 self.converted = part_before_last_search_str.replace(self.search_str, self.replace_to_str)
                 self.search_str_appeared = True
+
                 pass
             else:
                 # 出現待ちになっている文字列がまるごとは来ていなかった場合
 
                 # たとえば、前回ターンが "abc<" で　今回ターンが "NL" のようなパターンの可能性をさぐる
                 len_search_str = len(self.str_expected_to_appear)
 
@@ -114,30 +129,32 @@
                 need_continue_to_matching = False
 
                 for i in range(len_search_str - 1, 0, -1):  # -1 してるのは length の場合はフル一致のため
 
                     # "NL>" を "NL" "N" に分解して、一部でもマッチしていないか確認する
                     part_of_waiting = self.str_expected_to_appear[:i]
 
+
                     # "NL>" を "NL" に分解したときの、残りパート ">"
                     # "NL>" を "N" に分解したときの残りパート "L>"
                     rest_of_waiting = self.str_expected_to_appear[i:]
 
                     if token.startswith(part_of_waiting):
+
                         # 文字ピースが "NL>" のように出現待ちで開始している場合
                         need_continue_to_matching = True  # 引き続きマッチングを続ける
                         self.str_expected_to_appear = rest_of_waiting
 
                 if not need_continue_to_matching:
                     # 現時点で、検索文字列との一致可能性がなくなった場合
 
                     # 今ターンまでのマッチング処理を行ったが、出現しないことが確定したので、
                     # （一旦）役目終了のフラグをたてる
                     self.confirmed_not_to_appear = True
-                    self.str_matching_started = False
+                    self.is_possible_str_started = False
 
     def extract_after_last_nl(self, target, text):
         split_text = text.rsplit(target, 1)  # '<NL>'で文字列を最後から分割し、最大分割数を1に設定
         after_last_nl = split_text[1] if len(split_text) > 1 else split_text[0]
         return after_last_nl
 
     def extract_until_last_nl(self, target_str, text):
```

