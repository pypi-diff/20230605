# Comparing `tmp/commonX-0.4.6.tar.gz` & `tmp/commonX-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.4.6.tar", last modified: Mon Jun  5 13:01:09 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.7.tar", last modified: Mon Jun  5 14:10:45 2023, max compression
```

## Comparing `commonX-0.4.6.tar` & `commonX-0.4.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/
--rw-rw-rw-   0        0        0      714 2023-06-05 13:01:09.000000 commonX-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-06-05 13:00:25.000000 commonX-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/
--rw-rw-rw-   0        0        0       86 2023-06-05 13:00:25.000000 commonX-0.4.6/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/base/
--rw-rw-rw-   0        0        0      622 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5194 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-06-05 13:00:25.000000 commonX-0.4.6/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/ext/
--rw-rw-rw-   0        0        0      187 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-06-05 13:00:25.000000 commonX-0.4.6/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/postman/
--rw-rw-rw-   0        0        0       87 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5045 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     4438 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4782 2023-06-05 13:00:25.000000 commonX-0.4.6/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/common/util/
--rw-rw-rw-   0        0        0      304 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     2725 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/exception_utll.py
--rw-rw-rw-   0        0        0     7244 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/file_util.py
--rw-rw-rw-   0        0        0     2961 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/image_util.py
--rw-rw-rw-   0        0        0     2921 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/json_util.py
--rw-rw-rw-   0        0        0     6928 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4616 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-06-05 13:00:25.000000 commonX-0.4.6/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/
--rw-rw-rw-   0        0        0      714 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 13:01:09.000000 commonX-0.4.6/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 13:01:09.000000 commonX-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-06-05 13:00:25.000000 commonX-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:10:45.000000 commonX-0.4.7/
+-rw-rw-rw-   0        0        0      714 2023-06-05 14:10:45.000000 commonX-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-06-05 14:09:40.000000 commonX-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/
+-rw-rw-rw-   0        0        0       86 2023-06-05 14:09:40.000000 commonX-0.4.7/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/base/
+-rw-rw-rw-   0        0        0      622 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5194 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5045 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     4438 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     4782 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:10:45.000000 commonX-0.4.7/common/util/
+-rw-rw-rw-   0        0        0      304 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     3273 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     2725 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/exception_utll.py
+-rw-rw-rw-   0        0        0     7244 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2935 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/image_util.py
+-rw-rw-rw-   0        0        0     2921 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/json_util.py
+-rw-rw-rw-   0        0        0     6928 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4616 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 14:10:45.000000 commonX-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-06-05 14:09:40.000000 commonX-0.4.7/setup.py
```

### Comparing `commonX-0.4.6/PKG-INFO` & `commonX-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.6
+Version: 0.4.7
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.6/common/base/__init__.py` & `commonX-0.4.7/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/entity.py` & `commonX-0.4.7/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/genor.py` & `commonX-0.4.7/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/hook.py` & `commonX-0.4.7/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/logger.py` & `commonX-0.4.7/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/mapper.py` & `commonX-0.4.7/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/multi_task.py` & `commonX-0.4.7/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/packer.py` & `commonX-0.4.7/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/base/registry.py` & `commonX-0.4.7/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/ext/cookie_parser.py` & `commonX-0.4.7/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/ext/iphone_client.py` & `commonX-0.4.7/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/ext/qq_email.py` & `commonX-0.4.7/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/postman/postman_api.py` & `commonX-0.4.7/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/postman/postman_impl.py` & `commonX-0.4.7/common/postman/postman_impl.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/postman/postman_proxy.py` & `commonX-0.4.7/common/postman/postman_proxy.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/args_util.py` & `commonX-0.4.7/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/assert_util.py` & `commonX-0.4.7/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/decorator_util.py` & `commonX-0.4.7/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/exception_utll.py` & `commonX-0.4.7/common/util/exception_utll.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/file_util.py` & `commonX-0.4.7/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/image_util.py` & `commonX-0.4.7/common/util/image_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import imghdr
 import os
 
 from PIL import Image
 
 
 def merge_images(folder_path, limit=None, delete_org_file=True, suffix='.webp'):
     # 获取文件夹名称
@@ -61,24 +60,22 @@
         print(f'保存: {save_path}')
 
     if delete_org_file is True:
         for f in webp_files:
             os.remove(os.path.join(folder_path, f))
 
 
-def convert_images_to_jpg(folder_path):
-    # 遍历文件夹中的所有文件
-    for filename in os.listdir(folder_path):
-        # 获取文件路径
-        file_path = os.path.join(folder_path, filename)
-        # 判断是否为图片文件，并且不是jpg格式
-        if os.path.isfile(file_path) and \
-                imghdr.what(file_path) and \
-                not filename.lower().endswith('.jpg'):
-            # 打开图片文件并转换为JPG格式
-            with Image.open(file_path) as im:
-                new_filename = os.path.splitext(filename)[0] + '.jpg'
-                new_file_path = os.path.join(folder_path, new_filename)
-                im.convert('RGB').save(new_file_path)
-
-                # 删除原始图片文件
-                os.remove(file_path)
+def convert_images_to_jpg(folder_path, delete_org_file=True):
+    for root, dirs, files in os.walk(folder_path):
+        for filename in files:
+            # 检查文件扩展名是否为图片格式
+            if filename.lower().endswith(('.png', '.bmp', '.gif', '.jpeg', '.ppm', '.tiff', 'webp')):
+                file_path = os.path.join(root, filename)
+                # 打开图片并转换为JPG格式
+                with Image.open(file_path) as img:
+                    new_file_path = os.path.splitext(file_path)[0] + '.jpg'
+                    img.convert('RGB').save(new_file_path)
+
+                if delete_org_file is True:
+                    # 删除原始文件
+                    os.remove(file_path)
+                print(f'{file_path} → {new_file_path}')
```

### Comparing `commonX-0.4.6/common/util/json_util.py` & `commonX-0.4.7/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/requests_util.py` & `commonX-0.4.7/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/sys_util.py` & `commonX-0.4.7/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/time_util.py` & `commonX-0.4.7/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/common/util/typing_util.py` & `commonX-0.4.7/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/commonX.egg-info/PKG-INFO` & `commonX-0.4.7/commonX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.6
+Version: 0.4.7
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.6/commonX.egg-info/SOURCES.txt` & `commonX-0.4.7/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.4.6/setup.py` & `commonX-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.4.6'
+VERSION = '0.4.7'
 DESCRIPTION = 'python common toolkit'
 
 setup(
     name='commonX',
     version=VERSION,
     description=DESCRIPTION,
     author='hect0x7',
```

