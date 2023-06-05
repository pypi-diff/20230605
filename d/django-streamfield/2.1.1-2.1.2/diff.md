# Comparing `tmp/django-streamfield-2.1.1.tar.gz` & `tmp/django-streamfield-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-streamfield-2.1.1.tar", last modified: Mon Jun  5 14:18:03 2023, max compression
+gzip compressed data, was "django-streamfield-2.1.2.tar", last modified: Mon Jun  5 16:02:53 2023, max compression
```

## Comparing `django-streamfield-2.1.1.tar` & `django-streamfield-2.1.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.450133 django-streamfield-2.1.1/
--rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/LICENSE
--rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/MANIFEST.in
--rw-r--r--   0 raagin     (501) staff       (20)    17050 2023-06-05 14:18:03.449614 django-streamfield-2.1.1/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)    16105 2023-06-05 13:57:08.000000 django-streamfield-2.1.1/README.md
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.422575 django-streamfield-2.1.1/django_streamfield.egg-info/
--rw-r--r--   0 raagin     (501) staff       (20)    17050 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/SOURCES.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/dependency_links.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.1.1/django_streamfield.egg-info/not-zip-safe
--rw-r--r--   0 raagin     (501) staff       (20)       12 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/top_level.txt
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 14:18:03.450275 django-streamfield-2.1.1/setup.cfg
--rw-r--r--   0 raagin     (501) staff       (20)     1200 2023-06-05 13:58:21.000000 django-streamfield-2.1.1/setup.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.430244 django-streamfield-2.1.1/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 13:58:36.000000 django-streamfield-2.1.1/streamfield/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.1.1/streamfield/admin.py
--rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/apps.py
--rw-r--r--   0 raagin     (501) staff       (20)     8674 2023-06-05 13:59:13.000000 django-streamfield-2.1.1/streamfield/base.py
--rw-r--r--   0 raagin     (501) staff       (20)     3753 2023-06-05 10:23:34.000000 django-streamfield-2.1.1/streamfield/fields.py
--rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.1.1/streamfield/forms.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416852 django-streamfield-2.1.1/streamfield/locale/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416277 django-streamfield-2.1.1/streamfield/locale/en/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.432036 django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416632 django-streamfield-2.1.1/streamfield/locale/it/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.433229 django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416992 django-streamfield-2.1.1/streamfield/locale/ru/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.434607 django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/models.py
--rw-r--r--   0 raagin     (501) staff       (20)      706 2023-04-05 10:56:09.000000 django-streamfield-2.1.1/streamfield/settings.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.417336 django-streamfield-2.1.1/streamfield/static/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.436797 django-streamfield-2.1.1/streamfield/static/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)      267 2023-05-24 19:55:59.000000 django-streamfield-2.1.1/streamfield/static/streamfield/admin_popup_response.js
--rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-05-24 19:55:59.000000 django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.css
--rw-r--r--   0 raagin     (501) staff       (20)   302343 2023-05-24 19:55:59.000000 django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.js
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.417673 django-streamfield-2.1.1/streamfield/templates/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.442248 django-streamfield-2.1.1/streamfield/templates/streamfield/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.445317 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/
--rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/abstract_block_template.html
--rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/change_form.html
--rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/change_form_render_template.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.447827 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/
--rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/default.html
--rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/select.html
--rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/streamfield_popup_response.html
--rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/default_block_tmpl.html
--rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/streamfield_admin_help.html
--rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/streamfield_widget.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.448693 django-streamfield-2.1.1/streamfield/templatetags/
--rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templatetags/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templatetags/streamfield_tags.py
--rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/tests.py
--rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.1.1/streamfield/urls.py
--rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.1.1/streamfield/views.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.384773 django-streamfield-2.1.2/
+-rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/LICENSE
+-rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/MANIFEST.in
+-rw-r--r--   0 raagin     (501) staff       (20)    17050 2023-06-05 16:02:53.383288 django-streamfield-2.1.2/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)    16105 2023-06-05 16:01:28.000000 django-streamfield-2.1.2/README.md
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.351094 django-streamfield-2.1.2/django_streamfield.egg-info/
+-rw-r--r--   0 raagin     (501) staff       (20)    17050 2023-06-05 16:02:53.000000 django-streamfield-2.1.2/django_streamfield.egg-info/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-06-05 16:02:53.000000 django-streamfield-2.1.2/django_streamfield.egg-info/SOURCES.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-06-05 16:02:53.000000 django-streamfield-2.1.2/django_streamfield.egg-info/dependency_links.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.1.2/django_streamfield.egg-info/not-zip-safe
+-rw-r--r--   0 raagin     (501) staff       (20)       12 2023-06-05 16:02:53.000000 django-streamfield-2.1.2/django_streamfield.egg-info/top_level.txt
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 16:02:53.385053 django-streamfield-2.1.2/setup.cfg
+-rw-r--r--   0 raagin     (501) staff       (20)     1200 2023-06-05 16:01:33.000000 django-streamfield-2.1.2/setup.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.357998 django-streamfield-2.1.2/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 16:01:42.000000 django-streamfield-2.1.2/streamfield/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.1.2/streamfield/admin.py
+-rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/apps.py
+-rw-r--r--   0 raagin     (501) staff       (20)     9244 2023-06-05 15:56:37.000000 django-streamfield-2.1.2/streamfield/base.py
+-rw-r--r--   0 raagin     (501) staff       (20)     3753 2023-06-05 10:23:34.000000 django-streamfield-2.1.2/streamfield/fields.py
+-rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.1.2/streamfield/forms.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.345709 django-streamfield-2.1.2/streamfield/locale/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.345331 django-streamfield-2.1.2/streamfield/locale/en/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.359980 django-streamfield-2.1.2/streamfield/locale/en/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.1.2/streamfield/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.1.2/streamfield/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.345565 django-streamfield-2.1.2/streamfield/locale/it/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.362606 django-streamfield-2.1.2/streamfield/locale/it/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.1.2/streamfield/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.1.2/streamfield/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.345795 django-streamfield-2.1.2/streamfield/locale/ru/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.364708 django-streamfield-2.1.2/streamfield/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.1.2/streamfield/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.1.2/streamfield/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/models.py
+-rw-r--r--   0 raagin     (501) staff       (20)      706 2023-04-05 10:56:09.000000 django-streamfield-2.1.2/streamfield/settings.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.346023 django-streamfield-2.1.2/streamfield/static/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.367560 django-streamfield-2.1.2/streamfield/static/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)      267 2023-05-24 19:55:59.000000 django-streamfield-2.1.2/streamfield/static/streamfield/admin_popup_response.js
+-rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-05-24 19:55:59.000000 django-streamfield-2.1.2/streamfield/static/streamfield/streamfield_widget.css
+-rw-r--r--   0 raagin     (501) staff       (20)   302343 2023-05-24 19:55:59.000000 django-streamfield-2.1.2/streamfield/static/streamfield/streamfield_widget.js
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.346251 django-streamfield-2.1.2/streamfield/templates/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.372997 django-streamfield-2.1.2/streamfield/templates/streamfield/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.376316 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/
+-rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/abstract_block_template.html
+-rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/change_form.html
+-rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/change_form_render_template.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.379148 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/fields/
+-rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/fields/default.html
+-rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/fields/select.html
+-rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/admin/streamfield_popup_response.html
+-rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/default_block_tmpl.html
+-rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/streamfield_admin_help.html
+-rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.1.2/streamfield/templates/streamfield/streamfield_widget.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 16:02:53.380445 django-streamfield-2.1.2/streamfield/templatetags/
+-rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templatetags/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/templatetags/streamfield_tags.py
+-rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.1.2/streamfield/tests.py
+-rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.1.2/streamfield/urls.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.1.2/streamfield/views.py
```

### Comparing `django-streamfield-2.1.1/LICENSE` & `django-streamfield-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/PKG-INFO` & `django-streamfield-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.1.1
+Version: 2.1.2
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.1.1
+Stable version: 2.1.2
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.1.1/README.md` & `django-streamfield-2.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.1.1
+Stable version: 2.1.2
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.1.1/django_streamfield.egg-info/PKG-INFO` & `django-streamfield-2.1.2/django_streamfield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.1.1
+Version: 2.1.2
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.1.1
+Stable version: 2.1.2
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.1.1/django_streamfield.egg-info/SOURCES.txt` & `django-streamfield-2.1.2/django_streamfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/setup.py` & `django-streamfield-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-streamfield",
-    version="2.1.1",
+    version="2.1.2",
     author="Yury Lapshinov",
     author_email="y.raagin@gmail.com",
     description="StreamField for native Django Admin or with Grappelli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raagin/django-streamfield",
     packages=setuptools.find_packages(exclude=['test_project', 'frontend']),
```

### Comparing `django-streamfield-2.1.1/streamfield/admin.py` & `django-streamfield-2.1.2/streamfield/admin.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/base.py` & `django-streamfield-2.1.2/streamfield/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -134,18 +134,32 @@
             model_list=self.model_list
             )
 
     def to_json(self):
         return json.dumps(self.value)
 
     def add(self, block):
-        model_class = block.__class__
+        if isinstance(block, list):
+            model_class = block[0].__class__
+            if hasattr(model_class, 'as_list') and model_class.as_list:
+                id = []
+                for b in block:
+                    if b.__class__ != model_class:
+                        raise ValueError("not all list objects have the same model class")
+                    else:
+                        id.append(b.id)
+            else:
+                raise ValueError("block is list. but model hasn't as_list property")
+        else:
+            model_class = block.__class__
+            id = block.id
+            
         options = _get_default_options(model_class)
         self.value.append({
-            "id": block.id, 
+            "id": id,
             "options": options, 
             "unique_id": uuid4().hex[:6], 
             "model_name": model_class.__name__
         })
 
     @cached_property
     def help_text(self):
```

### Comparing `django-streamfield-2.1.1/streamfield/fields.py` & `django-streamfield-2.1.2/streamfield/fields.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/django.po` & `django-streamfield-2.1.2/streamfield/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.mo` & `django-streamfield-2.1.2/streamfield/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.po` & `django-streamfield-2.1.2/streamfield/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.mo` & `django-streamfield-2.1.2/streamfield/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.po` & `django-streamfield-2.1.2/streamfield/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/settings.py` & `django-streamfield-2.1.2/streamfield/settings.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.css` & `django-streamfield-2.1.2/streamfield/static/streamfield/streamfield_widget.css`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.js` & `django-streamfield-2.1.2/streamfield/static/streamfield/streamfield_widget.js`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/templates/streamfield/admin/change_form.html` & `django-streamfield-2.1.2/streamfield/templates/streamfield/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/file_browse_widget.html` & `django-streamfield-2.1.2/streamfield/templates/streamfield/admin/fields/file_browse_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/templates/streamfield/streamfield_widget.html` & `django-streamfield-2.1.2/streamfield/templates/streamfield/streamfield_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/templatetags/streamfield_tags.py` & `django-streamfield-2.1.2/streamfield/templatetags/streamfield_tags.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/urls.py` & `django-streamfield-2.1.2/streamfield/urls.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.1/streamfield/views.py` & `django-streamfield-2.1.2/streamfield/views.py`

 * *Files identical despite different names*

