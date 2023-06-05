# Comparing `tmp/naver-db-0.0.5.post5.tar.gz` & `tmp/naver-db-0.0.5.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naver-db-0.0.5.post5.tar", last modified: Fri May  5 21:22:12 2023, max compression
+gzip compressed data, was "naver-db-0.0.5.post6.tar", last modified: Mon Jun  5 04:19:44 2023, max compression
```

## Comparing `naver-db-0.0.5.post5.tar` & `naver-db-0.0.5.post6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/
--rw-rw-rw-   0        0        0      412 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.179930 naver-db-0.0.5.post5/naver_db/
--rw-rw-rw-   0        0        0      554 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/naver_db/__init__.py
--rw-rw-rw-   0        0        0    15142 2023-05-05 21:18:26.000000 naver-db-0.0.5.post5/naver_db/persistence.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.194904 naver-db-0.0.5.post5/naver_db.egg-info/
--rw-rw-rw-   0        0        0      412 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-05-05 21:18:58.000000 naver-db-0.0.5.post5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/test/
--rw-rw-rw-   0        0        0      194 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/__init__.py
--rw-rw-rw-   0        0        0      139 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_getprops.py
--rw-rw-rw-   0        0        0      263 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_nextval.py
--rw-rw-rw-   0        0        0      138 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_param.py
--rw-rw-rw-   0        0        0      178 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_query.py
--rw-rw-rw-   0        0        0      145 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_userpermission.py
--rw-rw-rw-   0        0        0      487 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_write.py
--rw-rw-rw-   0        0        0      381 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_writelog.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.357256 naver-db-0.0.5.post6/
+-rw-rw-rw-   0        0        0      412 2023-06-05 04:19:44.356135 naver-db-0.0.5.post6/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.314845 naver-db-0.0.5.post6/naver_db/
+-rw-rw-rw-   0        0        0      345 2023-06-05 04:16:55.000000 naver-db-0.0.5.post6/naver_db/__init__.py
+-rw-rw-rw-   0        0        0    15028 2023-06-05 04:16:07.000000 naver-db-0.0.5.post6/naver_db/persistence.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.332337 naver-db-0.0.5.post6/naver_db.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 04:19:44.358735 naver-db-0.0.5.post6/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-06-05 04:17:49.000000 naver-db-0.0.5.post6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.354143 naver-db-0.0.5.post6/test/
+-rw-rw-rw-   0        0        0      194 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_getprops.py
+-rw-rw-rw-   0        0        0      263 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_nextval.py
+-rw-rw-rw-   0        0        0      138 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_param.py
+-rw-rw-rw-   0        0        0      178 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_query.py
+-rw-rw-rw-   0        0        0      145 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_userpermission.py
+-rw-rw-rw-   0        0        0      487 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_write.py
+-rw-rw-rw-   0        0        0      381 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_writelog.py
```

### Comparing `naver-db-0.0.5.post5/naver_db/persistence.py` & `naver-db-0.0.5.post6/naver_db/persistence.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from sqlalchemy import exc
 import json
 import redis
 import ast
+import os
+from flask_sqlalchemy import SQLAlchemy
 
 
 class Persistence:
     """Clase para el manejo de los datos de la base de datos"""
 
-    def __init__(self, config, myApp, myDb):
+    def __init__(self, app, config):
         """Constructor de la clase
 
         Args:
             config (NaverConfig): Objeto de configuracion
-            myApp (Flask): Objeto de la aplicacion
-            myDb (FlaskAlchemy): Objeto de la base de datos
+            app (Flask): Objeto de la aplicacion 
         """
-        self.myApp = myApp
-        self.myApp.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
-        # self.myApp.config["SQLALCHEMY_ENGINE_OPTIONS"] = dict()
-        self.myDb = myDb
         self.config = config
+        app.config["DEBUG"] = False
+        app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
+        app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///:memory:"
+        self.db = SQLAlchemy(app, engine_options=dict(pool_pre_ping=True))
         self.mySession = [1, 1]
         self.redis = redis.Redis(
-            host=config.core.myVariables.get("REDIS_HOST"),
-            port=config.core.myVariables.get("REDIS_PORT"))
-        if(config.core.myVariables.get("REDIS_PASSWORD")is not None):
+            host=os.environ.get("REDIS_HOST"),
+            port=os.environ.get("REDIS_PORT"))
+        if(os.environ.get("REDIS_PASSWORD")is not None):
             self.redis = redis.Redis(
-            username=config.core.myVariables.get("REDIS_USER"),
-            host=config.core.myVariables.get("REDIS_HOST"),
-            port=config.core.myVariables.get("REDIS_PORT"),
-            password=config.core.myVariables.get("REDIS_PASSWORD")
+            host=os.environ.get("REDIS_HOST"),
+            port=os.environ.get("REDIS_PORT"),
+            password=os.environ.get("REDIS_PASSWORD")
             )
 
     def _sql(self, rawSql):
         """Método para ejecutar una consulta SQL
 
         Args:
             rawSql (str): Consulta SQL
@@ -42,18 +42,18 @@
             res: Resultado de la consulta
         """
         try:
             assert type(rawSql) == str
             # assert type(sqlVars) == dict
             res = self._sqltran(rawSql)
             if res is not None:
-                self.myDb.session.commit()
+                self.db.session.commit()
             return res
         except exc.SQLAlchemyError as e:
-            self.myDb.session.rollback()
+            self.db.session.rollback()
             print(e)
             raise e
 
     # TESTED
 
     def _sqltran(self, rawSql):
         """Método Raw para ejecutar una consulta SQL
@@ -63,16 +63,16 @@
 
         Returns:
             dict: Diccionario que contiene el cursor y la sesión de la consulta
         """
         try:
             assert type(rawSql) == str
             # assert type(sqlVars) == dict
-            cursor = self.myDb.session.execute(rawSql)
-            session = self.myDb.session
+            cursor = self.db.session.execute(rawSql)
+            session = self.db.session
             return {"cursor": cursor, "session": session}
         except exc.SQLAlchemyError as e:
             print(e)
             raise e
 
     # TESTED
```

### Comparing `naver-db-0.0.5.post5/setup.py` & `naver-db-0.0.5.post6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='naver-db',
-    version='0.0.5-5',
+    version='0.0.5-6',
     packages=setuptools.find_packages(),
     author="Jose Cuevas",
     author_email="jose.cuevas.cv@gmail.com",
     description="A DB Persistence Ancestor Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jacr6/naver-db",
```

