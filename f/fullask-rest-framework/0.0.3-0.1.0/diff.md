# Comparing `tmp/fullask-rest-framework-0.0.3.tar.gz` & `tmp/fullask-rest-framework-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask-rest-framework-0.0.3.tar", last modified: Sun Nov  6 18:46:29 2022, max compression
+gzip compressed data, was "fullask-rest-framework-0.1.0.tar", last modified: Mon Jun  5 16:29:19 2023, max compression
```

## Comparing `fullask-rest-framework-0.0.3.tar` & `fullask-rest-framework-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,100 @@
-drwxr-xr-x   0 goddessana   (501) staff       (20)        0 2022-11-06 18:46:29.109642 fullask-rest-framework-0.0.3/
--rw-r--r--   0 goddessana   (501) staff       (20)     1068 2022-10-21 11:16:47.000000 fullask-rest-framework-0.0.3/LICENSE
--rw-r--r--   0 goddessana   (501) staff       (20)     6392 2022-11-06 18:46:29.109698 fullask-rest-framework-0.0.3/PKG-INFO
--rw-r--r--   0 goddessana   (501) staff       (20)     5347 2022-11-06 18:44:46.000000 fullask-rest-framework-0.0.3/README.md
--rw-r--r--   0 goddessana   (501) staff       (20)     1225 2022-11-06 18:46:29.109994 fullask-rest-framework-0.0.3/setup.cfg
--rw-r--r--   0 goddessana   (501) staff       (20)      400 2022-10-22 15:35:31.000000 fullask-rest-framework-0.0.3/setup.py
-drwxr-xr-x   0 goddessana   (501) staff       (20)        0 2022-11-06 18:46:29.108011 fullask-rest-framework-0.0.3/src/
-drwxr-xr-x   0 goddessana   (501) staff       (20)        0 2022-11-06 18:46:29.108720 fullask-rest-framework-0.0.3/src/fullask_rest_framework/
--rw-r--r--   0 goddessana   (501) staff       (20)        0 2022-10-22 15:35:54.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework/__init__.py
--rw-r--r--   0 goddessana   (501) staff       (20)      830 2022-10-27 01:21:02.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework/cli.py
-drwxr-xr-x   0 goddessana   (501) staff       (20)        0 2022-11-06 18:46:29.109503 fullask-rest-framework-0.0.3/src/fullask_rest_framework.egg-info/
--rw-r--r--   0 goddessana   (501) staff       (20)     6392 2022-11-06 18:46:29.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework.egg-info/PKG-INFO
--rw-r--r--   0 goddessana   (501) staff       (20)      411 2022-11-06 18:46:29.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework.egg-info/SOURCES.txt
--rw-r--r--   0 goddessana   (501) staff       (20)        1 2022-11-06 18:46:29.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework.egg-info/dependency_links.txt
--rw-r--r--   0 goddessana   (501) staff       (20)       63 2022-11-06 18:46:29.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework.egg-info/entry_points.txt
--rw-r--r--   0 goddessana   (501) staff       (20)       11 2022-11-06 18:46:29.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework.egg-info/requires.txt
--rw-r--r--   0 goddessana   (501) staff       (20)       23 2022-11-06 18:46:29.000000 fullask-rest-framework-0.0.3/src/fullask_rest_framework.egg-info/top_level.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.395936 fullask-rest-framework-0.1.0/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      175 2023-04-17 01:36:01.000000 fullask-rest-framework-0.1.0/AUTHORS.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       89 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/HISTORY.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1070 2023-04-17 01:40:34.000000 fullask-rest-framework-0.1.0/LICENSE
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      306 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/MANIFEST.in
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      833 2023-06-05 16:29:19.395936 fullask-rest-framework-0.1.0/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5613 2023-05-12 14:14:35.000000 fullask-rest-framework-0.1.0/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.375935 fullask-rest-framework-0.1.0/docs/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      632 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/Makefile
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.379936 fullask-rest-framework-0.1.0/docs/docfiles/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/docfiles/authors.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5075 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/docfiles/conf.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1997 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/docfiles/contributing.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/docfiles/history.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      313 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/docfiles/index.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1246 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/docfiles/installation.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       99 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/docfiles/usage.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      829 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/docs/make.bat
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.379936 fullask-rest-framework-0.1.0/fullask_rest_framework/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      150 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      604 2023-04-21 13:51:24.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/cli.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.379936 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-18 18:19:58.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.383936 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.383936 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/templates/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      851 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/templates/login_form.html
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.383936 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/templates/static/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1146 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/contrib/admin/views.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.375935 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.383936 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/app_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/app_template/schemas.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.383936 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/project_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-08 13:47:33.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      112 2023-03-12 13:06:42.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      322 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      628 2023-04-18 19:16:45.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       65 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/createproject_template/project_template/tests.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.387936 fullask-rest-framework-0.1.0/fullask_rest_framework/entities/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-07 17:34:01.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/entities/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       49 2023-05-15 10:40:45.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/entities/base_entity.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      346 2023-05-08 13:47:35.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/entities/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      450 2023-06-05 16:00:39.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/entities/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      407 2023-05-15 10:15:36.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/entities/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.387936 fullask-rest-framework-0.1.0/fullask_rest_framework/factory/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-02 15:45:42.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/factory/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3842 2023-05-07 17:40:59.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/factory/app_factory.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      641 2023-06-05 06:20:45.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/factory/extensions.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.387936 fullask-rest-framework-0.1.0/fullask_rest_framework/orm/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:06:42.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/orm/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.387936 fullask-rest-framework-0.1.0/fullask_rest_framework/orm/sqlalchemy/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-13 16:25:47.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/orm/sqlalchemy/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      228 2023-06-05 16:15:54.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/orm/sqlalchemy/base_model.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      985 2023-06-05 16:15:24.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/orm/sqlalchemy/mixins.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.387936 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.391936 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       37 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/.gitignore
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      191 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      302 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.375935 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/v/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.391936 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/v/cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       69 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/v/cache/lastfailed
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       63 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        2 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-20 07:40:30.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      427 2023-06-05 16:03:17.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/base.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     2852 2023-06-05 16:03:27.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/crud.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     8568 2023-06-05 16:03:08.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/repositories/sqlalchemy.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.391936 fullask-rest-framework-0.1.0/fullask_rest_framework/schemas/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/schemas/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1212 2023-05-15 07:28:57.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/schemas/fields.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      267 2023-06-05 16:08:35.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/schemas/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1033 2023-06-05 16:10:52.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/schemas/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      636 2023-06-05 16:11:02.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/schemas/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.391936 fullask-rest-framework-0.1.0/fullask_rest_framework/service/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-12 12:54:11.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/service/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.391936 fullask-rest-framework-0.1.0/fullask_rest_framework/utils/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/utils/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      572 2023-04-14 13:52:15.000000 fullask-rest-framework-0.1.0/fullask_rest_framework/utils/jwt.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.379936 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      833 2023-06-05 16:29:19.000000 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3227 2023-06-05 16:29:19.000000 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 16:29:19.000000 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       68 2023-06-05 16:29:19.000000 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/entry_points.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 16:25:15.000000 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/not-zip-safe
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       22 2023-06-05 16:29:19.000000 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/requires.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       23 2023-06-05 16:29:19.000000 fullask-rest-framework-0.1.0/fullask_rest_framework.egg-info/top_level.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      846 2023-06-05 15:57:14.000000 fullask-rest-framework-0.1.0/pyproject.toml
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      394 2023-06-05 16:29:19.395936 fullask-rest-framework-0.1.0/setup.cfg
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1538 2023-06-05 16:28:12.000000 fullask-rest-framework-0.1.0/setup.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.391936 fullask-rest-framework-0.1.0/tests/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:34:17.000000 fullask-rest-framework-0.1.0/tests/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:29:19.391936 fullask-rest-framework-0.1.0/tests/repositories/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:35:54.000000 fullask-rest-framework-0.1.0/tests/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)    20125 2023-06-05 16:00:28.000000 fullask-rest-framework-0.1.0/tests/repositories/test_sqlalchemy_repository.py
```

### Comparing `fullask-rest-framework-0.0.3/LICENSE` & `fullask-rest-framework-0.1.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 TGoddessana
+Copyright (c) 2023, tgoddessana
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -15,7 +15,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `fullask-rest-framework-0.0.3/PKG-INFO` & `fullask-rest-framework-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: fullask-rest-framework
-Version: 0.0.3
-Summary: A fully-supported flask extension to build REST API.
-Home-page: https://github.com/tgoddessana/flask-rest-framework/
-Author: TGoddessana
-Author-email: twicegoddessana1229@gmail.com
-Maintainer: TGoddessana
-Maintainer-email: twicegoddessana1229@gmail.com
-License: MIT
-Project-URL: Documentation, https://tgoddessana.github.io/fullask-rest-framework/
-Project-URL: Source Code, https://github.com/tgoddessana/flask-rest-framework/
-Project-URL: Issue Tracker, https://github.com/tgoddessana/flask-rest-framework/issues
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Flask
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 
 <div align="center">
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
@@ -37,15 +12,15 @@
 </div>
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/tgoddessana/flask-rest-framework">
-    <img src="images/logo.png" alt="Logo" width="300" height="300">
+    <img src="/artworks/frf-logo.png.png" style="width:75%";>
   </a>
 
 <h3 align="center">Fullask-REST-Framework</h3>
 
   <p align="center">
     A fully-supported flask extension to build REST API.
     <br />
@@ -55,115 +30,105 @@
     <a href="">Report Bug</a>
     ·
     <a href="">Request Feature</a>
   </p>
 </div>
 
 
-<!-- ABOUT THE PROJECT -->
+<!---------------------------------------------------------------------------------------------->
+
+<br/>
 
 ## About Fullask-REST-Framework
 
 ---
 
-[![Product Name Screen Shot][product-screenshot]](https://example.com)
+Fullask REST Framework is a framework that makes it easier and faster to build REST APIs.
+
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Built With
 
-![Flask][Flask]  
+![Flask][Flask]
 ![Python][Python]
 
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
+<!---------------------------------------------------------------------------------------------->
 
-<!-- Requirements -->
+<br/>
 
 ## Requirements
 
 ---
 
 - python 3.8+
 - flask 2.0 +
 
-<!-- GETTING STARTED -->
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!---------------------------------------------------------------------------------------------->
+
+<br/>
 
 ## Getting Started
 
+---
+
 ### Installation
 
----
 
 install using pip command.
 
    ```
-   pip install flask-rest-framework
+   pip install fullask-rest-framework
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
-<!-- USAGE EXAMPLES -->
+<!---------------------------------------------------------------------------------------------->
+
+<br/>
 
 ## Usage
 
 ---
-something usage..  
+something usage..
 _For more examples, please refer to the [Documentation](https://tgoddessana.github.io/fullask-rest-framework/)_
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## Versioning rules
-
----
-_writing in progress..._
 
+<!---------------------------------------------------------------------------------------------->
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+<br/>
 
 ## Commit convention
 
 ---
 
 - FEAT : A new feature.
 - FIX : A bug fix.
 - TYPO : A typo fix.
 - DOCS : Documentation only changes. this includes "README.md", and "/docs/".
 - REFACTOR : A code change that neither fixes a bug nor adds a feature.
 - DEPLOY : A code change for deploy this package.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-<!-- ROADMAP -->
+<!---------------------------------------------------------------------------------------------->
 
-## Roadmap
-
----
-
-- [ ] create fully-supported app directories by command line interface
-    - [ ] create api packages
-    - [ ] create test packages
-      - [ ]create model packages
-- [ ] support sqlalchemy ORM system
-- [ ] support serialize & deserialize system
-- [ ] support admin page
-
-See the [open issues](https://github.com/tgoddessana/flask-rest-framework/issues) for a full list of proposed features (
-and known issues).
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- CONTRIBUTING -->
+<br/>
 
 ## Contributing
 
 ---
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
 contributions you make are **greatly appreciated**.
@@ -176,43 +141,44 @@
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add : some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
+<!---------------------------------------------------------------------------------------------->
 
-
-<!-- LICENSE -->
+<br/>
 
 ## License
 
 ---
 
 Distributed under the MIT License. See `LICENSE.txt` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
+<!---------------------------------------------------------------------------------------------->
 
-
-<!-- CONTACT -->
+<br/>
 
 ## Contact
 
 ---
 
-Email: twicegoddessana1229@gmail.com  
+Email: twicegoddessana1229@gmail.com
 Project Link: [https://github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/flask-rest-framework)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
+<!---------------------------------------------------------------------------------------------->
+<!---------------------------------------------------------------------------------------------->
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
 [contributors-shield]: https://img.shields.io/github/contributors/tgoddessana/flask-rest-framework.svg?style=for-the-badge
 
 [contributors-url]: https://github.com/tgoddessana/flask-rest-framework/graphs/contributors
@@ -236,9 +202,7 @@
 [product-screenshot]: images/screenshot.png
 
 [Flask]: https://img.shields.io/badge/flask-00000?style=for-the-badge&logo=flask&logoColor=white
 
 [Python]: https://img.shields.io/badge/python-306998?style=for-the-badge&logo=python&logoColor=white
 
 
-
-
```

#### html2text {}

```diff
@@ -1,76 +1,62 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.0.3 Summary: A
-fully-supported flask extension to build REST API. Home-page: https://
-github.com/tgoddessana/flask-rest-framework/ Author: TGoddessana Author-email:
-twicegoddessana1229@gmail.com Maintainer: TGoddessana Maintainer-email:
-twicegoddessana1229@gmail.com License: MIT Project-URL: Documentation, https://
-tgoddessana.github.io/fullask-rest-framework/ Project-URL: Source Code, https:/
-/github.com/tgoddessana/flask-rest-framework/ Project-URL: Issue Tracker,
-https://github.com/tgoddessana/flask-rest-framework/issues Platform: UNKNOWN
-Classifier: Environment :: Web Environment Classifier: Framework :: Flask
-Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
-Development :: Libraries :: Application Frameworks Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE
+
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
-                                    [Logo]
+                                       >
                        **** Fullask-REST-Framework ****
              A fully-supported flask extension to build REST API.
                              Explore_the_docs_Â»
 
                          Report Bug Â· Request Feature
- ## About Fullask-REST-Framework --- [![Product Name Screen Shot][product-
-screenshot]](https://example.com)
+
+## About Fullask-REST-Framework --- Fullask REST Framework is a framework that
+makes it easier and faster to build REST APIs.
                                                                   (back_to_top)
 ### Built With ![Flask][Flask] ![Python][Python]
                                                                   (back_to_top)
- ## Requirements --- - python 3.8+ - flask 2.0 +  ## Getting Started ###
-Installation --- install using pip command. ``` pip install flask-rest-
-framework ```
+
+## Requirements --- - python 3.8+ - flask 2.0 +
                                                                   (back_to_top)
- ## Usage --- something usage.. _For more examples, please refer to the
-[Documentation](https://tgoddessana.github.io/fullask-rest-framework/)_
+
+## Getting Started --- ### Installation install using pip command. ``` pip
+install fullask-rest-framework ```
                                                                   (back_to_top)
-## Versioning rules --- _writing in progress..._
+
+## Usage --- something usage.. _For more examples, please refer to the
+[Documentation](https://tgoddessana.github.io/fullask-rest-framework/)_
                                                                   (back_to_top)
+
 ## Commit convention --- - FEAT : A new feature. - FIX : A bug fix. - TYPO : A
 typo fix. - DOCS : Documentation only changes. this includes "README.md", and
 "/docs/". - REFACTOR : A code change that neither fixes a bug nor adds a
 feature. - DEPLOY : A code change for deploy this package.
                                                                   (back_to_top)
- ## Roadmap --- - [ ] create fully-supported app directories by command line
-interface - [ ] create api packages - [ ] create test packages - [ ]create
-model packages - [ ] support sqlalchemy ORM system - [ ] support serialize &
-deserialize system - [ ] support admin page See the [open issues](https://
-github.com/tgoddessana/flask-rest-framework/issues) for a full list of proposed
-features ( and known issues).
-                                                                  (back_to_top)
- ## Contributing --- Contributions are what make the open source community such
+
+## Contributing --- Contributions are what make the open source community such
 an amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
 -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add : some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (back_to_top)
- ## License --- Distributed under the MIT License. See `LICENSE.txt` for more
+
+## License --- Distributed under the MIT License. See `LICENSE.txt` for more
 information.
                                                                   (back_to_top)
- ## Contact --- Email: twicegoddessana1229@gmail.com Project Link: [https://
+
+## Contact --- Email: twicegoddessana1229@gmail.com Project Link: [https://
 github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/
 flask-rest-framework)
                                                                   (back_to_top)
-                                                                  (back_to_top)
-  [contributors-shield]: https://img.shields.io/github/contributors/
+    [contributors-shield]: https://img.shields.io/github/contributors/
 tgoddessana/flask-rest-framework.svg?style=for-the-badge [contributors-url]:
 https://github.com/tgoddessana/flask-rest-framework/graphs/contributors [forks-
 shield]: https://img.shields.io/github/forks/tgoddessana/flask-rest-
 framework.svg?style=for-the-badge [forks-url]: https://github.com/tgoddessana/
 flask-rest-framework/network/members [stars-shield]: https://img.shields.io/
 github/stars/tgoddessana/flask-rest-framework.svg?style=for-the-badge [stars-
 url]: https://github.com/tgoddessana/flask-rest-framework/stargazers [issues-
```

