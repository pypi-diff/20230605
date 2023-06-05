# Comparing `tmp/django-magicauth-0.8.tar.gz` & `tmp/django-magicauth-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magicauth-0.8.tar", last modified: Wed Mar 23 16:25:20 2022, max compression
+gzip compressed data, was "django-magicauth-0.9.tar", last modified: Wed Mar 23 16:33:27 2022, max compression
```

## Comparing `django-magicauth-0.8.tar` & `django-magicauth-0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:25:20.979891 django-magicauth-0.8/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1068 2021-12-04 16:03:09.000000 django-magicauth-0.8/LICENSE
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       74 2021-12-04 16:03:09.000000 django-magicauth-0.8/MANIFEST.in
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     7468 2022-03-23 16:25:20.979891 django-magicauth-0.8/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     6776 2022-03-23 16:14:06.000000 django-magicauth-0.8/README.md
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:25:20.971891 django-magicauth-0.8/django_magicauth.egg-info/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     7468 2022-03-23 16:25:20.000000 django-magicauth-0.8/django_magicauth.egg-info/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      956 2022-03-23 16:25:20.000000 django-magicauth-0.8/django_magicauth.egg-info/SOURCES.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        1 2022-03-23 16:25:20.000000 django-magicauth-0.8/django_magicauth.egg-info/dependency_links.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       16 2022-03-23 16:25:20.000000 django-magicauth-0.8/django_magicauth.egg-info/top_level.txt
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:25:20.975891 django-magicauth-0.8/magicauth/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2022-03-03 10:29:41.000000 django-magicauth-0.8/magicauth/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      212 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/admin.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      125 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/apps.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      704 2022-03-03 10:29:41.000000 django-magicauth-0.8/magicauth/forms.py
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:25:20.975891 django-magicauth-0.8/magicauth/migrations/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1364 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/migrations/0001_initial.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/migrations/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      668 2022-03-03 10:26:51.000000 django-magicauth-0.8/magicauth/models.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1691 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/next_url.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1328 2022-03-03 10:29:41.000000 django-magicauth-0.8/magicauth/otp_forms.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2435 2022-03-23 16:14:06.000000 django-magicauth-0.8/magicauth/send_token.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     5140 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/settings.py
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:25:20.967891 django-magicauth-0.8/magicauth/templates/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:25:20.975891 django-magicauth-0.8/magicauth/templates/magicauth/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)    10163 2022-03-23 16:14:06.000000 django-magicauth-0.8/magicauth/templates/magicauth/email.html
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      373 2022-03-23 16:14:06.000000 django-magicauth-0.8/magicauth/templates/magicauth/email.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      972 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/templates/magicauth/email_sent.html
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1995 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/templates/magicauth/login.html
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      934 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/templates/magicauth/wait.html
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      698 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/urls.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      423 2021-12-04 16:03:09.000000 django-magicauth-0.8/magicauth/utils.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     5957 2022-03-03 10:29:41.000000 django-magicauth-0.8/magicauth/views.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       38 2022-03-23 16:25:20.979891 django-magicauth-0.8/setup.cfg
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1087 2022-03-23 16:21:26.000000 django-magicauth-0.8/setup.py
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:25:20.979891 django-magicauth-0.8/tests/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2021-12-04 16:03:09.000000 django-magicauth-0.8/tests/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      572 2021-12-04 16:03:09.000000 django-magicauth-0.8/tests/factories.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2043 2021-12-04 16:03:09.000000 django-magicauth-0.8/tests/test_1_GET_login_view.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     5281 2022-03-03 10:26:51.000000 django-magicauth-0.8/tests/test_2_POST_login_view.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      912 2021-12-04 16:03:09.000000 django-magicauth-0.8/tests/test_3_email_sent_view.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2109 2021-12-04 16:03:09.000000 django-magicauth-0.8/tests/test_4_wait_view.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     4235 2021-12-04 16:03:09.000000 django-magicauth-0.8/tests/test_5_validate_token_view.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      869 2022-03-23 16:14:06.000000 django-magicauth-0.8/tests/test_settings.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      247 2021-12-04 16:03:09.000000 django-magicauth-0.8/tests/test_url.py
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:33:27.874362 django-magicauth-0.9/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1068 2021-12-04 16:03:09.000000 django-magicauth-0.9/LICENSE
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       74 2021-12-04 16:03:09.000000 django-magicauth-0.9/MANIFEST.in
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     7648 2022-03-23 16:33:27.874362 django-magicauth-0.9/PKG-INFO
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     6956 2022-03-23 16:31:43.000000 django-magicauth-0.9/README.md
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:33:27.870362 django-magicauth-0.9/django_magicauth.egg-info/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     7648 2022-03-23 16:33:27.000000 django-magicauth-0.9/django_magicauth.egg-info/PKG-INFO
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      956 2022-03-23 16:33:27.000000 django-magicauth-0.9/django_magicauth.egg-info/SOURCES.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        1 2022-03-23 16:33:27.000000 django-magicauth-0.9/django_magicauth.egg-info/dependency_links.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       16 2022-03-23 16:33:27.000000 django-magicauth-0.9/django_magicauth.egg-info/top_level.txt
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:33:27.870362 django-magicauth-0.9/magicauth/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2022-03-03 10:29:41.000000 django-magicauth-0.9/magicauth/__init__.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      212 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/admin.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      125 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/apps.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      704 2022-03-03 10:29:41.000000 django-magicauth-0.9/magicauth/forms.py
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:33:27.870362 django-magicauth-0.9/magicauth/migrations/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1364 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/migrations/0001_initial.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/migrations/__init__.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      668 2022-03-03 10:26:51.000000 django-magicauth-0.9/magicauth/models.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1691 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/next_url.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1328 2022-03-03 10:29:41.000000 django-magicauth-0.9/magicauth/otp_forms.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2659 2022-03-23 16:31:43.000000 django-magicauth-0.9/magicauth/send_token.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     5140 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/settings.py
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:33:27.866362 django-magicauth-0.9/magicauth/templates/
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:33:27.870362 django-magicauth-0.9/magicauth/templates/magicauth/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)    10163 2022-03-23 16:31:43.000000 django-magicauth-0.9/magicauth/templates/magicauth/email.html
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      373 2022-03-23 16:31:43.000000 django-magicauth-0.9/magicauth/templates/magicauth/email.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      972 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/templates/magicauth/email_sent.html
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1995 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/templates/magicauth/login.html
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      934 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/templates/magicauth/wait.html
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      698 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/urls.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      423 2021-12-04 16:03:09.000000 django-magicauth-0.9/magicauth/utils.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     5957 2022-03-03 10:29:41.000000 django-magicauth-0.9/magicauth/views.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       38 2022-03-23 16:33:27.874362 django-magicauth-0.9/setup.cfg
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1087 2022-03-23 16:32:23.000000 django-magicauth-0.9/setup.py
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2022-03-23 16:33:27.874362 django-magicauth-0.9/tests/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2021-12-04 16:03:09.000000 django-magicauth-0.9/tests/__init__.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      572 2021-12-04 16:03:09.000000 django-magicauth-0.9/tests/factories.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2043 2021-12-04 16:03:09.000000 django-magicauth-0.9/tests/test_1_GET_login_view.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     5281 2022-03-03 10:26:51.000000 django-magicauth-0.9/tests/test_2_POST_login_view.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      912 2021-12-04 16:03:09.000000 django-magicauth-0.9/tests/test_3_email_sent_view.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2109 2021-12-04 16:03:09.000000 django-magicauth-0.9/tests/test_4_wait_view.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     4235 2021-12-04 16:03:09.000000 django-magicauth-0.9/tests/test_5_validate_token_view.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      910 2022-03-23 16:31:43.000000 django-magicauth-0.9/tests/test_settings.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      247 2021-12-04 16:03:09.000000 django-magicauth-0.9/tests/test_url.py
```

### Comparing `django-magicauth-0.8/LICENSE` & `django-magicauth-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/PKG-INFO` & `django-magicauth-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magicauth
-Version: 0.8
+Version: 0.9
 Summary: Password-less authentication: login by clicking on a magic link received by email.
 Home-page: 
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -93,14 +93,18 @@
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.sites.middleware.CurrentSiteMiddleware",
 ]
 ```
 
+7. Configure the projet's domain name using the `Site` model and, if needed, the corresponding `SITE_ID`.
+If you dont configure the domain name, it will default to the URL path.
+
+
 ## Two-Factor Authentication (2FA) using One Time Passwords (OTP)
 
 Two-Factor Authentication means you ask for two different passwords from your user : their normal password and an OTP. (See https://en.wikipedia.org/wiki/Multi-factor_authentication)
 They will get the magic link only if the two are valid, else they get an error and the link is not sent.
 
 What is a OTP ? It is a short code (6 to 8 digits), usually generated by a dedicated app on a user's device (smartphone, hardware). See https://en.wikipedia.org/wiki/Time-based_One-time_Password_algorithm
```

### Comparing `django-magicauth-0.8/README.md` & `django-magicauth-0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,18 @@
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.sites.middleware.CurrentSiteMiddleware",
 ]
 ```
 
+7. Configure the projet's domain name using the `Site` model and, if needed, the corresponding `SITE_ID`.
+If you dont configure the domain name, it will default to the URL path.
+
+
 ## Two-Factor Authentication (2FA) using One Time Passwords (OTP)
 
 Two-Factor Authentication means you ask for two different passwords from your user : their normal password and an OTP. (See https://en.wikipedia.org/wiki/Multi-factor_authentication)
 They will get the magic link only if the two are valid, else they get an error and the link is not sent.
 
 What is a OTP ? It is a short code (6 to 8 digits), usually generated by a dedicated app on a user's device (smartphone, hardware). See https://en.wikipedia.org/wiki/Time-based_One-time_Password_algorithm
```

### Comparing `django-magicauth-0.8/django_magicauth.egg-info/PKG-INFO` & `django-magicauth-0.9/django_magicauth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magicauth
-Version: 0.8
+Version: 0.9
 Summary: Password-less authentication: login by clicking on a magic link received by email.
 Home-page: 
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -93,14 +93,18 @@
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.sites.middleware.CurrentSiteMiddleware",
 ]
 ```
 
+7. Configure the projet's domain name using the `Site` model and, if needed, the corresponding `SITE_ID`.
+If you dont configure the domain name, it will default to the URL path.
+
+
 ## Two-Factor Authentication (2FA) using One Time Passwords (OTP)
 
 Two-Factor Authentication means you ask for two different passwords from your user : their normal password and an OTP. (See https://en.wikipedia.org/wiki/Multi-factor_authentication)
 They will get the magic link only if the two are valid, else they get an error and the link is not sent.
 
 What is a OTP ? It is a short code (6 to 8 digits), usually generated by a dedicated app on a user's device (smartphone, hardware). See https://en.wikipedia.org/wiki/Time-based_One-time_Password_algorithm
```

### Comparing `django-magicauth-0.8/django_magicauth.egg-info/SOURCES.txt` & `django-magicauth-0.9/django_magicauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/forms.py` & `django-magicauth-0.9/magicauth/forms.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/migrations/0001_initial.py` & `django-magicauth-0.9/magicauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/models.py` & `django-magicauth-0.9/magicauth/models.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/next_url.py` & `django-magicauth-0.9/magicauth/next_url.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/otp_forms.py` & `django-magicauth-0.9/magicauth/otp_forms.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/send_token.py` & `django-magicauth-0.9/magicauth/send_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 
 from django.contrib.auth import get_user_model
+from django.contrib.sites.models import Site
 from django.contrib.sites.shortcuts import get_current_site
 from django.core.mail import send_mail
 from django.template import loader
 
 from magicauth import settings as magicauth_settings
 from magicauth.models import MagicToken
 
@@ -33,19 +34,25 @@
         return user
 
     def send_email(self, user, user_email, token, extra_context=None):
         email_subject = magicauth_settings.EMAIL_SUBJECT
         html_template = magicauth_settings.EMAIL_HTML_TEMPLATE
         text_template = magicauth_settings.EMAIL_TEXT_TEMPLATE
         from_email = magicauth_settings.FROM_EMAIL
+        try:
+            site_domain = get_current_site(self.request).domain
+        except Site.DoesNotExist:
+            site_domain = self.request.get_host()
         context = {
             "token": token,
             "user": user,
-            "site": get_current_site(self.request),
-            "TOKEN_DURATION_MINUTES": math.floor(magicauth_settings.TOKEN_DURATION_SECONDS / 60),
+            "site_domain": site_domain,
+            "TOKEN_DURATION_MINUTES": math.floor(
+                magicauth_settings.TOKEN_DURATION_SECONDS / 60
+            ),
             "TOKEN_DURATION_SECONDS": magicauth_settings.TOKEN_DURATION_SECONDS,
         }
         if extra_context:
             context.update(extra_context)
         text_message = loader.render_to_string(text_template, context)
         html_message = loader.render_to_string(html_template, context)
         send_mail(
```

### Comparing `django-magicauth-0.8/magicauth/settings.py` & `django-magicauth-0.9/magicauth/settings.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/templates/magicauth/email.html` & `django-magicauth-0.9/magicauth/templates/magicauth/email.html`

 * *Files 2% similar despite different names*

```diff
@@ -297,23 +297,23 @@
               <!-- START MAIN CONTENT AREA -->
               <tr>
                 <td class="wrapper">
                   <table border="0" cellpadding="6" cellspacing="0">
                     <tr>
                       <td>
                         <p>Bonjour {{ user.first_name }} {{ user.last_name }},</p>
-                        <p>Pour accéder à {{ site.domain }}, vous avez juste à cliquer sur ce bouton :</p>
+                        <p>Pour accéder à {{ site_domain }}, vous avez juste à cliquer sur ce bouton :</p>
                         <table border="0" cellpadding="0" cellspacing="0" class="btn btn-primary">
                           <tbody>
                             <tr>
                               <td align="center">
                                 <table border="0" cellpadding="0" cellspacing="0">
                                   <tbody>
                                     <tr>
-                                      <td align="center"> <a href="https://{{ site.domain }}{% url 'magicauth-wait' token.key %}?next={{ next_url|urlencode }}">Connexion</a> </td>
+                                      <td align="center"> <a href="https://{{ site_domain }}{% url 'magicauth-wait' token.key %}?next={{ next_url|urlencode }}">Connexion</a> </td>
                                     </tr>
                                   </tbody>
                                 </table>
                               </td>
                             </tr>
                           </tbody>
                         </table>
@@ -322,19 +322,19 @@
                         <div>
                           <p>Des difficultés pour vous connecter ?</p>
                           <p>
                             Nous vous recommandons de copier-coller ce lien dans un navigateur :
                           </p>
                           <p class="mb-6 align-center">
                             <strong>
-                              https://{{ site.domain }}{% url 'magicauth-wait' token.key %}?next={{ next_url|urlencode }}
+                              https://{{ site_domain }}{% url 'magicauth-wait' token.key %}?next={{ next_url|urlencode }}
                             </strong>
                           </p>
                           <p>Bonne journée,</p>
-                          <p>L'équipe de {{ site.domain }}</p>
+                          <p>L'équipe de {{ site_domain }}</p>
                         </div>
                       </td>
                     </tr>
                   </table>
                 </td>
               </tr>
             <!-- END MAIN CONTENT AREA -->
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 
   Bonjour {{ user.first_name }} {{ user.last_name }},
-  Pour accéder à {{ site.domain }}, vous avez juste à cliquer sur ce bouton :
+  Pour accéder à {{ site_domain }}, vous avez juste à cliquer sur ce bouton :
   Connexion
   Ce lien n'est valable que {{ TOKEN_DURATION_MINUTES }} minutes. Il est à usage
   unique.
  ===============================================================================
   Des difficultés pour vous connecter ?
   Nous vous recommandons de copier-coller ce lien dans un navigateur :
-  https://{{ site.domain }}{% url 'magicauth-wait' token.key %}?next={
+  https://{{ site_domain }}{% url 'magicauth-wait' token.key %}?next={
   { next_url|urlencode }}
   Bonne journée,
-  L'équipe de {{ site.domain }}
+  L'équipe de {{ site_domain }}
```

### Comparing `django-magicauth-0.8/magicauth/templates/magicauth/email_sent.html` & `django-magicauth-0.9/magicauth/templates/magicauth/email_sent.html`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/templates/magicauth/login.html` & `django-magicauth-0.9/magicauth/templates/magicauth/login.html`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/templates/magicauth/wait.html` & `django-magicauth-0.9/magicauth/templates/magicauth/wait.html`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/urls.py` & `django-magicauth-0.9/magicauth/urls.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/magicauth/views.py` & `django-magicauth-0.9/magicauth/views.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/setup.py` & `django-magicauth-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="django-magicauth",
-    version="0.8",
+    version="0.9",
     packages=find_packages(),
     include_package_data=True,
     license="",
     description=(
         "Password-less authentication: login by clicking on "
         "a magic link received by email."),
     long_description=README,
```

### Comparing `django-magicauth-0.8/tests/factories.py` & `django-magicauth-0.9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/tests/test_1_GET_login_view.py` & `django-magicauth-0.9/tests/test_1_GET_login_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/tests/test_2_POST_login_view.py` & `django-magicauth-0.9/tests/test_2_POST_login_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/tests/test_3_email_sent_view.py` & `django-magicauth-0.9/tests/test_3_email_sent_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/tests/test_4_wait_view.py` & `django-magicauth-0.9/tests/test_4_wait_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/tests/test_5_validate_token_view.py` & `django-magicauth-0.9/tests/test_5_validate_token_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-0.8/tests/test_settings.py` & `django-magicauth-0.9/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 INSTALLED_APPS = [
     "tests",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "magicauth",
     "django_otp",
     "django_otp.plugins.otp_static",
+    "django.contrib.sites",
 ]
 
 SESSION_ENGINE = "django.contrib.sessions.backends.cache"
 
 MAGICAUTH_FROM_EMAIL = "user@domain.user"
 MAGICAUTH_LOGGED_IN_REDIRECT_URL_NAME = "test_home"
 
@@ -26,7 +27,9 @@
 MIDDLEWARE = [
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.sites.middleware.CurrentSiteMiddleware",
     "django_otp.middleware.OTPMiddleware",
 ]
+
+SITE_ID = 1
```

