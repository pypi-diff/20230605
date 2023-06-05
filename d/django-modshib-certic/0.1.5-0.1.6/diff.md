# Comparing `tmp/django_modshib_certic-0.1.5.tar.gz` & `tmp/django_modshib_certic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_modshib_certic-0.1.5.tar", max compression
+gzip compressed data, was "django_modshib_certic-0.1.6.tar", max compression
```

## Comparing `django_modshib_certic-0.1.5.tar` & `django_modshib_certic-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/admin.py
--rw-r--r--   0        0        0      146 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/apps.py
--rw-r--r--   0        0        0      400 2023-06-01 08:51:10.568109 django_modshib_certic-0.1.5/modshib/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/models.py
--rw-r--r--   0        0        0      896 2023-06-02 14:33:23.664664 django_modshib_certic-0.1.5/modshib/templates/registration/logged_out.html
--rw-r--r--   0        0        0     3065 2023-06-02 15:32:51.152782 django_modshib_certic-0.1.5/modshib/templates/registration/login.html
--rw-r--r--   0        0        0     1012 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/templates/registration/reg_base.html
--rw-r--r--   0        0        0      811 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/templates/registration/sso_fail.html
--rw-r--r--   0        0        0      830 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/templates/registration/sso_no_account.html
--rw-r--r--   0        0        0       60 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.5/modshib/tests.py
--rw-r--r--   0        0        0      117 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.5/modshib/urls.py
--rw-r--r--   0        0        0     2746 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/views.py
--rw-r--r--   0        0        0      550 2023-06-02 15:33:48.796784 django_modshib_certic-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 django_modshib_certic-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/admin.py
+-rw-r--r--   0        0        0      146 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/apps.py
+-rw-r--r--   0        0        0      400 2023-06-01 08:51:10.568109 django_modshib_certic-0.1.6/modshib/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/models.py
+-rw-r--r--   0        0        0      896 2023-06-02 14:33:23.664664 django_modshib_certic-0.1.6/modshib/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     3065 2023-06-02 15:32:51.152782 django_modshib_certic-0.1.6/modshib/templates/registration/login.html
+-rw-r--r--   0        0        0     1032 2023-06-05 14:35:51.956852 django_modshib_certic-0.1.6/modshib/templates/registration/reg_base.html
+-rw-r--r--   0        0        0      811 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.6/modshib/templates/registration/sso_fail.html
+-rw-r--r--   0        0        0      830 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.6/modshib/templates/registration/sso_no_account.html
+-rw-r--r--   0        0        0       60 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.6/modshib/tests.py
+-rw-r--r--   0        0        0      117 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.6/modshib/urls.py
+-rw-r--r--   0        0        0     2746 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.6/modshib/views.py
+-rw-r--r--   0        0        0      550 2023-06-05 14:36:13.932852 django_modshib_certic-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 django_modshib_certic-0.1.6/PKG-INFO
```

### Comparing `django_modshib_certic-0.1.5/modshib/templates/registration/logged_out.html` & `django_modshib_certic-0.1.6/modshib/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.5/modshib/templates/registration/login.html` & `django_modshib_certic-0.1.6/modshib/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.5/modshib/templates/registration/reg_base.html` & `django_modshib_certic-0.1.6/modshib/templates/registration/reg_base.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load i18n %}
 <!doctype html>
 <html lang="{% get_current_language as LANGUAGE_CODE %}">
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <title>{% block head_title %}Titre{% endblock head_title %} - {{ site_name }}</title>
+    <title>{% block head_title %}Titre{% endblock head_title %} - {% translate MODSHIB_FORMS_TITLE %}</title>
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet"
           integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"
             integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4"
             crossorigin="anonymous"></script>
     {% if MODSHIB_STYLESHEET_URL is not null %}
         <link href="{{ MODSHIB_STYLESHEET_URL }}" rel="stylesheet" crossorigin="anonymous">
```

### Comparing `django_modshib_certic-0.1.5/modshib/templates/registration/sso_fail.html` & `django_modshib_certic-0.1.6/modshib/templates/registration/sso_fail.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.5/modshib/templates/registration/sso_no_account.html` & `django_modshib_certic-0.1.6/modshib/templates/registration/sso_no_account.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.5/modshib/views.py` & `django_modshib_certic-0.1.6/modshib/views.py`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.5/pyproject.toml` & `django_modshib_certic-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-modshib-CERTIC"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>"]
 license = "Cecill-B"
 packages = [
     { include = "modshib"},
 ]
 homepage = "https://www.certic.unicaen.fr"
```

### Comparing `django_modshib_certic-0.1.5/PKG-INFO` & `django_modshib_certic-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modshib-certic
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://www.certic.unicaen.fr
 License: CECILL-B
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
```

