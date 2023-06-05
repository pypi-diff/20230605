# Comparing `tmp/pararamio-1.0.8.tar.gz` & `tmp/pararamio-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pararamio-1.0.8.tar", last modified: Tue Aug  3 20:13:54 2021, max compression
+gzip compressed data, was "dist/pararamio-1.0.9.tar", last modified: Wed Aug  4 10:50:10 2021, max compression
```

## Comparing `pararamio-1.0.8.tar` & `pararamio-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 20:13:54.000000 pararamio-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      627 2021-08-03 20:13:54.000000 pararamio-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1071 2021-08-03 20:13:43.000000 pararamio-1.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1007 2021-08-03 20:13:43.000000 pararamio-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio.egg-info/
--rw-r--r--   0 root         (0) root         (0)      627 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      727 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      311 2021-08-03 20:13:43.000000 pararamio-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio/
--rw-rw-rw-   0 root         (0) root         (0)     1033 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/group.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4068 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/bot.py
--rw-rw-rw-   0 root         (0) root         (0)    14990 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/chat.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    13434 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/client.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4483 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/team.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/file.py
--rw-rw-rw-   0 root         (0) root         (0)     2739 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/deferred_post.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/user.py
--rw-rw-rw-   0 root         (0) root         (0)     8009 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 20:13:54.000000 pararamio-1.0.8/pararamio/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7173 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/utils/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     7506 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/utils/requests.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2021-08-03 20:13:43.000000 pararamio-1.0.8/pararamio/utils/captcha.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-03 20:13:54.000000 pararamio-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 20:13:54.000000 pararamio-1.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)       74 2021-08-03 20:13:43.000000 pararamio-1.0.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2021-08-03 20:13:43.000000 pararamio-1.0.8/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 20:13:54.000000 pararamio-1.0.8/tests/integrations/
--rw-rw-rw-   0 root         (0) root         (0)    11088 2021-08-03 20:13:43.000000 pararamio-1.0.8/tests/integrations/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2021-08-03 20:13:43.000000 pararamio-1.0.8/tests/integrations/_base.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-03 20:13:43.000000 pararamio-1.0.8/tests/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 10:50:10.000000 pararamio-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      627 2021-08-04 10:50:10.000000 pararamio-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2021-08-04 10:49:59.000000 pararamio-1.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2021-08-04 10:49:59.000000 pararamio-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      627 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      727 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      311 2021-08-04 10:49:59.000000 pararamio-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio/
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/bot.py
+-rw-rw-rw-   0 root         (0) root         (0)    14990 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2021-08-04 10:50:09.000000 pararamio-1.0.9/pararamio/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    13434 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4483 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/team.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2739 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/deferred_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     7981 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 10:50:10.000000 pararamio-1.0.9/pararamio/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/utils/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/utils/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2021-08-04 10:49:59.000000 pararamio-1.0.9/pararamio/utils/captcha.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-04 10:50:10.000000 pararamio-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 10:50:10.000000 pararamio-1.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2021-08-04 10:49:59.000000 pararamio-1.0.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2021-08-04 10:49:59.000000 pararamio-1.0.9/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-04 10:50:10.000000 pararamio-1.0.9/tests/integrations/
+-rw-rw-rw-   0 root         (0) root         (0)    11040 2021-08-04 10:49:59.000000 pararamio-1.0.9/tests/integrations/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2021-08-04 10:49:59.000000 pararamio-1.0.9/tests/integrations/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-04 10:49:59.000000 pararamio-1.0.9/tests/integrations/__init__.py
```

### Comparing `pararamio-1.0.8/PKG-INFO` & `pararamio-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pararamio
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pararam Library
 Home-page: https://gitlab.com/pararam-public/py-pararamio
 Author: Ilya Volnistov
 Author-email: i.volnistov@gaijin.team
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `pararamio-1.0.8/LICENSE` & `pararamio-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/setup.py` & `pararamio-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio.egg-info/PKG-INFO` & `pararamio-1.0.9/pararamio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pararamio
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pararam Library
 Home-page: https://gitlab.com/pararam-public/py-pararamio
 Author: Ilya Volnistov
 Author-email: i.volnistov@gaijin.team
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `pararamio-1.0.8/pararamio.egg-info/SOURCES.txt` & `pararamio-1.0.9/pararamio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/_types.py` & `pararamio-1.0.9/pararamio/_types.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/group.py` & `pararamio-1.0.9/pararamio/group.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/exceptions.py` & `pararamio-1.0.9/pararamio/exceptions.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/bot.py` & `pararamio-1.0.9/pararamio/bot.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/chat.py` & `pararamio-1.0.9/pararamio/chat.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/client.py` & `pararamio-1.0.9/pararamio/client.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/team.py` & `pararamio-1.0.9/pararamio/team.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/file.py` & `pararamio-1.0.9/pararamio/file.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/deferred_post.py` & `pararamio-1.0.9/pararamio/deferred_post.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/user.py` & `pararamio-1.0.9/pararamio/user.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/post.py` & `pararamio-1.0.9/pararamio/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,27 +168,27 @@
 
         return map(make_post_from_re, res['data'])
 
     def get_tree(self, load_limit: int = 1000) -> 'OrderedDict[int, Post]':
         posts = {self.post_no: self}
         for post in self.rerere():
             posts[post.post_no] = post
-        first = posts[min(sorted(posts.keys()))]
+        first = posts[min(posts.keys())]
+        tree = OrderedDict(sorted(posts.items()))  # type: ignore
         load_start = first.post_no + 1
         if self.post_no - first.post_no > load_limit:
             load_start = self.post_no - load_limit
-        tree = posts
         for post in self.chat._lazy_posts_loader(*sorted([load_start, self.post_no - 1])):
             posts[post.post_no] = post
-        for no, post in sorted(posts.items(), reverse=True)[1:]:
-            if post.reply_no not in posts:
+
+        for no, post in sorted(posts.items()):
+            if post.reply_no is None or post.reply_no not in tree:
                 continue
-            if post.reply_no and post.reply_no not in tree:
-                tree[post.reply_no] = posts[post.reply_no]
-        return OrderedDict(sorted(tree.items())) # noqa
+            tree[post.post_no] = post
+        return OrderedDict(sorted(tree.items()))  # type: ignore
 
     def get_reply_to_post(self) -> Optional['Post']:
         reply_no = self.reply_no
         if reply_no is not None:
             return Post(self._chat, reply_no, load_on_key_error=self.load_on_key_error).load()
         return None
```

### Comparing `pararamio-1.0.8/pararamio/utils/authentication.py` & `pararamio-1.0.9/pararamio/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/utils/requests.py` & `pararamio-1.0.9/pararamio/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/utils/helpers.py` & `pararamio-1.0.9/pararamio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/pararamio/utils/captcha.py` & `pararamio-1.0.9/pararamio/utils/captcha.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/tests/test_utils.py` & `pararamio-1.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pararamio-1.0.8/tests/integrations/test_client.py` & `pararamio-1.0.9/tests/integrations/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,38 +196,36 @@
         with patch.object(Post, 'rerere', return_value=[
             Post(chat, post_no=96, text='post no 96', reply_no=None),
             Post(chat, post_no=99, text='post no 99', reply_no=96),
             Post(chat, post_no=100, text='post no 100', reply_no=99, meta={})
         ]):
             with patch.object(chat, '_lazy_posts_loader', return_value=iter([
                 Post(chat, post_no=96, text='post no 96', reply_no=None),
-                Post(chat, post_no=97, text='post no 97', reply_no=96),
-                Post(chat, post_no=98, text='post no 98', reply_no=97),
+                Post(chat, post_no=97, text='post no 97', reply_no=None),
+                Post(chat, post_no=98, text='post no 98', reply_no=96),
                 Post(chat, post_no=99, text='post no 99', reply_no=96),
             ])):
                 post = Post(chat, post_no=100, text='post no 100', reply_no=99, meta={})
-                self.assertListEqual([96, 97, 98, 99, 100], list(post.get_tree().keys()))
+                self.assertListEqual([96, 98, 99, 100], list(post.get_tree().keys()))
         many_fake_posts = [
             Post(chat, post_no=1, text='post no 1', reply_no=None),
             *[Post(chat, text=f'post no {i}', post_no=i, reply_no=i - 1) for i in range(2, 2000)],
             Post(chat, post_no=2000, text='post no 2000', reply_no=1999, meta={})
         ]
 
         def _load_posts_side_effect(start, end):
             return iter(many_fake_posts[start: end])
 
-        import logging
-
-        logging.basicConfig(level=logging.DEBUG)
         with patch.object(Post, 'rerere', return_value=[many_fake_posts[0], *many_fake_posts[1000:]]):
             chat._load_posts = MagicMock(side_effect=_load_posts_side_effect)
-            self.assertListEqual([many_fake_posts[0].post_no, *[p.post_no for p in many_fake_posts[1000:]]], list(many_fake_posts[-1].get_tree().keys()))
+            posts = list(many_fake_posts[-1].get_tree().keys())
+            self.assertListEqual([many_fake_posts[0].post_no, *[p.post_no for p in many_fake_posts[1000:]]], posts)
 
         with patch.object(Post, 'rerere', return_value=[]):
-            chat._load_posts = MagicMock(side_effect=lambda a,b: [])
+            chat._load_posts = MagicMock(side_effect=lambda a, b: [])
             self.assertListEqual([2000], list(many_fake_posts[-1].get_tree().keys()))
 
     def test_020_send_and_delete_message_by_email(self):
         text = 'test by mail'
         try:
             self.client.post_private_message_by_user_email(self.recipient_email + '1111', text)
             self.assertTrue(False, 'the message cannot be sent to a non-existent email')
```

### Comparing `pararamio-1.0.8/tests/integrations/_base.py` & `pararamio-1.0.9/tests/integrations/_base.py`

 * *Files identical despite different names*

