# Comparing `tmp/orbitkit-0.4.0.tar.gz` & `tmp/orbitkit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.4.0.tar", last modified: Thu May 25 06:26:04 2023, max compression
+gzip compressed data, was "dist/orbitkit-0.4.1.tar", last modified: Mon Jun  5 03:33:26 2023, max compression
```

## Comparing `orbitkit-0.4.0.tar` & `orbitkit-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-25 06:26:04.000000 orbitkit-0.4.0/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.4.0/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.4.0/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3137 2023-05-25 06:26:04.000000 orbitkit-0.4.0/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.4.0/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-25 06:26:04.000000 orbitkit-0.4.0/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2023-05-25 06:23:46.000000 orbitkit-0.4.0/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.4.0/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-25 06:26:04.000000 orbitkit-0.4.0/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.4.0/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.4.0/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-25 06:26:04.000000 orbitkit-0.4.0/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.4.0/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.4.0/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-25 06:26:04.000000 orbitkit-0.4.0/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.4.0/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.4.0/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     6115 2023-05-24 08:44:38.000000 orbitkit-0.4.0/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    13625 2023-05-24 09:10:22.000000 orbitkit-0.4.0/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-25 06:26:04.000000 orbitkit-0.4.0/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      104 2023-05-10 05:26:36.000000 orbitkit-0.4.0/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      790 2023-05-10 05:20:41.000000 orbitkit-0.4.0/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      520 2023-05-10 05:26:36.000000 orbitkit-0.4.0/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     1781 2023-05-20 01:15:42.000000 orbitkit-0.4.0/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      148 2023-05-10 05:19:04.000000 orbitkit-0.4.0/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    19087 2021-12-26 13:51:52.000000 orbitkit-0.4.0/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-25 06:26:04.000000 orbitkit-0.4.0/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3137 2023-05-25 06:26:03.000000 orbitkit-0.4.0/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)      726 2023-05-25 06:26:03.000000 orbitkit-0.4.0/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-25 06:26:03.000000 orbitkit-0.4.0/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-25 06:26:03.000000 orbitkit-0.4.0/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       89 2023-05-25 06:26:03.000000 orbitkit-0.4.0/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2023-05-25 06:26:03.000000 orbitkit-0.4.0/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2023-05-25 06:26:04.000000 orbitkit-0.4.0/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1547 2023-05-10 05:35:02.000000 orbitkit-0.4.0/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.4.1/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.4.1/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2023-06-05 03:33:26.000000 orbitkit-0.4.1/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.4.1/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2023-06-05 03:30:31.000000 orbitkit-0.4.1/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.4.1/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.4.1/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.4.1/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.4.1/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.4.1/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6115 2023-05-24 08:44:38.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13625 2023-05-24 09:10:22.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      438 2023-06-05 03:28:29.000000 orbitkit-0.4.1/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      790 2023-05-10 05:20:41.000000 orbitkit-0.4.1/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      520 2023-05-10 05:26:36.000000 orbitkit-0.4.1/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     1781 2023-05-20 01:15:42.000000 orbitkit-0.4.1/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      148 2023-05-10 05:19:04.000000 orbitkit-0.4.1/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    20634 2023-06-05 03:28:29.000000 orbitkit-0.4.1/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)      726 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       89 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2023-06-05 03:33:26.000000 orbitkit-0.4.1/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1547 2023-05-10 05:35:02.000000 orbitkit-0.4.1/setup.py
```

### Comparing `orbitkit-0.4.0/LICENSE` & `orbitkit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/PKG-INFO` & `orbitkit-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.4.0/README.md` & `orbitkit-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/id_srv/id_gen.py` & `orbitkit-0.4.1/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/lark_send/lark.py` & `orbitkit-0.4.1/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/util/common.py` & `orbitkit-0.4.1/orbitkit/util/common.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/util/util_aws.py` & `orbitkit-0.4.1/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/util/util_date.py` & `orbitkit-0.4.1/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/orbitkit/util/util_type_mapping.py` & `orbitkit-0.4.1/orbitkit/util/util_type_mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,52 @@
 import threading
+from enum import Enum
 
 '''
 Reference link: https://www.lifewire.com/file-extensions-and-mime-types-3469109
-
-json / html / htm / doc / docx / ppt / pptx / xls / xlsx / js / pdf / txt
+# Applications
+doc / docx / ppt / pptx / xls / xlsx / pdf / json / js
+# Text Files
+html / htm / txt
 '''
 
-content_file_mapping = {
+
+class ExtenCons(Enum):
+    '''
+    Useful constant variables
+    '''
+
+    EXTEN_OCTET_STREAM = 'application/octet-stream'
+    # Application
+    EXTEN_APPLI_PDF = 'application/pdf'
+    EXTEN_APPLI_JSON = 'application/json'
+    EXTEN_APPLI_JS = 'application/x-javascript'
+    EXTEN_APPLI_DOC = 'application/msword'
+    EXTEN_APPLI_DOCX = 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'
+    EXTEN_APPLI_XLS = 'application/vnd.ms-excel'
+    EXTEN_APPLI_XLSX = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
+    EXTEN_APPLI_PPT = 'application/vnd.ms-powerpoint'
+    EXTEN_APPLI_PPTX = 'application/vnd.openxmlformats-officedocument.presentationml.presentation'
+    # Text Files
+    EXTEN_TEXT_HTML = 'text/html'
+    EXTEN_TEXT_HTM = 'text/html'
+    EXTEN_TEXT_TXT = 'text/plain'
+    EXTEN_TEXT_HTML_UTF8 = 'text/html;charset=utf-8'
+    EXTEN_TEXT_HTM_UTF8 = 'text/html;charset=utf-8'
+    EXTEN_TEXT_TXT_UTF8 = 'text/plain;charset=utf-8'
+
+
+_content_file_mapping = {
+    # MIME Types: Applications
     '*': {'application': 'Binary file', 'mine': 'application/octet-stream'},
-    # Others
-    'json': {'application': 'json document', 'mine': 'application/json'},
-    'docx': {'application': 'docx document', 'mine': 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'},
-    'pptx': {'application': 'pptx document', 'mine': 'application/vnd.openxmlformats-officedocument.presentationml.presentation'},
-    'xlsx': {'application': 'xlsx document', 'mine': 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'},
     'pdf': {'application': 'pdf document', 'mine': 'application/pdf'},
-    # MIME Types: Applications
+    'json': {'application': 'json document', 'mine': 'application/json'},
     'evy': {'application': 'Corel Envoy', 'mine': 'application/envoy'},
     'doc': {'application': 'Word document', 'mine': 'application/msword'},
+    'docx': {'application': 'docx document', 'mine': 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'},
     'fif': {'application': 'fractal image file', 'mine': 'application/fractals'},
     'spl': {'application': 'Windows print spool file', 'mine': 'application/futuresplash'},
     'hta': {'application': 'HTML application', 'mine': 'application/hta'},
     'acx': {'application': 'Atari ST Program', 'mine': 'application/internet-property-stream'},
     'hqx': {'application': 'BinHex encoded file', 'mine': 'application/mac-binhex40'},
     'dot': {'application': 'Word document template', 'mine': 'application/msword'},
     'bin': {'application': 'binary disk image', 'mine': 'application/octet-stream'},
@@ -40,23 +66,25 @@
     'rtf': {'application': 'rich text format file', 'mine': 'application/rtf'},
     'setpay': {'application': 'set payment initiation', 'mine': 'application/set-payment-initiation'},
     'setreg': {'application': 'set registration initiation', 'mine': 'application/set-registration-initiation'},
     'xla': {'application': 'Excel Add-in file', 'mine': 'application/vnd.ms-excel'},
     'xlc': {'application': 'Excel chart', 'mine': 'application/vnd.ms-excel'},
     'xlm': {'application': 'Excel macro', 'mine': 'application/vnd.ms-excel'},
     'xls': {'application': 'Excel spreadsheet', 'mine': 'application/vnd.ms-excel'},
+    'xlsx': {'application': 'xlsx document', 'mine': 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'},
     'xlt': {'application': 'Excel template', 'mine': 'application/vnd.ms-excel'},
     'xlw': {'application': 'Excel worspace', 'mine': 'application/vnd.ms-excel'},
     'msg': {'application': 'Outlook mail message', 'mine': 'application/vnd.ms-outlook'},
     'sst': {'application': 'serialized certificate store file', 'mine': 'application/vnd.ms-pkicertstore'},
     'cat': {'application': 'Windows catalog file', 'mine': 'application/vnd.ms-pkiseccat'},
     'stl': {'application': 'stereolithography file', 'mine': 'application/vnd.ms-pkistl'},
     'pot': {'application': 'PowerPoint template', 'mine': 'application/vnd.ms-powerpoint'},
     'pps': {'application': 'PowerPoint slide show', 'mine': 'application/vnd.ms-powerpoint'},
     'ppt': {'application': 'PowerPoint presentation', 'mine': 'application/vnd.ms-powerpoint'},
+    'pptx': {'application': 'pptx document', 'mine': 'application/vnd.openxmlformats-officedocument.presentationml.presentation'},
     'mpp': {'application': 'Microsoft Project file', 'mine': 'application/vnd.ms-project'},
     'wcm': {'application': 'WordPerfect macro', 'mine': 'application/vnd.ms-works'},
     'wdb': {'application': 'Microsoft Works database', 'mine': 'application/vnd.ms-works'},
     'wks': {'application': 'Microsoft Works spreadsheet', 'mine': 'application/vnd.ms-works'},
     'wps': {'application': 'Microsoft Works word processsor document', 'mine': 'application/vnd.ms-works'},
     'hlp': {'application': 'Windows help file', 'mine': 'application/winhlp'},
     'bcpio': {'application': 'binary CPIO archive', 'mine': 'application/x-bcpio'},
@@ -213,38 +241,38 @@
 }
 
 
 def get_content_type_v1(extension):
     current_type = 'application/octet-stream'
 
     try:
-        current_type = content_file_mapping[extension]['mine']
+        current_type = _content_file_mapping[extension]['mine']
     except Exception as e:
         pass
 
     return current_type
 
 
-class SingletonType(type):
+class _SingletonType(type):
     _instance_lock = threading.Lock()
 
     def __call__(cls, *args, **kwargs):
         if not hasattr(cls, "_instance"):
-            with SingletonType._instance_lock:
+            with _SingletonType._instance_lock:
                 if not hasattr(cls, "_instance"):
-                    cls._instance = super(SingletonType, cls).__call__(*args, **kwargs)
+                    cls._instance = super(_SingletonType, cls).__call__(*args, **kwargs)
         return cls._instance
 
 
-class SwitchContentFileType(metaclass=SingletonType):
+class _SwitchContentFileType(metaclass=_SingletonType):
     def __init__(self):
         self.content2file_type_mapping = {}
         self.file2content_type_mapping = {}
         # To load all mapping data
-        for key, value in content_file_mapping.items():
+        for key, value in _content_file_mapping.items():
             # print(key, value['mine'])
             self.file2content_type_mapping[key] = value['mine']
             if value['mine'] in self.content2file_type_mapping:
                 self.content2file_type_mapping[value['mine']].append(key)
             else:
                 self.content2file_type_mapping[value['mine']] = [key]
 
@@ -262,20 +290,31 @@
             current_type = self.file2content_type_mapping[str(file_type).strip().lower()]
         except Exception as e:
             pass
         return current_type
 
 
 def content2file_type(content_type):
-    switch_content_file_type = SwitchContentFileType()
+    switch_content_file_type = _SwitchContentFileType()
     return switch_content_file_type.content2file_type(content_type)
 
 
 def file2content_type(file_type):
-    switch_content_file_type = SwitchContentFileType()
+    switch_content_file_type = _SwitchContentFileType()
     return switch_content_file_type.file2content_type(file_type)
 
 
-if __name__ == '__main__':
-    # print(get_content_type_v1('json'))
-    print(content2file_type(content_type='application/octet-streamxxx'))
-    print(file2content_type(file_type='json sdsd'))
+# -------------------------------------------------------------------------------------------------------------
+# Below are the recommended methods
+# -------------------------------------------------------------------------------------------------------------
+
+def get_content_type_4_filename(filename: str, text_with_utf8=False):
+    # If no '.' in filename then get the full filename instead.
+    file_extension = filename.split('.')[-1]
+
+    try:
+        extension = _content_file_mapping[file_extension.strip().lower()]['mine']
+        if text_with_utf8 and extension.startswith('text/'):
+            extension += ';charset=utf-8'
+        return extension
+    except:
+        return 'application/octet-stream'
```

### Comparing `orbitkit-0.4.0/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.4.1/orbitkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.4.0/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.4.1/orbitkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.0/setup.py` & `orbitkit-0.4.1/setup.py`

 * *Files identical despite different names*

