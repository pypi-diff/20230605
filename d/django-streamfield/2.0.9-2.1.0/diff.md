# Comparing `tmp/django-streamfield-2.0.9.tar.gz` & `tmp/django-streamfield-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-streamfield-2.0.9.tar", last modified: Fri Jun  2 09:19:28 2023, max compression
+gzip compressed data, was "django-streamfield-2.1.0.tar", last modified: Mon Jun  5 10:46:52 2023, max compression
```

## Comparing `django-streamfield-2.0.9.tar` & `django-streamfield-2.1.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.346094 django-streamfield-2.0.9/
--rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/LICENSE
--rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/MANIFEST.in
--rw-r--r--   0 raagin     (501) staff       (20)    17277 2023-06-02 09:19:28.345793 django-streamfield-2.0.9/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)    16106 2023-06-02 09:14:07.000000 django-streamfield-2.0.9/README.md
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.323186 django-streamfield-2.0.9/django_streamfield.egg-info/
--rw-r--r--   0 raagin     (501) staff       (20)    17277 2023-06-02 09:19:27.000000 django-streamfield-2.0.9/django_streamfield.egg-info/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-06-02 09:19:28.000000 django-streamfield-2.0.9/django_streamfield.egg-info/SOURCES.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-06-02 09:19:27.000000 django-streamfield-2.0.9/django_streamfield.egg-info/dependency_links.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.0.9/django_streamfield.egg-info/not-zip-safe
--rw-r--r--   0 raagin     (501) staff       (20)       12 2023-06-02 09:19:27.000000 django-streamfield-2.0.9/django_streamfield.egg-info/top_level.txt
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-02 09:19:28.346186 django-streamfield-2.0.9/setup.cfg
--rw-r--r--   0 raagin     (501) staff       (20)     1421 2023-06-02 09:14:14.000000 django-streamfield-2.0.9/setup.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.330348 django-streamfield-2.0.9/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-02 09:16:40.000000 django-streamfield-2.0.9/streamfield/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.0.9/streamfield/admin.py
--rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/apps.py
--rw-r--r--   0 raagin     (501) staff       (20)     8275 2023-04-03 14:01:51.000000 django-streamfield-2.0.9/streamfield/base.py
--rw-r--r--   0 raagin     (501) staff       (20)     3673 2023-06-02 09:12:27.000000 django-streamfield-2.0.9/streamfield/fields.py
--rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.0.9/streamfield/forms.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.318795 django-streamfield-2.0.9/streamfield/locale/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.318400 django-streamfield-2.0.9/streamfield/locale/en/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.331835 django-streamfield-2.0.9/streamfield/locale/en/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.0.9/streamfield/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.0.9/streamfield/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.318641 django-streamfield-2.0.9/streamfield/locale/it/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.333195 django-streamfield-2.0.9/streamfield/locale/it/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.0.9/streamfield/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.0.9/streamfield/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.318885 django-streamfield-2.0.9/streamfield/locale/ru/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.334861 django-streamfield-2.0.9/streamfield/locale/ru/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.0.9/streamfield/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.0.9/streamfield/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/models.py
--rw-r--r--   0 raagin     (501) staff       (20)      706 2023-04-05 10:56:09.000000 django-streamfield-2.0.9/streamfield/settings.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.319123 django-streamfield-2.0.9/streamfield/static/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.337077 django-streamfield-2.0.9/streamfield/static/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)      267 2023-05-24 19:55:59.000000 django-streamfield-2.0.9/streamfield/static/streamfield/admin_popup_response.js
--rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-05-24 19:55:59.000000 django-streamfield-2.0.9/streamfield/static/streamfield/streamfield_widget.css
--rw-r--r--   0 raagin     (501) staff       (20)   302343 2023-05-24 19:55:59.000000 django-streamfield-2.0.9/streamfield/static/streamfield/streamfield_widget.js
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.319373 django-streamfield-2.0.9/streamfield/templates/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.340619 django-streamfield-2.0.9/streamfield/templates/streamfield/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.342757 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/
--rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/abstract_block_template.html
--rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/change_form.html
--rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/change_form_render_template.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.344659 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/fields/
--rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/fields/default.html
--rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/fields/select.html
--rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/admin/streamfield_popup_response.html
--rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/default_block_tmpl.html
--rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/streamfield_admin_help.html
--rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.0.9/streamfield/templates/streamfield/streamfield_widget.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-02 09:19:28.345257 django-streamfield-2.0.9/streamfield/templatetags/
--rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templatetags/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/templatetags/streamfield_tags.py
--rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.0.9/streamfield/tests.py
--rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.0.9/streamfield/urls.py
--rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.0.9/streamfield/views.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.333786 django-streamfield-2.1.0/
+-rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/LICENSE
+-rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/MANIFEST.in
+-rw-r--r--   0 raagin     (501) staff       (20)    17277 2023-06-05 10:46:52.333328 django-streamfield-2.1.0/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)    16106 2023-06-05 10:46:20.000000 django-streamfield-2.1.0/README.md
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.316352 django-streamfield-2.1.0/django_streamfield.egg-info/
+-rw-r--r--   0 raagin     (501) staff       (20)    17277 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/SOURCES.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/dependency_links.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.1.0/django_streamfield.egg-info/not-zip-safe
+-rw-r--r--   0 raagin     (501) staff       (20)       12 2023-06-05 10:46:52.000000 django-streamfield-2.1.0/django_streamfield.egg-info/top_level.txt
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 10:46:52.333911 django-streamfield-2.1.0/setup.cfg
+-rw-r--r--   0 raagin     (501) staff       (20)     1421 2023-06-05 10:46:27.000000 django-streamfield-2.1.0/setup.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.321137 django-streamfield-2.1.0/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-06-05 10:46:40.000000 django-streamfield-2.1.0/streamfield/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.1.0/streamfield/admin.py
+-rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/apps.py
+-rw-r--r--   0 raagin     (501) staff       (20)     8275 2023-04-03 14:01:51.000000 django-streamfield-2.1.0/streamfield/base.py
+-rw-r--r--   0 raagin     (501) staff       (20)     3753 2023-06-05 10:23:34.000000 django-streamfield-2.1.0/streamfield/fields.py
+-rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.1.0/streamfield/forms.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311672 django-streamfield-2.1.0/streamfield/locale/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311357 django-streamfield-2.1.0/streamfield/locale/en/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.322142 django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311553 django-streamfield-2.1.0/streamfield/locale/it/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.323068 django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.311750 django-streamfield-2.1.0/streamfield/locale/ru/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.323984 django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/models.py
+-rw-r--r--   0 raagin     (501) staff       (20)      706 2023-04-05 10:56:09.000000 django-streamfield-2.1.0/streamfield/settings.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.312054 django-streamfield-2.1.0/streamfield/static/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.325389 django-streamfield-2.1.0/streamfield/static/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)      267 2023-05-24 19:55:59.000000 django-streamfield-2.1.0/streamfield/static/streamfield/admin_popup_response.js
+-rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-05-24 19:55:59.000000 django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.css
+-rw-r--r--   0 raagin     (501) staff       (20)   302343 2023-05-24 19:55:59.000000 django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.js
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.312270 django-streamfield-2.1.0/streamfield/templates/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.327835 django-streamfield-2.1.0/streamfield/templates/streamfield/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.329837 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/
+-rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/abstract_block_template.html
+-rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/change_form.html
+-rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/change_form_render_template.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.331882 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/
+-rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/default.html
+-rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/select.html
+-rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/admin/streamfield_popup_response.html
+-rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/default_block_tmpl.html
+-rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/streamfield_admin_help.html
+-rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.1.0/streamfield/templates/streamfield/streamfield_widget.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-06-05 10:46:52.332672 django-streamfield-2.1.0/streamfield/templatetags/
+-rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templatetags/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/templatetags/streamfield_tags.py
+-rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.1.0/streamfield/tests.py
+-rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.1.0/streamfield/urls.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.1.0/streamfield/views.py
```

### Comparing `django-streamfield-2.0.9/LICENSE` & `django-streamfield-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/PKG-INFO` & `django-streamfield-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.0.9
+Version: 2.1.0
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.0.9 
+Stable version: 2.1.0 
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.0.9/README.md` & `django-streamfield-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.0.9 
+Stable version: 2.1.0 
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.0.9/django_streamfield.egg-info/PKG-INFO` & `django-streamfield-2.1.0/django_streamfield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.0.9
+Version: 2.1.0
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.0.9 
+Stable version: 2.1.0 
 Django <= 4.2.1
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.0.9/django_streamfield.egg-info/SOURCES.txt` & `django-streamfield-2.1.0/django_streamfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/setup.py` & `django-streamfield-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-streamfield",
-    version="2.0.9",
+    version="2.1.0",
     author="Yury Lapshinov",
     author_email="y.raagin@gmail.com",
     description="StreamField for native Django Admin or with Grappelli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raagin/django-streamfield",
     packages=setuptools.find_packages(exclude=['test_project', 'frontend']),
```

### Comparing `django-streamfield-2.0.9/streamfield/admin.py` & `django-streamfield-2.1.0/streamfield/admin.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/base.py` & `django-streamfield-2.1.0/streamfield/base.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/fields.py` & `django-streamfield-2.1.0/streamfield/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,15 +86,17 @@
 
     def get_prep_value(self, value):
         if isinstance(value, StreamObject):
             value = value.value
         return json.dumps(value)
 
     def get_db_prep_value(self, value, connection, prepared=False):
-        return super().get_db_prep_value(value.value, connection, prepared)
+        if value and isinstance(value, StreamObject):
+            value = value.value
+        return super().get_db_prep_value(value, connection, prepared)
 
     def value_to_string(self, obj):
         value = self.value_from_object(obj)
         return value.value
 
     def formfield(self, **kwargs):
         attrs = {}
```

### Comparing `django-streamfield-2.0.9/streamfield/locale/en/LC_MESSAGES/django.po` & `django-streamfield-2.1.0/streamfield/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/locale/it/LC_MESSAGES/django.mo` & `django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/locale/it/LC_MESSAGES/django.po` & `django-streamfield-2.1.0/streamfield/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/locale/ru/LC_MESSAGES/django.mo` & `django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/locale/ru/LC_MESSAGES/django.po` & `django-streamfield-2.1.0/streamfield/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/settings.py` & `django-streamfield-2.1.0/streamfield/settings.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/static/streamfield/streamfield_widget.css` & `django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.css`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/static/streamfield/streamfield_widget.js` & `django-streamfield-2.1.0/streamfield/static/streamfield/streamfield_widget.js`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/templates/streamfield/admin/change_form.html` & `django-streamfield-2.1.0/streamfield/templates/streamfield/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/templates/streamfield/admin/fields/file_browse_widget.html` & `django-streamfield-2.1.0/streamfield/templates/streamfield/admin/fields/file_browse_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/templates/streamfield/streamfield_widget.html` & `django-streamfield-2.1.0/streamfield/templates/streamfield/streamfield_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/templatetags/streamfield_tags.py` & `django-streamfield-2.1.0/streamfield/templatetags/streamfield_tags.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/urls.py` & `django-streamfield-2.1.0/streamfield/urls.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.9/streamfield/views.py` & `django-streamfield-2.1.0/streamfield/views.py`

 * *Files identical despite different names*

