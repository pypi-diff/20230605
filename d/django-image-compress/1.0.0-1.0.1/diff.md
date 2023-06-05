# Comparing `tmp/django_image_compress-1.0.0.tar.gz` & `tmp/django_image_compress-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_image_compress-1.0.0.tar", last modified: Mon Jun  5 10:26:43 2023, max compression
+gzip compressed data, was "django_image_compress-1.0.1.tar", last modified: Mon Jun  5 12:59:09 2023, max compression
```

## Comparing `django_image_compress-1.0.0.tar` & `django_image_compress-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 10:26:43.494596 django_image_compress-1.0.0/
--rw-rw-rw-   0        0        0      245 2023-06-05 10:26:43.493592 django_image_compress-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      893 2023-06-05 10:22:08.000000 django_image_compress-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 10:26:43.472602 django_image_compress-1.0.0/django_image_compress/
--rw-rw-rw-   0        0        0        0 2023-06-05 09:47:45.000000 django_image_compress-1.0.0/django_image_compress/__init__.py
--rw-rw-rw-   0        0        0       44 2023-06-05 09:47:45.000000 django_image_compress-1.0.0/django_image_compress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-05 10:26:43.491593 django_image_compress-1.0.0/django_image_compress.egg-info/
--rw-rw-rw-   0        0        0      245 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-05 10:26:43.000000 django_image_compress-1.0.0/django_image_compress.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 10:26:43.495589 django_image_compress-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-06-05 10:26:31.000000 django_image_compress-1.0.0/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-05 12:59:09.072314 django_image_compress-1.0.1/
+-rw-r--r--   0 mac        (501) staff       (20)      235 2023-06-05 12:59:09.071844 django_image_compress-1.0.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      893 2023-06-05 12:20:07.000000 django_image_compress-1.0.1/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-05 12:59:09.067947 django_image_compress-1.0.1/django_image_compress/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-05 12:20:07.000000 django_image_compress-1.0.1/django_image_compress/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1458 2023-06-05 12:50:35.000000 django_image_compress-1.0.1/django_image_compress/compress.py
+-rw-r--r--   0 mac        (501) staff       (20)     1130 2023-06-05 12:37:39.000000 django_image_compress-1.0.1/django_image_compress/dimension.py
+-rw-r--r--   0 mac        (501) staff       (20)     1321 2023-06-05 12:50:35.000000 django_image_compress-1.0.1/django_image_compress/image_file.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-05 12:59:09.071154 django_image_compress-1.0.1/django_image_compress.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      235 2023-06-05 12:59:09.000000 django_image_compress-1.0.1/django_image_compress.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      381 2023-06-05 12:59:09.000000 django_image_compress-1.0.1/django_image_compress.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-05 12:59:09.000000 django_image_compress-1.0.1/django_image_compress.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)        7 2023-06-05 12:59:09.000000 django_image_compress-1.0.1/django_image_compress.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       22 2023-06-05 12:59:09.000000 django_image_compress-1.0.1/django_image_compress.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-05 12:59:09.072465 django_image_compress-1.0.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      505 2023-06-05 12:58:59.000000 django_image_compress-1.0.1/setup.py
```

### Comparing `django_image_compress-1.0.0/README.md` & `django_image_compress-1.0.1/README.md`

 * *Files identical despite different names*

