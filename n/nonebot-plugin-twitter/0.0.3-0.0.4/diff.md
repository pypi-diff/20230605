# Comparing `tmp/nonebot-plugin-twitter-0.0.3.tar.gz` & `tmp/nonebot-plugin-twitter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.0.3.tar", last modified: Mon Jun  5 07:42:27 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.0.4.tar", last modified: Mon Jun  5 11:30:46 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.0.3.tar` & `nonebot-plugin-twitter-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-05 07:42:16.613709 nonebot-plugin-twitter-0.0.3/LICENSE
--rw-r--r--   0        0        0     2777 2023-06-05 07:42:16.613709 nonebot-plugin-twitter-0.0.3/README.md
--rw-r--r--   0        0        0    14959 2023-06-05 07:42:16.613709 nonebot-plugin-twitter-0.0.3/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     1041 2023-06-05 07:42:16.613709 nonebot-plugin-twitter-0.0.3/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      646 2023-06-05 07:42:16.613709 nonebot-plugin-twitter-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2777 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/README.md
+-rw-r--r--   0        0        0    14977 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      646 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.4/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.0.3/LICENSE` & `nonebot-plugin-twitter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.3/README.md` & `nonebot-plugin-twitter-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.3/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         return MessageSegment.node_custom(user_id=user_id, nickname=name,
                                    content=Message(MessageSegment.image(f"file://{task}")))
     elif task.endswith("mp4"):
         return MessageSegment.node_custom(user_id=user_id, nickname=name,
                                           content=Message(MessageSegment.video(f"file:///{task}")))        
         
 async def get_pic(url: str) -> str:
-    path = Path() / "data" / "twitter" / "cache" /  url.split('/').pop()
+    path = Path() / "data" / "twitter" / "cache" /  f"{str(random.randint(1, 1000))}.jpg"
     path = f"{os.getcwd()}/{str(path)}"
     if config_dev.twitter_proxy:
         async with AsyncClient(proxies=f"http://{config_dev.twitter_proxy}") as client:
             res = await client.get(url)
             if res.status_code != 200:
                 raise ValueError("图片下载失败")
             with open(path,'wb') as file:
@@ -201,15 +201,15 @@
                 raise ValueError("图片下载失败")
             with open(path,'wb') as file:
                 file.write(res.read())
             
     return path
 
 async def get_video(url: str) -> str:
-    path = Path() / "data" / "twitter" / "cache" /  f"{str(random.randint(1, 100))}.mp4"
+    path = Path() / "data" / "twitter" / "cache" /  f"{str(random.randint(1, 1000))}.mp4"
     path = f"{os.getcwd()}/{str(path)}"
     if config_dev.twitter_proxy:
         async with AsyncClient(proxies=f"http://{config_dev.twitter_proxy}") as client:
             async with client.stream('GET',url,headers=header) as res:
                 if res.status_code != 200:
                     raise ValueError("视频下载失败")
                 with open(path,'wb') as file:
```

### Comparing `nonebot-plugin-twitter-0.0.3/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.3/pyproject.toml` & `nonebot-plugin-twitter-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.0.3"
+version = "0.0.4"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.0.3/PKG-INFO` & `nonebot-plugin-twitter-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.0.3
+Version: 0.0.4
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.4 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
```

