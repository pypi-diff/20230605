# Comparing `tmp/django-protoni-0.3.4.tar.gz` & `tmp/django-protoni-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-protoni-0.3.4.tar", last modified: Wed Sep  7 12:15:07 2022, max compression
+gzip compressed data, was "django-protoni-0.3.6.tar", last modified: Mon Jun  5 10:34:33 2023, max compression
```

## Comparing `django-protoni-0.3.4.tar` & `django-protoni-0.3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-09-07 12:15:07.613559 django-protoni-0.3.4/
--rw-r--r--   0 aha        (501) staff       (20)       58 2022-09-07 12:15:07.613427 django-protoni-0.3.4/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-09-07 12:15:07.604105 django-protoni-0.3.4/django_protoni.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)       58 2022-09-07 12:15:07.000000 django-protoni-0.3.4/django_protoni.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      783 2022-09-07 12:15:07.000000 django-protoni-0.3.4/django_protoni.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2022-09-07 12:15:07.000000 django-protoni-0.3.4/django_protoni.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      505 2022-09-07 12:15:07.000000 django-protoni-0.3.4/django_protoni.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     8237 2022-09-07 12:15:07.000000 django-protoni-0.3.4/django_protoni.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)       23 2022-09-07 12:15:07.000000 django-protoni-0.3.4/django_protoni.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)       15 2022-09-07 12:15:07.000000 django-protoni-0.3.4/django_protoni.egg-info/top_level.txt
--rwxr-xr-x   0 aha        (501) staff       (20)     1426 2022-09-05 05:28:17.000000 django-protoni-0.3.4/manage.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-09-07 12:15:07.612012 django-protoni-0.3.4/protoni/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     6463 2022-09-05 05:28:04.000000 django-protoni-0.3.4/protoni/asetukset.py
--rw-r--r--   0 aha        (501) staff       (20)     1168 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/asgi.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-09-07 12:15:07.613279 django-protoni-0.3.4/protoni/laajennos/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/laajennos/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/laajennos/celery.py
--rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django-protoni-0.3.4/protoni/laajennos/debug_toolbar.py
--rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/laajennos/dj_database_url.py
--rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django-protoni-0.3.4/protoni/laajennos/extensions.py
--rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/laajennos/heroku.py
--rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django-protoni-0.3.4/protoni/laajennos/hosts.py
--rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/laajennos/pipeline.py
--rw-r--r--   0 aha        (501) staff       (20)     1623 2022-02-09 13:43:22.000000 django-protoni-0.3.4/protoni/laajennos/sentry.py
--rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django-protoni-0.3.4/protoni/laajennos/whitenoise.py
--rw-r--r--   0 aha        (501) staff       (20)     1705 2022-06-01 07:20:57.000000 django-protoni-0.3.4/protoni/nakymat.py
--rw-r--r--   0 aha        (501) staff       (20)     1186 2022-02-14 07:28:19.000000 django-protoni-0.3.4/protoni/osoitteet.py
--rw-r--r--   0 aha        (501) staff       (20)     2066 2022-06-14 09:31:09.000000 django-protoni-0.3.4/protoni/palvelimet.py
--rw-r--r--   0 aha        (501) staff       (20)     1664 2022-07-28 10:27:33.000000 django-protoni-0.3.4/protoni/palvelin.py
--rw-r--r--   0 aha        (501) staff       (20)      162 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/tyoasema.py
--rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django-protoni-0.3.4/protoni/wsgi.py
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-10-04 08:10:20.000000 django-protoni-0.3.4/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2022-09-07 12:15:07.613598 django-protoni-0.3.4/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      959 2022-02-14 07:28:21.000000 django-protoni-0.3.4/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.506913 django-protoni-0.3.6/
+-rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 10:34:33.506769 django-protoni-0.3.6/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.503589 django-protoni-0.3.6/django_protoni.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      783 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      505 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     6603 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)       23 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)       15 2023-06-05 10:34:33.000000 django-protoni-0.3.6/django_protoni.egg-info/top_level.txt
+-rwxr-xr-x   0 aha        (501) staff       (20)     1426 2022-09-09 09:54:32.000000 django-protoni-0.3.6/manage.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.505393 django-protoni-0.3.6/protoni/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     6463 2022-09-05 05:28:04.000000 django-protoni-0.3.6/protoni/asetukset.py
+-rw-r--r--   0 aha        (501) staff       (20)      731 2022-11-08 12:28:37.000000 django-protoni-0.3.6/protoni/asgi.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 10:34:33.506607 django-protoni-0.3.6/protoni/laajennos/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/celery.py
+-rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django-protoni-0.3.6/protoni/laajennos/debug_toolbar.py
+-rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/dj_database_url.py
+-rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django-protoni-0.3.6/protoni/laajennos/extensions.py
+-rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/heroku.py
+-rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django-protoni-0.3.6/protoni/laajennos/hosts.py
+-rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/laajennos/pipeline.py
+-rw-r--r--   0 aha        (501) staff       (20)     1713 2023-06-05 10:31:40.000000 django-protoni-0.3.6/protoni/laajennos/sentry.py
+-rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django-protoni-0.3.6/protoni/laajennos/whitenoise.py
+-rw-r--r--   0 aha        (501) staff       (20)     1705 2022-06-01 07:20:57.000000 django-protoni-0.3.6/protoni/nakymat.py
+-rw-r--r--   0 aha        (501) staff       (20)     1186 2022-02-14 07:28:19.000000 django-protoni-0.3.6/protoni/osoitteet.py
+-rw-r--r--   0 aha        (501) staff       (20)     2066 2022-06-14 09:31:09.000000 django-protoni-0.3.6/protoni/palvelimet.py
+-rw-r--r--   0 aha        (501) staff       (20)     1664 2022-07-28 10:27:33.000000 django-protoni-0.3.6/protoni/palvelin.py
+-rw-r--r--   0 aha        (501) staff       (20)      162 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/tyoasema.py
+-rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django-protoni-0.3.6/protoni/wsgi.py
+-rw-r--r--   0 aha        (501) staff       (20)       72 2021-10-04 08:10:20.000000 django-protoni-0.3.6/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 10:34:33.506950 django-protoni-0.3.6/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      967 2023-06-05 10:34:12.000000 django-protoni-0.3.6/setup.py
```

### Comparing `django-protoni-0.3.4/django_protoni.egg-info/SOURCES.txt` & `django-protoni-0.3.6/django_protoni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/manage.py` & `django-protoni-0.3.6/manage.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/protoni/asetukset.py` & `django-protoni-0.3.6/protoni/asetukset.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/protoni/laajennos/hosts.py` & `django-protoni-0.3.6/protoni/laajennos/hosts.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/protoni/laajennos/pipeline.py` & `django-protoni-0.3.6/protoni/laajennos/pipeline.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/protoni/laajennos/sentry.py` & `django-protoni-0.3.6/protoni/laajennos/sentry.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 '''
 Sentry-SDK-käyttöönotto. Edellyttää seuraavien muuttujien määrityksen:
 - SENTRY_DSN: Sentry-palvelimen yhteysosoite
 - SENTRY_PAKETTIVERSIO: sen Pip-paketin nimi, jonka versionumero
   ilmoitetaan Sentrylle.
 '''
+import functools
 import logging
 
 import sentry_sdk
 from sentry_sdk.integrations.django import DjangoIntegration
 from sentry_sdk.integrations.logging import LoggingIntegration
 
 # Poimi DSN-yhteysosoite.
@@ -41,24 +42,29 @@
 if CONFIG('SENTRY_OHITA_VARMENNE', cast=bool, default=False):
   sentry_sdk.transport.HttpTransport._get_pool_options \
   = lambda self, ca_certs: {
     'num_pools': 2,
     'cert_reqs': 'CERT_NONE',
   }
 
+
 # Alusta Sentry-määritys.
 # Ks. https://docs.sentry.io/platforms/python/guides/django/
 sentry_sdk.init(
   dsn=dsn,
   release=versio,
   integrations=[
     LoggingIntegration(
       level=logging.INFO,
       event_level=logging.WARNING,
     ),
     DjangoIntegration(),
   ],
-  send_default_pii=True,
+  send_default_pii=CONFIG(
+    'SENTRY_SEND_DEFAULT_PII',
+    cast=bool,
+    default=False,
+  ),
 )
 del logging
 del sentry_sdk, DjangoIntegration, LoggingIntegration
 del dsn, versio
```

### Comparing `django-protoni-0.3.4/protoni/nakymat.py` & `django-protoni-0.3.6/protoni/nakymat.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/protoni/osoitteet.py` & `django-protoni-0.3.6/protoni/osoitteet.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/protoni/palvelimet.py` & `django-protoni-0.3.6/protoni/palvelimet.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/protoni/palvelin.py` & `django-protoni-0.3.6/protoni/palvelin.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.4/setup.py` & `django-protoni-0.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -* - coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
-  setup_requires='git-versiointi',
+  setup_requires='git-versiointi>=1.6rc3',
   name='django-protoni',
   packages=find_packages(),
   py_modules=['manage'],
   include_package_data=True,
   scripts=['manage.py'],
   install_requires=['Django', 'python-decouple'],
   entry_points={
```

