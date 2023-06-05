# Comparing `tmp/django-postgres-metrics-0.8.0.tar.gz` & `tmp/django-postgres-metrics-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-postgres-metrics-0.8.0.tar", last modified: Sun Jan  3 19:26:24 2021, max compression
+gzip compressed data, was "django-postgres-metrics-0.9.0.tar", last modified: Tue Jan  5 19:08:19 2021, max compression
```

## Comparing `django-postgres-metrics-0.8.0.tar` & `django-postgres-metrics-0.9.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.268893 django-postgres-metrics-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.248893 django-postgres-metrics-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.260893 django-postgres-metrics-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     4765 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      457 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      178 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      390 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)     1548 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      126 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5613 2021-01-03 19:26:24.268893 django-postgres-metrics-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3248 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.260893 django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5613 2021-01-03 19:26:23.000000 django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1554 2021-01-03 19:26:24.000000 django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-03 19:26:23.000000 django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      139 2021-01-03 19:26:23.000000 django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-03 19:26:23.000000 django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.260893 django-postgres-metrics-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)       11 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      637 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      831 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (116)    83339 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/_static/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (116)      898 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/background.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3281 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2467 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/docs/source/contributing/
--rw-r--r--   0 runner    (1001) docker     (116)      106 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      550 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/contributing/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1769 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/ext.py
--rw-r--r--   0 runner    (1001) docker     (116)     5423 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (116)      334 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/docs/source/ref/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/ref/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (116)       71 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/docs/source/ref/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/example/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/example/example/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2970 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/example/example/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)      198 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/example/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)      168 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/example/example/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      540 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/example/manage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2689 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/post_screenshot_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/postgres_metrics/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      199 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)    19824 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)      282 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.252893 django-postgres-metrics-0.8.0/postgres_metrics/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.252893 django-postgres-metrics-0.8.0/postgres_metrics/static/postgres_metrics/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/postgres_metrics/static/postgres_metrics/css/
--rw-r--r--   0 runner    (1001) docker     (116)      701 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/static/postgres_metrics/css/base.css
--rw-r--r--   0 runner    (1001) docker     (116)      256 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/static/postgres_metrics/css/rtl.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.252893 django-postgres-metrics-0.8.0/postgres_metrics/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/postgres_metrics/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (116)     1327 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.264893 django-postgres-metrics-0.8.0/postgres_metrics/templates/postgres_metrics/
--rw-r--r--   0 runner    (1001) docker     (116)     3600 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/templates/postgres_metrics/table.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.268893 django-postgres-metrics-0.8.0/postgres_metrics/templatetags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2413 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/templatetags/postgres_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)      302 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)      756 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/postgres_metrics/views.py
--rw-r--r--   0 runner    (1001) docker     (116)      382 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       88 2021-01-03 19:26:24.268893 django-postgres-metrics-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2247 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:24.268893 django-postgres-metrics-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3505 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     3478 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/tests/test_liveserver.py
--rw-r--r--   0 runner    (1001) docker     (116)    17471 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     4722 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (116)     3720 2021-01-03 19:26:10.000000 django-postgres-metrics-0.8.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.874402 django-postgres-metrics-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.866402 django-postgres-metrics-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     5897 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     5546 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      457 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      390 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (116)     1548 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      126 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     5700 2021-01-05 19:08:19.874402 django-postgres-metrics-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3327 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5700 2021-01-05 19:08:19.000000 django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1554 2021-01-05 19:08:19.000000 django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-05 19:08:19.000000 django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      139 2021-01-05 19:08:19.000000 django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-05 19:08:19.000000 django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      637 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)      831 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (116)    83339 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/_static/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (116)      898 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/background.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3570 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2467 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/docs/source/contributing/
+-rw-r--r--   0 runner    (1001) docker     (116)      106 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      550 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/contributing/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1769 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/ext.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5423 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      334 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/docs/source/ref/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/ref/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (116)       71 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/docs/source/ref/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/example/example/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2970 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/example/example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)      198 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/example/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)      168 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/example/example/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      540 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/example/manage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2689 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/post_screenshot_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/postgres_metrics/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      199 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/apps.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22048 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)      282 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.866402 django-postgres-metrics-0.9.0/postgres_metrics/static/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.866402 django-postgres-metrics-0.9.0/postgres_metrics/static/postgres_metrics/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/postgres_metrics/static/postgres_metrics/css/
+-rw-r--r--   0 runner    (1001) docker     (116)      701 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/static/postgres_metrics/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (116)      256 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/static/postgres_metrics/css/rtl.css
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.866402 django-postgres-metrics-0.9.0/postgres_metrics/templates/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.870401 django-postgres-metrics-0.9.0/postgres_metrics/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (116)     1327 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.874402 django-postgres-metrics-0.9.0/postgres_metrics/templates/postgres_metrics/
+-rw-r--r--   0 runner    (1001) docker     (116)     3847 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/templates/postgres_metrics/table.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.874402 django-postgres-metrics-0.9.0/postgres_metrics/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2413 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/templatetags/postgres_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)      302 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)      756 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/postgres_metrics/views.py
+-rw-r--r--   0 runner    (1001) docker     (116)      382 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       88 2021-01-05 19:08:19.874402 django-postgres-metrics-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2247 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:19.874402 django-postgres-metrics-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4540 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3478 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/tests/test_liveserver.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17642 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4722 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3789 2021-01-05 19:08:08.000000 django-postgres-metrics-0.9.0/tests/test_views.py
```

### Comparing `django-postgres-metrics-0.8.0/.github/workflows/publish.yml` & `django-postgres-metrics-0.9.0/.github/workflows/test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-name: Publish Python Package
+name: Lint & Test
 
 on:
   push:
-    tags:
-      - "[0-9]+.[0-9]+.[0-9]+"
+    branches:
+      - master
+  pull_request:
+    branches:
+      - master
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
@@ -39,25 +42,80 @@
         run: |
           pre-commit run --all-files
   test:
     runs-on: ubuntu-latest
     name: "Test Python ${{ matrix.python-version }} & Django ${{ matrix.django-version }}"
     needs: [lint]
     services:
-      postgres:
-        image: postgres
+      postgres95:
+        image: postgres:9.5
         env:
           POSTGRES_PASSWORD: postgres
         options: >-
           --health-cmd pg_isready
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
         ports:
-          - 5432:5432
+          - 5495:5432
+      postgres96:
+        image: postgres:9.6
+        env:
+          POSTGRES_PASSWORD: postgres
+        options: >-
+          --health-cmd pg_isready
+          --health-interval 10s
+          --health-timeout 5s
+          --health-retries 5
+        ports:
+          - 5496:5432
+      postgres10:
+        image: postgres:10
+        env:
+          POSTGRES_PASSWORD: postgres
+        options: >-
+          --health-cmd pg_isready
+          --health-interval 10s
+          --health-timeout 5s
+          --health-retries 5
+        ports:
+          - 5410:5432
+      postgres11:
+        image: postgres:11
+        env:
+          POSTGRES_PASSWORD: postgres
+        options: >-
+          --health-cmd pg_isready
+          --health-interval 10s
+          --health-timeout 5s
+          --health-retries 5
+        ports:
+          - 5411:5432
+      postgres12:
+        image: postgres:12
+        env:
+          POSTGRES_PASSWORD: postgres
+        options: >-
+          --health-cmd pg_isready
+          --health-interval 10s
+          --health-timeout 5s
+          --health-retries 5
+        ports:
+          - 5412:5432
+      postgres13:
+        image: postgres:13
+        env:
+          POSTGRES_PASSWORD: postgres
+        options: >-
+          --health-cmd pg_isready
+          --health-interval 10s
+          --health-timeout 5s
+          --health-retries 5
+        ports:
+          - 5413:5432
     strategy:
       matrix:
         django-version: ["2.2", "3.0", "3.1"]
         python-version: ["3.5", "3.6", "3.7", "3.8", "3.9"]
         exclude:
           # 3.0
           - django-version: "3.0"
@@ -80,30 +138,39 @@
           restore-keys: |
             ${{ runner.os }}-pip-
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install Django~=${{ matrix.django-version }}.0
           python -m pip install '.[test]'
-      - name: Create additional DB users
-        run: |
-          psql -c "CREATE ROLE someuser WITH LOGIN PASSWORD 'somepass' CREATEDB;"
-          psql -c "CREATE ROLE otheruser WITH LOGIN PASSWORD 'otherpass' CREATEDB;"
-        env:
-          PGHOST: localhost
-          PGPASSWORD: postgres
-          PGUSER: postgres
       - name: Run tests
         run: |
           coverage run "$(command -v django-admin.py)" test --pythonpath . -v 2 --settings=tests.settings
           coverage report
+        env:
+          PG_VERSIONS: "95,96,10,11,12,13"
       - name: Upload coverage to codecov.io
         uses: codecov/codecov-action@v1
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
+      - uses: actions/upload-artifact@v2
+        with:
+          name: "screnshots-py${{ matrix.python-version }}-dj${{ matrix.django-version }}"
+          path: tests/output/
+          if-no-files-found: error
+          retention-days: 1
+      - name: Post screenshots
+        if: "${{ github.ref != 'refs/heads/master' &&  matrix.python-version == '3.9' && matrix.django-version == '3.1' }}"
+        run: |
+          python -m pip install imgbox-cli
+          imgbox --json tests/output/*.png > imgbox-response.json
+          python post_screenshot_comment.py "$(jq --raw-output .pull_request.number "$GITHUB_EVENT_PATH")" "$(readlink -f imgbox-response.json)"
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+
   docs:
     runs-on: ubuntu-latest
     needs: [lint]
     steps:
       - name: Checkout
         uses: actions/checkout@v2
       - uses: actions/setup-python@v2
@@ -115,43 +182,7 @@
           python -m pip install -r docs/requirements.txt
       - name: Generate and test API docs
         run: |
           make html
         env:
           SPHINXOPTS: "-n -v -W --keep-going"
         working-directory: ./docs
-  deploy:
-    runs-on: ubuntu-latest
-    needs: [test, docs]
-    steps:
-      - uses: actions/checkout@v2
-      - name: Set up Python
-        uses: actions/setup-python@v2
-        with:
-          python-version: "3.9"
-      - uses: actions/cache@v2
-        name: Configure pip caching
-        with:
-          path: ~/.cache/pip
-          key: ${{ runner.os }}-publish-pip-${{ hashFiles('setup.py') }}
-          restore-keys: |
-            ${{ runner.os }}-publish-pip-
-      - name: Install dependencies
-        run: |
-          pip install -U pip
-          python -m pip install setuptools wheel twine
-      - name: Publish
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
-        run: |
-          python setup.py sdist bdist_wheel
-          twine upload dist/*
-      - name: Create Release
-        uses: actions/create-release@v1
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        with:
-          tag_name: ${{ github.ref }}
-          release_name: Release ${{ github.ref }}
-          draft: false
-          prerelease: false
```

### Comparing `django-postgres-metrics-0.8.0/LICENSE` & `django-postgres-metrics-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/PKG-INFO` & `django-postgres-metrics-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postgres-metrics
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Django app that exposes a bunch of PostgreSQL database metrics.
 Home-page: https://github.com/django-postgres-metrics/django-postgres-metrics
 Author: Markus Holtermann
 Author-email: info@markusholtermann.eu
 License: BSD
 Project-URL: CI, https://github.com/django-postgres-metrics/django-postgres-metrics/actions
 Project-URL: Changelog, https://django-postgres-metrics.readthedocs.io/en/latest/changelog.html
@@ -81,15 +81,16 @@
         
         urlpatterns = [
             path('admin/postgres-metrics/', include('postgres_metrics.urls')),
             path('admin/', admin.site.urls),
         ]
         ```
         
-        This is what a metric could look like: ![Metric example](docs/source/_static/screenshot.png)
+        This is what a metric could look like:
+        ![Metric example](https://github.com/django-postgres-metrics/django-postgres-metrics/blob/master/docs/source/_static/screenshot.png)
         
         ## Security
         
         If you found or if you think you found a security issue please get in touch via
         `info+django-postgres-metrics *AT* markusholtermann *DOT* eu`.
         
         I'm working about this in my free time. I don't have time to monitor the email 24/7. But you
```

### Comparing `django-postgres-metrics-0.8.0/README.md` & `django-postgres-metrics-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
 urlpatterns = [
     path('admin/postgres-metrics/', include('postgres_metrics.urls')),
     path('admin/', admin.site.urls),
 ]
 ```
 
-This is what a metric could look like: ![Metric example](docs/source/_static/screenshot.png)
+This is what a metric could look like:
+![Metric example](https://github.com/django-postgres-metrics/django-postgres-metrics/blob/master/docs/source/_static/screenshot.png)
 
 ## Security
 
 If you found or if you think you found a security issue please get in touch via
 `info+django-postgres-metrics *AT* markusholtermann *DOT* eu`.
 
 I'm working about this in my free time. I don't have time to monitor the email 24/7. But you
```

### Comparing `django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/PKG-INFO` & `django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postgres-metrics
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Django app that exposes a bunch of PostgreSQL database metrics.
 Home-page: https://github.com/django-postgres-metrics/django-postgres-metrics
 Author: Markus Holtermann
 Author-email: info@markusholtermann.eu
 License: BSD
 Project-URL: CI, https://github.com/django-postgres-metrics/django-postgres-metrics/actions
 Project-URL: Changelog, https://django-postgres-metrics.readthedocs.io/en/latest/changelog.html
@@ -81,15 +81,16 @@
         
         urlpatterns = [
             path('admin/postgres-metrics/', include('postgres_metrics.urls')),
             path('admin/', admin.site.urls),
         ]
         ```
         
-        This is what a metric could look like: ![Metric example](docs/source/_static/screenshot.png)
+        This is what a metric could look like:
+        ![Metric example](https://github.com/django-postgres-metrics/django-postgres-metrics/blob/master/docs/source/_static/screenshot.png)
         
         ## Security
         
         If you found or if you think you found a security issue please get in touch via
         `info+django-postgres-metrics *AT* markusholtermann *DOT* eu`.
         
         I'm working about this in my free time. I don't have time to monitor the email 24/7. But you
```

### Comparing `django-postgres-metrics-0.8.0/django_postgres_metrics.egg-info/SOURCES.txt` & `django-postgres-metrics-0.9.0/django_postgres_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/Makefile` & `django-postgres-metrics-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/make.bat` & `django-postgres-metrics-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/source/_static/screenshot.png` & `django-postgres-metrics-0.9.0/docs/source/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/source/background.rst` & `django-postgres-metrics-0.9.0/docs/source/background.rst`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/source/changelog.rst` & `django-postgres-metrics-0.9.0/docs/source/changelog.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 =========
 
 .. currentmodule:: postgres_metrics
 
 Under Development
 =================
 
+0.9.0 (2021-01-05)
+==================
+
+* Added support for translatable column titles.
+
+* Added support for metrics to only be available on certain PostgreSQL versions.
+
+* Fixed an issue in the :class:`Cache Hits <metrics.CacheHits>` metric when a
+  database doesn't track those metrics.
+
 0.8.0 (2021-01-03)
 ==================
 
 * Dropped support for Django 1.11, 2.0, and 2.1.
 
   .. warning::
```

### Comparing `django-postgres-metrics-0.8.0/docs/source/conf.py` & `django-postgres-metrics-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/source/contributing/releasing.rst` & `django-postgres-metrics-0.9.0/docs/source/contributing/releasing.rst`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/source/ext.py` & `django-postgres-metrics-0.9.0/docs/source/ext.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/docs/source/getting-started.rst` & `django-postgres-metrics-0.9.0/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/example/example/settings.py` & `django-postgres-metrics-0.9.0/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/example/manage.py` & `django-postgres-metrics-0.9.0/example/manage.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/post_screenshot_comment.py` & `django-postgres-metrics-0.9.0/post_screenshot_comment.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/postgres_metrics/metrics.py` & `django-postgres-metrics-0.9.0/postgres_metrics/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,21 +137,36 @@
        <http://initd.org/psycopg/docs/connection.html#connection.dsn>`_.
 
     .. attribute:: records
 
        The rows returned by a metric for the given database.
     """
 
+    holds_data = True
+
     def __init__(self, connection, records):
         connection.ensure_connection()
         self.alias = connection.alias
         self.dsn = connection.connection.dsn
         self.records = records
 
 
+class NoMetricResult(MetricResult):
+    """
+    Internal class to pass an error message to the template when a metric is
+    not available.
+    """
+
+    holds_data = False
+
+    def __init__(self, connection, reason):
+        super().__init__(connection, [])
+        self.reason = reason
+
+
 class MetricMeta(type):
     def __new__(mcs, name, bases, attrs):
         if bases:
             # Only subclasses of `Metric`
             if not attrs.get("label"):
                 attrs["label"] = name
             if not attrs.get("slug"):
@@ -223,18 +238,35 @@
        white spaces and fix newlines. ``'\\r\\n'`` and ``'\\r'`` line breaks will
        be normalized to ``'\\n'``. Two or more consecutive occurances of
        ``'\\n'`` mark a paragraph which will be escaped and wrapped in
        ``<p></p>`` HTML tags. Further, each paragraph will call into Django's
        ``urlize()`` method to create ``<a></a>`` HTML tags around links.
     """
 
-    #: The label is what is used in the Django Admin views. Consider marking
-    #: this string as translateable.
+    #: A list of strings used as column headers in the admin. Consider making
+    #: the strings translateable. If the attribute is undefined, the column
+    #: names returned by the database will be used.
+    header_labels = None
+
+    #: The label is what is used in the Django Admin views. Consider making
+    #: this string translateable.
     label = ""
 
+    #: The maximum PostgreSQL version possible to provide the metric data.
+    #: If not explicitly specified, every PostgreSQL version is suitable. This
+    # value is checked against
+    # :attr:`django.db.backends.postgresql.base.DatabaseWrapper.pg_version`.
+    max_pg_version = None
+
+    #: The minimum PostgreSQL version necessary to provide the metric data.
+    #: If not explicitly specified, every PostgreSQL version is suitable. This
+    # value is checked against
+    # :attr:`django.db.backends.postgresql.base.DatabaseWrapper.pg_version`.
+    min_pg_version = None
+
     #: The default ordering that should be applied to the SQL query by default.
     #: This needs to be a valid ordering string as defined on
     #: :attr:`parsed_ordering`.
     ordering = ""
 
     #: A URL safe representation of the label and unique across all metrics.
     slug = ""
@@ -283,31 +315,52 @@
         :return: Returns a list of :class:`MetricResult` instances.
         :rtype: list
         """
         results = []
         for connection in connections.all():
             if connection.vendor != "postgresql":
                 continue
-            with connection.cursor() as cursor:
-                cursor.execute(self.full_sql)
-                self.headers = [
-                    MetricHeader(c.name, index, self.parsed_ordering)
-                    for index, c in enumerate(cursor.description, start=1)
-                ]
-                data = cursor.fetchall()
-            db = MetricResult(connection, data)
+            if (
+                self.min_pg_version is None
+                or connection.pg_version >= self.min_pg_version
+            ) and (
+                self.max_pg_version is None
+                or connection.pg_version <= self.max_pg_version
+            ):
+                with connection.cursor() as cursor:
+                    cursor.execute(self.full_sql)
+                    if self.header_labels is None:
+                        self.header_labels = [c.name for c in cursor.description]
+                    data = cursor.fetchall()
+                db = MetricResult(connection, data)
+            else:
+                db = NoMetricResult(
+                    connection,
+                    "This metric is not supported on this PostgreSQL version.",
+                )
             results.append(db)
         return results
 
     @cached_property
+    def headers(self):
+        """
+        A wrapper around the :attr:`header_labels` to make the tables in the
+        admin sortable.
+        """
+        return [
+            MetricHeader(label, index, self.parsed_ordering)
+            for index, label in enumerate(self.header_labels, start=1)
+        ]
+
+    @cached_property
     def parsed_ordering(self):
         """
         Turn an ordering string like ``1.5.-3.-2.6`` into the respective abstraction.
 
-        Given :attr:`ordering` as ``1.5.-3.-2.6`` return a lis of 2-tuples
+        Given :attr:`ordering` as ``1.5.-3.-2.6`` return a list of 2-tuples
         like ``[('', 1), ('', 5), ('-', 3), ('-', 2), ('', 6)]``.
         """
         if self.ordering:
             return [
                 ("-" if o.startswith("-") else "", int(o.lstrip("-")))
                 for o in self.ordering.split(".")
             ]
@@ -382,14 +435,15 @@
     cache. Generally you want your database to have a cache hit rate of about
     99%.
 
     (Source:
     http://www.craigkerstiens.com/2012/10/01/understanding-postgres-performance/)
     """
 
+    header_labels = [_("Reads"), _("Hits"), _("Ratio")]
     label = _("Cache Hits")
     slug = "cache-hits"
     sql = """
         WITH cache AS (
             SELECT
                 sum(heap_blks_read) heap_read,
                 sum(heap_blks_hit) heap_hit,
@@ -406,35 +460,36 @@
         FROM
             cache
         {ORDER_BY}
         ;
     """
 
     def get_record_item_style(self, record, item, index):
-        if index == 2 and item != "N/A":
+        if index == 2 and item is not None and item != "N/A":
             ratio = float(item)
             if ratio < 0.95:
                 return "critical"
             if ratio < 0.99:
                 return "warning"
             return "ok"
 
 
 registry.register(CacheHits)
 
 
 class IndexSize(Metric):
+    header_labels = [_("Table"), _("Index"), _("Size")]
     label = _("Index Size")
     ordering = "1.2"
     slugify = "index-size"
     sql = """
         SELECT
-            relname "table",
-            indexrelname "index",
-            pg_size_pretty(pg_relation_size(indexrelid)) size
+            relname,
+            indexrelname,
+            pg_size_pretty(pg_relation_size(indexrelid))
         FROM
             pg_stat_user_indexes
         {ORDER_BY}
         ;
     """
 
 
@@ -449,36 +504,42 @@
     was used in comparison to the total number of sequential and index scans on
     the table.
 
     Similarly, the "index scan on table" shows how often an index was used
     compared to the other indexes on the table.
     """
 
+    header_labels = [
+        _("Table"),
+        _("Index"),
+        _("Index Scan over Sequential Scan"),
+        _("Index Scan on table"),
+    ]
     label = _("Detailed Index Usage")
     ordering = "1.2"
     slug = "detailed-index-usage"
     sql = """
         SELECT
-            t.relname "table",
-            i.indexrelname "index",
+            t.relname,
+            i.indexrelname,
             CASE t.seq_scan + t.idx_scan
                 WHEN 0
                     THEN round(0.0, 2)
                 ELSE
                     round(
                         (100::float * i.idx_scan / (t.seq_scan + t.idx_scan))::numeric,
                         2::int
                     )
-            END "index scan over sequential scan",
+            END,
             CASE t.idx_scan
                 WHEN 0
                     THEN round(0.0, 2)
                 ELSE
                     round((100::float * i.idx_scan / t.idx_scan)::numeric, 2::int)
-            END "index scan on table"
+            END
         FROM
             pg_stat_user_tables t
         INNER JOIN
             pg_stat_user_indexes i
             ON t.relid = i.relid
         {ORDER_BY}
         ;
@@ -497,25 +558,26 @@
     up by some other id or on values that you're commonly filtering on such as
     created_at fields.
 
     (Source:
     http://www.craigkerstiens.com/2012/10/01/understanding-postgres-performance/)
     """
 
+    header_labels = [_("Table"), _("Index used (in %)"), _("Num rows")]
     label = _("Index Usage")
     ordering = "2"
     slug = "index-usage"
     sql = """
         SELECT
             relname,
             round(
                 (100::float * idx_scan / (seq_scan + idx_scan))::numeric,
                 2::int
-            ) percent_of_times_index_used,
-            n_live_tup rows_in_table
+            ),
+            n_live_tup
         FROM
             pg_stat_user_tables
         WHERE
             seq_scan + idx_scan > 0
         {ORDER_BY}
         ;
     """
@@ -532,21 +594,22 @@
                 return "ok"
 
 
 registry.register(IndexUsage)
 
 
 class TableSize(Metric):
+    header_labels = [_("Table"), _("Size")]
     label = _("Table Size")
     ordering = "1"
     slugify = "table-size"
     sql = """
         SELECT
-            relname "table",
-            pg_size_pretty(pg_relation_size(relid)) size
+            relname,
+            pg_size_pretty(pg_relation_size(relid))
         FROM
             pg_stat_user_tables
         {ORDER_BY}
         ;
     """
 
 
@@ -587,35 +650,44 @@
 
 
 registry.register(AvailableExtensions)
 
 
 class SequenceUsage(Metric):
     """
-    Show the sequence usage within a PostgreSQL database. A usage over 90%
-    will be marked as red, and a usage over 75% will be marked as yellow.
+    Show the sequence usage within a PostgreSQL database. A usage over 75%
+    will be marked as red, and a usage over 50% will be marked as yellow.
     """
 
+    header_labels = [
+        _("Table"),
+        _("Column"),
+        _("Sequence"),
+        _("Last value"),
+        _("Max value"),
+        _("Used (in %)"),
+    ]
     label = _("Sequence Usage")
+    min_pg_version = 100000
     ordering = "-6.1.2.3"
     slug = "sequence-usage"
     sql = """
         SELECT
-            tabcls.relname "table",
-            attrib.attname "column",
-            seqcls.relname "sequence",
-            seq.last_value "last_value",
-            seq.max_value "max_value",
+            tabcls.relname,
+            attrib.attname,
+            seqcls.relname,
+            seq.last_value,
+            seq.max_value,
             round(
                 (
                     100::float * COALESCE(seq.last_value, 0)
                     / (seq.max_value - seq.start_value + 1)
                 )::numeric,
                 2::int
-            ) percent_sequence_used
+            )
         FROM
             pg_class AS seqcls
         INNER JOIN
             pg_sequences AS seq
             ON seqcls.relname = seq.sequencename
         INNER JOIN
             pg_depend AS dep
```

### Comparing `django-postgres-metrics-0.8.0/postgres_metrics/static/postgres_metrics/css/base.css` & `django-postgres-metrics-0.9.0/postgres_metrics/static/postgres_metrics/css/base.css`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/postgres_metrics/templates/admin/index.html` & `django-postgres-metrics-0.9.0/postgres_metrics/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/postgres_metrics/templates/postgres_metrics/table.html` & `django-postgres-metrics-0.9.0/postgres_metrics/templates/postgres_metrics/table.html`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,22 @@
                             <div class="text"><a href="?o={{ header.url_primary }}">{{ header }}</a></div>
                             <div class="clear"></div>
                         </th>
                         {% endfor %}
                     </tr>
                 </thead>
                 <tbody>
-                    {% for record in result.records %}
-                    <tr class="{% cycle 'row1' 'row2' %} {% record_style %}">{% for item in record %}<td class="{% record_item_style %}">{{ item }}</td>{% endfor %}</tr>
-                    {% endfor %}
-                    {% resetcycle %}
+                    {% if result.holds_data %}
+                        {% for record in result.records %}
+                        <tr class="{% cycle 'row1' 'row2' %} {% record_style %}">{% for item in record %}<td class="{% record_item_style %}">{{ item }}</td>{% endfor %}</tr>
+                        {% endfor %}
+                        {% resetcycle %}
+                    {% else %}
+                        <tr class="pgm-critical"><td colspan="{{ metric.headers|length }}">{{ result.reason }}</td></tr>
+                    {% endif %}
                 </tbody>
             </table>
         </div>
     </div>
     {% endfor %}
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -24,9 +24,10 @@
 {% if header.sort_priority > 0 %}
  %}">
  {{ header.sort_priority }}
  %}">
 {% endif %}
 {{_header_}}
 {{ item }}
+{{ result.reason }}
 {% endfor %}
 {% endblock %}
```

### Comparing `django-postgres-metrics-0.8.0/postgres_metrics/templatetags/postgres_metrics.py` & `django-postgres-metrics-0.9.0/postgres_metrics/templatetags/postgres_metrics.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/postgres_metrics/views.py` & `django-postgres-metrics-0.9.0/postgres_metrics/views.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/setup.py` & `django-postgres-metrics-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/tests/settings.py` & `django-postgres-metrics-0.9.0/tests/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -68,34 +68,64 @@
 ]
 
 WSGI_APPLICATION = "wsgi.application"
 
 # Database
 # https://docs.djangoproject.com/en/dev/ref/settings/#databases
 
-DATABASES = {
-    "default": {
-        "ENGINE": "django.db.backends.postgresql",
-        "HOST": "localhost",
-        "NAME": "somedb",
-        "USER": "someuser",
-        "PASSWORD": "somepass",
-    },
-    "second": {
-        "ENGINE": "django.db.backends.postgresql",
-        "HOST": "localhost",
-        "NAME": "otherdb",
-        "USER": "otheruser",
-        "PASSWORD": "otherpass",
-    },
-    "sqlite": {
-        "ENGINE": "django.db.backends.sqlite3",
-        "NAME": ":memory:",
-    },
-}
+pg_services = os.getenv("PG_VERSIONS") or ""
+pg_versions = list(map(int, filter(str, map(str.strip, pg_services.split(",")))))
+
+if not pg_versions:
+    DATABASES = {
+        "default": {
+            "ENGINE": "django.db.backends.postgresql",
+            "HOST": "localhost",
+            "PORT": 5432,
+            "NAME": "somedb",
+            "USER": "someuser",
+            "PASSWORD": "somepass",
+        },
+        "second": {
+            "ENGINE": "django.db.backends.postgresql",
+            "HOST": "localhost",
+            "PORT": 5432,
+            "NAME": "otherdb",
+            "USER": "otheruser",
+            "PASSWORD": "otherpass",
+        },
+        "sqlite": {
+            "ENGINE": "django.db.backends.sqlite3",
+            "NAME": ":memory:",
+        },
+    }
+else:
+    DATABASES = {
+        "default": {
+            "ENGINE": "django.db.backends.postgresql",
+            "HOST": "localhost",
+            "PORT": 5400 + pg_versions[0],
+            "NAME": "pg%d" % pg_versions[0],
+            "USER": "postgres",
+            "PASSWORD": "postgres",
+        },
+        "sqlite": {
+            "ENGINE": "django.db.backends.sqlite3",
+            "NAME": ":memory:",
+        },
+    }
+    for pg_version in pg_versions[1:]:
+        DATABASES["postgres%d" % pg_version] = {
+            "ENGINE": "django.db.backends.postgresql",
+            "HOST": "localhost",
+            "PORT": 5400 + pg_version,
+            "NAME": "pg%d" % pg_version,
+            "USER": "postgres",
+            "PASSWORD": "postgres",
+        }
 
 # Password validation
 # https://docs.djangoproject.com/en/dev/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
     {
         "NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator",  # noqa
```

### Comparing `django-postgres-metrics-0.8.0/tests/test_liveserver.py` & `django-postgres-metrics-0.9.0/tests/test_liveserver.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/tests/test_metrics.py` & `django-postgres-metrics-0.9.0/tests/test_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.db import connections
 from django.test import SimpleTestCase, TestCase
 
 from postgres_metrics.metrics import (
     AvailableExtensions,
     CacheHits,
@@ -49,15 +50,15 @@
         registry.register(FooBar)
         registry.register(BarFoo)
         registry.register(LoremIpsum)
         self.assertEqual(registry.sorted, [BarFoo, FooBar, LoremIpsum])
 
 
 class MetricTest(TestCase):
-    databases = {"default", "second"}
+    databases = {name for name in settings.DATABASES if name != "sqlite"}
 
     def test_required_arguments(self):
         msg = (
             'Metric "MissingSQLMetric" is missing a "sql" attribute or "sql" is empty.'
         )
         with self.assertRaisesMessage(ImproperlyConfigured, msg):
 
@@ -153,22 +154,23 @@
         self.assertEqual(
             metric.headers,
             [
                 MetricHeader("app", 1, [("-", 2), ("", 1)]),
                 MetricHeader("count", 2, [("-", 2), ("", 1)]),
             ],
         )
-        # Two databases
-        self.assertEqual(len(data), 2)
-        # 4 apps
-        self.assertEqual(len(data[0].records), 4)
-        self.assertEqual(len(data[1].records), 4)
-        # 2 columns
-        self.assertEqual(len(data[0].records[0]), 2)
-        self.assertEqual(len(data[1].records[0]), 2)
+
+        num_databases = len(settings.DATABASES) - 1  # One SQLite3 database
+        self.assertEqual(len(data), num_databases)
+        for i in range(num_databases):
+            with self.subTest(db_number=i):
+                # 4 apps
+                self.assertEqual(len(data[i].records), 4)
+                # 2 columns
+                self.assertEqual(len(data[i].records[0]), 2)
 
     def test_get_record_style(self):
         class MyMetric(Metric):
             sql = "SELECT 1;"
 
         self.assertEqual(MyMetric().get_record_style(None), "")
 
@@ -335,37 +337,36 @@
 
     def test_urls_from_desc_non_primary_sorting_later_column_make_toggle_url(self):
         header = MetricHeader("H", 4, [("-", 2), ("", 3), ("-", 4)])
         self.assertEqual(header.url_toggle, "-2.3.4")
 
 
 class MetricResultTest(TestCase):
-    databases = {"default", "second"}
-
-    def test_default(self):
-        result = MetricResult(connections["default"], [("foo", 1, 2), ("bar", 3, 4)])
-        self.assertEqual(result.alias, "default")
-        self.assertEqual(
-            sorted(result.dsn.split()),
-            sorted(
-                "user=someuser host=localhost password=xxx dbname=test_somedb".split()
-            ),
-        )
-        self.assertEqual(result.records, [("foo", 1, 2), ("bar", 3, 4)])
+    databases = {name for name in settings.DATABASES if name != "sqlite"}
 
-    def test_second(self):
-        result = MetricResult(connections["second"], [("foo", 1, 2), ("bar", 3, 4)])
-        self.assertEqual(result.alias, "second")
-        self.assertEqual(
-            sorted(result.dsn.split()),
-            sorted(
-                "user=otheruser host=localhost password=xxx dbname=test_otherdb".split()
-            ),
-        )
-        self.assertEqual(result.records, [("foo", 1, 2), ("bar", 3, 4)])
+    def test_db(self):
+        for dbname, dbcfg in settings.DATABASES.items():
+            if dbname == "sqlite":
+                continue
+
+            with self.subTest(dbname=dbname):
+                result = MetricResult(
+                    connections[dbname], [("foo", 1, 2), ("bar", 3, 4)]
+                )
+                self.assertEqual(result.alias, dbname)
+                self.assertEqual(
+                    sorted(result.dsn.split()),
+                    sorted(
+                        (
+                            "host=localhost port=%d user=%s password=xxx dbname=%s"
+                            % (dbcfg["PORT"], dbcfg["USER"], dbcfg["NAME"])
+                        ).split()
+                    ),
+                )
+                self.assertEqual(result.records, [("foo", 1, 2), ("bar", 3, 4)])
 
 
 class StyleAssertionMixin:
     def assertRecordStylesEqual(self, metric_class, records, expecteds):
         metric = metric_class()
         for record, expected in zip(records, expecteds):
             with self.subTest(record=record):
@@ -476,15 +477,15 @@
     def test_repr(self):
         self.assertEqual(
             repr(self.metric_class()), '<Metric "%s">' % self.metric_class.label
         )
 
     tc_name = "Dynamic_" + metric_class.__name__ + "Test"
     attrs = {
-        "databases": {"default", "second"},
+        "databases": {name for name in settings.DATABASES if name != "sqlite"},
         "metric_class": metric_class,
         "test_get_data_default_ordering": test_get_data_default_ordering,
         "test_get_data_no_ordering": test_get_data_no_ordering,
         "test_get_data_explicit_ordering": test_get_data_explicit_ordering,
         "test_repr": test_repr,
     }
     cls = type(tc_name, (TestCase,), attrs)
```

### Comparing `django-postgres-metrics-0.8.0/tests/test_templatetags.py` & `django-postgres-metrics-0.9.0/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-postgres-metrics-0.8.0/tests/test_views.py` & `django-postgres-metrics-0.9.0/tests/test_views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from django.conf import settings
 from django.conf.urls import include, url as path
 from django.contrib import admin
 from django.contrib.auth.models import Permission, User
 from django.test import TestCase, override_settings
 
 urlpatterns = [
     path("^postgres-metrics/", include("postgres_metrics.urls")),
     path("^admin/", admin.site.urls),
 ]
 
 
 @override_settings(ROOT_URLCONF=__name__)
 class TestMetricsView(TestCase):
-    databases = {"default", "second"}
+    databases = {name for name in settings.DATABASES if name != "sqlite"}
 
     @classmethod
     def setUpTestData(cls):
         cls.user = User.objects.create_user("user", "user@local")
         cls.superuser = User.objects.create_superuser(
             "superuser", "superuser@local", "secret"
         )
```

