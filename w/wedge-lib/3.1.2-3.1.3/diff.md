# Comparing `tmp/wedge-lib-3.1.2.tar.gz` & `tmp/wedge-lib-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedge-lib-3.1.2.tar", last modified: Thu Jun  1 10:13:27 2023, max compression
+gzip compressed data, was "wedge-lib-3.1.3.tar", last modified: Mon Jun  5 07:53:57 2023, max compression
```

## Comparing `wedge-lib-3.1.2.tar` & `wedge-lib-3.1.3.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.167855 wedge-lib-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-01 10:13:27.167855 wedge-lib-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-01 10:13:27.167855 wedge-lib-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/data_test_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/data_test_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/data_test_factory/data_test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/commands/abstract_maintenance_mode_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/services/business/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/services/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/services/business/user_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/templatetags/util_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/tests/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/builders/user_test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/django_testcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/django/tests/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/factories/auth_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/factories/reference_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/tests/view_testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/django/w_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/drf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/drf/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/decorators/group_required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/exception_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/drf/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/jwt/jwt_authentication_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/jwt/jwt_viewset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/jwt/login_viewset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.151855 wedge-lib-3.1.2/w/drf/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/middlewares/maintenance_mode_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/drf/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/serializers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/serializers/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/serializers/serpy_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/drf/sso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/sso/sso_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/sso/sso_user_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/drf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/tests/api_testcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/drf/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/tests/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/drf/tests/helpers/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/tests/helpers/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/tests/helpers/jwt/jwt_test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/drf/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/validators/drf_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/mixins/dataclasses_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/mixins/thread_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/serializers/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/abstract_model_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/abstract_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/services/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/imports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.155855 wedge-lib-3.1.2/w/services/imports/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/imports/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/imports/models/import_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/services/technical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/abstract_import_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/boto3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/cloudinary_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/context_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/csv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/date_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/db_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/dict_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/excel_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/filesystem_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/google_map_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/ip_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/json_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/key_generator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/list_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/maintenance_mode_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/services/technical/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/models/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/models/csv_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/models/request_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/models/request_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/models/yousign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/pdf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/sso_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/string_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/template_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/uniqid_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/url_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/yaml_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/services/technical/yousign_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/tests/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/builders/abstract_test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/builders/test_test_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/tests/drf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/drf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/tests/drf/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/drf/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/drf/middlewares/test_maintenance_mode_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/drf/test_model_service_viewset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/drf/test_viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/tests/fixtures/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.159855 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/builder_with_auto_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/factory_boy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/simple_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.163855 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/drf_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/dtf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/dtf_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/example_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/factory_boys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/serpy_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/simple_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.163855 wedge-lib-3.1.2/w/tests/fixtures/datasets/sso_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/sso_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/sso_service/create_sso_user_with_success_return_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/sso_service/get_or_create_sso_user_with_success_return_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/fixtures/datasets/sso_service/get_or_create_user_with_unknown_user_return_user.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.163855 wedge-lib-3.1.2/w/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/auth_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/cloudinary_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/date_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/google_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/orm_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/request_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/service_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/sso_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/helpers/yousign_test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.163855 wedge-lib-3.1.2/w/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/mixins/api_viewset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/mixins/boto3test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/mixins/factory_boy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/mixins/faker_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/mixins/serializer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/mixins/testcase_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.163855 wedge-lib-3.1.2/w/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/serializers/serpy_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/serializers/test_serpy_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.163855 wedge-lib-3.1.2/w/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.167855 wedge-lib-3.1.2/w/tests/services/technical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_abstract_import_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_boto3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_cloudinary_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_context_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_csv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_date_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_dict_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_excel_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_filesystem_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_google_map_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_ip_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_json_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_key_generator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_list_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_mail_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_maintenance_mode_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_pdf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_sso_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_string_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_template_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_uniqid_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_url_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_yaml_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/technical/test_yousign_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/tests/services/test_abstract_model_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-01 10:11:11.000000 wedge-lib-3.1.2/w/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:13:27.167855 wedge-lib-3.1.2/wedge_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-01 10:13:27.000000 wedge-lib-3.1.2/wedge_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-01 10:13:27.000000 wedge-lib-3.1.2/wedge_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:13:27.000000 wedge-lib-3.1.2/wedge_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 10:13:27.000000 wedge-lib-3.1.2/wedge_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-01 10:13:27.000000 wedge-lib-3.1.2/wedge_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.981782 wedge-lib-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-05 07:53:57.981782 wedge-lib-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-05 07:53:57.981782 wedge-lib-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/data_test_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/data_test_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/data_test_factory/data_test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/commands/abstract_maintenance_mode_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/services/business/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/services/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/services/business/user_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/templatetags/util_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/tests/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/builders/user_test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/django_testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.953782 wedge-lib-3.1.3/w/django/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/factories/auth_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/factories/reference_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/tests/view_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/django/w_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/decorators/group_required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/exception_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/jwt/jwt_authentication_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/jwt/jwt_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/jwt/login_viewset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/middlewares/maintenance_mode_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/serializers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/serializers/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/serializers/serpy_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/sso/sso_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/sso/sso_user_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/tests/api_testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/tests/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/tests/helpers/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/tests/helpers/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/tests/helpers/jwt/jwt_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/drf/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/validators/drf_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.957782 wedge-lib-3.1.3/w/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/mixins/dataclasses_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/mixins/thread_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.961782 wedge-lib-3.1.3/w/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/serializers/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.961782 wedge-lib-3.1.3/w/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/abstract_model_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/abstract_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.961782 wedge-lib-3.1.3/w/services/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/imports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.961782 wedge-lib-3.1.3/w/services/imports/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/imports/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/imports/models/import_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.965782 wedge-lib-3.1.3/w/services/technical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/abstract_import_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/boto3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/cloudinary_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/context_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/csv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/date_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/db_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/dict_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/excel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/filesystem_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/google_map_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/ip_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/json_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/key_generator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/list_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/maintenance_mode_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.965782 wedge-lib-3.1.3/w/services/technical/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/models/csv_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/models/request_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/models/request_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/models/yousign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/pdf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/sso_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/string_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/template_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/uniqid_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/url_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/yaml_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/services/technical/yousign_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.965782 wedge-lib-3.1.3/w/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.965782 wedge-lib-3.1.3/w/tests/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/builders/abstract_test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/builders/test_test_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.969782 wedge-lib-3.1.3/w/tests/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/drf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.969782 wedge-lib-3.1.3/w/tests/drf/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/drf/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/drf/middlewares/test_maintenance_mode_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/drf/test_model_service_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/drf/test_viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.969782 wedge-lib-3.1.3/w/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.969782 wedge-lib-3.1.3/w/tests/fixtures/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.969782 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/builder_with_auto_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/factory_boy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/simple_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.969782 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/drf_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/dtf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/dtf_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/example_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/factory_boys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/serpy_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/simple_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.973782 wedge-lib-3.1.3/w/tests/fixtures/datasets/sso_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/sso_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/sso_service/create_sso_user_with_success_return_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/sso_service/get_or_create_sso_user_with_success_return_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/fixtures/datasets/sso_service/get_or_create_user_with_unknown_user_return_user.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.973782 wedge-lib-3.1.3/w/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/auth_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/cloudinary_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/date_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/google_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/orm_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/request_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/service_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/sso_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/helpers/yousign_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.973782 wedge-lib-3.1.3/w/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/mixins/api_viewset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/mixins/boto3test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/mixins/factory_boy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/mixins/faker_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/mixins/serializer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/mixins/testcase_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.973782 wedge-lib-3.1.3/w/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/serializers/serpy_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/serializers/test_serpy_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.977782 wedge-lib-3.1.3/w/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.981782 wedge-lib-3.1.3/w/tests/services/technical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_abstract_import_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_boto3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_cloudinary_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_context_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_csv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_date_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_dict_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_excel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_filesystem_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_google_map_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_ip_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_json_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_key_generator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_list_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_maintenance_mode_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_pdf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_sso_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_string_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_template_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_uniqid_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_url_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_yaml_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/technical/test_yousign_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/tests/services/test_abstract_model_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-05 07:51:11.000000 wedge-lib-3.1.3/w/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:53:57.981782 wedge-lib-3.1.3/wedge_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-05 07:53:57.000000 wedge-lib-3.1.3/wedge_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-05 07:53:57.000000 wedge-lib-3.1.3/wedge_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:53:57.000000 wedge-lib-3.1.3/wedge_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 07:53:57.000000 wedge-lib-3.1.3/wedge_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 07:53:57.000000 wedge-lib-3.1.3/wedge_lib.egg-info/top_level.txt
```

### Comparing `wedge-lib-3.1.2/LICENSE.txt` & `wedge-lib-3.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/PKG-INFO` & `wedge-lib-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedge-lib
-Version: 3.1.2
+Version: 3.1.3
 Summary: Wedge library for django application
 Home-page: https://github.com/Wedge-Digital/w
 Author-email: francois.schneider@wedge-digital.com
 License: MIT
 Description: # Wedge Library
         
         ## Démarrage rapide
```

### Comparing `wedge-lib-3.1.2/README.md` & `wedge-lib-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/setup.cfg` & `wedge-lib-3.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/setup.py` & `wedge-lib-3.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/data_test_factory/data_test_factory.py` & `wedge-lib-3.1.3/w/data_test_factory/data_test_factory.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/debug.py` & `wedge-lib-3.1.3/w/debug.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/commands/abstract_maintenance_mode_command.py` & `wedge-lib-3.1.3/w/django/commands/abstract_maintenance_mode_command.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/models.py` & `wedge-lib-3.1.3/w/django/models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/services/business/user_service.py` & `wedge-lib-3.1.3/w/django/services/business/user_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/tests/django_testcase.py` & `wedge-lib-3.1.3/w/django/tests/django_testcase.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/tests/factories/auth_factories.py` & `wedge-lib-3.1.3/w/django/tests/factories/auth_factories.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/tests/view_testcase.py` & `wedge-lib-3.1.3/w/django/tests/view_testcase.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/utils.py` & `wedge-lib-3.1.3/w/django/utils.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/django/w_command.py` & `wedge-lib-3.1.3/w/django/w_command.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/decorators/group_required.py` & `wedge-lib-3.1.3/w/drf/decorators/group_required.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/exception_handler.py` & `wedge-lib-3.1.3/w/drf/exception_handler.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/jwt/jwt_authentication_backend.py` & `wedge-lib-3.1.3/w/drf/jwt/jwt_authentication_backend.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/jwt/jwt_viewset.py` & `wedge-lib-3.1.3/w/drf/jwt/jwt_viewset.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/jwt/login_viewset.py` & `wedge-lib-3.1.3/w/drf/jwt/login_viewset.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/middlewares/maintenance_mode_middleware.py` & `wedge-lib-3.1.3/w/drf/middlewares/maintenance_mode_middleware.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/mixins.py` & `wedge-lib-3.1.3/w/drf/mixins.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/serializers/fields.py` & `wedge-lib-3.1.3/w/drf/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/serializers/serpy_serializers.py` & `wedge-lib-3.1.3/w/drf/serializers/serpy_serializers.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/sso/sso_auth_backend.py` & `wedge-lib-3.1.3/w/drf/sso/sso_auth_backend.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/sso/sso_user_mixin.py` & `wedge-lib-3.1.3/w/drf/sso/sso_user_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/tests/api_testcase.py` & `wedge-lib-3.1.3/w/drf/tests/api_testcase.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/tests/helpers/jwt/jwt_test_helper.py` & `wedge-lib-3.1.3/w/drf/tests/helpers/jwt/jwt_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/drf/viewsets.py` & `wedge-lib-3.1.3/w/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/exceptions.py` & `wedge-lib-3.1.3/w/exceptions.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/serializers/serializer.py` & `wedge-lib-3.1.3/w/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/abstract_model_service.py` & `wedge-lib-3.1.3/w/services/abstract_model_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/abstract_service.py` & `wedge-lib-3.1.3/w/services/abstract_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/abstract_import_service.py` & `wedge-lib-3.1.3/w/services/technical/abstract_import_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/auth_service.py` & `wedge-lib-3.1.3/w/services/technical/auth_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/boto3_service.py` & `wedge-lib-3.1.3/w/services/technical/boto3_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/cloudinary_service.py` & `wedge-lib-3.1.3/w/services/technical/cloudinary_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/context_service.py` & `wedge-lib-3.1.3/w/services/technical/context_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/csv_service.py` & `wedge-lib-3.1.3/w/services/technical/csv_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/date_service.py` & `wedge-lib-3.1.3/w/services/technical/date_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/dict_service.py` & `wedge-lib-3.1.3/w/services/technical/dict_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/excel_service.py` & `wedge-lib-3.1.3/w/services/technical/excel_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/file_service.py` & `wedge-lib-3.1.3/w/services/technical/file_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/filesystem_service.py` & `wedge-lib-3.1.3/w/services/technical/filesystem_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/google_map_service.py` & `wedge-lib-3.1.3/w/services/technical/google_map_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/json_service.py` & `wedge-lib-3.1.3/w/services/technical/json_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/key_generator_service.py` & `wedge-lib-3.1.3/w/services/technical/key_generator_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/list_service.py` & `wedge-lib-3.1.3/w/services/technical/list_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/mail_service.py` & `wedge-lib-3.1.3/w/services/technical/mail_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/maintenance_mode_service.py` & `wedge-lib-3.1.3/w/services/technical/maintenance_mode_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/models/request_response.py` & `wedge-lib-3.1.3/w/services/technical/models/request_response.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/models/request_session.py` & `wedge-lib-3.1.3/w/services/technical/models/request_session.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/models/sso.py` & `wedge-lib-3.1.3/w/services/technical/models/sso.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/models/yousign.py` & `wedge-lib-3.1.3/w/services/technical/models/yousign.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/pdf_service.py` & `wedge-lib-3.1.3/w/services/technical/pdf_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/request_service.py` & `wedge-lib-3.1.3/w/services/technical/request_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             data (dict|str): data to post/put/patch
             session (RequestSession|None): session from RequestService::init_session
             **kwargs:  Optional arguments that lib ``request`` takes (like timeout).
 
         Returns:
             Response
         """
-        logger.info('Request %s %s"', action.upper(), url, data)
+        logger.info("Request %s %s", action.upper(), url, data)
         logger.debug('data="%s" kwargs="%s"', data, kwargs)
         try:
             if session is not None:
                 if session.timeout is not None:
                     kwargs["timeout"] = session.timeout
                 response = getattr(session.request, action)(
                     session.render_url(url), data=data, **kwargs
```

### Comparing `wedge-lib-3.1.2/w/services/technical/sso_service.py` & `wedge-lib-3.1.3/w/services/technical/sso_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/string_service.py` & `wedge-lib-3.1.3/w/services/technical/string_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/uniqid_service.py` & `wedge-lib-3.1.3/w/services/technical/uniqid_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/url_service.py` & `wedge-lib-3.1.3/w/services/technical/url_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/yaml_service.py` & `wedge-lib-3.1.3/w/services/technical/yaml_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/services/technical/yousign_service.py` & `wedge-lib-3.1.3/w/services/technical/yousign_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/builders/abstract_test_builder.py` & `wedge-lib-3.1.3/w/tests/builders/abstract_test_builder.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/builders/test_test_builder.py` & `wedge-lib-3.1.3/w/tests/builders/test_test_builder.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/drf/middlewares/test_maintenance_mode_middleware.py` & `wedge-lib-3.1.3/w/tests/drf/middlewares/test_maintenance_mode_middleware.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/drf/test_model_service_viewset.py` & `wedge-lib-3.1.3/w/tests/drf/test_model_service_viewset.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/drf/test_viewsets.py` & `wedge-lib-3.1.3/w/tests/drf/test_viewsets.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/builder_with_internal_dependencies.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/builder_with_related_dependencies.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/factory_boy.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/factory_boy.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/builders/models.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/builders/models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/drf_serializer.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/drf_serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/dtf_models.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/dtf_models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/dtf_recipes.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/dtf_recipes.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/models.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/models.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/serpy_serializer.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/serpy_serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/fixtures/datasets/django_app/viewsets.py` & `wedge-lib-3.1.3/w/tests/fixtures/datasets/django_app/viewsets.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/helpers/cloudinary_test_helper.py` & `wedge-lib-3.1.3/w/tests/helpers/cloudinary_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/helpers/google_test_helper.py` & `wedge-lib-3.1.3/w/tests/helpers/google_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/helpers/request_test_helper.py` & `wedge-lib-3.1.3/w/tests/helpers/request_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/helpers/service_test_helper.py` & `wedge-lib-3.1.3/w/tests/helpers/service_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/helpers/sso_test_helper.py` & `wedge-lib-3.1.3/w/tests/helpers/sso_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/helpers/yousign_test_helper.py` & `wedge-lib-3.1.3/w/tests/helpers/yousign_test_helper.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/mixins/api_viewset_mixin.py` & `wedge-lib-3.1.3/w/tests/mixins/api_viewset_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/mixins/boto3test_mixin.py` & `wedge-lib-3.1.3/w/tests/mixins/boto3test_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/mixins/factory_boy_mixin.py` & `wedge-lib-3.1.3/w/tests/mixins/factory_boy_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/mixins/testcase_mixin.py` & `wedge-lib-3.1.3/w/tests/mixins/testcase_mixin.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/serializers/serpy_serializers.py` & `wedge-lib-3.1.3/w/tests/serializers/serpy_serializers.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/serializers/test_serpy_serializer.py` & `wedge-lib-3.1.3/w/tests/serializers/test_serpy_serializer.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_abstract_import_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_abstract_import_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_auth_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_auth_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_boto3_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_boto3_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_cloudinary_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_cloudinary_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_context_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_context_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_csv_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_csv_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_date_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_date_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_dict_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_dict_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_excel_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_excel_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_file_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_file_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_filesystem_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_filesystem_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_google_map_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_google_map_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_ip_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_ip_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_json_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_json_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_key_generator_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_key_generator_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_list_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_list_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_mail_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_mail_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_maintenance_mode_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_maintenance_mode_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_pdf_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_pdf_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_request_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_request_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_sso_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_sso_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_string_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_string_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_template_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_template_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_uniqid_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_uniqid_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_url_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_url_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_yaml_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_yaml_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/technical/test_yousign_service.py` & `wedge-lib-3.1.3/w/tests/services/technical/test_yousign_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/tests/services/test_abstract_model_service.py` & `wedge-lib-3.1.3/w/tests/services/test_abstract_model_service.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/w/utils.py` & `wedge-lib-3.1.3/w/utils.py`

 * *Files identical despite different names*

### Comparing `wedge-lib-3.1.2/wedge_lib.egg-info/PKG-INFO` & `wedge-lib-3.1.3/wedge_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedge-lib
-Version: 3.1.2
+Version: 3.1.3
 Summary: Wedge library for django application
 Home-page: https://github.com/Wedge-Digital/w
 Author-email: francois.schneider@wedge-digital.com
 License: MIT
 Description: # Wedge Library
         
         ## Démarrage rapide
```

### Comparing `wedge-lib-3.1.2/wedge_lib.egg-info/SOURCES.txt` & `wedge-lib-3.1.3/wedge_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

