# Comparing `tmp/django_idp_user-2.0.4.tar.gz` & `tmp/django_idp_user-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_idp_user-2.0.4.tar", last modified: Tue Jan 10 10:39:20 2023, max compression
+gzip compressed data, was "django_idp_user-2.1.0.tar", last modified: Mon Jun  5 14:51:04 2023, max compression
```

## Comparing `django_idp_user-2.0.4.tar` & `django_idp_user-2.1.0.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.537174 django_idp_user-2.0.4/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       73 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3624 2023-01-10 10:39:20.537174 django_idp_user-2.0.4/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2507 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/README.rst
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.529174 django_idp_user-2.0.4/django_idp_user.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3624 2023-01-10 10:39:20.000000 django_idp_user-2.0.4/django_idp_user.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1219 2023-01-10 10:39:20.000000 django_idp_user-2.0.4/django_idp_user.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-01-10 10:39:20.000000 django_idp_user-2.0.4/django_idp_user.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       55 2023-01-10 10:39:20.000000 django_idp_user-2.0.4/django_idp_user.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        9 2023-01-10 10:39:20.000000 django_idp_user-2.0.4/django_idp_user.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.533174 django_idp_user-2.0.4/idp_user/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       95 2022-05-27 08:20:34.000000 django_idp_user-2.0.4/idp_user/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1972 2023-01-04 10:16:32.000000 django_idp_user-2.0.4/idp_user/agents.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1024 2022-06-02 16:12:38.000000 django_idp_user-2.0.4/idp_user/apps.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.533174 django_idp_user-2.0.4/idp_user/auth/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       66 2022-06-02 14:58:31.000000 django_idp_user-2.0.4/idp_user/auth/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3921 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/idp_user/auth/authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2345 2022-06-02 14:58:31.000000 django_idp_user-2.0.4/idp_user/checks.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.533174 django_idp_user-2.0.4/idp_user/management/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-05-27 08:20:34.000000 django_idp_user-2.0.4/idp_user/management/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.533174 django_idp_user-2.0.4/idp_user/management/commands/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2022-05-27 08:20:34.000000 django_idp_user-2.0.4/idp_user/management/commands/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      823 2022-05-27 08:20:34.000000 django_idp_user-2.0.4/idp_user/management/commands/put_app_entities_records_to_kafka.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.533174 django_idp_user-2.0.4/idp_user/migrations/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4340 2022-08-12 09:17:30.000000 django_idp_user-2.0.4/idp_user/migrations/0001_initial.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      378 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/idp_user/migrations/0002_auto_20220120_1617.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      390 2022-05-27 08:20:34.000000 django_idp_user-2.0.4/idp_user/migrations/0003_auto_20220513_1025.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      579 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/idp_user/migrations/0004_auto_20220817_1526.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      446 2022-08-18 10:03:14.000000 django_idp_user-2.0.4/idp_user/migrations/0005_alter_userrole_id.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      648 2022-08-30 09:11:12.000000 django_idp_user-2.0.4/idp_user/migrations/0006_auto_20220830_0911.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/idp_user/migrations/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.537174 django_idp_user-2.0.4/idp_user/models/
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       55 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/idp_user/models/__init__.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       89 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/idp_user/models/user.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)      713 2022-11-04 17:01:58.000000 django_idp_user-2.0.4/idp_user/models/user_role.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      959 2022-05-27 08:20:34.000000 django_idp_user-2.0.4/idp_user/producer.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      800 2022-08-18 10:04:17.000000 django_idp_user-2.0.4/idp_user/schema_extensions.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.537174 django_idp_user-2.0.4/idp_user/services/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       30 2022-06-02 14:58:31.000000 django_idp_user-2.0.4/idp_user/services/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17047 2023-01-10 10:39:15.000000 django_idp_user-2.0.4/idp_user/services/user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      771 2023-01-10 10:39:15.000000 django_idp_user-2.0.4/idp_user/settings.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      132 2022-05-16 23:05:38.000000 django_idp_user-2.0.4/idp_user/signals.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2868 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/idp_user/typing.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       16 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/idp_user/urls.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-01-10 10:39:20.537174 django_idp_user-2.0.4/idp_user/utils/
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/idp_user/utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      600 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/idp_user/utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2022-05-27 08:20:34.000000 django_idp_user-2.0.4/idp_user/utils/classes.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      435 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/idp_user/utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2557 2022-08-17 17:42:38.000000 django_idp_user-2.0.4/idp_user/utils/functions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1141 2023-01-10 10:39:20.537174 django_idp_user-2.0.4/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2022-04-20 16:03:29.000000 django_idp_user-2.0.4/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       73 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3604 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2507 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/README.rst
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/django_idp_user.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3604 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1172 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       55 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        9 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       95 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1972 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/agents.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1024 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/apps.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/auth/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       66 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/auth/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3921 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/auth/authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2345 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/checks.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/management/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/management/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/management/commands/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/management/commands/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      823 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/management/commands/put_app_entities_records_to_kafka.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/migrations/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4340 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0001_initial.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      378 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0002_auto_20220120_1617.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      390 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0003_auto_20220513_1025.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      579 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0004_auto_20220817_1526.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      446 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0005_alter_userrole_id.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/models/
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       55 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/models/__init__.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       89 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/models/user.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)      713 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/models/user_role.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      959 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/producer.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      800 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/schema_extensions.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/services/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       30 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/services/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17047 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/services/user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      771 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/settings.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      132 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/signals.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2868 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/typing.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       16 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/urls.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/utils/
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      600 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/classes.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      435 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2312 2023-06-05 14:49:38.000000 django_idp_user-2.1.0/idp_user/utils/functions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1141 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/setup.py
```

### Comparing `django_idp_user-2.0.4/LICENSE` & `django_idp_user-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/PKG-INFO` & `django_idp_user-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django_idp_user
-Version: 2.0.4
+Version: 2.1.0
 Summary: A Django app that handles the communication between the IDP and the products for the authorization of users.
 Home-page: https://github.com/CardoAI/django-idp-user
 Author: Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri
 Author-email: hello@cardoai.com
 License: MIT (X11)
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -112,9 +111,7 @@
     so that they can be used for authorization purposes. In the value dicts, the attributes that will be
     used as the identifier and label are declared as well.
 
 * ``CONSUMER_APP_ENV``
 
   * The environment of the Faust Kafka Consumer app.
   * If not set, the value of ``APP_ENV`` will be used.
-
-
```

### Comparing `django_idp_user-2.0.4/README.rst` & `django_idp_user-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/django_idp_user.egg-info/PKG-INFO` & `django_idp_user-2.1.0/django_idp_user.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-idp-user
-Version: 2.0.4
+Version: 2.1.0
 Summary: A Django app that handles the communication between the IDP and the products for the authorization of users.
 Home-page: https://github.com/CardoAI/django-idp-user
 Author: Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri
 Author-email: hello@cardoai.com
 License: MIT (X11)
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -112,9 +111,7 @@
     so that they can be used for authorization purposes. In the value dicts, the attributes that will be
     used as the identifier and label are declared as well.
 
 * ``CONSUMER_APP_ENV``
 
   * The environment of the Faust Kafka Consumer app.
   * If not set, the value of ``APP_ENV`` will be used.
-
-
```

### Comparing `django_idp_user-2.0.4/django_idp_user.egg-info/SOURCES.txt` & `django_idp_user-2.1.0/django_idp_user.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 idp_user/management/commands/__init__.py
 idp_user/management/commands/put_app_entities_records_to_kafka.py
 idp_user/migrations/0001_initial.py
 idp_user/migrations/0002_auto_20220120_1617.py
 idp_user/migrations/0003_auto_20220513_1025.py
 idp_user/migrations/0004_auto_20220817_1526.py
 idp_user/migrations/0005_alter_userrole_id.py
-idp_user/migrations/0006_auto_20220830_0911.py
 idp_user/migrations/__init__.py
 idp_user/models/__init__.py
 idp_user/models/user.py
 idp_user/models/user_role.py
 idp_user/services/__init__.py
 idp_user/services/user.py
 idp_user/utils/__init__.py
```

### Comparing `django_idp_user-2.0.4/idp_user/agents.py` & `django_idp_user-2.1.0/idp_user/agents.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/apps.py` & `django_idp_user-2.1.0/idp_user/apps.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/auth/authentication.py` & `django_idp_user-2.1.0/idp_user/auth/authentication.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/checks.py` & `django_idp_user-2.1.0/idp_user/checks.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/management/commands/put_app_entities_records_to_kafka.py` & `django_idp_user-2.1.0/idp_user/management/commands/put_app_entities_records_to_kafka.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/migrations/0001_initial.py` & `django_idp_user-2.1.0/idp_user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/migrations/0004_auto_20220817_1526.py` & `django_idp_user-2.1.0/idp_user/migrations/0004_auto_20220817_1526.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/models/user_role.py` & `django_idp_user-2.1.0/idp_user/models/user_role.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/producer.py` & `django_idp_user-2.1.0/idp_user/producer.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/schema_extensions.py` & `django_idp_user-2.1.0/idp_user/schema_extensions.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/services/user.py` & `django_idp_user-2.1.0/idp_user/services/user.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/settings.py` & `django_idp_user-2.1.0/idp_user/settings.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/typing.py` & `django_idp_user-2.1.0/idp_user/typing.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/utils/choices.py` & `django_idp_user-2.1.0/idp_user/utils/choices.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.0.4/idp_user/utils/functions.py` & `django_idp_user-2.1.0/idp_user/utils/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -53,21 +53,15 @@
 
 def get_kafka_bootstrap_servers(include_uri_scheme=True):
     """
     If ARN is available, it means we can connect to the production servers.
     We have to find the bootstrap servers and create the connection using them.
     """
     if kafka_arn := settings.KAFKA_ARN:
-        session = boto3.Session(
-            aws_access_key_id=settings.KAFKA_AWS_ACCESS_KEY_ID,
-            aws_secret_access_key=base64.b64decode(
-                settings.KAFKA_AWS_SECRET_ACCESS_KEY
-            ).decode("utf-8"),
-        )
-        resource = session.client("kafka", region_name=AWS_S3_REGION_NAME)
+        resource = boto3.client("kafka", region_name=AWS_S3_REGION_NAME)
         response = resource.get_bootstrap_brokers(
             ClusterArn=base64.b64decode(kafka_arn).decode("utf-8")
         )
         assert (
                 "BootstrapBrokerString" in response.keys()
         ), "Something went wrong while receiving kafka servers!"
```

### Comparing `django_idp_user-2.0.4/setup.cfg` & `django_idp_user-2.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_idp_user
-version = 2.0.4
+version = 2.1.0
 description = A Django app that handles the communication between the IDP and the products for the authorization of users.
 long_description = file: README.rst
 url = https://github.com/CardoAI/django-idp-user
 author = Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri
 author_email = hello@cardoai.com
 license = MIT (X11)
 classifiers =
```

