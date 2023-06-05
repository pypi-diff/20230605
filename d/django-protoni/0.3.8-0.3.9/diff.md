# Comparing `tmp/django-protoni-0.3.8.tar.gz` & `tmp/django-protoni-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-protoni-0.3.8.tar", last modified: Mon Jun  5 11:09:32 2023, max compression
+gzip compressed data, was "django-protoni-0.3.9.tar", last modified: Mon Jun  5 11:18:29 2023, max compression
```

## Comparing `django-protoni-0.3.8.tar` & `django-protoni-0.3.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.021957 django-protoni-0.3.8/
--rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 11:09:32.021788 django-protoni-0.3.8/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.018494 django-protoni-0.3.8/django_protoni.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      816 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      549 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     6938 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)       23 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)       15 2023-06-05 11:09:32.000000 django-protoni-0.3.8/django_protoni.egg-info/top_level.txt
--rwxr-xr-x   0 aha        (501) staff       (20)     1426 2022-09-09 09:54:32.000000 django-protoni-0.3.8/manage.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.020360 django-protoni-0.3.8/protoni/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     6463 2022-09-05 05:28:04.000000 django-protoni-0.3.8/protoni/asetukset.py
--rw-r--r--   0 aha        (501) staff       (20)      731 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/asgi.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:09:32.021614 django-protoni-0.3.8/protoni/laajennos/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/celery.py
--rw-r--r--   0 aha        (501) staff       (20)      441 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/laajennos/corsheaders.py
--rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django-protoni-0.3.8/protoni/laajennos/debug_toolbar.py
--rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/dj_database_url.py
--rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django-protoni-0.3.8/protoni/laajennos/extensions.py
--rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/heroku.py
--rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django-protoni-0.3.8/protoni/laajennos/hosts.py
--rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/laajennos/pipeline.py
--rw-r--r--   0 aha        (501) staff       (20)     1713 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/laajennos/sentry.py
--rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django-protoni-0.3.8/protoni/laajennos/whitenoise.py
--rw-r--r--   0 aha        (501) staff       (20)     1705 2022-06-01 07:20:57.000000 django-protoni-0.3.8/protoni/nakymat.py
--rw-r--r--   0 aha        (501) staff       (20)     1186 2022-02-14 07:28:19.000000 django-protoni-0.3.8/protoni/osoitteet.py
--rw-r--r--   0 aha        (501) staff       (20)     2066 2022-06-14 09:31:09.000000 django-protoni-0.3.8/protoni/palvelimet.py
--rw-r--r--   0 aha        (501) staff       (20)     1656 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/palvelin.py
--rw-r--r--   0 aha        (501) staff       (20)      253 2023-06-05 11:08:55.000000 django-protoni-0.3.8/protoni/tyoasema.py
--rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django-protoni-0.3.8/protoni/wsgi.py
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-10-04 08:10:20.000000 django-protoni-0.3.8/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 11:09:32.021999 django-protoni-0.3.8/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)     1020 2023-06-05 11:08:55.000000 django-protoni-0.3.8/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:29.288889 django-protoni-0.3.9/
+-rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 11:18:29.288743 django-protoni-0.3.9/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:29.285345 django-protoni-0.3.9/django_protoni.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)       58 2023-06-05 11:18:29.000000 django-protoni-0.3.9/django_protoni.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      816 2023-06-05 11:18:29.000000 django-protoni-0.3.9/django_protoni.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 11:18:29.000000 django-protoni-0.3.9/django_protoni.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      549 2023-06-05 11:18:29.000000 django-protoni-0.3.9/django_protoni.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     7064 2023-06-05 11:18:29.000000 django-protoni-0.3.9/django_protoni.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)       23 2023-06-05 11:18:29.000000 django-protoni-0.3.9/django_protoni.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)       15 2023-06-05 11:18:29.000000 django-protoni-0.3.9/django_protoni.egg-info/top_level.txt
+-rwxr-xr-x   0 aha        (501) staff       (20)     1426 2022-09-09 09:54:32.000000 django-protoni-0.3.9/manage.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:29.287097 django-protoni-0.3.9/protoni/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.9/protoni/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     6463 2022-09-05 05:28:04.000000 django-protoni-0.3.9/protoni/asetukset.py
+-rw-r--r--   0 aha        (501) staff       (20)      731 2023-06-05 11:08:55.000000 django-protoni-0.3.9/protoni/asgi.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:29.288596 django-protoni-0.3.9/protoni/laajennos/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django-protoni-0.3.9/protoni/laajennos/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django-protoni-0.3.9/protoni/laajennos/celery.py
+-rw-r--r--   0 aha        (501) staff       (20)      441 2023-06-05 11:08:55.000000 django-protoni-0.3.9/protoni/laajennos/corsheaders.py
+-rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django-protoni-0.3.9/protoni/laajennos/debug_toolbar.py
+-rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django-protoni-0.3.9/protoni/laajennos/dj_database_url.py
+-rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django-protoni-0.3.9/protoni/laajennos/extensions.py
+-rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django-protoni-0.3.9/protoni/laajennos/heroku.py
+-rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django-protoni-0.3.9/protoni/laajennos/hosts.py
+-rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django-protoni-0.3.9/protoni/laajennos/pipeline.py
+-rw-r--r--   0 aha        (501) staff       (20)     1713 2023-06-05 11:08:55.000000 django-protoni-0.3.9/protoni/laajennos/sentry.py
+-rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django-protoni-0.3.9/protoni/laajennos/whitenoise.py
+-rw-r--r--   0 aha        (501) staff       (20)     1705 2022-06-01 07:20:57.000000 django-protoni-0.3.9/protoni/nakymat.py
+-rw-r--r--   0 aha        (501) staff       (20)     1186 2022-02-14 07:28:19.000000 django-protoni-0.3.9/protoni/osoitteet.py
+-rw-r--r--   0 aha        (501) staff       (20)     2066 2022-06-14 09:31:09.000000 django-protoni-0.3.9/protoni/palvelimet.py
+-rw-r--r--   0 aha        (501) staff       (20)     1656 2023-06-05 11:08:55.000000 django-protoni-0.3.9/protoni/palvelin.py
+-rw-r--r--   0 aha        (501) staff       (20)      253 2023-06-05 11:08:55.000000 django-protoni-0.3.9/protoni/tyoasema.py
+-rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django-protoni-0.3.9/protoni/wsgi.py
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-05 11:16:28.000000 django-protoni-0.3.9/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 11:18:29.288926 django-protoni-0.3.9/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)     1020 2023-06-05 11:08:55.000000 django-protoni-0.3.9/setup.py
```

### Comparing `django-protoni-0.3.8/django_protoni.egg-info/SOURCES.txt` & `django-protoni-0.3.9/django_protoni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/django_protoni.egg-info/entry_points.txt` & `django-protoni-0.3.9/django_protoni.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/django_protoni.egg-info/historia.json` & `django-protoni-0.3.9/django_protoni.egg-info/historia.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '7c675d7f15eda853ccadaa56e66e0f3676813350'), ('versio', "*

 * *           "'0.3.9'), ('kuvaus', 'Korjaus edelliseen')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "Korjaus edelliseen",
+        "revisio": "7c675d7f15eda853ccadaa56e66e0f3676813350",
+        "versio": "0.3.9"
+    },
+    {
         "kuvaus": "P\u00e4ivitetty versiointij\u00e4rjestelm\u00e4",
         "revisio": "d0e3dc7d331300b3f19858d3f4a9fc4c0fe74c93",
         "versio": "0.3.8"
     },
     {
         "kuvaus": "Sentry: parametrisoitu `send_default_pii`-parametrin arvo",
         "revisio": "d01461385713cc1873467d9bcec6d72aedeb88ff",
```

### Comparing `django-protoni-0.3.8/manage.py` & `django-protoni-0.3.9/manage.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/asetukset.py` & `django-protoni-0.3.9/protoni/asetukset.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/asgi.py` & `django-protoni-0.3.9/protoni/asgi.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/laajennos/hosts.py` & `django-protoni-0.3.9/protoni/laajennos/hosts.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/laajennos/pipeline.py` & `django-protoni-0.3.9/protoni/laajennos/pipeline.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/laajennos/sentry.py` & `django-protoni-0.3.9/protoni/laajennos/sentry.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/nakymat.py` & `django-protoni-0.3.9/protoni/nakymat.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/osoitteet.py` & `django-protoni-0.3.9/protoni/osoitteet.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/palvelimet.py` & `django-protoni-0.3.9/protoni/palvelimet.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/protoni/palvelin.py` & `django-protoni-0.3.9/protoni/palvelin.py`

 * *Files identical despite different names*

### Comparing `django-protoni-0.3.8/setup.py` & `django-protoni-0.3.9/setup.py`

 * *Files identical despite different names*

