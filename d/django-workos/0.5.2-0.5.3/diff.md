# Comparing `tmp/django-workos-0.5.2.tar.gz` & `tmp/django-workos-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-workos-0.5.2.tar", last modified: Thu May 25 01:13:45 2023, max compression
+gzip compressed data, was "django-workos-0.5.3.tar", last modified: Sun Jun  4 23:26:27 2023, max compression
```

## Comparing `django-workos-0.5.2.tar` & `django-workos-0.5.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-25 01:13:45.767707 django-workos-0.5.2/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1484 2022-08-09 22:13:18.000000 django-workos-0.5.2/LICENSE
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      121 2022-08-15 04:11:13.000000 django-workos-0.5.2/MANIFEST.in
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20115 2023-05-25 01:13:45.767707 django-workos-0.5.2/PKG-INFO
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    19671 2023-02-27 00:53:08.000000 django-workos-0.5.2/README.md
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-25 01:13:45.747707 django-workos-0.5.2/django_workos.egg-info/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20115 2023-05-25 01:13:45.000000 django-workos-0.5.2/django_workos.egg-info/PKG-INFO
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2996 2023-05-25 01:13:45.000000 django-workos-0.5.2/django_workos.egg-info/SOURCES.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        1 2023-05-25 01:13:45.000000 django-workos-0.5.2/django_workos.egg-info/dependency_links.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-05-25 01:13:45.000000 django-workos-0.5.2/django_workos.egg-info/requires.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-05-25 01:13:45.000000 django-workos-0.5.2/django_workos.egg-info/top_level.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      585 2023-05-25 01:13:17.000000 django-workos-0.5.2/pyproject.toml
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       73 2023-05-25 01:13:45.767707 django-workos-0.5.2/setup.cfg
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-25 01:13:45.757707 django-workos-0.5.2/workos_login/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.2/workos_login/__init__.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1799 2023-02-27 00:17:50.000000 django-workos-0.5.2/workos_login/admin.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1505 2022-08-13 16:56:52.000000 django-workos-0.5.2/workos_login/admin_site.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1045 2022-10-05 00:27:58.000000 django-workos-0.5.2/workos_login/apps.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2650 2023-05-22 03:56:47.000000 django-workos-0.5.2/workos_login/conf.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       99 2022-10-09 19:59:00.000000 django-workos-0.5.2/workos_login/exceptions.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     5731 2023-02-27 00:17:50.000000 django-workos-0.5.2/workos_login/forms.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-25 01:13:45.757707 django-workos-0.5.2/workos_login/migrations/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     3267 2022-08-15 00:43:37.000000 django-workos-0.5.2/workos_login/migrations/0001_initial.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      629 2022-08-13 00:41:11.000000 django-workos-0.5.2/workos_login/migrations/0002_auto_20220803_2242.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      563 2022-09-20 04:37:45.000000 django-workos-0.5.2/workos_login/migrations/0003_loginrule_jit_username_format.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      908 2022-10-04 22:32:58.000000 django-workos-0.5.2/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      655 2022-10-05 06:11:28.000000 django-workos-0.5.2/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      542 2023-02-27 00:19:33.000000 django-workos-0.5.2/workos_login/migrations/0006_loginrule_jit_creation_type.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      475 2023-02-27 00:25:07.000000 django-workos-0.5.2/workos_login/migrations/0007_auto_20230227_0020.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:25:13.000000 django-workos-0.5.2/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.2/workos_login/migrations/__init__.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-25 01:13:45.757707 django-workos-0.5.2/workos_login/migrations/__pycache__/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2654 2022-08-15 00:43:43.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      817 2022-08-13 00:41:12.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      788 2022-09-20 04:37:55.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1012 2022-08-06 22:56:24.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1192 2022-08-10 00:17:47.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1049 2022-10-04 22:32:58.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      720 2022-08-12 22:31:04.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      874 2022-10-05 06:14:09.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:20:58.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      784 2023-02-27 00:25:13.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      950 2023-02-27 00:26:25.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      166 2022-07-28 06:31:59.000000 django-workos-0.5.2/workos_login/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11451 2023-05-24 02:03:02.000000 django-workos-0.5.2/workos_login/models.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      200 2022-10-17 23:45:50.000000 django-workos-0.5.2/workos_login/signals.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-25 01:13:45.747707 django-workos-0.5.2/workos_login/templates/
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-25 01:13:45.767707 django-workos-0.5.2/workos_login/templates/registration/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4439 2023-05-22 03:56:47.000000 django-workos-0.5.2/workos_login/templates/registration/base_login.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1720 2022-09-19 21:22:58.000000 django-workos-0.5.2/workos_login/templates/registration/base_registration.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      307 2022-08-13 17:15:38.000000 django-workos-0.5.2/workos_login/templates/registration/bootstrap.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      498 2022-08-10 00:23:34.000000 django-workos-0.5.2/workos_login/templates/registration/form.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       47 2022-10-21 22:11:19.000000 django-workos-0.5.2/workos_login/templates/registration/login.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       46 2022-08-13 18:16:16.000000 django-workos-0.5.2/workos_login/templates/registration/logo.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      276 2023-05-22 04:27:37.000000 django-workos-0.5.2/workos_login/templates/registration/magic_link_complete.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      394 2022-08-09 05:19:03.000000 django-workos-0.5.2/workos_login/templates/registration/messages.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1397 2022-10-21 22:15:37.000000 django-workos-0.5.2/workos_login/templates/registration/mfa_enroll.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2122 2022-08-09 04:14:47.000000 django-workos-0.5.2/workos_login/templates/registration/mfa_enroll_start.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      678 2022-10-21 22:17:30.000000 django-workos-0.5.2/workos_login/templates/registration/mfa_verify.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      316 2022-09-15 22:29:19.000000 django-workos-0.5.2/workos_login/templates/registration/password_reset_complete.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      666 2022-09-15 22:32:39.000000 django-workos-0.5.2/workos_login/templates/registration/password_reset_confirm.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      493 2022-09-15 22:32:39.000000 django-workos-0.5.2/workos_login/templates/registration/password_reset_done.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      501 2022-09-15 22:24:22.000000 django-workos-0.5.2/workos_login/templates/registration/password_reset_form.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1589 2022-10-21 21:39:41.000000 django-workos-0.5.2/workos_login/templates/registration/style.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4718 2022-10-17 23:00:04.000000 django-workos-0.5.2/workos_login/tests.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2073 2023-02-23 05:45:24.000000 django-workos-0.5.2/workos_login/urls.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    10399 2023-02-23 07:23:03.000000 django-workos-0.5.2/workos_login/utils.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    22224 2023-05-25 01:12:59.000000 django-workos-0.5.2/workos_login/views.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.689859 django-workos-0.5.3/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1484 2022-08-09 22:13:18.000000 django-workos-0.5.3/LICENSE
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      121 2022-08-15 04:11:13.000000 django-workos-0.5.3/MANIFEST.in
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20395 2023-06-04 23:26:27.689859 django-workos-0.5.3/PKG-INFO
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    19951 2023-06-04 23:24:05.000000 django-workos-0.5.3/README.md
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.669859 django-workos-0.5.3/django_workos.egg-info/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20395 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/PKG-INFO
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2996 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/SOURCES.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        1 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/dependency_links.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/requires.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/top_level.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      585 2023-06-04 23:25:12.000000 django-workos-0.5.3/pyproject.toml
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       73 2023-06-04 23:26:27.689859 django-workos-0.5.3/setup.cfg
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.679859 django-workos-0.5.3/workos_login/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.3/workos_login/__init__.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1799 2023-02-27 00:17:50.000000 django-workos-0.5.3/workos_login/admin.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1505 2022-08-13 16:56:52.000000 django-workos-0.5.3/workos_login/admin_site.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1045 2022-10-05 00:27:58.000000 django-workos-0.5.3/workos_login/apps.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2650 2023-05-22 03:56:47.000000 django-workos-0.5.3/workos_login/conf.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      154 2023-06-04 22:15:55.000000 django-workos-0.5.3/workos_login/exceptions.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     5731 2023-02-27 00:17:50.000000 django-workos-0.5.3/workos_login/forms.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.679859 django-workos-0.5.3/workos_login/migrations/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     3267 2022-08-15 00:43:37.000000 django-workos-0.5.3/workos_login/migrations/0001_initial.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      629 2022-08-13 00:41:11.000000 django-workos-0.5.3/workos_login/migrations/0002_auto_20220803_2242.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      563 2022-09-20 04:37:45.000000 django-workos-0.5.3/workos_login/migrations/0003_loginrule_jit_username_format.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      908 2022-10-04 22:32:58.000000 django-workos-0.5.3/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      655 2022-10-05 06:11:28.000000 django-workos-0.5.3/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      542 2023-02-27 00:19:33.000000 django-workos-0.5.3/workos_login/migrations/0006_loginrule_jit_creation_type.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      475 2023-02-27 00:25:07.000000 django-workos-0.5.3/workos_login/migrations/0007_auto_20230227_0020.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:25:13.000000 django-workos-0.5.3/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.3/workos_login/migrations/__init__.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.689859 django-workos-0.5.3/workos_login/migrations/__pycache__/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2654 2022-08-15 00:43:43.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      817 2022-08-13 00:41:12.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      788 2022-09-20 04:37:55.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1012 2022-08-06 22:56:24.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1192 2022-08-10 00:17:47.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1049 2022-10-04 22:32:58.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      720 2022-08-12 22:31:04.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      874 2022-10-05 06:14:09.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:20:58.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      784 2023-02-27 00:25:13.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      950 2023-02-27 00:26:25.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      166 2022-07-28 06:31:59.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11451 2023-05-24 02:03:02.000000 django-workos-0.5.3/workos_login/models.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      200 2022-10-17 23:45:50.000000 django-workos-0.5.3/workos_login/signals.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.669859 django-workos-0.5.3/workos_login/templates/
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.689859 django-workos-0.5.3/workos_login/templates/registration/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4723 2023-06-04 23:24:05.000000 django-workos-0.5.3/workos_login/templates/registration/base_login.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1720 2022-09-19 21:22:58.000000 django-workos-0.5.3/workos_login/templates/registration/base_registration.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      307 2022-08-13 17:15:38.000000 django-workos-0.5.3/workos_login/templates/registration/bootstrap.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      498 2022-08-10 00:23:34.000000 django-workos-0.5.3/workos_login/templates/registration/form.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       47 2022-10-21 22:11:19.000000 django-workos-0.5.3/workos_login/templates/registration/login.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       46 2022-08-13 18:16:16.000000 django-workos-0.5.3/workos_login/templates/registration/logo.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      276 2023-05-22 04:27:37.000000 django-workos-0.5.3/workos_login/templates/registration/magic_link_complete.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      394 2022-08-09 05:19:03.000000 django-workos-0.5.3/workos_login/templates/registration/messages.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1397 2022-10-21 22:15:37.000000 django-workos-0.5.3/workos_login/templates/registration/mfa_enroll.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2122 2022-08-09 04:14:47.000000 django-workos-0.5.3/workos_login/templates/registration/mfa_enroll_start.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      678 2022-10-21 22:17:30.000000 django-workos-0.5.3/workos_login/templates/registration/mfa_verify.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      316 2022-09-15 22:29:19.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_complete.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      666 2022-09-15 22:32:39.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      493 2022-09-15 22:32:39.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_done.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      501 2022-09-15 22:24:22.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_form.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1589 2022-10-21 21:39:41.000000 django-workos-0.5.3/workos_login/templates/registration/style.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4718 2022-10-17 23:00:04.000000 django-workos-0.5.3/workos_login/tests.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2073 2023-02-23 05:45:24.000000 django-workos-0.5.3/workos_login/urls.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11432 2023-06-04 22:31:47.000000 django-workos-0.5.3/workos_login/utils.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    22224 2023-05-25 01:12:59.000000 django-workos-0.5.3/workos_login/views.py
```

### Comparing `django-workos-0.5.2/LICENSE` & `django-workos-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/PKG-INFO` & `django-workos-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-workos
-Version: 0.5.2
+Version: 0.5.3
 Summary: Enabling SSO, MFA and passwordless login for Django projects by using WorkOS.
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/surefyresystems/django-workos
 Keywords: django,sso,workos,mfa
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -121,14 +121,18 @@
 
 ### Using the login page
 When logging in directly to your Django app you will be presented with a login screen that looks like this:
 
 For all forms of login, if a `next` query parameter is provided the user will be redirected to that URL after authenticating.
 If `next` is not provided `LOGIN_REDIRECT_URL` setting will be used to determine where to redirect the user.
 
+If `username` query parameter is provided the username input will be prefilled.
+If `start` query parameter with value of `true` is provided in addition to username it will move the login to the second step. 
+This allows for an automatic redirect to an SSO login page if desired.
+
 Once a username is entered django-workos will determine which rule applies for this username.
 The next step depends on the rule that applies:
 #### Username / Password
 If the login rule dictates username and password a password input will be presented.
 There will also be a forgot your password link presented to allow users to reset password via email.
 
 #### Magic Email
```

### Comparing `django-workos-0.5.2/README.md` & `django-workos-0.5.3/django_workos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: django-workos
+Version: 0.5.3
+Summary: Enabling SSO, MFA and passwordless login for Django projects by using WorkOS.
+License: BSD 3-Clause License
+Project-URL: Homepage, https://github.com/surefyresystems/django-workos
+Keywords: django,sso,workos,mfa
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Django WorkOS
 
 Django WorkOS builds on top of Django contrib auth to support a variety of login methods.
 Django WorKOS adds support for the following login methods:
 
 1. Username/Password authentication provided by `django.contrib.auth`
 2. SSO authentication provided by [WorkOS](https://workos.com)
@@ -108,14 +121,18 @@
 
 ### Using the login page
 When logging in directly to your Django app you will be presented with a login screen that looks like this:
 
 For all forms of login, if a `next` query parameter is provided the user will be redirected to that URL after authenticating.
 If `next` is not provided `LOGIN_REDIRECT_URL` setting will be used to determine where to redirect the user.
 
+If `username` query parameter is provided the username input will be prefilled.
+If `start` query parameter with value of `true` is provided in addition to username it will move the login to the second step. 
+This allows for an automatic redirect to an SSO login page if desired.
+
 Once a username is entered django-workos will determine which rule applies for this username.
 The next step depends on the rule that applies:
 #### Username / Password
 If the login rule dictates username and password a password input will be presented.
 There will also be a forgot your password link presented to allow users to reset password via email.
 
 #### Magic Email
```

### Comparing `django-workos-0.5.2/django_workos.egg-info/PKG-INFO` & `django-workos-0.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: django-workos
-Version: 0.5.2
-Summary: Enabling SSO, MFA and passwordless login for Django projects by using WorkOS.
-License: BSD 3-Clause License
-Project-URL: Homepage, https://github.com/surefyresystems/django-workos
-Keywords: django,sso,workos,mfa
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django WorkOS
 
 Django WorkOS builds on top of Django contrib auth to support a variety of login methods.
 Django WorKOS adds support for the following login methods:
 
 1. Username/Password authentication provided by `django.contrib.auth`
 2. SSO authentication provided by [WorkOS](https://workos.com)
@@ -121,14 +108,18 @@
 
 ### Using the login page
 When logging in directly to your Django app you will be presented with a login screen that looks like this:
 
 For all forms of login, if a `next` query parameter is provided the user will be redirected to that URL after authenticating.
 If `next` is not provided `LOGIN_REDIRECT_URL` setting will be used to determine where to redirect the user.
 
+If `username` query parameter is provided the username input will be prefilled.
+If `start` query parameter with value of `true` is provided in addition to username it will move the login to the second step. 
+This allows for an automatic redirect to an SSO login page if desired.
+
 Once a username is entered django-workos will determine which rule applies for this username.
 The next step depends on the rule that applies:
 #### Username / Password
 If the login rule dictates username and password a password input will be presented.
 There will also be a forgot your password link presented to allow users to reset password via email.
 
 #### Magic Email
```

### Comparing `django-workos-0.5.2/django_workos.egg-info/SOURCES.txt` & `django-workos-0.5.3/django_workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/pyproject.toml` & `django-workos-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-workos"
-version = "0.5.2"
+version = "0.5.3"
 description = "Enabling SSO, MFA and passwordless login for Django projects by using WorkOS."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["django", "sso", "workos", "mfa"]
 license = {text = "BSD 3-Clause License"}
 classifiers = [
     "Framework :: Django",
```

### Comparing `django-workos-0.5.2/workos_login/admin.py` & `django-workos-0.5.3/workos_login/admin.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/admin_site.py` & `django-workos-0.5.3/workos_login/admin_site.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/apps.py` & `django-workos-0.5.3/workos_login/apps.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/conf.py` & `django-workos-0.5.3/workos_login/conf.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/forms.py` & `django-workos-0.5.3/workos_login/forms.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/0001_initial.py` & `django-workos-0.5.3/workos_login/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/0002_auto_20220803_2242.py` & `django-workos-0.5.3/workos_login/migrations/0002_auto_20220803_2242.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/0003_loginrule_jit_username_format.py` & `django-workos-0.5.3/workos_login/migrations/0003_loginrule_jit_username_format.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py` & `django-workos-0.5.3/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py` & `django-workos-0.5.3/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/0006_loginrule_jit_creation_type.py` & `django-workos-0.5.3/workos_login/migrations/0006_loginrule_jit_creation_type.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py` & `django-workos-0.5.3/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc` & `django-workos-0.5.3/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/models.py` & `django-workos-0.5.3/workos_login/models.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/templates/registration/base_login.html` & `django-workos-0.5.3/workos_login/templates/registration/base_login.html`

 * *Files 6% similar despite different names*

```diff
@@ -162,9 +162,22 @@
     }
 
     document.getElementById('btn-next').addEventListener("click", next);
     document.getElementById('btn-back').addEventListener("click", back);
     hideInput('id_password');
     submitOnEnter("id_password");
     submitOnEnter("id_username");
+
+    const urlParams = new URLSearchParams(window.location.search);
+    const username = urlParams.get('username');
+    const start = urlParams.get('start') === 'true';
+
+    if(username){
+      setValue('id_username', username);
+    }
+
+    if(username && start){
+      next();
+    }
+
   </script>
 {% endblock %}
```

### Comparing `django-workos-0.5.2/workos_login/templates/registration/base_registration.html` & `django-workos-0.5.3/workos_login/templates/registration/base_registration.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/templates/registration/mfa_enroll.html` & `django-workos-0.5.3/workos_login/templates/registration/mfa_enroll.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/templates/registration/mfa_enroll_start.html` & `django-workos-0.5.3/workos_login/templates/registration/mfa_enroll_start.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/templates/registration/mfa_verify.html` & `django-workos-0.5.3/workos_login/templates/registration/mfa_verify.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/templates/registration/password_reset_confirm.html` & `django-workos-0.5.3/workos_login/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/templates/registration/style.html` & `django-workos-0.5.3/workos_login/templates/registration/style.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/tests.py` & `django-workos-0.5.3/workos_login/tests.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/urls.py` & `django-workos-0.5.3/workos_login/urls.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.2/workos_login/utils.py` & `django-workos-0.5.3/workos_login/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.template import Template, Context
 from workos.exceptions import BadRequestException
 
 from workos_login.conf import conf
 from django.db import models, transaction
 import workos
 
-from workos_login.exceptions import RelationDoesNotExist
+from workos_login.exceptions import RelationDoesNotExist, ImproperConfigurationError
 
 
 def get_users():
     return get_user_model().objects.filter(**conf.WORKOS_ACTIVE_USER_FILTER)
 
 
 def find_user_by_email(email: str) -> Optional[models.Model]:
@@ -112,28 +112,29 @@
     """
     user_login = get_user_login_model(user)
     user_login.mfa_type = mfa_type
     user_login.mfa_factor = factor_id
     user_login.save()
 
 
-def render_attribute(value: Any, profile: dict) -> Any:
+def render_attribute(value: Any, profile: dict, object: models.Model) -> Any:
     """
     Helper to render an attribute that will convert strings to templates that are provided with `profile`.
     If value is a dictionary it will nest down and render the leaf values.
     :param value: the attribute value to render
+    :param object: the current object
     :param profile: the profile dict passed from WorkOS
     :return: Rendered value to save
     """
     if isinstance(value, dict):
         for k, v in value.items():
-            value[k] = render_attribute(v, profile)
+            value[k] = render_attribute(v, profile, object)
     if isinstance(value, str):
         t = Template(value)
-        c = Context({"profile": profile})
+        c = Context({"profile": profile, "object": object})
         return t.render(c)
     return value
 
 
 def _link_attributes(obj: models.Model, attributes: Optional[dict], profile: dict) -> None:
     """
     Given a user object link any attributes that are needed.
@@ -149,15 +150,15 @@
         if field_name.startswith(("!", "~")) is False:
             continue
         required = field_name.startswith("!")
         field_name = field_name[1:]
         # This should not error out since "!/~" can only be used for fields that exist and have related lookups.
         field = obj._meta.get_field(field_name)
         try:
-            related_instance = field.related_model.objects.get(**render_attribute(value, profile))
+            related_instance = field.related_model.objects.get(**render_attribute(value, profile, obj))
         except ObjectDoesNotExist:
             related_instance = None
 
         if required and related_instance is None:
             raise RelationDoesNotExist()
 
         setattr(obj, field_name, related_instance)
@@ -178,38 +179,54 @@
         if field_name.startswith(("!", "~")):
             continue
         try:
             field = obj._meta.get_field(field_name)
         except FieldDoesNotExist:
             # Even though this isn't a proper field it might be some custom attribute or settable property.
             # Still set the attribute if it exists on the object.
-            if hasattr(obj, field_name) and (template_only is False or value != render_attribute(value, profile)):
-                setattr(obj, field_name, render_attribute(value, profile))
+            if hasattr(obj, field_name) and (template_only is False or value != render_attribute(value, profile, obj)):
+                setattr(obj, field_name, render_attribute(value, profile, obj))
             continue
 
         if field.is_relation is False:
             # If template only, do not update if the value equals the rendered value which implies it is not a template field.
-            if template_only is False or value != render_attribute(value, profile):
-                setattr(obj, field_name, render_attribute(value, profile))
+            if template_only is False or value != render_attribute(value, profile, obj):
+                setattr(obj, field_name, render_attribute(value, profile, obj))
 
         elif field.many_to_one or field.one_to_one:
             if value is None:
                 if template_only is False:
                     setattr(obj, field_name, None)
             else:
                 # Might need to create object
                 related_obj = getattr(obj, field_name)
                 if related_obj is None:
                     # Need to create object with the top level attributes
-                    related_obj_attrs = {k: v for k,v in value.items() if not isinstance(v, dict)}
+                    related_obj_attrs = {k: render_attribute(v, profile, obj) for k,v in value.items() if not (isinstance(v, dict) or isinstance(v, list))}
                     related_obj = field.related_model.objects.create(**related_obj_attrs)
                     setattr(obj, field_name, related_obj)
 
                 _update_attributes(getattr(obj, field_name), value, profile)
 
+        elif field.many_to_many or field.one_to_many:
+            if not isinstance(value, list):
+                raise ImproperConfigurationError("Many to many or reverse relations must be of type array")
+            for item in value:
+                related_obj_attrs = {k: render_attribute(v, profile, obj) for k, v in item.items() if not (isinstance(v, dict) or isinstance(v, list))}
+
+                related_manager = getattr(obj, field_name)
+                try:
+                    related_obj, created = related_manager.get_or_create(**related_obj_attrs)
+                    _update_attributes(related_obj, item, profile)
+                except MultipleObjectsReturned:
+                    for related_obj in related_manager.filter(**related_obj_attrs):
+                        _update_attributes(related_obj, item, profile)
+
+
+
     obj.save()
 
 
 def jit_create_user(rule: models.Model, profile: dict) -> models.Model:
     """
     Given a profile from workos and a rule create a user
     """
```

### Comparing `django-workos-0.5.2/workos_login/views.py` & `django-workos-0.5.3/workos_login/views.py`

 * *Files identical despite different names*

