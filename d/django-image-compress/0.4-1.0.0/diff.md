# Comparing `tmp/django_image_compress-0.4.tar.gz` & `tmp/django_image_compress-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_image_compress-0.4.tar", last modified: Mon Jun  5 09:42:44 2023, max compression
+gzip compressed data, was "django_image_compress-1.0.0.tar", last modified: Mon Jun  5 10:26:43 2023, max compression
```

## Comparing `django_image_compress-0.4.tar` & `django_image_compress-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:42:44.092036 django_image_compress-0.4/
--rw-rw-rw-   0        0        0      221 2023-06-05 09:42:44.091034 django_image_compress-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-06-05 09:34:54.000000 django_image_compress-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 09:42:44.066051 django_image_compress-0.4/django_image_compress/
--rw-rw-rw-   0        0        0        0 2023-06-05 08:57:01.000000 django_image_compress-0.4/django_image_compress/__init__.py
--rw-rw-rw-   0        0        0       46 2023-06-05 03:33:20.000000 django_image_compress-0.4/django_image_compress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:42:44.089043 django_image_compress-0.4/django_image_compress.egg-info/
--rw-rw-rw-   0        0        0      221 2023-06-05 09:42:43.000000 django_image_compress-0.4/django_image_compress.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-06-05 09:42:44.000000 django_image_compress-0.4/django_image_compress.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:42:43.000000 django_image_compress-0.4/django_image_compress.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 09:42:43.000000 django_image_compress-0.4/django_image_compress.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-05 09:42:43.000000 django_image_compress-0.4/django_image_compress.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 09:42:44.092036 django_image_compress-0.4/setup.cfg
--rw-rw-rw-   0        0        0      500 2023-06-05 09:42:38.000000 django_image_compress-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:26:43.494596 django_image_compress-1.0.0/
+-rw-rw-rw-   0        0        0      245 2023-06-05 10:26:43.493592 django_image_compress-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      893 2023-06-05 10:22:08.000000 django_image_compress-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 10:26:43.472602 django_image_compress-1.0.0/django_image_compress/
+-rw-rw-rw-   0        0        0        0 2023-06-05 09:47:45.000000 django_image_compress-1.0.0/django_image_compress/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-06-05 09:47:45.000000 django_image_compress-1.0.0/django_image_compress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:26:43.491593 django_image_compress-1.0.0/django_image_compress.egg-info/
+-rw-rw-rw-   0        0        0      245 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 10:26:43.495589 django_image_compress-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-06-05 10:26:31.000000 django_image_compress-1.0.0/setup.py
```

### Comparing `django_image_compress-0.4/README.md` & `django_image_compress-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,9 @@
     ``
     # build and create dist folder
     python setup.py build 
     python setup.py sdist 
     # install twine
     pip3 install twine
     # upload project
-    twine upload --repository pypi dist/*
+    twine upload --repository pypi dist/*
+    # note it may error because of name already exist
```

