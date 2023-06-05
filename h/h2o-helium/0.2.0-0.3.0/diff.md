# Comparing `tmp/h2o_helium-0.2.0-py3-none-any.whl.zip` & `tmp/h2o_helium-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4600 bytes, number of entries: 5
--rw-rw-r--  2.0 unx    12680 b- defN 23-May-30 06:48 h2o_helium/__init__.py
--rw-rw-r--  2.0 unx     2044 b- defN 23-May-30 06:51 h2o_helium-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-30 06:51 h2o_helium-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-30 06:51 h2o_helium-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      390 b- defN 23-May-30 06:51 h2o_helium-0.2.0.dist-info/RECORD
-5 files, 15217 bytes uncompressed, 3874 bytes compressed:  74.5%
+Zip file size: 4602 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx    12680 b- defN 23-Jun-05 11:59 h2o_helium/__init__.py
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      390 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/RECORD
+5 files, 15219 bytes uncompressed, 3876 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: h2o_helium/__init__.py
 Comment: 
 
-Filename: h2o_helium-0.2.0.dist-info/METADATA
+Filename: h2o_helium-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: h2o_helium-0.2.0.dist-info/WHEEL
+Filename: h2o_helium-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_helium-0.2.0.dist-info/top_level.txt
+Filename: h2o_helium-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_helium-0.2.0.dist-info/RECORD
+Filename: h2o_helium-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_helium/__init__.py

```diff
@@ -6,15 +6,15 @@
 from typing import Iterable, Optional, List
 from urllib.parse import urlparse
 
 import requests
 from pydantic import BaseModel
 from websockets.sync.client import connect as ws_connect, ClientConnection
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 
 class Status(str, Enum):
     Unknown = 'unknown'
     Scheduled = 'scheduled'
     Queued = 'queued'
     Running = 'running'
```

## Comparing `h2o_helium-0.2.0.dist-info/METADATA` & `h2o_helium-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-helium
-Version: 0.2.0
+Version: 0.3.0
 Summary: Client library for H2O Helium
 Author-email: Prithvi Prabhu <prithvi.prabhu@gmail.com>
 Project-URL: Source, https://github.com/h2oai/helium
 Project-URL: Issues, https://github.com/h2oai/helium/issues
 Project-URL: Documentation, https://github.com/h2oai/helium/wiki
 Keywords: information-retrieval,LLM,large-language-models,question-answering,search,semantic-search,analytical-search,lexical-search,document-search,natural-language-querying
 Classifier: Development Status :: 4 - Beta
@@ -35,17 +35,17 @@
 
 helium = Helium(address='https://helium.h2o.ai', api_key='sk-xxxxxx')
 
 # Create a new collection
 collection_id = helium.create_collection(name='Contracts', description='Paper clip supply contracts')
 
 # Upload documents
-with open('/path/to/dunder_mifflin.pdf', 'w') as f:
+with open('/path/to/dunder_mifflin.pdf', 'rb') as f:
     dunder_mifflin = helium.upload('Dunder Mifflin.pdf', f)
-with open('/path/to/wernham_hogg.pdf', 'w') as f:
+with open('/path/to/wernham_hogg.pdf', 'rb') as f:
     initech = helium.upload('Wernham Hogg.pdf', f)
 
 # Ingest documents
 helium.ingest_uploads(collection_id, [dunder_mifflin, initech])
 
 # Create a chat session
 chat_session_id = helium.create_chat_session(collection_id)
```

