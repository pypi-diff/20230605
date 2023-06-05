# Comparing `tmp/django_tbase_post_product-2023.6.216856966.tar.gz` & `tmp/django_tbase_post_product-2023.6.516859753.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.6.216856966.tar", last modified: Fri Jun  2 09:04:18 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.6.516859753.tar", last modified: Mon Jun  5 14:29:43 2023, max compression
```

## Comparing `django_tbase_post_product-2023.6.216856966.tar` & `django_tbase_post_product-2023.6.516859753.tar`

### file list

```diff
@@ -1,59 +1,52 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.6.216856966/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1423 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1101 2023-06-02 09:03:18.000000 django_tbase_post_product-2023.6.216856966/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.795704 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1423 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     2109 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.6.216856966/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.835703 django_tbase_post_product-2023.6.216856966/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.216856966/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.6.216856966/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.216856966/tbase_post/apps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.835703 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.835703 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.6.216856966/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.6.216856966/tbase_post/sitemaps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.795704 django_tbase_post_product-2023.6.216856966/tbase_post/static/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.845703 django_tbase_post_product-2023.6.216856966/tbase_post/static/images/
--rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.845703 django_tbase_post_product-2023.6.216856966/tbase_post/templates/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.845703 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/
--rw-r--r--   0 terry     (1000) terry     (1000)     2799 2023-06-02 09:00:28.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/article_list_by_tag.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/article_list_by_tag.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)     2120 2023-05-09 11:29:39.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/blog_index.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/blog_index.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)     4173 2023-06-02 08:58:32.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/detail.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/detail.html:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/
--rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-05-09 11:22:22.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/amazon_link.html
--rw-r--r--   0 terry     (1000) terry     (1000)      376 2023-05-08 23:37:48.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/last_update.html
--rw-r--r--   0 terry     (1000) terry     (1000)      294 2023-05-08 23:37:59.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/related_post_by_tags.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)      415 2023-05-01 19:23:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/tags.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/sitemap.xml
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__init__.py:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     5044 2023-05-09 11:42:47.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/post_extras.py
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/post_extras.py:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.216856966/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.6.216856966/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3823 2023-06-02 08:57:44.000000 django_tbase_post_product-2023.6.216856966/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.6.516859753/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1524 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1165 2023-06-05 14:24:55.000000 django_tbase_post_product-2023.6.516859753/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.179309 django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1524 2023-06-05 14:29:43.000000 django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-06-05 14:29:43.000000 django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-06-05 14:29:43.000000 django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-06-05 14:29:43.000000 django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-06-05 14:29:43.000000 django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.6.516859753/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.179309 django_tbase_post_product-2023.6.516859753/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.516859753/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.6.516859753/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.516859753/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.179309 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.6.516859753/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.6.516859753/tbase_post/sitemaps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.179309 django_tbase_post_product-2023.6.516859753/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.516859753/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.516859753/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     2799 2023-06-02 09:00:28.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     2120 2023-05-09 11:29:39.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     4173 2023-06-02 08:58:32.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/detail.html
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-05-09 11:22:22.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/extras/amazon_link.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      374 2023-06-05 14:20:37.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/extras/last_update.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      288 2023-06-05 14:21:44.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      415 2023-05-01 19:23:09.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templates/sitemap.xml
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 14:29:43.189309 django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3934 2023-06-05 14:22:38.000000 django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.516859753/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.6.516859753/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3823 2023-06-02 08:57:44.000000 django_tbase_post_product-2023.6.516859753/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.6.216856966/PKG-INFO` & `django_tbase_post_product-2023.6.516859753/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.6.216856966
+Version: 2023.6.516859753
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
@@ -31,22 +33,28 @@
     'martor',
     'taggit',
 
  ]
 ```
 
 
+## 更新
 
+- 2023/06/05
+优化相关内容查询,模板文件
 
-# 2023/06/02
+
+- 2023/06/02
 加入seo优化，对tags内容过少（小于10）的页面添加noindex
 
 
 
 
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
@@ -66,7 +74,9 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
+
+
```

### Comparing `django_tbase_post_product-2023.6.216856966/README.md` & `django_tbase_post_product-2023.6.516859753/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -22,22 +22,28 @@
     'martor',
     'taggit',
 
  ]
 ```
 
 
+## 更新
 
+- 2023/06/05
+优化相关内容查询,模板文件
 
-# 2023/06/02
+
+- 2023/06/02
 加入seo优化，对tags内容过少（小于10）的页面添加noindex
 
 
 
 
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
```

### Comparing `django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.6.216856966
+Version: 2023.6.516859753
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
@@ -31,22 +33,28 @@
     'martor',
     'taggit',
 
  ]
 ```
 
 
+## 更新
 
+- 2023/06/05
+优化相关内容查询,模板文件
 
-# 2023/06/02
+
+- 2023/06/02
 加入seo优化，对tags内容过少（小于10）的页面添加noindex
 
 
 
 
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
@@ -66,7 +74,9 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
+
+
```

### Comparing `django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.6.516859753/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,24 +22,17 @@
 tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
 tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
 tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
 tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
 tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
 tbase_post/templates/sitemap.xml
 tbase_post/templates/post/article_list_by_tag.html
-tbase_post/templates/post/article_list_by_tag.html:Zone.Identifier
 tbase_post/templates/post/blog_index.html
-tbase_post/templates/post/blog_index.html:Zone.Identifier
 tbase_post/templates/post/detail.html
-tbase_post/templates/post/detail.html:Zone.Identifier
 tbase_post/templates/post/extras/amazon_link.html
 tbase_post/templates/post/extras/last_update.html
 tbase_post/templates/post/extras/related_post_by_tags.html
-tbase_post/templates/post/extras/related_post_by_tags.html:Zone.Identifier
 tbase_post/templates/post/extras/tags.html
-tbase_post/templates/post/extras/tags.html:Zone.Identifier
 tbase_post/templatetags/__init__.py
-tbase_post/templatetags/__init__.py:Zone.Identifier
 tbase_post/templatetags/post_extras.py
-tbase_post/templatetags/post_extras.py:Zone.Identifier
 tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
 tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
```

### Comparing `django_tbase_post_product-2023.6.216856966/setup.py` & `django_tbase_post_product-2023.6.516859753/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/admin.py` & `django_tbase_post_product-2023.6.516859753/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc` & `django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc` & `django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc` & `django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc` & `django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc` & `django_tbase_post_product-2023.6.516859753/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/models.py` & `django_tbase_post_product-2023.6.516859753/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.6.516859753/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/article_list_by_tag.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.6.516859753/tbase_post/templates/post/detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.6.516859753/tbase_post/templatetags/post_extras.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django import template
 from tbase_post.models import Post
+from pprint import pprint as pp
 from django.db.models import F
 register = template.Library()
 
 
 
 # 创建信息
 # https://docs.djangoproject.com/zh-hans/4.2/howto/custom-template-tags/
@@ -85,83 +86,41 @@
 
 """
 
 @register.inclusion_tag('post/extras/related_post_by_tags.html',
                         takes_context=False)
 def related_post_by_tags(tags=[], limit=5,exclude_pk=None):
     try:
-        slugs = list(tags.slugs())
-        # print("slugs", slugs)
-        # 排除本节点，查询相关的tags
-        if exclude_pk==None:
-            page_obj = Post.objects.filter(tags__slug__in=slugs).order_by('-pk').distinct()[:limit]
-        else:
-            page_obj = Post.objects.filter(tags__slug__in=slugs).exclude(
-                pk=exclude_pk).order_by('-pk').distinct()[:limit]
+        page_obj=tags.similar_objects()[-limit:]
+        # slugs = list(tags.slugs())
+        # # print("slugs", slugs)
+        # # 排除本节点，查询相关的tags
+        # if exclude_pk==None:
+        #     page_obj = Post.objects.filter(tags__slug__in=slugs).order_by('-pk').distinct()[:limit]
+        # else:
+        #     page_obj = Post.objects.filter(tags__slug__in=slugs).exclude(
+        #         pk=exclude_pk).order_by('-pk').distinct()[:limit]
 
         # print("page_obj", page_obj)
         return {
             'state': True,
             'link': "context['home_link']",
-            'title': "context['home_title']",
+            'title': "Related Content",
             "page_obj": page_obj,
             # "content": context
         }
     except Exception as e:
         # print(e)
         return {
             'state': False,
             'link': "context['home_link']",
-            'title': "context['home_title']",
+            'title': "Related Content",
             "page_obj": [],
             # "content": context
         }
-from pprint import pprint as pp
-# @register.inclusion_tag('post/extras/related_post_by_tags.html',
-#                         takes_context=False)
-@register.simple_tag(takes_context=True)
-def next_post(context):
-    #
-    # pp(context)
-    # print(context['object'])
-    # print("context", dir(context))
-    current_instance = context['object']
-    next_instance = Post.objects.filter(
-        pk__gt=current_instance.pk).order_by('-pk').first()
-    # return next_instance
-
-    # return previous_instance
-    if next_instance == None:
-        return ''
-    else:
-        return "<a href='%s'>%s</a>" % (next_instance.pk, next_instance.title)
-
-
-@register.simple_tag(takes_context=True)
-def previous_post(context):
-    #
-    # pp(context)
-    # print(context['object'])
-    # print("context", dir(context))
-    current_instance = context['object']
-    previous_instance = Post.objects.filter(
-        pk__lt=current_instance.pk).order_by('-pk').first()
-
-
-    # return previous_instance
-    if previous_instance==None:
-        return ''
-    else:
-        return "<a href='%s'>%s</a>" % (previous_instance.pk,
-                                        previous_instance.title)
-
-
-
-
-
 
 @register.inclusion_tag('post/extras/last_update.html',
                         takes_context=False)
 def last_update( limit=5,exclude_pk=None):
     """
     
     
@@ -174,20 +133,20 @@
             page_obj = Post.objects.all().exclude(
                 pk=exclude_pk).order_by('-pk').distinct()[:limit]
 
         # print("page_obj", page_obj)
         return {
             'state': True,
             'link': "context['home_link']",
-            'title': "context['home_title']",
+            'title': "Last Update",
             "page_obj": page_obj,
             # "content": context
         }
     except Exception as e:
         # print(e)
         return {
             'state': False,
             'link': "context['home_link']",
-            'title': "context['home_title']",
+            'title': "Last Update",
             "page_obj": [],
             # "content": context
         }
```

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/urls.py` & `django_tbase_post_product-2023.6.516859753/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.216856966/tbase_post/views.py` & `django_tbase_post_product-2023.6.516859753/tbase_post/views.py`

 * *Files identical despite different names*

