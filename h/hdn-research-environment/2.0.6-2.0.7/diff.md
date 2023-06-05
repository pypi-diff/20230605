# Comparing `tmp/hdn-research-environment-2.0.6.tar.gz` & `tmp/hdn-research-environment-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.0.6.tar", last modified: Fri Jun  2 15:32:34 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.0.7.tar", last modified: Mon Jun  5 06:46:33 2023, max compression
```

## Comparing `hdn-research-environment-2.0.6.tar` & `hdn-research-environment-2.0.7.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.6/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.6/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.6/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.6/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.6/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.6/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.6/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    19234 2023-06-01 18:10:39.000000 hdn-research-environment-2.0.6/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.0.6/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.6/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.6/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     7425 2023-06-01 18:10:39.000000 hdn-research-environment-2.0.6/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.0.6/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.6/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.6/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.6/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.6/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.6/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.6/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    13441 2023-06-02 15:32:09.000000 hdn-research-environment-2.0.6/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-02 15:32:33.000000 hdn-research-environment-2.0.6/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-06-02 15:32:33.000000 hdn-research-environment-2.0.6/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-02 15:32:33.000000 hdn-research-environment-2.0.6/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-02 15:32:33.000000 hdn-research-environment-2.0.6/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-02 15:32:33.000000 hdn-research-environment-2.0.6/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.6/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-02 15:32:34.000000 hdn-research-environment-2.0.6/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.6/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.7/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.7/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.7/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.7/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.7/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1600 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.7/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    18751 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.0.7/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.7/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.7/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7615 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.0.7/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.7/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.7/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      251 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.7/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.7/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.7/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.7/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13367 2023-06-05 06:46:01.000000 hdn-research-environment-2.0.7/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3028 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.7/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-05 06:46:33.000000 hdn-research-environment-2.0.7/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.7/setup.py
```

### Comparing `hdn-research-environment-2.0.6/LICENSE` & `hdn-research-environment-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/PKG-INFO` & `hdn-research-environment-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.6
+Version: 2.0.7
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.6/environment/api/v1/__init__.py` & `hdn-research-environment-2.0.7/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/api/v1/auth.py` & `hdn-research-environment-2.0.7/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/api/v1/decorators.py` & `hdn-research-environment-2.0.7/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/api/v2/__init__.py` & `hdn-research-environment-2.0.7/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/api/v2/decorators.py` & `hdn-research-environment-2.0.7/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/constants.py` & `hdn-research-environment-2.0.7/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/decorators.py` & `hdn-research-environment-2.0.7/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/deserializers.py` & `hdn-research-environment-2.0.7/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/entities.py` & `hdn-research-environment-2.0.7/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/exceptions.py` & `hdn-research-environment-2.0.7/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/forms.py` & `hdn-research-environment-2.0.7/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/migrations/0001_initial.py` & `hdn-research-environment-2.0.7/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.0.7/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.0.7/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.0.7/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.0.7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/models.py` & `hdn-research-environment-2.0.7/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/services.py` & `hdn-research-environment-2.0.7/environment/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Tuple, Iterable, Optional, Dict
 from collections import defaultdict
 
 from django.db.models import Model
-from django.core.mail import send_mail
-from django.template import loader
-from django.conf import settings
+from django.contrib.sites.shortcuts import get_current_site
 from django.apps import apps
 from google.cloud.workflows import executions_v1beta
 from google.cloud.workflows.executions_v1beta.types import executions
 
 import environment.constants as constants
 import environment.mailers as mailers
 import environment.api.v1 as api_v1
@@ -114,15 +112,16 @@
     request, owner: User, user_email: str, billing_account_id: str
 ) -> BillingAccountSharingInvite:
     invite = BillingAccountSharingInvite.objects.create(
         owner=owner,
         billing_account_id=billing_account_id,
         user_contact_email=user_email,
     )
-    mailers.send_billing_sharing_confirmation(request=request, invite=invite)
+    site_domain = get_current_site(request).domain
+    mailers.send_billing_sharing_confirmation(site_domain=site_domain, invite=invite)
     return invite
 
 
 def consume_billing_account_sharing_token(
     user: User, token: str
 ) -> BillingAccountSharingInvite:
     invite = BillingAccountSharingInvite.objects.get(token=token, is_revoked=False)
@@ -514,30 +513,14 @@
         type=Workflow.DESTROY,
         workspace_name=gcp_project_id,
     )
 
     return response.json()
 
 
-def send_environment_access_expired_email(
-    user: User, projects: Iterable[PublishedProject]
-):
-    subject = f"{settings.SITE_NAME} Environment Access Expired"
-    email_context = {
-        "signature": settings.EMAIL_SIGNATURE,
-        "projects": projects,
-    }
-    body = loader.render_to_string(
-        "environment/email/environment_access_expired.html", email_context
-    )
-    send_mail(
-        subject, body, settings.DEFAULT_FROM_EMAIL, [user.email], fail_silently=False
-    )
-
-
 def persist_workflow(
     user: User,
     execution_resource_name: str,
     type: int,
     project_id: Optional[int] = None,
     workspace_name: Optional[str] = None,
 ) -> Workflow:
```

### Comparing `hdn-research-environment-2.0.6/environment/signals.py` & `hdn-research-environment-2.0.7/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.0.7/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.0.7/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.0.7/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.0.7/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tasks.py` & `hdn-research-environment-2.0.7/environment/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from django.db import transaction
 from django.utils import timezone
 
 from environment.services import (
     get_environment_project_pairs_with_expired_access,
     stop_running_environment,
     delete_environment,
-    send_environment_access_expired_email,
     share_billing_account,
 )
+from environment.mailers import send_environment_access_expired
 from environment.models import BillingAccountSharingInvite
 
 
 User = get_user_model()
 
 Event = apps.get_model("events", "Event")
 
@@ -51,15 +51,15 @@
     expired_pairs = get_environment_project_pairs_with_expired_access(user)
     environments, projects = zip(*expired_pairs)
     for environment in environments:
         if environment.is_running:
             stop_running_environment(
                 user, environment.id, environment.region, environment.workspace_name
             )
-    send_environment_access_expired_email(user, projects)
+    send_environment_access_expired(user, projects)
     if len(environments) > 0:
         environment_ids = [environment.id for environment in environments]
         terminate_environments_if_access_still_expired(
             user_id,
             environment_ids,
             schedule=_expired_environment_termination_schedule(),
         )
```

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.0.7/environment/templates/environment/_available_environments_list.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 {% load action_buttons %}
 
 {% if recent_workflow %}
     {% if recent_workflow_failed %}
-        <div class="alert alert-danger" role="alert">
-            {{ recent_workflow.get_type_display }} {{ recent_workflow.project }} failed! Try again later.
+    <div class="alert alert-danger" role="alert">
+            {{ recent_workflow.get_type_display }}
+            {% if recent_workflow.project %}
+                {{ recent_workflow.project }}
+            {% endif %}
+            failed! Try again later.
         </div>
     {% elif recent_workflow_succeeded %}
         <div class="alert alert-success" role="alert">
-            {{ recent_workflow.get_type_display }} {{ recent_workflow.project }} finished!
+            {{ recent_workflow.get_type_display }}
+            {% if recent_workflow.project %}
+                {{ recent_workflow.project }}
+            {% endif %}
+            finished!
         </div>
     {% endif %}
 {% endif %}
 
 <div class="d-flex flex-column align-items-end px-4 mb-3">
     <a class="btn btn-primary btn-sm" href="{% url 'create_workspace' %}">
       + Workspace
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% load action_buttons %} {% if recent_workflow %} {% if recent_workflow_failed
 %}
-{{ recent_workflow.get_type_display }} {{ recent_workflow.project }} failed!
-Try again later.
+{{ recent_workflow.get_type_display }} {% if recent_workflow.project %} {
+{ recent_workflow.project }} {% endif %} failed! Try again later.
 {% elif recent_workflow_succeeded %}
-{{ recent_workflow.get_type_display }} {{ recent_workflow.project }} finished!
+{{ recent_workflow.get_type_display }} {% if recent_workflow.project %} {
+{ recent_workflow.project }} {% endif %} finished!
 {% endif %} {% endif %}
 +_Workspace
 {% for workflow in workspace_creation_workflows %}
 {{ heading }}">
 Provisioning
 Loading...
 {% endfor %} {% for workspace_name, environments_project_workflow_triplets in
```

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.0.7/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.0.7/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.0.7/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.0.7/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.0.7/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.0.7/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.0.7/environment/templates/environment/manage_billing_account.html`

 * *Files 8% similar despite different names*

```diff
@@ -73,16 +73,16 @@
                                     {{ share.user_contact_email }}
                                 </div>
                                 <div class="col-md-4">
                                     <form action="{% url 'manage_billing_account' billing_account_id=billing_account_id %}" method="post">
                                         {% csrf_token %}
                                         <input type="hidden" name="action" value="revoke_access">
                                         <input type="hidden" name="share_id" value="{{ share.id }}">
-                                        <button class="btn btn-sm btn-danger" type="submit">
-                                            Revoke
+                                        <button class="btn btn-sm btn-secondary" type="submit">
+                                            Cancel
                                         </button>
                                     </form>
                                 </div>
                             </div>
                         </li>
                         {% endfor %}
                     </ul>
@@ -110,17 +110,22 @@
                         {% for share in consumed_shares %}
                         <li class="list-group-item">
                             <div class="row">
                                 <div class="col-md-8">
                                     {{ share.user_contact_email }}
                                 </div>
                                 <div class="col-md-4">
-                                    <a href="" class="btn btn-sm btn-danger disabled">
-                                        Revoke
-                                    </a>
+                                    <form action="{% url 'manage_billing_account' billing_account_id=billing_account_id %}" method="post">
+                                        {% csrf_token %}
+                                        <input type="hidden" name="action" value="revoke_access">
+                                        <input type="hidden" name="share_id" value="{{ share.id }}">
+                                        <button class="btn btn-sm btn-danger" type="submit">
+                                            Revoke
+                                        </button>
+                                    </form>
                                 </div>
                             </div>
                         </li>
                         {% endfor %}
                     </ul>
                 </div>
             </div>
```

### Comparing `hdn-research-environment-2.0.6/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.0.7/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.0.7/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.0.7/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/helpers.py` & `hdn-research-environment-2.0.7/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/mocks.py` & `hdn-research-environment-2.0.7/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/test_decorators.py` & `hdn-research-environment-2.0.7/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/test_services.py` & `hdn-research-environment-2.0.7/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/test_signals.py` & `hdn-research-environment-2.0.7/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/test_utilities.py` & `hdn-research-environment-2.0.7/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/test_validators.py` & `hdn-research-environment-2.0.7/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/tests/test_views.py` & `hdn-research-environment-2.0.7/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/urls.py` & `hdn-research-environment-2.0.7/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/utilities.py` & `hdn-research-environment-2.0.7/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.6/environment/views.py` & `hdn-research-environment-2.0.7/environment/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,19 +233,18 @@
                 messages.error(
                     request,
                     f"Quota exceeded - the specified configuration would use {cpu_usage} out of {constants.MAX_CPU_USAGE} CPUs",
                 )
     else:
         form = CreateResearchEnvironmentForm(workspace_list=workspaces_list)
 
-    exceeded_quotas = services.exceeded_quotas(request.user)
     context = {
         "form": form,
         "project": project,
-        "exceeded_quotas": exceeded_quotas,
+        "exceeded_quotas": [],
         "instance_projected_costs": constants.INSTANCE_PROJECTED_COSTS,
         "gpu_projected_costs": constants.GPU_PROJECTED_COSTS,
         "data_storage_projected_costs": constants.DATA_STORAGE_PROJECTED_COSTS,
     }
     return render(request, "environment/create_research_environment.html", context)
```

### Comparing `hdn-research-environment-2.0.6/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.0.7/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.6
+Version: 2.0.7
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.6/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.0.7/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 environment/templates/environment/_billing_accounts_list.html
 environment/templates/environment/base_environment_home.html
 environment/templates/environment/create_research_environment.html
 environment/templates/environment/create_workspace.html
 environment/templates/environment/identity_provisioning.html
 environment/templates/environment/manage_billing_account.html
 environment/templates/environment/research_environments.html
+environment/templates/environment/email/billing_sharing_confirmation.html
 environment/templates/environment/email/environment_access_expired.html
 environment/templates/tag/environment_action_button.html
 environment/templates/tag/environment_modal_button.html
 environment/templatetags/__init__.py
 environment/templatetags/action_buttons.py
 environment/tests/__init__.py
 environment/tests/helpers.py
```

### Comparing `hdn-research-environment-2.0.6/setup.cfg` & `hdn-research-environment-2.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.0.6
+version = 2.0.7
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

