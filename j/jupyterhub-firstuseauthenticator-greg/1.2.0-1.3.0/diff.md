# Comparing `tmp/jupyterhub-firstuseauthenticator-greg-1.2.0.tar.gz` & `tmp/jupyterhub-firstuseauthenticator-greg-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-firstuseauthenticator-greg-1.2.0.tar", last modified: Mon Jun  5 18:14:36 2023, max compression
+gzip compressed data, was "jupyterhub-firstuseauthenticator-greg-1.3.0.tar", last modified: Mon Jun  5 18:21:26 2023, max compression
```

## Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0.tar` & `jupyterhub-firstuseauthenticator-greg-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 18:14:36.482142 jupyterhub-firstuseauthenticator-greg-1.2.0/
--rw-rw-rw-   0        0        0     1528 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3806 2023-06-05 18:14:36.482142 jupyterhub-firstuseauthenticator-greg-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 18:14:36.475638 jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/
--rw-rw-rw-   0        0        0      341 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/__init__.py
--rw-rw-rw-   0        0        0      385 2023-06-05 18:10:50.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/_version.py
--rw-rw-rw-   0        0        0    14151 2023-06-05 18:07:49.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/firstuseauthenticator.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:14:36.476637 jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/templates/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/templates/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/templates/reset.html
-drwxrwxrwx   0        0        0        0 2023-06-05 18:14:36.481141 jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/
--rw-rw-rw-   0        0        0     3806 2023-06-05 18:14:36.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-06-05 18:14:36.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 18:14:36.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-05 18:14:36.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-05 18:14:36.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 18:14:36.482142 jupyterhub-firstuseauthenticator-greg-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      919 2023-06-05 18:13:53.000000 jupyterhub-firstuseauthenticator-greg-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:21:26.488842 jupyterhub-firstuseauthenticator-greg-1.3.0/
+-rw-rw-rw-   0        0        0     1528 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3806 2023-06-05 18:21:26.488842 jupyterhub-firstuseauthenticator-greg-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3348 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 18:21:26.479335 jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/
+-rw-rw-rw-   0        0        0      341 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-06-05 18:10:50.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/_version.py
+-rw-rw-rw-   0        0        0    14276 2023-06-05 18:20:15.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/firstuseauthenticator.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:21:26.480335 jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/templates/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/templates/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-05 17:40:53.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/templates/reset.html
+drwxrwxrwx   0        0        0        0 2023-06-05 18:21:26.488842 jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/
+-rw-rw-rw-   0        0        0     3806 2023-06-05 18:21:26.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-06-05 18:21:26.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 18:21:26.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-05 18:21:26.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-05 18:21:26.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 18:21:26.489842 jupyterhub-firstuseauthenticator-greg-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      919 2023-06-05 18:21:07.000000 jupyterhub-firstuseauthenticator-greg-1.3.0/setup.py
```

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/LICENSE` & `jupyterhub-firstuseauthenticator-greg-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/PKG-INFO` & `jupyterhub-firstuseauthenticator-greg-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-firstuseauthenticator-greg
-Version: 1.2.0
+Version: 1.3.0
 Summary: JupyterHub Authenticator that lets users set passwords on first use, Greg style
 Home-page: https://github.com/gahogg/firstuseauthenticator
 Author: Yuvi Panda, Project Jupyter Contributors
 Author-email: greg.hogg1@outlook.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/README.md` & `jupyterhub-firstuseauthenticator-greg-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/firstuseauthenticator.py` & `jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/firstuseauthenticator.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,18 +295,16 @@
         if any((char in name) for char in invalid_chars):
             return False
         return super().validate_username(name)
 
     async def authenticate(self, handler, data):
         print('Called 2!!!')
 
-        # Check the authorization header or any other desired criteria
-        authorization_header = handler.request.headers.get("Authorization")
-        if authorization_header != "123":
-            return None
+        
+        
 
         username = self.normalize_username(data["username"])
         password = data["password"]
 
         if not self.create_users:
             if not self._user_exists(username):
                 return None
@@ -315,14 +313,20 @@
             stored_pw = db.get(username.encode("utf8"), None)
 
             if stored_pw is not None:
                 # for existing passwords: ensure password hash match
                 if bcrypt.hashpw(password.encode("utf8"), stored_pw) != stored_pw:
                     return None
             else:
+                # Check the authorization header or any other desired criteria
+                authorization_header = handler.request.headers.get("Authorization")
+                print('Hopefully because first time')
+                if authorization_header != "123":
+                    return None
+                
                 # for new users: ensure password validity and store password hash
                 if not self._validate_password(password):
                     handler.custom_login_error = (
                         'Password too short! Please choose a password at least %d characters long.'
                         % self.min_password_length
                     )
                     self.log.error(handler.custom_login_error)
```

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/firstuseauthenticator/templates/reset.html` & `jupyterhub-firstuseauthenticator-greg-1.3.0/firstuseauthenticator/templates/reset.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/PKG-INFO` & `jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-firstuseauthenticator-greg
-Version: 1.2.0
+Version: 1.3.0
 Summary: JupyterHub Authenticator that lets users set passwords on first use, Greg style
 Home-page: https://github.com/gahogg/firstuseauthenticator
 Author: Yuvi Panda, Project Jupyter Contributors
 Author-email: greg.hogg1@outlook.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/jupyterhub_firstuseauthenticator_greg.egg-info/SOURCES.txt` & `jupyterhub-firstuseauthenticator-greg-1.3.0/jupyterhub_firstuseauthenticator_greg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-firstuseauthenticator-greg-1.2.0/setup.py` & `jupyterhub-firstuseauthenticator-greg-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 version_ns = {}
 with open(os.path.join(here, 'firstuseauthenticator', '_version.py')) as f:
     exec(f.read(), {}, version_ns)
 
 setup(
     name='jupyterhub-firstuseauthenticator-greg',
-    version='1.2.0',
+    version='1.3.0',
     description='JupyterHub Authenticator that lets users set passwords on first use, Greg style',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/gahogg/firstuseauthenticator",
     author="Yuvi Panda, Project Jupyter Contributors",
     author_email="greg.hogg1@outlook.com",
     license="BSD-3-Clause",
```

