# Comparing `tmp/chatai-streamer-0.0.1.tar.gz` & `tmp/chatai-streamer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-streamer-0.0.1.tar", last modified: Sun Jun  4 11:32:27 2023, max compression
+gzip compressed data, was "chatai-streamer-0.0.2.tar", last modified: Mon Jun  5 16:17:57 2023, max compression
```

## Comparing `chatai-streamer-0.0.1.tar` & `chatai-streamer-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-04 11:32:27.270921 chatai-streamer-0.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-0.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-04 11:32:27.270921 chatai-streamer-0.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    12766 2023-06-04 11:18:16.000000 chatai-streamer-0.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-04 11:32:27.270921 chatai-streamer-0.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-04 11:18:16.000000 chatai-streamer-0.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-04 11:32:27.270921 chatai-streamer-0.0.1/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      929 2023-06-04 11:18:16.000000 chatai-streamer-0.0.1/src/ChatAIStreamer.py
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4560 2023-06-04 11:18:16.000000 chatai-streamer-0.0.1/src/GttsAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-04 11:18:16.000000 chatai-streamer-0.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-04 11:32:27.270921 chatai-streamer-0.0.1/src/chatai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-04 11:32:27.000000 chatai-streamer-0.0.1/src/chatai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-04 11:32:27.000000 chatai-streamer-0.0.1/src/chatai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-04 11:32:27.000000 chatai-streamer-0.0.1/src/chatai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-04 11:32:27.000000 chatai-streamer-0.0.1/src/chatai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      134 2023-06-04 11:32:27.000000 chatai-streamer-0.0.1/src/chatai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-04 11:32:27.000000 chatai-streamer-0.0.1/src/chatai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-0.0.2/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    12612 2023-06-04 13:03:07.000000 chatai-streamer-0.0.2/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-05 16:15:43.000000 chatai-streamer-0.0.2/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/src/
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      929 2023-06-04 12:04:18.000000 chatai-streamer-0.0.2/src/ChatAIStreamer.py
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4560 2023-06-05 04:09:57.000000 chatai-streamer-0.0.2/src/GttsAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-05 16:15:43.000000 chatai-streamer-0.0.2/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-05 16:15:43.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/top_level.txt
```

### Comparing `chatai-streamer-0.0.1/LICENSE` & `chatai-streamer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-streamer-0.0.1/PKG-INFO` & `chatai-streamer-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 0.0.1
+Version: 0.0.2
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-streamer-0.0.1/README.md` & `chatai-streamer-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,16 @@
 
   ```usage
   $ python3 ./sample.py VIDEO-ID OpenAI-API-KEY
   ```
 - Output of the sample<br>
   The outputs of the voices and the right window are provided by this sample.<br>
   Left outputs are also available by ChatAIStreamer.
-  <iframe width="560" height="315" src="https://www.youtube.com/embed/sesl9VZHDA8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
+  
+  [![GttsAIStreamer sample](ReadMeParts/ChatAIStreamer.png)](https://www.youtube.com/embed/sesl9VZHDA8)
 
 ## Arguments of Constructor
 - ChatAIStreamer object can be configured with following params given to constructor.
 
   ### steamParams
     | name | description | default |
     |------|------------|---------|
@@ -279,20 +280,20 @@
 ### disconnect()
 - Request to terminate YouTube Chat polling, ChatGPT conversation, voice generation and calling user callbacks.
 - Internal process will be terminated soon after.
 - No arguments required, nothing returns.
 
 And other [threading.Thread](https://docs.python.org/3/library/threading.html) public pethods are available.<br><br>
 
-## Classess
+## Classes
 ### voiceGenerator
 -  voiceGenerator class has hollowing method.
     | name | description | default |
     |------|------------|---------|
-    | generate | virtual method to generate voice. String of text is given. Modified text and generated voice shoud be returended by this method. The type of modified text shoud be string. No restriction exist for voice type. | - |
+    | generate | virtual method to generate voice. String of text is given. Modified text and generated voice shoud be returended by this method. The type of modified text shoud be string. No restriction exists for voice type. | - |
 
 ## Callbacks
 ### get_item_cb
 - Callback for getting YouTube chat items.
 - You can implement several processes in it.
 - YouTube chat item is thrown as an argument.
 - It's not be assumed that any values are returned.
```

### Comparing `chatai-streamer-0.0.1/setup.py` & `chatai-streamer-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-streamer",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     description="ChatGPT answer aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-streamer-0.0.1/src/ChatAIStreamer.py` & `chatai-streamer-0.0.2/src/ChatAIStreamer.py`

 * *Files identical despite different names*

### Comparing `chatai-streamer-0.0.1/src/GttsAIStreamer.py` & `chatai-streamer-0.0.2/src/GttsAIStreamer.py`

 * *Files identical despite different names*

### Comparing `chatai-streamer-0.0.1/src/chatai_streamer.egg-info/PKG-INFO` & `chatai-streamer-0.0.2/src/chatai_streamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 0.0.1
+Version: 0.0.2
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

