# Comparing `tmp/aquarium-python-api-2.0.3.tar.gz` & `tmp/aquarium-python-api-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-2.0.3.tar", last modified: Mon Jun  5 10:12:25 2023, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.0.4.tar", last modified: Mon Jun  5 10:41:45 2023, max compression
```

## Comparing `aquarium-python-api-2.0.3.tar` & `aquarium-python-api-2.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.695484 aquarium-python-api-2.0.3/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.3/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 10:12:25.695887 aquarium-python-api-2.0.3/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.3/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.669954 aquarium-python-api-2.0.3/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.3/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)    12505 2023-06-05 10:02:50.000000 aquarium-python-api-2.0.3/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.3/aquarium/auth.py
--rw-r--r--   0 yann       (501) staff       (20)     3351 2023-06-05 10:10:06.000000 aquarium-python-api-2.0.3/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.3/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.3/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.3/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    27404 2023-06-05 10:06:41.000000 aquarium-python-api-2.0.3/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.689102 aquarium-python-api-2.0.3/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.3/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.3/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     5068 2023-06-05 10:10:16.000000 aquarium-python-api-2.0.3/aquarium/items/organisation.py
--rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.3/aquarium/items/playlist.py
--rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.3/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.3/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.3/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.3/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     4029 2023-06-05 09:29:59.000000 aquarium-python-api-2.0.3/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.0.3/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.3/aquarium/tools.py
--rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.3/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.694871 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-05 10:12:25.697665 aquarium-python-api-2.0.3/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.3/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:41:45.623232 aquarium-python-api-2.0.4/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.4/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 10:41:45.623642 aquarium-python-api-2.0.4/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.4/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:41:45.608315 aquarium-python-api-2.0.4/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.4/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    12505 2023-06-05 10:02:50.000000 aquarium-python-api-2.0.4/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.4/aquarium/auth.py
+-rw-r--r--   0 yann       (501) staff       (20)     3351 2023-06-05 10:10:06.000000 aquarium-python-api-2.0.4/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.4/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.4/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.4/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    27404 2023-06-05 10:06:41.000000 aquarium-python-api-2.0.4/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:41:45.617978 aquarium-python-api-2.0.4/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.4/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.4/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     5068 2023-06-05 10:10:16.000000 aquarium-python-api-2.0.4/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.4/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.4/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.4/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.4/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.4/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     4345 2023-06-05 10:38:49.000000 aquarium-python-api-2.0.4/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.0.4/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.4/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.4/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:41:45.622506 aquarium-python-api-2.0.4/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 10:41:45.000000 aquarium-python-api-2.0.4/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-05 10:41:45.000000 aquarium-python-api-2.0.4/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-05 10:41:45.000000 aquarium-python-api-2.0.4/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-05 10:41:45.000000 aquarium-python-api-2.0.4/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-05 10:41:45.000000 aquarium-python-api-2.0.4/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-05 10:41:45.625592 aquarium-python-api-2.0.4/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.4/setup.py
```

### Comparing `aquarium-python-api-2.0.3/LICENSE.md` & `aquarium-python-api-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/PKG-INFO` & `aquarium-python-api-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.3
+Version: 2.0.4
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.3/README.md` & `aquarium-python-api-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/__init__.py` & `aquarium-python-api-2.0.4/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/aquarium.py` & `aquarium-python-api-2.0.4/aquarium/aquarium.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/edge.py` & `aquarium-python-api-2.0.4/aquarium/edge.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/element.py` & `aquarium-python-api-2.0.4/aquarium/element.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/entity.py` & `aquarium-python-api-2.0.4/aquarium/entity.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/exceptions.py` & `aquarium-python-api-2.0.4/aquarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/item.py` & `aquarium-python-api-2.0.4/aquarium/item.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/items/asset.py` & `aquarium-python-api-2.0.4/aquarium/items/asset.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/items/organisation.py` & `aquarium-python-api-2.0.4/aquarium/items/organisation.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/items/playlist.py` & `aquarium-python-api-2.0.4/aquarium/items/playlist.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/items/project.py` & `aquarium-python-api-2.0.4/aquarium/items/project.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/items/task.py` & `aquarium-python-api-2.0.4/aquarium/items/task.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/items/template.py` & `aquarium-python-api-2.0.4/aquarium/items/template.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/items/user.py` & `aquarium-python-api-2.0.4/aquarium/items/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 
 
 class User(Item):
     """
     This class describes an User object child of Item class.
     """
 
+    def set_data_variables(self, data={}):
+        """
+        Sets the data variables of the User
+
+        :param      data:  The object item from Aquarium API
+        :type       data:  dictionary
+        """
+        super(Item, self).set_data_variables(data=data)
+        self.active = data.get('active', False)
+
     def signin(self, email='', password=''):
         """
         Sign in a user with it's email and password
 
         :param      email:     The email of the user
         :type       email:     string
         :param      password:  The password of the user
```

### Comparing `aquarium-python-api-2.0.3/aquarium/items/usergroup.py` & `aquarium-python-api-2.0.4/aquarium/items/usergroup.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/tools.py` & `aquarium-python-api-2.0.4/aquarium/tools.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium/utils.py` & `aquarium-python-api-2.0.4/aquarium/utils.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.0.4/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.3
+Version: 2.0.4
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.3/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.0.4/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.3/setup.cfg` & `aquarium-python-api-2.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.fatfish.app/dev/python/index.html
 project_urls = 
 	Documentation = https://docs.fatfish.app/dev/python/index.html
 	Source = https://github.com/fatfish-lab/aquarium-python-api
 	Aquarium = https://fatfi.sh/aquarium
-version = 2.0.3
+version = 2.0.4
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
```

