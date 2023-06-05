# Comparing `tmp/hdn-research-environment-2.0.7.tar.gz` & `tmp/hdn-research-environment-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.0.7.tar", last modified: Mon Jun  5 06:46:33 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.1.0.tar", last modified: Mon Jun  5 16:03:05 2023, max compression
```

## Comparing `hdn-research-environment-2.0.7.tar` & `hdn-research-environment-2.1.0.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.7/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.7/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.7/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.7/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.7/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1600 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.7/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    18751 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.0.7/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.7/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.7/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     7615 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.0.7/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.7/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.7/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      251 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.7/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.7/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    13367 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     3028 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.7/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.7/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.0/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.0/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.0/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.0/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3074 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.0/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3641 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1600 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.0/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.0/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    18751 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.0/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.0/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.0/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.0/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.0/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7616 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.0/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.1.0/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      251 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.0/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.0/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.0/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.0/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1467 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.0/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.0/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.0/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13857 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.0/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 16:03:04.000000 hdn-research-environment-2.1.0/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3100 2023-06-05 16:03:04.000000 hdn-research-environment-2.1.0/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-05 16:03:04.000000 hdn-research-environment-2.1.0/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-05 16:03:04.000000 hdn-research-environment-2.1.0/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-05 16:03:04.000000 hdn-research-environment-2.1.0/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.0/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-05 16:03:05.000000 hdn-research-environment-2.1.0/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.0/setup.py
```

### Comparing `hdn-research-environment-2.0.7/LICENSE` & `hdn-research-environment-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/PKG-INFO` & `hdn-research-environment-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.7
+Version: 2.1.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.7/environment/api/v1/__init__.py` & `hdn-research-environment-2.1.0/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/api/v1/auth.py` & `hdn-research-environment-2.1.0/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/api/v1/decorators.py` & `hdn-research-environment-2.1.0/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/api/v2/__init__.py` & `hdn-research-environment-2.1.0/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/api/v2/decorators.py` & `hdn-research-environment-2.1.0/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/constants.py` & `hdn-research-environment-2.1.0/environment/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,7 +82,14 @@
     Region.US_CENTRAL: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
     Region.NORTHAMERICA_NORTHEAST: ProjectedWorkbenchCost(
         PERSISTENT_DATA_DISK_NAME, 0.05
     ),
     Region.EUROPE_WEST: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
     Region.AUSTRALIA_SOUTHEAST: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
 }
+
+INSTANCE_TYPE_SPECIFICATION = {
+    InstanceType.N1_STANDARD_2: "2 CPU, 7.5GB RAM",
+    InstanceType.N1_STANDARD_4: "4 CPU, 15GB RAM",
+    InstanceType.N1_STANDARD_8: "8 CPU, 30GB RAM",
+    InstanceType.N1_STANDARD_16: "16 CPU, 60GB RAM",
+}
```

### Comparing `hdn-research-environment-2.0.7/environment/decorators.py` & `hdn-research-environment-2.1.0/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/deserializers.py` & `hdn-research-environment-2.1.0/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/entities.py` & `hdn-research-environment-2.1.0/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/exceptions.py` & `hdn-research-environment-2.1.0/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/forms.py` & `hdn-research-environment-2.1.0/environment/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Iterable
 
 from django import forms
 
 from environment.entities import ResearchWorkspace
+from environment.constants import INSTANCE_TYPE_SPECIFICATION
 
 
 class CloudIdentityPasswordForm(forms.Form):
     password = forms.CharField(widget=forms.PasswordInput())
     confirm_password = forms.CharField(widget=forms.PasswordInput())
     recovery_email = forms.EmailField(
         widget=forms.EmailInput(attrs={"class": "form-control"})
@@ -29,28 +30,26 @@
         ("australia-southeast1", "australia-southeast1"),
     ]
     billing_account_id = forms.ChoiceField(label="Billing Account")
     region = forms.ChoiceField(label="Region", choices=AVAILABLE_REGIONS)
 
     def __init__(self, *args, billing_accounts_list: Iterable[str], **kwargs):
         super(CreateWorkspaceForm, self).__init__(*args, **kwargs)
-        billing_account_ids = [
-            billing_account["id"] for billing_account in billing_accounts_list
-        ]
         self.fields["billing_account_id"].choices = [
-            (billing_id, billing_id) for billing_id in billing_account_ids
+            (billing_account["id"], billing_account["name"])
+            for billing_account in billing_accounts_list
         ]
 
 
 class CreateResearchEnvironmentForm(forms.Form):
     AVAILABLE_INSTANCE_TYPES = [
-        ("n1-standard-2", "2 CPU, 7.5GB RAM"),
-        ("n1-standard-4", "4 CPU, 15GB RAM"),
-        ("n1-standard-8", "8 CPU, 30GB RAM"),
-        ("n1-standard-16", "16 CPU, 60GB RAM"),
+        ("n1-standard-2", INSTANCE_TYPE_SPECIFICATION.N1_STANDARD_2),
+        ("n1-standard-4", INSTANCE_TYPE_SPECIFICATION.N1_STANDARD_4),
+        ("n1-standard-8", INSTANCE_TYPE_SPECIFICATION.N1_STANDARD_8),
+        ("n1-standard-16", INSTANCE_TYPE_SPECIFICATION.N1_STANDARD_16),
     ]
     AVAILABLE_ENVIRONMENT_TYPES = [
         ("jupyter", "Jupyter"),
         ("rstudio", "RStudio"),
     ]
     AVAILABLE_GPU_ACCELERATOR_TYPES = [
         ("", "Machine without GPU attached"),
```

### Comparing `hdn-research-environment-2.0.7/environment/mailers.py` & `hdn-research-environment-2.1.0/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/migrations/0001_initial.py` & `hdn-research-environment-2.1.0/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.1.0/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.1.0/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.1.0/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.1.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/models.py` & `hdn-research-environment-2.1.0/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/services.py` & `hdn-research-environment-2.1.0/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/signals.py` & `hdn-research-environment-2.1.0/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.1.0/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.1.0/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.1.0/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.1.0/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tasks.py` & `hdn-research-environment-2.1.0/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.1.0/environment/templates/environment/_available_environments_list.html`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                                             </div>
                                         </div>
                                     </li>
                                 {% endfor %}
                             </ul>
                         {% else %}
                             <div class="text-center">
-                                You don't have any worbenches in this workspace.<br>
+                                You don't have any workbenches in this workspace.<br>
                                 Create one in the "Projects" tab.
                             </div>
                         {% endif %}
                     </div>
                 </div>
             </div>
         {% endwith %}
```

#### html2text {}

```diff
@@ -34,12 +34,12 @@
       project=project button_type="modal_start" %} {% endif %} {%
       environment_modal_button environment=environment project=project
       button_type="modal_instance" %} {% environment_modal_button
       environment=environment project=project button_type="modal_destroy" %} {%
       endif %}
     * {% endfor %}
 {% else %}
-You don't have any worbenches in this workspace.
+You don't have any workbenches in this workspace.
 Create one in the "Projects" tab.
 {% endif %}
 {% endwith %} {% endfor %}
```

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.1.0/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.1.0/environment/templates/environment/_billing_accounts_list.html`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,16 @@
                         </a>
                     </div>
                     <div class="col-md-4">
                     {% if billing_account.is_owner %}
                         <a href="{% url 'manage_billing_account' billing_account_id=billing_account.id %}" class="btn btn-sm btn-primary">
                             Manage
                         </a>
+                    {% else %}
+                        Shared
                     {% endif %}
                     </div>
                 </div>
             </li>
         {% endfor %}
     </ul>
 {% else %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% if billing_accounts_list|length %}
 +_Billing_Account
     * Name
       Actions
     * {% for billing_account in billing_accounts_list %}
     * {{_billing_account.name_}}
-      {% if billing_account.is_owner %} Manage {% endif %}
+      {% if billing_account.is_owner %} Manage {% else %} Shared {% endif %}
     * {% endfor %}
 {% else %}
 You don't have any billing accounts.
 Create_one_using_the_Google_Cloud_Platform_console.
 {% endif %}
```

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.1.0/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.1.0/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.1.0/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.1.0/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.1.0/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.1.0/environment/templates/environment/research_environments.html`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     const csrfToken = getCookie("csrftoken");
 
     return function(request_data, http_method, url, button_type) {
         $(".inside-modal-button").prop("disabled", true);
 
         let data = request_data;
         if (button_type === "update") {
-            const instance = $("#form-select option:selected").text();
+            const instance = $("#form-select option:selected").val();
             if (instance === "") return;
 
             data = JSON.parse(data);
             data["instance_type"] = instance;
             data = JSON.stringify(data);
         }
         fetch(url, {
```

### Comparing `hdn-research-environment-2.0.7/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.1.0/environment/templates/tag/environment_modal_button.html`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       <div class="modal-header">
         <h5 class="modal-title" id="exampleModalLongTitle">{{ modal_title }}</h5>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
           <span aria-hidden="true">&times;</span>
         </button>
       </div>
       <div class="modal-body">
-        {% if instance_types != None %}
+        {% if instances_dict != None %}
             <select class="form-select" id="form-select" size="5" aria-label="size 5 select example">
-              {% for instance_type in instance_types %}
-                <option value="instance_type">{{ instance_type }}</option>
+              {% for instance_type, instance_specification in instances_dict.items %}
+                <option value="{{ instance_type }}">{{ instance_specification }}</option>
               {% endfor %}
             </select>
         {% else %}
             <p>{{ modal_body }}</p>
         {% endif %}
       </div>
       <div class="modal-footer">
```

### Comparing `hdn-research-environment-2.0.7/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.1.0/environment/templatetags/action_buttons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 from django import template
 from django.urls import reverse
 from django.db.models import Model
 
-from environment.entities import ResearchEnvironment, InstanceType
+from environment.entities import ResearchEnvironment
+from environment.constants import INSTANCE_TYPE_SPECIFICATION
 
 
 PublishedProject = Model
 
 
 register = template.Library()
 
@@ -83,16 +84,15 @@
         "button_class": data["button_class"],
         "modal_title": data["modal_title"],
         "modal_body": data["modal_body"],
         "modal_id": f"{data['action_button_type']}-{environment.id}",
         "action_button_type": data["action_button_type"],
     }
     if button_type == "modal_instance":
-        instance_types = [t.value for t in InstanceType]
-        result_data["instance_types"] = instance_types
+        result_data["instances_dict"] = INSTANCE_TYPE_SPECIFICATION
 
     return result_data
 
 
 @register.inclusion_tag("tag/environment_action_button.html")
 def environment_action_button(
     environment: ResearchEnvironment,
```

### Comparing `hdn-research-environment-2.0.7/environment/tests/helpers.py` & `hdn-research-environment-2.1.0/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tests/mocks.py` & `hdn-research-environment-2.1.0/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tests/test_decorators.py` & `hdn-research-environment-2.1.0/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tests/test_services.py` & `hdn-research-environment-2.1.0/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tests/test_signals.py` & `hdn-research-environment-2.1.0/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tests/test_utilities.py` & `hdn-research-environment-2.1.0/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tests/test_validators.py` & `hdn-research-environment-2.1.0/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/tests/test_views.py` & `hdn-research-environment-2.1.0/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/urls.py` & `hdn-research-environment-2.1.0/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/utilities.py` & `hdn-research-environment-2.1.0/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.7/environment/views.py` & `hdn-research-environment-2.1.0/environment/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     require_DELETE,
     require_PATCH,
 )
 from environment.entities import Region, InstanceType
 from environment.utilities import (
     user_has_cloud_identity,
 )
-from environment.models import Workflow
+from environment.models import Workflow, BillingAccountSharingInvite
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 def identity_provisioning(request):
     if user_has_cloud_identity(request.user):
         return redirect("research_environments")
@@ -286,20 +286,30 @@
         "pending_shares": pending_shares,
         "consumed_shares": consumed_shares,
     }
 
     return render(request, "environment/manage_billing_account.html", context)
 
 
-@require_GET
+@require_http_methods(["GET", "POST"])
 @login_required
 def confirm_billing_account_sharing(request):
-    token = request.GET.get("token")
-    if token:
+    if request.method == "POST":
+        token = request.POST["token"]
         services.consume_billing_account_sharing_token(user=request.user, token=token)
+    else:
+        token = request.GET.get("token")
+        if token:
+            invite = BillingAccountSharingInvite.objects.select_related("owner").get(
+                token=token, is_revoked=False
+            )
+            context = {"token": token, "invitation_owner": invite.owner}
+            return render(
+                request, "environment/manage_shared_billing_invitation.html", context
+            )
 
     return redirect("research_environments")
 
 
 @require_PATCH
 @login_required
 @cloud_identity_required
```

### Comparing `hdn-research-environment-2.0.7/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.1.0/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.7
+Version: 2.1.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.7/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.1.0/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 environment/templates/environment/_available_projects_list.html
 environment/templates/environment/_billing_accounts_list.html
 environment/templates/environment/base_environment_home.html
 environment/templates/environment/create_research_environment.html
 environment/templates/environment/create_workspace.html
 environment/templates/environment/identity_provisioning.html
 environment/templates/environment/manage_billing_account.html
+environment/templates/environment/manage_shared_billing_invitation.html
 environment/templates/environment/research_environments.html
 environment/templates/environment/email/billing_sharing_confirmation.html
 environment/templates/environment/email/environment_access_expired.html
 environment/templates/tag/environment_action_button.html
 environment/templates/tag/environment_modal_button.html
 environment/templatetags/__init__.py
 environment/templatetags/action_buttons.py
```

### Comparing `hdn-research-environment-2.0.7/setup.cfg` & `hdn-research-environment-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.0.7
+version = 2.1.0
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

