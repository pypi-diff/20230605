# Comparing `tmp/fullask-rest-framework-0.1.1.tar.gz` & `tmp/fullask-rest-framework-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask-rest-framework-0.1.1.tar", last modified: Mon Jun  5 17:04:03 2023, max compression
+gzip compressed data, was "fullask-rest-framework-0.1.2.tar", last modified: Mon Jun  5 17:34:27 2023, max compression
```

## Comparing `fullask-rest-framework-0.1.1.tar` & `fullask-rest-framework-0.1.2.tar`

### file list

```diff
@@ -1,100 +1,98 @@
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      175 2023-04-17 01:36:01.000000 fullask-rest-framework-0.1.1/AUTHORS.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       89 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/HISTORY.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1070 2023-04-17 01:40:34.000000 fullask-rest-framework-0.1.1/LICENSE
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      306 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/MANIFEST.in
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      833 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/PKG-INFO
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5613 2023-05-12 14:14:35.000000 fullask-rest-framework-0.1.1/README.md
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.137071 fullask-rest-framework-0.1.1/docs/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      632 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/Makefile
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.137071 fullask-rest-framework-0.1.1/docs/docfiles/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/docfiles/authors.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5075 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/docfiles/conf.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1997 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/docfiles/contributing.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/docfiles/history.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      313 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/docfiles/index.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1246 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/docfiles/installation.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       99 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/docfiles/usage.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      829 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/docs/make.bat
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.137071 fullask-rest-framework-0.1.1/fullask_rest_framework/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      150 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      604 2023-04-21 13:51:24.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/cli.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.141071 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-18 18:19:58.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.141071 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.141071 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/templates/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/templates/index.html
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      851 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/templates/login_form.html
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.141071 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/templates/static/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1146 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/views.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.129071 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.141071 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/app_template/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/app_template/schemas.txt
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.145071 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/project_template/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-08 13:47:33.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      112 2023-03-12 13:06:42.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      322 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      628 2023-04-18 19:16:45.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       65 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/project_template/tests.txt
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.145071 fullask-rest-framework-0.1.1/fullask_rest_framework/entities/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-07 17:34:01.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/entities/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       49 2023-05-15 10:40:45.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/entities/base_entity.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      346 2023-05-08 13:47:35.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/entities/filtering.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      450 2023-06-05 16:00:39.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/entities/pagination.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      407 2023-05-15 10:15:36.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/entities/sorting.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.145071 fullask-rest-framework-0.1.1/fullask_rest_framework/factory/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-02 15:45:42.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/factory/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3875 2023-06-05 16:58:36.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/factory/app_factory.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      641 2023-06-05 06:20:45.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/factory/extensions.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.145071 fullask-rest-framework-0.1.1/fullask_rest_framework/orm/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:06:42.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/orm/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.149071 fullask-rest-framework-0.1.1/fullask_rest_framework/orm/sqlalchemy/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-13 16:25:47.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/orm/sqlalchemy/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      228 2023-06-05 16:15:54.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/orm/sqlalchemy/base_model.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      985 2023-06-05 16:15:24.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/orm/sqlalchemy/mixins.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.149071 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.149071 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       37 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/.gitignore
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      191 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      302 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/README.md
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.133071 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/v/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.149071 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/v/cache/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       69 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/v/cache/lastfailed
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       63 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        2 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-20 07:40:30.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      427 2023-06-05 16:03:17.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/base.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     2852 2023-06-05 16:03:27.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/crud.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     8568 2023-06-05 16:03:08.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/sqlalchemy.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1212 2023-05-15 07:28:57.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/fields.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      267 2023-06-05 16:08:35.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/filtering.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1033 2023-06-05 16:10:52.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/pagination.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      636 2023-06-05 16:11:02.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/sorting.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/fullask_rest_framework/service/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-12 12:54:11.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/service/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/fullask_rest_framework/utils/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/utils/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      572 2023-04-14 13:52:15.000000 fullask-rest-framework-0.1.1/fullask_rest_framework/utils/jwt.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.141071 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      833 2023-06-05 17:04:03.000000 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/PKG-INFO
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3227 2023-06-05 17:04:03.000000 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 17:04:03.000000 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       68 2023-06-05 17:04:03.000000 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/entry_points.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 17:04:03.000000 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/not-zip-safe
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       22 2023-06-05 17:04:03.000000 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/requires.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       23 2023-06-05 17:04:03.000000 fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/top_level.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      846 2023-06-05 15:57:14.000000 fullask-rest-framework-0.1.1/pyproject.toml
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      394 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/setup.cfg
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1538 2023-06-05 17:02:42.000000 fullask-rest-framework-0.1.1/setup.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/tests/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:34:17.000000 fullask-rest-framework-0.1.1/tests/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:04:03.153071 fullask-rest-framework-0.1.1/tests/repositories/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:35:54.000000 fullask-rest-framework-0.1.1/tests/repositories/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)    20125 2023-06-05 16:00:28.000000 fullask-rest-framework-0.1.1/tests/repositories/test_sqlalchemy_repository.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      175 2023-04-17 01:36:01.000000 fullask-rest-framework-0.1.2/AUTHORS.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1070 2023-04-17 01:40:34.000000 fullask-rest-framework-0.1.2/LICENSE
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      306 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/MANIFEST.in
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5482 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     4659 2023-06-05 17:27:25.000000 fullask-rest-framework-0.1.2/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.875509 fullask-rest-framework-0.1.2/docs/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      632 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/Makefile
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.875509 fullask-rest-framework-0.1.2/docs/docfiles/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/authors.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5075 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/conf.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1997 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/contributing.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      313 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/index.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1246 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/installation.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       99 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/usage.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      829 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/make.bat
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      150 2023-06-05 17:33:38.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      604 2023-04-21 13:51:24.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/cli.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-18 18:19:58.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      851 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/login_form.html
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/static/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1146 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/views.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.871509 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/schemas.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-08 13:47:33.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      112 2023-03-12 13:06:42.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      322 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      628 2023-04-18 19:16:45.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       65 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/tests.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-07 17:34:01.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       49 2023-05-15 10:40:45.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/base_entity.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      346 2023-05-08 13:47:35.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      450 2023-06-05 16:00:39.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      407 2023-05-15 10:15:36.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-02 15:45:42.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3875 2023-06-05 16:58:36.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/app_factory.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      641 2023-06-05 06:20:45.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/extensions.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:06:42.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-13 16:25:47.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      228 2023-06-05 16:15:54.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/base_model.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      985 2023-06-05 16:15:24.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/mixins.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       37 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/.gitignore
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      191 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      302 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.871509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       69 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/lastfailed
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       63 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        2 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-20 07:40:30.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      427 2023-06-05 16:03:17.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/base.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     2852 2023-06-05 16:03:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/crud.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     8568 2023-06-05 16:03:08.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/sqlalchemy.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1212 2023-05-15 07:28:57.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/fields.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      267 2023-06-05 16:08:35.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1033 2023-06-05 16:10:52.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      636 2023-06-05 16:11:02.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/fullask_rest_framework/service/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-12 12:54:11.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/service/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/fullask_rest_framework/utils/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/utils/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      572 2023-04-14 13:52:15.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/utils/jwt.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5482 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3189 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       68 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/entry_points.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/not-zip-safe
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      153 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/requires.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       23 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/top_level.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      846 2023-06-05 15:57:14.000000 fullask-rest-framework-0.1.2/pyproject.toml
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      394 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/setup.cfg
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1654 2023-06-05 17:30:32.000000 fullask-rest-framework-0.1.2/setup.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/tests/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:34:17.000000 fullask-rest-framework-0.1.2/tests/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/tests/repositories/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:35:54.000000 fullask-rest-framework-0.1.2/tests/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)    20125 2023-06-05 16:00:28.000000 fullask-rest-framework-0.1.2/tests/repositories/test_sqlalchemy_repository.py
```

### Comparing `fullask-rest-framework-0.1.1/LICENSE` & `fullask-rest-framework-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/README.md` & `fullask-rest-framework-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,29 @@
-<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
+Metadata-Version: 2.1
+Name: fullask-rest-framework
+Version: 0.1.2
+Summary: A fully-supported flask extension to build REST API.
+Home-page: https://github.com/tgoddessana/fullask-rest-framework
+Author: tgoddessana
+Author-email: twicegoddessana1229@gmail.com
+License: MIT license
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
 <a name="readme-top"></a>
 
 <div align="center">
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
@@ -95,15 +116,17 @@
 <!---------------------------------------------------------------------------------------------->
 
 <br/>
 
 ## Usage
 
 ---
-something usage..
+
+
+
 _For more examples, please refer to the [Documentation](https://tgoddessana.github.io/fullask-rest-framework/)_
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!---------------------------------------------------------------------------------------------->
 
@@ -122,37 +145,14 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!---------------------------------------------------------------------------------------------->
 
 <br/>
 
-## Contributing
-
----
-
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
-contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also
-simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add : some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-<!---------------------------------------------------------------------------------------------->
-
-<br/>
-
 ## License
 
 ---
 
 Distributed under the MIT License. See `LICENSE.txt` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
@@ -161,16 +161,16 @@
 
 <br/>
 
 ## Contact
 
 ---
 
-Email: twicegoddessana1229@gmail.com
-Project Link: [https://github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/flask-rest-framework)
+- Email: twicegoddessana1229@gmail.com
+- Project Link: [https://github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/flask-rest-framework)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 
 <!---------------------------------------------------------------------------------------------->
```

#### html2text {}

```diff
@@ -1,8 +1,18 @@
-
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.2 Summary: A
+fully-supported flask extension to build REST API. Home-page: https://
+github.com/tgoddessana/fullask-rest-framework Author: tgoddessana Author-email:
+twicegoddessana1229@gmail.com License: MIT license Classifier: Development
+Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE License-File: AUTHORS.rst
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                        >
                        **** Fullask-REST-Framework ****
              A fully-supported flask extension to build REST API.
@@ -19,40 +29,29 @@
 ## Requirements --- - python 3.8+ - flask 2.0 +
                                                                   (back_to_top)
 
 ## Getting Started --- ### Installation install using pip command. ``` pip
 install fullask-rest-framework ```
                                                                   (back_to_top)
 
-## Usage --- something usage.. _For more examples, please refer to the
-[Documentation](https://tgoddessana.github.io/fullask-rest-framework/)_
+## Usage --- _For more examples, please refer to the [Documentation](https://
+tgoddessana.github.io/fullask-rest-framework/)_
                                                                   (back_to_top)
 
 ## Commit convention --- - FEAT : A new feature. - FIX : A bug fix. - TYPO : A
 typo fix. - DOCS : Documentation only changes. this includes "README.md", and
 "/docs/". - REFACTOR : A code change that neither fixes a bug nor adds a
 feature. - DEPLOY : A code change for deploy this package.
                                                                   (back_to_top)
 
-## Contributing --- Contributions are what make the open source community such
-an amazing place to learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. If you have a suggestion that would make this better,
-please fork the repo and create a pull request. You can also simply open an
-issue with the tag "enhancement". Don't forget to give the project a star!
-Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
--b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add : some
-AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request
-                                                                  (back_to_top)
-
 ## License --- Distributed under the MIT License. See `LICENSE.txt` for more
 information.
                                                                   (back_to_top)
 
-## Contact --- Email: twicegoddessana1229@gmail.com Project Link: [https://
+## Contact --- - Email: twicegoddessana1229@gmail.com - Project Link: [https://
 github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/
 flask-rest-framework)
                                                                   (back_to_top)
     [contributors-shield]: https://img.shields.io/github/contributors/
 tgoddessana/flask-rest-framework.svg?style=for-the-badge [contributors-url]:
 https://github.com/tgoddessana/flask-rest-framework/graphs/contributors [forks-
 shield]: https://img.shields.io/github/forks/tgoddessana/flask-rest-
```

### Comparing `fullask-rest-framework-0.1.1/docs/Makefile` & `fullask-rest-framework-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/docs/docfiles/conf.py` & `fullask-rest-framework-0.1.2/docs/docfiles/conf.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/docs/docfiles/contributing.rst` & `fullask-rest-framework-0.1.2/docs/docfiles/contributing.rst`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/docs/docfiles/installation.rst` & `fullask-rest-framework-0.1.2/docs/docfiles/installation.rst`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/docs/make.bat` & `fullask-rest-framework-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/cli.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/factory/app_factory.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/factory/app_factory.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/factory/extensions.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/orm/sqlalchemy/mixins.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/crud.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/crud.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/repositories/sqlalchemy.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/fields.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/pagination.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/schemas/sorting.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework/utils/jwt.py` & `fullask-rest-framework-0.1.2/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/fullask_rest_framework.egg-info/SOURCES.txt` & `fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 AUTHORS.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 docs/Makefile
 docs/make.bat
 docs/docfiles/authors.rst
 docs/docfiles/conf.py
 docs/docfiles/contributing.rst
-docs/docfiles/history.rst
 docs/docfiles/index.rst
 docs/docfiles/installation.rst
 docs/docfiles/usage.rst
 fullask_rest_framework/__init__.py
 fullask_rest_framework/cli.py
 fullask_rest_framework.egg-info/PKG-INFO
 fullask_rest_framework.egg-info/SOURCES.txt
```

### Comparing `fullask-rest-framework-0.1.1/pyproject.toml` & `fullask-rest-framework-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.1/setup.py` & `fullask-rest-framework-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 """The setup script."""
 
 from setuptools import find_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-with open("HISTORY.rst") as history_file:
-    history = history_file.read()
-
-requirements = ["Click>=7.0", "Flask>=2.2"]
+requirements = [
+    "Click>=7.0",
+    "Flask>=2.2",
+    "flask-jwt-extended",
+    "marshmallow",
+    "marshmallow-sqlalchemy",
+    "flask-sqlalchemy",
+    "flask-marshmallow",
+    "flask-migrate",
+    "flask-smorest",
+    "python-dotenv",
+]
 
 test_requirements = []
 
 setup(
     author="tgoddessana",
     author_email="twicegoddessana1229@gmail.com",
     python_requires=">=3.8",
@@ -31,20 +39,20 @@
     ],
     description="A fully-supported flask extension to build REST API.",
     entry_points={
         "console_scripts": ["fullask-manager=fullask_rest_framework.cli:main"],
     },
     install_requires=requirements,
     license="MIT license",
-    long_description="README.md",
+    long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     name="fullask-rest-framework",
     packages=find_packages(
         include=["fullask_rest_framework", "fullask_rest_framework.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/tgoddessana/fullask-rest-framework",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `fullask-rest-framework-0.1.1/tests/repositories/test_sqlalchemy_repository.py` & `fullask-rest-framework-0.1.2/tests/repositories/test_sqlalchemy_repository.py`

 * *Files identical despite different names*

