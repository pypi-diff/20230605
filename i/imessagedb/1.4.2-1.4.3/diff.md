# Comparing `tmp/imessagedb-1.4.2.tar.gz` & `tmp/imessagedb-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.4.2.tar", max compression
+gzip compressed data, was "imessagedb-1.4.3.tar", max compression
```

## Comparing `imessagedb-1.4.2.tar` & `imessagedb-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-05-30 17:28:36.645317 imessagedb-1.4.2/LICENSE
--rw-r--r--   0        0        0     9445 2023-05-30 17:28:36.645317 imessagedb-1.4.2/README.md
--rw-r--r--   0        0        0     1336 2023-05-30 17:29:09.449304 imessagedb-1.4.2/pyproject.toml
--rw-r--r--   0        0        0    13235 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8476 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3186 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2365 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/chat.py
--rw-r--r--   0        0        0     4100 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3300 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/default.ini
--rw-r--r--   0        0        0     1092 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/handle.py
--rw-r--r--   0        0        0     3760 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/handles.py
--rw-r--r--   0        0        0    30347 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/html.py
--rw-r--r--   0        0        0     5037 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/message.py
--rw-r--r--   0        0        0     6222 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/messages.py
--rw-r--r--   0        0        0     6757 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/text.py
--rw-r--r--   0        0        0      677 2023-05-30 17:28:36.657317 imessagedb-1.4.2/src/imessagedb/utils.py
--rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 imessagedb-1.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-06-05 13:37:46.357285 imessagedb-1.4.3/LICENSE
+-rw-r--r--   0        0        0     9445 2023-06-05 13:37:46.357285 imessagedb-1.4.3/README.md
+-rw-r--r--   0        0        0     1336 2023-06-05 13:38:16.286171 imessagedb-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0    13235 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3186 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2365 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     4100 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3300 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/default.ini
+-rw-r--r--   0        0        0     1092 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     3760 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    30347 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/html.py
+-rw-r--r--   0        0        0     5037 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/message.py
+-rw-r--r--   0        0        0     6222 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     6757 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/text.py
+-rw-r--r--   0        0        0      677 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/utils.py
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 imessagedb-1.4.3/PKG-INFO
```

### Comparing `imessagedb-1.4.2/LICENSE` & `imessagedb-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/README.md` & `imessagedb-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/pyproject.toml` & `imessagedb-1.4.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.4.2"
+version = "1.4.3"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.4.2/src/imessagedb/__init__.py` & `imessagedb-1.4.3/src/imessagedb/__init__.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/attachment.py` & `imessagedb-1.4.3/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/attachments.py` & `imessagedb-1.4.3/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/chat.py` & `imessagedb-1.4.3/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/chats.py` & `imessagedb-1.4.3/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/db.py` & `imessagedb-1.4.3/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/default.ini` & `imessagedb-1.4.3/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/handle.py` & `imessagedb-1.4.3/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/handles.py` & `imessagedb-1.4.3/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/html.py` & `imessagedb-1.4.3/src/imessagedb/html.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/message.py` & `imessagedb-1.4.3/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/messages.py` & `imessagedb-1.4.3/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/text.py` & `imessagedb-1.4.3/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/src/imessagedb/utils.py` & `imessagedb-1.4.3/src/imessagedb/utils.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.2/PKG-INFO` & `imessagedb-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.4.2
+Version: 1.4.3
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

