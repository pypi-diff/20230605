# Comparing `tmp/commonX-0.4.5.tar.gz` & `tmp/commonX-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.4.5.tar", last modified: Wed May 10 10:30:54 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.6.tar", last modified: Mon Jun  5 13:01:09 2023, max compression
```

## Comparing `commonX-0.4.5.tar` & `commonX-0.4.6.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/
--rw-rw-rw-   0        0        0      714 2023-05-10 10:30:54.000000 commonX-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-05-10 10:30:27.000000 commonX-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/
--rw-rw-rw-   0        0        0       86 2023-05-10 10:30:27.000000 commonX-0.4.5/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/base/
--rw-rw-rw-   0        0        0      622 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5194 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/ext/
--rw-rw-rw-   0        0        0      187 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/postman/
--rw-rw-rw-   0        0        0       87 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     4457 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4528 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/util/
--rw-rw-rw-   0        0        0      277 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     2725 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/exception_utll.py
--rw-rw-rw-   0        0        0     7244 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/file_util.py
--rw-rw-rw-   0        0        0     2921 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/json_util.py
--rw-rw-rw-   0        0        0     6928 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4616 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/
--rw-rw-rw-   0        0        0      714 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 10:30:54.000000 commonX-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-05-10 10:30:27.000000 commonX-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/
+-rw-rw-rw-   0        0        0      714 2023-06-05 13:01:09.000000 commonX-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-06-05 13:00:25.000000 commonX-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/
+-rw-rw-rw-   0        0        0       86 2023-06-05 13:00:25.000000 commonX-0.4.6/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/base/
+-rw-rw-rw-   0        0        0      622 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5194 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5045 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     4438 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     4782 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/util/
+-rw-rw-rw-   0        0        0      304 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     3273 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     2725 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/exception_utll.py
+-rw-rw-rw-   0        0        0     7244 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2961 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/image_util.py
+-rw-rw-rw-   0        0        0     2921 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/json_util.py
+-rw-rw-rw-   0        0        0     6928 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4616 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 13:01:09.000000 commonX-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-06-05 13:00:25.000000 commonX-0.4.6/setup.py
```

### Comparing `commonX-0.4.5/PKG-INFO` & `commonX-0.4.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.5
+Version: 0.4.6
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.5/common/base/__init__.py` & `commonX-0.4.6/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/entity.py` & `commonX-0.4.6/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/genor.py` & `commonX-0.4.6/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/hook.py` & `commonX-0.4.6/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/logger.py` & `commonX-0.4.6/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/mapper.py` & `commonX-0.4.6/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/multi_task.py` & `commonX-0.4.6/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/packer.py` & `commonX-0.4.6/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/base/registry.py` & `commonX-0.4.6/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/ext/cookie_parser.py` & `commonX-0.4.6/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/ext/iphone_client.py` & `commonX-0.4.6/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/ext/qq_email.py` & `commonX-0.4.6/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/postman/postman_api.py` & `commonX-0.4.6/common/postman/postman_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,24 +160,22 @@
 
 class AbstractSessionPostman(AbstractPostman):
 
     def __init__(self, kwargs: dict) -> None:
         super().__init__(kwargs)
 
         self.session = self.create_session(kwargs)
-        self.init = False
 
     def create_session(self, kwargs):
         raise NotImplementedError
 
     def __get__(self):
         return self.session.get
 
     def __post__(self):
         return self.session.post
 
-    def before_request(self, kwargs):
-        if self.init is False:
-            self.init = True
-            return super().before_request(kwargs)
+    def __getitem__(self, item):
+        return getattr(self.session, item)
 
-        return kwargs
+    def __setitem__(self, key, value):
+        setattr(self.session, key, value)
```

### Comparing `commonX-0.4.5/common/postman/postman_impl.py` & `commonX-0.4.6/common/postman/postman_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,25 +66,25 @@
     def __post__(self):
         from curl_cffi import requests
         return requests.post
 
 
 class CffiSessionPostman(AbstractSessionPostman):
 
-    def __init__(self, kwargs: dict) -> None:
-        super().__init__(kwargs)
-
     def create_session(self, kwargs):
         return self.new_cffi_session(kwargs)
 
     # noinspection PyMethodMayBeStatic
     def new_cffi_session(self, kwargs: dict):
         from curl_cffi import requests
         return requests.Session(**kwargs)
 
+    def before_request(self, kwargs):
+        return kwargs
+
 
 # help typing
 PostmanImplClazz = Union[
     Type[CffiPostman],
     Type[CffiSessionPostman],
     Type[RequestsPostman],
     Type[RequestsSessionPostman],
```

### Comparing `commonX-0.4.5/common/postman/postman_proxy.py` & `commonX-0.4.6/common/postman/postman_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,26 @@
 
     def post(self, *args, **kwargs):
         return self.postman.post(*args, **kwargs)
 
     def get_meta_data(self, key=None, dv=None) -> dict:
         return self.postman.get_meta_data(key, dv)
 
+    def __getitem__(self, item):
+        return self.postman.__getitem__(item)
+
+    def __setitem__(self, key, value):
+        self.postman.__setitem__(key, value)
+
     def copy(self):
         return self.__class__(self.postman.copy())
 
+    def get_root_postman(self):
+        return self.postman.get_root_postman()
+
 
 class FixUrlPostman(PostmanProxy):
 
     def __init__(self,
                  postman: Postman,
                  fix_url: str,
                  ):
```

### Comparing `commonX-0.4.5/common/util/args_util.py` & `commonX-0.4.6/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/assert_util.py` & `commonX-0.4.6/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/decorator_util.py` & `commonX-0.4.6/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/exception_utll.py` & `commonX-0.4.6/common/util/exception_utll.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/file_util.py` & `commonX-0.4.6/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/json_util.py` & `commonX-0.4.6/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/requests_util.py` & `commonX-0.4.6/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/sys_util.py` & `commonX-0.4.6/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/time_util.py` & `commonX-0.4.6/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/common/util/typing_util.py` & `commonX-0.4.6/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.5/commonX.egg-info/PKG-INFO` & `commonX-0.4.6/commonX.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.5
+Version: 0.4.6
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.5/commonX.egg-info/SOURCES.txt` & `commonX-0.4.6/commonX.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 common/postman/postman_proxy.py
 common/util/__init__.py
 common/util/args_util.py
 common/util/assert_util.py
 common/util/decorator_util.py
 common/util/exception_utll.py
 common/util/file_util.py
+common/util/image_util.py
 common/util/json_util.py
 common/util/requests_util.py
 common/util/sys_util.py
 common/util/time_util.py
 common/util/typing_util.py
```

### Comparing `commonX-0.4.5/setup.py` & `commonX-0.4.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.4.5'
+VERSION = '0.4.6'
 DESCRIPTION = 'python common toolkit'
 
 setup(
     name='commonX',
     version=VERSION,
     description=DESCRIPTION,
     author='hect0x7',
```

