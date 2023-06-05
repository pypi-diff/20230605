# Comparing `tmp/django-extensions-3.2.1.tar.gz` & `tmp/django-extensions-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-extensions-3.2.1.tar", last modified: Fri Sep  9 11:09:29 2022, max compression
+gzip compressed data, was "django-extensions-3.2.3.tar", last modified: Mon Jun  5 17:08:43 2023, max compression
```

## Comparing `django-extensions-3.2.1.tar` & `django-extensions-3.2.3.tar`

### file list

```diff
@@ -1,598 +1,466 @@
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.437248 django-extensions-3.2.1/
--rw-r--r--   0 sqrbass    (501) staff       (20)    44221 2022-09-09 11:08:09.000000 django-extensions-3.2.1/CHANGELOG.md
--rw-r--r--   0 sqrbass    (501) staff       (20)     1057 2017-08-09 17:53:20.000000 django-extensions-3.2.1/LICENSE
--rw-r--r--   0 sqrbass    (501) staff       (20)      350 2019-03-11 09:24:14.000000 django-extensions-3.2.1/MANIFEST.in
--rw-r--r--   0 sqrbass    (501) staff       (20)     1257 2020-09-11 12:44:34.000000 django-extensions-3.2.1/Makefile
--rw-r--r--   0 sqrbass    (501) staff       (20)     6178 2022-09-09 11:09:29.437339 django-extensions-3.2.1/PKG-INFO
--rw-r--r--   0 sqrbass    (501) staff       (20)     4527 2022-09-09 08:54:00.000000 django-extensions-3.2.1/README.rst
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.330184 django-extensions-3.2.1/django_extensions/
--rw-r--r--   0 sqrbass    (501) staff       (20)      545 2022-09-09 11:07:31.000000 django-extensions-3.2.1/django_extensions/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.331438 django-extensions-3.2.1/django_extensions/admin/
--rw-r--r--   0 sqrbass    (501) staff       (20)     6853 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/admin/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1819 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/admin/filter.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3191 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/admin/widgets.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      171 2020-04-21 13:29:06.000000 django-extensions-3.2.1/django_extensions/apps.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.331667 django-extensions-3.2.1/django_extensions/auth/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2019-11-02 20:24:08.000000 django-extensions-3.2.1/django_extensions/auth/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      488 2019-11-02 20:28:36.000000 django-extensions-3.2.1/django_extensions/auth/mixins.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    10644 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/collision_resolvers.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1930 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/compat.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.322672 django-extensions-3.2.1/django_extensions/conf/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.332737 django-extensions-3.2.1/django_extensions/conf/app_template/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/app_template/__init__.py.tmpl
--rw-r--r--   0 sqrbass    (501) staff       (20)       55 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/app_template/forms.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.332872 django-extensions-3.2.1/django_extensions/conf/app_template/migrations/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/app_template/migrations/__init__.py.tmpl
--rw-r--r--   0 sqrbass    (501) staff       (20)       57 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/app_template/models.py.tmpl
--rw-r--r--   0 sqrbass    (501) staff       (20)       69 2020-05-26 08:25:15.000000 django-extensions-3.2.1/django_extensions/conf/app_template/urls.py.tmpl
--rw-r--r--   0 sqrbass    (501) staff       (20)       26 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/app_template/views.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.313760 django-extensions-3.2.1/django_extensions/conf/command_template/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.332969 django-extensions-3.2.1/django_extensions/conf/command_template/management/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/command_template/management/__init__.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.333176 django-extensions-3.2.1/django_extensions/conf/command_template/management/commands/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/command_template/management/commands/__init__.py.tmpl
--rw-r--r--   0 sqrbass    (501) staff       (20)      306 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/command_template/management/commands/sample.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.313909 django-extensions-3.2.1/django_extensions/conf/jobs_template/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.333405 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/__init__.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.333533 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/daily/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/daily/__init__.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.333622 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/hourly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/hourly/__init__.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.333709 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/monthly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/monthly/__init__.py.tmpl
--rw-r--r--   0 sqrbass    (501) staff       (20)      178 2017-12-25 22:41:09.000000 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/sample.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.333790 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/weekly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/weekly/__init__.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.333869 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/yearly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/jobs_template/jobs/yearly/__init__.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.322734 django-extensions-3.2.1/django_extensions/conf/template_tags_template/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.334030 django-extensions-3.2.1/django_extensions/conf/template_tags_template/templatetags/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/template_tags_template/templatetags/__init__.py.tmpl
--rw-r--r--   0 sqrbass    (501) staff       (20)       59 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/conf/template_tags_template/templatetags/sample.py.tmpl
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.334250 django-extensions-3.2.1/django_extensions/db/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/db/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.334814 django-extensions-3.2.1/django_extensions/db/fields/
--rw-r--r--   0 sqrbass    (501) staff       (20)    20790 2022-09-09 10:41:45.000000 django-extensions-3.2.1/django_extensions/db/fields/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2862 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/db/fields/json.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3811 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/db/models.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2291 2019-02-26 12:52:19.000000 django-extensions-3.2.1/django_extensions/import_subclasses.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.335031 django-extensions-3.2.1/django_extensions/jobs/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.335437 django-extensions-3.2.1/django_extensions/jobs/daily/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/daily/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      646 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/jobs/daily/cache_cleanup.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      388 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/daily/daily_cleanup.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.335633 django-extensions-3.2.1/django_extensions/jobs/hourly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/hourly/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.335707 django-extensions-3.2.1/django_extensions/jobs/minutely/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/minutely/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.335781 django-extensions-3.2.1/django_extensions/jobs/monthly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/monthly/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.335857 django-extensions-3.2.1/django_extensions/jobs/weekly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/weekly/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.335930 django-extensions-3.2.1/django_extensions/jobs/yearly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/jobs/yearly/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324642 django-extensions-3.2.1/django_extensions/locale/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323352 django-extensions-3.2.1/django_extensions/locale/ar/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.336004 django-extensions-3.2.1/django_extensions/locale/ar/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     3126 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323444 django-extensions-3.2.1/django_extensions/locale/da/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.336442 django-extensions-3.2.1/django_extensions/locale/da/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)      797 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1667 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323532 django-extensions-3.2.1/django_extensions/locale/de/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.336832 django-extensions-3.2.1/django_extensions/locale/de/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1227 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1755 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323621 django-extensions-3.2.1/django_extensions/locale/el/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.337114 django-extensions-3.2.1/django_extensions/locale/el/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1581 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     2116 2020-03-04 23:07:46.000000 django-extensions-3.2.1/django_extensions/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323711 django-extensions-3.2.1/django_extensions/locale/en/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.337387 django-extensions-3.2.1/django_extensions/locale/en/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)      367 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     2229 2020-03-04 23:06:01.000000 django-extensions-3.2.1/django_extensions/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323797 django-extensions-3.2.1/django_extensions/locale/es/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.337668 django-extensions-3.2.1/django_extensions/locale/es/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1260 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1788 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323884 django-extensions-3.2.1/django_extensions/locale/fr/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.337907 django-extensions-3.2.1/django_extensions/locale/fr/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)      743 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1930 2017-08-09 17:53:20.000000 django-extensions-3.2.1/django_extensions/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.323974 django-extensions-3.2.1/django_extensions/locale/hu/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.338156 django-extensions-3.2.1/django_extensions/locale/hu/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1242 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1770 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324061 django-extensions-3.2.1/django_extensions/locale/id/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.338408 django-extensions-3.2.1/django_extensions/locale/id/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1508 2020-08-10 07:19:05.000000 django-extensions-3.2.1/django_extensions/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     2243 2020-08-10 07:19:05.000000 django-extensions-3.2.1/django_extensions/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324150 django-extensions-3.2.1/django_extensions/locale/it/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.338664 django-extensions-3.2.1/django_extensions/locale/it/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1247 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1775 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324236 django-extensions-3.2.1/django_extensions/locale/ja/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.338996 django-extensions-3.2.1/django_extensions/locale/ja/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1397 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1925 2017-07-05 14:18:57.000000 django-extensions-3.2.1/django_extensions/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324325 django-extensions-3.2.1/django_extensions/locale/pl/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.339258 django-extensions-3.2.1/django_extensions/locale/pl/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     2002 2020-08-10 07:19:05.000000 django-extensions-3.2.1/django_extensions/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     2788 2020-08-10 07:19:05.000000 django-extensions-3.2.1/django_extensions/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324412 django-extensions-3.2.1/django_extensions/locale/pt/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.345213 django-extensions-3.2.1/django_extensions/locale/pt/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1262 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1790 2017-07-05 14:34:26.000000 django-extensions-3.2.1/django_extensions/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324504 django-extensions-3.2.1/django_extensions/locale/pt_BR/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.345496 django-extensions-3.2.1/django_extensions/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1310 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     2082 2017-07-05 14:36:16.000000 django-extensions-3.2.1/django_extensions/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324592 django-extensions-3.2.1/django_extensions/locale/ro/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.345731 django-extensions-3.2.1/django_extensions/locale/ro/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1352 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     1891 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.324678 django-extensions-3.2.1/django_extensions/locale/ru/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.345962 django-extensions-3.2.1/django_extensions/locale/ru/LC_MESSAGES/
--rw-r--r--   0 sqrbass    (501) staff       (20)     2009 2021-11-07 15:20:18.000000 django-extensions-3.2.1/django_extensions/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 sqrbass    (501) staff       (20)     3820 2019-05-31 15:05:13.000000 django-extensions-3.2.1/django_extensions/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.346157 django-extensions-3.2.1/django_extensions/logging/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/logging/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1126 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/logging/filters.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.348416 django-extensions-3.2.1/django_extensions/management/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/management/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1431 2020-04-21 10:35:32.000000 django-extensions-3.2.1/django_extensions/management/base.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      907 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/color.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.362243 django-extensions-3.2.1/django_extensions/management/commands/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/management/commands/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    11791 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/commands/admin_generator.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1555 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/clean_pyc.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1486 2019-02-26 12:35:07.000000 django-extensions-3.2.1/django_extensions/management/commands/clear_cache.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1273 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/compile_pyc.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3780 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/create_command.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2457 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/create_jobs.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2855 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/create_template_tags.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     7241 2020-08-10 07:22:18.000000 django-extensions-3.2.1/django_extensions/management/commands/delete_squashed_migrations.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2737 2020-04-27 16:33:58.000000 django-extensions-3.2.1/django_extensions/management/commands/describe_form.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     8450 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/drop_test_database.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    27698 2022-09-09 10:47:52.000000 django-extensions-3.2.1/django_extensions/management/commands/dumpscript.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5565 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/commands/export_emails.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      695 2019-03-11 09:24:14.000000 django-extensions-3.2.1/django_extensions/management/commands/find_template.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      971 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/generate_password.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      484 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/generate_secret_key.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    14685 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/graph_models.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6038 2020-04-21 10:35:32.000000 django-extensions-3.2.1/django_extensions/management/commands/list_model_info.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2602 2020-05-23 21:44:26.000000 django-extensions-3.2.1/django_extensions/management/commands/list_signals.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2977 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/mail_debug.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6747 2022-09-09 10:41:45.000000 django-extensions-3.2.1/django_extensions/management/commands/managestate.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     9552 2019-05-02 15:38:26.000000 django-extensions-3.2.1/django_extensions/management/commands/merge_model_instances.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2716 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/commands/notes.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    15513 2021-11-07 16:12:46.000000 django-extensions-3.2.1/django_extensions/management/commands/pipchecker.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2640 2020-08-10 07:22:18.000000 django-extensions-3.2.1/django_extensions/management/commands/print_settings.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2144 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/commands/print_user_for_session.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      659 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/raise_test_exception.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     7748 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/reset_db.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2859 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/reset_schema.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1987 2020-05-23 21:44:26.000000 django-extensions-3.2.1/django_extensions/management/commands/runjob.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3384 2020-05-23 21:44:26.000000 django-extensions-3.2.1/django_extensions/management/commands/runjobs.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    11625 2020-08-31 11:46:13.000000 django-extensions-3.2.1/django_extensions/management/commands/runprofileserver.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    11952 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/runscript.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    22604 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/runserver_plus.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2821 2021-05-02 08:56:08.000000 django-extensions-3.2.1/django_extensions/management/commands/set_default_site.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3874 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/set_fake_emails.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1764 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/set_fake_passwords.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    22891 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/shell_plus.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3907 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/commands/show_template_tags.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     9218 2022-09-09 10:54:23.000000 django-extensions-3.2.1/django_extensions/management/commands/show_urls.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     4262 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/sqlcreate.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    63924 2022-09-09 10:54:23.000000 django-extensions-3.2.1/django_extensions/management/commands/sqldiff.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6074 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/management/commands/sqldsn.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    15720 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/commands/sync_s3.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     9771 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/commands/syncdata.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1787 2019-03-15 10:43:35.000000 django-extensions-3.2.1/django_extensions/management/commands/unreferenced_files.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2488 2022-09-09 10:41:45.000000 django-extensions-3.2.1/django_extensions/management/commands/update_permissions.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3627 2020-04-21 10:35:32.000000 django-extensions-3.2.1/django_extensions/management/commands/validate_templates.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     4446 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/debug_cursor.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5360 2020-04-21 10:35:32.000000 django-extensions-3.2.1/django_extensions/management/email_notifications.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5070 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/jobs.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    18655 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/management/modelviz.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1506 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/mysql.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      324 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/notebook_extension.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    15410 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/shells.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      307 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/management/signals.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1758 2020-08-10 07:34:58.000000 django-extensions-3.2.1/django_extensions/management/technical_response.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2259 2020-04-07 13:32:14.000000 django-extensions-3.2.1/django_extensions/management/utils.py
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/models.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.362504 django-extensions-3.2.1/django_extensions/mongodb/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/mongodb/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.362934 django-extensions-3.2.1/django_extensions/mongodb/fields/
--rw-r--r--   0 sqrbass    (501) staff       (20)     9342 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/mongodb/fields/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2158 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/mongodb/fields/json.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2405 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/mongodb/models.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1120 2021-11-07 15:14:59.000000 django-extensions-3.2.1/django_extensions/settings.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.325013 django-extensions-3.2.1/django_extensions/static/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.325151 django-extensions-3.2.1/django_extensions/static/django_extensions/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.363147 django-extensions-3.2.1/django_extensions/static/django_extensions/css/
--rw-r--r--   0 sqrbass    (501) staff       (20)      740 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/static/django_extensions/css/jquery.autocomplete.css
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.363375 django-extensions-3.2.1/django_extensions/static/django_extensions/img/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1553 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/static/django_extensions/img/indicator.gif
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.365771 django-extensions-3.2.1/django_extensions/static/django_extensions/js/
--rw-r--r--   0 sqrbass    (501) staff       (20)     2911 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/static/django_extensions/js/jquery.ajaxQueue.js
--rw-r--r--   0 sqrbass    (501) staff       (20)    36679 2018-06-07 13:44:40.000000 django-extensions-3.2.1/django_extensions/static/django_extensions/js/jquery.autocomplete.js
--rw-r--r--   0 sqrbass    (501) staff       (20)     1820 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/static/django_extensions/js/jquery.bgiframe.js
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.325247 django-extensions-3.2.1/django_extensions/templates/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.325425 django-extensions-3.2.1/django_extensions/templates/django_extensions/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.325374 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.366351 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/django2018/
--rw-r--r--   0 sqrbass    (501) staff       (20)      846 2021-09-09 11:59:34.000000 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/django2018/digraph.dot
--rw-r--r--   0 sqrbass    (501) staff       (20)     1875 2019-05-17 12:33:45.000000 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/django2018/label.dot
--rw-r--r--   0 sqrbass    (501) staff       (20)      589 2019-05-13 11:43:36.000000 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/django2018/relation.dot
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.366785 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/original/
--rw-r--r--   0 sqrbass    (501) staff       (20)      851 2021-09-09 11:59:34.000000 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/original/digraph.dot
--rw-r--r--   0 sqrbass    (501) staff       (20)     1697 2018-09-12 19:58:20.000000 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/original/label.dot
--rw-r--r--   0 sqrbass    (501) staff       (20)      591 2017-08-09 17:53:20.000000 django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/original/relation.dot
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.366907 django-extensions-3.2.1/django_extensions/templates/django_extensions/widgets/
--rw-r--r--   0 sqrbass    (501) staff       (20)     2032 2019-07-29 12:31:25.000000 django-extensions-3.2.1/django_extensions/templates/django_extensions/widgets/foreignkey_searchinput.html
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.367673 django-extensions-3.2.1/django_extensions/templatetags/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/django_extensions/templatetags/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      596 2019-01-23 12:49:58.000000 django-extensions-3.2.1/django_extensions/templatetags/debugger_tags.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3224 2019-02-26 12:50:46.000000 django-extensions-3.2.1/django_extensions/templatetags/highlighting.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1751 2019-02-26 12:50:56.000000 django-extensions-3.2.1/django_extensions/templatetags/indent_text.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3172 2022-09-09 08:54:00.000000 django-extensions-3.2.1/django_extensions/templatetags/syntax_color.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1925 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/templatetags/widont.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.368389 django-extensions-3.2.1/django_extensions/utils/
--rw-r--r--   0 sqrbass    (501) staff       (20)       70 2020-07-14 11:05:36.000000 django-extensions-3.2.1/django_extensions/utils/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      155 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/utils/deprecation.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    10177 2020-08-10 07:20:56.000000 django-extensions-3.2.1/django_extensions/utils/dia2django.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1952 2020-07-14 11:05:36.000000 django-extensions-3.2.1/django_extensions/utils/internal_ips.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3820 2022-07-08 20:17:38.000000 django-extensions-3.2.1/django_extensions/validators.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.330795 django-extensions-3.2.1/django_extensions.egg-info/
--rw-r--r--   0 sqrbass    (501) staff       (20)     6178 2022-09-09 11:09:29.000000 django-extensions-3.2.1/django_extensions.egg-info/PKG-INFO
--rw-r--r--   0 sqrbass    (501) staff       (20)    20314 2022-09-09 11:09:29.000000 django-extensions-3.2.1/django_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)        1 2022-09-09 11:09:29.000000 django-extensions-3.2.1/django_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)       12 2022-09-09 11:09:29.000000 django-extensions-3.2.1/django_extensions.egg-info/requires.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)       18 2022-09-09 11:09:29.000000 django-extensions-3.2.1/django_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.376129 django-extensions-3.2.1/docs/
--rw-r--r--   0 sqrbass    (501) staff       (20)     1023 2019-05-20 20:23:44.000000 django-extensions-3.2.1/docs/AUTHORS
--rw-r--r--   0 sqrbass    (501) staff       (20)     2375 2016-09-06 14:17:16.000000 django-extensions-3.2.1/docs/Makefile
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.376359 django-extensions-3.2.1/docs/__pycache__/
--rw-r--r--   0 sqrbass    (501) staff       (20)      730 2020-09-11 12:40:53.000000 django-extensions-3.2.1/docs/__pycache__/conf.cpython-38.pyc
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.376518 django-extensions-3.2.1/docs/_build/
--rw-r--r--   0 sqrbass    (501) staff       (20)     6148 2018-02-16 16:10:36.000000 django-extensions-3.2.1/docs/_build/.DS_Store
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.383367 django-extensions-3.2.1/docs/_build/doctrees/
--rw-r--r--   0 sqrbass    (501) staff       (20)    15147 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/admin_extensions.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    10654 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/admin_generator.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    43395 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/command_extensions.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    11597 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/command_signals.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     4935 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/create_template_tags.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     4938 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/debugger_tags.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     6542 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/delete_squashed_migrations.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    14125 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/dumpscript.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    88281 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 sqrbass    (501) staff       (20)    15499 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/export_emails.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    24009 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/field_extensions.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     5605 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/generate_password.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    20478 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/graph_models.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    12558 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/index.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    11104 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/installation_instructions.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    16429 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/jobs_scheduling.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    11065 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/list_model_info.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     4060 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/list_signals.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     5478 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/merge_model_instances.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    16063 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/model_extensions.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     6683 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/permissions.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    12612 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/print_settings.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     8677 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/reset_db.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    17773 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/runprofileserver.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    27790 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/runscript.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    37851 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/runserver_plus.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    57901 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/shell_plus.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     9335 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/sqlcreate.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     6836 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/sqldiff.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     6203 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/sqldsn.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     9997 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/sync_s3.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     6564 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/syncdata.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     6211 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/utilities.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)    10973 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/validate_templates.doctree
--rw-r--r--   0 sqrbass    (501) staff       (20)     7020 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/doctrees/validators.doctree
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.390435 django-extensions-3.2.1/docs/_build/html/
--rw-r--r--   0 sqrbass    (501) staff       (20)      230 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/.buildinfo
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.401822 django-extensions-3.2.1/docs/_build/html/_sources/
--rw-r--r--   0 sqrbass    (501) staff       (20)     3325 2021-01-31 22:56:40.000000 django-extensions-3.2.1/docs/_build/html/_sources/admin_extensions.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     3642 2018-11-16 07:59:51.000000 django-extensions-3.2.1/docs/_build/html/_sources/admin_generator.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     6756 2021-01-31 22:56:40.000000 django-extensions-3.2.1/docs/_build/html/_sources/command_extensions.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     3011 2017-08-09 17:53:20.000000 django-extensions-3.2.1/docs/_build/html/_sources/command_signals.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      534 2019-02-07 16:00:19.000000 django-extensions-3.2.1/docs/_build/html/_sources/create_template_tags.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      527 2020-07-14 11:31:21.000000 django-extensions-3.2.1/docs/_build/html/_sources/debugger_tags.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     1078 2016-12-12 15:50:52.000000 django-extensions-3.2.1/docs/_build/html/_sources/delete_squashed_migrations.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     2524 2017-08-09 17:53:20.000000 django-extensions-3.2.1/docs/_build/html/_sources/dumpscript.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     3422 2021-02-07 21:05:29.000000 django-extensions-3.2.1/docs/_build/html/_sources/export_emails.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     4811 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/_build/html/_sources/field_extensions.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      635 2018-03-07 12:35:55.000000 django-extensions-3.2.1/docs/_build/html/_sources/generate_password.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     4570 2021-01-31 22:56:40.000000 django-extensions-3.2.1/docs/_build/html/_sources/graph_models.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     2320 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     1991 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/_build/html/_sources/installation_instructions.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     2566 2020-07-14 11:31:11.000000 django-extensions-3.2.1/docs/_build/html/_sources/jobs_scheduling.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     2109 2020-06-29 08:20:08.000000 django-extensions-3.2.1/docs/_build/html/_sources/list_model_info.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      319 2020-05-23 21:44:26.000000 django-extensions-3.2.1/docs/_build/html/_sources/list_signals.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      881 2017-12-25 22:11:15.000000 django-extensions-3.2.1/docs/_build/html/_sources/merge_model_instances.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     2528 2020-07-14 11:31:45.000000 django-extensions-3.2.1/docs/_build/html/_sources/model_extensions.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     1212 2021-02-07 20:59:27.000000 django-extensions-3.2.1/docs/_build/html/_sources/permissions.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     3433 2020-08-10 07:22:18.000000 django-extensions-3.2.1/docs/_build/html/_sources/print_settings.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     2068 2020-11-16 19:19:37.000000 django-extensions-3.2.1/docs/_build/html/_sources/reset_db.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     3831 2020-11-16 19:21:12.000000 django-extensions-3.2.1/docs/_build/html/_sources/runprofileserver.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     5967 2020-08-31 11:18:20.000000 django-extensions-3.2.1/docs/_build/html/_sources/runscript.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     9402 2020-08-10 07:22:18.000000 django-extensions-3.2.1/docs/_build/html/_sources/runserver_plus.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)    14294 2020-04-29 11:44:13.000000 django-extensions-3.2.1/docs/_build/html/_sources/shell_plus.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     1480 2020-09-17 07:59:49.000000 django-extensions-3.2.1/docs/_build/html/_sources/sqlcreate.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     1071 2016-09-06 14:17:16.000000 django-extensions-3.2.1/docs/_build/html/_sources/sqldiff.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      809 2020-08-10 07:19:05.000000 django-extensions-3.2.1/docs/_build/html/_sources/sqldsn.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     2075 2016-09-06 14:17:16.000000 django-extensions-3.2.1/docs/_build/html/_sources/sync_s3.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      877 2020-04-21 07:21:17.000000 django-extensions-3.2.1/docs/_build/html/_sources/syncdata.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      739 2020-07-14 10:56:10.000000 django-extensions-3.2.1/docs/_build/html/_sources/utilities.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     1991 2020-03-06 11:51:52.000000 django-extensions-3.2.1/docs/_build/html/_sources/validate_templates.rst.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)     1017 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/_build/html/_sources/validators.rst.txt
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.405440 django-extensions-3.2.1/docs/_build/html/_static/
--rw-r--r--   0 sqrbass    (501) staff       (20)    13647 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/_static/basic.css
--rw-r--r--   0 sqrbass    (501) staff       (20)     4256 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/_static/classic.css
--rw-r--r--   0 sqrbass    (501) staff       (20)       28 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/default.css
--rw-r--r--   0 sqrbass    (501) staff       (20)     9416 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0 sqrbass    (501) staff       (20)      355 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 sqrbass    (501) staff       (20)      286 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/file.png
--rw-r--r--   0 sqrbass    (501) staff       (20)   287630 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 sqrbass    (501) staff       (20)    89476 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/jquery.js
--rw-r--r--   0 sqrbass    (501) staff       (20)    10847 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0 sqrbass    (501) staff       (20)       90 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 sqrbass    (501) staff       (20)       90 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 sqrbass    (501) staff       (20)     4837 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0 sqrbass    (501) staff       (20)    16323 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 sqrbass    (501) staff       (20)     4803 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/_static/sidebar.js
--rw-r--r--   0 sqrbass    (501) staff       (20)    35168 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 sqrbass    (501) staff       (20)    12140 2021-02-07 20:57:49.000000 django-extensions-3.2.1/docs/_build/html/_static/underscore.js
--rw-r--r--   0 sqrbass    (501) staff       (20)    12264 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/admin_extensions.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    21896 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/admin_generator.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    26691 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/command_extensions.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    13961 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/command_signals.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     6125 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/create_template_tags.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     6034 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/debugger_tags.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     6017 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/delete_squashed_migrations.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     9901 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/dumpscript.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    11906 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/export_emails.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    17468 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/field_extensions.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     5974 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/generate_password.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     2780 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/genindex.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    12264 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/graph_models.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    13965 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/index.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     8435 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/installation_instructions.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    12147 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/jobs_scheduling.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     9027 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/list_model_info.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     5244 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/list_signals.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     5804 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/merge_model_instances.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    10553 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/model_extensions.html
--rw-r--r--   0 sqrbass    (501) staff       (20)      719 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/objects.inv
--rw-r--r--   0 sqrbass    (501) staff       (20)     7718 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/permissions.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     9162 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/print_settings.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     9135 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/reset_db.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    10423 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/runprofileserver.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    16736 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/runscript.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    19952 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/runserver_plus.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     3124 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/search.html
--rw-r--r--   0 sqrbass    (501) staff       (20)    29313 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/searchindex.js
--rw-r--r--   0 sqrbass    (501) staff       (20)    36098 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/shell_plus.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     7424 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/sqlcreate.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     6429 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/sqldiff.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     6509 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/sqldsn.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     8843 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/sync_s3.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     6298 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/syncdata.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     6219 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/utilities.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     9878 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/validate_templates.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     8049 2021-02-07 21:05:32.000000 django-extensions-3.2.1/docs/_build/html/validators.html
--rw-r--r--   0 sqrbass    (501) staff       (20)     3325 2021-01-31 22:56:40.000000 django-extensions-3.2.1/docs/admin_extensions.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     3642 2018-11-16 07:59:51.000000 django-extensions-3.2.1/docs/admin_generator.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     6889 2022-07-11 20:41:45.000000 django-extensions-3.2.1/docs/command_extensions.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     3011 2017-08-09 17:53:20.000000 django-extensions-3.2.1/docs/command_signals.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     6470 2022-09-09 11:07:38.000000 django-extensions-3.2.1/docs/conf.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      534 2019-02-07 16:00:19.000000 django-extensions-3.2.1/docs/create_template_tags.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1058 2020-06-29 20:30:11.000000 django-extensions-3.2.1/docs/creating_release.txt
--rw-r--r--   0 sqrbass    (501) staff       (20)      527 2020-07-14 11:31:21.000000 django-extensions-3.2.1/docs/debugger_tags.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1078 2016-12-12 15:50:52.000000 django-extensions-3.2.1/docs/delete_squashed_migrations.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2524 2017-08-09 17:53:20.000000 django-extensions-3.2.1/docs/dumpscript.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     3422 2021-02-07 21:06:16.000000 django-extensions-3.2.1/docs/export_emails.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     4811 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/field_extensions.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)      635 2018-03-07 12:35:55.000000 django-extensions-3.2.1/docs/generate_password.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     4914 2022-07-08 20:17:38.000000 django-extensions-3.2.1/docs/graph_models.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2320 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/index.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1991 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/installation_instructions.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2566 2020-07-14 11:31:11.000000 django-extensions-3.2.1/docs/jobs_scheduling.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2109 2020-06-29 08:20:08.000000 django-extensions-3.2.1/docs/list_model_info.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)      319 2020-05-23 21:44:26.000000 django-extensions-3.2.1/docs/list_signals.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2434 2022-07-08 20:17:38.000000 django-extensions-3.2.1/docs/managestate.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)      881 2017-12-25 22:11:15.000000 django-extensions-3.2.1/docs/merge_model_instances.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2528 2020-07-14 11:31:45.000000 django-extensions-3.2.1/docs/model_extensions.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1242 2021-05-02 08:56:08.000000 django-extensions-3.2.1/docs/permissions.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     3433 2020-08-10 07:22:18.000000 django-extensions-3.2.1/docs/print_settings.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2068 2020-11-16 19:19:37.000000 django-extensions-3.2.1/docs/reset_db.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     3831 2020-11-16 19:21:12.000000 django-extensions-3.2.1/docs/runprofileserver.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     5967 2020-08-31 11:18:20.000000 django-extensions-3.2.1/docs/runscript.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     9496 2022-09-09 08:54:00.000000 django-extensions-3.2.1/docs/runserver_plus.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)    14818 2022-02-04 16:48:39.000000 django-extensions-3.2.1/docs/shell_plus.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1480 2020-09-17 07:59:49.000000 django-extensions-3.2.1/docs/sqlcreate.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1071 2016-09-06 14:17:16.000000 django-extensions-3.2.1/docs/sqldiff.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2098 2022-07-08 20:17:38.000000 django-extensions-3.2.1/docs/sqldsn.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     2075 2016-09-06 14:17:16.000000 django-extensions-3.2.1/docs/sync_s3.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)      877 2020-04-21 07:21:17.000000 django-extensions-3.2.1/docs/syncdata.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)      739 2020-07-14 10:56:10.000000 django-extensions-3.2.1/docs/utilities.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1991 2022-09-09 10:47:52.000000 django-extensions-3.2.1/docs/validate_templates.rst
--rw-r--r--   0 sqrbass    (501) staff       (20)     1017 2020-07-14 11:29:56.000000 django-extensions-3.2.1/docs/validators.rst
--rwxr-xr-x   0 sqrbass    (501) staff       (20)      282 2020-08-10 07:20:56.000000 django-extensions-3.2.1/manage.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      776 2022-09-09 11:09:29.437616 django-extensions-3.2.1/setup.cfg
--rw-r--r--   0 sqrbass    (501) staff       (20)     5184 2022-09-09 08:54:00.000000 django-extensions-3.2.1/setup.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.410143 django-extensions-3.2.1/tests/
--rw-r--r--   0 sqrbass    (501) staff       (20)      173 2020-09-11 12:51:43.000000 django-extensions-3.2.1/tests/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.410336 django-extensions-3.2.1/tests/auth/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2019-11-02 20:24:08.000000 django-extensions-3.2.1/tests/auth/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1628 2019-11-02 20:28:36.000000 django-extensions-3.2.1/tests/auth/test_mixins.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.410913 django-extensions-3.2.1/tests/collisions/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2017-10-31 13:28:07.000000 django-extensions-3.2.1/tests/collisions/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      147 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/collisions/apps.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1067 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/collisions/models.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.326115 django-extensions-3.2.1/tests/db/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.411324 django-extensions-3.2.1/tests/db/fields/
--rw-r--r--   0 sqrbass    (501) staff       (20)     5363 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/db/fields/test_uniq_field_mixin.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5521 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/db/fields/test_uniq_field_mixin_compat.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.326199 django-extensions-3.2.1/tests/jobs/
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.411534 django-extensions-3.2.1/tests/jobs/daily/
--rw-r--r--   0 sqrbass    (501) staff       (20)      894 2019-03-27 22:25:44.000000 django-extensions-3.2.1/tests/jobs/daily/test_cache_cleanup.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.412158 django-extensions-3.2.1/tests/management/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/management/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.422338 django-extensions-3.2.1/tests/management/commands/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/management/commands/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      229 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/management/commands/error_raising_command.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.423629 django-extensions-3.2.1/tests/management/commands/shell_plus_tests/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-02-21 20:28:25.000000 django-extensions-3.2.1/tests/management/commands/shell_plus_tests/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    16015 2020-10-26 23:34:32.000000 django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_collision_resolver.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5666 2019-02-24 20:54:37.000000 django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_import_subclasses.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5500 2021-11-07 15:14:59.000000 django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_shell_plus.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2270 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_utils.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1774 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_admin_generator.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2600 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/management/commands/test_clear_cache.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3856 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_create_command.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2640 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_create_jobs.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1569 2020-10-26 23:29:12.000000 django-extensions-3.2.1/tests/management/commands/test_create_template_tags.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     7916 2021-02-07 20:42:20.000000 django-extensions-3.2.1/tests/management/commands/test_delete_squashed_migrations.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2203 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_describe_form.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    12422 2021-04-05 11:21:32.000000 django-extensions-3.2.1/tests/management/commands/test_drop_test_database.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3637 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_export_emails.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      379 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_generate_password.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      653 2021-02-07 20:42:20.000000 django-extensions-3.2.1/tests/management/commands/test_generate_secret_key.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6970 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/management/commands/test_graph_models.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      863 2020-05-23 21:44:26.000000 django-extensions-3.2.1/tests/management/commands/test_list_signals.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      332 2021-02-07 20:54:18.000000 django-extensions-3.2.1/tests/management/commands/test_mail_debug.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3792 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/management/commands/test_managestate.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2125 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/management/commands/test_notes.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5712 2021-02-07 20:42:20.000000 django-extensions-3.2.1/tests/management/commands/test_pipchecker.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1674 2020-08-10 07:22:18.000000 django-extensions-3.2.1/tests/management/commands/test_print_settings.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3593 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_print_user_for_session.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      324 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/management/commands/test_raise_test_exception.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     8134 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_reset_db.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2331 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_reset_schema.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3083 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_runjob.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      388 2020-09-06 22:34:14.000000 django-extensions-3.2.1/tests/management/commands/test_runserver_plus.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3980 2021-05-02 08:56:08.000000 django-extensions-3.2.1/tests/management/commands/test_set_default_site.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6258 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_set_fake_emails.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2473 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_set_fake_passwords.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1045 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_show_template_tags.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6437 2022-09-09 10:54:23.000000 django-extensions-3.2.1/tests/management/commands/test_show_urls.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     5106 2020-10-26 23:09:21.000000 django-extensions-3.2.1/tests/management/commands/test_sqlcreate.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     8772 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/management/commands/test_sqldsn.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     8508 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_sync_s3.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3383 2021-02-07 20:42:20.000000 django-extensions-3.2.1/tests/management/commands/test_syncdata.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1875 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_unreferenced_files.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2518 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_update_permissions.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2367 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/commands/test_validate_templates.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3295 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/management/test_email_notifications.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2221 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/management/test_modelviz.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       83 2018-04-19 20:51:45.000000 django-extensions-3.2.1/tests/pythonrc.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      886 2020-09-11 12:51:48.000000 django-extensions-3.2.1/tests/runner.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.427898 django-extensions-3.2.1/tests/templatetags/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2019-02-21 20:35:33.000000 django-extensions-3.2.1/tests/templatetags/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2375 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/templatetags/test_highlighting.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1661 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/templatetags/test_indent_text.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3654 2021-04-05 11:21:32.000000 django-extensions-3.2.1/tests/templatetags/test_syntax_color.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3059 2022-09-09 08:54:00.000000 django-extensions-3.2.1/tests/test_admin_filter.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1584 2019-10-02 20:07:16.000000 django-extensions-3.2.1/tests/test_admin_widgets.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     9842 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_autoslug_fields.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2392 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_clean_pyc.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      688 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_color.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      946 2019-05-12 13:19:29.000000 django-extensions-3.2.1/tests/test_compat.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2009 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_compile_pyc.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3475 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_dumpscript.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      681 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_find_template.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     4260 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_json_field.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2556 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/test_logging_filters.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    20080 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/test_management_command.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1590 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/test_models.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1162 2019-05-18 16:36:32.000000 django-extensions-3.2.1/tests/test_modificationdatetime_fields.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      143 2018-02-21 20:28:25.000000 django-extensions-3.2.1/tests/test_module_in_project_dir.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1800 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_parse_mysql_cnf.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3575 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/test_randomchar_field.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    10183 2020-09-01 20:45:48.000000 django-extensions-3.2.1/tests/test_runscript.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2987 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/test_runserver.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1180 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_shortuuid_field.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6141 2022-09-09 10:54:23.000000 django-extensions-3.2.1/tests/test_sqldiff.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      485 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/test_template_rendering.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1190 2020-08-10 07:20:56.000000 django-extensions-3.2.1/tests/test_templatetags.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      583 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/test_timestamped_model.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     6225 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/test_validators.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      517 2019-04-29 15:37:28.000000 django-extensions-3.2.1/tests/test_version.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.432109 django-extensions-3.2.1/tests/testapp/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2022-09-09 08:54:00.000000 django-extensions-3.2.1/tests/testapp/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      115 2018-09-10 21:03:30.000000 django-extensions-3.2.1/tests/testapp/admin.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      119 2020-09-17 19:10:00.000000 django-extensions-3.2.1/tests/testapp/apps.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      160 2018-02-21 20:28:25.000000 django-extensions-3.2.1/tests/testapp/classes_to_include.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.432359 django-extensions-3.2.1/tests/testapp/derived_classes_for_testing/
--rw-r--r--   0 sqrbass    (501) staff       (20)      143 2018-02-21 20:28:25.000000 django-extensions-3.2.1/tests/testapp/derived_classes_for_testing/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      182 2019-02-24 21:09:57.000000 django-extensions-3.2.1/tests/testapp/derived_classes_for_testing/test_module.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      309 2020-08-31 12:40:04.000000 django-extensions-3.2.1/tests/testapp/factories.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      395 2020-04-21 10:35:32.000000 django-extensions-3.2.1/tests/testapp/fields.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       96 2018-06-15 18:26:25.000000 django-extensions-3.2.1/tests/testapp/file_with_utf8_notes.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       53 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/testapp/file_without_utf8_notes.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.432681 django-extensions-3.2.1/tests/testapp/jobs/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2017-12-25 22:39:26.000000 django-extensions-3.2.1/tests/testapp/jobs/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.432930 django-extensions-3.2.1/tests/testapp/jobs/daily/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-01-10 22:24:10.000000 django-extensions-3.2.1/tests/testapp/jobs/daily/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      248 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/testapp/jobs/daily/test_daily_job.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.433140 django-extensions-3.2.1/tests/testapp/jobs/hourly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-01-10 22:24:10.000000 django-extensions-3.2.1/tests/testapp/jobs/hourly/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      253 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/testapp/jobs/hourly/test_hourly_job.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.433488 django-extensions-3.2.1/tests/testapp/jobs/monthly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-01-10 22:24:10.000000 django-extensions-3.2.1/tests/testapp/jobs/monthly/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      258 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/testapp/jobs/monthly/test_monthly_job.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      202 2018-01-10 22:24:10.000000 django-extensions-3.2.1/tests/testapp/jobs/sample.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      196 2017-12-25 22:55:38.000000 django-extensions-3.2.1/tests/testapp/jobs/sample_job.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.433714 django-extensions-3.2.1/tests/testapp/jobs/weekly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-01-10 22:24:10.000000 django-extensions-3.2.1/tests/testapp/jobs/weekly/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      253 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/testapp/jobs/weekly/test_weekly_job.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.433937 django-extensions-3.2.1/tests/testapp/jobs/yearly/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-01-10 22:24:10.000000 django-extensions-3.2.1/tests/testapp/jobs/yearly/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      253 2020-08-10 07:20:31.000000 django-extensions-3.2.1/tests/testapp/jobs/yearly/test_yearly_job.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.434060 django-extensions-3.2.1/tests/testapp/management/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2019-03-27 22:25:44.000000 django-extensions-3.2.1/tests/testapp/management/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.434218 django-extensions-3.2.1/tests/testapp/management/commands/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2019-03-27 22:25:44.000000 django-extensions-3.2.1/tests/testapp/management/commands/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      277 2019-03-27 22:26:03.000000 django-extensions-3.2.1/tests/testapp/management/commands/test_email_notification_command.py
--rw-r--r--   0 sqrbass    (501) staff       (20)    15455 2022-09-09 10:54:23.000000 django-extensions-3.2.1/tests/testapp/models.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.434887 django-extensions-3.2.1/tests/testapp/scripts/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/testapp/scripts/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      196 2017-10-23 23:46:00.000000 django-extensions-3.2.1/tests/testapp/scripts/directory_checker_script.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       55 2017-09-12 12:57:57.000000 django-extensions-3.2.1/tests/testapp/scripts/error_script.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       76 2019-02-24 21:10:29.000000 django-extensions-3.2.1/tests/testapp/scripts/invalid_import_script.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       44 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/testapp/scripts/sample_script.py
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2017-09-12 12:57:57.000000 django-extensions-3.2.1/tests/testapp/scripts/script_no_run_function.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     3003 2021-04-19 17:42:12.000000 django-extensions-3.2.1/tests/testapp/settings.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.435040 django-extensions-3.2.1/tests/testapp/templatetags/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-08-23 15:03:02.000000 django-extensions-3.2.1/tests/testapp/templatetags/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      146 2018-08-23 15:18:22.000000 django-extensions-3.2.1/tests/testapp/templatetags/dummy_tags.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     1165 2022-07-08 20:17:38.000000 django-extensions-3.2.1/tests/testapp/urls.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.436026 django-extensions-3.2.1/tests/testapp_with_appconfig/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2022-09-09 08:54:00.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       89 2018-08-23 15:17:52.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/admin.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      147 2018-08-23 15:17:32.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/apps.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.436142 django-extensions-3.2.1/tests/testapp_with_appconfig/migrations/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-08-23 15:03:02.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/migrations/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       83 2018-08-23 15:18:00.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/models.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.436296 django-extensions-3.2.1/tests/testapp_with_appconfig/templatetags/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2018-08-23 15:03:02.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/templatetags/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      166 2018-08-23 15:18:31.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/templatetags/dummy_tags_appconfig.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       86 2018-08-23 15:18:05.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/tests.py
--rw-r--r--   0 sqrbass    (501) staff       (20)       89 2018-08-23 15:18:03.000000 django-extensions-3.2.1/tests/testapp_with_appconfig/views.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.436599 django-extensions-3.2.1/tests/testapp_with_no_models_file/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/testapp_with_no_models_file/__init__.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.436976 django-extensions-3.2.1/tests/testapp_with_no_models_file/scripts/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2017-10-23 23:46:00.000000 django-extensions-3.2.1/tests/testapp_with_no_models_file/scripts/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      102 2017-10-23 23:46:00.000000 django-extensions-3.2.1/tests/testapp_with_no_models_file/scripts/other_directory_checker_script.py
--rw-r--r--   0 sqrbass    (501) staff       (20)      184 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/testapp_with_no_models_file/teslacar.py
-drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2022-09-09 11:09:29.437174 django-extensions-3.2.1/tests/testapp_with_template_errors/
--rw-r--r--   0 sqrbass    (501) staff       (20)        0 2016-09-06 14:17:16.000000 django-extensions-3.2.1/tests/testapp_with_template_errors/__init__.py
--rw-r--r--   0 sqrbass    (501) staff       (20)     2576 2022-09-09 10:41:16.000000 django-extensions-3.2.1/tox.ini
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.506213 django-extensions-3.2.3/
+-rw-r--r--   0 sqrbass    (501) staff       (20)    44940 2023-06-05 17:05:46.000000 django-extensions-3.2.3/CHANGELOG.md
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1057 2023-06-05 12:54:40.000000 django-extensions-3.2.3/LICENSE
+-rw-r--r--   0 sqrbass    (501) staff       (20)      350 2023-06-05 12:54:40.000000 django-extensions-3.2.3/MANIFEST.in
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1257 2023-06-05 12:54:40.000000 django-extensions-3.2.3/Makefile
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6272 2023-06-05 17:08:43.506283 django-extensions-3.2.3/PKG-INFO
+-rw-r--r--   0 sqrbass    (501) staff       (20)     4530 2023-06-05 17:05:46.000000 django-extensions-3.2.3/README.rst
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.465431 django-extensions-3.2.3/django_extensions/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      545 2023-06-05 17:07:52.000000 django-extensions-3.2.3/django_extensions/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.466328 django-extensions-3.2.3/django_extensions/admin/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6853 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/admin/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1819 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/admin/filter.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3191 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/admin/widgets.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      171 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/apps.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.466537 django-extensions-3.2.3/django_extensions/auth/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/auth/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      488 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/auth/mixins.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    10644 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/collision_resolvers.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1930 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/compat.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.456419 django-extensions-3.2.3/django_extensions/conf/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467046 django-extensions-3.2.3/django_extensions/conf/app_template/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/app_template/__init__.py.tmpl
+-rw-r--r--   0 sqrbass    (501) staff       (20)       55 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/app_template/forms.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467153 django-extensions-3.2.3/django_extensions/conf/app_template/migrations/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/app_template/migrations/__init__.py.tmpl
+-rw-r--r--   0 sqrbass    (501) staff       (20)       57 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/app_template/models.py.tmpl
+-rw-r--r--   0 sqrbass    (501) staff       (20)       69 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/app_template/urls.py.tmpl
+-rw-r--r--   0 sqrbass    (501) staff       (20)       26 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/app_template/views.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.455846 django-extensions-3.2.3/django_extensions/conf/command_template/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467260 django-extensions-3.2.3/django_extensions/conf/command_template/management/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/command_template/management/__init__.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467468 django-extensions-3.2.3/django_extensions/conf/command_template/management/commands/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/command_template/management/commands/__init__.py.tmpl
+-rw-r--r--   0 sqrbass    (501) staff       (20)      306 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/command_template/management/commands/sample.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.456028 django-extensions-3.2.3/django_extensions/conf/jobs_template/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467684 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/__init__.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467789 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/daily/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/daily/__init__.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467882 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/hourly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/hourly/__init__.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.467977 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/monthly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/monthly/__init__.py.tmpl
+-rw-r--r--   0 sqrbass    (501) staff       (20)      178 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/sample.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.468067 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/weekly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/weekly/__init__.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.468159 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/yearly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/jobs_template/jobs/yearly/__init__.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.456467 django-extensions-3.2.3/django_extensions/conf/template_tags_template/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.468337 django-extensions-3.2.3/django_extensions/conf/template_tags_template/templatetags/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/template_tags_template/templatetags/__init__.py.tmpl
+-rw-r--r--   0 sqrbass    (501) staff       (20)       59 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/conf/template_tags_template/templatetags/sample.py.tmpl
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.468607 django-extensions-3.2.3/django_extensions/db/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/db/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.468886 django-extensions-3.2.3/django_extensions/db/fields/
+-rw-r--r--   0 sqrbass    (501) staff       (20)    20792 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/db/fields/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2862 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/db/fields/json.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3811 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/db/models.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2296 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/import_subclasses.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.468995 django-extensions-3.2.3/django_extensions/jobs/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.469291 django-extensions-3.2.3/django_extensions/jobs/daily/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/daily/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      646 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/daily/cache_cleanup.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      388 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/daily/daily_cleanup.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.469396 django-extensions-3.2.3/django_extensions/jobs/hourly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/hourly/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.469482 django-extensions-3.2.3/django_extensions/jobs/minutely/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/minutely/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.469571 django-extensions-3.2.3/django_extensions/jobs/monthly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/monthly/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.469661 django-extensions-3.2.3/django_extensions/jobs/weekly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/weekly/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.469752 django-extensions-3.2.3/django_extensions/jobs/yearly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/jobs/yearly/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.459457 django-extensions-3.2.3/django_extensions/locale/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.457361 django-extensions-3.2.3/django_extensions/locale/ar/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.469843 django-extensions-3.2.3/django_extensions/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3126 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.457470 django-extensions-3.2.3/django_extensions/locale/da/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.470057 django-extensions-3.2.3/django_extensions/locale/da/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      797 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1667 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.457587 django-extensions-3.2.3/django_extensions/locale/de/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.470277 django-extensions-3.2.3/django_extensions/locale/de/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1227 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1755 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.457695 django-extensions-3.2.3/django_extensions/locale/el/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.470484 django-extensions-3.2.3/django_extensions/locale/el/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1581 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2116 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.457838 django-extensions-3.2.3/django_extensions/locale/en/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.470705 django-extensions-3.2.3/django_extensions/locale/en/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      367 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2229 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.457994 django-extensions-3.2.3/django_extensions/locale/es/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.470927 django-extensions-3.2.3/django_extensions/locale/es/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1260 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1788 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.458153 django-extensions-3.2.3/django_extensions/locale/fr/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.471137 django-extensions-3.2.3/django_extensions/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      743 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1931 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.458305 django-extensions-3.2.3/django_extensions/locale/hu/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.471341 django-extensions-3.2.3/django_extensions/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1242 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1770 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.458410 django-extensions-3.2.3/django_extensions/locale/id/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.471544 django-extensions-3.2.3/django_extensions/locale/id/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1508 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2243 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.458521 django-extensions-3.2.3/django_extensions/locale/it/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.471754 django-extensions-3.2.3/django_extensions/locale/it/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1247 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1775 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.458639 django-extensions-3.2.3/django_extensions/locale/ja/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.471968 django-extensions-3.2.3/django_extensions/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1397 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1925 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.458757 django-extensions-3.2.3/django_extensions/locale/pl/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.472178 django-extensions-3.2.3/django_extensions/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2002 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2788 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.458957 django-extensions-3.2.3/django_extensions/locale/pt/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.472388 django-extensions-3.2.3/django_extensions/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1262 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1790 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.459191 django-extensions-3.2.3/django_extensions/locale/pt_BR/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.472610 django-extensions-3.2.3/django_extensions/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1310 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2082 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.459363 django-extensions-3.2.3/django_extensions/locale/ro/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.472857 django-extensions-3.2.3/django_extensions/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1352 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1891 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.459526 django-extensions-3.2.3/django_extensions/locale/ru/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.473090 django-extensions-3.2.3/django_extensions/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2009 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3820 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.473327 django-extensions-3.2.3/django_extensions/logging/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/logging/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1126 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/logging/filters.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.474743 django-extensions-3.2.3/django_extensions/management/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1431 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/base.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      907 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/color.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.480376 django-extensions-3.2.3/django_extensions/management/commands/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    11791 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/admin_generator.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1555 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/clean_pyc.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1487 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/clear_cache.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1273 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/compile_pyc.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3780 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/create_command.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2457 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/create_jobs.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2855 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/create_template_tags.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     7241 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/delete_squashed_migrations.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2737 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/describe_form.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     8731 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/drop_test_database.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    27672 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/dumpscript.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5565 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/export_emails.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      695 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/find_template.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      971 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/generate_password.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      484 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/generate_secret_key.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    14685 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/graph_models.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6035 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/list_model_info.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2602 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/list_signals.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2977 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/mail_debug.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6747 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/managestate.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     9552 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/merge_model_instances.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2716 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/notes.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    15381 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/pipchecker.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2640 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/print_settings.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2144 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/print_user_for_session.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      659 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/raise_test_exception.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     8030 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/reset_db.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2859 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/reset_schema.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1987 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/runjob.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3384 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/runjobs.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    11625 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/runprofileserver.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    11952 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/runscript.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    24539 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/runserver_plus.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2821 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/set_default_site.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3874 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/set_fake_emails.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1764 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/set_fake_passwords.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    22889 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/shell_plus.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3908 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/show_template_tags.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     9218 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/show_urls.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     4262 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/sqlcreate.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    63926 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/commands/sqldiff.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6074 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/sqldsn.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    15720 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/sync_s3.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     9771 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/syncdata.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1787 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/unreferenced_files.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2488 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/update_permissions.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3627 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/commands/validate_templates.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     4386 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/debug_cursor.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5360 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/email_notifications.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5070 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/jobs.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    18624 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/management/modelviz.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1506 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/mysql.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      324 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/notebook_extension.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    15410 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/shells.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      307 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/signals.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1758 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/technical_response.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2259 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/management/utils.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/models.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.480613 django-extensions-3.2.3/django_extensions/mongodb/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/mongodb/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.480846 django-extensions-3.2.3/django_extensions/mongodb/fields/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     9344 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/mongodb/fields/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2158 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/mongodb/fields/json.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2405 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/mongodb/models.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1120 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/settings.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.459980 django-extensions-3.2.3/django_extensions/static/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.460157 django-extensions-3.2.3/django_extensions/static/django_extensions/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.480980 django-extensions-3.2.3/django_extensions/static/django_extensions/css/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      740 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/static/django_extensions/css/jquery.autocomplete.css
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.481111 django-extensions-3.2.3/django_extensions/static/django_extensions/img/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1553 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/static/django_extensions/img/indicator.gif
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.481505 django-extensions-3.2.3/django_extensions/static/django_extensions/js/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2800 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/static/django_extensions/js/jquery.ajaxQueue.js
+-rw-r--r--   0 sqrbass    (501) staff       (20)    36679 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/static/django_extensions/js/jquery.autocomplete.js
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1821 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/static/django_extensions/js/jquery.bgiframe.js
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.460268 django-extensions-3.2.3/django_extensions/templates/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.460524 django-extensions-3.2.3/django_extensions/templates/django_extensions/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.460438 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.481898 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/django2018/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      846 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/django2018/digraph.dot
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1875 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/django2018/label.dot
+-rw-r--r--   0 sqrbass    (501) staff       (20)      589 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/django2018/relation.dot
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.482275 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/original/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      851 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/original/digraph.dot
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1697 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/original/label.dot
+-rw-r--r--   0 sqrbass    (501) staff       (20)      591 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/original/relation.dot
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.482546 django-extensions-3.2.3/django_extensions/templates/django_extensions/widgets/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2032 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templates/django_extensions/widgets/foreignkey_searchinput.html
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.483389 django-extensions-3.2.3/django_extensions/templatetags/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templatetags/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      596 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templatetags/debugger_tags.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3086 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/templatetags/highlighting.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1751 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templatetags/indent_text.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3173 2023-06-05 17:05:46.000000 django-extensions-3.2.3/django_extensions/templatetags/syntax_color.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1925 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/templatetags/widont.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.484071 django-extensions-3.2.3/django_extensions/utils/
+-rw-r--r--   0 sqrbass    (501) staff       (20)       70 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/utils/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      155 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/utils/deprecation.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    10177 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/utils/dia2django.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1952 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/utils/internal_ips.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3820 2023-06-05 12:54:40.000000 django-extensions-3.2.3/django_extensions/validators.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.465999 django-extensions-3.2.3/django_extensions.egg-info/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6272 2023-06-05 17:08:43.000000 django-extensions-3.2.3/django_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 sqrbass    (501) staff       (20)    15091 2023-06-05 17:08:43.000000 django-extensions-3.2.3/django_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 sqrbass    (501) staff       (20)        1 2023-06-05 17:08:43.000000 django-extensions-3.2.3/django_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 sqrbass    (501) staff       (20)       12 2023-06-05 17:08:43.000000 django-extensions-3.2.3/django_extensions.egg-info/requires.txt
+-rw-r--r--   0 sqrbass    (501) staff       (20)       18 2023-06-05 17:08:43.000000 django-extensions-3.2.3/django_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.489226 django-extensions-3.2.3/docs/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1024 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/AUTHORS
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2375 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/Makefile
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3325 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/admin_extensions.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3642 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/admin_generator.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6901 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/command_extensions.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3011 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/command_signals.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6470 2023-06-05 17:08:19.000000 django-extensions-3.2.3/docs/conf.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      534 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/create_template_tags.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1058 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/creating_release.txt
+-rw-r--r--   0 sqrbass    (501) staff       (20)      527 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/debugger_tags.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1078 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/delete_squashed_migrations.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2524 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/dumpscript.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3423 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/export_emails.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     4811 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/field_extensions.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)      635 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/generate_password.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     4916 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/graph_models.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2321 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/index.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1991 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/installation_instructions.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2566 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/jobs_scheduling.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2109 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/list_model_info.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)      319 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/list_signals.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2434 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/managestate.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)      881 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/merge_model_instances.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2528 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/model_extensions.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1242 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/permissions.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3433 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/print_settings.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2068 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/reset_db.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3666 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/runprofileserver.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5967 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/runscript.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     9572 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/runserver_plus.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)    14819 2023-06-05 17:05:46.000000 django-extensions-3.2.3/docs/shell_plus.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1480 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/sqlcreate.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1071 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/sqldiff.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2109 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/sqldsn.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2075 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/sync_s3.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)      877 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/syncdata.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)      739 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/utilities.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1991 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/validate_templates.rst
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1017 2023-06-05 12:54:40.000000 django-extensions-3.2.3/docs/validators.rst
+-rwxr-xr-x   0 sqrbass    (501) staff       (20)      282 2023-06-05 12:54:40.000000 django-extensions-3.2.3/manage.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      776 2023-06-05 17:08:43.506697 django-extensions-3.2.3/setup.cfg
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5275 2023-06-05 17:05:46.000000 django-extensions-3.2.3/setup.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.492976 django-extensions-3.2.3/tests/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      173 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.493216 django-extensions-3.2.3/tests/auth/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/auth/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1628 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/auth/test_mixins.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.493631 django-extensions-3.2.3/tests/collisions/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/collisions/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      147 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/collisions/apps.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1067 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/collisions/models.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.461238 django-extensions-3.2.3/tests/db/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.493898 django-extensions-3.2.3/tests/db/fields/
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5363 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/db/fields/test_uniq_field_mixin.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5521 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/db/fields/test_uniq_field_mixin_compat.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.461537 django-extensions-3.2.3/tests/jobs/
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.494030 django-extensions-3.2.3/tests/jobs/daily/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      894 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/jobs/daily/test_cache_cleanup.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.494388 django-extensions-3.2.3/tests/management/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.498980 django-extensions-3.2.3/tests/management/commands/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      229 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/error_raising_command.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.499529 django-extensions-3.2.3/tests/management/commands/shell_plus_tests/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/shell_plus_tests/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    16015 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_collision_resolver.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5666 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_import_subclasses.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5500 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_shell_plus.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2270 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_utils.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1774 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_admin_generator.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2600 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_clear_cache.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3856 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_create_command.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2640 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_create_jobs.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1569 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_create_template_tags.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     7916 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_delete_squashed_migrations.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2203 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_describe_form.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    13005 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_drop_test_database.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3637 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_export_emails.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      379 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_generate_password.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      653 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_generate_secret_key.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6970 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_graph_models.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      863 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_list_signals.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      332 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_mail_debug.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3792 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_managestate.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2125 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_notes.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5752 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_pipchecker.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1674 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_print_settings.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3593 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_print_user_for_session.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      324 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_raise_test_exception.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     8526 2023-06-05 17:05:46.000000 django-extensions-3.2.3/tests/management/commands/test_reset_db.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2331 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_reset_schema.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3083 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_runjob.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      388 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_runserver_plus.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3980 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_set_default_site.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6258 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_set_fake_emails.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2473 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_set_fake_passwords.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1045 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_show_template_tags.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6437 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_show_urls.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     5106 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_sqlcreate.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     8772 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_sqldsn.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     8508 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_sync_s3.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3383 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_syncdata.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1875 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_unreferenced_files.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2518 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_update_permissions.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2367 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/commands/test_validate_templates.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3295 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/test_email_notifications.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2221 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/management/test_modelviz.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       83 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/pythonrc.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      886 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/runner.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.499931 django-extensions-3.2.3/tests/templatetags/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/templatetags/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2398 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/templatetags/test_highlighting.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1661 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/templatetags/test_indent_text.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3654 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/templatetags/test_syntax_color.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3059 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_admin_filter.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1584 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_admin_widgets.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     9842 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_autoslug_fields.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2392 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_clean_pyc.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      688 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_color.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      946 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_compat.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2009 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_compile_pyc.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3475 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_dumpscript.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      681 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_find_template.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     4260 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_json_field.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2556 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_logging_filters.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    20080 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_management_command.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1590 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_models.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1162 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_modificationdatetime_fields.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      143 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_module_in_project_dir.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1800 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_parse_mysql_cnf.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3575 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_randomchar_field.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    10183 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_runscript.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     2987 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_runserver.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1180 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_shortuuid_field.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6141 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_sqldiff.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      485 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_template_rendering.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1190 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_templatetags.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      583 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_timestamped_model.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     6225 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_validators.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      517 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/test_version.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.501098 django-extensions-3.2.3/tests/testapp/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      115 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/admin.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      119 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/apps.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      160 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/classes_to_include.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.501317 django-extensions-3.2.3/tests/testapp/derived_classes_for_testing/
+-rw-r--r--   0 sqrbass    (501) staff       (20)      143 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/derived_classes_for_testing/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      182 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/derived_classes_for_testing/test_module.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      309 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/factories.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      395 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/fields.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       96 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/file_with_utf8_notes.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       53 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/file_without_utf8_notes.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.501634 django-extensions-3.2.3/tests/testapp/jobs/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.501991 django-extensions-3.2.3/tests/testapp/jobs/daily/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/daily/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      248 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/daily/test_daily_job.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.502342 django-extensions-3.2.3/tests/testapp/jobs/hourly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/hourly/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      253 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/hourly/test_hourly_job.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.502583 django-extensions-3.2.3/tests/testapp/jobs/monthly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/monthly/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      258 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/monthly/test_monthly_job.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      202 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/sample.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      196 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/sample_job.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.502823 django-extensions-3.2.3/tests/testapp/jobs/weekly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/weekly/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      253 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/weekly/test_weekly_job.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.503075 django-extensions-3.2.3/tests/testapp/jobs/yearly/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/yearly/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      253 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/jobs/yearly/test_yearly_job.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.503214 django-extensions-3.2.3/tests/testapp/management/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/management/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.503430 django-extensions-3.2.3/tests/testapp/management/commands/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/management/commands/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      277 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/management/commands/test_email_notification_command.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)    15455 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/models.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.504194 django-extensions-3.2.3/tests/testapp/scripts/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/scripts/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      196 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/scripts/directory_checker_script.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       55 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/scripts/error_script.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       76 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/scripts/invalid_import_script.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       44 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/scripts/sample_script.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/scripts/script_no_run_function.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3003 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/settings.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.504379 django-extensions-3.2.3/tests/testapp/templatetags/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/templatetags/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      146 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/templatetags/dummy_tags.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     1165 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp/urls.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.505159 django-extensions-3.2.3/tests/testapp_with_appconfig/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       89 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/admin.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      147 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/apps.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.505325 django-extensions-3.2.3/tests/testapp_with_appconfig/migrations/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/migrations/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       83 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/models.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.505558 django-extensions-3.2.3/tests/testapp_with_appconfig/templatetags/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/templatetags/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      166 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/templatetags/dummy_tags_appconfig.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       86 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/tests.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)       89 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_appconfig/views.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.505796 django-extensions-3.2.3/tests/testapp_with_no_models_file/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_no_models_file/__init__.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.506002 django-extensions-3.2.3/tests/testapp_with_no_models_file/scripts/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_no_models_file/scripts/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      102 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_no_models_file/scripts/other_directory_checker_script.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)      184 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_no_models_file/teslacar.py
+drwxr-xr-x   0 sqrbass    (501) staff       (20)        0 2023-06-05 17:08:43.506115 django-extensions-3.2.3/tests/testapp_with_template_errors/
+-rw-r--r--   0 sqrbass    (501) staff       (20)        0 2023-06-05 12:54:40.000000 django-extensions-3.2.3/tests/testapp_with_template_errors/__init__.py
+-rw-r--r--   0 sqrbass    (501) staff       (20)     3013 2023-06-05 17:05:46.000000 django-extensions-3.2.3/tox.ini
```

### Comparing `django-extensions-3.2.1/CHANGELOG.md` & `django-extensions-3.2.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 Changelog
 =========
 
 See https://github.com/django-extensions/django-extensions/releases
 
+3.2.2
+-----
+
+Changes:
+
+- Improvement: Add support for psycopg3 (#1814)
+- Improvement: runserver_plus, autoreload on template change (#1796)
+- Improvement: highlighting, test_should_highlight_bash_syntax_without_name to include whitespace spans (#1797)
+- Improvement: tests, add Python 3.11 to tox and actions to formally support python 3.11 (#1786)
+- Improvement: runserver_plus, Send the file_changed event when a reload is triggered (#1775)
+- Improvement: runserver_plus, Add REMOTE_USER to werkzeug environment (#1708)
+- Improvement: pipchecker, force pip to use pkg_resources as backend for resolving distributions (#1782)
+- Fix: Fix error with lack of PosixPath support (#1785)
+- Fix: Cleanup http: links (#1798)
+
 3.2.1
 -----
 
 Changes:
 
 - Improvement: fix translation interpolation in prospective arabic translations (#1740)
 - Improvement: runserver_plus, Add option to ignore files on runserver_plus reload (#1762)
```

### Comparing `django-extensions-3.2.1/LICENSE` & `django-extensions-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/Makefile` & `django-extensions-3.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/PKG-INFO` & `django-extensions-3.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-extensions
-Version: 3.2.1
+Version: 3.2.3
 Summary: Extensions for Django
-Home-page: http://github.com/django-extensions/django-extensions
+Home-page: https://github.com/django-extensions/django-extensions
 Author: Michael Trier
 Author-email: mtrier@gmail.com
 Maintainer: Bas van Oostveen
 Maintainer-email: v.oostveen@gmail.com
 License: MIT License
 Project-URL: Documentation, https://django-extensions.readthedocs.io/
 Project-URL: Changelog, https://github.com/django-extensions/django-extensions/blob/main/CHANGELOG.md
@@ -15,25 +15,27 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 License-File: LICENSE
 
 ===================
@@ -144,15 +146,15 @@
 Getting Involved
 ================
 
 Open Source projects can always use more help. Fixing a problem, documenting a feature, adding
 translation in your language. If you have some time to spare and like to help us, here are the places to do so:
 
 - GitHub: https://github.com/django-extensions/django-extensions
-- Mailing list: http://groups.google.com/group/django-extensions
+- Mailing list: https://groups.google.com/group/django-extensions
 - Translations: https://www.transifex.com/projects/p/django-extensions/
 
 
 Documentation
 =============
 
 You can view documentation online at:
@@ -168,10 +170,10 @@
 Django Extensions is free and always will be. It is developed and maintained by developers in an Open Source manner.
 Any support is welcome. You could help by writing documentation, pull-requests, report issues and/or translations.
 
 Please remember that nobody is paid directly to develop or maintain Django Extensions so we do have to divide our time
 between putting food on the table, family, this project and the rest of life :-)
 
 
-__ http://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
-__ http://vimeo.com/1720508
+__ https://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
+__ https://vimeo.com/1720508
 __ https://www.youtube.com/watch?v=1F6G3ONhr4k
```

### Comparing `django-extensions-3.2.1/README.rst` & `django-extensions-3.2.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 Getting Involved
 ================
 
 Open Source projects can always use more help. Fixing a problem, documenting a feature, adding
 translation in your language. If you have some time to spare and like to help us, here are the places to do so:
 
 - GitHub: https://github.com/django-extensions/django-extensions
-- Mailing list: http://groups.google.com/group/django-extensions
+- Mailing list: https://groups.google.com/group/django-extensions
 - Translations: https://www.transifex.com/projects/p/django-extensions/
 
 
 Documentation
 =============
 
 You can view documentation online at:
@@ -130,10 +130,10 @@
 Django Extensions is free and always will be. It is developed and maintained by developers in an Open Source manner.
 Any support is welcome. You could help by writing documentation, pull-requests, report issues and/or translations.
 
 Please remember that nobody is paid directly to develop or maintain Django Extensions so we do have to divide our time
 between putting food on the table, family, this project and the rest of life :-)
 
 
-__ http://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
-__ http://vimeo.com/1720508
+__ https://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
+__ https://vimeo.com/1720508
 __ https://www.youtube.com/watch?v=1F6G3ONhr4k
```

### Comparing `django-extensions-3.2.1/django_extensions/__init__.py` & `django-extensions-3.2.3/django_extensions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-VERSION = (3, 2, 1)
+VERSION = (3, 2, 3)
 
 
 def get_version(version):
     """Dynamically calculate the version based on VERSION tuple."""
     if len(version) > 2 and version[2] is not None:
         if len(version) == 4:
             str_version = "%s.%s.%s.%s" % version
```

### Comparing `django-extensions-3.2.1/django_extensions/admin/__init__.py` & `django-extensions-3.2.3/django_extensions/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/admin/filter.py` & `django-extensions-3.2.3/django_extensions/admin/filter.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/admin/widgets.py` & `django-extensions-3.2.3/django_extensions/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/collision_resolvers.py` & `django-extensions-3.2.3/django_extensions/collision_resolvers.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/compat.py` & `django-extensions-3.2.3/django_extensions/compat.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/db/fields/__init__.py` & `django-extensions-3.2.3/django_extensions/db/fields/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             def slugify_function(self, content):
                 return content.replace('_', '-').lower()
 
             title = models.CharField(max_length=42)
             slug = AutoSlugField(populate_from='title')
 
     Inspired by SmileyChris' Unique Slugify snippet:
-    http://www.djangosnippets.org/snippets/690/
+    https://www.djangosnippets.org/snippets/690/
     """
 
     def __init__(self, *args, **kwargs):
         kwargs.setdefault('blank', True)
         kwargs.setdefault('editable', False)
 
         populate_from = kwargs.pop('populate_from', None)
@@ -480,15 +480,15 @@
 class UUIDFieldMixin:
     """
     UUIDFieldMixin
 
     By default uses UUID version 4 (randomly generated UUID).
 
     The field support all uuid versions which are natively supported by the uuid python module, except version 2.
-    For more information see: http://docs.python.org/lib/module-uuid.html
+    For more information see: https://docs.python.org/lib/module-uuid.html
     """
 
     DEFAULT_MAX_LENGTH = 36
 
     def __init__(self, verbose_name=None, name=None, auto=True, version=4,
                  node=None, clock_seq=None, namespace=None, uuid_name=None, *args,
                  **kwargs):
```

### Comparing `django-extensions-3.2.1/django_extensions/db/fields/json.py` & `django-extensions-3.2.3/django_extensions/db/fields/json.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/db/models.py` & `django-extensions-3.2.3/django_extensions/db/models.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/import_subclasses.py` & `django-extensions-3.2.3/django_extensions/import_subclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         Collect all subclasses of user-defined base classes from project.
         :return: Dictionary from module name to list of tuples.
         First element of tuple is model name and second is alias.
         Currently we set alias equal to model name,
         but in future functionality of aliasing subclasses can be added.
         """
         result = {}  # type: Dict[str, List[Tuple[str, str]]]
-        for loader, module_name, is_pkg in walk_packages(path=[settings.BASE_DIR]):
+        for loader, module_name, is_pkg in walk_packages(path=[str(settings.BASE_DIR)]):
             subclasses_from_module = self._collect_classes_from_module(module_name)
             if subclasses_from_module:
                 result[module_name] = subclasses_from_module
         return result
 
     def _collect_classes_from_module(self, module_name):  # type: (str) -> List[Tuple[str, str]]
         for excluded_module in getattr(settings, 'SHELL_PLUS_SUBCLASSES_IMPORT_MODULES_BLACKLIST', []):
```

### Comparing `django-extensions-3.2.1/django_extensions/jobs/daily/cache_cleanup.py` & `django-extensions-3.2.3/django_extensions/jobs/daily/cache_cleanup.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/ar/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/da/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/da/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/de/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/de/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/el/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/el/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/en/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/es/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/es/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/fr/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/fr/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-extensions\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2011-02-02 11:42+0100\n"
 "PO-Revision-Date: 2014-01-11 11:14+0000\n"
 "Last-Translator: mathiasuk\n"
-"Language-Team: French (http://www.transifex.com/projects/p/django-extensions/language/fr/)\n"
+"Language-Team: French (https://www.transifex.com/projects/p/django-extensions/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: admin/__init__.py:121
```

### Comparing `django-extensions-3.2.1/django_extensions/locale/hu/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/hu/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/id/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/id/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/it/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/it/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/ja/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/ja/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/pl/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/pl/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/pt/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/pt/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/pt_BR/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/pt_BR/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/ro/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/ro/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/ru/LC_MESSAGES/django.mo` & `django-extensions-3.2.3/django_extensions/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/locale/ru/LC_MESSAGES/django.po` & `django-extensions-3.2.3/django_extensions/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/logging/filters.py` & `django-extensions-3.2.3/django_extensions/logging/filters.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/base.py` & `django-extensions-3.2.3/django_extensions/management/base.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/color.py` & `django-extensions-3.2.3/django_extensions/management/color.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/admin_generator.py` & `django-extensions-3.2.3/django_extensions/management/commands/admin_generator.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/clean_pyc.py` & `django-extensions-3.2.3/django_extensions/management/commands/clean_pyc.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/clear_cache.py` & `django-extensions-3.2.3/django_extensions/management/commands/clear_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Author: AxiaCore S.A.S. http://axiacore.com
+# Author: AxiaCore S.A.S. https://axiacore.com
 from django.conf import settings
 from django.core.cache import DEFAULT_CACHE_ALIAS, caches
 from django.core.cache.backends.base import InvalidCacheBackendError
 from django.core.management.base import BaseCommand, CommandError
 
 from django_extensions.management.utils import signalcommand
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/compile_pyc.py` & `django-extensions-3.2.3/django_extensions/management/commands/compile_pyc.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/create_command.py` & `django-extensions-3.2.3/django_extensions/management/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/create_jobs.py` & `django-extensions-3.2.3/django_extensions/management/commands/create_jobs.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/create_template_tags.py` & `django-extensions-3.2.3/django_extensions/management/commands/create_template_tags.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/delete_squashed_migrations.py` & `django-extensions-3.2.3/django_extensions/management/commands/delete_squashed_migrations.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/describe_form.py` & `django-extensions-3.2.3/django_extensions/management/commands/describe_form.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/drop_test_database.py` & `django-extensions-3.2.3/django_extensions/management/commands/drop_test_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import importlib.util
 from itertools import count
 import os
 import logging
 import warnings
 
 from django.conf import settings
 from django.core.management.base import BaseCommand, CommandError
@@ -163,28 +164,35 @@
                 if row_count < 1:
                     break
                 drop_query = 'DROP DATABASE IF EXISTS `%s`' % db_name
                 logging.info('Executing: "' + drop_query + '"')
                 cursor.execute(drop_query)
 
         elif engine in POSTGRESQL_ENGINES:
-            import psycopg2 as Database  # NOQA
+            has_psycopg3 = importlib.util.find_spec("psycopg")
+            if has_psycopg3:
+                import psycopg as Database  # NOQA
+            else:
+                import psycopg2 as Database  # NOQA
 
-            conn_params = {'database': 'template1'}
+            conn_params = {'dbname': 'template1'}
             if user:
                 conn_params['user'] = user
             if password:
                 conn_params['password'] = password
             if database_host:
                 conn_params['host'] = database_host
             if database_port:
                 conn_params['port'] = database_port
 
             connection = Database.connect(**conn_params)
-            connection.set_isolation_level(0)  # autocommit false
+            if has_psycopg3:
+                connection.autocommit = True
+            else:
+                connection.set_isolation_level(0)  # autocommit false
             cursor = connection.cursor()
 
             for db_name in get_database_names('{}_{}'.format):
                 exists_query = "SELECT datname FROM pg_catalog.pg_database WHERE datname='%s';" \
                     % db_name
                 try:
                     cursor.execute(exists_query)
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/dumpscript.py` & `django-extensions-3.2.3/django_extensions/management/commands/dumpscript.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
       Title: Dumpscript management command
     Project: Hardytools (queryset-refactor version)
-     Author: Will Hardy (http://willhardy.com.au)
+     Author: Will Hardy
        Date: June 2008
       Usage: python manage.py dumpscript appname > scripts/scriptname.py
   $Revision: 217 $
 
 Description:
     Generates a Python script that will repopulate the database using objects.
     The advantage of this approach is that it is easy to understand, and more
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/export_emails.py` & `django-extensions-3.2.3/django_extensions/management/commands/export_emails.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/find_template.py` & `django-extensions-3.2.3/django_extensions/management/commands/find_template.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/generate_password.py` & `django-extensions-3.2.3/django_extensions/management/commands/generate_password.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/graph_models.py` & `django-extensions-3.2.3/django_extensions/management/commands/graph_models.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/list_model_info.py` & `django-extensions-3.2.3/django_extensions/management/commands/list_model_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Author: OmenApps. http://www.omenapps.com
+# Author: OmenApps. https://omenapps.com
 import inspect
 
 from django.apps import apps as django_apps
 from django.conf import settings
 from django.core.management.base import BaseCommand
 from django.db import connection
 from django_extensions.management.color import color_style
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/list_signals.py` & `django-extensions-3.2.3/django_extensions/management/commands/list_signals.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/mail_debug.py` & `django-extensions-3.2.3/django_extensions/management/commands/mail_debug.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/managestate.py` & `django-extensions-3.2.3/django_extensions/management/commands/managestate.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/merge_model_instances.py` & `django-extensions-3.2.3/django_extensions/management/commands/merge_model_instances.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/notes.py` & `django-extensions-3.2.3/django_extensions/management/commands/notes.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/pipchecker.py` & `django-extensions-3.2.3/django_extensions/management/commands/pipchecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,24 @@
             editables_only=False,
             user_only=False,
             paths=None,
         ):
             """Return a list of installed Distribution objects.
             Left for compatibility until direct pkg_resources uses are refactored out.
             """
-            from pip._internal.metadata import get_default_environment, get_environment
-            from pip._internal.metadata.pkg_resources import Distribution as _Dist
 
-            if paths is None:
-                env = get_default_environment()
-            else:
-                env = get_environment(paths)
-            dists = env.iter_installed_distributions(
+            from pip._internal.metadata import pkg_resources
+
+            dists = pkg_resources.Environment.from_paths(paths).iter_installed_distributions(
                 local_only=local_only,
                 include_editables=include_editables,
                 editables_only=editables_only,
                 user_only=user_only,
             )
-            return [cast(_Dist, dist)._dist for dist in dists]
+            return [cast(pkg_resources.Distribution, dist)._dist for dist in dists]
 except ImportError:
     # pip < 10
     try:
         from pip import get_installed_distributions  # type:ignore
         from pip.download import PipSession  # type:ignore
         from pip.req import parse_requirements  # type:ignore
     except ImportError:
@@ -216,16 +212,16 @@
         variable ``GITHUB_API_TOKEN`` or setting the command flag
         --github-api-token='mytoken'``.
 
         To create a github api token for use at the command line::
              curl -u 'rizumu' -d '{"scopes":["repo"], "note":"pipchecker"}' https://api.github.com/authorizations
 
         For more info on github api tokens:
-            https://help.github.com/articles/creating-an-oauth-token-for-command-line-use
-            http://developer.github.com/v3/oauth/#oauth-authorizations-api
+            https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
+            https://docs.github.com/en/developers/apps/building-oauth-apps/authorizing-oauth-apps
 
         Requirement Format
         ------------------
         Pipchecker gets the sha of frozen repo and checks if it is
         found at the head of any branches. If it is not found then
         the requirement is considered to be out of date.
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/print_settings.py` & `django-extensions-3.2.3/django_extensions/management/commands/print_settings.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/print_user_for_session.py` & `django-extensions-3.2.3/django_extensions/management/commands/print_user_for_session.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/raise_test_exception.py` & `django-extensions-3.2.3/django_extensions/management/commands/raise_test_exception.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/reset_db.py` & `django-extensions-3.2.3/django_extensions/management/commands/reset_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 reset_db command
 
-originally from http://www.djangosnippets.org/snippets/828/ by dnordberg
+originally from https://www.djangosnippets.org/snippets/828/ by dnordberg
 """
+import importlib.util
 import os
 import logging
 import warnings
 
 from django.conf import settings
 from django.core.management.base import BaseCommand, CommandError
 from django.db import DEFAULT_DB_ALIAS
@@ -137,28 +138,35 @@
             utf8_support = '' if options['no_utf8_support'] else 'CHARACTER SET utf8'
             create_query = 'CREATE DATABASE `%s` %s' % (database_name, utf8_support)
             logging.info('Executing... "%s"', drop_query)
             connection.query(drop_query)
             logging.info('Executing... "%s"', create_query)
             connection.query(create_query.strip())
         elif engine in POSTGRESQL_ENGINES:
-            import psycopg2 as Database  # NOQA
+            has_psycopg3 = importlib.util.find_spec("psycopg")
+            if has_psycopg3:
+                import psycopg as Database  # NOQA
+            else:
+                import psycopg2 as Database  # NOQA
 
-            conn_params = {'database': 'template1'}
+            conn_params = {'dbname': 'template1'}
             if user:
                 conn_params['user'] = user
             if password:
                 conn_params['password'] = password
             if database_host:
                 conn_params['host'] = database_host
             if database_port:
                 conn_params['port'] = database_port
 
             connection = Database.connect(**conn_params)
-            connection.set_isolation_level(0)  # autocommit false
+            if has_psycopg3:
+                connection.autocommit = True
+            else:
+                connection.set_isolation_level(0)  # autocommit false
             cursor = connection.cursor()
 
             if options['close_sessions']:
                 close_sessions_query = """
                     SELECT pg_terminate_backend(pg_stat_activity.pid)
                     FROM pg_stat_activity
                     WHERE pg_stat_activity.datname = '%s';
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/reset_schema.py` & `django-extensions-3.2.3/django_extensions/management/commands/reset_schema.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/runjob.py` & `django-extensions-3.2.3/django_extensions/management/commands/runjob.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/runjobs.py` & `django-extensions-3.2.3/django_extensions/management/commands/runjobs.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/runprofileserver.py` & `django-extensions-3.2.3/django_extensions/management/commands/runprofileserver.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/runscript.py` & `django-extensions-3.2.3/django_extensions/management/commands/runscript.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/runserver_plus.py` & `django-extensions-3.2.3/django_extensions/management/commands/runserver_plus.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 import os
 import re
 import socket
 import sys
 import traceback
 import webbrowser
 import functools
-from typing import List, Set
+from pathlib import Path
+from typing import List, Set  # NOQA
 
 import django
 from django.conf import settings
 from django.core.management.base import BaseCommand, CommandError, SystemCheckError
 from django.core.management.color import color_style
 from django.core.servers.basehttp import get_internal_wsgi_application
 from django.dispatch import Signal
-from django.utils.autoreload import get_reloader
+from django.template.autoreload import get_template_directories, reset_loaders
+from django.utils.autoreload import file_changed, get_reloader
 from django.views import debug as django_views_debug
 
 try:
     if 'whitenoise.runserver_nostatic' in settings.INSTALLED_APPS:
         USE_STATICFILES = False
     else:
         from django.contrib.staticfiles.handlers import StaticFilesHandler
@@ -72,30 +74,70 @@
 DEFAULT_POLLER_RELOADER_INTERVAL = getattr(settings, 'RUNSERVERPLUS_POLLER_RELOADER_INTERVAL', 1)
 DEFAULT_POLLER_RELOADER_TYPE = getattr(settings, 'RUNSERVERPLUS_POLLER_RELOADER_TYPE', 'auto')
 
 logger = logging.getLogger(__name__)
 _error_files = set()  # type: Set[str]
 
 
+def get_all_template_files() -> Set[str]:
+    template_list = set()
+
+    for template_dir in get_template_directories():
+        for base_dir, _, filenames in os.walk(template_dir):
+            for filename in filenames:
+                template_list.add(os.path.join(base_dir, filename))
+
+    return template_list
+
+
 if HAS_WERKZEUG:
     # Monkey patch the reloader to support adding more files to extra_files
     for name, reloader_loop_klass in _reloader.reloader_loops.items():
         class WrappedReloaderLoop(reloader_loop_klass):  # type: ignore
             def __init__(self, *args, **kwargs):
+                self._template_files: Set[str] = get_all_template_files()
                 super().__init__(*args, **kwargs)
                 self._extra_files = self.extra_files
 
             @property
             def extra_files(self):
-                return self._extra_files.union(_error_files)
+                template_files = get_all_template_files()
+
+                # reset loaders if there are new files detected
+                if len(self._template_files) != len(template_files):
+
+                    changed = template_files.difference(self._template_files)
+                    for filename in changed:
+                        _log("info", f" * New file {filename} added, reset template loaders")
+                        self.register_file_changed(filename)
+
+                    reset_loaders()
+
+                self._template_files = template_files
+
+                return self._extra_files.union(_error_files, template_files)
 
             @extra_files.setter
             def extra_files(self, extra_files):
                 self._extra_files = extra_files
 
+            def trigger_reload(self, filename: str) -> None:
+                path = Path(filename)
+                results = file_changed.send(sender=self, file_path=path)
+                if not any(res[1] for res in results):
+                    super().trigger_reload(filename)
+                else:
+                    _log("info", f" * Detected change in {filename!r}, reset template loaders")
+                    self.register_file_changed(filename)
+
+            def register_file_changed(self, filename):
+                if hasattr(self, "mtimes"):
+                    mtime = os.stat(filename).st_mtime
+                    self.mtimes[filename] = mtime
+
         _reloader.reloader_loops[name] = WrappedReloaderLoop
 
 
 def gen_filenames():
     return get_reloader().watched_files()
 
 
@@ -307,29 +349,32 @@
 
             raise exc
 
         return application
 
     def inner_run(self, options):
         if not HAS_WERKZEUG:
-            raise CommandError("Werkzeug is required to use runserver_plus.  Please visit http://werkzeug.pocoo.org/ or install via pip. (pip install Werkzeug)")
+            raise CommandError("Werkzeug is required to use runserver_plus. Please visit https://werkzeug.palletsprojects.com/ or install via pip. (pip install Werkzeug)")
 
         # Set colored output
         if settings.DEBUG:
             try:
                 set_werkzeug_log_color()
             except Exception:  # We are dealing with some internals, anything could go wrong
                 if self.show_startup_messages:
                     print("Wrapping internal werkzeug logger for color highlighting has failed!")
 
         class WSGIRequestHandler(_WSGIRequestHandler):
             def make_environ(self):
                 environ = super().make_environ()
                 if not options['keep_meta_shutdown_func'] and 'werkzeug.server.shutdown' in environ:
                     del environ['werkzeug.server.shutdown']
+                remote_user = os.getenv('REMOTE_USER')
+                if remote_user is not None:
+                    environ['REMOTE_USER'] = remote_user
                 return environ
 
         threaded = options['threaded']
         use_reloader = options['use_reloader']
         open_browser = options['open_browser']
         quit_command = 'CONTROL-C' if sys.platform != 'win32' else 'CTRL-BREAK'
         reloader_interval = options['reloader_interval']
@@ -379,15 +424,15 @@
 
         bind_url = "%s://%s:%s/" % (
             "https" if ssl_context else "http", self.addr if not self._raw_ipv6 else '[%s]' % self.addr, self.port)
 
         if self.show_startup_messages:
             print("\nDjango version %s, using settings %r" % (django.get_version(), settings.SETTINGS_MODULE))
             print("Development server is running at %s" % (bind_url,))
-            print("Using the Werkzeug debugger (http://werkzeug.pocoo.org/)")
+            print("Using the Werkzeug debugger (https://werkzeug.palletsprojects.com/)")
             print("Quit the server with %s." % quit_command)
 
         if open_browser:
             webbrowser.open(bind_url)
 
         if use_reloader and settings.USE_I18N:
             self.extra_files |= set(filter(lambda filename: str(filename).endswith('.mo'), gen_filenames()))
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/set_default_site.py` & `django-extensions-3.2.3/django_extensions/management/commands/set_default_site.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/set_fake_emails.py` & `django-extensions-3.2.3/django_extensions/management/commands/set_fake_emails.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/set_fake_passwords.py` & `django-extensions-3.2.3/django_extensions/management/commands/set_fake_passwords.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/shell_plus.py` & `django-extensions-3.2.3/django_extensions/management/commands/shell_plus.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,15 +480,15 @@
     def set_application_name(self, options):
         """
         Set the application_name on PostgreSQL connection
 
         Use the fallback_application_name to let the user override
         it with PGAPPNAME env variable
 
-        http://www.postgresql.org/docs/9.4/static/libpq-connect.html#LIBPQ-PARAMKEYWORDS  # noqa
+        https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-PARAMKEYWORDS  # noqa
         """
         supported_backends = (
             'django.db.backends.postgresql',
             'django.db.backends.postgresql_psycopg2',
         )
         opt_name = 'fallback_application_name'
         default_app_name = 'django_shell'
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/show_template_tags.py` & `django-extensions-3.2.3/django_extensions/management/commands/show_template_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def format_block(block, nlspaces=0):
     """
     Format the given block of text, trimming leading/trailing
     empty lines and any leading whitespace that is common to all lines.
     The purpose is to let us list a code block as a multiline,
     triple-quoted Python string, taking care of
     indentation concerns.
-    http://code.activestate.com/recipes/145672/
+    https://code.activestate.com/recipes/145672/
     """
     # separate block into lines
     lines = smart_str(block).split('\n')
 
     # remove leading/trailing empty lines
     while lines and not lines[0]:
         del lines[0]
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/show_urls.py` & `django-extensions-3.2.3/django_extensions/management/commands/show_urls.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/sqlcreate.py` & `django-extensions-3.2.3/django_extensions/management/commands/sqlcreate.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/sqldiff.py` & `django-extensions-3.2.3/django_extensions/management/commands/sqldiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
     def sql_to_dict(self, query, param):
         """
         Execute query and return a dict
 
         sql_to_dict(query, param) -> list of dicts
 
-        code from snippet at http://www.djangosnippets.org/snippets/1383/
+        code from snippet at https://www.djangosnippets.org/snippets/1383/
         """
         cursor = connection.cursor()
         cursor.execute(query, param)
         fieldnames = [name[0] for name in cursor.description]
         fieldnames = self.format_field_names(fieldnames)
         result = []
         for row in cursor.fetchall():
@@ -943,15 +943,15 @@
     can_detect_unsigned_differ = False
 
     def load_null(self):
         for table_name in self.db_tables:
             # sqlite does not support tablespaces
             tablespace = "public"
             # index, column_name, column_type, nullable, default_value
-            # see: http://www.sqlite.org/pragma.html#pragma_table_info
+            # see: https://www.sqlite.org/pragma.html#pragma_table_info
             for table_info in self.sql_to_dict("PRAGMA table_info('%s');" % table_name, []):
                 key = (tablespace, table_name, table_info['name'])
                 self.null[key] = not table_info['notnull']
 
     def load_unsigned(self):
         pass
```

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/sqldsn.py` & `django-extensions-3.2.3/django_extensions/management/commands/sqldsn.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/sync_s3.py` & `django-extensions-3.2.3/django_extensions/management/commands/sync_s3.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/syncdata.py` & `django-extensions-3.2.3/django_extensions/management/commands/syncdata.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/unreferenced_files.py` & `django-extensions-3.2.3/django_extensions/management/commands/unreferenced_files.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/update_permissions.py` & `django-extensions-3.2.3/django_extensions/management/commands/update_permissions.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/commands/validate_templates.py` & `django-extensions-3.2.3/django_extensions/management/commands/validate_templates.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/debug_cursor.py` & `django-extensions-3.2.3/django_extensions/management/debug_cursor.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 def monkey_patch_cursordebugwrapper(print_sql=None, print_sql_location=False, truncate=None, logger=print, confprefix="DJANGO_EXTENSIONS"):
     if not print_sql:
         yield
     else:
         if truncate is None:
             truncate = getattr(settings, '%s_PRINT_SQL_TRUNCATE' % confprefix, DEFAULT_PRINT_SQL_TRUNCATE_CHARS)
 
-        # Code orginally from http://gist.github.com/118990
         sqlparse = None
         if getattr(settings, '%s_SQLPARSE_ENABLED' % confprefix, True):
             try:
                 import sqlparse
 
                 sqlparse_format_kwargs_defaults = dict(
                     reindent_aligned=True,
```

### Comparing `django-extensions-3.2.1/django_extensions/management/email_notifications.py` & `django-extensions-3.2.3/django_extensions/management/email_notifications.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/jobs.py` & `django-extensions-3.2.3/django_extensions/management/jobs.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/modelviz.py` & `django-extensions-3.2.3/django_extensions/management/modelviz.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 from django.utils.translation import activate as activate_language
 
 
 __version__ = "1.1"
 __license__ = "Python"
 __author__ = "Bas van Oostveen <v.oostveen@gmail.com>",
 __contributors__ = [
-    "Antonio Cavedoni <http://cavedoni.com/>"
-    "Stefano J. Attardi <http://attardi.org/>",
-    "limodou <http://www.donews.net/limodou/>",
+    "Antonio Cavedoni <https://cavedoni.com/>"
+    "Stefano J. Attardi <https://attardi.org/>",
+    "limodou",
     "Carlo C8E Miron",
     "Andre Campos <cahenan@gmail.com>",
     "Justin Findlay <jfindlay@gmail.com>",
     "Alexander Houben <alexander@houben.ch>",
     "Joern Hees <gitdev@joernhees.de>",
     "Kevin Cherepski <cherepski@gmail.com>",
     "Jose Tomas Tocino <theom3ga@gmail.com>",
```

### Comparing `django-extensions-3.2.1/django_extensions/management/mysql.py` & `django-extensions-3.2.3/django_extensions/management/mysql.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/shells.py` & `django-extensions-3.2.3/django_extensions/management/shells.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/technical_response.py` & `django-extensions-3.2.3/django_extensions/management/technical_response.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/management/utils.py` & `django-extensions-3.2.3/django_extensions/management/utils.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/mongodb/fields/__init__.py` & `django-extensions-3.2.3/django_extensions/mongodb/fields/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     separator
         Defines the used separator (default: '-')
 
     overwrite
         If set to True, overwrites the slug on every save (default: False)
 
     Inspired by SmileyChris' Unique Slugify snippet:
-    http://www.djangosnippets.org/snippets/690/
+    https://www.djangosnippets.org/snippets/690/
     """
 
     def __init__(self, *args, **kwargs):
         kwargs.setdefault('blank', True)
         kwargs.setdefault('editable', False)
 
         populate_from = kwargs.pop('populate_from', None)
@@ -212,15 +212,15 @@
 class UUIDField(StringField):
     """
     UUIDField
 
     By default uses UUID version 1 (generate from host ID, sequence number and current time)
 
     The field support all uuid versions which are natively supported by the uuid python module.
-    For more information see: http://docs.python.org/lib/module-uuid.html
+    For more information see: https://docs.python.org/lib/module-uuid.html
     """
 
     def __init__(self, verbose_name=None, name=None, auto=True, version=1, node=None, clock_seq=None, namespace=None, **kwargs):
         kwargs['max_length'] = 36
         self.auto = auto
         self.version = version
         if version == 1:
```

### Comparing `django-extensions-3.2.1/django_extensions/mongodb/fields/json.py` & `django-extensions-3.2.3/django_extensions/mongodb/fields/json.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/mongodb/models.py` & `django-extensions-3.2.3/django_extensions/mongodb/models.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/settings.py` & `django-extensions-3.2.3/django_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/static/django_extensions/css/jquery.autocomplete.css` & `django-extensions-3.2.3/django_extensions/static/django_extensions/css/jquery.autocomplete.css`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/static/django_extensions/img/indicator.gif` & `django-extensions-3.2.3/django_extensions/static/django_extensions/img/indicator.gif`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/static/django_extensions/js/jquery.ajaxQueue.js` & `django-extensions-3.2.3/django_extensions/static/django_extensions/js/jquery.ajaxQueue.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,9 @@
 /**
  * Ajax Queue Plugin
- *
- * Homepage: http://jquery.com/plugins/project/ajaxqueue
- * Documentation: http://docs.jquery.com/AjaxQueue
  */
 
 /**
 
 <script>
 $(function(){
 	jQuery.ajaxQueue({
```

### Comparing `django-extensions-3.2.1/django_extensions/static/django_extensions/js/jquery.autocomplete.js` & `django-extensions-3.2.3/django_extensions/static/django_extensions/js/jquery.autocomplete.js`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/static/django_extensions/js/jquery.bgiframe.js` & `django-extensions-3.2.3/django_extensions/static/django_extensions/js/jquery.bgiframe.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! Copyright (c) 2010 Brandon Aaron (http://brandonaaron.net)
+/*! Copyright (c) 2010 Brandon Aaron (http://brandon.aaron.sh/)
  * Licensed under the MIT License (LICENSE.txt).
  *
  * Version 2.1.2
  */
 
 (function($) {
```

### Comparing `django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/django2018/digraph.dot` & `django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/django2018/digraph.dot`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/django2018/label.dot` & `django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/django2018/label.dot`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/django2018/relation.dot` & `django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/django2018/relation.dot`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/original/digraph.dot` & `django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/original/digraph.dot`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/original/label.dot` & `django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/original/label.dot`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templates/django_extensions/graph_models/original/relation.dot` & `django-extensions-3.2.3/django_extensions/templates/django_extensions/graph_models/original/relation.dot`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templates/django_extensions/widgets/foreignkey_searchinput.html` & `django-extensions-3.2.3/django_extensions/templates/django_extensions/widgets/foreignkey_searchinput.html`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templatetags/debugger_tags.py` & `django-extensions-3.2.3/django_extensions/templatetags/debugger_tags.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templatetags/highlighting.py` & `django-extensions-3.2.3/django_extensions/templatetags/highlighting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 Similar to syntax_color.py but this is intended more for being able to
 copy+paste actual code into your Django templates without needing to
 escape or anything crazy.
 
-http://lobstertech.com/2008/aug/30/django_syntax_highlight_template_tag/
-
 Example:
 
  {% load highlighting %}
 
  <style>
- @import url("http://lobstertech.com/media/css/highlight.css");
  .highlight { background: #f8f8f8; }
  .highlight { font-size: 11px; margin: 1em; border: 1px solid #ccc;
               border-left: 3px solid #F90; padding: 0; }
  .highlight pre { padding: 1em; overflow: auto; line-height: 120%; margin: 0; }
  .predesc { margin: 1.5em 1.5em -2.5em 1em; text-align: right;
             font: bold 12px Tahoma, Arial, sans-serif;
             letter-spacing: 1px; color: #333; }
```

### Comparing `django-extensions-3.2.1/django_extensions/templatetags/indent_text.py` & `django-extensions-3.2.3/django_extensions/templatetags/indent_text.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/templatetags/syntax_color.py` & `django-extensions-3.2.3/django_extensions/templatetags/syntax_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     {% load syntax_color %}
     {{ code_string|colorize:"python" }}
 
 You may use any lexer in Pygments. The complete list of which
 can be found [on the Pygments website][1].
 
-[1]: http://pygments.org/docs/lexers/
+[1]: https://pygments.org/docs/lexers/
 
 You may also have Pygments attempt to guess the correct lexer for
 a particular string. However, if may not be able to choose a lexer,
 in which case it will simply return the string unmodified. This is
 less efficient compared to specifying the lexer to use.
 
     {{ code_string|colorize }}
```

### Comparing `django-extensions-3.2.1/django_extensions/templatetags/widont.py` & `django-extensions-3.2.3/django_extensions/templatetags/widont.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/utils/dia2django.py` & `django-extensions-3.2.3/django_extensions/utils/dia2django.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/utils/internal_ips.py` & `django-extensions-3.2.3/django_extensions/utils/internal_ips.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions/validators.py` & `django-extensions-3.2.3/django_extensions/validators.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/django_extensions.egg-info/PKG-INFO` & `django-extensions-3.2.3/django_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-extensions
-Version: 3.2.1
+Version: 3.2.3
 Summary: Extensions for Django
-Home-page: http://github.com/django-extensions/django-extensions
+Home-page: https://github.com/django-extensions/django-extensions
 Author: Michael Trier
 Author-email: mtrier@gmail.com
 Maintainer: Bas van Oostveen
 Maintainer-email: v.oostveen@gmail.com
 License: MIT License
 Project-URL: Documentation, https://django-extensions.readthedocs.io/
 Project-URL: Changelog, https://github.com/django-extensions/django-extensions/blob/main/CHANGELOG.md
@@ -15,25 +15,27 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 License-File: LICENSE
 
 ===================
@@ -144,15 +146,15 @@
 Getting Involved
 ================
 
 Open Source projects can always use more help. Fixing a problem, documenting a feature, adding
 translation in your language. If you have some time to spare and like to help us, here are the places to do so:
 
 - GitHub: https://github.com/django-extensions/django-extensions
-- Mailing list: http://groups.google.com/group/django-extensions
+- Mailing list: https://groups.google.com/group/django-extensions
 - Translations: https://www.transifex.com/projects/p/django-extensions/
 
 
 Documentation
 =============
 
 You can view documentation online at:
@@ -168,10 +170,10 @@
 Django Extensions is free and always will be. It is developed and maintained by developers in an Open Source manner.
 Any support is welcome. You could help by writing documentation, pull-requests, report issues and/or translations.
 
 Please remember that nobody is paid directly to develop or maintain Django Extensions so we do have to divide our time
 between putting food on the table, family, this project and the rest of life :-)
 
 
-__ http://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
-__ http://vimeo.com/1720508
+__ https://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
+__ https://vimeo.com/1720508
 __ https://www.youtube.com/watch?v=1F6G3ONhr4k
```

### Comparing `django-extensions-3.2.1/docs/AUTHORS` & `django-extensions-3.2.3/docs/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The following individuals have contributed to this project
 
-Antonio Cavedoni - For the GraphViz stuff (http://cavedoni.com/)
+Antonio Cavedoni - For the GraphViz stuff (https://cavedoni.com/)
 Ludvig Ericson (toxic)
 Collin Grady (magus)
 Gabriel Grant (gabrielgrant)
 Rob Hudson (robhudson)
 Jannis Leidel (leidel)
 Brian Rosner (brosner)
 Michael Trier (empty)
```

### Comparing `django-extensions-3.2.1/docs/Makefile` & `django-extensions-3.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/admin_extensions.rst.txt` & `django-extensions-3.2.3/docs/admin_extensions.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/admin_generator.rst.txt` & `django-extensions-3.2.3/docs/admin_generator.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/command_extensions.rst.txt` & `django-extensions-3.2.3/docs/command_extensions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
    dumpscript
    runscript
    export_emails
    generate_password
    graph_models
    list_model_info
    list_signals
+   managestate
    merge_model_instances
    print_settings
    reset_db
    runprofileserver
    runserver_plus
    sync_s3
    syncdata
@@ -103,14 +104,16 @@
   It seems this works only if setting ``SESSION_ENGINE`` is
   ``'django.contrib.sessions.backends.db'`` (default value).
 
 * *drop_test_database* - Drops the test database. Usefull when running Django
   test via some automated system (BuildBot, Jenkins, etc) and making sure that
   the test database is always dropped at the end.
 
+* *raise_test_exception* - Raises a test exception via command. Useful for debugging error reporters such as Sentry.
+
 * :doc:`reset_db` - Resets a database (currently sqlite3, mysql, postgres). Uses "DROP DATABASE" and "CREATE DATABASE".
 
 * *runjob* - Run a single maintenance job.  Part of the jobs system.
 
 * *runjobs* - Runs scheduled maintenance jobs. Specify hourly, daily, weekly,
   monthly.  Part of the jobs system.
 
@@ -160,9 +163,9 @@
 .. _`export_emails`: export_emails.html
 .. _`graph_models`: graph_models.html
 .. _`list_model_info`: list_model_info.html
 .. _`print_settings`: print_settings.html
 .. _`runscript`: runscript.html
 .. _`runserver_plus`: runserver_plus.html
 .. _`sync_s3`: sync_s3.html
-.. _GraphViz: http://www.graphviz.org/
-.. _Werkzeug: http://werkzeug.pocoo.org/
+.. _GraphViz: https://www.graphviz.org/
+.. _Werkzeug: https://werkzeug.palletsprojects.com/
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/command_signals.rst.txt` & `django-extensions-3.2.3/docs/command_signals.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/create_template_tags.rst.txt` & `django-extensions-3.2.3/docs/create_template_tags.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/debugger_tags.rst.txt` & `django-extensions-3.2.3/docs/debugger_tags.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/delete_squashed_migrations.rst.txt` & `django-extensions-3.2.3/docs/delete_squashed_migrations.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/dumpscript.rst.txt` & `django-extensions-3.2.3/docs/dumpscript.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/export_emails.rst.txt` & `django-extensions-3.2.3/docs/export_emails.rst`

 * *Files 0% similar despite different names*

```diff
@@ -112,8 +112,8 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 A function to use to create a full name based on the database fields selected by
 `EXPORT_EMAILS_FULL_NAME_FUNC`. The default implementation can be looked up in
 https://github.com/django-extensions/django-extensions/blob/master/django_extensions/management/commands/export_emails.py#L23
 
 
-.. _`LinkedIn Groups`: http://www.linkedin.com/static?key=groups_info
+.. _`LinkedIn Groups`: https://www.linkedin.com/static?key=groups_info
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/field_extensions.rst.txt` & `django-extensions-3.2.3/docs/field_extensions.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/generate_password.rst.txt` & `django-extensions-3.2.3/docs/generate_password.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/graph_models.rst.txt` & `django-extensions-3.2.3/docs/graph_models.rst`

 * *Files 10% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 Templates used:
 
  - django_extensions/graph_models/digraph.dot
  - django_extensions/graph_models/label.dot
  - django_extensions/graph_models/relation.dot
 
-Documentation on how to create dot files can be found here: http://www.graphviz.org/documentation/
+Documentation on how to create dot files can be found here: https://www.graphviz.org/documentation/
 
 .. warning::
   Modifying Django's default templates behaviour might break *graph_models*
 
   Please be aware that if you use any *template_loaders* or extensions that change the
   way templates are rendered that this can cause *graph_models* to fail.
 
@@ -129,12 +129,23 @@
   $ ./manage.py graph_models -a --hide-edge-labels -o my_project_sans_foo_bar.png
 
 ::
 
   # Create a graph with 'normal' arrow shape for relations
   $ ./manage.py graph_models -a --arrow-shape normal -o my_project_sans_foo_bar.png
 
+::
+
+  # Create a graph with colored edges for relations with on_delete settings
+  $ ./manage.py graph_models -a --color-code-deletions -o my_project_colored.png
+
+::
+
+  # Create a graph with different layout direction,
+  # supported directions: "TB", "LR", "BT", "RL"
+  $ ./manage.py graph_models -a --rankdir BT -o my_project_sans_foo_bar.png
+
 
 
-.. _GraphViz: http://www.graphviz.org/
+.. _GraphViz: https://www.graphviz.org/
 .. _pygraphviz: https://pygraphviz.github.io/
 .. _pydot: https://pypi.python.org/pypi/pydot
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/index.rst.txt` & `django-extensions-3.2.3/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,9 @@
 
 
 Indices and tables
 ==================
 
 * :ref:`search`
 
-__ http://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
+__ https://ericholscher.com/blog/2008/sep/12/screencast-django-command-extensions/
 __ https://vimeo.com/1720508
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/installation_instructions.rst.txt` & `django-extensions-3.2.3/docs/installation_instructions.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/jobs_scheduling.rst.txt` & `django-extensions-3.2.3/docs/jobs_scheduling.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/list_model_info.rst.txt` & `django-extensions-3.2.3/docs/list_model_info.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/merge_model_instances.rst.txt` & `django-extensions-3.2.3/docs/merge_model_instances.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/model_extensions.rst.txt` & `django-extensions-3.2.3/docs/model_extensions.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/permissions.rst.txt` & `django-extensions-3.2.3/docs/permissions.rst`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Introduction
 ------------
 Django Extensions offers mixins for Class Based Views that make it easier to
 query and limit access to certain views.
 
 Current Mixins
 ---------------------------------
-* *UserPermissionMixin* - A Class Based View mixin that limits the accessibility to the view based on the "owner" of the view.
+* *ModelUserFieldPermissionMixin* - A Class Based View mixin that limits the accessibility to the view based on the "owner" of the view.
 
 This will check if the currently logged in user (``self.request.user``) matches the owner of the model instance.
 By default, the "owner" will be called "user".
 
 .. code-block:: python
 
    # models.py
@@ -29,15 +29,15 @@
 
 .. code-block:: python
 
    # views.py
 
    from django.views.generic import UpdateView
 
-   from django_extensions.auth.mixins import UserPermissionMixin
+   from django_extensions.auth.mixins import ModelUserFieldPermissionMixin
 
    from .models import MyModel
 
-   class MyModelUpdateView(UserPermissionMixin, UpdateView):
+   class MyModelUpdateView(ModelUserFieldPermissionMixin, UpdateView):
       model = MyModel
       template_name = 'mymodels/update.html'
       model_permission_user_field = 'author'
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/print_settings.rst.txt` & `django-extensions-3.2.3/docs/print_settings.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/reset_db.rst.txt` & `django-extensions-3.2.3/docs/reset_db.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/runprofileserver.rst.txt` & `django-extensions-3.2.3/docs/runprofileserver.rst`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 By default the profile-data-files are saved in /tmp use the --prof-path option
 to specify your own target directory. Saving the data in a meaningful directory
 structure helps to keep your profile data organized and keeps /tmp uncluttered.
 (Yes this probably malfunctions systems such as Windows where /tmp does not exist)
 
 To define profile filenames use --prof-file option. Default format
 is "{path}.{duration:06d}ms.{time}" (Python
-`Format Specification <http://docs.python.org/3/library/string.html#formatspec>`_
+`Format Specification <https://docs.python.org/3/library/string.html#formatspec>`_
 is used).
 
 Examples:
 
   * "{time}-{path}-{duration}ms" - to order profile-data-files by request time
   * "{duration:06d}ms.{path}.{time}" - to order by request duration
 
@@ -83,12 +83,10 @@
   [13/Nov/2008 06:29:39] "GET /site_media/base.js HTTP/1.1" 200 751
   <ctrl-c>
   $ kcachegrind /tmp/my-profile-data/root.12574391.592.prof
 
 Links
 -----
 
-* http://code.djangoproject.com/wiki/ProfilingDjango
-* http://www.rkblog.rk.edu.pl/w/p/django-profiling-hotshot-and-kcachegrind/
-* http://code.djangoproject.com/browser/django/trunk/django/bin/profiling/gather_profile_stats.py
-* http://www.oluyede.org/blog/2007/03/07/profiling-django/
-* http://simonwillison.net/2008/May/22/debugging/
+* https://code.djangoproject.com/wiki/ProfilingDjango
+* https://rk.edu.pl/en/django-profiling-hotshot-and-kcachegrind/
+* https://simonwillison.net/2008/May/22/debugging/
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/runscript.rst.txt` & `django-extensions-3.2.3/docs/runscript.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/runserver_plus.rst.txt` & `django-extensions-3.2.3/docs/runserver_plus.rst`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   * Restarting with reloader...
 
   Validating models...
   0 errors found
 
   Django version X.Y.Z, using settings 'screencasts.settings'
   Development server is running at http://127.0.0.1:8000/
-  Using the Werkzeug debugger (http://werkzeug.pocoo.org/)
+  Using the Werkzeug debugger (https://werkzeug.palletsprojects.com/)
   Quit the server with CONTROL-C.
 
 Note: all normal runserver options apply. In other words, if you need to change
 the port number or the host information, you can do so like you would normally.
 
 
 Usage
@@ -86,15 +86,15 @@
 environment parameter coming into the function.
 
 *WARNING*: This should *never* be used in any kind of production environment.
 Not even for a quick problem check.  I cannot emphasize this enough. The
 interactive debugger allows you to evaluate python code right against the
 server.  You've been warned.
 
-.. _`Werkzeug WSGI utilities`: http://werkzeug.pocoo.org/
+.. _`Werkzeug WSGI utilities`: https://werkzeug.palletsprojects.com/
 
 
 SSL
 ^^^
 
 runserver_plus also supports SSL, so that you can easily debug bugs that pop up
 when https is used. To use SSL simply provide a file name for certificates;
@@ -102,24 +102,24 @@
 
   $ python manage.py runserver_plus --cert-file cert.crt
   Validating models...
   0 errors found
 
   Django version X.Y.Z, using settings 'mysite.settings'
   Development server is running at http://127.0.0.1:8000/
-  Using the Werkzeug debugger (http://werkzeug.pocoo.org/)
+  Using the Werkzeug debugger (https://werkzeug.palletsprojects.com/)
   Quit the server with CONTROL-C.
    * Running on https://127.0.0.1:8000/
    * Restarting with reloader
   Validating models...
   0 errors found
 
   Django version X.Y.Z, using settings 'mysite.settings'
   Development server is running at http://127.0.0.1:8000/
-  Using the Werkzeug debugger (http://werkzeug.pocoo.org/)
+  Using the Werkzeug debugger (https://werkzeug.palletsprojects.com/)
   Quit the server with CONTROL-C.
 
 After running this command, your web application can be accessed through
 https://127.0.0.1:8000.
 
 You will also find that two files are created in  the current working directory:
 a key file and a certificate file. If you run the above command again, these
@@ -202,14 +202,17 @@
 
   # Werkzeug reloader type [auto, watchdog, or stat]
   RUNSERVERPLUS_POLLER_RELOADER_TYPE = 'auto'
 
   # Add extra files to watch
   RUNSERVER_PLUS_EXTRA_FILES = []
 
+  # Do not watch files matching any of these patterns
+  RUNSERVER_PLUS_EXCLUDE_PATTERNS = []
+
 
 IO Calls and CPU Usage
 ^^^^^^^^^^^^^^^^^^^^^^
 
 As noted in gh625_ `runserver_plus` can be seen to use a lot of CPU and generate many
 I/O when idle.
 
@@ -218,15 +221,15 @@
 
 The `stat polling` approach is pretty brute force and continously issues `stat` system calls which
 causes the CPU and IO load.
 
 If possible try to install the Watchdog_ package, this should automatically cause Werkzeug_ to use
 `file system events` whenever possible.
 
-You can read more about this in `Werkzeug documentation <http://werkzeug.pocoo.org/docs/serving/#reloader>`_
+You can read more about this in `Werkzeug documentation <https://werkzeug.palletsprojects.com/serving/#reloader>`_
 
 You can also increase the poll interval when using `stat polling` from the default of 1 second. This
 will decrease the CPU load at the expense of file edits taking longer to pick up.
 
 This can be set two ways, in the django settings file::
 
     RUNSERVERPLUS_POLLER_RELOADER_INTERVAL = 5
@@ -236,15 +239,15 @@
   $ python manage.py runserver_plus --reloader-interval 5
 
 
 Debugger PIN
 ------------
 
 .. epigraph::
-   The following text about the debugger PIN is taken verbatim from the Werkzeug `documentation about its debugger PIN <http://werkzeug.pocoo.org/docs/debug/#debugger-pin>`_.
+   The following text about the debugger PIN is taken verbatim from the Werkzeug `documentation about its debugger PIN <https://werkzeug.palletsprojects.com/en/2.2.x/debug/#debugger-pin>`_.
 
 Starting with Werkzeug 0.11 the debugger is additionally protected by a PIN. This is a security helper to
 make it less likely for the debugger to be exploited in production as it has happened to people to keep the
 debugger active. The PIN based authentication is enabled by default.
 
 When the debugger comes up, on first usage it will prompt for a PIN that is printed to the command line.
 The PIN is generated in a stable way that is specific to the project. In some situations it might be not possible
@@ -257,9 +260,9 @@
 If the PIN is entered too many times incorrectly the server needs to be restarted.
 
 **This feature is not supposed to entirely secure the debugger. It’s intended to make it harder for an attacker to
 exploit the debugger. Never enable the debugger in production.**
 
 
 .. _gh625: https://github.com/django-extensions/django-extensions/issues/625
-.. _Werkzeug: http://werkzeug.pocoo.org/
+.. _Werkzeug: https://werkzeug.palletsprojects.com/
 .. _Watchdog: https://pypi.python.org/pypi/watchdog
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/shell_plus.rst.txt` & `django-extensions-3.2.3/docs/shell_plus.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   $ ./manage.py shell_plus --ptpython
 
 
 Python::
 
   $ ./manage.py shell_plus --plain
 
-It is possible to directly add command line arguments to the underlying Python shell using `--`::
+It is possible to directly add command line arguments to the underlying Python shell using ``--``::
 
   $ ./manage.py shell_plus --ipython -- --profile=foo
 
 
 The default resolution order is: ptpython, bpython, ipython, python.
 
 You can also set the configuration option SHELL_PLUS to explicitly specify which version you want.
@@ -175,19 +175,19 @@
 
 Default collision resolver. Model from last application in alphabetical order is selected::
 
     from workers import Language
 
 **InstalledAppsOrderCR**
 
-Collision resolver which selects first model from INSTALLED_APPS.
+Collision resolver which selects the first model from INSTALLED_APPS.
 You can set your own app priorities list subclassing him and overwriting ``APP_PRIORITIES`` field.
 
-This collision resolver will select model from first app on this list.
-If both app's are absent on this list, resolver will choose model from first app in alphabetical order::
+This collision resolver will select a model from the first app on this list.
+If both app's are absent on this list, resolver will choose a model from the first app in alphabetical order::
 
     from programming import Language
 
 **FullPathCR**
 
 Collision resolver which transform full model name to alias by changing dots to underscores.
 He also removes 'models' part of alias, because all models are in models.py files.
@@ -216,42 +216,42 @@
     from programming import Language (as Language_programming)
     from workers import Language, Language (as Language_workers)
 
 **AppNamePrefixCustomOrderCR**
 
 Collision resolver which is mixin of AppNamePrefixCR and InstalledAppsOrderCR.
 
-In case of collisions he sets aliases like AppNamePrefixCR, but sets default model using InstalledAppsOrderCR::
+In case of collisions he sets aliases like AppNamePrefixCR, but sets the default model using InstalledAppsOrderCR::
 
     from programming import Language, Language (as programming_Language)
     from workers import Language (as workers_Language)
 
 **AppNameSuffixCustomOrderCR**
 
-Collision resolver which is mixin of AppNameSuffixCR and InstalledAppsOrderCR.
+Collision resolver which is a mixin of AppNameSuffixCR and InstalledAppsOrderCR.
 
-In case of collisions he sets aliases like AppNameSuffixCR, but sets default model using InstalledAppsOrderCR::
+In case of collisions he sets aliases like AppNameSuffixCR, but sets the default model using InstalledAppsOrderCR::
 
     from programming import Language, Language (as Language_programming)
     from workers import Language (as Language_workers)
 
 **FullPathCustomOrderCR**
 
-Collision resolver which is mixin of FullPathCR and InstalledAppsOrderCR.
+Collision resolver which is a mixin of FullPathCR and InstalledAppsOrderCR.
 
-In case of collisions he sets aliases like FullPathCR, but sets default model using InstalledAppsOrderCR::
+In case of collisions he sets aliases like FullPathCR, but sets the default model using InstalledAppsOrderCR::
 
     from programming import Language, Language (as programming_Language)
     from workers import Language (as workers_Language)
 
 **AppLabelPrefixCR**
 
 Collision resolver which transform pair (app_label, model_name) to alias ``{app_label}_{model_name}``
 
-This is very similar to ``AppNamePrefixCR`` but this may generate shorter names in case of apps nested
+This is very similar to ``AppNamePrefixCR`` but this may generate shorter names in the case of apps nested
 into several namespace (like Django's auth app)::
 
     # with AppNamePrefixCR
     from django.contrib.auth.models import Group (as django_contrib_auth_Group)
 
     # with AppLabelPrefixCR
     from django.contrib.auth.models import Group (as auth_Group)
@@ -277,69 +277,69 @@
 
 **PathBasedCR**
 
 Abstract resolver which transforms full model name into alias.
 To use him you need to overwrite transform_import function
 which should have one parameter.
 
-It will be full model name. It should return valid alias as str instance.
+It will be a full model name. It should return valid alias as a str instance.
 
 **AppNameCR**
 
 Abstract collision resolver which transform pair (app name, model_name) to alias by changing dots to underscores.
 
 You must define ``MODIFICATION_STRING`` which should be string to format with two keyword arguments:
 app_name and model_name. For example: ``{app_name}_{model_name}``.
 
 Model from last application in alphabetical order is selected.
 
-You can mix PathBasedCR or AppNameCR with InstalledAppsOrderCR, but InstalledAppsOrderCR should be second base class.
+You can mix PathBasedCR or AppNameCR with InstalledAppsOrderCR, but InstalledAppsOrderCR should be the second base class.
 
 **BaseCR**
 
 Abstract base collision resolver. All collision resolvers needs to inherit from this class.
 
-To write custom collision resolver you need to overwrite resolve_collisions function.
+To write a custom collision resolver you need to overwrite the resolve_collisions function.
 It receives ``Dict[str, List[str]]`` where key is model name and values are full model names
 (full model name means: module + model_name).
 
 You should return ``Dict[str, str]``, where key is model name and value is full model name.
 
 Import Subclasses
 -------------------
 If you want to load automatically all project subclasses of some base class,
 you can achieve this by setting ``SHELL_PLUS_SUBCLASSES_IMPORT`` option.
 
-It must be list of either classes or strings containing paths to this classes.
+It must be a list of either classes or strings containing paths to these classes.
 
-For example if you want to load all your custom managers than you should provide::
+For example, if you want to load all your custom managers then you should provide::
 
     from django.db.models import Manager
     SHELL_PLUS_SUBCLASSES_IMPORT = [Manager]
 
-Than shell_plus will load all your custom managers::
+Then shell_plus will load all your custom managers::
 
     # Shell Plus Subclasses Imports
     from utils.managers import AbstractManager
     from myapp.managers import MyCustomManager
     from somewhere.else import MyOtherManager
     # django.db.models.Manager is not loaded because only project classes are.
 
-By default all subclasses of your base class from all projects module will be loaded.
+By default, all subclasses of your base class from all projects modules will be loaded.
 
 You can exclude some modules and all their submodules by passing ``SHELL_PLUS_SUBCLASSES_IMPORT_MODULES_BLACKLIST`` option::
 
     SHELL_PLUS_SUBCLASSES_IMPORT_MODULES_BLACKLIST = ['utils', 'somewhere.else']
 
 Elements of this list must be strings containing full modules paths.
 If these modules are excluded only ``MyCustomManager`` from ``myapp.managers`` will be loaded.
 
 If you are using ``SHELL_PLUS_SUBCLASSES_IMPORT`` shell_plus loads all project modules for finding subclasses.
 
-Sometimes it can lead to some errors(for example when we have old unused module which contains syntax errors).
+Sometimes it can lead to some errors(for example when we have an old unused module which contains syntax errors).
 
 Excluding these modules can help avoid shell_plus crashes in some situations.
 It is recommended to exclude all ``setup.py`` files.
 
 IPython Notebook
 ----------------
 There are two settings that you can use to pass your custom options to the IPython
@@ -378,25 +378,25 @@
 
 To activate auto-loading, remember to either include the django-extensions' default
 notebook extension or copy its auto-loading code into your own extension.
 
 Note that the IPython Notebook feature doesn't currently honor the
 ``--dont-load`` option.
 
-.. _`IPython Notebook`: http://ipython.org/ipython-doc/dev/interactive/htmlnotebook.html
+.. _`IPython Notebook`: https://ipython.org/ipython-doc/dev/interactive/htmlnotebook.html
 
 
 
 Additional Imports
 ------------------
 
-In addition to importing the models you can specify other items to import by default.
+In addition to importing the models, you can specify other items to import by default.
 These can be specified with the settings ``SHELL_PLUS_IMPORTS``, ``SHELL_PLUS_PRE_IMPORTS`` and ``SHELL_PLUS_POST_IMPORTS``.
 
-The other of import loading is as follows:
+The order of import loading is as follows:
 
  - ``SHELL_PLUS_PRE_IMPORTS``
  - Subclasses (if enabled)
  - Models (if not disabled)
  - Default Django imports (if not disabled)
  - ``SHELL_PLUS_IMPORTS``
  - ``SHELL_PLUS_POST_IMPORTS``
@@ -432,7 +432,20 @@
 
 You can also set the configuration option SHELL_PLUS_PRINT_SQL to omit the above command line option.
 
 ::
 
   # print SQL queries in shell_plus
   SHELL_PLUS_PRINT_SQL = True
+
+Printing SQL queries also comes with the possibility of specifying the maximum amount of characters to display:
+
+  $ ./manage.py shell_plus --print-sql --truncate-sql
+
+`--truncate-sql` accepts an int value starting from 0 (which disables truncation). Defaults to 1000.
+
+You can also set the configuration option SHELL_PLUS_PRINT_SQL_TRUNCATE to omit the above command line option.
+
+::
+
+  # print SQL queries in shell_plus
+  SHELL_PLUS_PRINT_SQL_TRUNCATE = None
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/sqlcreate.rst.txt` & `django-extensions-3.2.3/docs/sqlcreate.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/sqldiff.rst.txt` & `django-extensions-3.2.3/docs/sqldiff.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/sync_s3.rst.txt` & `django-extensions-3.2.3/docs/sync_s3.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/syncdata.rst.txt` & `django-extensions-3.2.3/docs/syncdata.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/utilities.rst.txt` & `django-extensions-3.2.3/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/validate_templates.rst.txt` & `django-extensions-3.2.3/docs/validate_templates.rst`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 A higher verbosity level will print out all the files that are processed
 instead of only the ones that contain errors.
 
 break
 ~~~~~
 Do not continue scanning other templates after the first failure.
 
-ignore_app
+ignore-app
 ~~~~~~~~~~
 Ignore this app (can be used multiple times).
 
 includes
 ~~~~~~~~
 Use -i (can be used multiple times) to add directories to the TEMPLATE DIRS.
 
-no_apps
+no-apps
 ~~~~~~~
 Do not automatically include app template directories.
 
 
 Settings
 --------
```

### Comparing `django-extensions-3.2.1/docs/_build/html/_sources/validators.rst.txt` & `django-extensions-3.2.3/docs/validators.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/conf.py` & `django-extensions-3.2.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '3.2'
 # The full version, including alpha/beta/rc tags.
-release = '3.2.1'
+release = '3.2.3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `django-extensions-3.2.1/docs/creating_release.txt` & `django-extensions-3.2.3/docs/creating_release.txt`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/managestate.rst` & `django-extensions-3.2.3/docs/managestate.rst`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/docs/sqldsn.rst` & `django-extensions-3.2.3/docs/sqldsn.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 Supported Databases
 -------------------
 
 Currently the following databases are supported:
 
-* PostgreSQL (psycopg2 or postgis)
+* PostgreSQL (psycopg2, psycopg3, or postgis)
 * Sqlite3
 * MySQL
 
 Patches to support other databases are welcome! :-)
 
 
 Supported Styles
```

### Comparing `django-extensions-3.2.1/setup.cfg` & `django-extensions-3.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/setup.py` & `django-extensions-3.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     if head == path:
         return result
     return fullsplit(head, [tail] + result)
 
 
 # Tell distutils to put the data_files in platform-specific installation
 # locations. See here for an explanation:
-# http://groups.google.com/group/comp.lang.python/browse_thread/thread/35ec7b2fed36eaec/2105ee4d9e8042cb
+# https://groups.google.com/group/comp.lang.python/browse_thread/thread/35ec7b2fed36eaec/2105ee4d9e8042cb
 for scheme in INSTALL_SCHEMES.values():
     scheme['data'] = scheme['purelib']
 
 
 # Compile the list of packages available, because distutils doesn't have
 # an easy way to do this.
 packages, package_data = [], {}
@@ -82,29 +82,29 @@
 version = __import__('django_extensions').__version__
 
 if int(setuptools.__version__.split(".", 1)[0]) < 18:
     assert "bdist_wheel" not in sys.argv, "setuptools 18 or later is required for wheels."
 
 long_description = """django-extensions bundles several useful
 additions for Django projects. See the project page for more information:
-  http://github.com/django-extensions/django-extensions"""
+  https://github.com/django-extensions/django-extensions"""
 if os.path.isfile("README.rst"):
     with open("README.rst") as f:
         long_description = f.read()
 
 setup(
     name='django-extensions',
     version=version,
     description="Extensions for Django",
     long_description=long_description,
     author='Michael Trier',
     author_email='mtrier@gmail.com',
     maintainer='Bas van Oostveen',
     maintainer_email='v.oostveen@gmail.com',
-    url='http://github.com/django-extensions/django-extensions',
+    url='https://github.com/django-extensions/django-extensions',
     license='MIT License',
     platforms=['any'],
     packages=packages,
     cmdclass=cmdclasses,
     package_data=package_data,
     python_requires=">=3.6",
     install_requires=["Django>=3.2"],
@@ -112,25 +112,27 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Utilities',
     ],
     project_urls={
         "Documentation": "https://django-extensions.readthedocs.io/",
         "Changelog": "https://github.com/django-extensions/django-extensions/blob/main/CHANGELOG.md",
```

### Comparing `django-extensions-3.2.1/tests/auth/test_mixins.py` & `django-extensions-3.2.3/tests/auth/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/collisions/models.py` & `django-extensions-3.2.3/tests/collisions/models.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/db/fields/test_uniq_field_mixin.py` & `django-extensions-3.2.3/tests/db/fields/test_uniq_field_mixin.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/db/fields/test_uniq_field_mixin_compat.py` & `django-extensions-3.2.3/tests/db/fields/test_uniq_field_mixin_compat.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/jobs/daily/test_cache_cleanup.py` & `django-extensions-3.2.3/tests/jobs/daily/test_cache_cleanup.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_collision_resolver.py` & `django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_collision_resolver.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_import_subclasses.py` & `django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_import_subclasses.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_shell_plus.py` & `django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_shell_plus.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/shell_plus_tests/test_utils.py` & `django-extensions-3.2.3/tests/management/commands/shell_plus_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_admin_generator.py` & `django-extensions-3.2.3/tests/management/commands/test_admin_generator.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_clear_cache.py` & `django-extensions-3.2.3/tests/management/commands/test_clear_cache.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_create_command.py` & `django-extensions-3.2.3/tests/management/commands/test_create_command.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_create_jobs.py` & `django-extensions-3.2.3/tests/management/commands/test_create_jobs.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_create_template_tags.py` & `django-extensions-3.2.3/tests/management/commands/test_create_template_tags.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_delete_squashed_migrations.py` & `django-extensions-3.2.3/tests/management/commands/test_delete_squashed_migrations.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_describe_form.py` & `django-extensions-3.2.3/tests/management/commands/test_describe_form.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_drop_test_database.py` & `django-extensions-3.2.3/tests/management/commands/test_drop_test_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import importlib.util
 from io import StringIO
 from unittest.mock import MagicMock, Mock, PropertyMock, call, patch
 
 from django.core.management import CommandError, call_command
 from django.test import TestCase
 from django.test.utils import override_settings
 
@@ -247,15 +248,19 @@
     def test_postgresql_should_drop_database(self, m_stdout):
         m_database = MagicMock()
         m_cursor = Mock()
         m_database.connect.return_value.cursor.return_value = m_cursor
         # Indicate that no clone databases exist
         type(m_cursor).rowcount = PropertyMock(side_effect=(1, 0))
 
-        with patch.dict("sys.modules", psycopg2=m_database):
+        mock_kwargs = {"psycopg2": m_database}
+        has_psycopg3 = importlib.util.find_spec("psycopg") is not None
+        if has_psycopg3:
+            mock_kwargs = {"psycopg": m_database}
+        with patch.dict("sys.modules", **mock_kwargs):
             call_command('drop_test_database', '--noinput', verbosity=2)
 
         with self.subTest('Should check for and remove test database names until failure'):
             exists_query = "SELECT datname FROM pg_catalog.pg_database WHERE datname="
             self.assertListEqual(
                 m_cursor.execute.call_args_list,
                 [
@@ -273,15 +278,19 @@
         """Test cloned test databases created via 'manage.py test --parallel'."""
         m_database = MagicMock()
         m_cursor = Mock()
         m_database.connect.return_value.cursor.return_value = m_cursor
         # Indicate that clone databases exist up to test_test_2
         type(m_cursor).rowcount = PropertyMock(side_effect=(1, 1, 1, 0))
 
-        with patch.dict("sys.modules", psycopg2=m_database):
+        mock_kwargs = {"psycopg2": m_database}
+        has_psycopg3 = importlib.util.find_spec("psycopg") is not None
+        if has_psycopg3:
+            mock_kwargs = {"psycopg": m_database}
+        with patch.dict("sys.modules", **mock_kwargs):
             call_command('drop_test_database', '--noinput')
 
         exists_query = "SELECT datname FROM pg_catalog.pg_database WHERE datname="
         self.assertListEqual(
             m_cursor.execute.call_args_list,
             [
                 call(exists_query + "'test_test';"),
@@ -299,11 +308,15 @@
     def test_postgresql_should_not_print_Reset_successful_when_exception_occured(self, m_stdout):
         m_database = MagicMock()
         m_database.ProgrammingError = Exception
         m_cursor = Mock()
         m_cursor.execute.side_effect = m_database.ProgrammingError
         m_database.connect.return_value.cursor.return_value = m_cursor
 
-        with patch.dict("sys.modules", psycopg2=m_database):
+        mock_kwargs = {"psycopg2": m_database}
+        has_psycopg3 = importlib.util.find_spec("psycopg") is not None
+        if has_psycopg3:
+            mock_kwargs = {"psycopg": m_database}
+        with patch.dict("sys.modules", **mock_kwargs):
             call_command('drop_test_database', '--noinput', verbosity=2)
 
         self.assertNotIn("Reset successful.", m_stdout.getvalue())
```

### Comparing `django-extensions-3.2.1/tests/management/commands/test_export_emails.py` & `django-extensions-3.2.3/tests/management/commands/test_export_emails.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_generate_secret_key.py` & `django-extensions-3.2.3/tests/management/commands/test_generate_secret_key.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_graph_models.py` & `django-extensions-3.2.3/tests/management/commands/test_graph_models.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_list_signals.py` & `django-extensions-3.2.3/tests/management/commands/test_list_signals.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_managestate.py` & `django-extensions-3.2.3/tests/management/commands/test_managestate.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_notes.py` & `django-extensions-3.2.3/tests/management/commands/test_notes.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_pipchecker.py` & `django-extensions-3.2.3/tests/management/commands/test_pipchecker.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         f.write('iniconfig')
         f.write('mypy-extensions')
         f.write('packaging')
         f.write('pathspec')
         f.write('Pillow')
         f.write('pluggy')
         f.write('psycopg2-binary')
+        f.write('psycopg[binary,pool]')
         f.write('py')
         f.write('pyparsing')
         f.write('pytest')
         f.write('pytz')
         f.write('regex')
         f.write('requests')
         f.write('sentry-sdk')
```

### Comparing `django-extensions-3.2.1/tests/management/commands/test_print_settings.py` & `django-extensions-3.2.3/tests/management/commands/test_print_settings.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_print_user_for_session.py` & `django-extensions-3.2.3/tests/management/commands/test_print_user_for_session.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_reset_db.py` & `django-extensions-3.2.3/tests/management/commands/test_reset_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import importlib.util
 import os
 from io import StringIO
 
 from django.core.management import CommandError, call_command
 from django.test import TestCase
 from django.test.utils import override_settings
 
@@ -162,18 +163,22 @@
         m_cursor = mock.Mock()
         m_database.connect.return_value.cursor.return_value = m_cursor
         expected_calls = [
             mock.call('DROP DATABASE "test_db";'),
             mock.call('CREATE DATABASE "test_db" WITH OWNER = "foo"  ENCODING = \'UTF8\';'),
         ]
 
-        with mock.patch.dict("sys.modules", psycopg2=m_database):
+        mock_kwargs = {"psycopg2": m_database}
+        has_psycopg3 = importlib.util.find_spec("psycopg") is not None
+        if has_psycopg3:
+            mock_kwargs = {"psycopg": m_database}
+        with mock.patch.dict("sys.modules", **mock_kwargs):
             call_command('reset_db', '--noinput', verbosity=2)
 
-        m_database.connect.assert_called_once_with(database='template1', host='127.0.0.1', password='bar', port='5432', user='foo')
+        m_database.connect.assert_called_once_with(dbname='template1', host='127.0.0.1', password='bar', port='5432', user='foo')
 
         m_cursor.execute.assert_has_calls(expected_calls, any_order=False)
         self.assertEqual("Reset successful.\n", m_stdout.getvalue())
 
     @override_settings(DEFAULT_TABLESPACE='TEST_TABLESPACE')
     @mock.patch('sys.stdout', new_callable=StringIO)
     def test_should_drop_create_database_close_sessions_and_print_success_messsage(self, m_stdout):
@@ -182,14 +187,18 @@
         m_database.connect.return_value.cursor.return_value = m_cursor
         expected_calls = [
             mock.call("\n                    SELECT pg_terminate_backend(pg_stat_activity.pid)\n                    FROM pg_stat_activity\n                    WHERE pg_stat_activity.datname = 'test_db';\n                "),
             mock.call('DROP DATABASE "test_db";'),
             mock.call('CREATE DATABASE "test_db" WITH OWNER = "foo"  ENCODING = \'UTF8\' TABLESPACE = TEST_TABLESPACE;'),
         ]
 
-        with mock.patch.dict("sys.modules", psycopg2=m_database):
+        mock_kwargs = {"psycopg2": m_database}
+        has_psycopg3 = importlib.util.find_spec("psycopg") is not None
+        if has_psycopg3:
+            mock_kwargs = {"psycopg": m_database}
+        with mock.patch.dict("sys.modules", **mock_kwargs):
             call_command('reset_db', '--noinput', '--close-sessions', verbosity=2)
 
-        m_database.connect.assert_called_once_with(database='template1', host='127.0.0.1', password='bar', port='5432', user='foo')
+        m_database.connect.assert_called_once_with(dbname='template1', host='127.0.0.1', password='bar', port='5432', user='foo')
 
         m_cursor.execute.assert_has_calls(expected_calls, any_order=False)
         self.assertEqual("Reset successful.\n", m_stdout.getvalue())
```

### Comparing `django-extensions-3.2.1/tests/management/commands/test_reset_schema.py` & `django-extensions-3.2.3/tests/management/commands/test_reset_schema.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_runjob.py` & `django-extensions-3.2.3/tests/management/commands/test_runjob.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_set_default_site.py` & `django-extensions-3.2.3/tests/management/commands/test_set_default_site.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_set_fake_emails.py` & `django-extensions-3.2.3/tests/management/commands/test_set_fake_emails.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_set_fake_passwords.py` & `django-extensions-3.2.3/tests/management/commands/test_set_fake_passwords.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_show_template_tags.py` & `django-extensions-3.2.3/tests/management/commands/test_show_template_tags.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_show_urls.py` & `django-extensions-3.2.3/tests/management/commands/test_show_urls.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_sqlcreate.py` & `django-extensions-3.2.3/tests/management/commands/test_sqlcreate.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_sqldsn.py` & `django-extensions-3.2.3/tests/management/commands/test_sqldsn.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_sync_s3.py` & `django-extensions-3.2.3/tests/management/commands/test_sync_s3.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_syncdata.py` & `django-extensions-3.2.3/tests/management/commands/test_syncdata.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_unreferenced_files.py` & `django-extensions-3.2.3/tests/management/commands/test_unreferenced_files.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_update_permissions.py` & `django-extensions-3.2.3/tests/management/commands/test_update_permissions.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/commands/test_validate_templates.py` & `django-extensions-3.2.3/tests/management/commands/test_validate_templates.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/test_email_notifications.py` & `django-extensions-3.2.3/tests/management/test_email_notifications.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/management/test_modelviz.py` & `django-extensions-3.2.3/tests/management/test_modelviz.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/runner.py` & `django-extensions-3.2.3/tests/runner.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/templatetags/test_highlighting.py` & `django-extensions-3.2.3/tests/templatetags/test_highlighting.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.assertHTMLEqual(result, expected_result)
 
     def test_should_highlight_bash_syntax_without_name(self):
         content = """{% load highlighting %}
 {% highlight 'bash' %}
 echo "Hello $1"
 {% endhighlight %}"""
-        expected_result = '''<div class="highlight"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Hello </span><span class="nv">$1</span><span class="s2">&quot;</span>
+        expected_result = '''<div class="highlight"><pre><span></span><span class="nb">echo</span><span class="w"> </span><span class="s2">&quot;Hello </span><span class="nv">$1</span><span class="s2">&quot;</span>
 </pre></div>'''
 
         result = Template(content).render(self.ctx)
 
         self.assertHTMLEqual(result, expected_result)
```

### Comparing `django-extensions-3.2.1/tests/templatetags/test_indent_text.py` & `django-extensions-3.2.3/tests/templatetags/test_indent_text.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/templatetags/test_syntax_color.py` & `django-extensions-3.2.3/tests/templatetags/test_syntax_color.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_admin_filter.py` & `django-extensions-3.2.3/tests/test_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_admin_widgets.py` & `django-extensions-3.2.3/tests/test_admin_widgets.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_autoslug_fields.py` & `django-extensions-3.2.3/tests/test_autoslug_fields.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_clean_pyc.py` & `django-extensions-3.2.3/tests/test_clean_pyc.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_color.py` & `django-extensions-3.2.3/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_compat.py` & `django-extensions-3.2.3/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_compile_pyc.py` & `django-extensions-3.2.3/tests/test_compile_pyc.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_dumpscript.py` & `django-extensions-3.2.3/tests/test_dumpscript.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_find_template.py` & `django-extensions-3.2.3/tests/test_find_template.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_json_field.py` & `django-extensions-3.2.3/tests/test_json_field.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_logging_filters.py` & `django-extensions-3.2.3/tests/test_logging_filters.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_management_command.py` & `django-extensions-3.2.3/tests/test_management_command.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_models.py` & `django-extensions-3.2.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_modificationdatetime_fields.py` & `django-extensions-3.2.3/tests/test_modificationdatetime_fields.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_parse_mysql_cnf.py` & `django-extensions-3.2.3/tests/test_parse_mysql_cnf.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_randomchar_field.py` & `django-extensions-3.2.3/tests/test_randomchar_field.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_runscript.py` & `django-extensions-3.2.3/tests/test_runscript.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_runserver.py` & `django-extensions-3.2.3/tests/test_runserver.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_shortuuid_field.py` & `django-extensions-3.2.3/tests/test_shortuuid_field.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_sqldiff.py` & `django-extensions-3.2.3/tests/test_sqldiff.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_templatetags.py` & `django-extensions-3.2.3/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_timestamped_model.py` & `django-extensions-3.2.3/tests/test_timestamped_model.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_validators.py` & `django-extensions-3.2.3/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/test_version.py` & `django-extensions-3.2.3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/testapp/models.py` & `django-extensions-3.2.3/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/testapp/settings.py` & `django-extensions-3.2.3/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tests/testapp/urls.py` & `django-extensions-3.2.3/tests/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `django-extensions-3.2.1/tox.ini` & `django-extensions-3.2.3/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-# Tox (http://tox.testrun.org/) is a tool for running tests
+# Tox (https://tox.wiki/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
 envlist =
     precommit
     safety
     mypy
-    {py37,py38,py39,py310}-flake8
+    {py37,py38,py39,py310,py311}-flake8
     {py36,py37,py38,py39,py310,pypy}-dj32
     {py38,py39,py310,pypy}-dj40
-    {py38,py39,py310,pypy}-dj41
+    {py38,py39,py310,py311,pypy}-dj41
+    {py38,py39,py310,py311,pypy}-dj42
     {py38,py39,py310,pypy}-djmaster
     py310-dj32-postgres
     py310-dj40-postgres
     py310-dj41-postgres
+    py310-dj42-postgres
+    py310-dj42-postgres3
     py310-dj32-mysql
     py310-dj40-mysql
     py310-dj41-mysql
+    py310-dj42-mysql
     py310-djmaster-postgres
+    py310-djmaster-postgres3
 
 [testenv]
 commands = make test
 allowlist_externals = make
 passenv =
     DJANGO_EXTENSIONS_DATABASE_ENGINE
     DJANGO_EXTENSIONS_DATABASE_NAME
@@ -31,25 +36,29 @@
     DJANGO_EXTENSIONS_DATABASE_PASSWORD
     DJANGO_EXTENSIONS_DATABASE_HOST
     DJANGO_EXTENSIONS_DATABASE_PORT
 
 setenv =
     postgres: DJANGO_EXTENSIONS_DATABASE_ENGINE = {env:DJANGO_EXTENSIONS_DATABASE_ENGINE:django.db.backends.postgresql}
     postgres: DJANGO_EXTENSIONS_DATABASE_NAME = {env:DJANGO_EXTENSIONS_DATABASE_NAME:django_extensions_test}
+    postgres3: DJANGO_EXTENSIONS_DATABASE_ENGINE = {env:DJANGO_EXTENSIONS_DATABASE_ENGINE:django.db.backends.postgresql}
+    postgres3: DJANGO_EXTENSIONS_DATABASE_NAME = {env:DJANGO_EXTENSIONS_DATABASE_NAME:django_extensions_test}
     mysql: DJANGO_EXTENSIONS_DATABASE_ENGINE = {env:DJANGO_EXTENSIONS_DATABASE_ENGINE:django.db.backends.mysql}
     mysql: DJANGO_EXTENSIONS_DATABASE_NAME = {env:DJANGO_EXTENSIONS_DATABASE_NAME:django_extensions_test}
 
 deps =
     pip >= 21.1
     -rrequirements-dev.txt
     dj32: Django>=3.2,<4.0
     dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djmaster: https://github.com/django/django/archive/refs/heads/main.zip
     postgres: psycopg2-binary
+    postgres3: psycopg[binary,pool]
     mysql: mysqlclient
 
 [testenv:precommit]
 deps =
     pip >= 21.1
     pre-commit
 commands = pre-commit run -a
```

