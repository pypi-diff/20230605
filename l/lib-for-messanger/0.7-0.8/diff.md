# Comparing `tmp/lib_for_messanger-0.7.tar.gz` & `tmp/lib_for_messanger-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_for_messanger-0.7.tar", last modified: Thu Jun  1 19:07:46 2023, max compression
+gzip compressed data, was "lib_for_messanger-0.8.tar", last modified: Mon Jun  5 16:26:02 2023, max compression
```

## Comparing `lib_for_messanger-0.7.tar` & `lib_for_messanger-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-01 19:07:46.636707 lib_for_messanger-0.7/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-06-01 19:07:46.636707 lib_for_messanger-0.7/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.7/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-01 19:07:46.636707 lib_for_messanger-0.7/lib_for_messanger/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.7/lib_for_messanger/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1363 2023-05-31 19:41:07.000000 lib_for_messanger-0.7/lib_for_messanger/chat.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 19:15:38.000000 lib_for_messanger-0.7/lib_for_messanger/file_service.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.7/lib_for_messanger/message.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      838 2023-06-01 19:04:38.000000 lib_for_messanger-0.7/lib_for_messanger/user.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-01 19:07:46.636707 lib_for_messanger-0.7/lib_for_messanger.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-06-01 19:07:46.000000 lib_for_messanger-0.7/lib_for_messanger.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-06-01 19:07:46.000000 lib_for_messanger-0.7/lib_for_messanger.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-01 19:07:46.000000 lib_for_messanger-0.7/lib_for_messanger.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-06-01 19:07:46.000000 lib_for_messanger-0.7/lib_for_messanger.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-01 19:07:46.636707 lib_for_messanger-0.7/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      478 2023-06-01 19:04:48.000000 lib_for_messanger-0.7/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 16:26:02.008794 lib_for_messanger-0.8/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-06-05 16:26:02.004794 lib_for_messanger-0.8/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.8/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 16:26:02.004794 lib_for_messanger-0.8/lib_for_messanger/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.8/lib_for_messanger/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1429 2023-06-05 16:17:42.000000 lib_for_messanger-0.8/lib_for_messanger/chat.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 19:15:38.000000 lib_for_messanger-0.8/lib_for_messanger/file_service.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.8/lib_for_messanger/message.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      838 2023-06-01 19:04:38.000000 lib_for_messanger-0.8/lib_for_messanger/user.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 16:26:02.004794 lib_for_messanger-0.8/lib_for_messanger.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-06-05 16:26:02.000000 lib_for_messanger-0.8/lib_for_messanger.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-06-05 16:26:02.000000 lib_for_messanger-0.8/lib_for_messanger.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-05 16:26:02.000000 lib_for_messanger-0.8/lib_for_messanger.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-06-05 16:26:02.000000 lib_for_messanger-0.8/lib_for_messanger.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-05 16:26:02.008794 lib_for_messanger-0.8/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      478 2023-06-05 16:23:03.000000 lib_for_messanger-0.8/setup.py
```

### Comparing `lib_for_messanger-0.7/lib_for_messanger/chat.py` & `lib_for_messanger-0.8/lib_for_messanger/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
     def add_new_member(self, member_name):
         self.__members.append(member_name)
 
     def get_members(self):
         return self.__members
 
+    def get_messages_id(self):
+        return self.__messages_id
+
     def add_new_message_id(self, message_id):
         self.__messages_id.append(message_id)
 
     def to_json_object(self):
         return {"chat_name": self.__chat_name,
                 "chat_admin_name": self.__chat_admin_name,
                 "chat_password": self.__chat_password,
```

### Comparing `lib_for_messanger-0.7/lib_for_messanger/file_service.py` & `lib_for_messanger-0.8/lib_for_messanger/file_service.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.7/lib_for_messanger/message.py` & `lib_for_messanger-0.8/lib_for_messanger/message.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.7/lib_for_messanger/user.py` & `lib_for_messanger-0.8/lib_for_messanger/user.py`

 * *Files identical despite different names*

