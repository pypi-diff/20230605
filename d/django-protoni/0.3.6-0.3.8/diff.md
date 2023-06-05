# Comparing `tmp/django-protoni-0.3.6.tar.gz` & `tmp/django-protoni-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-protoni-0.3.6.tar", last modified: Mon Jun  5 10:34:33 2023, max compression
+gzip compressed data, was "django-protoni-0.3.8.tar", last modified: Mon Jun  5 11:09:32 2023, max compression
```

## Comparing `django-protoni-0.3.6.tar` & `django-protoni-0.3.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.506913 django-protoni-0.3.6/
--rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 10:34:33.506769 django-protoni-0.3.6/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.503589 django-protoni-0.3.6/django_protoni.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      783 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      505 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     6603 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)       23 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)       15 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/top_level.txt
--rwxr-xr-x   0 aha        (501) staff       (20)     1426 2022-09-09 09:54:32.000000 django-protoni-0.3.6/manage.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.505393 django-protoni-0.3.6/protoni/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     6463 2022-09-05 05:28:04.000000 django-protoni-0.3.6/protoni/asetukset.py
--rw-r--r--   0 aha        (501) staff       (20)      731 2022-11-08 12:28:37.000000 django-protoni-0.3.6/protoni/asgi.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.506607 django-protoni-0.3.6/protoni/laajennos/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/celery.py
--rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django-protoni-0.3.6/protoni/laajennos/debug_toolbar.py
--rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/dj_database_url.py
--rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django-protoni-0.3.6/protoni/laajennos/extensions.py
--rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/heroku.py
--rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django-protoni-0.3.6/protoni/laajennos/hosts.py
--rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/pipeline.py
--rw-r--r--   0 aha        (501) staff       (20)     1713 2023-06-05 10:31:40.000000 django-protoni-0.3.6/protoni/laajennos/sentry.py
--rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django-protoni-0.3.6/protoni/laajennos/whitenoise.py
--rw-r--r--   0 aha        (501) staff       (20)     1705 2022-06-01 07:20:57.000000 django-protoni-0.3.6/protoni/nakymat.py
--rw-r--r--   0 aha        (501) staff       (20)     1186 2022-02-14 07:28:19.000000 django-protoni-0.3.6/protoni/osoitteet.py
--rw-r--r--   0 aha        (501) staff       (20)     2066 2022-06-14 09:31:09.000000 django-protoni-0.3.6/protoni/palvelimet.py
--rw-r--r--   0 aha        (501) staff       (20)     1664 2022-07-28 10:27:33.000000 django-protoni-0.3.6/protoni/palvelin.py
--rw-r--r--   0 aha        (501) staff       (20)      162 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/tyoasema.py
--rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/wsgi.py
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-10-04 08:10:20.000000 django-protoni-0.3.6/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 10:34:33.506950 django-protoni-0.3.6/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      967 2023-06-05 10:34:12.000000 django-protoni-0.3.6/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.021957 django-protoni-0.3.8/
+-rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 11:09:32.021788 django-protoni-0.3.8/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.018494 django-protoni-0.3.8/django_protoni.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      816 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      549 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     6938 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)       23 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)       15 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/top_level.txt
+-rwxr-xr-x   0 aha        (501) staff       (20)     1426 2022-09-09 09:54:32.000000 django-protoni-0.3.8/manage.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.020360 django-protoni-0.3.8/protoni/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     6463 2022-09-05 05:28:04.000000 django-protoni-0.3.8/protoni/asetukset.py
+-rw-r--r--   0 aha        (501) staff       (20)      731 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/asgi.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.021614 django-protoni-0.3.8/protoni/laajennos/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/celery.py
+-rw-r--r--   0 aha        (501) staff       (20)      441 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/laajennos/corsheaders.py
+-rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django-protoni-0.3.8/protoni/laajennos/debug_toolbar.py
+-rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/dj_database_url.py
+-rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django-protoni-0.3.8/protoni/laajennos/extensions.py
+-rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/heroku.py
+-rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django-protoni-0.3.8/protoni/laajennos/hosts.py
+-rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/pipeline.py
+-rw-r--r--   0 aha        (501) staff       (20)     1713 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/laajennos/sentry.py
+-rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django-protoni-0.3.8/protoni/laajennos/whitenoise.py
+-rw-r--r--   0 aha        (501) staff       (20)     1705 2022-06-01 07:20:57.000000 django-protoni-0.3.8/protoni/nakymat.py
+-rw-r--r--   0 aha        (501) staff       (20)     1186 2022-02-14 07:28:19.000000 django-protoni-0.3.8/protoni/osoitteet.py
+-rw-r--r--   0 aha        (501) staff       (20)     2066 2022-06-14 09:31:09.000000 django-protoni-0.3.8/protoni/palvelimet.py
+-rw-r--r--   0 aha        (501) staff       (20)     1656 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/palvelin.py
+-rw-r--r--   0 aha        (501) staff       (20)      253 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/tyoasema.py
+-rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/wsgi.py
+-rw-r--r--   0 aha        (501) staff       (20)       72 2021-10-04 08:10:20.000000 django-protoni-0.3.8/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 11:09:32.021999 django-protoni-0.3.8/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)     1020 2023-06-05 11:08:55.000000 django-protoni-0.3.8/setup.py
```

### Comparing `django-protoni-0.3.6/django_protoni.egg-info/SOURCES.txt` & `django-protoni-0.3.8/django_protoni.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 protoni/osoitteet.py
 protoni/palvelimet.py
 protoni/palvelin.py
 protoni/tyoasema.py
 protoni/wsgi.py
 protoni/laajennos/__init__.py
 protoni/laajennos/celery.py
+protoni/laajennos/corsheaders.py
 protoni/laajennos/debug_toolbar.py
 protoni/laajennos/dj_database_url.py
 protoni/laajennos/extensions.py
 protoni/laajennos/heroku.py
 protoni/laajennos/hosts.py
 protoni/laajennos/pipeline.py
 protoni/laajennos/sentry.py
```

### Comparing `django-protoni-0.3.6/django_protoni.egg-info/historia.json` & `django-protoni-0.3.8/django_protoni.egg-info/historia.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9379844961240309%*

 * *Differences: {'2': "{'revisio': '11e5ebab5281bce1faa64eb2cfd6247bfe5c89d0', 'kuvaus': 'Lisätty "*

 * *      "`corsheaders`-laajennos'}",*

 * * '3': "{'revisio': '3662ffc95fd28b7263a46445f5d37fb9ad83b4f5', 'kuvaus': 'Käytetään "*

 * *      "`ALLOWED_HOSTS`-parametriä myös työasemalla'}",*

 * * 'insert': "[(0, OrderedDict([('revisio', 'd0e3dc7d331300b3f19858d3f4a9fc4c0fe74c93'), ('versio', "*

 * *           "'0.3.8'), ('kuvaus', 'Päivitetty versiointijärjestelmä')])), (1, "*

 * *           "OrderedDict([('revisio', 'd01461385713cc1873467d9bcec6d72aede […]*

```diff
@@ -1,16 +1,26 @@
 [
     {
         "kuvaus": "P\u00e4ivitetty versiointij\u00e4rjestelm\u00e4",
-        "revisio": "286106c71f80aff28f0757779335f556dc89dd41",
-        "versio": "0.3.6"
+        "revisio": "d0e3dc7d331300b3f19858d3f4a9fc4c0fe74c93",
+        "versio": "0.3.8"
     },
     {
         "kuvaus": "Sentry: parametrisoitu `send_default_pii`-parametrin arvo",
-        "revisio": "51df73dfae82c8de0c98045e7d8671ea3b6fa336",
+        "revisio": "d01461385713cc1873467d9bcec6d72aedeb88ff",
+        "versio": "0.3.7"
+    },
+    {
+        "kuvaus": "Lis\u00e4tty `corsheaders`-laajennos",
+        "revisio": "11e5ebab5281bce1faa64eb2cfd6247bfe5c89d0",
+        "versio": "0.3.6"
+    },
+    {
+        "kuvaus": "K\u00e4ytet\u00e4\u00e4n `ALLOWED_HOSTS`-parametri\u00e4 my\u00f6s ty\u00f6asemalla",
+        "revisio": "3662ffc95fd28b7263a46445f5d37fb9ad83b4f5",
         "versio": "0.3.5"
     },
     {
         "kuvaus": "Lis\u00e4tty `RUNSERVER_SSL_{KEY,CERT}FILE`-asetukset",
         "revisio": "a3904c736e1152d2b5a0d6a188c2d3ac020b8853",
         "versio": "0.3.4"
     },
```

### Comparing `django-protoni-0.3.6/manage.py` & `django-protoni-0.3.8/manage.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/asetukset.py` & `django-protoni-0.3.8/protoni/asetukset.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/asgi.py` & `django-protoni-0.3.8/protoni/asgi.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/laajennos/hosts.py` & `django-protoni-0.3.8/protoni/laajennos/hosts.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/laajennos/pipeline.py` & `django-protoni-0.3.8/protoni/laajennos/pipeline.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/laajennos/sentry.py` & `django-protoni-0.3.8/protoni/laajennos/sentry.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/nakymat.py` & `django-protoni-0.3.8/protoni/nakymat.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/osoitteet.py` & `django-protoni-0.3.8/protoni/osoitteet.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/palvelimet.py` & `django-protoni-0.3.8/protoni/palvelimet.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.6/protoni/palvelin.py` & `django-protoni-0.3.8/protoni/palvelin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from .asetukset import *
 
 
 SECRET_KEY = CONFIG('SECRET_KEY', default='subatominen-hiukkanen')
 
-ALLOWED_HOSTS = CONFIG('ALLOWED_HOSTS', cast=lambda v: [
-  s.strip() for s in v.split(',')
-], default='')
+ALLOWED_HOSTS = CONFIG(
+  'ALLOWED_HOSTS',
+  cast=lambda x: list(map(str.strip, x.split(','))),
+)
 
 DEBUG = CONFIG("DEBUG", cast=bool, default=False)
 
 SECURE_CONTENT_TYPE_NOSNIFF = True # per security.W006
 SECURE_BROWSER_XSS_FILTER = True # per security.W007
 SECURE_SSL_REDIRECT = True # per security.W008
 SESSION_COOKIE_SECURE = True # per security.W012
```

### Comparing `django-protoni-0.3.6/setup.py` & `django-protoni-0.3.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     'django.nakymat': [
       '__debug__ = protoni.nakymat:DebugToolbar',
       'kirjaudu = protoni.nakymat:Kirjautuminen',
       'kanta = protoni.nakymat:Kanta',
     ],
     'django.asetukset': [
       'celery = protoni.laajennos.celery',
+      'corsheaders = protoni.laajennos.corsheaders',
       'debug_toolbar = protoni.laajennos.debug_toolbar',
       'dj_database_url = protoni.laajennos.dj_database_url',
       'extensions = protoni.laajennos.extensions',
       'heroku = protoni.laajennos.heroku',
       'hosts = protoni.laajennos.hosts',
       'pipeline = protoni.laajennos.pipeline',
       'sentry = protoni.laajennos.sentry',
```

