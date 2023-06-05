# Comparing `tmp/django-streamfield-2.1.0.tar.gz` & `tmp/django-streamfield-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-streamfield-2.1.0.tar", last modified: Mon Jun  5 10:46:52 2023, max compression
+gzip compressed data, was "django-streamfield-2.1.1.tar", last modified: Mon Jun  5 14:18:03 2023, max compression
```

## Comparing `django-streamfield-2.1.0.tar` & `django-streamfield-2.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.333786 django-streamfield-2.1.0/
--rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/LICENSE
--rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/MANIFEST.in
--rw-r--r--   0 raagin     (501) staff       (20)    17277 2023-06-05 10:46:52.333328 django-streamfield-2.1.0/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)    16106 2023-06-05 10:46:20.000000 django-streamfield-2.1.0/README.md
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.316352 django-streamfield-2.1.0/django_streamfield.egg-info/
--rw-r--r--   0 raagin     (501) staff       (20)    17277 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/SOURCES.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/dependency_links.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.1.0/django_streamfield.egg-info/not-zip-safe
--rw-r--r--   0 raagin     (501) staff       (20)       12 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/top_level.txt
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 10:46:52.333911 django-streamfield-2.1.0/setup.cfg
--rw-r--r--   0 raagin     (501) staff       (20)     1421 2023-06-05 10:46:27.000000 django-streamfield-2.1.0/setup.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.321137 django-streamfield-2.1.0/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 10:46:40.000000 django-streamfield-2.1.0/streamfield/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.1.0/streamfield/admin.py
--rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/apps.py
--rw-r--r--   0 raagin     (501) staff       (20)     8275 2023-04-03 14:01:51.000000 django-streamfield-2.1.0/streamfield/base.py
--rw-r--r--   0 raagin     (501) staff       (20)     3753 2023-06-05 10:23:34.000000 django-streamfield-2.1.0/streamfield/fields.py
--rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.1.0/streamfield/forms.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311672 django-streamfield-2.1.0/streamfield/locale/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311357 django-streamfield-2.1.0/streamfield/locale/en/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.322142 django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311553 django-streamfield-2.1.0/streamfield/locale/it/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.323068 django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311750 django-streamfield-2.1.0/streamfield/locale/ru/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.323984 django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/models.py
--rw-r--r--   0 raagin     (501) staff       (20)      706 2023-04-05 10:56:09.000000 django-streamfield-2.1.0/streamfield/settings.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.312054 django-streamfield-2.1.0/streamfield/static/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.325389 django-streamfield-2.1.0/streamfield/static/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)      267 2023-05-24 19:55:59.000000 django-streamfield-2.1.0/streamfield/static/streamfield/admin_popup_response.js
--rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-05-24 19:55:59.000000 django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.css
--rw-r--r--   0 raagin     (501) staff       (20)   302343 2023-05-24 19:55:59.000000 django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.js
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.312270 django-streamfield-2.1.0/streamfield/templates/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.327835 django-streamfield-2.1.0/streamfield/templates/streamfield/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.329837 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/
--rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/abstract_block_template.html
--rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/change_form.html
--rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/change_form_render_template.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.331882 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/
--rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/default.html
--rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/select.html
--rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/streamfield_popup_response.html
--rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/default_block_tmpl.html
--rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/streamfield_admin_help.html
--rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/streamfield_widget.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.332672 django-streamfield-2.1.0/streamfield/templatetags/
--rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templatetags/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templatetags/streamfield_tags.py
--rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/tests.py
--rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.1.0/streamfield/urls.py
--rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.1.0/streamfield/views.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.450133 django-streamfield-2.1.1/
+-rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/LICENSE
+-rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/MANIFEST.in
+-rw-r--r--   0 raagin     (501) staff       (20)    17050 2023-06-05 14:18:03.449614 django-streamfield-2.1.1/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)    16105 2023-06-05 13:57:08.000000 django-streamfield-2.1.1/README.md
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.422575 django-streamfield-2.1.1/django_streamfield.egg-info/
+-rw-r--r--   0 raagin     (501) staff       (20)    17050 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/SOURCES.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/dependency_links.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.1.1/django_streamfield.egg-info/not-zip-safe
+-rw-r--r--   0 raagin     (501) staff       (20)       12 2023-06-05 14:18:03.000000 django-streamfield-2.1.1/django_streamfield.egg-info/top_level.txt
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 14:18:03.450275 django-streamfield-2.1.1/setup.cfg
+-rw-r--r--   0 raagin     (501) staff       (20)     1200 2023-06-05 13:58:21.000000 django-streamfield-2.1.1/setup.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.430244 django-streamfield-2.1.1/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 13:58:36.000000 django-streamfield-2.1.1/streamfield/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.1.1/streamfield/admin.py
+-rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/apps.py
+-rw-r--r--   0 raagin     (501) staff       (20)     8674 2023-06-05 13:59:13.000000 django-streamfield-2.1.1/streamfield/base.py
+-rw-r--r--   0 raagin     (501) staff       (20)     3753 2023-06-05 10:23:34.000000 django-streamfield-2.1.1/streamfield/fields.py
+-rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.1.1/streamfield/forms.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416852 django-streamfield-2.1.1/streamfield/locale/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416277 django-streamfield-2.1.1/streamfield/locale/en/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.432036 django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416632 django-streamfield-2.1.1/streamfield/locale/it/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.433229 django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.416992 django-streamfield-2.1.1/streamfield/locale/ru/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.434607 django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/models.py
+-rw-r--r--   0 raagin     (501) staff       (20)      706 2023-04-05 10:56:09.000000 django-streamfield-2.1.1/streamfield/settings.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.417336 django-streamfield-2.1.1/streamfield/static/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.436797 django-streamfield-2.1.1/streamfield/static/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)      267 2023-05-24 19:55:59.000000 django-streamfield-2.1.1/streamfield/static/streamfield/admin_popup_response.js
+-rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-05-24 19:55:59.000000 django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.css
+-rw-r--r--   0 raagin     (501) staff       (20)   302343 2023-05-24 19:55:59.000000 django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.js
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.417673 django-streamfield-2.1.1/streamfield/templates/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.442248 django-streamfield-2.1.1/streamfield/templates/streamfield/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.445317 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/
+-rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/abstract_block_template.html
+-rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/change_form.html
+-rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/change_form_render_template.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.447827 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/
+-rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/default.html
+-rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/select.html
+-rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/admin/streamfield_popup_response.html
+-rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/default_block_tmpl.html
+-rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/streamfield_admin_help.html
+-rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.1.1/streamfield/templates/streamfield/streamfield_widget.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 14:18:03.448693 django-streamfield-2.1.1/streamfield/templatetags/
+-rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templatetags/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/templatetags/streamfield_tags.py
+-rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.1.1/streamfield/tests.py
+-rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.1.1/streamfield/urls.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.1.1/streamfield/views.py
```

### Comparing `django-streamfield-2.1.0/LICENSE` & `django-streamfield-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/PKG-INFO` & `django-streamfield-2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,11 @@
-Metadata-Version: 2.1
-Name: django-streamfield
-Version: 2.1.0
-Summary: StreamField for native Django Admin or with Grappelli
-Home-page: https://github.com/raagin/django-streamfield
-Author: Yury Lapshinov
-Author-email: y.raagin@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.1.0 
+Stable version: 2.1.1
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
@@ -567,9 +536,7 @@
 
     operations = [
         migrations.RunPython(migrate_options),
     ]
 ```
 
 
-
-
```

### Comparing `django-streamfield-2.1.0/README.md` & `django-streamfield-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,37 @@
+Metadata-Version: 2.1
+Name: django-streamfield
+Version: 2.1.1
+Summary: StreamField for native Django Admin or with Grappelli
+Home-page: https://github.com/raagin/django-streamfield
+Author: Yury Lapshinov
+Author-email: y.raagin@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.1.0 
+Stable version: 2.1.1
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
@@ -536,7 +562,9 @@
 
     operations = [
         migrations.RunPython(migrate_options),
     ]
 ```
 
 
+
+
```

### Comparing `django-streamfield-2.1.0/django_streamfield.egg-info/PKG-INFO` & `django-streamfield-2.1.1/django_streamfield.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.1.0
+Version: 2.1.1
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.1.0 
+Stable version: 2.1.1
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.1.0/django_streamfield.egg-info/SOURCES.txt` & `django-streamfield-2.1.1/django_streamfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/admin.py` & `django-streamfield-2.1.1/streamfield/admin.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/base.py` & `django-streamfield-2.1.1/streamfield/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,24 @@
             value=self._iterate_over_models(_copy),
             model_list=self.model_list
             )
 
     def to_json(self):
         return json.dumps(self.value)
 
+    def add(self, block):
+        model_class = block.__class__
+        options = _get_default_options(model_class)
+        self.value.append({
+            "id": block.id, 
+            "options": options, 
+            "unique_id": uuid4().hex[:6], 
+            "model_name": model_class.__name__
+        })
+
     @cached_property
     def help_text(self):
         return ADMIN_HELP_TEXT
 
 
 
 def _get_block_tmpl(model_class, model_str):
@@ -193,14 +203,22 @@
             changed = True
             value = getattr(obj, f.name)
             # value is StreamObject
             setattr(obj, f.name, value.copy())
     if changed:
         obj.save()
 
+def _get_default_options(model_class):
+    options = model_class.options if hasattr(model_class, "options") else BLOCK_OPTIONS
+    if hasattr(model_class, "extra_options"):
+        options = deepcopy(options)
+        options.update(model_class.extra_options)
+    options = { k: v['default'] for k, v in options.items() if bool(v.get('default')) }
+    return options
+
 def _copy(model_class, model_str, content, ctx):
     as_list = ctx['as_list']
     resp = dict(
         unique_id=uuid4().hex[:6],
         model_name=model_str,
         options=ctx['options']
         ) 
@@ -245,18 +263,14 @@
     Receive StreamObject from StreamField in your model
     Return updated StreamObject, with new default options.  
     At the moment this only works with unique streamblocks class names.  
     """
     stream_dict = stream_obj.from_json()
     for b in stream_dict:
         model_class = get_model_by_string(b['model_name'])
-        options = model_class.options if hasattr(model_class, "options") else BLOCK_OPTIONS
-        if hasattr(model_class, "extra_options"):
-            options = deepcopy(options)
-            options.update(model_class.extra_options)
-        options = { k: v['default'] for k, v in options.items() if bool(v.get('default')) }
+        options = _get_default_options(model_class)
         options.update(b['options'])
         b['options'] = options
     return StreamObject(
         stream_dict, 
         stream_obj.model_list
         )
```

### Comparing `django-streamfield-2.1.0/streamfield/fields.py` & `django-streamfield-2.1.1/streamfield/fields.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/django.po` & `django-streamfield-2.1.1/streamfield/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.mo` & `django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.po` & `django-streamfield-2.1.1/streamfield/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.mo` & `django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.po` & `django-streamfield-2.1.1/streamfield/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/settings.py` & `django-streamfield-2.1.1/streamfield/settings.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.css` & `django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.css`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.js` & `django-streamfield-2.1.1/streamfield/static/streamfield/streamfield_widget.js`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/templates/streamfield/admin/change_form.html` & `django-streamfield-2.1.1/streamfield/templates/streamfield/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/file_browse_widget.html` & `django-streamfield-2.1.1/streamfield/templates/streamfield/admin/fields/file_browse_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/templates/streamfield/streamfield_widget.html` & `django-streamfield-2.1.1/streamfield/templates/streamfield/streamfield_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/templatetags/streamfield_tags.py` & `django-streamfield-2.1.1/streamfield/templatetags/streamfield_tags.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/urls.py` & `django-streamfield-2.1.1/streamfield/urls.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.1.0/streamfield/views.py` & `django-streamfield-2.1.1/streamfield/views.py`

 * *Files identical despite different names*

