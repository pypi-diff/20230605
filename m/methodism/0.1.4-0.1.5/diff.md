# Comparing `tmp/methodism-0.1.4.tar.gz` & `tmp/methodism-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.1.4.tar", last modified: Tue May 30 07:54:23 2023, max compression
+gzip compressed data, was "methodism-0.1.5.tar", last modified: Mon Jun  5 09:22:43 2023, max compression
```

## Comparing `methodism-0.1.4.tar` & `methodism-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:54:23.194344 methodism-0.1.4/
--rw-rw-rw-   0        0        0     4356 2023-05-30 07:54:23.194344 methodism-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3874 2023-05-30 07:51:57.000000 methodism-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:54:23.194344 methodism-0.1.4/methodism/
--rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.4/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.4/methodism/costumizing.py
--rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.4/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.4/methodism/error_messages.py
--rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.4/methodism/helper.py
--rw-rw-rw-   0        0        0     6906 2023-05-30 07:48:34.000000 methodism-0.1.4/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:54:23.194344 methodism-0.1.4/methodism.egg-info/
--rw-rw-rw-   0        0        0     4356 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-05-30 07:52:09.000000 methodism-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-05-30 07:54:23.210244 methodism-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 09:22:43.576184 methodism-0.1.5/
+-rw-rw-rw-   0        0        0     4537 2023-06-05 09:22:43.576184 methodism-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4055 2023-06-05 09:21:58.000000 methodism-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 09:22:43.556042 methodism-0.1.5/methodism/
+-rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.5/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.5/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.5/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.5/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.5/methodism/helper.py
+-rw-rw-rw-   0        0        0     6982 2023-06-05 09:21:58.000000 methodism-0.1.5/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:22:43.576184 methodism-0.1.5/methodism.egg-info/
+-rw-rw-rw-   0        0        0     4537 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-06-05 09:21:58.000000 methodism-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-06-05 09:22:43.585229 methodism-0.1.5/setup.cfg
```

### Comparing `methodism-0.1.4/PKG-INFO` & `methodism-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.4
+Version: 0.1.5
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -107,14 +107,20 @@
 ### funksiya taxmianan shunaqa yozilishi shart!
 ```python
 def funk(request, params):
     return "select colums from your_table", False
 # sql zaprosga istalgancha uzunlik mumkin, funk 2ta qiymat strda->sql va ikkinchisi Bool typiga ega bo'lishi kerak
 # True -> agar natija bitta bo'lsa
 # False -> agar natija bittadan ko'p bo'lsa
+
+# AGARDA XATOLIK QAYTARMOQCHI BO'LINSA
+
+def funk(request, params):
+    return {"error": "xatolik"}  # xatolikni chiqarish uchun list yoki dict formatlaridan foydalananing!!
+
 ```
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
```

### Comparing `methodism-0.1.4/README.md` & `methodism-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,20 @@
 ### funksiya taxmianan shunaqa yozilishi shart!
 ```python
 def funk(request, params):
     return "select colums from your_table", False
 # sql zaprosga istalgancha uzunlik mumkin, funk 2ta qiymat strda->sql va ikkinchisi Bool typiga ega bo'lishi kerak
 # True -> agar natija bitta bo'lsa
 # False -> agar natija bittadan ko'p bo'lsa
+
+# AGARDA XATOLIK QAYTARMOQCHI BO'LINSA
+
+def funk(request, params):
+    return {"error": "xatolik"}  # xatolikni chiqarish uchun list yoki dict formatlaridan foydalananing!!
+
 ```
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
```

### Comparing `methodism-0.1.4/methodism/costumizing.py` & `methodism-0.1.5/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.4/methodism/decors.py` & `methodism-0.1.5/methodism/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.4/methodism/error_messages.py` & `methodism-0.1.5/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.4/methodism/helper.py` & `methodism-0.1.5/methodism/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.4/methodism/main.py` & `methodism-0.1.5/methodism/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
                 # return "sql zapros"
                 return "select colums from your_table", True  # True-returns one, False-returns many
 
 
         in methodism your_funk == your.funk
 
         DIQQAT !!!  BearerAuth yoki TokenAuthentication classlaridan foydalanish mumkin emas!!!
+
+
         """
 
     file = "__main__"
     token_key = "Bearer"
     auth_headers = 'Authorization'
     token_class = Token
     not_auth_methods = []  # def hello_world() => hello.world
@@ -130,14 +132,16 @@
             return Response(custom_response(False, method=method, message=MESSAGE['UndefinedError'],
                                             data=exception_data(e)))
         funk = map(funk, [requests], [params])
 
         # sql code larini ishlatish uchun!
         try:
             sql = list(funk)[0]
+            if sql is not tuple:
+                return Response(sql)
             with closing(connection.cursor()) as cursor:
                 try:
                     cursor.execute(sql[0])
                     result = dictfetchone(cursor) if sql[1] else dictfetchall(cursor)
                     response = Response(custom_response(True, data=result))
                 except Exception as e:
                     response = Response(custom_response(False, method=method, message=MESSAGE['UndefinedError'],
```

### Comparing `methodism-0.1.4/methodism.egg-info/PKG-INFO` & `methodism-0.1.5/methodism.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.4
+Version: 0.1.5
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -107,14 +107,20 @@
 ### funksiya taxmianan shunaqa yozilishi shart!
 ```python
 def funk(request, params):
     return "select colums from your_table", False
 # sql zaprosga istalgancha uzunlik mumkin, funk 2ta qiymat strda->sql va ikkinchisi Bool typiga ega bo'lishi kerak
 # True -> agar natija bitta bo'lsa
 # False -> agar natija bittadan ko'p bo'lsa
+
+# AGARDA XATOLIK QAYTARMOQCHI BO'LINSA
+
+def funk(request, params):
+    return {"error": "xatolik"}  # xatolikni chiqarish uchun list yoki dict formatlaridan foydalananing!!
+
 ```
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
```

### Comparing `methodism-0.1.4/pyproject.toml` & `methodism-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.1.4/setup.cfg` & `methodism-0.1.5/setup.cfg`

 * *Files identical despite different names*

