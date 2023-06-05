# Comparing `tmp/jmcomic-2.0.3.tar.gz` & `tmp/jmcomic-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-6nshgqpf/jmcomic-2.0.3.tar", last modified: Thu Jun  1 06:55:02 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-1esw4jd9/jmcomic-2.0.4.tar", last modified: Mon Jun  5 08:06:15 2023, max compression
```

## Comparing `jmcomic-2.0.3.tar` & `jmcomic-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 06:54:50.000000 jmcomic-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-01 06:55:02.000000 jmcomic-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-01 06:54:50.000000 jmcomic-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 06:55:02.000000 jmcomic-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 06:54:50.000000 jmcomic-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-05 08:06:06.000000 jmcomic-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-05 08:06:15.000000 jmcomic-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-05 08:06:06.000000 jmcomic-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 08:06:15.000000 jmcomic-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-05 08:06:06.000000 jmcomic-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.0.3/LICENSE` & `jmcomic-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/PKG-INFO` & `jmcomic-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.0.3/README.md` & `jmcomic-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/setup.py` & `jmcomic-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/src/jmcomic/api.py` & `jmcomic-2.0.4/src/jmcomic/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,18 @@
         return download_album_batch(jm_album_id, option)
 
     option, jm_client = build_client(option)
     album: JmAlbumDetail = jm_client.get_album_detail(jm_album_id)
 
     jm_debug('album',
              f'本子获取成功: [{album.id}], '
-             f'标题: [{album.title}], '
              f'作者: [{album.author}], '
-             f'章节数: [{len(album)}]')
+             f'章节数: [{len(album)}]'
+             f'标题: [{album.title}], '
+             )
 
     def download_photo(photo: JmPhotoDetail,
                        debug_topic='photo',
                        ):
         jm_client.ensure_photo_can_use(photo)
 
         jm_debug(debug_topic,
@@ -88,31 +89,31 @@
     use_cache = option.download_cache
     decode_image = option.download_image_decode
     jm_client.ensure_photo_can_use(photo_detail)
 
     # 下载每个图片的函数
     def download_image(index, image: JmImageDetail, debug_topic='image'):
         img_save_path = option.decide_image_filepath(photo_detail, index)
+        debug_tag = f'{image.aid}/{image.filename} [{index + 1}/{len(photo_detail)}]'
 
         # 已下载过，缓存命中
         if use_cache is True and file_exists(img_save_path):
             jm_debug(debug_topic,
-                     f'图片已存在: {image.aid}[{image.filename}] → {img_save_path}')
+                     f'图片已存在: {debug_tag} ← [{img_save_path}]')
             return
 
         # 开始下载
         jm_client.download_by_image_detail(
             image,
             img_save_path,
             decode_image=decode_image,
         )
 
         jm_debug(debug_topic,
-                 f'图片下载完成: {image.aid}/{image.filename}, '
-                 f'[{image.img_url}] → [{img_save_path}]')
+                 f'图片下载完成: {debug_tag}, [{image.img_url}] → [{img_save_path}]')
 
     length = len(photo_detail)
     # 根据图片数，决定下载策略
     if length <= option.download_threading_batch_count:
         # 如果图片数小的话，直接使用多线程下载，一张图一个线程。
         multi_thread_launcher(
             iter_objs=enumerate(photo_detail),
```

### Comparing `jmcomic-2.0.3/src/jmcomic/jm_client_impl.py` & `jmcomic-2.0.4/src/jmcomic/jm_client_impl.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/src/jmcomic/jm_client_interface.py` & `jmcomic-2.0.4/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/src/jmcomic/jm_config.py` & `jmcomic-2.0.4/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/src/jmcomic/jm_entity.py` & `jmcomic-2.0.4/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/src/jmcomic/jm_option.py` & `jmcomic-2.0.4/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.4/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.3/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.4/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

