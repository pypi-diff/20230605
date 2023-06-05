# Comparing `tmp/django_tbase_post_product-2023.6.616859820.tar.gz` & `tmp/django_tbase_post_product-2023.6.616859875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.6.616859820.tar", last modified: Mon Jun  5 16:21:17 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.6.616859875.tar", last modified: Mon Jun  5 17:53:06 2023, max compression
```

## Comparing `django_tbase_post_product-2023.6.616859820.tar` & `django_tbase_post_product-2023.6.616859875.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.668084 django_tbase_post_product-2023.6.616859820/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.6.616859820/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-06-05 16:21:17.668084 django_tbase_post_product-2023.6.616859820/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.6.616859820/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.658084 django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-06-05 16:21:17.000000 django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-06-05 16:21:17.000000 django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-06-05 16:21:17.000000 django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-06-05 16:21:17.000000 django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-06-05 16:21:17.000000 django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-06-05 16:21:17.668084 django_tbase_post_product-2023.6.616859820/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.6.616859820/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.658084 django_tbase_post_product-2023.6.616859820/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859820/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.6.616859820/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859820/tbase_post/apps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.658084 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.658084 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.6.616859820/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.6.616859820/tbase_post/sitemaps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.648084 django_tbase_post_product-2023.6.616859820/tbase_post/static/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.658084 django_tbase_post_product-2023.6.616859820/tbase_post/static/images/
--rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859820/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859820/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.658084 django_tbase_post_product-2023.6.616859820/tbase_post/templates/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.668084 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/
--rw-r--r--   0 terry     (1000) terry     (1000)     2795 2023-06-05 15:21:00.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/article_list_by_tag.html
--rw-r--r--   0 terry     (1000) terry     (1000)     2116 2023-06-05 15:38:41.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/blog_index.html
--rw-r--r--   0 terry     (1000) terry     (1000)     5001 2023-06-05 16:20:34.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/detail.html
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.668084 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/extras/
--rw-r--r--   0 terry     (1000) terry     (1000)      511 2023-06-05 16:10:39.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/extras/amazon_link.html
--rw-r--r--   0 terry     (1000) terry     (1000)      374 2023-06-05 14:30:33.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/extras/last_update.html
--rw-r--r--   0 terry     (1000) terry     (1000)      288 2023-06-05 14:30:33.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      505 2023-06-05 15:36:14.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/extras/tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templates/sitemap.xml
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.668084 django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 16:21:17.668084 django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     5397 2023-06-05 15:31:14.000000 django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/post_extras.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859820/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.6.616859820/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3823 2023-06-02 08:57:44.000000 django_tbase_post_product-2023.6.616859820/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.6.616859875/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.6.616859875/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-06-05 17:53:06.000000 django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-06-05 17:53:06.000000 django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-06-05 17:53:06.000000 django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-06-05 17:53:06.000000 django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-06-05 17:53:06.000000 django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.6.616859875/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859875/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.6.616859875/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859875/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.6.616859875/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.6.616859875/tbase_post/sitemaps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.157074 django_tbase_post_product-2023.6.616859875/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859875/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859875/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     3626 2023-06-05 17:51:37.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     2116 2023-06-05 15:38:41.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     5001 2023-06-05 16:20:34.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/detail.html
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      511 2023-06-05 16:10:39.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/extras/amazon_link.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      374 2023-06-05 14:30:33.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/extras/last_update.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      288 2023-06-05 14:30:33.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      505 2023-06-05 15:36:14.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templates/sitemap.xml
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 17:53:06.167074 django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     5397 2023-06-05 15:31:14.000000 django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859875/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.6.616859875/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3823 2023-06-02 08:57:44.000000 django_tbase_post_product-2023.6.616859875/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.6.616859820/PKG-INFO` & `django_tbase_post_product-2023.6.616859875/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.6.616859820
+Version: 2023.6.616859875
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.6.616859820/README.md` & `django_tbase_post_product-2023.6.616859875/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.6.616859820
+Version: 2023.6.616859875
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.6.616859820/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.6.616859875/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/setup.py` & `django_tbase_post_product-2023.6.616859875/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/admin.py` & `django_tbase_post_product-2023.6.616859875/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc` & `django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc` & `django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc` & `django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc` & `django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc` & `django_tbase_post_product-2023.6.616859875/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/models.py` & `django_tbase_post_product-2023.6.616859875/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.6.616859875/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/article_list_by_tag.html`

 * *Files 19% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                     <a href="{% url 'detail_view' detail.pk %}" class="text-3xl font-bold hover:text-gray-700 pb-4">{{detail.title}}</a>
                     <p  class="text-sm pb-3">
                         By <a href="#" class="font-semibold hover:text-gray-800">David Grzyb</a>, Published on {{detail.created_on}}
                     </p>
 
                     <p class="pb-6">
                         {% comment %} 限制文本长度 {% endcomment %}
-                          {{detail.content|truncatechars:3}}
+                          {{detail.content|truncatechars:128}}
                     </p>
 {% tags detail.tags%}
 
                     <a href="{% url 'detail_view' detail.pk %}" class="uppercase text-gray-800 hover:text-black">Continue Reading {{detail.product_name}}<i class="fas fa-arrow-right"></i></a>
                 </div>
             </article>
 
@@ -74,10 +74,36 @@
             <a class="h-10 w-10 font-semibold text-gray-800 hover:text-gray-900 text-sm flex items-center justify-center ml-3" href="?page={{ page_obj.next_page_number }}">next</a>
             <a href="?page={{ page_obj.paginator.num_pages }}">last &raquo;</a>
         {% endif %}
     </span>
 
 
 </div> {% endcomment %}
+
+
 {% endblock %}
 
 
+
+
+
+
+{% block sidebar_section %}
+<!-- sidebar_section -->
+ {% block about_us %}
+    <!-- about_us -->
+    <div class="w-full bg-white shadow flex flex-col my-4 p-6">
+        <!-- <p class="text-xl font-semibold pb-5">About Us</p>
+        <p class="pb-2">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas mattis est eu odio sagittis tristique. Vestibulum ut finibus leo. In hac habitasse platea dictumst.</p>
+        <a href="#" class="w-full bg-blue-800 text-white font-bold text-sm uppercase rounded hover:bg-blue-700 flex items-center justify-center px-2 py-3 mt-4">
+            Get to know us
+        </a> -->
+        {% last_update 10 %}
+
+        
+    </div>
+   {% endblock %}
+    <div class="w-full bg-white shadow flex flex-col my-4 p-6">
+
+    </div>
+    <!-- sidebar_section endblock -->
+   {% endblock %}
```

#### html2text {}

```diff
@@ -6,15 +6,19 @@
 block article_list %} {% for detail in object_list %}   {%if
 detail.article_img%}
 [{{detail.product_name}}]
 {%endif%}
 {{detail.title}}
 By David_Grzyb, Published on {{detail.created_on}}
 {% comment %} éå¶ææ¬é¿åº¦ {% endcomment %} {
-{detail.content|truncatechars:3}}
+{detail.content|truncatechars:128}}
 {% tags detail.tags%}
 Continue_Reading_{{detail.product_name}}
  {% endfor %} {% comment %}
  {% if page_obj.has_previous %} «_first previous {% endif %}  Page {
 { page_obj.number }} of {{ page_obj.paginator.num_pages }}.  {% if
 page_obj.has_next %} next last_» {% endif %}
-{% endcomment %} {% endblock %}
+{% endcomment %} {% endblock %} {% block sidebar_section %}  {% block about_us
+%}
+ {% last_update 10 %}
+{% endblock %}
+ {% endblock %}
```

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.6.616859875/tbase_post/templates/post/detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.6.616859875/tbase_post/templatetags/post_extras.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/urls.py` & `django_tbase_post_product-2023.6.616859875/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859820/tbase_post/views.py` & `django_tbase_post_product-2023.6.616859875/tbase_post/views.py`

 * *Files identical despite different names*

