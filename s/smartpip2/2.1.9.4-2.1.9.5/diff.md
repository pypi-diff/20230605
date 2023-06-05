# Comparing `tmp/smartpip2-2.1.9.4.tar.gz` & `tmp/smartpip2-2.1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smartpip2-2.1.9.4.tar", last modified: Wed Apr 26 09:55:12 2023, max compression
+gzip compressed data, was "dist/smartpip2-2.1.9.5.tar", last modified: Mon Jun  5 02:46:38 2023, max compression
```

## Comparing `smartpip2-2.1.9.4.tar` & `smartpip2-2.1.9.5.tar`

### file list

```diff
@@ -1,1118 +1,1117 @@
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/
--rw-rw-r--   0 johnyan    (501) staff       (20)   274732 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/CHANGELOG.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)    13444 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/LICENSE
--rw-rw-r--   0 johnyan    (501) staff       (20)     1433 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/MANIFEST.in
--rw-rw-r--   0 johnyan    (501) staff       (20)      404 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/NOTICE
--rw-r--r--   0 johnyan    (501) staff       (20)    26641 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/PKG-INFO
--rw-rw-r--   0 johnyan    (501) staff       (20)    20139 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/README.md
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/
--rw-r--r--   0 johnyan    (501) staff       (20)     2751 2022-07-19 14:54:13.000000 smartpip2-2.1.9.4/airflow/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1368 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/__main__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/
--rw-r--r--   0 johnyan    (501) staff       (20)     1430 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)       95 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/__main__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/
--rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18192 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/abstract.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14270 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/aiohttp_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12812 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2222 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_utils.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/
--rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10764 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/abstract.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/aiohttp_app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5023 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/flask_app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/cli.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1842 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/coroutine_wrappers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1441 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/decorator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1752 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/metrics.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/parameter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/produces.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/response.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9853 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/security.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11690 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/uri_parsing.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15533 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/validation.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/exceptions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2692 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/handlers.py
--rw-r--r--   0 johnyan    (501) staff       (20)      212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/http_facts.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4050 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/json_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/jsonifier.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/lifecycle.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/mock.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/
--rw-r--r--   0 johnyan    (501) staff       (20)      294 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15461 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/abstract.py
--rw-r--r--   0 johnyan    (501) staff       (20)      127 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/compat.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14505 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/openapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6782 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/secure.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/swagger2.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4444 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/options.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1926 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/problem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6810 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/resolver.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3408 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/setup.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/spec.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6515 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2320 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/alembic.ini
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/
--rw-r--r--   0 johnyan    (501) staff       (20)     1550 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/auth/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2258 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/basic_auth.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1342 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/default.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/deny_all.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5563 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/kerberos_auth.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1500 2022-07-04 11:00:25.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/smart_auth.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/client/
--rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2465 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/api_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/json_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2223 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/local_client.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/common/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/
--rw-r--r--   0 johnyan    (501) staff       (20)     2045 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/delete_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)      329 2020-10-10 01:23:08.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/gen_dag_file.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1426 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_code.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1381 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_run_state.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1982 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_runs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1886 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_lineage.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_task.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1628 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14243 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/mark_tasks.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2833 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/pool.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4413 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/trigger_dag.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3303 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/config_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5383 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/connection_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8558 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_run_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2044 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_source_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5487 2022-07-05 00:33:48.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dagsetup_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2517 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/event_log_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/extra_link_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1732 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/health_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2618 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/import_error_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3649 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/log_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1560 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/plugin_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5506 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/pool_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/provider_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6330 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/role_and_permission_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2401 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11479 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_instance_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2509 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/user_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4008 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/variable_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1363 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/version_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3848 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/xcom_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5017 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/exceptions.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/openapi/
--rw-r--r--   0 johnyan    (501) staff       (20)   107667 2022-07-05 06:13:09.000000 smartpip2-2.1.9.4/airflow/api_connexion/openapi/v1.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     3655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/parameters.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/common_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/config_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1995 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/connection_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_run_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)      971 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_source_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1349 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/enum_schemas.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1738 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/error_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/event_log_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/health_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/log_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1754 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/plugin_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2370 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/pool_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1452 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/provider_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2531 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/role_and_permission_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1327 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/sla_miss_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6966 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_instance_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2992 2021-08-06 13:05:03.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2331 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/user_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/variable_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/version_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1769 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/xcom_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/security.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/cli/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    59796 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/cli_parser.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/cli/commands/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6551 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/celery_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2366 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/cheat_sheet_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/config_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/connection_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13203 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/dag_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3345 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/db_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/info_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/jobs_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1740 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/kerberos_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/kubernetes_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1999 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/legacy_commands.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/plugins_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/pool_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3862 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/provider_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1582 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/role_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1379 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/rotate_fernet_key_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/scheduler_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/sync_perm_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/task_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8359 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/user_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3968 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/variable_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)      929 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/version_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    20747 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/webserver_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5290 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/simple_table.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/common/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2022-07-03 02:40:42.000000 smartpip2-2.1.9.4/airflow/common/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9162 2022-07-03 03:12:30.000000 smartpip2-2.1.9.4/airflow/common/datax.py
--rw-r--r--   0 johnyan    (501) staff       (20)    58815 2023-04-26 09:55:02.000000 smartpip2-2.1.9.4/airflow/common/smartpip.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/compat/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/compat/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/compat/functools.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/config_templates/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11726 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/airflow_local_settings.py
--rw-r--r--   0 johnyan    (501) staff       (20)    75766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/config.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1629 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/config.yml.schema.json
--rw-r--r--   0 johnyan    (501) staff       (20)    44296 2022-08-26 06:07:49.000000 smartpip2-2.1.9.4/airflow/config_templates/default_airflow.cfg
--rw-r--r--   0 johnyan    (501) staff       (20)     4094 2022-08-01 06:06:39.000000 smartpip2-2.1.9.4/airflow/config_templates/default_celery.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2028 2022-07-03 06:20:29.000000 smartpip2-2.1.9.4/airflow/config_templates/default_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3770 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/default_test.cfg
--rw-r--r--   0 johnyan    (501) staff       (20)     4700 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/default_webserver_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)    44793 2022-07-22 10:03:34.000000 smartpip2-2.1.9.4/airflow/configuration.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/
--rw-r--r--   0 johnyan    (501) staff       (20)      821 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/
--rw-r--r--   0 johnyan    (501) staff       (20)       86 2020-10-10 01:23:08.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7650 2023-04-26 08:41:20.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/config_dagfile.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2586 2021-11-22 09:21:52.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/dagfile_test.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17582 2023-04-26 07:37:37.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/gen_airflow_dagfile.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/
--rw-r--r--   0 johnyan    (501) staff       (20)     1053 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_athena_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_datasync_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_dynamodb_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_firehose_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_glue_catalog_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1597 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_lambda_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_logs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1114 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sns_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sqs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_instance_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1220 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_registry_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_volume_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1162 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_cosmos_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_data_lake_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_fileshare_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/bigquery_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/cassandra_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/cloudant_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1395 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/databricks_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/datadog_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/datastore_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/dingding_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/discord_webhook_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/emr_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/fs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1099 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/ftp_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1625 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_api_base_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_bigtable_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_cloud_build_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_compute_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_container_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataflow_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1593 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataproc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dlp_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_function_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1543 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_kms_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_mlengine_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_natural_language_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_pubsub_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1424 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_spanner_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_speech_to_text_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_sql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_tasks_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_text_to_speech_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1804 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_transfer_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_translate_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_video_intelligence_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_vision_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1130 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gdrive_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/grpc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/imap_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/jenkins_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/jira_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/mongo_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/openfaas_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/opsgenie_alert_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/pagerduty_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/pinot_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_check_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/redis_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/redshift_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/sagemaker_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/salesforce_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/segment_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/sftp_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/slack_webhook_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/snowflake_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1143 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/spark_jdbc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1139 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/spark_sql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1151 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/spark_submit_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/sqoop_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1089 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/ssh_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/vertica_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/wasb_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/winrm_hook.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/operators/
--rw-r--r--   0 johnyan    (501) staff       (20)      890 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/adls_list_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/adls_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/aws_athena_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/aws_sqs_publish_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2504 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/awsbatch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1239 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/azure_container_instances_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/azure_cosmos_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_get_data.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_table_delete_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_bigquery.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1701 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_mysql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/cassandra_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1202 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/databricks_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2883 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dataflow_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8275 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dataproc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1737 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/datastore_export_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1736 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/datastore_import_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dingding_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/discord_webhook_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/docker_swarm_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/druid_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dynamodb_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/ecs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/emr_add_steps_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/emr_create_job_flow_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/emr_terminate_job_flow_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1728 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/file_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/file_to_wasb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4792 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_bigtable_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_cloud_build_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4827 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_compute_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_container_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4405 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_dlp_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2348 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_function_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3958 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_natural_language_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3976 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_spanner_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1808 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_speech_to_text_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5195 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_sql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1566 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_tasks_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_text_to_speech_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_transfer_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1757 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_speech_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1337 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_video_intelligence_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7931 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_vision_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2296 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_acl_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_delete_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_download_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1645 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_list_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1657 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1695 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_bq.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1672 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gdrive_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1636 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/grpc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/hive_to_dynamodb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/imap_attachment_to_s3_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/jenkins_job_trigger_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/jira_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/kubernetes_pod_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3494 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mlengine_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mongo_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mssql_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mysql_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1163 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/opsgenie_alert_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_oracle_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1707 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/postgres_to_gcs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3949 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/pubsub_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1188 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/qubole_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/qubole_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/redis_publish_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_copy_object_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1182 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_delete_objects_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_list_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1264 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_transfer_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_sftp_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_base_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_config_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_model_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1185 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_training_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1189 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_transform_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_tuning_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/segment_track_event_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sftp_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sftp_to_s3_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/slack_webhook_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/snowflake_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sns_publish_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/spark_jdbc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/spark_sql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/spark_submit_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sql_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sqoop_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/ssh_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/vertica_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1702 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_hive.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1193 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/wasb_delete_blob_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/winrm_operator.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/
--rw-r--r--   0 johnyan    (501) staff       (20)      884 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/aws_secrets_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/aws_systems_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/azure_key_vault.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1699 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/gcp_secrets_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/hashicorp_vault.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/
--rw-r--r--   0 johnyan    (501) staff       (20)     1059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_athena_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_redshift_cluster_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_sqs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/azure_cosmos_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/bash_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/bigquery_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1158 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_record_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_table_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/celery_queue_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/datadog_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/emr_base_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/emr_job_flow_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/emr_step_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1068 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/file_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1109 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/ftp_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/gcp_transfer_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/gcs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/hdfs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/imap_attachment_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1123 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/jira_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/mongo_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/pubsub_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/python_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/qubole_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/redis_key_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/redis_pub_sub_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_base_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_endpoint_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1205 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_training_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_transform_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_tuning_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sftp_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/wasb_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/weekday_sensor.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/task_runner/
--rw-r--r--   0 johnyan    (501) staff       (20)      860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/task_runner/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/task_runner/cgroup_task_runner.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)      973 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1206 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_sanitizer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_validator.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/utils/log/
--rw-r--r--   0 johnyan    (501) staff       (20)      979 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/log/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/log/task_handler_with_custom_formatter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_operator_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_prediction_summary.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1369 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/sendgrid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)      735 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/customized_form_field_behaviours.schema.json
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/decorators/
--rw-r--r--   0 johnyan    (501) staff       (20)     7051 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8901 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3297 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/python.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3658 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/python_virtualenv.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/task_group.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/example_dags/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2357 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_bash_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2828 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_datetime_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1767 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_day_of_week_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_labels.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2040 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2121 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_python_dop_operator_3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7964 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_complex.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2336 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_dag_decorator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_external_task_marker_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3398 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6683 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1313 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_latest_only.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1632 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_latest_only_with_trigger.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_nested_branch_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2943 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_passing_params_via_test_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3122 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_python_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1705 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_short_circuit_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2211 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_skip_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_subdag_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2329 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_task_group.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1988 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_task_group_decorator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1631 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_trigger_controller_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_trigger_target_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2662 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_xcom.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2118 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_xcomargs.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/example_dags/libs/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/libs/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)      832 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/libs/helper.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/example_dags/subdags/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/subdags/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1733 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/subdags/subdag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/test_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4311 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial_etl_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3302 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3481 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6925 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/exceptions.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/executors/
--rw-r--r--   0 johnyan    (501) staff       (20)      802 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11695 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/base_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    25085 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/celery_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/celery_kubernetes_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4430 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/dask_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5674 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/debug_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/executor_constants.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4985 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/executor_loader.py
--rw-r--r--   0 johnyan    (501) staff       (20)    32831 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/kubernetes_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13912 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/local_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/sequential_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2022-10-24 03:38:18.000000 smartpip2-2.1.9.4/airflow/git_version
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/hooks/
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/S3_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)      800 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6597 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/base_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/dbapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/dbapi_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/docker_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/druid_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1527 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/filesystem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/hdfs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/hive_hooks.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/http_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1108 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/jdbc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/mssql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/mysql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/oracle_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/pig_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/postgres_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/presto_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/samba_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/slack_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/sqlite_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3589 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/subprocess.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/webhdfs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/zendesk_hook.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/jobs/
--rw-r--r--   0 johnyan    (501) staff       (20)      928 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    38099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/backfill_job.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9737 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/base_job.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/local_task_job.py
--rw-r--r--   0 johnyan    (501) staff       (20)    81963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/scheduler_job.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/kubernetes/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/k8s_model.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5528 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/kube_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/kube_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/kubernetes_helper_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1215 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod.py
--rw-r--r--   0 johnyan    (501) staff       (20)    20148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_generator.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13034 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0 johnyan    (501) staff       (20)      996 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher_deprecated.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_runtime_info_env.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4555 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/refresh_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5242 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/secret.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/volume.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/volume_mount.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/lineage/
--rw-r--r--   0 johnyan    (501) staff       (20)     6456 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/lineage/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1730 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/lineage/backend.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2197 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/lineage/entities.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4442 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/logging_config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/macros/
--rw-r--r--   0 johnyan    (501) staff       (20)     2574 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/macros/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4884 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/macros/hive.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/migrations/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/env.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/migrations/versions/
--rw-r--r--   0 johnyan    (501) staff       (20)     1739 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/05f30312d566_merge_heads.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15150 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/13eb55f81627_for_compatibility.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1726 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/211e584da130_add_ti_state_index.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16341 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1475 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2e541a1dcfed_task_duration.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2315 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1360 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3490 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/40e67319e3a9_dagrun_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1372 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/4446e08588_dagrun_start_end.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1689 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1230 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/502898887f84_adding_extra_to_log.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2605 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1257 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/52d714495f0_job_id_indices.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1952 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2512 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4511 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16875 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2634 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5447 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1323 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2958 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3222 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7211 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/92c57b58940d_add_fab_tables.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1920 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2874 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1301 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/9635ae0956e7_index_faskfail.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4170 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6567 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1278 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1600 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1839 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1204 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b0125267960b_merge_heads.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1479 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1706 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1332 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1284 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1965 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3520 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1367 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5115 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1488 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3199 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1477 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1216 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1503 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1534 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3522 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11190 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e3a246e0dc1_current_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1536 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/models/
--rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)    66313 2021-08-06 14:28:15.000000 smartpip2-2.1.9.4/airflow/models/baseoperator.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13786 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/connection.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2771 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/crypto.py
--rw-r--r--   0 johnyan    (501) staff       (20)    96020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)    27766 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagbag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagcode.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagparam.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1914 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagpickle.py
--rw-r--r--   0 johnyan    (501) staff       (20)    30854 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagrun.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/errors.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2239 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/log.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/pool.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/renderedtifields.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6417 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/sensorinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/serialized_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6652 2021-09-30 12:06:57.000000 smartpip2-2.1.9.4/airflow/models/skipmixin.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/slamiss.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/taskfail.py
--rw-r--r--   0 johnyan    (501) staff       (20)    82807 2022-08-01 13:38:00.000000 smartpip2-2.1.9.4/airflow/models/taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/taskmixin.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/taskreschedule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7485 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/variable.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9883 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/xcom.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/xcom_arg.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/mypy/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/mypy/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/mypy/plugin/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/mypy/plugin/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2866 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/mypy/plugin/decorators.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/operators/
--rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6978 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/bash.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/bash_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2120 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/branch.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1070 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/branch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2897 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/dagrun_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/datetime.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/docker_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/druid_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/dummy.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/dummy_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/email.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/email_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/gcs_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/generic_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/google_api_to_s3_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1166 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_stats_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_to_druid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1663 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_to_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_to_samba_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1118 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/http_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/jdbc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2696 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/latest_only.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/latest_only_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mssql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1668 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mssql_to_hive.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mysql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mysql_to_hive.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/oracle_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/papermill_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/pig_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/postgres_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/presto_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1658 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/presto_to_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18378 2021-08-07 01:46:07.000000 smartpip2-2.1.9.4/airflow/operators/python.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/python_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1680 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/redshift_to_s3_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/s3_file_transform_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1622 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/s3_to_hive_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/s3_to_redshift_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/slack_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)    20630 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/sql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1476 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/sql_branch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/sqlite_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8631 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/subdag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1098 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/subdag_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6935 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/trigger_dagrun.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14314 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/plugins_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)      882 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/provider_info.schema.json
--rw-r--r--   0 johnyan    (501) staff       (20)    17989 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/providers_manager.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/secrets/
--rw-r--r--   0 johnyan    (501) staff       (20)     1267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3321 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/base_secrets.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1601 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/environment_variables.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12137 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/local_filesystem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/metastore.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/security/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/kerberos.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2582 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/permissions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2880 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/utils.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/sensors/
--rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/base_sensor_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3334 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/bash.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2851 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/date_time.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/date_time_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13029 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/external_task.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2380 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/filesystem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/hdfs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/hive_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/http_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/metastore_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/named_hive_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2864 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/python.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/s3_key_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/s3_prefix_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    30370 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/smart_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4769 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/sql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/sql_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/time_delta.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/time_delta_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1406 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/time_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/web_hdfs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/sentry.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/serialization/
--rw-r--r--   0 johnyan    (501) staff       (20)      813 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/enums.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/helpers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2313 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/json_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8061 2021-08-06 13:03:21.000000 smartpip2-2.1.9.4/airflow/serialization/schema.json
--rw-r--r--   0 johnyan    (501) staff       (20)    35709 2021-08-06 14:28:15.000000 smartpip2-2.1.9.4/airflow/serialization/serialized_objects.py
--rw-r--r--   0 johnyan    (501) staff       (20)    19657 2022-07-03 03:38:58.000000 smartpip2-2.1.9.4/airflow/settings.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/smart_sensor_dags/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/smart_sensor_dags/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2086 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/smart_sensor_dags/smart_sensor_group.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13906 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/stats.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/task/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/task/task_runner/
--rw-r--r--   0 johnyan    (501) staff       (20)     2443 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/base_task_runner.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/cgroup_task_runner.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4618 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/standard_task_runner.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/templates.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/ti_deps/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4779 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/dep_context.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/dependencies_deps.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1504 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/dependencies_states.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/
--rw-r--r--   0 johnyan    (501) staff       (20)      844 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5905 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/base_ti_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1449 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_ti_slots_available_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_unpaused_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2245 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_exists_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_id_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/exec_date_after_start_date_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2132 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/not_in_retry_period_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3232 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/not_previously_skipped_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2871 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/pool_slots_available_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/prev_dagrun_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/ready_to_reschedule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2275 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/runnable_exec_date_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1639 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/task_concurrency_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/task_not_running_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/trigger_rule_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/valid_state_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/typing_compat.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3672 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/callback_requests.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/cli.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3847 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/cli_action_loggers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/code_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1579 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/compression.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1409 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/configuration.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2413 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/dag_cycle_tester.py
--rw-r--r--   0 johnyan    (501) staff       (20)    49403 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/dag_processing.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10420 2021-08-09 11:44:27.000000 smartpip2-2.1.9.4/airflow/utils/dates.py
--rw-r--r--   0 johnyan    (501) staff       (20)    21208 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/db.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1859 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/decorators.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1312 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/docs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6061 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/dot_renderer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/edgemodifier.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12238 2022-07-03 05:03:18.000000 smartpip2-2.1.9.4/airflow/utils/email.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1521 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/entry_points.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1489 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/event_scheduler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8221 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/file.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7066 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/helpers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2457 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/json.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/utils/log/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/cloudwatch_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/colored_log.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/es_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/file_processor_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11716 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/file_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/gcs_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/json_formatter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/log_reader.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/logging_mixin.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/s3_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8849 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/secrets_masker.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/stackdriver_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2178 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/task_handler_with_custom_formatter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/wasb_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/mixins.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1414 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/module_loading.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/net.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/operator_helpers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/operator_resources.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/orm_event_handlers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2704 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/platform.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/process_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/python_virtualenv.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1892 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/python_virtualenv_script.jinja2
--rw-r--r--   0 johnyan    (501) staff       (20)     3817 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/retries.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2975 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/serve_logs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2420 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/session.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9571 2021-08-09 11:25:35.000000 smartpip2-2.1.9.4/airflow/utils/sqlalchemy.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/state.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/strings.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15018 2021-08-06 13:06:23.000000 smartpip2-2.1.9.4/airflow/utils/task_group.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/timeout.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5244 2021-08-09 11:25:54.000000 smartpip2-2.1.9.4/airflow/utils/timezone.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/trigger_rule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/types.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1640 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/weight_rule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2412 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/yaml.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1196 2022-10-13 03:18:37.000000 smartpip2-2.1.9.4/airflow/version.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/
--rw-r--r--   0 johnyan    (501) staff       (20)       87 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.eslintignore
--rw-r--r--   0 johnyan    (501) staff       (20)       84 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.eslintrc
--rw-r--r--   0 johnyan    (501) staff       (20)       26 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.stylelintignore
--rw-r--r--   0 johnyan    (501) staff       (20)       45 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.stylelintrc
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/api/
--rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/api/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/api/experimental/
--rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/api/experimental/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15690 2021-08-05 08:41:16.000000 smartpip2-2.1.9.4/airflow/www/api/experimental/endpoints.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5616 2021-08-09 08:25:04.000000 smartpip2-2.1.9.4/airflow/www/app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4186 2021-08-06 17:29:43.000000 smartpip2-2.1.9.4/airflow/www/auth.py
--rw-r--r--   0 johnyan    (501) staff       (20)      984 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/blueprints.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3152 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/decorators.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/extensions/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-09-15 03:14:39.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder_links.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_dagbag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_jinja_globals.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2102 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_manifest_files.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2041 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_security.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1683 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_session.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8001 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_views.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_wsgi_middlewares.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8227 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/forms.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/gunicorn_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2755 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    30652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/security.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/static/
--rw-r--r--   0 johnyan    (501) staff       (20)   622963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/airflow.gif
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/static/css/
--rw-r--r--   0 johnyan    (501) staff       (20)   127184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/bootstrap-theme.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1209 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/calendar.css
--rw-r--r--   0 johnyan    (501) staff       (20)     3047 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/dags.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1392 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/flash.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1325 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/gantt.css
--rw-r--r--   0 johnyan    (501) staff       (20)     3240 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/graph.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1385 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/loading-dots.css
--rw-r--r--   0 johnyan    (501) staff       (20)     9964 2022-10-13 06:28:22.000000 smartpip2-2.1.9.4/airflow/www/static/css/main.css
--rw-r--r--   0 johnyan    (501) staff       (20)   112025 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/material-icons.css
--rw-r--r--   0 johnyan    (501) staff       (20)     2416 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/switch.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/tree.css
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/static/dist/
--rw-r--r--   0 johnyan    (501) staff       (20)   104074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js
--rw-r--r--   0 johnyan    (501) staff       (20)     7718 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.css
--rw-r--r--   0 johnyan    (501) staff       (20)    37970 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)    10289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap3-typeahead.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1087 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css
--rw-r--r--   0 johnyan    (501) staff       (20)    15940 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js
--rw-r--r--   0 johnyan    (501) staff       (20)   346026 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/circles.995e0afd45c3641109e1.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5931 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.css
--rw-r--r--   0 johnyan    (501) staff       (20)   398753 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1466 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/coffeescript-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8981 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1310 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/css-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)    29780 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/d3-shape.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)     9207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/d3-tip.js
--rw-r--r--   0 johnyan    (501) staff       (20)   151725 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/d3.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)    14075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js
--rw-r--r--   0 johnyan    (501) staff       (20)     6495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js
--rw-r--r--   0 johnyan    (501) staff       (20)     9796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js
--rw-r--r--   0 johnyan    (501) staff       (20)    28194 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)    26948 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)   725181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)   668783 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)     2612 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css
--rw-r--r--   0 johnyan    (501) staff       (20)    16899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js
--rw-r--r--   0 johnyan    (501) staff       (20)     4226 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5203 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css
--rw-r--r--   0 johnyan    (501) staff       (20)    40502 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css
--rw-r--r--   0 johnyan    (501) staff       (20)    53822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1989 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/html-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)    16827 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/ie.e458fc4544c628f16e02.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2159 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/javascript-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)    38837 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/javascript.js
--rw-r--r--   0 johnyan    (501) staff       (20)    83565 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/jquery.dataTables.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)  1283507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/jshint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1333 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/json-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/lint.css
--rw-r--r--   0 johnyan    (501) staff       (20)     9125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4229 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js
--rw-r--r--   0 johnyan    (501) staff       (20)     7313 2022-10-13 06:28:22.000000 smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.css
--rw-r--r--   0 johnyan    (501) staff       (20)    15979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.js
--rw-r--r--   0 johnyan    (501) staff       (20)     3327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/manifest.json
--rw-r--r--   0 johnyan    (501) staff       (20)   111620 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js
--rw-r--r--   0 johnyan    (501) staff       (20)   385945 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/moment.c1933ee062e9650051f7.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8329 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css
--rw-r--r--   0 johnyan    (501) staff       (20)     3677 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css.map
--rw-r--r--   0 johnyan    (501) staff       (20)   253352 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)  1954533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)   993008 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2816 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0 johnyan    (501) staff       (20)  3389627 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/sum.md5
--rw-r--r--   0 johnyan    (501) staff       (20)     2091 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.js
--rw-r--r--   0 johnyan    (501) staff       (20)     9898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js
--rw-r--r--   0 johnyan    (501) staff       (20)    31314 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js
--rw-r--r--   0 johnyan    (501) staff       (20)    23111 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.css
--rw-r--r--   0 johnyan    (501) staff       (20)    46722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5116 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5055 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1255 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/yaml-lint.js
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/static/js/
--rw-r--r--   0 johnyan    (501) staff       (20)    11183 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/calendar.js
--rw-r--r--   0 johnyan    (501) staff       (20)     3436 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/circles.js
--rw-r--r--   0 johnyan    (501) staff       (20)     4994 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/connection_form.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8057 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dag.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1010 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dag_code.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5997 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dag_dependencies.js
--rw-r--r--   0 johnyan    (501) staff       (20)    11004 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dags.js
--rw-r--r--   0 johnyan    (501) staff       (20)     3593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/datetime_utils.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/duration_chart.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8882 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/gantt.js
--rw-r--r--   0 johnyan    (501) staff       (20)    21515 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/graph.js
--rw-r--r--   0 johnyan    (501) staff       (20)      887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/ie.js
--rw-r--r--   0 johnyan    (501) staff       (20)     6355 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/main.js
--rw-r--r--   0 johnyan    (501) staff       (20)      995 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/meta_value.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1107 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/task_instance.js
--rw-r--r--   0 johnyan    (501) staff       (20)     4274 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/task_instances.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5599 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/ti_log.js
--rw-r--r--   0 johnyan    (501) staff       (20)    15167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/tree.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/trigger.js
--rw-r--r--   0 johnyan    (501) staff       (20)      957 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/variable_edit.js
--rw-r--r--   0 johnyan    (501) staff       (20)    16671 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/loading.gif
--rw-r--r--   0 johnyan    (501) staff       (20)     3184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin.svg
--rw-r--r--   0 johnyan    (501) staff       (20)     7501 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_100.png
--rw-r--r--   0 johnyan    (501) staff       (20)     1547 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_25.png
--rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_32.png
--rw-r--r--   0 johnyan    (501) staff       (20)     2306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_35.png
--rw-r--r--   0 johnyan    (501) staff       (20)     2685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_40.png
--rw-r--r--   0 johnyan    (501) staff       (20)    24922 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_large.png
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/
--rw-r--r--   0 johnyan    (501) staff       (20)    31140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/gantt.png
--rw-r--r--   0 johnyan    (501) staff       (20)    38282 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/graph.png
--rw-r--r--   0 johnyan    (501) staff       (20)    35259 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/tree.png
--rw-r--r--   0 johnyan    (501) staff       (20)      160 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/sort_asc.png
--rw-r--r--   0 johnyan    (501) staff       (20)      201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/sort_both.png
--rw-r--r--   0 johnyan    (501) staff       (20)      158 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/sort_desc.png
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/templates/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/
--rw-r--r--   0 johnyan    (501) staff       (20)     1877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/calendar.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2581 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/chart.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1345 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/circles.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/code.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1894 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/config.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/confirm.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1038 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_create.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1049 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_edit.html
--rw-r--r--   0 johnyan    (501) staff       (20)    21916 2021-09-21 03:40:31.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_code.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_dependencies.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3424 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_details.html
--rw-r--r--   0 johnyan    (501) staff       (20)    16490 2021-09-21 04:00:33.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dags.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2900 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/duration_chart.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/gantt.html
--rw-r--r--   0 johnyan    (501) staff       (20)     5609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/graph.html
--rw-r--r--   0 johnyan    (501) staff       (20)     4035 2021-08-09 08:31:54.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/main.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3173 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/model_list.html
--rw-r--r--   0 johnyan    (501) staff       (20)      950 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/noaccess.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/plugin.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/redoc.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2213 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/task.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/task_instance.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1044 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_code.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2929 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_log.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1431 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/traceback.html
--rw-r--r--   0 johnyan    (501) staff       (20)     4480 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/tree.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/trigger.html
--rw-r--r--   0 johnyan    (501) staff       (20)      999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_edit.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_list.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1231 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/xcom.html
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/
--rw-r--r--   0 johnyan    (501) staff       (20)     1195 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/google_analytics.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1807 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/metarouter.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1810 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/segment.html
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/
--rw-r--r--   0 johnyan    (501) staff       (20)     4446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/custom_icons.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/dag_docs.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3000 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/flash.html
--rw-r--r--   0 johnyan    (501) staff       (20)      809 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/index.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/loading_dots.html
--rw-r--r--   0 johnyan    (501) staff       (20)     4388 2022-10-13 06:34:20.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2001 2022-10-13 08:38:39.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_menu.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3486 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_right.html
--rw-r--r--   0 johnyan    (501) staff       (20)    16328 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2615 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/validators.py
--rw-r--r--   0 johnyan    (501) staff       (20)   149695 2021-11-22 06:20:23.000000 smartpip2-2.1.9.4/airflow/www/views.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6792 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/webpack.config.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2549 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/widgets.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/licenses/
--rw-rw-r--   0 johnyan    (501) staff       (20)     1131 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-bootstrap.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)      984 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-bootstrap3-typeahead.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)      556 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-connexion.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-d3-shape.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1079 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-d3-tip.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-d3js.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1062 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-dagre-d3.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1076 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-datatables.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1081 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-elasticmock.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1301 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-flask-kerberos.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)    11349 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-hue.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)    11357 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-jqclock.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1605 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-jquery.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1077 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-moment-strftime.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1075 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-moment.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-normalize.txt
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/scripts/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/scripts/systemd/
--rw-rw-r--   0 johnyan    (501) staff       (20)      678 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/README
--rw-rw-r--   0 johnyan    (501) staff       (20)      968 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow
--rw-rw-r--   0 johnyan    (501) staff       (20)     1195 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-flower.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1200 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-kerberos.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1190 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-scheduler.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1243 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-webserver.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1203 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-worker.service
--rw-rw-r--   0 johnyan    (501) staff       (20)      824 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow.conf
--rw-rw-r--   0 johnyan    (501) staff       (20)     4042 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/setup.cfg
--rw-rw-r--   0 johnyan    (501) staff       (20)    33517 2023-04-26 09:55:02.000000 smartpip2-2.1.9.4/setup.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/smartpip2.egg-info/
--rw-r--r--   0 johnyan    (501) staff       (20)    26641 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)    44222 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/SOURCES.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/dependency_links.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/entry_points.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2021-08-07 01:38:26.000000 smartpip2-2.1.9.4/smartpip2.egg-info/not-zip-safe
--rw-r--r--   0 johnyan    (501) staff       (20)    29803 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/requires.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        8 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/top_level.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/
+-rw-rw-r--   0 johnyan    (501) staff       (20)   274732 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/CHANGELOG.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)    13444 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/LICENSE
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1433 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/MANIFEST.in
+-rw-rw-r--   0 johnyan    (501) staff       (20)      404 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/NOTICE
+-rw-r--r--   0 johnyan    (501) staff       (20)    26641 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/PKG-INFO
+-rw-rw-r--   0 johnyan    (501) staff       (20)    20139 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/README.md
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/airflow/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2751 2022-07-19 14:54:13.000000 smartpip2-2.1.9.5/airflow/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1368 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/__main__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/airflow/_vendor/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1430 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)       95 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/__main__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/
+-rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18192 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/abstract.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14270 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/aiohttp_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12812 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/flask_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2222 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/flask_utils.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/
+-rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10764 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/abstract.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/aiohttp_app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5023 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/flask_app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/cli.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1842 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/coroutine_wrappers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1441 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/decorator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1752 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/metrics.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/parameter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/produces.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/response.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9853 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/security.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11690 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/uri_parsing.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15533 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/validation.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/exceptions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2692 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/handlers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/http_facts.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4050 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/json_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/jsonifier.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/lifecycle.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/mock.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/
+-rw-r--r--   0 johnyan    (501) staff       (20)      294 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15461 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/abstract.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      127 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/compat.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14505 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/openapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6782 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/secure.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/swagger2.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4444 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/options.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1926 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/problem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6810 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/resolver.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3408 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/setup.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/spec.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6515 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/_vendor/connexion/utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2320 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/alembic.ini
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1550 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api/auth/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/auth/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api/auth/backend/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/auth/backend/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2258 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/auth/backend/basic_auth.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1342 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/auth/backend/default.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/auth/backend/deny_all.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5563 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/auth/backend/kerberos_auth.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1500 2022-07-04 11:00:25.000000 smartpip2-2.1.9.5/airflow/api/auth/backend/smart_auth.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api/client/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/client/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2465 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/client/api_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/client/json_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2223 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/client/local_client.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api/common/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2045 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/delete_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      329 2020-10-10 01:23:08.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/gen_dag_file.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1426 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/get_code.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1381 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/get_dag_run_state.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1982 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/get_dag_runs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1886 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/get_lineage.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/get_task.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1628 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/get_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14243 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/mark_tasks.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2833 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/pool.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4413 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api/common/experimental/trigger_dag.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api_connexion/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3303 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/config_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5383 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/connection_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dag_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8558 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dag_run_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2044 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dag_source_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5487 2022-07-05 00:33:48.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dagsetup_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2517 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/event_log_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/extra_link_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1732 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/health_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2618 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/import_error_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3649 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/log_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1560 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/plugin_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5506 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/pool_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/provider_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6330 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/role_and_permission_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2401 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/task_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11479 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/task_instance_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2509 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/user_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4008 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/variable_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1363 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/version_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3848 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/endpoints/xcom_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5017 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/exceptions.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api_connexion/openapi/
+-rw-r--r--   0 johnyan    (501) staff       (20)   107667 2022-07-05 06:13:09.000000 smartpip2-2.1.9.5/airflow/api_connexion/openapi/v1.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     3655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/parameters.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/common_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/config_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1995 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/connection_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/dag_run_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/dag_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      971 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/dag_source_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1349 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/enum_schemas.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1738 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/error_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/event_log_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/health_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/log_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1754 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/plugin_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2370 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/pool_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1452 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/provider_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2531 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/role_and_permission_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1327 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/sla_miss_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6966 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/task_instance_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2992 2021-08-06 13:05:03.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/task_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2331 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/user_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/variable_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/version_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1769 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/schemas/xcom_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/api_connexion/security.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/cli/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    59796 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/cli_parser.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/cli/commands/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6551 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/celery_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2366 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/cheat_sheet_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/config_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/connection_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13203 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/dag_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3345 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/db_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/info_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/jobs_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1740 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/kerberos_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/kubernetes_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1999 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/legacy_commands.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/plugins_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/pool_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3862 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/provider_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1582 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/role_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1379 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/rotate_fernet_key_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/scheduler_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/sync_perm_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/task_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8359 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/user_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3968 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/variable_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      929 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/version_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    20747 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/commands/webserver_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5290 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/cli/simple_table.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/common/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2022-07-03 02:40:42.000000 smartpip2-2.1.9.5/airflow/common/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9162 2022-07-03 03:12:30.000000 smartpip2-2.1.9.5/airflow/common/datax.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    59006 2023-05-10 02:34:43.000000 smartpip2-2.1.9.5/airflow/common/smartpip.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/compat/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/compat/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/compat/functools.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/config_templates/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/config_templates/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11726 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/config_templates/airflow_local_settings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    75766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/config_templates/config.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1629 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/config_templates/config.yml.schema.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    44296 2022-08-26 06:07:49.000000 smartpip2-2.1.9.5/airflow/config_templates/default_airflow.cfg
+-rw-r--r--   0 johnyan    (501) staff       (20)     4094 2022-08-01 06:06:39.000000 smartpip2-2.1.9.5/airflow/config_templates/default_celery.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2028 2022-07-03 06:20:29.000000 smartpip2-2.1.9.5/airflow/config_templates/default_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3770 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/config_templates/default_test.cfg
+-rw-r--r--   0 johnyan    (501) staff       (20)     4700 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/config_templates/default_webserver_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    44793 2022-07-22 10:03:34.000000 smartpip2-2.1.9.5/airflow/configuration.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/
+-rw-r--r--   0 johnyan    (501) staff       (20)      821 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/dagsetup/
+-rw-r--r--   0 johnyan    (501) staff       (20)       86 2020-10-10 01:23:08.000000 smartpip2-2.1.9.5/airflow/contrib/dagsetup/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7650 2023-04-26 08:41:20.000000 smartpip2-2.1.9.5/airflow/contrib/dagsetup/config_dagfile.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2586 2021-11-22 09:21:52.000000 smartpip2-2.1.9.5/airflow/contrib/dagsetup/dagfile_test.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17582 2023-04-26 07:37:37.000000 smartpip2-2.1.9.5/airflow/contrib/dagsetup/gen_airflow_dagfile.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1053 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_athena_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_datasync_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_dynamodb_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_firehose_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_glue_catalog_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1597 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_lambda_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_logs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1114 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_sns_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/aws_sqs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/azure_container_instance_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1220 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/azure_container_registry_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/azure_container_volume_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1162 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/azure_cosmos_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/azure_data_lake_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/azure_fileshare_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/bigquery_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/cassandra_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/cloudant_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1395 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/databricks_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/datadog_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/datastore_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/dingding_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/discord_webhook_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/emr_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/fs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1099 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/ftp_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1625 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_api_base_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_bigtable_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_cloud_build_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_compute_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_container_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_dataflow_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1593 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_dataproc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_dlp_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_function_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1543 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_kms_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_mlengine_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_natural_language_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_pubsub_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1424 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_spanner_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_speech_to_text_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_sql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_tasks_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_text_to_speech_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1804 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_transfer_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_translate_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_video_intelligence_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_vision_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gcs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1130 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/gdrive_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/grpc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/imap_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/jenkins_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/jira_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/mongo_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/openfaas_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/opsgenie_alert_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/pagerduty_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/pinot_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/qubole_check_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/qubole_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/redis_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/redshift_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/sagemaker_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/salesforce_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/segment_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/sftp_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/slack_webhook_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/snowflake_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1143 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/spark_jdbc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1139 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/spark_sql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1151 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/spark_submit_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/sqoop_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1089 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/ssh_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/vertica_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/wasb_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/hooks/winrm_hook.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/operators/
+-rw-r--r--   0 johnyan    (501) staff       (20)      890 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/adls_list_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/adls_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/aws_athena_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/aws_sqs_publish_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2504 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/awsbatch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1239 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/azure_container_instances_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/azure_cosmos_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_get_data.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_table_delete_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_to_bigquery.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1701 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_to_mysql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/cassandra_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1202 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/databricks_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2883 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/dataflow_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8275 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/dataproc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1737 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/datastore_export_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1736 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/datastore_import_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/dingding_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/discord_webhook_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/docker_swarm_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/druid_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/dynamodb_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/ecs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/emr_add_steps_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/emr_create_job_flow_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/emr_terminate_job_flow_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1728 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/file_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/file_to_wasb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4792 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_bigtable_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_cloud_build_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4827 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_compute_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_container_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4405 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_dlp_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2348 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_function_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3958 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_natural_language_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3976 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_spanner_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1808 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_speech_to_text_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5195 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_sql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1566 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_tasks_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_text_to_speech_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_transfer_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_translate_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1757 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_translate_speech_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1337 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_video_intelligence_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7931 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcp_vision_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2296 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_acl_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_delete_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_download_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1645 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_list_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1657 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1695 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_bq.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1672 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_gdrive_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1636 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/grpc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/hive_to_dynamodb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/imap_attachment_to_s3_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/jenkins_job_trigger_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/jira_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/kubernetes_pod_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3494 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/mlengine_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/mongo_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/mssql_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/mysql_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1163 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/opsgenie_alert_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/oracle_to_oracle_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1707 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/postgres_to_gcs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3949 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/pubsub_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1188 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/qubole_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/qubole_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/redis_publish_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/s3_copy_object_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1182 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/s3_delete_objects_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/s3_list_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/s3_to_gcs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1264 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/s3_to_gcs_transfer_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/s3_to_sftp_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_base_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_endpoint_config_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_endpoint_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_model_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1185 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_training_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1189 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_transform_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_tuning_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/segment_track_event_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sftp_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sftp_to_s3_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/slack_webhook_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/snowflake_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sns_publish_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/spark_jdbc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/spark_sql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/spark_submit_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sql_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/sqoop_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/ssh_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/vertica_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1702 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/vertica_to_hive.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/vertica_to_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1193 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/wasb_delete_blob_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/operators/winrm_operator.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/secrets/
+-rw-r--r--   0 johnyan    (501) staff       (20)      884 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/secrets/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/secrets/aws_secrets_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/secrets/aws_systems_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/secrets/azure_key_vault.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1699 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/secrets/gcp_secrets_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/secrets/hashicorp_vault.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/aws_athena_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/aws_redshift_cluster_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/aws_sqs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/azure_cosmos_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/bash_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/bigquery_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1158 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/cassandra_record_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/cassandra_table_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/celery_queue_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/datadog_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/emr_base_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/emr_job_flow_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/emr_step_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1068 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/file_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1109 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/ftp_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/gcp_transfer_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/gcs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/hdfs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/imap_attachment_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1123 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/jira_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/mongo_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/pubsub_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/python_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/qubole_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/redis_key_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/redis_pub_sub_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_base_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_endpoint_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1205 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_training_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_transform_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_tuning_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/sftp_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/wasb_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/sensors/weekday_sensor.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/task_runner/
+-rw-r--r--   0 johnyan    (501) staff       (20)      860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/task_runner/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/task_runner/cgroup_task_runner.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)      973 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1206 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/gcp_field_sanitizer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/gcp_field_validator.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/contrib/utils/log/
+-rw-r--r--   0 johnyan    (501) staff       (20)      979 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/log/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/log/task_handler_with_custom_formatter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/mlengine_operator_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/mlengine_prediction_summary.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1369 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/sendgrid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/contrib/utils/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      735 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/customized_form_field_behaviours.schema.json
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/decorators/
+-rw-r--r--   0 johnyan    (501) staff       (20)     7051 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/decorators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8901 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/decorators/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3297 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/decorators/python.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3658 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/decorators/python_virtualenv.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/decorators/task_group.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/example_dags/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2357 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_bash_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2828 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_branch_datetime_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1767 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_branch_day_of_week_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_branch_labels.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2040 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_branch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2121 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_branch_python_dop_operator_3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7964 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_complex.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2336 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_dag_decorator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_external_task_marker_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3398 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_kubernetes_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6683 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_kubernetes_executor_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1313 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_latest_only.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1632 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_latest_only_with_trigger.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_nested_branch_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2943 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_passing_params_via_test_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3122 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_python_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1705 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_short_circuit_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2211 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_skip_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_subdag_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2329 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_task_group.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1988 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_task_group_decorator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1631 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_trigger_controller_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_trigger_target_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2662 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_xcom.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2118 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/example_dags/example_xcomargs.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/example_dags/libs/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/libs/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      832 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/libs/helper.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/example_dags/subdags/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/subdags/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1733 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/subdags/subdag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/test_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/tutorial.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4311 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/tutorial_etl_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3302 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/tutorial_taskflow_api_etl.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3481 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6984 2023-05-09 09:43:06.000000 smartpip2-2.1.9.5/airflow/exceptions.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/executors/
+-rw-r--r--   0 johnyan    (501) staff       (20)      802 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11695 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/base_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    25085 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/celery_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/celery_kubernetes_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4430 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/dask_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5674 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/debug_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/executor_constants.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4985 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/executor_loader.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    32831 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/kubernetes_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13912 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/local_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/executors/sequential_executor.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/hooks/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/S3_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      800 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6597 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/base_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/dbapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/dbapi_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/docker_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/druid_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1527 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/filesystem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/hdfs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/hive_hooks.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/http_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1108 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/jdbc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/mssql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/mysql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/oracle_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/pig_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/postgres_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/presto_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/samba_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/slack_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/sqlite_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3589 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/subprocess.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/webhdfs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/hooks/zendesk_hook.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/jobs/
+-rw-r--r--   0 johnyan    (501) staff       (20)      928 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/jobs/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    38099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/jobs/backfill_job.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9737 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/jobs/base_job.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/jobs/local_task_job.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    81963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/jobs/scheduler_job.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/kubernetes/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/k8s_model.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5528 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/kube_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/kube_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/kubernetes_helper_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1215 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/pod.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    20148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/pod_generator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13034 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      996 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/pod_launcher.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/pod_launcher_deprecated.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/pod_runtime_info_env.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4555 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/refresh_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5242 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/secret.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/volume.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/kubernetes/volume_mount.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/lineage/
+-rw-r--r--   0 johnyan    (501) staff       (20)     6456 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/lineage/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1730 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/lineage/backend.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2197 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/lineage/entities.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4442 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/logging_config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/macros/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2574 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/macros/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4884 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/macros/hive.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/migrations/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/env.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/migrations/versions/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1739 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/05f30312d566_merge_heads.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15150 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/13eb55f81627_for_compatibility.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1726 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/211e584da130_add_ti_state_index.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16341 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1475 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/2e541a1dcfed_task_duration.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2315 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1360 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3490 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/40e67319e3a9_dagrun_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1372 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/4446e08588_dagrun_start_end.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1689 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1230 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/502898887f84_adding_extra_to_log.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2605 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1257 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/52d714495f0_job_id_indices.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1952 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2512 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4511 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16875 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2634 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5447 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1323 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2958 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3222 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7211 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/92c57b58940d_add_fab_tables.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1920 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2874 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1301 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/9635ae0956e7_index_faskfail.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4170 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6567 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1278 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1600 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1839 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1204 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/b0125267960b_merge_heads.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1479 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1706 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1332 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1284 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1965 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3520 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1367 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5115 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1488 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3199 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1477 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1216 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1503 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1534 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3522 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11190 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/e3a246e0dc1_current_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1536 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/models/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    66313 2021-08-06 14:28:15.000000 smartpip2-2.1.9.5/airflow/models/baseoperator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13786 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/connection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2771 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/crypto.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    96020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    27766 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/dagbag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/dagcode.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/dagparam.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1914 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/dagpickle.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    30854 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/dagrun.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/errors.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2239 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/log.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/pool.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/renderedtifields.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6417 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/sensorinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/serialized_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6652 2021-09-30 12:06:57.000000 smartpip2-2.1.9.5/airflow/models/skipmixin.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/slamiss.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/taskfail.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    82913 2023-05-09 09:43:06.000000 smartpip2-2.1.9.5/airflow/models/taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/taskmixin.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/taskreschedule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7485 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/variable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9883 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/xcom.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/models/xcom_arg.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/mypy/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/mypy/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/mypy/plugin/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/mypy/plugin/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2866 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/mypy/plugin/decorators.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/operators/
+-rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6978 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/bash.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/bash_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2120 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/branch.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1070 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/branch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2897 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/dagrun_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/datetime.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/docker_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/druid_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/dummy.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/dummy_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/email.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/email_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/gcs_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/generic_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/google_api_to_s3_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/hive_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1166 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/hive_stats_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/hive_to_druid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1663 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/hive_to_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/hive_to_samba_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1118 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/http_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/jdbc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2696 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/latest_only.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/latest_only_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/mssql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1668 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/mssql_to_hive.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/mysql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/mysql_to_hive.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/oracle_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/papermill_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/pig_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/postgres_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/presto_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1658 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/presto_to_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18378 2021-08-07 01:46:07.000000 smartpip2-2.1.9.5/airflow/operators/python.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/python_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1680 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/redshift_to_s3_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/s3_file_transform_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1622 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/s3_to_hive_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/s3_to_redshift_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/slack_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    20630 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/sql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1476 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/sql_branch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/sqlite_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8631 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/subdag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1098 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/subdag_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6935 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/trigger_dagrun.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/operators/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14314 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/plugins_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      882 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/provider_info.schema.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    17989 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/providers_manager.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/secrets/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/secrets/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3321 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/secrets/base_secrets.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1601 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/secrets/environment_variables.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12137 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/secrets/local_filesystem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/secrets/metastore.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/security/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/security/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/security/kerberos.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2582 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/security/permissions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2880 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/security/utils.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/sensors/
+-rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/base_sensor_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3334 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/bash.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2851 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/date_time.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/date_time_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13029 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/external_task.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2380 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/filesystem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/hdfs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/hive_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/http_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/metastore_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/named_hive_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2864 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/python.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/s3_key_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/s3_prefix_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    30370 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/smart_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4769 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/sql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/sql_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/time_delta.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/time_delta_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1406 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/time_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/web_hdfs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/sensors/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/sentry.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/serialization/
+-rw-r--r--   0 johnyan    (501) staff       (20)      813 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/serialization/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/serialization/enums.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/serialization/helpers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2313 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/serialization/json_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8061 2021-08-06 13:03:21.000000 smartpip2-2.1.9.5/airflow/serialization/schema.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    35709 2021-08-06 14:28:15.000000 smartpip2-2.1.9.5/airflow/serialization/serialized_objects.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    19745 2023-05-10 01:22:38.000000 smartpip2-2.1.9.5/airflow/settings.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/smart_sensor_dags/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/smart_sensor_dags/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2086 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/smart_sensor_dags/smart_sensor_group.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13906 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/stats.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/task/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/task/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/task/task_runner/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2443 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/task/task_runner/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/task/task_runner/base_task_runner.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/task/task_runner/cgroup_task_runner.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4618 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/task/task_runner/standard_task_runner.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/templates.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/ti_deps/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4779 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/dep_context.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/dependencies_deps.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1504 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/dependencies_states.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/
+-rw-r--r--   0 johnyan    (501) staff       (20)      844 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5905 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/base_ti_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1449 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/dag_ti_slots_available_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/dag_unpaused_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2245 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/dagrun_exists_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/dagrun_id_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/exec_date_after_start_date_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2132 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/not_in_retry_period_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3232 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/not_previously_skipped_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2871 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/pool_slots_available_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/prev_dagrun_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/ready_to_reschedule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2275 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/runnable_exec_date_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1639 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/task_concurrency_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/task_not_running_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/trigger_rule_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/ti_deps/deps/valid_state_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:51.000000 smartpip2-2.1.9.5/airflow/typing_compat.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3672 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/callback_requests.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/cli.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3847 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/cli_action_loggers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/code_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1579 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/compression.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1409 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/configuration.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2413 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/dag_cycle_tester.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    49403 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/dag_processing.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10420 2021-08-09 11:44:27.000000 smartpip2-2.1.9.5/airflow/utils/dates.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    21208 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/db.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1859 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/decorators.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1312 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/docs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6061 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/dot_renderer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/edgemodifier.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12203 2023-05-09 06:05:26.000000 smartpip2-2.1.9.5/airflow/utils/email.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1521 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/entry_points.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1489 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/event_scheduler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8221 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/file.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7066 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/helpers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2457 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/json.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/utils/log/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/cloudwatch_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/colored_log.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/es_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/file_processor_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11716 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/file_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/gcs_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/json_formatter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/log_reader.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/logging_mixin.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/s3_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8849 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/secrets_masker.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/stackdriver_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2178 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/task_handler_with_custom_formatter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/log/wasb_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/mixins.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1414 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/module_loading.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/net.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/operator_helpers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/operator_resources.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/orm_event_handlers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2704 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/platform.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/process_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/python_virtualenv.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1892 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/python_virtualenv_script.jinja2
+-rw-r--r--   0 johnyan    (501) staff       (20)     3817 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/retries.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2975 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/serve_logs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2420 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/session.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9571 2021-08-09 11:25:35.000000 smartpip2-2.1.9.5/airflow/utils/sqlalchemy.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/state.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/strings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15018 2021-08-06 13:06:23.000000 smartpip2-2.1.9.5/airflow/utils/task_group.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/timeout.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5244 2021-08-09 11:25:54.000000 smartpip2-2.1.9.5/airflow/utils/timezone.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/trigger_rule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/types.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1640 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/weight_rule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2412 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/utils/yaml.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1196 2022-10-13 03:18:37.000000 smartpip2-2.1.9.5/airflow/version.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/
+-rw-r--r--   0 johnyan    (501) staff       (20)       87 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/.eslintignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       84 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/.eslintrc
+-rw-r--r--   0 johnyan    (501) staff       (20)       26 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/.stylelintignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       45 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/.stylelintrc
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/api/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/api/experimental/
+-rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/api/experimental/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15690 2021-08-05 08:41:16.000000 smartpip2-2.1.9.5/airflow/www/api/experimental/endpoints.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5616 2021-08-09 08:25:04.000000 smartpip2-2.1.9.5/airflow/www/app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4186 2021-08-06 17:29:43.000000 smartpip2-2.1.9.5/airflow/www/auth.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      984 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/blueprints.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3152 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/decorators.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/extensions/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_appbuilder.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-09-15 03:14:39.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_appbuilder_links.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_dagbag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_jinja_globals.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2102 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_manifest_files.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2041 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_security.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1683 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_session.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8001 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_views.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/extensions/init_wsgi_middlewares.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8227 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/forms.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/gunicorn_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2755 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    30652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/security.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/static/
+-rw-r--r--   0 johnyan    (501) staff       (20)   622963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/airflow.gif
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/static/css/
+-rw-r--r--   0 johnyan    (501) staff       (20)   127184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/bootstrap-theme.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1209 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/calendar.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     3047 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/dags.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1392 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/flash.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1325 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/gantt.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     3240 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/graph.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1385 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/loading-dots.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     9964 2022-10-13 06:28:22.000000 smartpip2-2.1.9.5/airflow/www/static/css/main.css
+-rw-r--r--   0 johnyan    (501) staff       (20)   112025 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/material-icons.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     2416 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/switch.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/css/tree.css
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/static/dist/
+-rw-r--r--   0 johnyan    (501) staff       (20)   104074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     7718 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/bootstrap-datetimepicker.min.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    37970 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/bootstrap-datetimepicker.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    10289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/bootstrap3-typeahead.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1087 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    15940 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   346026 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/circles.995e0afd45c3641109e1.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5931 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/codemirror.css
+-rw-r--r--   0 johnyan    (501) staff       (20)   398753 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/codemirror.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1466 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/coffeescript-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8981 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1310 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/css-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    29780 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/d3-shape.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     9207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/d3-tip.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   151725 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/d3.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    14075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     6495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     9796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    28194 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.core.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    26948 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.core.min.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)   725181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   668783 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.min.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)     2612 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    16899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     4226 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dataTables.bootstrap.min.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/dataTables.bootstrap.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5203 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/flash.d205b61edc54ed448412.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/flash.d205b61edc54ed448412.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    40502 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    53822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1989 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/html-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    16827 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/ie.e458fc4544c628f16e02.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2159 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/javascript-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    38837 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/javascript.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    83565 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/jquery.dataTables.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)  1283507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/jshint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1333 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/json-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/lint.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     9125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4229 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     7313 2022-10-13 06:28:22.000000 smartpip2-2.1.9.5/airflow/www/static/dist/main.e52cf607b64cdcd15089.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    15979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/main.e52cf607b64cdcd15089.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     3327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/manifest.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   111620 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   385945 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/moment.c1933ee062e9650051f7.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8329 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     3677 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.css.map
+-rw-r--r--   0 johnyan    (501) staff       (20)   253352 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)  1954533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)   993008 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/redoc.standalone.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2816 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)  3389627 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/redoc.standalone.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/sum.md5
+-rw-r--r--   0 johnyan    (501) staff       (20)     2091 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/switch.e97750fdb7423f33656a.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/switch.e97750fdb7423f33656a.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     9898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    31314 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    23111 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/tree.412f55814f4c1710d907.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    46722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/tree.412f55814f4c1710d907.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5116 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5055 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1255 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/dist/yaml-lint.js
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/static/js/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11183 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/calendar.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     3436 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/circles.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     4994 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/connection_form.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8057 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/dag.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1010 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/dag_code.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5997 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/dag_dependencies.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    11004 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/dags.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     3593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/datetime_utils.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/duration_chart.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8882 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/gantt.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    21515 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/graph.js
+-rw-r--r--   0 johnyan    (501) staff       (20)      887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/ie.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     6355 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/main.js
+-rw-r--r--   0 johnyan    (501) staff       (20)      995 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/meta_value.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1107 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/task_instance.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     4274 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/task_instances.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5599 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/ti_log.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    15167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/tree.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/trigger.js
+-rw-r--r--   0 johnyan    (501) staff       (20)      957 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/js/variable_edit.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    16671 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/loading.gif
+-rw-r--r--   0 johnyan    (501) staff       (20)     3184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/pin.svg
+-rw-r--r--   0 johnyan    (501) staff       (20)     7501 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/pin_100.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     1547 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/pin_25.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/pin_32.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     2306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/pin_35.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     2685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/pin_40.png
+-rw-r--r--   0 johnyan    (501) staff       (20)    24922 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/pin_large.png
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/static/screenshots/
+-rw-r--r--   0 johnyan    (501) staff       (20)    31140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/screenshots/gantt.png
+-rw-r--r--   0 johnyan    (501) staff       (20)    38282 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/screenshots/graph.png
+-rw-r--r--   0 johnyan    (501) staff       (20)    35259 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/screenshots/tree.png
+-rw-r--r--   0 johnyan    (501) staff       (20)      160 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/sort_asc.png
+-rw-r--r--   0 johnyan    (501) staff       (20)      201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/sort_both.png
+-rw-r--r--   0 johnyan    (501) staff       (20)      158 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/static/sort_desc.png
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/airflow/www/templates/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/calendar.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2581 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/chart.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1345 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/circles.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/code.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1894 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/config.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/confirm.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1038 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/conn_create.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1049 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/conn_edit.html
+-rw-r--r--   0 johnyan    (501) staff       (20)    21916 2021-09-21 03:40:31.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/dag.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/dag_code.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/dag_dependencies.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3424 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/dag_details.html
+-rw-r--r--   0 johnyan    (501) staff       (20)    16490 2021-09-21 04:00:33.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/dags.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2900 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/duration_chart.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/gantt.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     5609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/graph.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     4035 2021-08-09 08:31:54.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/main.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3173 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/model_list.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      950 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/noaccess.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/plugin.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/redoc.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2213 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/task.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/task_instance.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1044 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/ti_code.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2929 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/ti_log.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1431 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/traceback.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     4480 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/tree.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/trigger.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/variable_edit.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/variable_list.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1231 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/airflow/xcom.html
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/templates/analytics/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1195 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/analytics/google_analytics.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1807 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/analytics/metarouter.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1810 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/analytics/segment.html
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/
+-rw-r--r--   0 johnyan    (501) staff       (20)     4446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/custom_icons.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/dag_docs.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3000 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/flash.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      809 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/index.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/loading_dots.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     4388 2022-10-13 06:34:20.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/navbar.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2001 2022-10-13 08:38:39.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/navbar_menu.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3486 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/templates/appbuilder/navbar_right.html
+-rw-r--r--   0 johnyan    (501) staff       (20)    16328 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2615 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/validators.py
+-rw-r--r--   0 johnyan    (501) staff       (20)   149695 2021-11-22 06:20:23.000000 smartpip2-2.1.9.5/airflow/www/views.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6792 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/webpack.config.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2549 2021-08-04 09:43:52.000000 smartpip2-2.1.9.5/airflow/www/widgets.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/licenses/
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1131 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-bootstrap.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)      984 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-bootstrap3-typeahead.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)      556 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-connexion.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-d3-shape.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1079 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-d3-tip.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-d3js.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1062 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-dagre-d3.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1076 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-datatables.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1081 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-elasticmock.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1301 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-flask-kerberos.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)    11349 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-hue.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)    11357 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-jqclock.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1605 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-jquery.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1077 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-moment-strftime.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1075 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-moment.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/licenses/LICENSE-normalize.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/scripts/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/scripts/systemd/
+-rw-rw-r--   0 johnyan    (501) staff       (20)      678 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/README
+-rw-rw-r--   0 johnyan    (501) staff       (20)      968 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/airflow
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1195 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/airflow-flower.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1200 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/airflow-kerberos.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1190 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/airflow-scheduler.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1243 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/airflow-webserver.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1203 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/airflow-worker.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)      824 2021-08-03 16:23:18.000000 smartpip2-2.1.9.5/scripts/systemd/airflow.conf
+-rw-rw-r--   0 johnyan    (501) staff       (20)     4042 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/setup.cfg
+-rw-rw-r--   0 johnyan    (501) staff       (20)    33517 2023-06-05 02:46:19.000000 smartpip2-2.1.9.5/setup.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-05 02:46:38.000000 smartpip2-2.1.9.5/smartpip2.egg-info/
+-rw-r--r--   0 johnyan    (501) staff       (20)    26641 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/smartpip2.egg-info/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)    44202 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/smartpip2.egg-info/SOURCES.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/smartpip2.egg-info/dependency_links.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/smartpip2.egg-info/entry_points.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2021-08-07 01:38:26.000000 smartpip2-2.1.9.5/smartpip2.egg-info/not-zip-safe
+-rw-r--r--   0 johnyan    (501) staff       (20)    29803 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/smartpip2.egg-info/requires.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        8 2023-06-05 02:46:37.000000 smartpip2-2.1.9.5/smartpip2.egg-info/top_level.txt
```

### Comparing `smartpip2-2.1.9.4/CHANGELOG.txt` & `smartpip2-2.1.9.5/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/LICENSE` & `smartpip2-2.1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/MANIFEST.in` & `smartpip2-2.1.9.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/PKG-INFO` & `smartpip2-2.1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: smartpip2
-Version: 2.1.9.4
+Version: 2.1.9.5
 Summary: Programmatically author, schedule and monitor data pipelines
 Home-page: https://www.smartchart.cn/
 Author: Apache Software Foundation
 Author-email: 84345999@qq.com
 License: Apache License 2.0
-Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.4
+Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.5
 Project-URL: Documentation, https://airflow.apache.org/docs/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Description: <!--
          Licensed to the Apache Software Foundation (ASF) under one
          or more contributor license agreements.  See the NOTICE file
          distributed with this work for additional information
@@ -357,116 +357,116 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: jdbc
-Provides-Extra: statsd
-Provides-Extra: s3
-Provides-Extra: async
-Provides-Extra: cgroups
-Provides-Extra: all
-Provides-Extra: rabbitmq
-Provides-Extra: docker
-Provides-Extra: microsoft.winrm
-Provides-Extra: pagerduty
-Provides-Extra: druid
+Provides-Extra: mongo
+Provides-Extra: zendesk
+Provides-Extra: apache.hive
 Provides-Extra: snowflake
-Provides-Extra: plexus
-Provides-Extra: discord
-Provides-Extra: slack
-Provides-Extra: apache.livy
-Provides-Extra: celery
-Provides-Extra: databricks
 Provides-Extra: devel
 Provides-Extra: webhdfs
-Provides-Extra: kerberos
-Provides-Extra: jira
-Provides-Extra: devel_hadoop
-Provides-Extra: cncf.kubernetes
-Provides-Extra: crypto
-Provides-Extra: microsoft.azure
-Provides-Extra: spark
-Provides-Extra: tableau
-Provides-Extra: cloudant
-Provides-Extra: google
-Provides-Extra: apache.hive
-Provides-Extra: mongo
+Provides-Extra: hive
+Provides-Extra: sendgrid
 Provides-Extra: deprecated_api
+Provides-Extra: discord
+Provides-Extra: devel_all
+Provides-Extra: grpc
+Provides-Extra: apache.spark
+Provides-Extra: kubernetes
+Provides-Extra: all
+Provides-Extra: trino
+Provides-Extra: apache.drill
+Provides-Extra: async
+Provides-Extra: microsoft.winrm
+Provides-Extra: apache.sqoop
 Provides-Extra: openfaas
-Provides-Extra: hdfs
-Provides-Extra: hive
-Provides-Extra: amazon
-Provides-Extra: ldap
-Provides-Extra: presto
-Provides-Extra: qubole
-Provides-Extra: telegram
-Provides-Extra: airbyte
-Provides-Extra: gcp_api
-Provides-Extra: ftp
-Provides-Extra: pinot
-Provides-Extra: mysql
-Provides-Extra: odbc
+Provides-Extra: crypto
+Provides-Extra: docker
+Provides-Extra: qds
 Provides-Extra: salesforce
-Provides-Extra: neo4j
+Provides-Extra: databricks
+Provides-Extra: plexus
+Provides-Extra: celery
+Provides-Extra: kerberos
+Provides-Extra: jenkins
 Provides-Extra: dingding
-Provides-Extra: devel_ci
-Provides-Extra: apache.atlas
-Provides-Extra: hashicorp
+Provides-Extra: telegram
+Provides-Extra: devel_hadoop
+Provides-Extra: all_dbs
+Provides-Extra: sentry
 Provides-Extra: apache.hdfs
-Provides-Extra: mssql
-Provides-Extra: yandex
-Provides-Extra: dask
-Provides-Extra: samba
-Provides-Extra: gcp
-Provides-Extra: imap
-Provides-Extra: jenkins
-Provides-Extra: virtualenv
-Provides-Extra: github_enterprise
-Provides-Extra: segment
-Provides-Extra: devel_all
-Provides-Extra: apache.drill
-Provides-Extra: singularity
 Provides-Extra: aws
-Provides-Extra: postgres
+Provides-Extra: vertica
+Provides-Extra: jdbc
+Provides-Extra: datadog
+Provides-Extra: apache.cassandra
+Provides-Extra: apache.pig
 Provides-Extra: papermill
-Provides-Extra: sendgrid
-Provides-Extra: apache.kylin
+Provides-Extra: exasol
+Provides-Extra: redis
+Provides-Extra: imap
+Provides-Extra: apache.pinot
+Provides-Extra: tableau
+Provides-Extra: apache.atlas
+Provides-Extra: neo4j
+Provides-Extra: presto
+Provides-Extra: password
+Provides-Extra: oracle
+Provides-Extra: azure
+Provides-Extra: jira
 Provides-Extra: opsgenie
+Provides-Extra: gcp
+Provides-Extra: sftp
+Provides-Extra: google
+Provides-Extra: statsd
+Provides-Extra: ftp
+Provides-Extra: druid
+Provides-Extra: singularity
 Provides-Extra: asana
-Provides-Extra: oracle
-Provides-Extra: apache.pinot
-Provides-Extra: exasol
-Provides-Extra: apache.cassandra
-Provides-Extra: doc
-Provides-Extra: microsoft.mssql
-Provides-Extra: atlas
-Provides-Extra: kubernetes
+Provides-Extra: rabbitmq
+Provides-Extra: apache.webhdfs
+Provides-Extra: hashicorp
 Provides-Extra: apache.beam
-Provides-Extra: elasticsearch
-Provides-Extra: redis
-Provides-Extra: vertica
+Provides-Extra: facebook
+Provides-Extra: cgroups
+Provides-Extra: pagerduty
+Provides-Extra: hdfs
+Provides-Extra: microsoft.azure
+Provides-Extra: dask
+Provides-Extra: odbc
+Provides-Extra: postgres
 Provides-Extra: google_auth
-Provides-Extra: sentry
-Provides-Extra: zendesk
-Provides-Extra: apache.sqoop
+Provides-Extra: gcp_api
 Provides-Extra: http
+Provides-Extra: cloudant
+Provides-Extra: slack
+Provides-Extra: spark
+Provides-Extra: elasticsearch
+Provides-Extra: qubole
+Provides-Extra: airbyte
+Provides-Extra: doc
+Provides-Extra: pinot
+Provides-Extra: virtualenv
+Provides-Extra: apache.livy
+Provides-Extra: ldap
+Provides-Extra: samba
+Provides-Extra: cassandra
 Provides-Extra: leveldb
-Provides-Extra: apache.pig
-Provides-Extra: facebook
-Provides-Extra: apache.webhdfs
-Provides-Extra: apache.druid
-Provides-Extra: trino
-Provides-Extra: all_dbs
-Provides-Extra: sftp
+Provides-Extra: s3
+Provides-Extra: github_enterprise
+Provides-Extra: yandex
+Provides-Extra: devel_ci
+Provides-Extra: mssql
 Provides-Extra: winrm
-Provides-Extra: azure
-Provides-Extra: grpc
+Provides-Extra: microsoft.mssql
+Provides-Extra: amazon
 Provides-Extra: sqlite
-Provides-Extra: password
-Provides-Extra: apache.spark
-Provides-Extra: cassandra
-Provides-Extra: qds
-Provides-Extra: datadog
+Provides-Extra: cncf.kubernetes
+Provides-Extra: segment
+Provides-Extra: apache.kylin
+Provides-Extra: mysql
+Provides-Extra: apache.druid
 Provides-Extra: ssh
+Provides-Extra: atlas
```

### Comparing `smartpip2-2.1.9.4/README.md` & `smartpip2-2.1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/__init__.py` & `smartpip2-2.1.9.5/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/__main__.py` & `smartpip2-2.1.9.5/airflow/__main__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/__init__.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/abstract.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/abstract.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/aiohttp_api.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/aiohttp_api.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_api.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/flask_api.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_utils.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/apis/flask_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/abstract.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/abstract.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/aiohttp_app.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/aiohttp_app.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/flask_app.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/apps/flask_app.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/cli.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/cli.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/coroutine_wrappers.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/coroutine_wrappers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/decorator.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/metrics.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/metrics.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/parameter.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/parameter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/produces.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/produces.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/response.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/response.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/security.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/uri_parsing.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/validation.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/decorators/validation.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/exceptions.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/handlers.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/handlers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/json_schema.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/json_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/jsonifier.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/jsonifier.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/lifecycle.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/lifecycle.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/mock.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/mock.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/abstract.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/abstract.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/openapi.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/openapi.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/secure.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/secure.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/swagger2.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/operations/swagger2.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/options.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/options.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/problem.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/problem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/resolver.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/resolver.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/setup.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/setup.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/spec.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/spec.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/_vendor/connexion/utils.py` & `smartpip2-2.1.9.5/airflow/_vendor/connexion/utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/alembic.ini` & `smartpip2-2.1.9.5/airflow/alembic.ini`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/__init__.py` & `smartpip2-2.1.9.5/airflow/api/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/auth/__init__.py` & `smartpip2-2.1.9.5/airflow/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/auth/backend/__init__.py` & `smartpip2-2.1.9.5/airflow/api/auth/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/auth/backend/basic_auth.py` & `smartpip2-2.1.9.5/airflow/api/auth/backend/basic_auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/auth/backend/default.py` & `smartpip2-2.1.9.5/airflow/api/auth/backend/default.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/auth/backend/deny_all.py` & `smartpip2-2.1.9.5/airflow/api/auth/backend/deny_all.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/auth/backend/kerberos_auth.py` & `smartpip2-2.1.9.5/airflow/api/auth/backend/kerberos_auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/auth/backend/smart_auth.py` & `smartpip2-2.1.9.5/airflow/api/auth/backend/smart_auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/client/__init__.py` & `smartpip2-2.1.9.5/airflow/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/client/api_client.py` & `smartpip2-2.1.9.5/airflow/api/client/api_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/client/json_client.py` & `smartpip2-2.1.9.5/airflow/api/client/json_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/client/local_client.py` & `smartpip2-2.1.9.5/airflow/api/client/local_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/__init__.py` & `smartpip2-2.1.9.5/airflow/api/common/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/__init__.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/delete_dag.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/delete_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/get_code.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/get_code.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_run_state.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/get_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_runs.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/get_dag_runs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/get_lineage.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/get_lineage.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/get_task.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/get_task.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/get_task_instance.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/get_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/mark_tasks.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/mark_tasks.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/pool.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/pool.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api/common/experimental/trigger_dag.py` & `smartpip2-2.1.9.5/airflow/api/common/experimental/trigger_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/__init__.py` & `smartpip2-2.1.9.5/airflow/api_connexion/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/__init__.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/config_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/config_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/connection_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/connection_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dag_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_run_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dag_run_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_source_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dag_source_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dagsetup_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/dagsetup_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/event_log_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/event_log_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/extra_link_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/extra_link_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/health_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/health_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/import_error_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/import_error_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/log_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/log_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/plugin_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/plugin_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/pool_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/pool_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/provider_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/provider_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/role_and_permission_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/role_and_permission_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/task_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_instance_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/task_instance_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/user_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/user_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/variable_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/variable_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/version_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/version_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/xcom_endpoint.py` & `smartpip2-2.1.9.5/airflow/api_connexion/endpoints/xcom_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/exceptions.py` & `smartpip2-2.1.9.5/airflow/api_connexion/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/openapi/v1.yaml` & `smartpip2-2.1.9.5/airflow/api_connexion/openapi/v1.yaml`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/parameters.py` & `smartpip2-2.1.9.5/airflow/api_connexion/parameters.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/__init__.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/common_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/common_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/config_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/config_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/connection_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/connection_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_run_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/dag_run_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/dag_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_source_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/dag_source_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/enum_schemas.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/enum_schemas.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/error_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/error_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/event_log_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/event_log_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/health_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/health_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/log_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/log_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/plugin_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/plugin_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/pool_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/pool_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/provider_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/provider_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/role_and_permission_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/role_and_permission_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/sla_miss_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/sla_miss_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_instance_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/task_instance_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/task_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/user_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/user_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/variable_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/variable_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/version_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/version_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/schemas/xcom_schema.py` & `smartpip2-2.1.9.5/airflow/api_connexion/schemas/xcom_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/api_connexion/security.py` & `smartpip2-2.1.9.5/airflow/api_connexion/security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/__init__.py` & `smartpip2-2.1.9.5/airflow/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/cli_parser.py` & `smartpip2-2.1.9.5/airflow/cli/cli_parser.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/__init__.py` & `smartpip2-2.1.9.5/airflow/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/celery_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/celery_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/cheat_sheet_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/cheat_sheet_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/config_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/config_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/connection_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/connection_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/dag_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/dag_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/db_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/db_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/info_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/jobs_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/jobs_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/kerberos_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/kerberos_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/kubernetes_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/kubernetes_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/legacy_commands.py` & `smartpip2-2.1.9.5/airflow/cli/commands/legacy_commands.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/plugins_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/plugins_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/pool_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/pool_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/provider_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/provider_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/role_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/role_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/rotate_fernet_key_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/rotate_fernet_key_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/scheduler_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/scheduler_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/sync_perm_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/sync_perm_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/task_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/task_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/user_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/user_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/variable_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/variable_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/version_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/version_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/commands/webserver_command.py` & `smartpip2-2.1.9.5/airflow/cli/commands/webserver_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/cli/simple_table.py` & `smartpip2-2.1.9.5/airflow/cli/simple_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/common/datax.py` & `smartpip2-2.1.9.5/airflow/common/datax.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/common/smartpip.py` & `smartpip2-2.1.9.5/airflow/common/smartpip.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,874 +10,870 @@
 except :#line:12
     logging .warning ('you need pip install kafka-python')#line:13
 os .environ ['NLS_LANG']='SIMPLIFIED CHINESE_CHINA.UTF8'#line:15
 requests .packages .urllib3 .disable_warnings ()#line:16
 from airflow .settings import ETL_FILE_PATH ,KETTLE_HOME ,HIVE_HOME ,P_URL ,DATASET_TOKEN ,REFRESH_TOKEN #line:18
 from airflow .utils .email import fun_email ,list_email #line:19
 from airflow .common .datax import datax_cmdStr #line:20
-_OOOOO00OO00O00OO0 =f'{P_URL}/echart/dataset_api/?token={DATASET_TOKEN}&visitor=Airflow&type='#line:23
-_O0OO0OO00OO0OO00O =f'{P_URL}/echart/refresh_ds/?token={REFRESH_TOKEN}&type='#line:24
-_O00OO00O000O0OOO0 =f'{P_URL}/dm/api/sync_tableQuality/?token={REFRESH_TOKEN}&project='#line:25
-class SmartPipError (Exception ):#line:28
-    def __init__ (OO0000O0O0OOOO0O0 ,err ='SmartPip Error'):#line:29
-        Exception .__init__ (OO0000O0O0OOOO0O0 ,err )#line:30
-def smart_upload (OO00OOO00O00O00O0 ):#line:34
-    OOO00000OOO00O0O0 ,O00O00OOO0OO0O00O =os .path .split (OO00OOO00O00O00O0 )#line:35
-    O00O00OOO0OO0O00O =O00O00OOO0OO0O00O .split ('.')[0 ]#line:36
-    O00OO0OOO0OOO0O0O ={"title":O00O00OOO0OO0O00O ,"token":DATASET_TOKEN ,"visitor":"Airflow"}#line:41
-    O00O0O00OO0O00000 ={'file':open (OO00OOO00O00O00O0 ,'rb')}#line:42
-    OOO000000000OOOO0 =f'''{P_URL}/echart/dataset_api/?type=uploadlog&visitor=Airflow&token={DATASET_TOKEN}&param={{"uptime":"{time.time()}","filename":"{O00O00OOO0OO0O00O}"}}'''#line:43
-    O0OO0O000O00O00O0 =60 #line:44
-    OO000000O0O00O0OO =requests .post (f'{P_URL}/etl/api/upload_file_api/',files =O00O0O00OO0O00000 ,data =O00OO0OOO0OOO0O0O, verify=False )#line:46
-    print (OO000000O0O00O0OO .status_code )#line:47
-    if OO000000O0O00O0OO .status_code ==200 :#line:48
-        OO000000O0O00O0OO =OO000000O0O00O0OO .json ()#line:49
-    elif OO000000O0O00O0OO .status_code ==504 :#line:50
-        print ('timeout, try waiting...')#line:51
-        OO000000O0O00O0OO ={"result":"error","data":"time out"}#line:52
-        for O000O0OOOOOOOO00O in range (20 ):#line:53
-            O00O0OOOOO0O0O00O =requests .get (OOO000000000OOOO0, verify=False).json ()#line:54
-            print (O00O0OOOOO0O0O00O )#line:55
-            O00OO0OOO0OOO0O0O =O00O0OOOOO0O0O00O ['data']#line:56
-            if len (O00OO0OOO0OOO0O0O )>1 :#line:57
-                OO000000O0O00O0OO ={"result":"success","data":"uploaded"}#line:58
-                break #line:59
-            time .sleep (O0OO0O000O00O00O0 )#line:60
-    else :#line:61
-        OO000000O0O00O0OO ={"result":"error","data":"some thing wrong"}#line:62
-    print (OO000000O0O00O0OO )#line:63
-    if OO000000O0O00O0OO ['result']=='error':#line:64
-        raise SmartPipError ('Upload Error')#line:65
-def get_dataset (O0OOO000O00OO0OOO, param=None ):#line:68
-    ""#line:73
-    O0OOO000O00OO0OOO = _OOOOO00OO00O00OO0 +str (O0OOO000O00OO0OOO )
-    if param:
-        O0OOO000O00OO0OOO = f'{O0OOO000O00OO0OOO}&param={json.dumps(param)}'
-    OO0O000OO000OO0OO =requests .get (_OOOOO00OO00O00OO0 +str (O0OOO000O00OO0OOO ),verify =False )#line:74
-    OO0O000OO000OO0OO =OO0O000OO000OO0OO .json ()#line:75
-    return OO0O000OO000OO0OO #line:76
-def dataset (OO00O0O000OOO0OO0 ,OOO0O0OO0O000O0OO ,OO0O0OO0O000OO000 ,tolist =None ):#line:79
+from airflow .exceptions import SmartpipException #line:21
+_OOO0OOOO0OOOOOOOO =f'{P_URL}/echart/dataset_api/?token={DATASET_TOKEN}&visitor=Airflow&type='#line:24
+_OOO00O000O0OO00OO =f'{P_URL}/echart/refresh_ds/?token={REFRESH_TOKEN}&type='#line:25
+_O0OOOO0O0O0OOOO0O =f'{P_URL}/dm/api/sync_tableQuality/?token={REFRESH_TOKEN}&project='#line:26
+def smart_upload (OOOOOO00OO0OO000O ):#line:30
+    OOOO0OOOOO0000O00 ,O000OO0O0OOO0O0OO =os .path .split (OOOOOO00OO0OO000O )#line:31
+    O000OO0O0OOO0O0OO =O000OO0O0OOO0O0OO .split ('.')[0 ]#line:32
+    O0O0OO0O00O0OO000 ={"title":O000OO0O0OOO0O0OO ,"token":DATASET_TOKEN ,"visitor":"Airflow"}#line:37
+    O00OOO00O000OO0O0 ={'file':open (OOOOOO00OO0OO000O ,'rb')}#line:38
+    O0OOOOO000000OO0O =f'''{P_URL}/echart/dataset_api/?type=uploadlog&visitor=Airflow&token={DATASET_TOKEN}&param={{"uptime":"{time.time()}","filename":"{O000OO0O0OOO0O0OO}"}}'''#line:39
+    OOO00O000OO00O000 =60 #line:40
+    OO0OOO00OOO0000O0 =requests .post (f'{P_URL}/etl/api/upload_file_api/',files =O00OOO00O000OO0O0 ,data =O0O0OO0O00O0OO000 ,verify =False )#line:42
+    print (OO0OOO00OOO0000O0 .status_code )#line:43
+    if OO0OOO00OOO0000O0 .status_code ==200 :#line:44
+        OO0OOO00OOO0000O0 =OO0OOO00OOO0000O0 .json ()#line:45
+    elif OO0OOO00OOO0000O0 .status_code ==504 :#line:46
+        print ('timeout, try waiting...')#line:47
+        OO0OOO00OOO0000O0 ={"result":"error","data":"time out"}#line:48
+        for O0OOOOOO00O0OOOO0 in range (20 ):#line:49
+            O0000000OO00O0000 =requests .get (O0OOOOO000000OO0O ,verify =False ).json ()#line:50
+            print (O0000000OO00O0000 )#line:51
+            O0O0OO0O00O0OO000 =O0000000OO00O0000 ['data']#line:52
+            if len (O0O0OO0O00O0OO000 )>1 :#line:53
+                OO0OOO00OOO0000O0 ={"result":"success","data":"uploaded"}#line:54
+                break #line:55
+            time .sleep (OOO00O000OO00O000 )#line:56
+    else :#line:57
+        OO0OOO00OOO0000O0 ={"result":"error","data":"some thing wrong"}#line:58
+    print (OO0OOO00OOO0000O0 )#line:59
+    if OO0OOO00OOO0000O0 ['result']=='error':#line:60
+        raise SmartpipException ('Upload Error')#line:61
+def get_dataset (O000OO0OO0OO0O0OO ,param =None ):#line:64
+    ""#line:70
+    O0O0O0OOOO0000OOO =_OOO0OOOO0OOOOOOOO +str (O000OO0OO0OO0O0OO )#line:71
+    if param :#line:72
+        O0O0O0OOOO0000OOO =f'{O0O0O0OOOO0000OOO}&param={json.dumps(param)}'#line:73
+    OOO00000OO00OOOO0 =requests .get (O0O0O0OOOO0000OOO ,verify =False )#line:74
+    OOO00000OO00OOOO0 =OOO00000OO00OOOO0 .json ()#line:75
+    return OOO00000OO00OOOO0 #line:76
+def dataset (O0O00OOOO0OOOO0O0 ,OO0O0000OOO0O0O00 ,OOO0OOO00OO0O0O0O ,tolist =None ):#line:79
     ""#line:86
-    O0O0OO00O0O0OOO0O =60 *15 #line:87
-    O00OO0000OO000OO0 =3600 *2 #line:88
-    OO000000O0O000OO0 =''#line:89
+    O00OOOOO00OO000OO =60 *15 #line:87
+    O0OOO0000OOOO0OO0 =3600 *2 #line:88
+    O0OOO000O00O00OO0 =''#line:89
     try :#line:90
         while True :#line:91
-            OOO000O0OO0OO0O00 =requests .get (_OOOOO00OO00O00OO0 +OOO0O0OO0O000O0OO ,verify =False )#line:92
-            OOO000O0OO0OO0O00 =OOO000O0OO0OO0O00 .json ()#line:93
-            O0O0O0OOO000OOO00 =OOO000O0OO0OO0O00 ['result']#line:94
-            OOO000O0OO0OO0O00 =OOO000O0OO0OO0O00 ['data']#line:95
-            if O0O0O0OOO000OOO00 =='error':#line:96
-                raise Exception (f'{OOO000O0OO0OO0O00}')#line:97
-            OO000000O0O000OO0 =',\n'.join ([str (O00O0OOO0OOOOO00O )for O00O0OOO0OOOOO00O in OOO000O0OO0OO0O00 ])#line:98
-            print (f'Dataset: {OO000000O0O000OO0} ')#line:99
-            if OO0O0OO0O000OO000 =='e3':#line:100
-                if len (OOO000O0OO0OO0O00 )<2 :#line:101
-                    if O00OO0000OO000OO0 <=0 :#line:102
+            O0O000OO00OOO0O0O =requests .get (_OOO0OOOO0OOOOOOOO +OO0O0000OOO0O0O00 ,verify =False )#line:92
+            O0O000OO00OOO0O0O =O0O000OO00OOO0O0O .json ()#line:93
+            OOO00O00OOO0O00OO =O0O000OO00OOO0O0O ['result']#line:94
+            O0O000OO00OOO0O0O =O0O000OO00OOO0O0O ['data']#line:95
+            if OOO00O00OOO0O00OO =='error':#line:96
+                raise Exception (f'{O0O000OO00OOO0O0O}')#line:97
+            O0OOO000O00O00OO0 =',\n'.join ([str (O0000O00O0000OO00 )for O0000O00O0000OO00 in O0O000OO00OOO0O0O ])#line:98
+            print (f'Dataset: {O0OOO000O00O00OO0} ')#line:99
+            if OOO0OOO00OO0O0O0O =='e3':#line:100
+                if len (O0O000OO00OOO0O0O )<2 :#line:101
+                    if O0OOO0000OOOO0OO0 <=0 :#line:102
                         raise Exception ('超时且数据为空')#line:103
                     else :#line:104
-                        time .sleep (O0O0OO00O0O0OOO0O )#line:105
-                        O00OO0000OO000OO0 =O00OO0000OO000OO0 -O0O0OO00O0O0OOO0O #line:106
+                        time .sleep (O00OOOOO00OO000OO )#line:105
+                        O0OOO0000OOOO0OO0 =O0OOO0000OOOO0OO0 -O00OOOOO00OO000OO #line:106
                 else :#line:107
                     break #line:108
             else :#line:109
-                if len (OOO000O0OO0OO0O00 )>1 :#line:110
-                    if OO0O0OO0O000OO000 =='e1':#line:111
+                if len (O0O000OO00OOO0O0O )>1 :#line:110
+                    if OOO0OOO00OO0O0O0O =='e1':#line:111
                         raise Exception ('有异常数据')#line:112
-                    elif OO0O0OO0O000OO000 =='e2':#line:113
-                        list_email (f'Info_{OO00O0O000OOO0OO0}',f'{OO00O0O000OOO0OO0}-Dataset Status',OOO000O0OO0OO0O00 ,to_list =tolist )#line:114
+                    elif OOO0OOO00OO0O0O0O =='e2':#line:113
+                        list_email (f'Info_{O0O00OOOO0OOOO0O0}',f'{O0O00OOOO0OOOO0O0}-Dataset Status',O0O000OO00OOO0O0O ,to_list =tolist )#line:114
                 else :#line:115
-                    if OO0O0OO0O000OO000 not in ['info','e1']:#line:116
-                        OO000000O0O000OO0 ='数据为空'#line:117
-                        raise Exception (OO000000O0O000OO0 )#line:118
+                    if OOO0OOO00OO0O0O0O not in ['info','e1']:#line:116
+                        O0OOO000O00O00OO0 ='数据为空'#line:117
+                        raise Exception (O0OOO000O00O00OO0 )#line:118
                 break #line:119
-    except Exception as O000OO000OOOOOOO0 :#line:120
-        fun_email (f'{OO00O0O000OOO0OO0}-执行Dataset校验出错',OO000000O0O000OO0 ,to_list =tolist )#line:121
-        raise SmartPipError (str (O000OO000OOOOOOO0 .args ))#line:122
-def refresh_dash (OOOO0OOO0O00O0000 ,O0OO0O0O0O0OOO000 ):#line:125
+    except Exception as OOOO00O0OO0O000O0 :#line:120
+        fun_email (f'{O0O00OOOO0OOOO0O0}-执行Dataset校验出错',O0OOO000O00O00OO0 ,to_list =tolist )#line:121
+        raise SmartpipException (str (OOOO00O0OO0O000O0 .args ))#line:122
+def refresh_dash (O0OO0O0OOOOOOOO0O ,O000OO0OOO00O0O0O ):#line:125
     ""#line:128
     try :#line:129
-        OO0OOOOOOOOO0O00O =requests .get (f'{_O0OO0OO00OO0OO00O}{O0OO0O0O0O0OOO000}',verify =False )#line:130
-        OO0OOOOOOOOO0O00O =OO0OOOOOOOOO0O00O .json ()#line:131
-        print (OO0OOOOOOOOO0O00O )#line:132
-        O0OO00OO00OOO0OOO =OO0OOOOOOOOO0O00O ['status']#line:133
-        if O0OO00OO00OOO0OOO !=200 :#line:134
-            raise SmartPipError ('refresh_dash')#line:135
-    except Exception as OOO0O0OO0O0O00OO0 :#line:136
-        fun_email (f'{OOOO0OOO0O00O0000}-执行refresh出错',str (OOO0O0OO0O0O00OO0 .args ))#line:137
-        raise SmartPipError (str (OOO0O0OO0O0O00OO0 .args ))#line:138
-def refresh_quality (OOO00O0OO0OO0000O ,OOOOOOO0000000O0O ,hours =1 ):#line:140
-    ""#line:143
-    try :#line:144
-        OO00OOO0OO0OO000O =requests .get (f'{_O00OO00O000O0OOO0}{OOOOOOO0000000O0O}&hours={hours}',verify =False )#line:145
-        OO00OOO0OO0OO000O =OO00OOO0OO0OO000O .json ()#line:146
-        print (OO00OOO0OO0OO000O )#line:147
-        OOO0OOO0O000OOOOO =OO00OOO0OO0OO000O ['status']#line:148
-        if OOO0OOO0O000OOOOO !=200 :#line:149
-            raise SmartPipError ('refresh_quality')#line:150
-    except Exception as O0O0OO0O000000O00 :#line:151
-        fun_email (f'{OOO00O0OO0OO0000O}-执行refresh_quality出错',str (O0O0OO0O000000O00 .args ))#line:152
-        raise SmartPipError (str (O0O0OO0O000000O00 .args ))#line:153
-def dash_mail (O000000OOO00O0000 ,OOO000O00OOOO0000 ,O0O00OOOOOO000O0O ):#line:1
-    ""#line:5
-    if callable (OOO000O00OOOO0000 ):#line:6
-        O000OOO00O0O0OOO0 =OOO000O00OOOO0000 ()#line:7
-    else :#line:8
-        O000OOO00O0O0OOO0 =OOO000O00OOOO0000 #line:9
-    print (O000OOO00O0O0OOO0 )#line:10
-    if isinstance (O000OOO00O0O0OOO0 ,str ):#line:11
-        fun_email (O000000OOO00O0000 ,O000OOO00O0O0OOO0 ,O0O00OOOOOO000O0O )#line:12
-    else :#line:13
-        fun_email (O000OOO00O0O0OOO0 [0 ],O000OOO00O0O0OOO0 [1 ],O0O00OOOOOO000O0O )#line:14
-    print ('发送邮件成功!')
-def run_bash (O000OOOOOO0OOO0OO ):#line:157
-    OOO0OO0O000O0000O =''#line:158
-    O0OO00O0OO0OO0OOO =subprocess .Popen (O000OOOOOO0OOO0OO ,stdout =subprocess .PIPE ,stderr =subprocess .STDOUT ,shell =True ,cwd =ETL_FILE_PATH )#line:159
-    print ('PID:',O0OO00O0OO0OO0OOO .pid )#line:160
-    for OOO0OOOOO00O0OOO0 in iter (O0OO00O0OO0OO0OOO .stdout .readline ,b''):#line:161
-        if O0OO00O0OO0OO0OOO .poll ()and OOO0OOOOO00O0OOO0 ==b'':#line:162
-            break #line:163
-        OOO0OOOOO00O0OOO0 =OOO0OOOOO00O0OOO0 .decode (encoding ='utf8')#line:164
-        print (OOO0OOOOO00O0OOO0 .rstrip ())#line:165
-        OOO0OO0O000O0000O =OOO0OO0O000O0000O +OOO0OOOOO00O0OOO0 #line:166
-    O0OO00O0OO0OO0OOO .stdout .close ()#line:167
-    O00000OOO00O00000 =O0OO00O0OO0OO0OOO .wait ()#line:168
-    print ('result code: ',O00000OOO00O00000 )#line:169
-    return OOO0OO0O000O0000O ,O00000OOO00O00000 #line:170
-def run_python (O0O0OOOO0OO0OO00O ,OOOO0O0O00O0OO00O ,dev =''):#line:173
-    O00OO0OOO0OO00OO0 =O0O0OOOO0OO0OO00O .split ('/')#line:174
-    _O0OOOOO0O0O0O000O ,OO0O000O000OO0OOO =run_bash ('python %s %s'%(O0O0OOOO0OO0OO00O ,OOOO0O0O00O0OO00O ))#line:175
-    if OO0O000O000OO0OOO !=0 :#line:176
-        fun_email (f'{O00OO0OOO0OO00OO0[-2]}/{O00OO0OOO0OO00OO0[-1]}出错','python error')#line:177
-        raise Exception ('error')#line:178
-def run_dataxx (O0O00OOO0000O0000 ,OOO00O00OOOOO0000 ,dev =''):#line:182
-    O00O00OO000000O0O =O0O00OOO0000O0000 .split ('/')#line:183
-    if OOO00O00OOOOO0000 :#line:184
-        OOO0OO0OOO0O00OO0 =[f'-D{O0OO0O0O0OO0O0OOO}:{O000OO00OO000OOO0}'for O0OO0O0O0OO0O0OOO ,O000OO00OO000OOO0 in OOO00O00OOOOO0000 .items ()]#line:185
-        O0OOO0O0O00000O00 =' '.join (OOO0OO0OOO0O00OO0 )#line:186
-        O0OOO000OOO00O000 =[f'-p"{O0OOO0O0O00000O00}"',O0O00OOO0000O0000 ]#line:187
-    else :#line:188
-        O0OOO000OOO00O000 =[O0O00OOO0000O0000 ]#line:189
-    O0O0O0O0OO0OO00O0 =datax_cmdStr (O0OOO000OOO00O000 )#line:190
-    _OO0OOOOO0OO0OO000 ,OOOOO0OOO00O0OOOO =run_bash (O0O0O0O0OO0OO00O0 )#line:191
-    if OOOOO0OOO00O0OOOO !=0 :#line:192
-        fun_email (f'{O00O00OO000000O0O[-2]}/{O00O00OO000000O0O[-1]}出错','datax error')#line:193
-        raise Exception ('error')#line:194
-def run_datax (O00OO00OOO0OOO0OO ,O0O0O0OO0O0O0OO0O ,OOOO00OO0OO000000 ,OO00O0OO00OOO000O ,dev =''):#line:197
-    with open (O00OO00OOO0OOO0OO ,'r',encoding ='utf8')as OO0000O0O0000OOO0 :#line:198
-        OOOO0O0O00O0O000O =readSqlstr (OO0000O0O0000OOO0 .read ().strip (),para_dict =OO00O0OO00OOO000O )#line:199
-    OOOO0O0O00O0O000O =OOOO0O0O00O0O000O .split ('##')#line:200
-    O00O0O00OO0O00OOO ={}#line:201
-    for OOO0OOOO0O0O000O0 in OOOO0O0O00O0O000O :#line:202
-        O0O0OOO000OO0O00O =OOO0OOOO0O0O000O0 .find ('=')#line:203
-        if O0O0OOO000OO0O00O >0 :#line:204
-            O00O0O00OO0O00OOO [OOO0OOOO0O0O000O0 [:O0O0OOO000OO0O00O ].strip ()]=OOO0OOOO0O0O000O0 [O0O0OOO000OO0O00O +1 :].replace ('\n',' ').strip ()#line:205
-    O00O0OOOOOO0OO0OO =O00O0O00OO0O00OOO .keys ()#line:206
-    OOO0OO00O00OO0O0O =O00O0O00OO0O00OOO .pop ('template')if 'template'in O00O0OOOOOO0OO0OO else 'default'#line:207
-    OO0OOOOOOOOO0OOO0 =O00O0O00OO0O00OOO .get ('targetColumn')#line:208
-    O0O0OOOOO000OOOOO =None #line:209
-    if OOO0OO00O00OO0O0O .endswith ('hdfs'):#line:210
-        O0O0OOOOO000OOOOO =O00O0O00OO0O00OOO .pop ('hiveSql')if 'hiveSql'in O00O0OOOOOO0OO0OO else None #line:212
-        if not O0O0OOOOO000OOOOO :#line:213
-            O0O0OOOOO000OOOOO =O00O0O00OO0O00OOO .pop ('postSql')if 'postSql'in O00O0OOOOOO0OO0OO else None #line:214
-        if OO0OOOOOOOOO0OOO0 :#line:216
-            OO0OOOOOOOOO0OOO0 =OO0OOOOOOOOO0OOO0 .split (',')#line:217
-            OOOO0000OOOO000O0 =[]#line:218
-            for OOO0OOOO0O0O000O0 in OO0OOOOOOOOO0OOO0 :#line:219
-                if ':'in OOO0OOOO0O0O000O0 :#line:220
-                    OOO0OOOO0O0O000O0 =OOO0OOOO0O0O000O0 .split (':')#line:221
-                    OOOO0000OOOO000O0 .append ({"name":OOO0OOOO0O0O000O0 [0 ].strip (),"type":OOO0OOOO0O0O000O0 [1 ].strip ()})#line:222
-                else :#line:223
-                    OOOO0000OOOO000O0 .append ({"name":OOO0OOOO0O0O000O0 .strip (),"type":"STRING"})#line:224
-            O00O0O00OO0O00OOO ['targetColumn']=json .dumps (OOOO0000OOOO000O0 )#line:225
-    else :#line:226
-        if OO0OOOOOOOOO0OOO0 :#line:227
-            OO0OOOOOOOOO0OOO0 =[OOO00OOO00000000O .strip ()for OOO00OOO00000000O in OO0OOOOOOOOO0OOO0 .split (',')]#line:228
-            O00O0O00OO0O00OOO ['targetColumn']=json .dumps (OO0OOOOOOOOO0OOO0 )#line:229
-        else :#line:230
-            O00O0O00OO0O00OOO ['targetColumn']='["*"]'#line:231
-        if OOO0OO00O00OO0O0O .endswith ('starrocks'):#line:233
-            if '.'in O00O0O00OO0O00OOO ['targetTable']:#line:234
-                O00O0O00OO0O00OOO ['targetDB'],O00O0O00OO0O00OOO ['targetTable']=O00O0O00OO0O00OOO ['targetTable'].split ('.')#line:235
-            else :#line:236
-                O00O0O00OO0O00OOO ['targetDB']='Test'#line:237
-        else:
-            if 'writeMode' not in O00O0OOOOOO0OO0OO:
-                O00O0OOOOOO0OO0OO['writeMode'] = 'insert'
-    if 'preSql'in O00O0OOOOOO0OO0OO :#line:239
-        O00O0O00OO0O00OOO ['preSql']=json .dumps (O00O0O00OO0O00OOO ['preSql'].strip ().split (';'))#line:240
-    else :#line:241
-        O00O0O00OO0O00OOO ['preSql']=''#line:242
-    if 'postSql'in O00O0OOOOOO0OO0OO :#line:243
-        O00O0O00OO0O00OOO ['postSql']=json .dumps (O00O0O00OO0O00OOO ['postSql'].strip ().split (';'))#line:244
-    else :#line:245
-        O00O0O00OO0O00OOO ['postSql']=''#line:246
-    OO00O0OO0O0000OO0 =O00OO00OOO0OOO0OO .split ('/')#line:247
-    OO00000O00O000O0O =OO00O0OO0O0000OO0 [-1 ].split ('.')[0 ]#line:248
-    with open (os .path .join (OOOO00OO0OO000000 ,'datax','templates',OOO0OO00O00OO0O0O ),'r')as OO0000O0O0000OOO0 :#line:249
-        OOOOOOOO0000OO000 =OO0000O0O0000OOO0 .read ()#line:250
-    O00OO00OOO0OOO0OO =os .path .join (OOOO00OO0OO000000 ,'datax',OO00000O00O000O0O +'.json')#line:251
-    with open (O00OO00OOO0OOO0OO ,'w',encoding ='utf8')as OO0000O0O0000OOO0 :#line:252
-        OO0000O0O0000OOO0 .write (readSqlstr (OOOOOOOO0000OO000 ,O00O0O00OO0O00OOO ))#line:253
-    OOOOO0OOOOO0OO0OO =datax_cmdStr ([O00OO00OOO0OOO0OO ])#line:254
-    _OOO0O00OOOO000000 ,OO0000000OO0OO0O0 =run_bash (OOOOO0OOOOO0OO0OO )#line:255
-    if OO0000000OO0OO0O0 !=0 :#line:256
-        fun_email (f'{OO00O0OO0O0000OO0[-2]}/{OO00O0OO0O0000OO0[-1]}出错','datax error')#line:257
-        raise Exception ('error')#line:258
-    if O0O0OOOOO000OOOOO :#line:259
-        print (_OO000OO0O0O000OO0 (O0O0OOOOO000OOOOO .split (';'),O0O0O0OO0O0O0OO0O ,db_connect ='hive',dev =dev ))#line:260
-def readSqlFile (OOOOO0O000O00O0OO ,para_dict =None ):#line:264
-    if OOOOO0O000O00O0OO .find ('.sql')<0 :#line:265
-        return 'file type error'#line:266
-    with open (OOOOO0O000O00O0OO ,'r',encoding ='utf-8')as O000OOOO0OO0OOOOO :#line:267
-        O000OO00OO0OOOOOO =O000OOOO0OO0OOOOO .read ()#line:268
-    O000O00OO00O0O0O0 =readSqlstr (O000OO00OO0OOOOOO ,para_dict )#line:269
-    return O000O00OO00O0O0O0 #line:270
-def readSqoopFile (O0OO00OOO0OOOOO0O ,para_dict =None ):#line:273
-    if not O0OO00OOO0OOOOO0O .endswith ('.sql'):#line:274
-        return 'file type error'#line:275
-    with open (O0OO00OOO0OOOOO0O ,'r',encoding ='utf8')as OO0OO0O00OOOOOOO0 :#line:276
-        OO0O0OOO000OOO00O =OO0OO0O00OOOOOOO0 .read ().strip ()#line:277
-    O000OO0O0O0OOO00O =re .match (r"/\*(.*?)\*/(.+)",OO0O0OOO000OOO00O ,re .M |re .S )#line:278
-    OOOO000O0000O00O0 =readSqlstr (O000OO0O0O0OOO00O .group (1 ).strip (),para_dict )#line:279
-    O0OO0O00O0000O00O =O000OO0O0O0OOO00O .group (2 ).strip ()#line:280
-    return OOOO000O0000O00O0 ,O0OO0O00O0000O00O #line:281
-def readSqlstr (O00OO00OO00O00OOO ,para_dict =None ):#line:1
-    O0O000O0OOOOOO0O0 =re .sub (r"(\/\*(.|\n)*?\*\/)|--.*",'',O00OO00OO00O00OOO .strip ())#line:2
-    if para_dict :#line:3
-        for OO0OO000OO0OOOOOO ,O00OO000OO0OOO000 in para_dict .items ():#line:4
-            if OO0OO000OO0OOOOOO .isnumeric ():#line:5
-                OO00O0O0OOOO0OOO0 =get_dataset (O00OO000OO0OOO000 )['data']#line:6
-                print ('dataset:',OO00O0O0OOOO0OOO0 )#line:7
-                if len (OO00O0O0OOOO0OOO0 )>1 :#line:8
-                    for OOOOOOOO00O0OO0O0 ,O0O00OO0OOOO0O000 in zip (OO00O0O0OOOO0OOO0 [0 ],OO00O0O0OOOO0OOO0 [1 ]):#line:9
-                        O0O000O0OOOOOO0O0 =O0O000O0OOOOOO0O0 .replace ('$'+OOOOOOOO00O0OO0O0 ,str (O0O00OO0OOOO0O000 ))#line:10
-            elif callable (O00OO000OO0OOO000 ):#line:11
-                O000O0OOOOO000OO0 =O00OO000OO0OOO000 ()#line:12
-                for OOOOOOOO00O0OO0O0 ,O0O00OO0OOOO0O000 in O000O0OOOOO000OO0 .items ():#line:13
-                    O0O000O0OOOOOO0O0 =O0O000O0OOOOOO0O0 .replace ('$'+OOOOOOOO00O0OO0O0 ,str (O0O00OO0OOOO0O000 ))#line:14
-            else :#line:15
-                O0O000O0OOOOOO0O0 =O0O000O0OOOOOO0O0 .replace ('$'+OO0OO000OO0OOOOOO ,str (O00OO000OO0OOO000 ))#line:16
-    return O0O000O0OOOOOO0O0
-def run_sql_file (O00OO0OOOOOOOOOOO ,O00000000OOOOOO00 ,db_connect ='starrocks',para_dict =None ,dev =''):#line:292
-    O0000O00O0OO0OO00 =O00OO0OOOOOOOOOOO .split ('/')#line:293
-    try :#line:294
-        OO0O000OO0OO00OO0 =readSqlFile (O00OO0OOOOOOOOOOO ,para_dict ).split (';')#line:295
-        OO0O0000O0OOO000O =O00000000OOOOOO00 .get (db_connect )#line:296
-        if dev :#line:297
-            if f'{db_connect}{dev}'in O00000000OOOOOO00 .keys ():#line:298
-                OO0O0000O0OOO000O =O00000000OOOOOO00 .get (f'{db_connect}{dev}')#line:299
-        OOOOOOO0O000OOO0O =connect_db_execute ().execute_sql_list (OO0O000OO0OO00OO0 ,db_connect ,connect_dict =OO0O0000O0OOO000O )#line:300
-        return OOOOOOO0O000OOO0O #line:301
-    except Exception as OO0000O0OOOOO0OOO :#line:302
-        fun_email ('{}/{}执行出错'.format (O0000O00O0OO0OO00 [-2 ],O0000O00O0OO0OO00 [-1 ]),str (OO0000O0OOOOO0OOO .args ))#line:303
-        print (OO0000O0OOOOO0OOO .args )#line:304
-        raise SmartPipError ('Run SQL Error')#line:305
-def _OO000OO0O0O000OO0 (O00O0000O00000O00 ,OOOOO0OOO0O0O0O0O ,db_connect ='starrocks',para_dict =None ,dev =''):#line:308
-    try :#line:309
-        if isinstance (O00O0000O00000O00 ,str ):#line:310
-            O00O0000O00000O00 =readSqlstr (O00O0000O00000O00 ,para_dict ).split (';')#line:311
-        OO0O0O00000OO0000 =OOOOO0OOO0O0O0O0O .get (db_connect )#line:312
-        if dev :#line:313
-            if f'{db_connect}{dev}'in OOOOO0OOO0O0O0O0O .keys ():#line:314
-                OO0O0O00000OO0000 =OOOOO0OOO0O0O0O0O .get (f'{db_connect}{dev}')#line:315
-        O0OOO00O000000OO0 =connect_db_execute ().execute_sql_list (O00O0000O00000O00 ,db_connect ,connect_dict =OO0O0O00000OO0000 )#line:316
-        return O0OOO00O000000OO0 #line:317
-    except Exception as O0OOO00000OOO00O0 :#line:318
-        fun_email ('SQL执行出错',f'{O00O0000O00000O00}{O0OOO00000OOO00O0.args}')#line:319
-        print (O0OOO00000OOO00O0 .args )#line:320
-        raise SmartPipError ('Run SQL Error')#line:321
-def run_sp (O0OOOOOO00O00OOOO ,O0O00000OOO0OOOO0 ,db_connect ='oracle',sp_para =None ,dev =''):#line:1
-    try :#line:2
-        O0O0OOO0OO0OOOO0O =O0O00000OOO0OOOO0 .get (db_connect )#line:3
-        if dev :#line:4
-            if f'{db_connect}{dev}'in O0O00000OOO0OOOO0 .keys ():#line:5
-                O0O0OOO0OO0OOOO0O =O0O00000OOO0OOOO0 .get (f'{db_connect}{dev}')#line:6
-        connect_db_execute ().excute_proc (O0OOOOOO00O00OOOO ,O0O0OOO0OO0OOOO0O ,sp_para )#line:7
-    except Exception as O0000O00O0000OO00 :#line:8
-        fun_email ('{}执行出错'.format (O0OOOOOO00O00OOOO ),str (O0000O00O0000OO00 .args ))#line:9
-        raise O0000O00O0000OO00
-def run_kettle (O00000O00O0OOOO0O ,para_str ='',dev =False ):#line:325
-    ""#line:332
-    O0OOOO00000OOO0OO =O00000O00O0OOOO0O .split ('/')#line:333
-    print ('kettle job start')#line:334
-    if '.ktr'in O00000O00O0OOOO0O :#line:336
-        OOO0000OO000OOO0O =f'{KETTLE_HOME}/pan.sh -level=Basic -file={O00000O00O0OOOO0O}{para_str}'#line:337
-    else :#line:338
-        OOO0000OO000OOO0O =f'{KETTLE_HOME}/kitchen.sh -level=Basic -file={O00000O00O0OOOO0O}{para_str}'#line:339
-    print (OOO0000OO000OOO0O )#line:340
-    OOOOOO00O0OO00OOO ,O00OO000OO0OOOOO0 =run_bash (OOO0000OO000OOO0O )#line:344
-    if O00OO000OO0OOOOO0 ==0 :#line:345
-        print ('{} 完成数据抽取'.format (str (O00000O00O0OOOO0O )))#line:346
-    else :#line:347
-        print ('{} 执行错误'.format (O00000O00O0OOOO0O ))#line:348
-        fun_email ('{}/{}出错'.format (O0OOOO00000OOO0OO [-2 ],O0OOOO00000OOO0OO [-1 ]),str (OOOOOO00O0OO00OOO ))#line:349
-        raise SmartPipError ('Run Kettle Error')#line:350
-def hdfsStarrocks (O0O0OOO0OO0OO0OOO ,OO0O0O0OO00O0O00O ,para_dict =None ):#line:354
-    ""#line:358
-    OO00OOOOOOOO0OO0O =O0O0OOO0OO0OO0OOO .split ('/')#line:359
-    print ('starrocks load job start')#line:360
-    OOOO0OO0OO0OO00OO ,O0OOOOO00O000O0OO =readSqoopFile (O0O0OOO0OO0OO0OOO ,para_dict =para_dict )#line:361
-    OOOO0OO0OO0OO00OO =OOOO0OO0OO0OO00OO .split ('\n')#line:362
-    OOOO0O00OO000000O ={}#line:363
-    OOOO0O00OO000000O ['LABEL']=f'{OO00OOOOOOOO0OO0O[-2]}{OO00OOOOOOOO0OO0O[-1][:-4]}{int(time.time())}'#line:364
-    OOOO0O00OO000000O ['HDFS']=HIVE_HOME #line:365
-    for O000O0OOOOOO0O0O0 in OOOO0OO0OO0OO00OO :#line:366
-        O0O000OO0OOO0O0O0 =O000O0OOOOOO0O0O0 .find ('=')#line:367
-        if O0O000OO0OOO0O0O0 >0 :#line:368
-            OOOO0O00OO000000O [O000O0OOOOOO0O0O0 [:O0O000OO0OOO0O0O0 ].strip ()]=O000O0OOOOOO0O0O0 [O0O000OO0OOO0O0O0 +1 :].strip ()#line:369
-    OO00O00OO0OO0000O =OOOO0O00OO000000O .get ('sleepTime')#line:371
-    if OO00O00OO0OO0000O :#line:372
-        OO00O00OO0OO0000O =int (OO00O00OO0OO0000O )#line:373
-        if OO00O00OO0OO0000O <30 :#line:374
-            OO00O00OO0OO0000O =30 #line:375
-    else :#line:376
-        OO00O00OO0OO0000O =30 #line:377
-    OOO00OOOOO00OOO00 =OOOO0O00OO000000O .get ('maxTime')#line:379
-    if OOO00OOOOO00OOO00 :#line:380
-        OOO00OOOOO00OOO00 =int (OOO00OOOOO00OOO00 )#line:381
-        if OOO00OOOOO00OOO00 >3600 :#line:382
-            OOO00OOOOO00OOO00 =3600 #line:383
-    else :#line:384
-        OOO00OOOOO00OOO00 =600 #line:385
-    _OO000OO0O0O000OO0 (O0OOOOO00O000O0OO ,OO0O0O0OO00O0O00O ,db_connect ='starrocks',para_dict =OOOO0O00OO000000O )#line:387
-    time .sleep (OO00O00OO0OO0000O )#line:388
-    OO0O00000O00O0000 =f'''show load from {OOOO0O00OO000000O.get('targetDB')} where label = '{OOOO0O00OO000000O['LABEL']}' order by CreateTime desc limit 1 '''#line:389
-    O0OOOO00OOOO000O0 ='start to check label'#line:390
-    try :#line:391
-        while True :#line:392
-            O0OOOO00OOOO000O0 =_OO000OO0O0O000OO0 ([OO0O00000O00O0000 ],OO0O0O0OO00O0O00O ,db_connect ='starrocks')#line:393
-            print (O0OOOO00OOOO000O0 )#line:394
-            OOOOO0OOOOOO0OOOO =O0OOOO00OOOO000O0 [1 ][2 ]#line:395
-            if OOOOO0OOOOOO0OOOO =='CANCELLED':#line:396
-                raise Exception (f'Starrocks:{OOOOO0OOOOOO0OOOO}')#line:397
-            elif OOOOO0OOOOOO0OOOO =='FINISHED':#line:398
-                print ('Load completed')#line:399
-                break #line:400
-            if OOO00OOOOO00OOO00 <=0 :#line:401
-                raise Exception ('超时未完成')#line:402
-            else :#line:403
-                time .sleep (OO00O00OO0OO0000O )#line:404
-                OOO00OOOOO00OOO00 =OOO00OOOOO00OOO00 -OO00O00OO0OO0000O #line:405
-    except Exception as O00O0000OO0O0O0O0 :#line:406
-        print ('{} 执行错误'.format (O0O0OOO0OO0OO0OOO ))#line:407
-        fun_email ('{}/{}执行出错'.format (OO00OOOOOOOO0OO0O [-2 ],OO00OOOOOOOO0OO0O [-1 ]),str (O0OOOO00OOOO000O0 ))#line:408
-        raise SmartPipError (str (O00O0000OO0O0O0O0 .args ))#line:409
-def kafkaStarrocks (OO00O0OO0OO0OO0OO ,O000OO0OOOOO000OO ,OOO00OOOOO0OO0OOO ,OO0000O0000OOO0OO ,O00OO0OOO0OO0O0O0 ,dev =''):#line:412
-    with open (OO00O0OO0OO0OO0OO ,'r',encoding ='utf8')as OOOOO0OO0000OOOO0 :#line:413
-        O00O00O00000O0OO0 =readSqlstr (OOOOO0OO0000OOOO0 .read ().strip (),para_dict =O00OO0OOO0OO0O0O0 )#line:414
-    O00O00O00000O0OO0 =O00O00O00000O0OO0 .split ('##')#line:415
-    O00OO0O00OO0OOO0O ={}#line:416
-    for O0O00OOOO0OO000O0 in O00O00O00000O0OO0 :#line:417
-        O0000OO0OOO0OOO00 =O0O00OOOO0OO000O0 .find ('=')#line:418
-        if O0000OO0OOO0OOO00 >0 :#line:419
-            O00O00OO0OO00O0O0 =O0O00OOOO0OO000O0 [O0000OO0OOO0OOO00 +1 :].replace ('\n',' ').strip ()#line:420
-            if O00O00OO0OO00O0O0 :#line:421
-                O00OO0O00OO0OOO0O [O0O00OOOO0OO000O0 [:O0000OO0OOO0OOO00 ].strip ()]=O00O00OO0OO00O0O0 #line:422
-    O000O0000O00O0000 =O00OO0O00OO0OOO0O .pop ('topic')#line:423
-    OO000O0O0000OOO00 =O00OO0O00OO0OOO0O .pop ('table')#line:424
-    O0O0OO000OOOOOO00 =O00OO0O00OO0OOO0O .keys ()#line:425
-    if 'skipError'in O0O0OO000OOOOOO00 :#line:426
-        skipError =O00OO0O00OO0OOO0O .pop ('skipError')#line:427
-    else :#line:428
-        skipError =None #line:429
-    if 'kafkaConn'in O0O0OO000OOOOOO00 :#line:430
-        O0O0O00OOOO0000O0 =O00OO0O00OO0OOO0O .pop ('kafkaConn')#line:431
-    else :#line:432
-        O0O0O00OOOO0000O0 ='default'#line:433
-    if 'offsets'in O0O0OO000OOOOOO00 :#line:434
-        O00O00OO000OOOO00 =json .loads (O00OO0O00OO0OOO0O .pop ('offsets'))#line:435
-    else :#line:436
-        O00O00OO000OOOO00 =None #line:437
-    if 'json_root'in O0O0OO000OOOOOO00 :#line:438
-        OO00O0O00O00OO000 =O00OO0O00OO0OOO0O .pop ('json_root')#line:439
-    else :#line:440
-        OO00O0O00O00OO000 =None #line:441
-    if 'jsonpaths'in O0O0OO000OOOOOO00 :#line:442
-        O0000000O0O0OOOOO =O00OO0O00OO0OOO0O .get ('jsonpaths')#line:443
-        if not O0000000O0O0OOOOO .startswith ('['):#line:444
-            O0000000O0O0OOOOO =O0000000O0O0OOOOO .split (',')#line:445
-            O0000000O0O0OOOOO =json .dumps (['$.'+OOOOO00O0OO00OO0O .strip ()for OOOOO00O0OO00OO0O in O0000000O0O0OOOOO ])#line:446
-            O00OO0O00OO0OOO0O ['jsonpaths']=O0000000O0O0OOOOO #line:447
-    OOO0O000O00O0OOO0 =_OO00O0OOO000O00O0 (O000O0000O00O0000 ,O000OO0OOOOO000OO [O0O0O00OOOO0000O0 ],OO0000O0000OOO0OO ,O00O00OO000OOOO00 )#line:448
-    def O00O0O00OO00OO0O0 (OOOO0OOOOO00O0OOO ):#line:450
-        OO0OOO0O0OOO0OO0O =b''#line:451
-        O0OO0OOOO0O0OOOOO =None #line:452
-        if 'format'in O0O0OO000OOOOOO00 :#line:453
-            for O0OO0OOOO0O0OOOOO in OOOO0OOOOO00O0OOO :#line:454
-                O0000OO00OO000OOO =O0OO0OOOO0O0OOOOO .value #line:455
-                if OO00O0O00O00OO000 :#line:456
-                    O0000OO00OO000OOO =json .loads (O0000OO00OO000OOO .decode ('utf8'))#line:457
-                    O0000OO00OO000OOO =json .dumps (O0000OO00OO000OOO [OO00O0O00O00OO000 ]).encode ('utf8')#line:458
-                if O0000OO00OO000OOO .startswith (b'['):#line:459
-                    OO0OOO0O0OOO0OO0O =OO0OOO0O0OOO0OO0O +b','+O0000OO00OO000OOO [1 :-1 ]#line:460
-                else :#line:461
-                    OO0OOO0O0OOO0OO0O =OO0OOO0O0OOO0OO0O +b','+O0000OO00OO000OOO #line:462
-                if len (OO0OOO0O0OOO0OO0O )>94857600 :#line:463
-                    streamStarrocks (OO000O0O0000OOO00 ,OOO00OOOOO0OO0OOO ,O00OO0O00OO0OOO0O ,OO0OOO0O0OOO0OO0O ,skipError )#line:464
-                    OOO0O000O00O0OOO0 .write_offset (O0OO0OOOO0O0OOOOO .partition ,O0OO0OOOO0O0OOOOO .offset +1 )#line:465
-                    OO0OOO0O0OOO0OO0O =b''#line:466
-                if O0OO0OOOO0O0OOOOO .offset ==OOO0O000O00O0OOO0 .end_offset -1 :#line:467
-                    break #line:468
-        else :#line:469
-            for O0OO0OOOO0O0OOOOO in OOOO0OOOOO00O0OOO :#line:470
-                O0000OO00OO000OOO =O0OO0OOOO0O0OOOOO .value #line:471
-                if OO00O0O00O00OO000 :#line:472
-                    O0000OO00OO000OOO =json .loads (O0000OO00OO000OOO .decode ('utf8'))#line:473
-                    O0000OO00OO000OOO =json .dumps (O0000OO00OO000OOO [OO00O0O00O00OO000 ]).encode ('utf8')#line:474
-                OO0OOO0O0OOO0OO0O =OO0OOO0O0OOO0OO0O +b'\n'+O0000OO00OO000OOO #line:475
-                if len (OO0OOO0O0OOO0OO0O )>94857600 :#line:476
-                    streamStarrocks (OO000O0O0000OOO00 ,OOO00OOOOO0OO0OOO ,O00OO0O00OO0OOO0O ,OO0OOO0O0OOO0OO0O ,skipError )#line:477
-                    OOO0O000O00O0OOO0 .write_offset (O0OO0OOOO0O0OOOOO .partition ,O0OO0OOOO0O0OOOOO .offset +1 )#line:478
-                    OO0OOO0O0OOO0OO0O =b''#line:479
-                if O0OO0OOOO0O0OOOOO .offset ==OOO0O000O00O0OOO0 .end_offset -1 :#line:480
-                    break #line:481
-        print (OO0OOO0O0OOO0OO0O [1 :1000 ])#line:482
-        if OO0OOO0O0OOO0OO0O :#line:483
-            streamStarrocks (OO000O0O0000OOO00 ,OOO00OOOOO0OO0OOO ,O00OO0O00OO0OOO0O ,OO0OOO0O0OOO0OO0O ,skipError )#line:484
-        return O0OO0OOOO0O0OOOOO #line:485
-    OOO0O000O00O0OOO0 .consumer_topic (O00O0O00OO00OO0O0 )#line:487
-def apiStarrocks (O0O0OO0O0OO0000O0 ,O00O0OOO0O0OOO00O ,O0000O00O0000O0OO ,OOO0OO00O0OOOOO00 ):#line:490
-    with open (O0O0OO0O0OO0000O0 ,'r',encoding ='utf8')as O0O0OO0O000OO0000 :#line:491
-        OO0OO0O0O0000OOOO =readSqlstr (O0O0OO0O000OO0000 .read ().strip (),para_dict =OOO0OO00O0OOOOO00 )#line:492
-    OO0OO0O0O0000OOOO =OO0OO0O0O0000OOOO .split ('##')#line:493
-    O00O0OO000OO00OOO ={}#line:494
-    for O0000000O00OO000O in OO0OO0O0O0000OOOO :#line:495
-        O00OOO0OO00000O0O =O0000000O00OO000O .find ('=')#line:496
-        if O00OOO0OO00000O0O >0 :#line:497
-            O00000O00O0O0O00O =O0000000O00OO000O [O00OOO0OO00000O0O +1 :].replace ('\n',' ').strip ()#line:498
-            if O00000O00O0O0O00O :#line:499
-                O00O0OO000OO00OOO [O0000000O00OO000O [:O00OOO0OO00000O0O ].strip ()]=O00000O00O0O0O00O #line:500
-    OOO00O0000O00OO00 =O00O0OO000OO00OOO .pop ('table')#line:501
-    OOOOO0O0O00000000 =O00O0OO000OO00OOO .keys ()#line:502
-    if 'param'in OOOOO0O0O00000000 :#line:503
-        OOO00O0O00OO0OO0O =O00O0OO000OO00OOO .pop ('param')#line:504
-    else :#line:505
-        OOO00O0O00OO0OO0O =None #line:506
-    if 'apiConn'in OOOOO0O0O00000000 :#line:507
-        O0O000000O000OO00 =O00O0OO000OO00OOO .pop ('apiConn')#line:508
-    else :#line:509
-        O0O000000O000OO00 ='default'#line:510
-    if 'skipError'in OOOOO0O0O00000000 :#line:511
-        skipError =O00O0OO000OO00OOO .pop ('skipError')#line:512
-    else :#line:513
-        skipError =None #line:514
-    if 'jsonpaths'in OOOOO0O0O00000000 :#line:515
-        O0OOO0O000O000000 =O00O0OO000OO00OOO .get ('jsonpaths')#line:516
-        if not O0OOO0O000O000000 .startswith ('['):#line:517
-            O0OOO0O000O000000 =O0OOO0O000O000000 .split (',')#line:518
-            O0OOO0O000O000000 =json .dumps (['$.'+O0OO0O00OO0000O0O .strip ()for O0OO0O00OO0000O0O in O0OOO0O000O000000 ])#line:519
-            O00O0OO000OO00OOO ['jsonpaths']=O0OOO0O000O000000 #line:520
-    OOOO00O00000OOOOO =O00O0OOO0O0OOO00O [O0O000000O000OO00 ](OOO00O0O00OO0OO0O )#line:521
-    if OOOO00O00000OOOOO :#line:522
-        streamStarrocks (OOO00O0000O00OO00 ,O0000O00O0000O0OO ,O00O0OO000OO00OOO ,OOOO00O00000OOOOO ,skipError )#line:523
-    else :#line:524
-        print ('无数据')#line:525
-def streamStarrocks (OO0OOO0OOOO00OO0O ,O00O0OO0O0O000OO0 ,O0O0000OOOOOOOOOO ,OO000OO0000O00000 ,skipError =False ):#line:528
-    ""#line:531
-    import base64 ,uuid #line:532
-    O0O0O0O0OOOOOOOO0 ,OO0OOO0OOOO00OO0O =OO0OOO0OOOO00OO0O .split ('.')#line:533
-    O00O0OOOOO00O0O00 =str (base64 .b64encode (f'{O00O0OO0O0O000OO0["user"]}:{O00O0OO0O0O000OO0["password"]}'.encode ('utf-8')),'utf-8')#line:534
-    OO000OO0000O00000 =OO000OO0000O00000 .strip ()#line:535
-    if OO000OO0000O00000 .startswith (b','):#line:536
-        O0O0000OOOOOOOOOO ['strip_outer_array']='true'#line:537
-        OO000OO0000O00000 =b'['+OO000OO0000O00000 [1 :]+b']'#line:538
-    O0OO0OOOO00000O00 ={'Content-Type':'application/json','Authorization':f'Basic {O00O0OOOOO00O0O00}','label':f'{OO0OOO0OOOO00OO0O}{uuid.uuid4()}',**O0O0000OOOOOOOOOO }#line:544
-    O0O0O0OOOO00O0O0O =f"{O00O0OO0O0O000OO0['url']}/api/{O0O0O0O0OOOOOOOO0}/{OO0OOO0OOOO00OO0O}/_stream_load"#line:545
-    print ('start loading to starrocks....')#line:546
-    O0O0O00OO00000OOO =requests .put (O0O0O0OOOO00O0O0O ,headers =O0OO0OOOO00000O00 ,data =OO000OO0000O00000 ).json ()#line:547
-    print (O0O0O00OO00000OOO )#line:548
-    if O0O0O00OO00000OOO ['Status']=='Fail':#line:549
-        if skipError :#line:550
-            print (f'Starrocks Load Error, Skip this offset')#line:551
-        else :#line:552
-            raise Exception ('Starrocks Load Error')#line:553
-def routineStarrocks (OOOO0O0O0OO0000O0 ,OO0O0OO00O00O0OOO ,flag =''):#line:556
-    O0000OOO0O000O000 =_OO000OO0O0O000OO0 ([f'SHOW ROUTINE LOAD FOR {OO0O0OO00O00O0OOO}'],OOOO0O0O0OO0000O0 ,db_connect ='starrocks')#line:557
-    O0000OOO0O000O000 =dict (zip (O0000OOO0O000O000 [0 ],O0000OOO0O000O000 [1 ]))#line:558
-    print ('状态:',O0000OOO0O000O000 ['State'])#line:559
-    print ('统计:',O0000OOO0O000O000 ['Statistic'])#line:560
-    print ('进度:',O0000OOO0O000O000 ['Progress'])#line:561
-    if O0000OOO0O000O000 ['State']!='RUNNING':#line:562
-        print ('ERROR: ',O0000OOO0O000O000 ['ReasonOfStateChanged'])#line:563
-        if not flag :#line:564
-            raise Exception ('Starrocks Routin Load')#line:565
-from airflow .utils .session import provide_session #line:571
-@provide_session #line:572
-def point_test (OOO000OOOO0O000OO ,sleeptime ='',maxtime ='',session =None ):#line:573
-    ""#line:580
-    if sleeptime :#line:581
-        sleeptime =int (sleeptime )#line:582
-        sleeptime =sleeptime if sleeptime >60 else 60 #line:583
-    if maxtime :#line:584
-        maxtime =int (maxtime )#line:585
-        maxtime =maxtime if maxtime <60 *60 *2 else 60 *60 *2 #line:586
-    else :#line:587
-        maxtime =0 #line:588
-    try :#line:589
-        OOO000OO0O0O000OO =f"select start_date,state from dag_run where dag_id ='{OOO000OOOO0O000OO}' ORDER BY id desc LIMIT 1"#line:590
-        while True :#line:591
-            O0O00OO0OOOO0OOOO =session .execute (OOO000OO0O0O000OO ).fetchall ()#line:592
-            if O0O00OO0OOOO0OOOO [0 ][1 ]!='success':#line:593
-                if maxtime >0 and O0O00OO0OOOO0OOOO [0 ][1 ]!='failed':#line:594
-                    print ('waiting...'+O0O00OO0OOOO0OOOO [0 ][1 ])#line:595
-                    time .sleep (sleeptime )#line:596
-                    maxtime =maxtime -sleeptime #line:597
-                else :#line:598
-                    O000OOO00OOO0O000 =O0O00OO0OOOO0OOOO [0 ][0 ].strftime ("%Y-%m-%d %H:%M:%S")#line:599
-                    OO0000OO00OOOO0OO ='所依赖的dag:'+OOO000OOOO0O000OO +',状态为'+O0O00OO0OOOO0OOOO [0 ][1 ]+'.其最新的执行时间为'+O000OOO00OOO0O000 #line:600
-                    fun_email (OO0000OO00OOOO0OO ,'前置DAG任务未成功')#line:601
-                    print (OO0000OO00OOOO0OO )#line:602
-                    raise SmartPipError ('Run DAG validate Error')#line:603
-            else :#line:604
-                print ('success...')#line:605
-                break #line:606
-    except Exception as O0OO000O0OO0O0O00 :#line:607
-        print (O0OO000O0OO0O0O00 .args )#line:608
-        raise SmartPipError ('DAG validate Error')#line:609
-class connect_db_execute ():#line:614
-    def __init__ (O0OO0OO000O000OO0 ,dev =False ,db =''):#line:615
-        O0OO0OO000O000OO0 .dev =dev #line:616
-    def insert_contents (OOO000OOO00000OO0 ,OO0O00O0O00000O0O ,OO000O0OOO0O0O0O0 ,per_in =1000 ,connect_dict =None ):#line:618
-        OO0O0O000OOOO0OOO =time .time ()#line:619
-        logging .info ('starting to execute insert contents...')#line:620
-        if isinstance (connect_dict ,dict ):#line:621
-            O0OO0O0000OO000OO =connect_dict ['dbtype']#line:622
-        else :#line:623
-            if connect_dict =='':#line:624
-                O0OO0O0000OO000OO ='oracle'#line:625
-            else :#line:626
-                O0OO0O0000OO000OO =connect_dict #line:627
-            connect_dict =None #line:628
-        O0OO00O0O0000000O =getattr (OOO000OOO00000OO0 ,'insert_contents_'+O0OO0O0000OO000OO )#line:629
-        OO0O0OOO0OOO00O0O =O0OO00O0O0000000O (OO0O00O0O00000O0O ,OO000O0OOO0O0O0O0 ,per_in ,connect_dict )#line:630
-        logging .info ('execute insert contents time : {}ms'.format (time .time ()-OO0O0O000OOOO0OOO ))#line:631
-        return OO0O0OOO0OOO00O0O #line:632
-    def impala (OO0OOO0OO00O00OO0 ,OOOO0OO0OOOOO0O00 ,connect_dict =None ):#line:634
-        ""#line:635
-        from impala .dbapi import connect as impala #line:636
-        O000O0O00OOO0OOO0 =impala (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =int (connect_dict ['port']),auth_mechanism ='PLAIN')#line:643
-        O0OOO000O00O0O0OO =O000O0O00OOO0OOO0 .cursor ()#line:644
-        O00000000000OOO00 =r'^insert\s|^update\s|^truncate\s|^delete\s|^load\s|^refresh\s|^upsert\s'#line:645
-        O0O0OOO0O000OOO00 =None #line:646
-        for O00OOOOOOO0O0O00O in OOOO0OO0OOOOO0O00 :#line:647
-            print (O00OOOOOOO0O0O00O )#line:648
-            O00OOOOOOO0O0O00O =O00OOOOOOO0O0O00O .strip ()#line:649
-            if not O00OOOOOOO0O0O00O :#line:650
-                continue #line:651
-            if re .search (O00000000000OOO00 ,O00OOOOOOO0O0O00O ,re .I |re .IGNORECASE ):#line:652
-                O0OOO000O00O0O0OO .execute (O00OOOOOOO0O0O00O )#line:653
-            else :#line:654
-                O0OOO000O00O0O0OO .execute (O00OOOOOOO0O0O00O )#line:655
-                try :#line:656
-                    O0O0OOO0O000OOO00 =O0OOO000O00O0O0OO .fetchall ()#line:657
-                except Exception as O0OOO000OOO00000O :#line:658
-                    print (O0OOO000OOO00000O .args )#line:659
-        O000O0O00OOO0OOO0 .close ()#line:660
-        return O0O0OOO0O000OOO00 #line:661
-    def hive (OOO0O00O00OO000O0 ,O0OOOO0OOO00O000O ,connect_dict =None ):#line:663
-        ""#line:664
-        from impala .dbapi import connect as impala #line:665
-        O0OOOOO0O0O0O0O0O =impala (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =int (connect_dict ['port']),auth_mechanism ='PLAIN')#line:672
-        OOOO0OO0OO0OOO0OO =O0OOOOO0O0O0O0O0O .cursor ()#line:673
-        O00000O0O0000O0O0 =r'^insert\s|^update\s|^truncate\s|^delete\s|^load\s'#line:674
-        OO0OOOOO0OOOOOOOO =None #line:675
-        for O0O0000OOOOOO0000 in O0OOOO0OOO00O000O :#line:676
-            O0O0000OOOOOO0000 =O0O0000OOOOOO0000 .strip ()#line:677
-            if not O0O0000OOOOOO0000 :#line:678
-                continue #line:679
-            print (O0O0000OOOOOO0000 )#line:680
-            if O0O0000OOOOOO0000 .startswith ('refresh'):#line:681
-                connect_dict ['port']=21050 #line:682
-                OOO0O00O00OO000O0 .impala ([O0O0000OOOOOO0000 ],connect_dict =connect_dict )#line:683
-            else :#line:684
-                if re .search (O00000O0O0000O0O0 ,O0O0000OOOOOO0000 ,re .I |re .IGNORECASE ):#line:685
-                    OOOO0OO0OO0OOO0OO .execute (O0O0000OOOOOO0000 )#line:686
-                else :#line:687
-                    OOOO0OO0OO0OOO0OO .execute (O0O0000OOOOOO0000 )#line:688
-                    try :#line:689
-                        OO0OOOOO0OOOOOOOO =OOOO0OO0OO0OOO0OO .fetchall ()#line:690
-                    except Exception as OOOO00O0OO0O0OOO0 :#line:691
-                        print (OOOO00O0OO0O0OOO0 .args )#line:692
-        O0OOOOO0O0O0O0O0O .close ()#line:693
-        return OO0OOOOO0OOOOOOOO #line:694
-    def mysql (O0OOO000000O000O0 ,OOOO0O0O0OO0O000O ,connect_dict =None ):#line:696
-        import pymysql #line:697
-        OOO00O0O000O0O00O =pymysql .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =connect_dict ['port'],database =connect_dict ['db'])#line:704
-        try :#line:705
-            O0O000OO00OO0OOOO =OOO00O0O000O0O00O .cursor ()#line:706
-            OO0000O0O0OO000O0 =r'^insert\s|^update\s|^truncate\s|^delete\s|^load\s'#line:707
-            for O000O0O0OOOO0O000 in OOOO0O0O0OO0O000O :#line:708
-                O000O0O0OOOO0O000 =O000O0O0OOOO0O000 .strip ()#line:709
-                if not O000O0O0OOOO0O000 :#line:710
-                    continue #line:711
-                print (O000O0O0OOOO0O000 )#line:712
-                if re .search (OO0000O0O0OO000O0 ,O000O0O0OOOO0O000 ,re .I |re .IGNORECASE ):#line:713
-                    try :#line:714
-                        O0O000OO00OO0OOOO .execute (O000O0O0OOOO0O000 )#line:715
-                        OOO00O0O000O0O00O .commit ()#line:716
-                    except Exception as OOOOO00OO00000000 :#line:717
-                        OOO00O0O000O0O00O .rollback ()#line:718
-                        raise OOOOO00OO00000000 #line:719
-                else :#line:720
-                    O0O000OO00OO0OOOO .execute (O000O0O0OOOO0O000 )#line:721
-                    O0O0O000O0000OO00 =O0O000OO00OO0OOOO .fetchall ()#line:722
-                    O0O0O000O0000OO00 =[[OO00OOO0000O0OO00 [0 ]for OO00OOO0000O0OO00 in O0O000OO00OO0OOOO .description ]]+list (O0O0O000O0000OO00 )#line:723
-                    return O0O0O000O0000OO00 #line:724
-        except Exception as O0O000000O0OOOO00 :#line:725
-            raise O0O000000O0OOOO00 #line:726
-        finally :#line:727
-            OOO00O0O000O0O00O .close ()#line:728
-    def starrocks (O0OOO000O0O0O0O00 ,OO0O0O0OOO0O000O0 ,connect_dict =None ):#line:730
-        return O0OOO000O0O0O0O00 .mysql (OO0O0O0OOO0O000O0 ,connect_dict )#line:731
-    def oracle (O00O0OO00O00O0OOO ,OO00O00O00OOO0OO0 ,connect_dict =None ):#line:733
-        import cx_Oracle #line:734
-        O00OOOO00000O000O ='{}/{}@{}/{}'.format (connect_dict ['user'],connect_dict ['password'],connect_dict ['host'],connect_dict ['db'])#line:739
-        O00000OO00O00O000 =cx_Oracle .connect (O00OOOO00000O000O )#line:740
-        try :#line:741
-            OO0OO0OOO00O00OOO =O00000OO00O00O000 .cursor ()#line:742
-            O00O0OOO0000OOO0O =r'^insert\s|^update\s|^truncate\s|^delete\s|^comment\s'#line:743
-            for OO0O00OO0000OOOO0 in OO00O00O00OOO0OO0 :#line:744
-                OO0O00OO0000OOOO0 =OO0O00OO0000OOOO0 .strip ()#line:745
-                if not OO0O00OO0000OOOO0 :#line:746
-                    continue #line:747
-                if re .search (O00O0OOO0000OOO0O ,OO0O00OO0000OOOO0 ,re .I ):#line:748
-                    try :#line:749
-                        OO0OO0OOO00O00OOO .execute (OO0O00OO0000OOOO0 )#line:750
-                        O00000OO00O00O000 .commit ()#line:751
-                    except Exception as O0O000OO0O0OOOO00 :#line:752
-                        if OO0O00OO0000OOOO0 .startswith ('comment'):#line:753
-                            print ('err:',OO0O00OO0000OOOO0 )#line:754
-                            continue #line:755
-                        O00000OO00O00O000 .rollback ()#line:756
-                        raise O0O000OO0O0OOOO00 #line:757
-                else :#line:758
-                    OO0OO0OOO00O00OOO .execute (OO0O00OO0000OOOO0 )#line:759
-                    O0OO0O000OOOO0000 =OO0OO0OOO00O00OOO .fetchall ()#line:760
-                    O0OO0O000OOOO0000 =[[O00OO000O00OO0000 [0 ]for O00OO000O00OO0000 in OO0OO0OOO00O00OOO .description ]]+list (O0OO0O000OOOO0000 )#line:761
-                    return O0OO0O000OOOO0000 #line:762
-        except Exception as OOO0000OOO0OOO0O0 :#line:763
-            raise OOO0000OOO0OOO0O0 #line:764
-        finally :#line:765
-            O00000OO00O00O000 .close ()#line:766
-    def gp (O0OOOO00OO00O00O0 ,O000O00O000OO0OOO ,connect_dict =None ):#line:768
-        import psycopg2 #line:769
-        O0OO000O00000O0OO =psycopg2 .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =connect_dict ['port'],database =connect_dict ['db'])#line:776
-        try :#line:777
-            O00O00000000O00O0 =O0OO000O00000O0OO .cursor ()#line:778
-            OOOOO0O0OOOOO0O00 =r'^insert\s|^update\s|^truncate\s|^delete\s'#line:779
-            for OOO0OO000OOOOO0OO in O000O00O000OO0OOO :#line:780
-                OOO0OO000OOOOO0OO =OOO0OO000OOOOO0OO .strip ()#line:781
-                if not OOO0OO000OOOOO0OO :#line:782
-                    continue #line:783
-                if re .search (OOOOO0O0OOOOO0O00 ,OOO0OO000OOOOO0OO ,re .I |re .IGNORECASE ):#line:784
-                    try :#line:785
-                        O00O00000000O00O0 .execute (OOO0OO000OOOOO0OO )#line:786
-                        O0OO000O00000O0OO .commit ()#line:787
-                    except Exception as OOO0OOOO0OO0O0000 :#line:788
-                        O0OO000O00000O0OO .rollback ()#line:789
-                        raise OOO0OOOO0OO0O0000 #line:790
-                else :#line:791
-                    O00O00000000O00O0 .execute (OOO0OO000OOOOO0OO )#line:792
-                    OO0000OOO000O0OO0 =O00O00000000O00O0 .fetchall ()#line:793
-                    OO0000OOO000O0OO0 =[[O00O0O00O0O0000O0 [0 ]for O00O0O00O0O0000O0 in O00O00000000O00O0 .description ]]+list (OO0000OOO000O0OO0 )#line:794
-                    return OO0000OOO000O0OO0 #line:795
-        except Exception as OOO0000000O00O00O :#line:796
-            raise OOO0000000O00O00O #line:797
-        finally :#line:798
-            O0OO000O00000O0OO .close ()#line:799
-    def mssql (O0OO00O0000OOO0OO ,O00OO00O000O0OO00 ,connect_dict =None ):#line:801
-        import pymssql #line:802
-        if connect_dict ['port']:#line:803
-            O00OO0OOOO00OOO00 =pymssql .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =int (connect_dict ['port']),database =connect_dict ['db'],charset ="utf8",)#line:811
-        else :#line:812
-            O00OO0OOOO00OOO00 =pymssql .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],database =connect_dict ['db'],charset ="utf8",)#line:819
-        try :#line:820
-            OO00000O00000O0O0 =O00OO0OOOO00OOO00 .cursor ()#line:821
-            OO0O0OOOOOO0O0OOO =r'^insert\s|^update\s|^truncate\s|^delete\s'#line:822
-            for O0O0OOOOOOO0000OO in O00OO00O000O0OO00 :#line:823
-                O0O0OOOOOOO0000OO =O0O0OOOOOOO0000OO .strip ()#line:824
-                if not O0O0OOOOOOO0000OO :#line:825
-                    continue #line:826
-                if re .search (OO0O0OOOOOO0O0OOO ,O0O0OOOOOOO0000OO ,re .I |re .IGNORECASE ):#line:827
-                    try :#line:828
-                        OO00000O00000O0O0 .execute (O0O0OOOOOOO0000OO )#line:829
-                        O00OO0OOOO00OOO00 .commit ()#line:830
-                    except Exception as O00O0000OO0O00OO0 :#line:831
-                        O00OO0OOOO00OOO00 .rollback ()#line:832
-                        raise O00O0000OO0O00OO0 #line:833
-                else :#line:834
-                    OO00000O00000O0O0 .execute (O0O0OOOOOOO0000OO )#line:835
-                    OO0OOOO00OOO00OOO =OO00000O00000O0O0 .fetchall ()#line:836
-                    OO0OOOO00OOO00OOO =[[O0O0O00OOOO00O00O [0 ]for O0O0O00OOOO00O00O in OO00000O00000O0O0 .description ]]+list (OO0OOOO00OOO00OOO )#line:837
-                    return OO0OOOO00OOO00OOO #line:838
-        except Exception as O00OOO0000O000O00 :#line:839
-            raise O00OOO0000O000O00 #line:840
-        finally :#line:841
-            O00OO0OOOO00OOO00 .close ()#line:842
-    def execute_sql_list (O0OO000000O00OO0O ,OO000000OO00O0O0O ,db_connect ='',connect_dict =None ):#line:844
-        if db_connect =='':db_connect ='oracle'#line:845
-        O0OOO00OOOO00OOO0 =getattr (O0OO000000O00OO0O ,db_connect )#line:846
-        return O0OOO00OOOO00OOO0 (OO000000OO00O0O0O ,connect_dict =connect_dict )#line:847
-    def excute_proc (O0O0O000O000O00OO ,O00OO000OO0OOO000 ,O0O0000O00O0OO0OO ,proc_para =None ):#line:849
-        import cx_Oracle #line:850
-        OOO0OO0OO0OO0OOOO ='{}/{}@{}/{}'.format (O0O0000O00O0OO0OO ['user'],O0O0000O00O0OO0OO ['password'],O0O0000O00O0OO0OO ['host'],O0O0000O00O0OO0OO ['db'])#line:856
-        OOO0OOOO0O0O0O000 =cx_Oracle .connect (OOO0OO0OO0OO0OOOO )#line:857
+        OO0OOO000OO0O00OO =requests .get (f'{_OOO00O000O0OO00OO}{O000OO0OOO00O0O0O}',verify =False )#line:130
+        OO0OOO000OO0O00OO =OO0OOO000OO0O00OO .json ()#line:131
+        print (OO0OOO000OO0O00OO )#line:132
+        O00O0OOO0O000OO00 =OO0OOO000OO0O00OO ['status']#line:133
+        if O00O0OOO0O000OO00 !=200 :#line:134
+            raise SmartpipException ('refresh_dash')#line:135
+    except Exception as O00000000O0O0000O :#line:136
+        fun_email (f'{O0OO0O0OOOOOOOO0O}-执行refresh出错',str (O00000000O0O0000O .args ))#line:137
+        raise SmartpipException (str (O00000000O0O0000O .args ))#line:138
+def refresh_quality (OO000000O0OO0OO00 ,OO0O00O00O0OOOOOO ,hours =1 ):#line:141
+    ""#line:144
+    try :#line:145
+        O00OO00OO00O0OOOO =requests .get (f'{_O0OOOO0O0O0OOOO0O}{OO0O00O00O0OOOOOO}&hours={hours}',verify =False )#line:146
+        O00OO00OO00O0OOOO =O00OO00OO00O0OOOO .json ()#line:147
+        print (O00OO00OO00O0OOOO )#line:148
+        O00OO0OO0OO0OOOO0 =O00OO00OO00O0OOOO ['status']#line:149
+        if O00OO0OO0OO0OOOO0 !=200 :#line:150
+            raise SmartpipException ('refresh_quality')#line:151
+    except Exception as OOOOO0O000O00O0OO :#line:152
+        fun_email (f'{OO000000O0OO0OO00}-执行refresh_quality出错',str (OOOOO0O000O00O0OO .args ))#line:153
+        raise SmartpipException (str (OOOOO0O000O00O0OO .args ))#line:154
+def dash_mail (OO000O00OOO0OOO0O ,O0000OO00OO00OO0O ,O0O0OO000OO0000OO ):#line:157
+    ""#line:161
+    if callable (O0000OO00OO00OO0O ):#line:162
+        OOOOO0OOO00OO0000 =O0000OO00OO00OO0O ()#line:163
+    else :#line:164
+        OOOOO0OOO00OO0000 =O0000OO00OO00OO0O #line:165
+    print (OOOOO0OOO00OO0000 )#line:166
+    if isinstance (OOOOO0OOO00OO0000 ,str ):#line:167
+        fun_email (OO000O00OOO0OOO0O ,OOOOO0OOO00OO0000 ,O0O0OO000OO0000OO )#line:168
+    else :#line:169
+        fun_email (OOOOO0OOO00OO0000 [0 ],OOOOO0OOO00OO0000 [1 ],O0O0OO000OO0000OO )#line:170
+    print ('发送邮件成功!')#line:171
+def run_bash (OO00OOO0OO0OO0O0O ):#line:175
+    OO0OOOOO0O0O0O00O =''#line:176
+    O0OOO00000O0O00OO =subprocess .Popen (OO00OOO0OO0OO0O0O ,stdout =subprocess .PIPE ,stderr =subprocess .STDOUT ,shell =True ,cwd =ETL_FILE_PATH )#line:177
+    print ('PID:',O0OOO00000O0O00OO .pid )#line:178
+    for OOOO000O00OOOOO00 in iter (O0OOO00000O0O00OO .stdout .readline ,b''):#line:179
+        if O0OOO00000O0O00OO .poll ()and OOOO000O00OOOOO00 ==b'':#line:180
+            break #line:181
+        OOOO000O00OOOOO00 =OOOO000O00OOOOO00 .decode (encoding ='utf8')#line:182
+        print (OOOO000O00OOOOO00 .rstrip ())#line:183
+        OO0OOOOO0O0O0O00O =OO0OOOOO0O0O0O00O +OOOO000O00OOOOO00 #line:184
+    O0OOO00000O0O00OO .stdout .close ()#line:185
+    OOO00O00OO000O00O =O0OOO00000O0O00OO .wait ()#line:186
+    print ('result code: ',OOO00O00OO000O00O )#line:187
+    return OO0OOOOO0O0O0O00O ,OOO00O00OO000O00O #line:188
+def run_python (OO0OO0O0000O000O0 ,OO0O0O00OOOOO000O ,dev =''):#line:191
+    O0OOOOOO0O00OOOOO =OO0OO0O0000O000O0 .split ('/')#line:192
+    _OO0O0O00O00OO0O00 ,OOOO00OOO0OO00OO0 =run_bash ('python %s %s'%(OO0OO0O0000O000O0 ,OO0O0O00OOOOO000O ))#line:193
+    if OOOO00OOO0OO00OO0 !=0 :#line:194
+        fun_email (f'{O0OOOOOO0O00OOOOO[-2]}/{O0OOOOOO0O00OOOOO[-1]}出错','python error')#line:195
+        raise SmartpipException ('python error')#line:196
+def run_dataxx (O0OO00000OOOO00OO ,O0OOOO0O0O0000000 ,dev =''):#line:200
+    O0O00OOOOO000O0O0 =O0OO00000OOOO00OO .split ('/')#line:201
+    if O0OOOO0O0O0000000 :#line:202
+        O00000O00OO00OO00 =[f'-D{OO0O000OOOO0OOO0O}:{OOOOOOO00OOOOOOOO}'for OO0O000OOOO0OOO0O ,OOOOOOO00OOOOOOOO in O0OOOO0O0O0000000 .items ()]#line:203
+        O0OOOOO0OOO0000O0 =' '.join (O00000O00OO00OO00 )#line:204
+        O00O0000OO00OO0OO =[f'-p"{O0OOOOO0OOO0000O0}"',O0OO00000OOOO00OO ]#line:205
+    else :#line:206
+        O00O0000OO00OO0OO =[O0OO00000OOOO00OO ]#line:207
+    OO0O0000O000OO0O0 =datax_cmdStr (O00O0000OO00OO0OO )#line:208
+    _OO0O0O0OO0000O000 ,OOO0O00O0000OOOOO =run_bash (OO0O0000O000OO0O0 )#line:209
+    if OOO0O00O0000OOOOO !=0 :#line:210
+        fun_email (f'{O0O00OOOOO000O0O0[-2]}/{O0O00OOOOO000O0O0[-1]}出错','datax error')#line:211
+        raise SmartpipException ('error')#line:212
+def run_datax (OO0O00000O0OOO000 ,O0OOO000O0000O00O ,O00OO0OO00000O0OO ,OOOOO00OOO0O00OO0 ,dev =''):#line:215
+    with open (OO0O00000O0OOO000 ,'r',encoding ='utf8')as O0O0OOOOOO0000O00 :#line:216
+        O0OO0000O0000000O =readSqlstr (O0O0OOOOOO0000O00 .read ().strip (),para_dict =OOOOO00OOO0O00OO0 )#line:217
+    O0OO0000O0000000O =O0OO0000O0000000O .split ('##')#line:218
+    O0O0000O00000O00O ={}#line:219
+    for O000OO0O0O0O0OO00 in O0OO0000O0000000O :#line:220
+        OO0O0O0O00O0O0000 =O000OO0O0O0O0OO00 .find ('=')#line:221
+        if OO0O0O0O00O0O0000 >0 :#line:222
+            O0O0000O00000O00O [O000OO0O0O0O0OO00 [:OO0O0O0O00O0O0000 ].strip ()]=O000OO0O0O0O0OO00 [OO0O0O0O00O0O0000 +1 :].replace ('\n',' ').strip ()#line:223
+    OOOO00000O00O0OOO =O0O0000O00000O00O .keys ()#line:224
+    OOOOOO00O0O000000 =O0O0000O00000O00O .pop ('template')if 'template'in OOOO00000O00O0OOO else 'default'#line:225
+    OOO00000O0O00O000 =O0O0000O00000O00O .get ('targetColumn')#line:226
+    OOO0OO0OO00000000 =None #line:227
+    if OOOOOO00O0O000000 .endswith ('hdfs'):#line:228
+        OOO0OO0OO00000000 =O0O0000O00000O00O .pop ('hiveSql')if 'hiveSql'in OOOO00000O00O0OOO else None #line:230
+        if not OOO0OO0OO00000000 :#line:231
+            OOO0OO0OO00000000 =O0O0000O00000O00O .pop ('postSql')if 'postSql'in OOOO00000O00O0OOO else None #line:232
+        if OOO00000O0O00O000 :#line:234
+            OOO00000O0O00O000 =OOO00000O0O00O000 .split (',')#line:235
+            OO00000000OOOOO0O =[]#line:236
+            for O000OO0O0O0O0OO00 in OOO00000O0O00O000 :#line:237
+                if ':'in O000OO0O0O0O0OO00 :#line:238
+                    O000OO0O0O0O0OO00 =O000OO0O0O0O0OO00 .split (':')#line:239
+                    OO00000000OOOOO0O .append ({"name":O000OO0O0O0O0OO00 [0 ].strip (),"type":O000OO0O0O0O0OO00 [1 ].strip ()})#line:240
+                else :#line:241
+                    OO00000000OOOOO0O .append ({"name":O000OO0O0O0O0OO00 .strip (),"type":"STRING"})#line:242
+            O0O0000O00000O00O ['targetColumn']=json .dumps (OO00000000OOOOO0O )#line:243
+    else :#line:244
+        if OOO00000O0O00O000 :#line:245
+            OOO00000O0O00O000 =[OOOOO00OOOOOO0O00 .strip ()for OOOOO00OOOOOO0O00 in OOO00000O0O00O000 .split (',')]#line:246
+            O0O0000O00000O00O ['targetColumn']=json .dumps (OOO00000O0O00O000 )#line:247
+        else :#line:248
+            O0O0000O00000O00O ['targetColumn']='["*"]'#line:249
+        if OOOOOO00O0O000000 .endswith ('starrocks'):#line:251
+            if '.'in O0O0000O00000O00O ['targetTable']:#line:252
+                O0O0000O00000O00O ['targetDB'],O0O0000O00000O00O ['targetTable']=O0O0000O00000O00O ['targetTable'].split ('.')#line:253
+            else :#line:254
+                O0O0000O00000O00O ['targetDB']='Test'#line:255
+        else :#line:256
+            if 'writeMode'not in OOOO00000O00O0OOO :#line:257
+                O0O0000O00000O00O ['writeMode']='insert'#line:258
+    if 'preSql'in OOOO00000O00O0OOO :#line:259
+        O0O0000O00000O00O ['preSql']=json .dumps (O0O0000O00000O00O ['preSql'].strip ().split (';'))#line:260
+    else :#line:261
+        O0O0000O00000O00O ['preSql']=''#line:262
+    if 'postSql'in OOOO00000O00O0OOO :#line:263
+        O0O0000O00000O00O ['postSql']=json .dumps (O0O0000O00000O00O ['postSql'].strip ().split (';'))#line:264
+    else :#line:265
+        O0O0000O00000O00O ['postSql']=''#line:266
+    O00O0O000O0O0OOO0 =OO0O00000O0OOO000 .split ('/')#line:267
+    OOO0O00000OO0O000 =O00O0O000O0O0OOO0 [-1 ].split ('.')[0 ]#line:268
+    with open (os .path .join (O00OO0OO00000O0OO ,'datax','templates',OOOOOO00O0O000000 ),'r')as O0O0OOOOOO0000O00 :#line:269
+        OO000O0O000000OOO =O0O0OOOOOO0000O00 .read ()#line:270
+    OO0O00000O0OOO000 =os .path .join (O00OO0OO00000O0OO ,'datax',OOO0O00000OO0O000 +'.json')#line:271
+    with open (OO0O00000O0OOO000 ,'w',encoding ='utf8')as O0O0OOOOOO0000O00 :#line:272
+        O0O0OOOOOO0000O00 .write (readSqlstr (OO000O0O000000OOO ,O0O0000O00000O00O ))#line:273
+    O0O000000OO000OOO =datax_cmdStr ([OO0O00000O0OOO000 ])#line:274
+    _O0OOOO0OOOOOOO000 ,O00O0OOO0OO0O0000 =run_bash (O0O000000OO000OOO )#line:275
+    if O00O0OOO0OO0O0000 !=0 :#line:276
+        fun_email (f'{O00O0O000O0O0OOO0[-2]}/{O00O0O000O0O0OOO0[-1]}出错','datax error')#line:277
+        raise SmartpipException ('datax error')#line:278
+    if OOO0OO0OO00000000 :#line:279
+        SmartpipException (_O0O00OO0OO00O0O0O (OOO0OO0OO00000000 .split (';'),O0OOO000O0000O00O ,db_connect ='hive',dev =dev ))#line:280
+def readSqlFile (OO0O0O0OOO0OO000O ,para_dict =None ):#line:284
+    if OO0O0O0OOO0OO000O .find ('.sql')<0 :#line:285
+        return 'file type error'#line:286
+    with open (OO0O0O0OOO0OO000O ,'r',encoding ='utf-8')as O00O000000OOOOOOO :#line:287
+        OOO000000O00O0OO0 =O00O000000OOOOOOO .read ()#line:288
+    OO00OO00O00OO0OO0 =readSqlstr (OOO000000O00O0OO0 ,para_dict )#line:289
+    return OO00OO00O00OO0OO0 #line:290
+def readSqoopFile (OO0OOO0O0OOO0OOOO ,para_dict =None ):#line:293
+    if not OO0OOO0O0OOO0OOOO .endswith ('.sql'):#line:294
+        return 'file type error'#line:295
+    with open (OO0OOO0O0OOO0OOOO ,'r',encoding ='utf8')as O0000O000O0000O0O :#line:296
+        O00000O0OO0OO000O =O0000O000O0000O0O .read ().strip ()#line:297
+    OOO00OOO000O00O0O =re .match (r"/\*(.*?)\*/(.+)",O00000O0OO0OO000O ,re .M |re .S )#line:298
+    OOOOO000OO00O0O0O =readSqlstr (OOO00OOO000O00O0O .group (1 ).strip (),para_dict )#line:299
+    O0OO0OO00OO0OO000 =OOO00OOO000O00O0O .group (2 ).strip ()#line:300
+    return OOOOO000OO00O0O0O ,O0OO0OO00OO0OO000 #line:301
+def readSqlstr (OOO0OO0OO0O00OO00 ,para_dict =None ):#line:304
+    OOOOOOOOOO00OOOO0 =re .sub (r"(\/\*(.|\n)*?\*\/)|--.*",'',OOO0OO0OO0O00OO00 .strip ())#line:305
+    if para_dict :#line:306
+        for O0OOO00O000O0O0OO ,O0OOOOO00OOOOO000 in para_dict .items ():#line:307
+            if O0OOO00O000O0O0OO .isnumeric ():#line:308
+                O0O0000O00O0OOO0O =get_dataset (O0OOOOO00OOOOO000 )#line:309
+                print ('dataset:',O0O0000O00O0OOO0O )#line:310
+                if O0O0000O00O0OOO0O['result'] != 'success':
+                    raise SmartpipException(O0O0000O00O0OOO0O['data'])
+                else:
+                    O0O0000O00O0OOO0O = O0O0000O00O0OOO0O['data']
+                if len (O0O0000O00O0OOO0O )>1 :#line:311
+                    for O0000OO00OOOOOOO0 ,O000OO000OOO00OO0 in zip (O0O0000O00O0OOO0O [0 ],O0O0000O00O0OOO0O [1 ]):#line:312
+                        OOOOOOOOOO00OOOO0 =OOOOOOOOOO00OOOO0 .replace ('$'+O0000OO00OOOOOOO0 ,str (O000OO000OOO00OO0 ))#line:313
+            elif callable (O0OOOOO00OOOOO000 ):#line:314
+                OOOO0OO0OOO0OO00O =O0OOOOO00OOOOO000 ()#line:315
+                for O0000OO00OOOOOOO0 ,O000OO000OOO00OO0 in OOOO0OO0OOO0OO00O .items ():#line:316
+                    OOOOOOOOOO00OOOO0 =OOOOOOOOOO00OOOO0 .replace ('$'+O0000OO00OOOOOOO0 ,str (O000OO000OOO00OO0 ))#line:317
+            else :#line:318
+                OOOOOOOOOO00OOOO0 =OOOOOOOOOO00OOOO0 .replace ('$'+O0OOO00O000O0O0OO ,str (O0OOOOO00OOOOO000 ))#line:319
+    return OOOOOOOOOO00OOOO0 #line:320
+def run_sql_file (OO0O0O00OOOOO0OO0 ,OO000000000O0O0O0 ,db_connect ='starrocks',para_dict =None ,dev =''):#line:323
+    O0O0000O0OO00OOO0 =OO0O0O00OOOOO0OO0 .split ('/')#line:324
+    try :#line:325
+        OOOO0OO00OO0OOOO0 =readSqlFile (OO0O0O00OOOOO0OO0 ,para_dict ).split (';')#line:326
+        OOO00O00OO0OOOOOO =OO000000000O0O0O0 .get (db_connect )#line:327
+        if dev :#line:328
+            if f'{db_connect}{dev}'in OO000000000O0O0O0 .keys ():#line:329
+                OOO00O00OO0OOOOOO =OO000000000O0O0O0 .get (f'{db_connect}{dev}')#line:330
+        OOOO0O00000O0O0O0 =connect_db_execute ().execute_sql_list (OOOO0OO00OO0OOOO0 ,db_connect ,connect_dict =OOO00O00OO0OOOOOO )#line:331
+        return OOOO0O00000O0O0O0 #line:332
+    except Exception as O00OO00O0000O0000 :#line:333
+        fun_email ('{}/{}执行出错'.format (O0O0000O0OO00OOO0 [-2 ],O0O0000O0OO00OOO0 [-1 ]),str (O00OO00O0000O0000 .args ))#line:334
+        raise SmartpipException (str (O00OO00O0000O0000 .args ))#line:335
+def _O0O00OO0OO00O0O0O (O00OOOO0000000OO0 ,OOO0000OOO00000OO ,db_connect ='starrocks',para_dict =None ,dev =''):#line:338
+    try :#line:339
+        if isinstance (O00OOOO0000000OO0 ,str ):#line:340
+            O00OOOO0000000OO0 =readSqlstr (O00OOOO0000000OO0 ,para_dict ).split (';')#line:341
+        O0OOO0OO0O0O00OOO =OOO0000OOO00000OO .get (db_connect )#line:342
+        if dev :#line:343
+            if f'{db_connect}{dev}'in OOO0000OOO00000OO .keys ():#line:344
+                O0OOO0OO0O0O00OOO =OOO0000OOO00000OO .get (f'{db_connect}{dev}')#line:345
+        O00O00O00OOOOOOOO =connect_db_execute ().execute_sql_list (O00OOOO0000000OO0 ,db_connect ,connect_dict =O0OOO0OO0O0O00OOO )#line:346
+        return O00O00O00OOOOOOOO #line:347
+    except Exception as O0O00000O00O0OOOO :#line:348
+        fun_email ('SQL执行出错',f'{O00OOOO0000000OO0}{O0O00000O00O0OOOO.args}')#line:349
+        raise SmartpipException (str (O0O00000O00O0OOOO .args ))#line:350
+def run_sp (OO0000O0O0O000O0O ,OO0000O000O00OO00 ,db_connect ='oracle',sp_para =None ,dev =''):#line:353
+    try :#line:354
+        OO0OO00O0OO0O0O00 =OO0000O000O00OO00 .get (db_connect )#line:355
+        if dev :#line:356
+            if f'{db_connect}{dev}'in OO0000O000O00OO00 .keys ():#line:357
+                OO0OO00O0OO0O0O00 =OO0000O000O00OO00 .get (f'{db_connect}{dev}')#line:358
+        connect_db_execute ().excute_proc (OO0000O0O0O000O0O ,OO0OO00O0OO0O0O00 ,sp_para )#line:359
+    except Exception as O0OOOOOOOOO0O0OOO :#line:360
+        fun_email ('{}执行出错'.format (OO0000O0O0O000O0O ),str (O0OOOOOOOOO0O0OOO .args ))#line:361
+        raise SmartpipException (str (O0OOOOOOOOO0O0OOO .args ))#line:362
+def run_kettle (OO000OOO0O00OO0O0 ,para_str ='',dev =False ):#line:366
+    ""#line:373
+    O0O0O0OOO0000OOO0 =OO000OOO0O00OO0O0 .split ('/')#line:374
+    print ('kettle job start')#line:375
+    if '.ktr'in OO000OOO0O00OO0O0 :#line:377
+        OO0O000OOO00OO0O0 =f'{KETTLE_HOME}/pan.sh -level=Basic -file={OO000OOO0O00OO0O0}{para_str}'#line:378
+    else :#line:379
+        OO0O000OOO00OO0O0 =f'{KETTLE_HOME}/kitchen.sh -level=Basic -file={OO000OOO0O00OO0O0}{para_str}'#line:380
+    print (OO0O000OOO00OO0O0 )#line:381
+    O0OO0O0O0OOOOOOOO ,O000OOO00O00OO0O0 =run_bash (OO0O000OOO00OO0O0 )#line:385
+    if O000OOO00O00OO0O0 ==0 :#line:386
+        print ('{} 完成数据抽取'.format (str (OO000OOO0O00OO0O0 )))#line:387
+    else :#line:388
+        print ('{} 执行错误'.format (OO000OOO0O00OO0O0 ))#line:389
+        fun_email ('{}/{}出错'.format (O0O0O0OOO0000OOO0 [-2 ],O0O0O0OOO0000OOO0 [-1 ]),str (O0OO0O0O0OOOOOOOO ))#line:390
+        raise SmartpipException ('Run Kettle Error')#line:391
+def hdfsStarrocks (OOO0O0000OOO0000O ,OO0O00OOOO0OO0O00 ,para_dict =None ):#line:395
+    ""#line:399
+    O000OOOOO0O0O00O0 =OOO0O0000OOO0000O .split ('/')#line:400
+    print ('starrocks load job start')#line:401
+    O0O0OO0O00O0OOOO0 ,O00OO0OOO0OOO0O0O =readSqoopFile (OOO0O0000OOO0000O ,para_dict =para_dict )#line:402
+    O0O0OO0O00O0OOOO0 =O0O0OO0O00O0OOOO0 .split ('\n')#line:403
+    OOOOO0OO0000OO000 ={'LABEL':f'{O000OOOOO0O0O00O0[-2]}{O000OOOOO0O0O00O0[-1][:-4]}{int(time.time())}','HDFS':HIVE_HOME }#line:404
+    for O0O00O00000O0OO0O in O0O0OO0O00O0OOOO0 :#line:405
+        OOOO0OO00OO0OO00O =O0O00O00000O0OO0O .find ('=')#line:406
+        if OOOO0OO00OO0OO00O >0 :#line:407
+            OOOOO0OO0000OO000 [O0O00O00000O0OO0O [:OOOO0OO00OO0OO00O ].strip ()]=O0O00O00000O0OO0O [OOOO0OO00OO0OO00O +1 :].strip ()#line:408
+    O0O00OO000OO000OO =OOOOO0OO0000OO000 .get ('sleepTime')#line:410
+    if O0O00OO000OO000OO :#line:411
+        O0O00OO000OO000OO =int (O0O00OO000OO000OO )#line:412
+        if O0O00OO000OO000OO <30 :#line:413
+            O0O00OO000OO000OO =30 #line:414
+    else :#line:415
+        O0O00OO000OO000OO =30 #line:416
+    O000OOOO00O00O0O0 =OOOOO0OO0000OO000 .get ('maxTime')#line:418
+    if O000OOOO00O00O0O0 :#line:419
+        O000OOOO00O00O0O0 =int (O000OOOO00O00O0O0 )#line:420
+        if O000OOOO00O00O0O0 >3600 :#line:421
+            O000OOOO00O00O0O0 =3600 #line:422
+    else :#line:423
+        O000OOOO00O00O0O0 =600 #line:424
+    _O0O00OO0OO00O0O0O (O00OO0OOO0OOO0O0O ,OO0O00OOOO0OO0O00 ,db_connect ='starrocks',para_dict =OOOOO0OO0000OO000 )#line:426
+    time .sleep (O0O00OO000OO000OO )#line:427
+    O00OOO0OO000O000O =f'''show load from {OOOOO0OO0000OO000.get('targetDB')} where label = '{OOOOO0OO0000OO000['LABEL']}' order by CreateTime desc limit 1 '''#line:428
+    OO0OOO0O0O0O00000 ='start to check label'#line:429
+    try :#line:430
+        while True :#line:431
+            OO0OOO0O0O0O00000 =_O0O00OO0OO00O0O0O ([O00OOO0OO000O000O ],OO0O00OOOO0OO0O00 ,db_connect ='starrocks')#line:432
+            print (OO0OOO0O0O0O00000 )#line:433
+            OO00O0OO0O0O0OOO0 =OO0OOO0O0O0O00000 [1 ][2 ]#line:434
+            if OO00O0OO0O0O0OOO0 =='CANCELLED':#line:435
+                raise Exception (f'Starrocks:{OO00O0OO0O0O0OOO0}')#line:436
+            elif OO00O0OO0O0O0OOO0 =='FINISHED':#line:437
+                print ('Load completed')#line:438
+                break #line:439
+            if O000OOOO00O00O0O0 <=0 :#line:440
+                raise Exception ('超时未完成')#line:441
+            else :#line:442
+                time .sleep (O0O00OO000OO000OO )#line:443
+                O000OOOO00O00O0O0 =O000OOOO00O00O0O0 -O0O00OO000OO000OO #line:444
+    except Exception as O0OO00O00OO00O0OO :#line:445
+        print ('{} 执行错误'.format (OOO0O0000OOO0000O ))#line:446
+        fun_email ('{}/{}执行出错'.format (O000OOOOO0O0O00O0 [-2 ],O000OOOOO0O0O00O0 [-1 ]),str (OO0OOO0O0O0O00000 ))#line:447
+        raise SmartpipException (str (O0OO00O00OO00O0OO .args ))#line:448
+def kafkaStarrocks (O000OOO0O0OOOOO00 ,O0O00O0O0O0O0OO0O ,OO0O00000O0O000OO ,O0OOO0O000OOOO000 ,O00OO00O0000O0OO0 ,dev =''):#line:451
+    with open (O000OOO0O0OOOOO00 ,'r',encoding ='utf8')as OO0O0OO0000OO0O00 :#line:452
+        OO0O00O0000000000 =readSqlstr (OO0O0OO0000OO0O00 .read ().strip (),para_dict =O00OO00O0000O0OO0 )#line:453
+    OO0O00O0000000000 =OO0O00O0000000000 .split ('##')#line:454
+    O0OO000000000OO00 ={}#line:455
+    for OOO00OO000O00O00O in OO0O00O0000000000 :#line:456
+        O0OO0OO0OO0OO0O0O =OOO00OO000O00O00O .find ('=')#line:457
+        if O0OO0OO0OO0OO0O0O >0 :#line:458
+            OO000000O0OOO0OOO =OOO00OO000O00O00O [O0OO0OO0OO0OO0O0O +1 :].replace ('\n',' ').strip ()#line:459
+            if OO000000O0OOO0OOO :#line:460
+                O0OO000000000OO00 [OOO00OO000O00O00O [:O0OO0OO0OO0OO0O0O ].strip ()]=OO000000O0OOO0OOO #line:461
+    O00OO0O000O00OO00 =O0OO000000000OO00 .pop ('topic')#line:462
+    OO0OOO00O0O0O000O =O0OO000000000OO00 .pop ('table')#line:463
+    OOOOOO0OO000O000O =O0OO000000000OO00 .keys ()#line:464
+    if 'skipError'in OOOOOO0OO000O000O :#line:465
+        skipError =O0OO000000000OO00 .pop ('skipError')#line:466
+    else :#line:467
+        skipError =None #line:468
+    if 'kafkaConn'in OOOOOO0OO000O000O :#line:469
+        O0O0000O0OOOOO0O0 =O0OO000000000OO00 .pop ('kafkaConn')#line:470
+    else :#line:471
+        O0O0000O0OOOOO0O0 ='default'#line:472
+    if 'offsets'in OOOOOO0OO000O000O :#line:473
+        O0O0O00OOO00OO0O0 =json .loads (O0OO000000000OO00 .pop ('offsets'))#line:474
+    else :#line:475
+        O0O0O00OOO00OO0O0 =None #line:476
+    if 'json_root'in OOOOOO0OO000O000O :#line:477
+        O0O0OOO00OO0OO000 =O0OO000000000OO00 .pop ('json_root')#line:478
+    else :#line:479
+        O0O0OOO00OO0OO000 =None #line:480
+    if 'jsonpaths'in OOOOOO0OO000O000O :#line:481
+        O00000OO0000OOOO0 =O0OO000000000OO00 .get ('jsonpaths')#line:482
+        if not O00000OO0000OOOO0 .startswith ('['):#line:483
+            O00000OO0000OOOO0 =O00000OO0000OOOO0 .split (',')#line:484
+            O00000OO0000OOOO0 =json .dumps (['$.'+O000OOOO0OO00OOOO .strip ()for O000OOOO0OO00OOOO in O00000OO0000OOOO0 ])#line:485
+            O0OO000000000OO00 ['jsonpaths']=O00000OO0000OOOO0 #line:486
+    OO0OOOO00OOOOO0OO =_O00OO000O0O0OO000 (O00OO0O000O00OO00 ,O0O00O0O0O0O0OO0O [O0O0000O0OOOOO0O0 ],O0OOO0O000OOOO000 ,O0O0O00OOO00OO0O0 )#line:487
+    def O0O0OO0O00OO0OOO0 (OO0OO0O00O0O00O0O ):#line:489
+        OO00000O00OO00OO0 =b''#line:490
+        OOO000OO0O0O00O00 =None #line:491
+        if 'format'in OOOOOO0OO000O000O :#line:492
+            for OOO000OO0O0O00O00 in OO0OO0O00O0O00O0O :#line:493
+                O00OO000O0O00O0OO =OOO000OO0O0O00O00 .value #line:494
+                if O0O0OOO00OO0OO000 :#line:495
+                    O00OO000O0O00O0OO =json .loads (O00OO000O0O00O0OO .decode ('utf8'))#line:496
+                    O00OO000O0O00O0OO =json .dumps (O00OO000O0O00O0OO [O0O0OOO00OO0OO000 ]).encode ('utf8')#line:497
+                if O00OO000O0O00O0OO .startswith (b'['):#line:498
+                    OO00000O00OO00OO0 =OO00000O00OO00OO0 +b','+O00OO000O0O00O0OO [1 :-1 ]#line:499
+                else :#line:500
+                    OO00000O00OO00OO0 =OO00000O00OO00OO0 +b','+O00OO000O0O00O0OO #line:501
+                if len (OO00000O00OO00OO0 )>94857600 :#line:502
+                    streamStarrocks (OO0OOO00O0O0O000O ,OO0O00000O0O000OO ,O0OO000000000OO00 ,OO00000O00OO00OO0 ,skipError )#line:503
+                    OO0OOOO00OOOOO0OO .write_offset (OOO000OO0O0O00O00 .partition ,OOO000OO0O0O00O00 .offset +1 )#line:504
+                    OO00000O00OO00OO0 =b''#line:505
+                if OOO000OO0O0O00O00 .offset ==OO0OOOO00OOOOO0OO .end_offset -1 :#line:506
+                    break #line:507
+        else :#line:508
+            for OOO000OO0O0O00O00 in OO0OO0O00O0O00O0O :#line:509
+                O00OO000O0O00O0OO =OOO000OO0O0O00O00 .value #line:510
+                if O0O0OOO00OO0OO000 :#line:511
+                    O00OO000O0O00O0OO =json .loads (O00OO000O0O00O0OO .decode ('utf8'))#line:512
+                    O00OO000O0O00O0OO =json .dumps (O00OO000O0O00O0OO [O0O0OOO00OO0OO000 ]).encode ('utf8')#line:513
+                OO00000O00OO00OO0 =OO00000O00OO00OO0 +b'\n'+O00OO000O0O00O0OO #line:514
+                if len (OO00000O00OO00OO0 )>94857600 :#line:515
+                    streamStarrocks (OO0OOO00O0O0O000O ,OO0O00000O0O000OO ,O0OO000000000OO00 ,OO00000O00OO00OO0 ,skipError )#line:516
+                    OO0OOOO00OOOOO0OO .write_offset (OOO000OO0O0O00O00 .partition ,OOO000OO0O0O00O00 .offset +1 )#line:517
+                    OO00000O00OO00OO0 =b''#line:518
+                if OOO000OO0O0O00O00 .offset ==OO0OOOO00OOOOO0OO .end_offset -1 :#line:519
+                    break #line:520
+        print (OO00000O00OO00OO0 [1 :1000 ])#line:521
+        if OO00000O00OO00OO0 :#line:522
+            streamStarrocks (OO0OOO00O0O0O000O ,OO0O00000O0O000OO ,O0OO000000000OO00 ,OO00000O00OO00OO0 ,skipError )#line:523
+        return OOO000OO0O0O00O00 #line:524
+    OO0OOOO00OOOOO0OO .consumer_topic (O0O0OO0O00OO0OOO0 )#line:526
+def apiStarrocks (OOO00OO0OO00OO0OO ,O00O000OOO0O0000O ,OOOO0OO00O0O00OO0 ,O0O00O0OOOOO0OOO0 ):#line:529
+    with open (OOO00OO0OO00OO0OO ,'r',encoding ='utf8')as O00000O0O0OOO0OOO :#line:530
+        O000O0OO0O0OO00OO =readSqlstr (O00000O0O0OOO0OOO .read ().strip (),para_dict =O0O00O0OOOOO0OOO0 )#line:531
+    O000O0OO0O0OO00OO =O000O0OO0O0OO00OO .split ('##')#line:532
+    O0OO0000O00OO000O ={}#line:533
+    for OO00O0OOOOOOOO0OO in O000O0OO0O0OO00OO :#line:534
+        O0O00OOO0O0O00000 =OO00O0OOOOOOOO0OO .find ('=')#line:535
+        if O0O00OOO0O0O00000 >0 :#line:536
+            O000O000OOO0OO0O0 =OO00O0OOOOOOOO0OO [O0O00OOO0O0O00000 +1 :].replace ('\n',' ').strip ()#line:537
+            if O000O000OOO0OO0O0 :#line:538
+                O0OO0000O00OO000O [OO00O0OOOOOOOO0OO [:O0O00OOO0O0O00000 ].strip ()]=O000O000OOO0OO0O0 #line:539
+    OO0O0O0OOO0000O00 =O0OO0000O00OO000O .pop ('table')#line:540
+    O0O0OO000O0O0O0OO =O0OO0000O00OO000O .keys ()#line:541
+    if 'param'in O0O0OO000O0O0O0OO :#line:542
+        O0O0OO0OO0O0O000O =O0OO0000O00OO000O .pop ('param')#line:543
+    else :#line:544
+        O0O0OO0OO0O0O000O =None #line:545
+    if 'apiConn'in O0O0OO000O0O0O0OO :#line:546
+        OO0OOOOO00OOOOOOO =O0OO0000O00OO000O .pop ('apiConn')#line:547
+    else :#line:548
+        OO0OOOOO00OOOOOOO ='default'#line:549
+    if 'skipError'in O0O0OO000O0O0O0OO :#line:550
+        skipError =O0OO0000O00OO000O .pop ('skipError')#line:551
+    else :#line:552
+        skipError =None #line:553
+    if 'jsonpaths'in O0O0OO000O0O0O0OO :#line:554
+        OO0O000O0O0000OOO =O0OO0000O00OO000O .get ('jsonpaths')#line:555
+        if not OO0O000O0O0000OOO .startswith ('['):#line:556
+            OO0O000O0O0000OOO =OO0O000O0O0000OOO .split (',')#line:557
+            OO0O000O0O0000OOO =json .dumps (['$.'+OOOOOO0000OOOO00O .strip ()for OOOOOO0000OOOO00O in OO0O000O0O0000OOO ])#line:558
+            O0OO0000O00OO000O ['jsonpaths']=OO0O000O0O0000OOO #line:559
+    OO0O000O0O0OO000O =O00O000OOO0O0000O [OO0OOOOO00OOOOOOO ](O0O0OO0OO0O0O000O )#line:560
+    if OO0O000O0O0OO000O :#line:561
+        streamStarrocks (OO0O0O0OOO0000O00 ,OOOO0OO00O0O00OO0 ,O0OO0000O00OO000O ,OO0O000O0O0OO000O ,skipError )#line:562
+    else :#line:563
+        print ('无数据')#line:564
+def streamStarrocks (OO000O0OO0OO0000O ,OO0OOO00OO00O0000 ,OOO000OO0000O0000 ,O00OO00O0000O000O ,skipError =False ):#line:567
+    ""#line:570
+    import base64 ,uuid #line:571
+    O00O0O0OO0OO00OOO ,OO000O0OO0OO0000O =OO000O0OO0OO0000O .split ('.')#line:572
+    O0OO00OOO0O000OO0 =str (base64 .b64encode (f'{OO0OOO00OO00O0000["user"]}:{OO0OOO00OO00O0000["password"]}'.encode ('utf-8')),'utf-8')#line:573
+    O00OO00O0000O000O =O00OO00O0000O000O .strip ()#line:574
+    if O00OO00O0000O000O .startswith (b','):#line:575
+        OOO000OO0000O0000 ['strip_outer_array']='true'#line:576
+        O00OO00O0000O000O =b'['+O00OO00O0000O000O [1 :]+b']'#line:577
+    OO0000OOO0OO00000 ={'Content-Type':'application/json','Authorization':f'Basic {O0OO00OOO0O000OO0}','label':f'{OO000O0OO0OO0000O}{uuid.uuid4()}',**OOO000OO0000O0000 }#line:583
+    OO00O0O0OO0O00O00 =f"{OO0OOO00OO00O0000['url']}/api/{O00O0O0OO0OO00OOO}/{OO000O0OO0OO0000O}/_stream_load"#line:584
+    print ('start loading to starrocks....')#line:585
+    O0OO0OOO000OOO000 =requests .put (OO00O0O0OO0O00O00 ,headers =OO0000OOO0OO00000 ,data =O00OO00O0000O000O ).json ()#line:586
+    print (O0OO0OOO000OOO000 )#line:587
+    if O0OO0OOO000OOO000 ['Status']=='Fail':#line:588
+        if skipError :#line:589
+            print (f'Starrocks Load Error, Skip this offset')#line:590
+        else :#line:591
+            raise SmartpipException ('Starrocks Load Error')#line:592
+def routineStarrocks (O00000000O000OO0O ,OO000000OO0O0O0OO ,flag =''):#line:595
+    O0O000OOOO00000OO =_O0O00OO0OO00O0O0O ([f'SHOW ROUTINE LOAD FOR {OO000000OO0O0O0OO}'],O00000000O000OO0O ,db_connect ='starrocks')#line:596
+    O0O000OOOO00000OO =dict (zip (O0O000OOOO00000OO [0 ],O0O000OOOO00000OO [1 ]))#line:597
+    print ('状态:',O0O000OOOO00000OO ['State'])#line:598
+    print ('统计:',O0O000OOOO00000OO ['Statistic'])#line:599
+    print ('进度:',O0O000OOOO00000OO ['Progress'])#line:600
+    if O0O000OOOO00000OO ['State']!='RUNNING':#line:601
+        print ('ERROR: ',O0O000OOOO00000OO ['ReasonOfStateChanged'])#line:602
+        if not flag :#line:603
+            raise SmartpipException ('Starrocks Routine Load fail')#line:604
+from airflow .utils .session import provide_session #line:610
+@provide_session #line:613
+def point_test (OOO0000O0O000OO00 ,sleeptime ='',maxtime ='',session =None ):#line:614
+    ""#line:621
+    if sleeptime :#line:622
+        sleeptime =int (sleeptime )#line:623
+        sleeptime =sleeptime if sleeptime >60 else 60 #line:624
+    if maxtime :#line:625
+        maxtime =int (maxtime )#line:626
+        maxtime =maxtime if maxtime <60 *60 *2 else 60 *60 *2 #line:627
+    else :#line:628
+        maxtime =0 #line:629
+    try :#line:630
+        O000000OOO0OOOOOO =f"select start_date,state from dag_run where dag_id ='{OOO0000O0O000OO00}' ORDER BY id desc LIMIT 1"#line:631
+        while True :#line:632
+            O0O0OO0OOOO00O000 =session .execute (O000000OOO0OOOOOO ).fetchall ()#line:633
+            if O0O0OO0OOOO00O000 [0 ][1 ]!='success':#line:634
+                if maxtime >0 and O0O0OO0OOOO00O000 [0 ][1 ]!='failed':#line:635
+                    print ('waiting...'+O0O0OO0OOOO00O000 [0 ][1 ])#line:636
+                    time .sleep (sleeptime )#line:637
+                    maxtime =maxtime -sleeptime #line:638
+                else :#line:639
+                    OO000OOOO00000000 =O0O0OO0OOOO00O000 [0 ][0 ].strftime ("%Y-%m-%d %H:%M:%S")#line:640
+                    O0OOO00O0OO0O0OO0 ='所依赖的dag:'+OOO0000O0O000OO00 +',状态为'+O0O0OO0OOOO00O000 [0 ][1 ]+'.其最新的执行时间为'+OO000OOOO00000000 #line:641
+                    fun_email (O0OOO00O0OO0O0OO0 ,'前置DAG任务未成功')#line:642
+                    raise SmartpipException (O0OOO00O0OO0O0OO0 )#line:643
+            else :#line:644
+                print ('success...',O0O0OO0OOOO00O000 )#line:645
+                break #line:646
+    except Exception as OO0OOOO0OO00OOO0O :#line:647
+        raise SmartpipException (str (OO0OOOO0OO00OOO0O .args ))#line:648
+class connect_db_execute ():#line:653
+    def __init__ (O0OO00O0O0O0O00OO ,dev =False ,db =''):#line:654
+        O0OO00O0O0O0O00OO .dev =dev #line:655
+    def insert_contents (O00OO00OO0OOOOO0O ,O000OO000O0O0O00O ,O0OOOOOOOO00OOOOO ,per_in =1000 ,connect_dict =None ):#line:657
+        OOO0000OOO000OO00 =time .time ()#line:658
+        logging .info ('starting to execute insert contents...')#line:659
+        if isinstance (connect_dict ,dict ):#line:660
+            OOOOO00O00OOO000O =connect_dict ['dbtype']#line:661
+        else :#line:662
+            if connect_dict =='':#line:663
+                OOOOO00O00OOO000O ='oracle'#line:664
+            else :#line:665
+                OOOOO00O00OOO000O =connect_dict #line:666
+            connect_dict =None #line:667
+        O0O0O00OO00OOO0O0 =getattr (O00OO00OO0OOOOO0O ,'insert_contents_'+OOOOO00O00OOO000O )#line:668
+        O000000O00OOO0OO0 =O0O0O00OO00OOO0O0 (O000OO000O0O0O00O ,O0OOOOOOOO00OOOOO ,per_in ,connect_dict )#line:669
+        logging .info ('execute insert contents time : {}ms'.format (time .time ()-OOO0000OOO000OO00 ))#line:670
+        return O000000O00OOO0OO0 #line:671
+    def impala (OOOO000O00OOO000O ,O0OO00O0OO0O00000 ,connect_dict =None ):#line:673
+        ""#line:674
+        from impala .dbapi import connect as impala #line:675
+        O0O0OOOO0000OOOO0 =impala (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =int (connect_dict ['port']),auth_mechanism ='PLAIN')#line:682
+        OOO00O0O00OO0O00O =O0O0OOOO0000OOOO0 .cursor ()#line:683
+        OO00O000OOO0000OO =r'^insert\s|^update\s|^truncate\s|^delete\s|^load\s|^refresh\s|^upsert\s'#line:684
+        OO0000OO0O0OOO000 =None #line:685
+        for OOO0OO0000O0OO000 in O0OO00O0OO0O00000 :#line:686
+            print (OOO0OO0000O0OO000 )#line:687
+            OOO0OO0000O0OO000 =OOO0OO0000O0OO000 .strip ()#line:688
+            if not OOO0OO0000O0OO000 :#line:689
+                continue #line:690
+            if re .search (OO00O000OOO0000OO ,OOO0OO0000O0OO000 ,re .I |re .IGNORECASE ):#line:691
+                OOO00O0O00OO0O00O .execute (OOO0OO0000O0OO000 )#line:692
+            else :#line:693
+                OOO00O0O00OO0O00O .execute (OOO0OO0000O0OO000 )#line:694
+                try :#line:695
+                    OO0000OO0O0OOO000 =OOO00O0O00OO0O00O .fetchall ()#line:696
+                except Exception as OOOO000OO00O000OO :#line:697
+                    print (OOOO000OO00O000OO .args )#line:698
+        O0O0OOOO0000OOOO0 .close ()#line:699
+        return OO0000OO0O0OOO000 #line:700
+    def hive (O00OO00OOO0O00O0O ,OO0O0OOOOO000000O ,connect_dict =None ):#line:702
+        ""#line:703
+        from impala .dbapi import connect as impala #line:704
+        OOO000O0OOO0O00O0 =impala (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =int (connect_dict ['port']),auth_mechanism ='PLAIN')#line:711
+        O0O000O0OOO0OOO00 =OOO000O0OOO0O00O0 .cursor ()#line:712
+        O00O0O00O000000OO =r'^insert\s|^update\s|^truncate\s|^delete\s|^load\s'#line:713
+        OO00O00O000000O00 =None #line:714
+        for OOOO00O0O0O00OO00 in OO0O0OOOOO000000O :#line:715
+            OOOO00O0O0O00OO00 =OOOO00O0O0O00OO00 .strip ()#line:716
+            if not OOOO00O0O0O00OO00 :#line:717
+                continue #line:718
+            print (OOOO00O0O0O00OO00 )#line:719
+            if OOOO00O0O0O00OO00 .startswith ('refresh'):#line:720
+                connect_dict ['port']=21050 #line:721
+                O00OO00OOO0O00O0O .impala ([OOOO00O0O0O00OO00 ],connect_dict =connect_dict )#line:722
+            else :#line:723
+                if re .search (O00O0O00O000000OO ,OOOO00O0O0O00OO00 ,re .I |re .IGNORECASE ):#line:724
+                    O0O000O0OOO0OOO00 .execute (OOOO00O0O0O00OO00 )#line:725
+                else :#line:726
+                    O0O000O0OOO0OOO00 .execute (OOOO00O0O0O00OO00 )#line:727
+                    try :#line:728
+                        OO00O00O000000O00 =O0O000O0OOO0OOO00 .fetchall ()#line:729
+                    except Exception as O000000O000O0OOO0 :#line:730
+                        print (O000000O000O0OOO0 .args )#line:731
+        OOO000O0OOO0O00O0 .close ()#line:732
+        return OO00O00O000000O00 #line:733
+    def mysql (OO00OO00000OOO00O ,O0OOO0OO0OOO0OO0O ,connect_dict =None ):#line:735
+        import pymysql #line:736
+        OO000OO0OO0O000O0 =pymysql .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =connect_dict ['port'],database =connect_dict ['db'])#line:743
+        try :#line:744
+            OOOO0O0O0O000000O =OO000OO0OO0O000O0 .cursor ()#line:745
+            OO00000OO00O0O0OO =r'^insert\s|^update\s|^truncate\s|^delete\s|^load\s'#line:746
+            for O0OOOO000O0OOOOOO in O0OOO0OO0OOO0OO0O :#line:747
+                O0OOOO000O0OOOOOO =O0OOOO000O0OOOOOO .strip ()#line:748
+                if not O0OOOO000O0OOOOOO :#line:749
+                    continue #line:750
+                print (O0OOOO000O0OOOOOO )#line:751
+                if re .search (OO00000OO00O0O0OO ,O0OOOO000O0OOOOOO ,re .I |re .IGNORECASE ):#line:752
+                    try :#line:753
+                        OOOO0O0O0O000000O .execute (O0OOOO000O0OOOOOO )#line:754
+                        OO000OO0OO0O000O0 .commit ()#line:755
+                    except Exception as OO0000OOOOOO0O00O :#line:756
+                        OO000OO0OO0O000O0 .rollback ()#line:757
+                        raise OO0000OOOOOO0O00O #line:758
+                else :#line:759
+                    OOOO0O0O0O000000O .execute (O0OOOO000O0OOOOOO )#line:760
+                    O000OOOO0O00OOO00 =OOOO0O0O0O000000O .fetchall ()#line:761
+                    O000OOOO0O00OOO00 =[[OOOO00OOOO000O00O [0 ]for OOOO00OOOO000O00O in OOOO0O0O0O000000O .description ]]+list (O000OOOO0O00OOO00 )#line:762
+                    return O000OOOO0O00OOO00 #line:763
+        except Exception as O0O0OOOOO00000O00 :#line:764
+            raise O0O0OOOOO00000O00 #line:765
+        finally :#line:766
+            OO000OO0OO0O000O0 .close ()#line:767
+    def starrocks (OOOOOO0OO0OO0O0OO ,OO00OO000OO000O0O ,connect_dict =None ):#line:769
+        return OOOOOO0OO0OO0O0OO .mysql (OO00OO000OO000O0O ,connect_dict )#line:770
+    def oracle (O00O0O0OOO0O00OOO ,OOOOOO0O00O0OOO0O ,connect_dict =None ):#line:772
+        import cx_Oracle #line:773
+        OO0000O00OOO00000 ='{}/{}@{}/{}'.format (connect_dict ['user'],connect_dict ['password'],connect_dict ['host'],connect_dict ['db'])#line:778
+        O00O00O0O0O0O0OO0 =cx_Oracle .connect (OO0000O00OOO00000 )#line:779
+        try :#line:780
+            OO000000O0OO0OOO0 =O00O00O0O0O0O0OO0 .cursor ()#line:781
+            OOOO000O0000OOO0O =r'^insert\s|^update\s|^truncate\s|^delete\s|^comment\s'#line:782
+            for O0O0OO0OOO0OOOOO0 in OOOOOO0O00O0OOO0O :#line:783
+                O0O0OO0OOO0OOOOO0 =O0O0OO0OOO0OOOOO0 .strip ()#line:784
+                if not O0O0OO0OOO0OOOOO0 :#line:785
+                    continue #line:786
+                if re .search (OOOO000O0000OOO0O ,O0O0OO0OOO0OOOOO0 ,re .I ):#line:787
+                    try :#line:788
+                        OO000000O0OO0OOO0 .execute (O0O0OO0OOO0OOOOO0 )#line:789
+                        O00O00O0O0O0O0OO0 .commit ()#line:790
+                    except Exception as OOOOOOOO0OOO0O00O :#line:791
+                        if O0O0OO0OOO0OOOOO0 .startswith ('comment'):#line:792
+                            print ('err:',O0O0OO0OOO0OOOOO0 )#line:793
+                            continue #line:794
+                        O00O00O0O0O0O0OO0 .rollback ()#line:795
+                        raise OOOOOOOO0OOO0O00O #line:796
+                else :#line:797
+                    OO000000O0OO0OOO0 .execute (O0O0OO0OOO0OOOOO0 )#line:798
+                    OOO0OOOO0O000OOOO =OO000000O0OO0OOO0 .fetchall ()#line:799
+                    OOO0OOOO0O000OOOO =[[O0OOO000OOO00OOO0 [0 ]for O0OOO000OOO00OOO0 in OO000000O0OO0OOO0 .description ]]+list (OOO0OOOO0O000OOOO )#line:800
+                    return OOO0OOOO0O000OOOO #line:801
+        except Exception as OO000O0O000OOOOO0 :#line:802
+            raise OO000O0O000OOOOO0 #line:803
+        finally :#line:804
+            O00O00O0O0O0O0OO0 .close ()#line:805
+    def gp (O0OO0OO000OO000O0 ,O0O00OOOO00OO000O ,connect_dict =None ):#line:807
+        import psycopg2 #line:808
+        O0OO000O0000OO0O0 =psycopg2 .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =connect_dict ['port'],database =connect_dict ['db'])#line:815
+        try :#line:816
+            O000O0O0OOOOOO00O =O0OO000O0000OO0O0 .cursor ()#line:817
+            OOOOOO0OO00OOOO00 =r'^insert\s|^update\s|^truncate\s|^delete\s'#line:818
+            for O00OO00OOOOOOOOO0 in O0O00OOOO00OO000O :#line:819
+                O00OO00OOOOOOOOO0 =O00OO00OOOOOOOOO0 .strip ()#line:820
+                if not O00OO00OOOOOOOOO0 :#line:821
+                    continue #line:822
+                if re .search (OOOOOO0OO00OOOO00 ,O00OO00OOOOOOOOO0 ,re .I |re .IGNORECASE ):#line:823
+                    try :#line:824
+                        O000O0O0OOOOOO00O .execute (O00OO00OOOOOOOOO0 )#line:825
+                        O0OO000O0000OO0O0 .commit ()#line:826
+                    except Exception as O0OOOO0O000O0O000 :#line:827
+                        O0OO000O0000OO0O0 .rollback ()#line:828
+                        raise O0OOOO0O000O0O000 #line:829
+                else :#line:830
+                    O000O0O0OOOOOO00O .execute (O00OO00OOOOOOOOO0 )#line:831
+                    OOO00OO0O00O0O0O0 =O000O0O0OOOOOO00O .fetchall ()#line:832
+                    OOO00OO0O00O0O0O0 =[[OO00O0O0OOO0OO0O0 [0 ]for OO00O0O0OOO0OO0O0 in O000O0O0OOOOOO00O .description ]]+list (OOO00OO0O00O0O0O0 )#line:833
+                    return OOO00OO0O00O0O0O0 #line:834
+        except Exception as OO0O0OO00OOOOO0OO :#line:835
+            raise OO0O0OO00OOOOO0OO #line:836
+        finally :#line:837
+            O0OO000O0000OO0O0 .close ()#line:838
+    def mssql (O00O0OOOO00OO0O00 ,OOO0OO0OO00OO0OOO ,connect_dict =None ):#line:840
+        import pymssql #line:841
+        if connect_dict ['port']:#line:842
+            O00OOOO000000OOOO =pymssql .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],port =int (connect_dict ['port']),database =connect_dict ['db'],charset ="utf8",)#line:850
+        else :#line:851
+            O00OOOO000000OOOO =pymssql .connect (user =connect_dict ['user'],password =connect_dict ['password'],host =connect_dict ['host'],database =connect_dict ['db'],charset ="utf8",)#line:858
         try :#line:859
-            OO0000O0OOOOO0O0O =OOO0OOOO0O0O0O000 .cursor ()#line:860
-            print ("开始执行过程:{}  参数: {}".format (O00OO000OO0OOO000 ,proc_para ))#line:861
-            if proc_para is None :#line:862
-                OOOO00000O0OO00O0 =OO0000O0OOOOO0O0O .callproc (O00OO000OO0OOO000 )#line:863
-                OOO0OOOO0O0O0O000 .commit ()#line:864
-            else :#line:865
-                OOOO00000O0OO00O0 =OO0000O0OOOOO0O0O .callproc (O00OO000OO0OOO000 ,proc_para )#line:867
-                OOO0OOOO0O0O0O000 .commit ()#line:868
-            OO0000O0OOOOO0O0O .close ()#line:869
-            OOO0OOOO0O0O0O000 .close ()#line:870
-            print (OOOO00000O0OO00O0 )#line:871
-        except Exception as OOO00O0OOO000O000 :#line:872
-            OOO0OOOO0O0O0O000 .rollback ()#line:873
-            OOO0OOOO0O0O0O000 .close ()#line:874
-            raise OOO00O0OOO000O000 #line:876
-        return True #line:877
-    def insert_contents_oracle (O0O0000OO00OO0O0O ,OOO0000OO00OOO000 ,OOOOOOO0OOOOO00O0 ,per_in =100 ,connect_dict =None ):#line:879
-        import cx_Oracle #line:880
-        OO000O00O0OO00OO0 ='{}/{}@{}:{}/{}'.format (connect_dict ['user'],connect_dict ['password'],connect_dict ['host'],connect_dict ['port'],connect_dict ['db'])#line:886
-        O0O0OO0OO0O0OOO0O =cx_Oracle .connect (OO000O00O0OO00OO0 )#line:887
-        OO0000O0000OO0O00 =O0O0OO0OO0O0OOO0O .cursor ()#line:888
-        O00OO0000O00OO00O =' into {} values {}'#line:889
-        O0OO00OOOOOOO0000 =''#line:890
-        OOO0O000OOOOOOO00 =len (OOO0000OO00OOO000 )#line:891
-        logging .info ("total {} records need to insert table {}: ".format (OOO0O000OOOOOOO00 ,OOOOOOO0OOOOO00O0 ))#line:892
-        try :#line:893
-            for OO0OO0000O0O0OOOO in range (OOO0O000OOOOOOO00 ):#line:894
-                O0OO00OOOOOOO0000 =O0OO00OOOOOOO0000 +O00OO0000O00OO00O .format (OOOOOOO0OOOOO00O0 ,tuple (OOO0000OO00OOO000 [OO0OO0000O0O0OOOO ]))+'\n'#line:895
-                if (OO0OO0000O0O0OOOO +1 )%per_in ==0 or OO0OO0000O0O0OOOO ==OOO0O000OOOOOOO00 -1 :#line:896
-                    OO0O0O00O00OOOOOO ='insert all '+O0OO00OOOOOOO0000 +'select 1 from dual'#line:897
-                    logging .debug (OO0O0O00O00OOOOOO )#line:898
-                    OO0000O0000OO0O00 .execute (OO0O0O00O00OOOOOO )#line:899
-                    O0O0OO0OO0O0OOO0O .commit ()#line:900
-                    O0OO00OOOOOOO0000 =''#line:901
-            return str (OOO0O000OOOOOOO00 )#line:902
-        except Exception as O0O0O0O000OOO0000 :#line:903
-            try :#line:904
-                O0O0OO0OO0O0OOO0O .rollback ()#line:905
-                OO0000O0000OO0O00 .execute ("delete from {} where UPLOADTIME = '{}'".format (OOOOOOO0OOOOO00O0 ,OOO0000OO00OOO000 [0 ][-1 ]))#line:906
-                O0O0OO0OO0O0OOO0O .commit ()#line:907
-            except Exception :#line:908
-                logging .error ('can not delete by uploadtime')#line:909
-            finally :#line:910
-                raise O0O0O0O000OOO0000 #line:911
-        finally :#line:912
-            O0O0OO0OO0O0OOO0O .close ()#line:913
-class _OO00O0OOO000O00O0 (object ):#line:917
-    connect =None #line:918
-    def __init__ (OO0OOO00O0O0OOOOO ,O00OOOO00000OO000 ,O00OO0OO00OO0O000 ,OOO00O00O0OOO0000 ,offsets =None ):#line:920
-        OO0OOO00O0O0OOOOO .end_offset =None #line:921
-        OO0OOO00O0O0OOOOO .db_err_count =0 #line:922
-        OO0OOO00O0O0OOOOO .topic =O00OOOO00000OO000 #line:923
-        OO0OOO00O0O0OOOOO .kafkaconfig =O00OO0OO00OO0O000 #line:924
-        OO0OOO00O0O0OOOOO .offsetDict ={}#line:925
-        OO0OOO00O0O0OOOOO .current_dir =OOO00O00O0OOO0000 #line:926
-        OO0OOO00O0O0OOOOO .offsets =offsets #line:927
-        try :#line:928
-            OO0OOO00O0O0OOOOO .consumer =OO0OOO00O0O0OOOOO .connect_kafka_customer ()#line:929
-        except Exception as OO00OO0O0OOO0O00O :#line:930
-            OO00OO0O0OOO0O00O ='kafka无法连接','ErrLocation：{}\n'.format (O00OOOO00000OO000 )+str (OO00OO0O0OOO0O00O )+',kafka消费者无法创建'#line:931
-            raise OO00OO0O0OOO0O00O #line:932
-    def get_toggle_or_offset (OO0O0O0OOOO00OO0O ,OO0O000OOOOO00O0O ,O0000OOOOOO0O0O0O ):#line:934
-        ""#line:935
-        if OO0O0O0OOOO00OO0O .offsets :#line:936
-            if isinstance (OO0O0O0OOOO00OO0O .offsets ,int ):#line:937
-                return OO0O0O0OOOO00OO0O .offsets #line:938
-            else :#line:939
-                O0O0O00OOO00OOOOO =OO0O0O0OOOO00OO0O .offsets .get (str (O0000OOOOOO0O0O0O ))#line:940
-                if O0O0O00OOO00OOOOO is not None :#line:941
-                    return int(O0O0O00OOO00OOOOO) #line:942
-        O0O0O00OOO00OOOOO =0 #line:943
-        try :#line:944
-            OOO0O0000O0O000OO =f"{OO0O0O0OOOO00OO0O.current_dir}/kafka/{OO0O000OOOOO00O0O}_offset_{O0000OOOOOO0O0O0O}.txt"#line:945
-            if os .path .exists (OOO0O0000O0O000OO ):#line:946
-                O000O0O0O000OOOO0 =open (OOO0O0000O0O000OO ).read ()#line:947
-                if O000O0O0O000OOOO0 :#line:948
-                    O0O0O00OOO00OOOOO =int (O000O0O0O000OOOO0 )#line:949
-            else :#line:950
-                with open (OOO0O0000O0O000OO ,encoding ='utf-8',mode ='a')as O0OO0O0OO000O0O0O :#line:951
-                    O0OO0O0OO000O0O0O .close ()#line:952
-        except Exception as OO000OOOO0OOO0OOO :#line:953
-            print (f"读取失败：{OO000OOOO0OOO0OOO}")#line:954
-            raise OO000OOOO0OOO0OOO #line:955
-        return O0O0O00OOO00OOOOO #line:956
-    def write_offset (OOOO0OOO0OOO00000 ,OO0O00OO0O00O00OO ,offset =None ):#line:958
-        ""#line:961
-        if OOOO0OOO0OOO00000 .topic and offset :#line:962
-            OOO0OOO000OO0OO0O =f"{OOOO0OOO0OOO00000.current_dir}/kafka/{OOOO0OOO0OOO00000.topic}_offset_{OO0O00OO0O00O00OO}.txt"#line:964
-            try :#line:965
-                with open (OOO0OOO000OO0OO0O ,'w')as OO000O000O0O0OOOO :#line:966
-                    OO000O000O0O0OOOO .write (str (offset ))#line:967
-                    OO000O000O0O0OOOO .close ()#line:968
-            except Exception as OO0O000O0OO0O0O0O :#line:969
-                print (f"写入offset出错：{OO0O000O0OO0O0O0O}")#line:970
-                raise OO0O000O0OO0O0O0O #line:971
-    def connect_kafka_customer (O0OOOO00O0O000O00 ):#line:973
+            O0O0O0OO0O0O00O0O =O00OOOO000000OOOO .cursor ()#line:860
+            O00000OO00OO0000O =r'^insert\s|^update\s|^truncate\s|^delete\s'#line:861
+            for O0OO00OO0O000O0O0 in OOO0OO0OO00OO0OOO :#line:862
+                O0OO00OO0O000O0O0 =O0OO00OO0O000O0O0 .strip ()#line:863
+                if not O0OO00OO0O000O0O0 :#line:864
+                    continue #line:865
+                if re .search (O00000OO00OO0000O ,O0OO00OO0O000O0O0 ,re .I |re .IGNORECASE ):#line:866
+                    try :#line:867
+                        O0O0O0OO0O0O00O0O .execute (O0OO00OO0O000O0O0 )#line:868
+                        O00OOOO000000OOOO .commit ()#line:869
+                    except Exception as O00O0O00O000O0000 :#line:870
+                        O00OOOO000000OOOO .rollback ()#line:871
+                        raise O00O0O00O000O0000 #line:872
+                else :#line:873
+                    O0O0O0OO0O0O00O0O .execute (O0OO00OO0O000O0O0 )#line:874
+                    O0OO0OOOOO000O0O0 =O0O0O0OO0O0O00O0O .fetchall ()#line:875
+                    O0OO0OOOOO000O0O0 =[[O00OOO00000000000 [0 ]for O00OOO00000000000 in O0O0O0OO0O0O00O0O .description ]]+list (O0OO0OOOOO000O0O0 )#line:876
+                    return O0OO0OOOOO000O0O0 #line:877
+        except Exception as OOOOOOOO0OOOOOOO0 :#line:878
+            raise OOOOOOOO0OOOOOOO0 #line:879
+        finally :#line:880
+            O00OOOO000000OOOO .close ()#line:881
+    def execute_sql_list (O0OO00000O000OO0O ,O00OOO0000000O00O ,db_connect ='',connect_dict =None ):#line:883
+        if db_connect =='':db_connect ='oracle'#line:884
+        O0O000O00O0OOO0OO =getattr (O0OO00000O000OO0O ,db_connect )#line:885
+        return O0O000O00O0OOO0OO (O00OOO0000000O00O ,connect_dict =connect_dict )#line:886
+    def excute_proc (OOOOOOOO00O00OO00 ,O00O0OO00O0O00OOO ,OOOO0O0OOO00O0O0O ,proc_para =None ):#line:888
+        import cx_Oracle #line:889
+        O00OOO00OOO00O00O ='{}/{}@{}/{}'.format (OOOO0O0OOO00O0O0O ['user'],OOOO0O0OOO00O0O0O ['password'],OOOO0O0OOO00O0O0O ['host'],OOOO0O0OOO00O0O0O ['db'])#line:895
+        OOO0000O000OO0O0O =cx_Oracle .connect (O00OOO00OOO00O00O )#line:896
+        try :#line:898
+            OOOO00O0OOO000OOO =OOO0000O000OO0O0O .cursor ()#line:899
+            print ("开始执行过程:{}  参数: {}".format (O00O0OO00O0O00OOO ,proc_para ))#line:900
+            if proc_para is None :#line:901
+                OO0OOOO00OO000000 =OOOO00O0OOO000OOO .callproc (O00O0OO00O0O00OOO )#line:902
+                OOO0000O000OO0O0O .commit ()#line:903
+            else :#line:904
+                OO0OOOO00OO000000 =OOOO00O0OOO000OOO .callproc (O00O0OO00O0O00OOO ,proc_para )#line:906
+                OOO0000O000OO0O0O .commit ()#line:907
+            OOOO00O0OOO000OOO .close ()#line:908
+            OOO0000O000OO0O0O .close ()#line:909
+            print (OO0OOOO00OO000000 )#line:910
+        except Exception as OO0O00O0O0O00OO0O :#line:911
+            OOO0000O000OO0O0O .rollback ()#line:912
+            OOO0000O000OO0O0O .close ()#line:913
+            raise OO0O00O0O0O00OO0O #line:915
+        return True #line:916
+    def insert_contents_oracle (OO000O000OO0O0O0O ,O00OO00OO0O000O00 ,O00O00OOO00000O0O ,per_in =100 ,connect_dict =None ):#line:918
+        import cx_Oracle #line:919
+        OOO0OOOO0OO0OOO00 ='{}/{}@{}:{}/{}'.format (connect_dict ['user'],connect_dict ['password'],connect_dict ['host'],connect_dict ['port'],connect_dict ['db'])#line:925
+        OOOO00OOOO0000OO0 =cx_Oracle .connect (OOO0OOOO0OO0OOO00 )#line:926
+        O0OO00O0OO0OO0OOO =OOOO00OOOO0000OO0 .cursor ()#line:927
+        O00O00OOOOO00000O =' into {} values {}'#line:928
+        OOO000O00O0O00OO0 =''#line:929
+        O0OO00000OOOO0000 =len (O00OO00OO0O000O00 )#line:930
+        logging .info ("total {} records need to insert table {}: ".format (O0OO00000OOOO0000 ,O00O00OOO00000O0O ))#line:931
+        try :#line:932
+            for O0OOOOOO0O0OOO00O in range (O0OO00000OOOO0000 ):#line:933
+                OOO000O00O0O00OO0 =OOO000O00O0O00OO0 +O00O00OOOOO00000O .format (O00O00OOO00000O0O ,tuple (O00OO00OO0O000O00 [O0OOOOOO0O0OOO00O ]))+'\n'#line:934
+                if (O0OOOOOO0O0OOO00O +1 )%per_in ==0 or O0OOOOOO0O0OOO00O ==O0OO00000OOOO0000 -1 :#line:935
+                    OOOO0O0000O000O0O ='insert all '+OOO000O00O0O00OO0 +'select 1 from dual'#line:936
+                    logging .debug (OOOO0O0000O000O0O )#line:937
+                    O0OO00O0OO0OO0OOO .execute (OOOO0O0000O000O0O )#line:938
+                    OOOO00OOOO0000OO0 .commit ()#line:939
+                    OOO000O00O0O00OO0 =''#line:940
+            return str (O0OO00000OOOO0000 )#line:941
+        except Exception as O000000O00O0O0OO0 :#line:942
+            try :#line:943
+                OOOO00OOOO0000OO0 .rollback ()#line:944
+                O0OO00O0OO0OO0OOO .execute ("delete from {} where UPLOADTIME = '{}'".format (O00O00OOO00000O0O ,O00OO00OO0O000O00 [0 ][-1 ]))#line:945
+                OOOO00OOOO0000OO0 .commit ()#line:946
+            except Exception :#line:947
+                logging .error ('can not delete by uploadtime')#line:948
+            finally :#line:949
+                raise O000000O00O0O0OO0 #line:950
+        finally :#line:951
+            OOOO00OOOO0000OO0 .close ()#line:952
+class _O00OO000O0O0OO000 (object ):#line:956
+    connect =None #line:957
+    def __init__ (OOO000O0000O00OO0 ,O0OOO00O0O0OOO0OO ,O0OO000OO000OOOOO ,O00OO0OOOO0OOO0O0 ,offsets =None ):#line:959
+        OOO000O0000O00OO0 .end_offset =None #line:960
+        OOO000O0000O00OO0 .db_err_count =0 #line:961
+        OOO000O0000O00OO0 .topic =O0OOO00O0O0OOO0OO #line:962
+        OOO000O0000O00OO0 .kafkaconfig =O0OO000OO000OOOOO #line:963
+        OOO000O0000O00OO0 .offsetDict ={}#line:964
+        OOO000O0000O00OO0 .current_dir =O00OO0OOOO0OOO0O0 #line:965
+        OOO000O0000O00OO0 .offsets =offsets #line:966
+        try :#line:967
+            OOO000O0000O00OO0 .consumer =OOO000O0000O00OO0 .connect_kafka_customer ()#line:968
+        except Exception as O0O00OO0O0O0000O0 :#line:969
+            O0O00OO0O0O0000O0 ='kafka无法连接','ErrLocation：{}\n'.format (O0OOO00O0O0OOO0OO )+str (O0O00OO0O0O0000O0 )+',kafka消费者无法创建'#line:970
+            raise O0O00OO0O0O0000O0 #line:971
+    def get_toggle_or_offset (O00O0OO00000O0OO0 ,OOOO0OOO00OO0OOO0 ,O0OOOOO000O0O0O00 ):#line:973
         ""#line:974
-        OO0OO00O000O0O000 =KafkaConsumer (**O0OOOO00O0O000O00 .kafkaconfig )#line:975
-        return OO0OO00O000O0O000 #line:976
-    def parse_data (O0OOO000OO0000000 ,OO0000O000O000O0O ):#line:978
-        ""#line:983
-        return dict ()#line:984
-    def gen_sql (OOO00OOO0O0O00OO0 ,O000OO00O000O0OO0 ):#line:986
-        ""#line:991
-        O0000000OOO0O0000 =[]#line:992
-        for O00OOO0O0OO0OO0OO in O000OO00O000O0OO0 :#line:993
-            O0000000OOO0O0000 .append (str (tuple (O00OOO0O0OO0OO0OO )))#line:995
-        return ','.join (O0000000OOO0O0000 )#line:996
-    def dispose_kafka_data (OO000OO0OO0O000OO ,OO00OOO000O0OO0OO ):#line:998
-        ""#line:1003
-        pass #line:1004
-    def get_now_time (OO000OOOO0O0OOO00 ):#line:1006
-        ""#line:1010
-        O000000O0O0OO0OOO =int (time .time ())#line:1011
-        return time .strftime ('%Y-%m-%d %H:%M:%S',time .localtime (O000000O0O0OO0OOO ))#line:1012
-    def tran_data (O000OOOO000O0OOOO ,O00OOOOOOO00OOOOO ,OOO00O0OOO0OOOO0O ):#line:1014
-        ""#line:1020
-        O0OOOO0000OOO0000 =O00OOOOOOO00OOOOO .get (OOO00O0OOO0OOOO0O ,"")#line:1021
-        O0OOOO0000OOO0000 =""if O0OOOO0000OOO0000 is None else O0OOOO0000OOO0000 #line:1022
-        return str (O0OOOO0000OOO0000 )#line:1023
-    def consumer_data (O00OOOOOOO00000O0 ,OOOO0OOOO0OO00O00 ,O0O00000O0O00O00O ,OO0O000O0O0O0OOO0 ):#line:1025
-        ""#line:1032
-        if O00OOOOOOO00000O0 .consumer :#line:1033
-            O00OOOOOOO00000O0 .consumer .assign ([TopicPartition (topic =O00OOOOOOO00000O0 .topic ,partition =OOOO0OOOO0OO00O00 )])#line:1034
-            O000O0O00O0O00OOO =TopicPartition (topic =O00OOOOOOO00000O0 .topic ,partition =OOOO0OOOO0OO00O00 )#line:1036
-            OOO000O0OO00O0OOO =O00OOOOOOO00000O0 .consumer .beginning_offsets ([O000O0O00O0O00OOO ])#line:1037
-            OO0O0OOO0O0OO0O00 =OOO000O0OO00O0OOO .get (O000O0O00O0O00OOO )#line:1038
-            O000OOO0O00OOO0O0 =O00OOOOOOO00000O0 .consumer .end_offsets ([O000O0O00O0O00OOO ])#line:1039
-            OO0O0OOO00O0000OO =O000OOO0O00OOO0O0 .get (O000O0O00O0O00OOO )#line:1040
-            print (f'建立消费者, {OOOO0OOOO0OO00O00}分区, 最小offset:{OO0O0OOO0O0OO0O00}, 最大offset:{OO0O0OOO00O0000OO}')#line:1041
-            if O0O00000O0O00O00O == -996:
-                O0O00000O0O00O00O = OO0O0OOO00O0000OO - 1
-            if O0O00000O0O00O00O <OO0O0OOO0O0OO0O00 :#line:1042
-                print (f'Warning: 消费offset：{O0O00000O0O00O00O} 小于最小offset:{OO0O0OOO0O0OO0O00}')#line:1043
-                O0O00000O0O00O00O =OO0O0OOO0O0OO0O00 #line:1044
-            if O0O00000O0O00O00O >=OO0O0OOO00O0000OO :#line:1045
-                print (f'消费offset：{O0O00000O0O00O00O} 大于最大offset:{OO0O0OOO00O0000OO}, 本次不消费')#line:1046
-                return #line:1050
-            O00OOOOOOO00000O0 .end_offset =OO0O0OOO00O0000OO #line:1051
-            O00OOOOOOO00000O0 .consumer .seek (TopicPartition (topic =O00OOOOOOO00000O0 .topic ,partition =OOOO0OOOO0OO00O00 ),offset =O0O00000O0O00O00O )#line:1052
-            print (f'消费{OOOO0OOOO0OO00O00}分区, 开始消费offset：{O0O00000O0O00O00O}!')#line:1053
-            O0OOOOO0OO0OO00O0 =OO0O000O0O0O0OOO0 (O00OOOOOOO00000O0 .consumer )#line:1054
-            O0O00000O0O00O00O =O0OOOOO0OO0OO00O0 .offset +1 #line:1055
-            O00OOOOOOO00000O0 .offsetDict [OOOO0OOOO0OO00O00 ]=O0O00000O0O00O00O #line:1058
-            O00OOOOOOO00000O0 .write_offset (OOOO0OOOO0OO00O00 ,O0O00000O0O00O00O )#line:1059
-            O00OOOOOOO00000O0 .offsetDict [OOOO0OOOO0OO00O00 ]=O0O00000O0O00O00O #line:1062
-            O00OOOOOOO00000O0 .write_offset (OOOO0OOOO0OO00O00 ,O0O00000O0O00O00O )#line:1063
-    def consumer_topic (OOO00O0OOOO00OOO0 ,OO00O00OOO0000O0O ):#line:1065
-        print (f"topic: {OOO00O0OOOO00OOO0.topic}")#line:1066
-        print ('开始解析。')#line:1067
-        OO0OOOO000O0O00O0 =OOO00O0OOOO00OOO0 .consumer .partitions_for_topic (topic =OOO00O0OOOO00OOO0 .topic )#line:1069
-        for OO0OOO00OOOOOO00O in OO0OOOO000O0O00O0 :#line:1070
-            O0OOOOOOOO0OOOO0O =OOO00O0OOOO00OOO0 .get_toggle_or_offset (OOO00O0OOOO00OOO0 .topic ,OO0OOO00OOOOOO00O )#line:1071
-            O000O0OOO00OO000O =0 if O0OOOOOOOO0OOOO0O <0 else O0OOOOOOOO0OOOO0O #line:1073
-            OOO00O0OOOO00OOO0 .consumer_data (OO0OOO00OOOOOO00O ,O000O0OOO00OO000O ,OO00O00OOO0000O0O )#line:1074
-    def save_all_offset (O0OOO0OO0O0OO0OOO ):#line:1076
-        for OO00O000OO0OOOOO0 ,O00OO0O000O00OO0O in O0OOO0OO0O0OO0OOO .offsetDict :#line:1077
-            O0OOO0OO0O0OO0OOO .write_offset (OO00O000OO0OOOOO0 ,O00OO0O000O00OO0O )#line:1078
+        if O00O0OO00000O0OO0 .offsets :#line:975
+            if isinstance (O00O0OO00000O0OO0 .offsets ,int ):#line:976
+                return O00O0OO00000O0OO0 .offsets #line:977
+            else :#line:978
+                O00OO00O0O00O000O =O00O0OO00000O0OO0 .offsets .get (str (O0OOOOO000O0O0O00 ))#line:979
+                if O00OO00O0O00O000O is not None :#line:980
+                    return int (O00OO00O0O00O000O )#line:981
+        O00OO00O0O00O000O =0 #line:982
+        try :#line:983
+            O0OOO0O000OO0OOO0 =f"{O00O0OO00000O0OO0.current_dir}/kafka/{OOOO0OOO00OO0OOO0}_offset_{O0OOOOO000O0O0O00}.txt"#line:984
+            if os .path .exists (O0OOO0O000OO0OOO0 ):#line:985
+                OO0OOOO0OO0OOO00O =open (O0OOO0O000OO0OOO0 ).read ()#line:986
+                if OO0OOOO0OO0OOO00O :#line:987
+                    O00OO00O0O00O000O =int (OO0OOOO0OO0OOO00O )#line:988
+            else :#line:989
+                with open (O0OOO0O000OO0OOO0 ,encoding ='utf-8',mode ='a')as O0O0O0O00OOOOOO00 :#line:990
+                    O0O0O0O00OOOOOO00 .close ()#line:991
+        except Exception as OOO0OOOO0O0O00OOO :#line:992
+            print (f"读取失败：{OOO0OOOO0O0O00OOO}")#line:993
+            raise OOO0OOOO0O0O00OOO #line:994
+        return O00OO00O0O00O000O #line:995
+    def write_offset (O00O0OO000OOO000O ,O0OO0000O0OO00O00 ,offset =None ):#line:997
+        ""#line:1000
+        if O00O0OO000OOO000O .topic and offset :#line:1001
+            O0O0O0OO00OOOO00O =f"{O00O0OO000OOO000O.current_dir}/kafka/{O00O0OO000OOO000O.topic}_offset_{O0OO0000O0OO00O00}.txt"#line:1003
+            try :#line:1004
+                with open (O0O0O0OO00OOOO00O ,'w')as OO00OO0O000OOO000 :#line:1005
+                    OO00OO0O000OOO000 .write (str (offset ))#line:1006
+                    OO00OO0O000OOO000 .close ()#line:1007
+            except Exception as O0O00O00000O00O00 :#line:1008
+                print (f"写入offset出错：{O0O00O00000O00O00}")#line:1009
+                raise O0O00O00000O00O00 #line:1010
+    def connect_kafka_customer (OOO0O000000OO0OOO ):#line:1012
+        ""#line:1013
+        OOO0OOO0OOOOO000O =KafkaConsumer (**OOO0O000000OO0OOO .kafkaconfig )#line:1014
+        return OOO0OOO0OOOOO000O #line:1015
+    def parse_data (O000OO0O000O00OOO ,O000O00000OO0O0O0 ):#line:1017
+        ""#line:1022
+        return dict ()#line:1023
+    def gen_sql (OO0OO00OO0000OOOO ,OOO0OO0OOOOOO00OO ):#line:1025
+        ""#line:1030
+        OOO00OOOOO000O0OO =[]#line:1031
+        for O0OO00O0O0O0O00O0 in OOO0OO0OOOOOO00OO :#line:1032
+            OOO00OOOOO000O0OO .append (str (tuple (O0OO00O0O0O0O00O0 )))#line:1034
+        return ','.join (OOO00OOOOO000O0OO )#line:1035
+    def dispose_kafka_data (O0OO0O0000000O00O ,O0O00OOOO0000OOOO ):#line:1037
+        ""#line:1042
+        pass #line:1043
+    def get_now_time (OOOOO0O00O0OOO000 ):#line:1045
+        ""#line:1049
+        O00OOOO000OOOOO00 =int (time .time ())#line:1050
+        return time .strftime ('%Y-%m-%d %H:%M:%S',time .localtime (O00OOOO000OOOOO00 ))#line:1051
+    def tran_data (O00O0OO00OOO0OOO0 ,O0O0000O0000000O0 ,OOO000000000000O0 ):#line:1053
+        ""#line:1059
+        OOO000OOO000OO0O0 =O0O0000O0000000O0 .get (OOO000000000000O0 ,"")#line:1060
+        OOO000OOO000OO0O0 =""if OOO000OOO000OO0O0 is None else OOO000OOO000OO0O0 #line:1061
+        return str (OOO000OOO000OO0O0 )#line:1062
+    def consumer_data (OO000OO00000OO00O ,O0O000O0OO00OOO00 ,OOOO0OO0OOO0OOO0O ,O000O000OO0OO00O0 ):#line:1064
+        ""#line:1071
+        if OO000OO00000OO00O .consumer :#line:1072
+            OO000OO00000OO00O .consumer .assign ([TopicPartition (topic =OO000OO00000OO00O .topic ,partition =O0O000O0OO00OOO00 )])#line:1073
+            O000OO00OOO00000O =TopicPartition (topic =OO000OO00000OO00O .topic ,partition =O0O000O0OO00OOO00 )#line:1075
+            O000O000OO00O0000 =OO000OO00000OO00O .consumer .beginning_offsets ([O000OO00OOO00000O ])#line:1076
+            O0O0OO00O000OOO0O =O000O000OO00O0000 .get (O000OO00OOO00000O )#line:1077
+            O0OOO0O0O0OO00O00 =OO000OO00000OO00O .consumer .end_offsets ([O000OO00OOO00000O ])#line:1078
+            O00OO00000OO0O0O0 =O0OOO0O0O0OO00O00 .get (O000OO00OOO00000O )#line:1079
+            print (f'建立消费者, {O0O000O0OO00OOO00}分区, 最小offset:{O0O0OO00O000OOO0O}, 最大offset:{O00OO00000OO0O0O0}')#line:1080
+            if OOOO0OO0OOO0OOO0O =='-996':#line:1081
+                OOOO0OO0OOO0OOO0O =O0OOO0O0O0OO00O00 -1 #line:1082
+            if OOOO0OO0OOO0OOO0O <O0O0OO00O000OOO0O :#line:1083
+                print (f'Warning: 消费offset：{OOOO0OO0OOO0OOO0O} 小于最小offset:{O0O0OO00O000OOO0O}')#line:1084
+                OOOO0OO0OOO0OOO0O =O0O0OO00O000OOO0O #line:1085
+            if OOOO0OO0OOO0OOO0O >=O00OO00000OO0O0O0 :#line:1086
+                print (f'消费offset：{OOOO0OO0OOO0OOO0O} 大于最大offset:{O00OO00000OO0O0O0}, 本次不消费')#line:1087
+                return #line:1088
+            OO000OO00000OO00O .end_offset =O00OO00000OO0O0O0 #line:1089
+            OO000OO00000OO00O .consumer .seek (TopicPartition (topic =OO000OO00000OO00O .topic ,partition =O0O000O0OO00OOO00 ),offset =OOOO0OO0OOO0OOO0O )#line:1090
+            print (f'消费{O0O000O0OO00OOO00}分区, 开始消费offset：{OOOO0OO0OOO0OOO0O}!')#line:1091
+            O000O0O00O000OO00 =O000O000OO0OO00O0 (OO000OO00000OO00O .consumer )#line:1092
+            OOOO0OO0OOO0OOO0O =O000O0O00O000OO00 .offset +1 #line:1093
+            OO000OO00000OO00O .offsetDict [O0O000O0OO00OOO00 ]=OOOO0OO0OOO0OOO0O #line:1096
+            OO000OO00000OO00O .write_offset (O0O000O0OO00OOO00 ,OOOO0OO0OOO0OOO0O )#line:1097
+            OO000OO00000OO00O .offsetDict [O0O000O0OO00OOO00 ]=OOOO0OO0OOO0OOO0O #line:1100
+            OO000OO00000OO00O .write_offset (O0O000O0OO00OOO00 ,OOOO0OO0OOO0OOO0O )#line:1101
+    def consumer_topic (O0000OO0OOOOO000O ,OOO0O00OO0O00O00O ):#line:1103
+        print (f"topic: {O0000OO0OOOOO000O.topic}")#line:1104
+        print ('开始解析。')#line:1105
+        O00OO00OO0OOO0000 =O0000OO0OOOOO000O .consumer .partitions_for_topic (topic =O0000OO0OOOOO000O .topic )#line:1107
+        for O0O0OOO0OOOO00O00 in O00OO00OO0OOO0000 :#line:1108
+            OO00OO0OOO0O00000 =O0000OO0OOOOO000O .get_toggle_or_offset (O0000OO0OOOOO000O .topic ,O0O0OOO0OOOO00O00 )#line:1109
+            O0O0000OO0O000OO0 =0 if OO00OO0OOO0O00000 <0 else OO00OO0OOO0O00000 #line:1111
+            O0000OO0OOOOO000O .consumer_data (O0O0OOO0OOOO00O00 ,O0O0000OO0O000OO0 ,OOO0O00OO0O00O00O )#line:1112
+    def save_all_offset (OO0OO0000OO00O00O ):#line:1114
+        for O0OOO0OO000OO0000 ,O0OO0000OO0000OO0 in OO0OO0000OO00O00O .offsetDict :#line:1115
+            OO0OO0000OO00O00O .write_offset (O0OOO0OO000OO0000 ,O0OO0000OO0000OO0 )#line:1116
```

### Comparing `smartpip2-2.1.9.4/airflow/compat/__init__.py` & `smartpip2-2.1.9.5/airflow/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/compat/functools.py` & `smartpip2-2.1.9.5/airflow/compat/functools.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/__init__.py` & `smartpip2-2.1.9.5/airflow/config_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/airflow_local_settings.py` & `smartpip2-2.1.9.5/airflow/config_templates/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/config.yml` & `smartpip2-2.1.9.5/airflow/config_templates/config.yml`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/config.yml.schema.json` & `smartpip2-2.1.9.5/airflow/config_templates/config.yml.schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/default_airflow.cfg` & `smartpip2-2.1.9.5/airflow/config_templates/default_airflow.cfg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/default_celery.py` & `smartpip2-2.1.9.5/airflow/config_templates/default_celery.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/default_functions.py` & `smartpip2-2.1.9.5/airflow/config_templates/default_functions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/default_test.cfg` & `smartpip2-2.1.9.5/airflow/config_templates/default_test.cfg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/config_templates/default_webserver_config.py` & `smartpip2-2.1.9.5/airflow/config_templates/default_webserver_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/configuration.py` & `smartpip2-2.1.9.5/airflow/configuration.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/dagsetup/config_dagfile.py` & `smartpip2-2.1.9.5/airflow/contrib/dagsetup/config_dagfile.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/dagsetup/dagfile_test.py` & `smartpip2-2.1.9.5/airflow/contrib/dagsetup/dagfile_test.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/dagsetup/gen_airflow_dagfile.py` & `smartpip2-2.1.9.5/airflow/contrib/dagsetup/gen_airflow_dagfile.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_athena_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_athena_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_datasync_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_datasync_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_dynamodb_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_dynamodb_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_firehose_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_firehose_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_glue_catalog_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_glue_catalog_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_lambda_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_lambda_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_logs_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_logs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sns_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_sns_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sqs_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/aws_sqs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_instance_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/azure_container_instance_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_registry_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/azure_container_registry_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_volume_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/azure_container_volume_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_cosmos_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/azure_cosmos_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_data_lake_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/azure_data_lake_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_fileshare_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/azure_fileshare_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/bigquery_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/bigquery_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/cassandra_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/cassandra_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/cloudant_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/cloudant_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/databricks_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/databricks_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/datadog_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/datadog_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/datastore_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/datastore_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/dingding_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/dingding_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/discord_webhook_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/discord_webhook_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/emr_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/emr_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/fs_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/fs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/ftp_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/ftp_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_api_base_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_api_base_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_bigtable_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_bigtable_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_cloud_build_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_cloud_build_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_compute_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_compute_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_container_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_container_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataflow_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_dataflow_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataproc_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_dataproc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dlp_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_dlp_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_function_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_function_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_kms_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_kms_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_mlengine_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_mlengine_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_natural_language_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_natural_language_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_pubsub_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_pubsub_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_spanner_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_spanner_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_speech_to_text_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_speech_to_text_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_sql_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_sql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_tasks_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_tasks_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_text_to_speech_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_text_to_speech_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_transfer_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_transfer_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_translate_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_translate_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_video_intelligence_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_video_intelligence_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_vision_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcp_vision_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gcs_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gcs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/gdrive_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/gdrive_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/grpc_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/grpc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/imap_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/imap_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/jenkins_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/jenkins_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/jira_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/jira_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/mongo_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/mongo_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/openfaas_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/openfaas_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/opsgenie_alert_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/opsgenie_alert_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/pagerduty_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/pagerduty_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/pinot_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/pinot_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_check_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/qubole_check_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/qubole_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/redis_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/redis_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/redshift_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/redshift_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/sagemaker_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/sagemaker_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/salesforce_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/salesforce_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/segment_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/segment_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/sftp_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/sftp_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/slack_webhook_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/slack_webhook_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/snowflake_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/snowflake_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/spark_jdbc_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/spark_jdbc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/spark_sql_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/spark_sql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/spark_submit_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/spark_submit_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/sqoop_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/sqoop_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/ssh_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/ssh_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/vertica_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/vertica_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/wasb_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/wasb_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/hooks/winrm_hook.py` & `smartpip2-2.1.9.5/airflow/contrib/hooks/winrm_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/adls_list_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/adls_list_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/adls_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/adls_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/aws_athena_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/aws_athena_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/aws_sqs_publish_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/aws_sqs_publish_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/awsbatch_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/awsbatch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/azure_container_instances_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/azure_container_instances_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/azure_cosmos_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/azure_cosmos_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_check_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_get_data.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_get_data.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_table_delete_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_table_delete_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_bigquery.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_mysql_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/bigquery_to_mysql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/cassandra_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/cassandra_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/databricks_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/databricks_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/dataflow_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/dataflow_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/dataproc_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/dataproc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/datastore_export_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/datastore_export_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/datastore_import_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/datastore_import_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/dingding_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/dingding_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/discord_webhook_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/discord_webhook_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/docker_swarm_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/docker_swarm_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/druid_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/druid_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/dynamodb_to_s3.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/ecs_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/ecs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/emr_add_steps_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/emr_add_steps_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/emr_create_job_flow_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/emr_create_job_flow_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/emr_terminate_job_flow_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/emr_terminate_job_flow_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/file_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/file_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/file_to_wasb.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/file_to_wasb.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_bigtable_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_bigtable_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_cloud_build_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_cloud_build_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_compute_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_compute_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_container_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_container_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_dlp_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_dlp_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_function_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_function_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_natural_language_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_natural_language_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_spanner_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_spanner_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_speech_to_text_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_speech_to_text_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_sql_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_sql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_tasks_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_tasks_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_text_to_speech_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_text_to_speech_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_transfer_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_transfer_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_translate_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_speech_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_translate_speech_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_video_intelligence_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_video_intelligence_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_vision_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcp_vision_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_acl_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_acl_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_delete_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_delete_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_download_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_download_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_list_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_list_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_bq.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_bq.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gdrive_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_gdrive_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_s3.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/grpc_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/grpc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/hive_to_dynamodb.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/imap_attachment_to_s3_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/imap_attachment_to_s3_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/jenkins_job_trigger_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/jenkins_job_trigger_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/jira_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/jira_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/kubernetes_pod_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/kubernetes_pod_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/mlengine_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/mlengine_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/mongo_to_s3.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/mssql_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/mssql_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/mysql_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/mysql_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/opsgenie_alert_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/opsgenie_alert_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_oracle_transfer.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/oracle_to_oracle_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/postgres_to_gcs_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/postgres_to_gcs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/pubsub_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/pubsub_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/qubole_check_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/qubole_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/qubole_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/qubole_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/redis_publish_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/redis_publish_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/s3_copy_object_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/s3_copy_object_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/s3_delete_objects_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/s3_delete_objects_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/s3_list_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/s3_list_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/s3_to_gcs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_transfer_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/s3_to_gcs_transfer_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_sftp_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/s3_to_sftp_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_base_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_base_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_config_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_endpoint_config_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_endpoint_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_model_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_model_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_training_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_training_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_transform_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_transform_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_tuning_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sagemaker_tuning_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/segment_track_event_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/segment_track_event_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sftp_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sftp_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sftp_to_s3_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sftp_to_s3_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/slack_webhook_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/slack_webhook_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/snowflake_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/snowflake_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sns_publish_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sns_publish_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/spark_jdbc_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/spark_jdbc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/spark_sql_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/spark_sql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/spark_submit_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/spark_submit_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sql_to_gcs.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sql_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/sqoop_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/sqoop_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/ssh_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/ssh_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/vertica_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/vertica_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_hive.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/vertica_to_hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_mysql.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/wasb_delete_blob_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/wasb_delete_blob_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/operators/winrm_operator.py` & `smartpip2-2.1.9.5/airflow/contrib/operators/winrm_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/secrets/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/secrets/aws_secrets_manager.py` & `smartpip2-2.1.9.5/airflow/contrib/secrets/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/secrets/aws_systems_manager.py` & `smartpip2-2.1.9.5/airflow/contrib/secrets/aws_systems_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/secrets/azure_key_vault.py` & `smartpip2-2.1.9.5/airflow/contrib/secrets/azure_key_vault.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/secrets/gcp_secrets_manager.py` & `smartpip2-2.1.9.5/airflow/contrib/secrets/gcp_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/secrets/hashicorp_vault.py` & `smartpip2-2.1.9.5/airflow/contrib/secrets/hashicorp_vault.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_athena_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/aws_athena_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_redshift_cluster_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/aws_redshift_cluster_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_sqs_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/aws_sqs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/azure_cosmos_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/azure_cosmos_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/bash_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/bash_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/bigquery_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/bigquery_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_record_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/cassandra_record_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_table_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/cassandra_table_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/celery_queue_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/celery_queue_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/datadog_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/datadog_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/emr_base_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/emr_base_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/emr_job_flow_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/emr_job_flow_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/emr_step_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/emr_step_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/file_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/file_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/ftp_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/ftp_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/gcp_transfer_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/gcp_transfer_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/gcs_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/gcs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/hdfs_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/hdfs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/imap_attachment_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/imap_attachment_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/jira_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/jira_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/mongo_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/mongo_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/pubsub_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/pubsub_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/python_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/python_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/qubole_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/qubole_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/redis_key_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/redis_key_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/redis_pub_sub_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/redis_pub_sub_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_base_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_base_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_endpoint_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_endpoint_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_training_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_training_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_transform_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_transform_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_tuning_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/sagemaker_tuning_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/sftp_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/sftp_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/wasb_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/wasb_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/sensors/weekday_sensor.py` & `smartpip2-2.1.9.5/airflow/contrib/sensors/weekday_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/task_runner/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/task_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/task_runner/cgroup_task_runner.py` & `smartpip2-2.1.9.5/airflow/contrib/task_runner/cgroup_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_sanitizer.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/gcp_field_sanitizer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_validator.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/gcp_field_validator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/log/__init__.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/log/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/log/task_handler_with_custom_formatter.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/log/task_handler_with_custom_formatter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_operator_utils.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/mlengine_operator_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_prediction_summary.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/mlengine_prediction_summary.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/sendgrid.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/sendgrid.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/contrib/utils/weekday.py` & `smartpip2-2.1.9.5/airflow/contrib/utils/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/customized_form_field_behaviours.schema.json` & `smartpip2-2.1.9.5/airflow/customized_form_field_behaviours.schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/decorators/__init__.py` & `smartpip2-2.1.9.5/airflow/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/decorators/base.py` & `smartpip2-2.1.9.5/airflow/decorators/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/decorators/python.py` & `smartpip2-2.1.9.5/airflow/decorators/python.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/decorators/python_virtualenv.py` & `smartpip2-2.1.9.5/airflow/decorators/python_virtualenv.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/decorators/task_group.py` & `smartpip2-2.1.9.5/airflow/decorators/task_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/__init__.py` & `smartpip2-2.1.9.5/airflow/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_bash_operator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_bash_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_branch_datetime_operator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_branch_datetime_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_branch_day_of_week_operator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_branch_day_of_week_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_branch_labels.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_branch_labels.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_branch_operator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_branch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_branch_python_dop_operator_3.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_branch_python_dop_operator_3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_complex.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_complex.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_dag_decorator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_dag_decorator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_external_task_marker_dag.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_external_task_marker_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor_config.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_kubernetes_executor_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_latest_only.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_latest_only.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_latest_only_with_trigger.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_latest_only_with_trigger.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_nested_branch_dag.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_nested_branch_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_passing_params_via_test_command.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_passing_params_via_test_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_python_operator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_python_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_short_circuit_operator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_short_circuit_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_skip_dag.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_skip_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_subdag_operator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_subdag_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_task_group.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_task_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_task_group_decorator.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_task_group_decorator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_trigger_controller_dag.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_trigger_controller_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_trigger_target_dag.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_trigger_target_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_xcom.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_xcom.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/example_xcomargs.py` & `smartpip2-2.1.9.5/airflow/example_dags/example_xcomargs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/libs/__init__.py` & `smartpip2-2.1.9.5/airflow/example_dags/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/libs/helper.py` & `smartpip2-2.1.9.5/airflow/example_dags/libs/helper.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/subdags/__init__.py` & `smartpip2-2.1.9.5/airflow/example_dags/subdags/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/subdags/subdag.py` & `smartpip2-2.1.9.5/airflow/example_dags/subdags/subdag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/test_utils.py` & `smartpip2-2.1.9.5/airflow/example_dags/test_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/tutorial.py` & `smartpip2-2.1.9.5/airflow/example_dags/tutorial.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/tutorial_etl_dag.py` & `smartpip2-2.1.9.5/airflow/example_dags/tutorial_etl_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl.py` & `smartpip2-2.1.9.5/airflow/example_dags/tutorial_taskflow_api_etl.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py` & `smartpip2-2.1.9.5/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/exceptions.py` & `smartpip2-2.1.9.5/airflow/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 """Exceptions used by Airflow"""
 from typing import List, NamedTuple, Optional
 
 from airflow.utils.code_utils import prepare_code_snippet
 from airflow.utils.platform import is_tty
 
 
+class SmartpipException(Exception):
+    status_code = 500
+
 class AirflowException(Exception):
     """
     Base class for all Airflow's errors.
     Each custom exception should be derived from this class
     """
 
     status_code = 500
```

### Comparing `smartpip2-2.1.9.4/airflow/executors/__init__.py` & `smartpip2-2.1.9.5/airflow/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/base_executor.py` & `smartpip2-2.1.9.5/airflow/executors/base_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/celery_executor.py` & `smartpip2-2.1.9.5/airflow/executors/celery_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/celery_kubernetes_executor.py` & `smartpip2-2.1.9.5/airflow/executors/celery_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/dask_executor.py` & `smartpip2-2.1.9.5/airflow/executors/dask_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/debug_executor.py` & `smartpip2-2.1.9.5/airflow/executors/debug_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/executor_constants.py` & `smartpip2-2.1.9.5/airflow/executors/executor_constants.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/executor_loader.py` & `smartpip2-2.1.9.5/airflow/executors/executor_loader.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/kubernetes_executor.py` & `smartpip2-2.1.9.5/airflow/executors/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/local_executor.py` & `smartpip2-2.1.9.5/airflow/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/executors/sequential_executor.py` & `smartpip2-2.1.9.5/airflow/executors/sequential_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/S3_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/S3_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/__init__.py` & `smartpip2-2.1.9.5/airflow/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/base.py` & `smartpip2-2.1.9.5/airflow/hooks/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/base_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/base_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/dbapi.py` & `smartpip2-2.1.9.5/airflow/hooks/dbapi.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/dbapi_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/dbapi_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/docker_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/docker_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/druid_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/druid_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/filesystem.py` & `smartpip2-2.1.9.5/airflow/hooks/filesystem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/hdfs_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/hdfs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/hive_hooks.py` & `smartpip2-2.1.9.5/airflow/hooks/hive_hooks.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/http_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/http_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/jdbc_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/jdbc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/mssql_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/mssql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/mysql_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/mysql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/oracle_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/oracle_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/pig_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/pig_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/postgres_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/postgres_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/presto_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/presto_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/samba_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/samba_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/slack_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/slack_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/sqlite_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/sqlite_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/subprocess.py` & `smartpip2-2.1.9.5/airflow/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/webhdfs_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/webhdfs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/hooks/zendesk_hook.py` & `smartpip2-2.1.9.5/airflow/hooks/zendesk_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/jobs/__init__.py` & `smartpip2-2.1.9.5/airflow/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/jobs/backfill_job.py` & `smartpip2-2.1.9.5/airflow/jobs/backfill_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/jobs/base_job.py` & `smartpip2-2.1.9.5/airflow/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/jobs/local_task_job.py` & `smartpip2-2.1.9.5/airflow/jobs/local_task_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/jobs/scheduler_job.py` & `smartpip2-2.1.9.5/airflow/jobs/scheduler_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/__init__.py` & `smartpip2-2.1.9.5/airflow/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/k8s_model.py` & `smartpip2-2.1.9.5/airflow/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/kube_client.py` & `smartpip2-2.1.9.5/airflow/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/kube_config.py` & `smartpip2-2.1.9.5/airflow/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/kubernetes_helper_functions.py` & `smartpip2-2.1.9.5/airflow/kubernetes/kubernetes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/pod.py` & `smartpip2-2.1.9.5/airflow/kubernetes/pod.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/pod_generator.py` & `smartpip2-2.1.9.5/airflow/kubernetes/pod_generator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/pod_generator_deprecated.py` & `smartpip2-2.1.9.5/airflow/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher.py` & `smartpip2-2.1.9.5/airflow/kubernetes/pod_launcher.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher_deprecated.py` & `smartpip2-2.1.9.5/airflow/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/pod_runtime_info_env.py` & `smartpip2-2.1.9.5/airflow/kubernetes/pod_runtime_info_env.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/refresh_config.py` & `smartpip2-2.1.9.5/airflow/kubernetes/refresh_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/secret.py` & `smartpip2-2.1.9.5/airflow/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/volume.py` & `smartpip2-2.1.9.5/airflow/kubernetes/volume.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/kubernetes/volume_mount.py` & `smartpip2-2.1.9.5/airflow/kubernetes/volume_mount.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/lineage/__init__.py` & `smartpip2-2.1.9.5/airflow/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/lineage/backend.py` & `smartpip2-2.1.9.5/airflow/lineage/backend.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/lineage/entities.py` & `smartpip2-2.1.9.5/airflow/lineage/entities.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/logging_config.py` & `smartpip2-2.1.9.5/airflow/logging_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/macros/__init__.py` & `smartpip2-2.1.9.5/airflow/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/macros/hive.py` & `smartpip2-2.1.9.5/airflow/macros/hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/__init__.py` & `smartpip2-2.1.9.5/airflow/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/env.py` & `smartpip2-2.1.9.5/airflow/migrations/env.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/05f30312d566_merge_heads.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/05f30312d566_merge_heads.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/13eb55f81627_for_compatibility.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/13eb55f81627_for_compatibility.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/211e584da130_add_ti_state_index.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/211e584da130_add_ti_state_index.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/2e541a1dcfed_task_duration.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/2e541a1dcfed_task_duration.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/40e67319e3a9_dagrun_config.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/40e67319e3a9_dagrun_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/4446e08588_dagrun_start_end.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/4446e08588_dagrun_start_end.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/502898887f84_adding_extra_to_log.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/502898887f84_adding_extra_to_log.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/52d714495f0_job_id_indices.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/52d714495f0_job_id_indices.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/92c57b58940d_add_fab_tables.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/92c57b58940d_add_fab_tables.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/9635ae0956e7_index_faskfail.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/9635ae0956e7_index_faskfail.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/__init__.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/b0125267960b_merge_heads.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/b0125267960b_merge_heads.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/e3a246e0dc1_current_schema.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/e3a246e0dc1_current_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py` & `smartpip2-2.1.9.5/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/__init__.py` & `smartpip2-2.1.9.5/airflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/base.py` & `smartpip2-2.1.9.5/airflow/models/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/baseoperator.py` & `smartpip2-2.1.9.5/airflow/models/baseoperator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/connection.py` & `smartpip2-2.1.9.5/airflow/models/connection.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/crypto.py` & `smartpip2-2.1.9.5/airflow/models/crypto.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/dag.py` & `smartpip2-2.1.9.5/airflow/models/dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/dagbag.py` & `smartpip2-2.1.9.5/airflow/models/dagbag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/dagcode.py` & `smartpip2-2.1.9.5/airflow/models/dagcode.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/dagparam.py` & `smartpip2-2.1.9.5/airflow/models/dagparam.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/dagpickle.py` & `smartpip2-2.1.9.5/airflow/models/dagpickle.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/dagrun.py` & `smartpip2-2.1.9.5/airflow/models/dagrun.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/errors.py` & `smartpip2-2.1.9.5/airflow/models/errors.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/log.py` & `smartpip2-2.1.9.5/airflow/models/log.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/pool.py` & `smartpip2-2.1.9.5/airflow/models/pool.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/renderedtifields.py` & `smartpip2-2.1.9.5/airflow/models/renderedtifields.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/sensorinstance.py` & `smartpip2-2.1.9.5/airflow/models/sensorinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/serialized_dag.py` & `smartpip2-2.1.9.5/airflow/models/serialized_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/skipmixin.py` & `smartpip2-2.1.9.5/airflow/models/skipmixin.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/slamiss.py` & `smartpip2-2.1.9.5/airflow/models/slamiss.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/taskfail.py` & `smartpip2-2.1.9.5/airflow/models/taskfail.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/taskinstance.py` & `smartpip2-2.1.9.5/airflow/models/taskinstance.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 from airflow.exceptions import (
     AirflowException,
     AirflowFailException,
     AirflowRescheduleException,
     AirflowSkipException,
     AirflowSmartSensorException,
     AirflowTaskTimeout,
+    SmartpipException
 )
 from airflow.models.base import COLLATION_ARGS, ID_LEN, Base
 from airflow.models.log import Log
 from airflow.models.taskfail import TaskFail
 from airflow.models.taskreschedule import TaskReschedule
 from airflow.models.variable import Variable
 from airflow.models.xcom import XCOM_RETURN_KEY, XCom
@@ -1189,14 +1190,18 @@
             # for case when task is marked as success/failed externally
             # current behavior doesn't hit the success callback
             if self.state in {State.SUCCESS, State.FAILED}:
                 return
             else:
                 self.handle_failure(e, test_mode, error_file=error_file)
                 raise
+        except SmartpipException as e:
+            log.error(e)
+            return
+
         except (Exception, KeyboardInterrupt) as e:
             self.handle_failure(e, test_mode, error_file=error_file)
             raise
         finally:
             Stats.incr(f'ti.finish.{task.dag_id}.{task.task_id}.{self.state}')
 
         # Recording SUCCESS
```

### Comparing `smartpip2-2.1.9.4/airflow/models/taskmixin.py` & `smartpip2-2.1.9.5/airflow/models/taskmixin.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/taskreschedule.py` & `smartpip2-2.1.9.5/airflow/models/taskreschedule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/variable.py` & `smartpip2-2.1.9.5/airflow/models/variable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/xcom.py` & `smartpip2-2.1.9.5/airflow/models/xcom.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/models/xcom_arg.py` & `smartpip2-2.1.9.5/airflow/models/xcom_arg.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/mypy/__init__.py` & `smartpip2-2.1.9.5/airflow/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/mypy/plugin/__init__.py` & `smartpip2-2.1.9.5/airflow/mypy/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/mypy/plugin/decorators.py` & `smartpip2-2.1.9.5/airflow/mypy/plugin/decorators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/__init__.py` & `smartpip2-2.1.9.5/airflow/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/bash.py` & `smartpip2-2.1.9.5/airflow/operators/bash.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/bash_operator.py` & `smartpip2-2.1.9.5/airflow/operators/bash_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/branch.py` & `smartpip2-2.1.9.5/airflow/operators/branch.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/branch_operator.py` & `smartpip2-2.1.9.5/airflow/operators/branch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/check_operator.py` & `smartpip2-2.1.9.5/airflow/operators/check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/dagrun_operator.py` & `smartpip2-2.1.9.5/airflow/operators/dagrun_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/datetime.py` & `smartpip2-2.1.9.5/airflow/operators/datetime.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/docker_operator.py` & `smartpip2-2.1.9.5/airflow/operators/docker_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/druid_check_operator.py` & `smartpip2-2.1.9.5/airflow/operators/druid_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/dummy.py` & `smartpip2-2.1.9.5/airflow/operators/dummy.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/dummy_operator.py` & `smartpip2-2.1.9.5/airflow/operators/dummy_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/email.py` & `smartpip2-2.1.9.5/airflow/operators/email.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/email_operator.py` & `smartpip2-2.1.9.5/airflow/operators/email_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/gcs_to_s3.py` & `smartpip2-2.1.9.5/airflow/operators/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/generic_transfer.py` & `smartpip2-2.1.9.5/airflow/operators/generic_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/google_api_to_s3_transfer.py` & `smartpip2-2.1.9.5/airflow/operators/google_api_to_s3_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/hive_operator.py` & `smartpip2-2.1.9.5/airflow/operators/hive_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/hive_stats_operator.py` & `smartpip2-2.1.9.5/airflow/operators/hive_stats_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/hive_to_druid.py` & `smartpip2-2.1.9.5/airflow/operators/hive_to_druid.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/hive_to_mysql.py` & `smartpip2-2.1.9.5/airflow/operators/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/hive_to_samba_operator.py` & `smartpip2-2.1.9.5/airflow/operators/hive_to_samba_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/http_operator.py` & `smartpip2-2.1.9.5/airflow/operators/http_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/jdbc_operator.py` & `smartpip2-2.1.9.5/airflow/operators/jdbc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/latest_only.py` & `smartpip2-2.1.9.5/airflow/operators/latest_only.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/latest_only_operator.py` & `smartpip2-2.1.9.5/airflow/operators/latest_only_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/mssql_operator.py` & `smartpip2-2.1.9.5/airflow/operators/mssql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/mssql_to_hive.py` & `smartpip2-2.1.9.5/airflow/operators/mssql_to_hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/mysql_operator.py` & `smartpip2-2.1.9.5/airflow/operators/mysql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/mysql_to_hive.py` & `smartpip2-2.1.9.5/airflow/operators/mysql_to_hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/oracle_operator.py` & `smartpip2-2.1.9.5/airflow/operators/oracle_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/papermill_operator.py` & `smartpip2-2.1.9.5/airflow/operators/papermill_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/pig_operator.py` & `smartpip2-2.1.9.5/airflow/operators/pig_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/postgres_operator.py` & `smartpip2-2.1.9.5/airflow/operators/postgres_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/presto_check_operator.py` & `smartpip2-2.1.9.5/airflow/operators/presto_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/presto_to_mysql.py` & `smartpip2-2.1.9.5/airflow/operators/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/python.py` & `smartpip2-2.1.9.5/airflow/operators/python.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/python_operator.py` & `smartpip2-2.1.9.5/airflow/operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/redshift_to_s3_operator.py` & `smartpip2-2.1.9.5/airflow/operators/redshift_to_s3_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/s3_file_transform_operator.py` & `smartpip2-2.1.9.5/airflow/operators/s3_file_transform_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/s3_to_hive_operator.py` & `smartpip2-2.1.9.5/airflow/operators/s3_to_hive_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/s3_to_redshift_operator.py` & `smartpip2-2.1.9.5/airflow/operators/s3_to_redshift_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/slack_operator.py` & `smartpip2-2.1.9.5/airflow/operators/slack_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/sql.py` & `smartpip2-2.1.9.5/airflow/operators/sql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/sql_branch_operator.py` & `smartpip2-2.1.9.5/airflow/operators/sql_branch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/sqlite_operator.py` & `smartpip2-2.1.9.5/airflow/operators/sqlite_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/subdag.py` & `smartpip2-2.1.9.5/airflow/operators/subdag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/subdag_operator.py` & `smartpip2-2.1.9.5/airflow/operators/subdag_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/trigger_dagrun.py` & `smartpip2-2.1.9.5/airflow/operators/trigger_dagrun.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/operators/weekday.py` & `smartpip2-2.1.9.5/airflow/operators/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/plugins_manager.py` & `smartpip2-2.1.9.5/airflow/plugins_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/provider_info.schema.json` & `smartpip2-2.1.9.5/airflow/provider_info.schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/providers_manager.py` & `smartpip2-2.1.9.5/airflow/providers_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/secrets/__init__.py` & `smartpip2-2.1.9.5/airflow/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/secrets/base_secrets.py` & `smartpip2-2.1.9.5/airflow/secrets/base_secrets.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/secrets/environment_variables.py` & `smartpip2-2.1.9.5/airflow/secrets/environment_variables.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/secrets/local_filesystem.py` & `smartpip2-2.1.9.5/airflow/secrets/local_filesystem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/secrets/metastore.py` & `smartpip2-2.1.9.5/airflow/secrets/metastore.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/security/__init__.py` & `smartpip2-2.1.9.5/airflow/security/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/security/kerberos.py` & `smartpip2-2.1.9.5/airflow/security/kerberos.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/security/permissions.py` & `smartpip2-2.1.9.5/airflow/security/permissions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/security/utils.py` & `smartpip2-2.1.9.5/airflow/security/utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/__init__.py` & `smartpip2-2.1.9.5/airflow/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/base.py` & `smartpip2-2.1.9.5/airflow/sensors/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/base_sensor_operator.py` & `smartpip2-2.1.9.5/airflow/sensors/base_sensor_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/bash.py` & `smartpip2-2.1.9.5/airflow/sensors/bash.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/date_time.py` & `smartpip2-2.1.9.5/airflow/sensors/date_time.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/date_time_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/date_time_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/external_task.py` & `smartpip2-2.1.9.5/airflow/sensors/external_task.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/external_task_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/filesystem.py` & `smartpip2-2.1.9.5/airflow/sensors/filesystem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/hdfs_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/hdfs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/hive_partition_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/hive_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/http_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/http_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/metastore_partition_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/metastore_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/named_hive_partition_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/named_hive_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/python.py` & `smartpip2-2.1.9.5/airflow/sensors/python.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/s3_key_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/s3_key_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/s3_prefix_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/s3_prefix_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/smart_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/smart_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/sql.py` & `smartpip2-2.1.9.5/airflow/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/sql_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/sql_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/time_delta.py` & `smartpip2-2.1.9.5/airflow/sensors/time_delta.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/time_delta_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/time_delta_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/time_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/time_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/web_hdfs_sensor.py` & `smartpip2-2.1.9.5/airflow/sensors/web_hdfs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sensors/weekday.py` & `smartpip2-2.1.9.5/airflow/sensors/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/sentry.py` & `smartpip2-2.1.9.5/airflow/sentry.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/serialization/__init__.py` & `smartpip2-2.1.9.5/airflow/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/serialization/enums.py` & `smartpip2-2.1.9.5/airflow/serialization/enums.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/serialization/helpers.py` & `smartpip2-2.1.9.5/airflow/serialization/helpers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/serialization/json_schema.py` & `smartpip2-2.1.9.5/airflow/serialization/json_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/serialization/schema.json` & `smartpip2-2.1.9.5/airflow/serialization/schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/serialization/serialized_objects.py` & `smartpip2-2.1.9.5/airflow/serialization/serialized_objects.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/settings.py` & `smartpip2-2.1.9.5/airflow/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,23 @@
         TIMEZONE = pendulum.tz.local_timezone()
     else:
         TIMEZONE = pendulum.tz.timezone(tz)
 except Exception:
     pass
 log.info("Configured default timezone %s", TIMEZONE)
 
-HEADER = '\n'.join(
-    [
-        r'  ____________       _____________',
-        r' ____    |__( )_________  __/__  /________      __',
-        r'____  /| |_  /__  ___/_  /_ __  /_  __ \_ | /| / /',
-        r'___  ___ |  / _  /   _  __/ _  / / /_/ /_ |/ |/ /',
-        r' _/_/  |_/_/  /_/    /_/    /_/  \____/____/|__/',
-        r'smartpip by www.smartchart.cn'
-    ]
-)
+HEADER = r"""
+ _____       ___  ___       ___   _____    _____   _____   _   _____
+/  ___/     /   |/   |     /   | |  _  \  |_   _| |  _  \ | | |  _  \
+| |___     / /|   /| |    / /| | | |_| |    | |   | |_| | | | | |_| |
+\___  \   / / |__/ | |   / / | | |  _  /    | |   |  ___/ | | |  ___/
+ ___| |  / /       | |  / /  | | | | \ \    | |   | |     | | | |
+/_____/ /_/        |_| /_/   |_| |_|  \_\   |_|   |_|     |_| |_|
+smartpip by www.smartchart.cn
+"""
 
 LOGGING_LEVEL = logging.INFO
 
 # the prefix to append to gunicorn worker processes after init
 GUNICORN_WORKER_READY_PREFIX = "[ready] "
 
 LOG_FORMAT = conf.get('logging', 'log_format')
```

### Comparing `smartpip2-2.1.9.4/airflow/smart_sensor_dags/__init__.py` & `smartpip2-2.1.9.5/airflow/smart_sensor_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/smart_sensor_dags/smart_sensor_group.py` & `smartpip2-2.1.9.5/airflow/smart_sensor_dags/smart_sensor_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/stats.py` & `smartpip2-2.1.9.5/airflow/stats.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/task/__init__.py` & `smartpip2-2.1.9.5/airflow/task/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/task/task_runner/__init__.py` & `smartpip2-2.1.9.5/airflow/task/task_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/task/task_runner/base_task_runner.py` & `smartpip2-2.1.9.5/airflow/task/task_runner/base_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/task/task_runner/cgroup_task_runner.py` & `smartpip2-2.1.9.5/airflow/task/task_runner/cgroup_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/task/task_runner/standard_task_runner.py` & `smartpip2-2.1.9.5/airflow/task/task_runner/standard_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/templates.py` & `smartpip2-2.1.9.5/airflow/templates.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/__init__.py` & `smartpip2-2.1.9.5/airflow/ti_deps/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/dep_context.py` & `smartpip2-2.1.9.5/airflow/ti_deps/dep_context.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/dependencies_deps.py` & `smartpip2-2.1.9.5/airflow/ti_deps/dependencies_deps.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/dependencies_states.py` & `smartpip2-2.1.9.5/airflow/ti_deps/dependencies_states.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/__init__.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/base_ti_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/base_ti_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_ti_slots_available_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/dag_ti_slots_available_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_unpaused_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/dag_unpaused_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_exists_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/dagrun_exists_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_id_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/dagrun_id_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/exec_date_after_start_date_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/exec_date_after_start_date_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/not_in_retry_period_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/not_in_retry_period_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/not_previously_skipped_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/not_previously_skipped_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/pool_slots_available_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/pool_slots_available_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/prev_dagrun_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/prev_dagrun_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/ready_to_reschedule.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/ready_to_reschedule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/runnable_exec_date_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/runnable_exec_date_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/task_concurrency_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/task_concurrency_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/task_not_running_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/task_not_running_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/trigger_rule_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/trigger_rule_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/ti_deps/deps/valid_state_dep.py` & `smartpip2-2.1.9.5/airflow/ti_deps/deps/valid_state_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/typing_compat.py` & `smartpip2-2.1.9.5/airflow/typing_compat.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/__init__.py` & `smartpip2-2.1.9.5/airflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/callback_requests.py` & `smartpip2-2.1.9.5/airflow/utils/callback_requests.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/cli.py` & `smartpip2-2.1.9.5/airflow/utils/cli.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/cli_action_loggers.py` & `smartpip2-2.1.9.5/airflow/utils/cli_action_loggers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/code_utils.py` & `smartpip2-2.1.9.5/airflow/utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/compression.py` & `smartpip2-2.1.9.5/airflow/utils/compression.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/configuration.py` & `smartpip2-2.1.9.5/airflow/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/dag_cycle_tester.py` & `smartpip2-2.1.9.5/airflow/utils/dag_cycle_tester.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/dag_processing.py` & `smartpip2-2.1.9.5/airflow/utils/dag_processing.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/dates.py` & `smartpip2-2.1.9.5/airflow/utils/dates.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/db.py` & `smartpip2-2.1.9.5/airflow/utils/db.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/decorators.py` & `smartpip2-2.1.9.5/airflow/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/docs.py` & `smartpip2-2.1.9.5/airflow/utils/docs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/dot_renderer.py` & `smartpip2-2.1.9.5/airflow/utils/dot_renderer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/edgemodifier.py` & `smartpip2-2.1.9.5/airflow/utils/edgemodifier.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/email.py` & `smartpip2-2.1.9.5/airflow/utils/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,34 +173,31 @@
     """Send MIME email."""
     smtp_host = conf.get('smtp', 'SMTP_HOST')
     smtp_port = conf.getint('smtp', 'SMTP_PORT')
     smtp_starttls = conf.getboolean('smtp', 'SMTP_STARTTLS')
     smtp_ssl = conf.getboolean('smtp', 'SMTP_SSL')
     smtp_retry_limit = conf.getint('smtp', 'SMTP_RETRY_LIMIT')
     smtp_timeout = conf.getint('smtp', 'SMTP_TIMEOUT')
-    smtp_user = None
-    smtp_password = None
-
     smtp_user, smtp_password = None, None
     if conn_id is not None:
         try:
             from airflow.hooks.base import BaseHook
 
             conn = BaseHook.get_connection(conn_id)
             smtp_user = conn.login
             smtp_password = conn.password
         except AirflowException:
             pass
     if smtp_user is None or smtp_password is None:
-        warnings.warn(
-            "Fetching SMTP credentials from configuration variables will be deprecated in a future "
-            "release. Please set credentials using a connection instead.",
-            PendingDeprecationWarning,
-            stacklevel=2,
-        )
+        # warnings.warn(
+        #     "Fetching SMTP credentials from configuration variables will be deprecated in a future "
+        #     "release. Please set credentials using a connection instead.",
+        #     PendingDeprecationWarning,
+        #     stacklevel=2,
+        # )
         try:
             smtp_user = conf.get('smtp', 'SMTP_USER')
             smtp_password = conf.get('smtp', 'SMTP_PASSWORD')
         except AirflowConfigException:
             log.debug("No user/password found for SMTP, so logging in with no authentication.")
 
     if not dryrun:
```

### Comparing `smartpip2-2.1.9.4/airflow/utils/entry_points.py` & `smartpip2-2.1.9.5/airflow/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/event_scheduler.py` & `smartpip2-2.1.9.5/airflow/utils/event_scheduler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/file.py` & `smartpip2-2.1.9.5/airflow/utils/file.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/helpers.py` & `smartpip2-2.1.9.5/airflow/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/json.py` & `smartpip2-2.1.9.5/airflow/utils/json.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/__init__.py` & `smartpip2-2.1.9.5/airflow/utils/log/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/cloudwatch_task_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/colored_log.py` & `smartpip2-2.1.9.5/airflow/utils/log/colored_log.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/es_task_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/es_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/file_processor_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/file_processor_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/file_task_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/file_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/gcs_task_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/gcs_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/json_formatter.py` & `smartpip2-2.1.9.5/airflow/utils/log/json_formatter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/log_reader.py` & `smartpip2-2.1.9.5/airflow/utils/log/log_reader.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/logging_mixin.py` & `smartpip2-2.1.9.5/airflow/utils/log/logging_mixin.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/s3_task_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/secrets_masker.py` & `smartpip2-2.1.9.5/airflow/utils/log/secrets_masker.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/stackdriver_task_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/stackdriver_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/task_handler_with_custom_formatter.py` & `smartpip2-2.1.9.5/airflow/utils/log/task_handler_with_custom_formatter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/log/wasb_task_handler.py` & `smartpip2-2.1.9.5/airflow/utils/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/mixins.py` & `smartpip2-2.1.9.5/airflow/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/module_loading.py` & `smartpip2-2.1.9.5/airflow/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/net.py` & `smartpip2-2.1.9.5/airflow/utils/net.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/operator_helpers.py` & `smartpip2-2.1.9.5/airflow/utils/operator_helpers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/operator_resources.py` & `smartpip2-2.1.9.5/airflow/utils/operator_resources.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/orm_event_handlers.py` & `smartpip2-2.1.9.5/airflow/utils/orm_event_handlers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/platform.py` & `smartpip2-2.1.9.5/airflow/utils/platform.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/process_utils.py` & `smartpip2-2.1.9.5/airflow/utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/python_virtualenv.py` & `smartpip2-2.1.9.5/airflow/utils/python_virtualenv.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/python_virtualenv_script.jinja2` & `smartpip2-2.1.9.5/airflow/utils/python_virtualenv_script.jinja2`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/retries.py` & `smartpip2-2.1.9.5/airflow/utils/retries.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/serve_logs.py` & `smartpip2-2.1.9.5/airflow/utils/serve_logs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/session.py` & `smartpip2-2.1.9.5/airflow/utils/session.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/sqlalchemy.py` & `smartpip2-2.1.9.5/airflow/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/state.py` & `smartpip2-2.1.9.5/airflow/utils/state.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/strings.py` & `smartpip2-2.1.9.5/airflow/utils/strings.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/task_group.py` & `smartpip2-2.1.9.5/airflow/utils/task_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/timeout.py` & `smartpip2-2.1.9.5/airflow/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/timezone.py` & `smartpip2-2.1.9.5/airflow/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/trigger_rule.py` & `smartpip2-2.1.9.5/airflow/utils/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/types.py` & `smartpip2-2.1.9.5/airflow/utils/types.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/weekday.py` & `smartpip2-2.1.9.5/airflow/utils/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/weight_rule.py` & `smartpip2-2.1.9.5/airflow/utils/weight_rule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/utils/yaml.py` & `smartpip2-2.1.9.5/airflow/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/version.py` & `smartpip2-2.1.9.5/airflow/version.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/__init__.py` & `smartpip2-2.1.9.5/airflow/www/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/api/__init__.py` & `smartpip2-2.1.9.5/airflow/www/api/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/api/experimental/__init__.py` & `smartpip2-2.1.9.5/airflow/www/api/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/api/experimental/endpoints.py` & `smartpip2-2.1.9.5/airflow/www/api/experimental/endpoints.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/app.py` & `smartpip2-2.1.9.5/airflow/www/app.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/auth.py` & `smartpip2-2.1.9.5/airflow/www/auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/blueprints.py` & `smartpip2-2.1.9.5/airflow/www/blueprints.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/decorators.py` & `smartpip2-2.1.9.5/airflow/www/decorators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/__init__.py` & `smartpip2-2.1.9.5/airflow/www/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_appbuilder.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder_links.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_appbuilder_links.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_dagbag.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_dagbag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_jinja_globals.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_jinja_globals.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_manifest_files.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_manifest_files.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_security.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_session.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_session.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_views.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_views.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/extensions/init_wsgi_middlewares.py` & `smartpip2-2.1.9.5/airflow/www/extensions/init_wsgi_middlewares.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/forms.py` & `smartpip2-2.1.9.5/airflow/www/forms.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/gunicorn_config.py` & `smartpip2-2.1.9.5/airflow/www/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/package.json` & `smartpip2-2.1.9.5/airflow/www/package.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/security.py` & `smartpip2-2.1.9.5/airflow/www/security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/airflow.gif` & `smartpip2-2.1.9.5/airflow/www/static/airflow.gif`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/bootstrap-theme.css` & `smartpip2-2.1.9.5/airflow/www/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/calendar.css` & `smartpip2-2.1.9.5/airflow/www/static/css/calendar.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/dags.css` & `smartpip2-2.1.9.5/airflow/www/static/css/dags.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/flash.css` & `smartpip2-2.1.9.5/airflow/www/static/css/flash.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/gantt.css` & `smartpip2-2.1.9.5/airflow/www/static/css/gantt.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/graph.css` & `smartpip2-2.1.9.5/airflow/www/static/css/graph.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/loading-dots.css` & `smartpip2-2.1.9.5/airflow/www/static/css/loading-dots.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/main.css` & `smartpip2-2.1.9.5/airflow/www/static/css/main.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/material-icons.css` & `smartpip2-2.1.9.5/airflow/www/static/css/material-icons.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/switch.css` & `smartpip2-2.1.9.5/airflow/www/static/css/switch.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/css/tree.css` & `smartpip2-2.1.9.5/airflow/www/static/css/tree.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap3-typeahead.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/bootstrap3-typeahead.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/circles.995e0afd45c3641109e1.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/circles.995e0afd45c3641109e1.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/codemirror.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/codemirror.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/coffeescript-lint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/coffeescript-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/css-lint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/css-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/d3-shape.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/d3-shape.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/d3-tip.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/d3-tip.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/d3.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/d3.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.core.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js.map` & `smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.core.min.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js.map` & `smartpip2-2.1.9.5/airflow/www/static/dist/dagre-d3.min.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/flash.d205b61edc54ed448412.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/flash.d205b61edc54ed448412.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/html-lint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/html-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/ie.e458fc4544c628f16e02.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/ie.e458fc4544c628f16e02.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/javascript-lint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/javascript-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/javascript.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/javascript.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/jquery.dataTables.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/jshint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/jshint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/json-lint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/json-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/lint.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/lint.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/lint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/main.e52cf607b64cdcd15089.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/main.e52cf607b64cdcd15089.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/manifest.json` & `smartpip2-2.1.9.5/airflow/www/static/dist/manifest.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/moment.c1933ee062e9650051f7.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/moment.c1933ee062e9650051f7.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css.map` & `smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.css.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js.map` & `smartpip2-2.1.9.5/airflow/www/static/dist/nv.d3.min.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt` & `smartpip2-2.1.9.5/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.map` & `smartpip2-2.1.9.5/airflow/www/static/dist/redoc.standalone.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/sum.md5` & `smartpip2-2.1.9.5/airflow/www/static/dist/sum.md5`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/switch.e97750fdb7423f33656a.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/switch.e97750fdb7423f33656a.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.css` & `smartpip2-2.1.9.5/airflow/www/static/dist/tree.412f55814f4c1710d907.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/tree.412f55814f4c1710d907.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/dist/yaml-lint.js` & `smartpip2-2.1.9.5/airflow/www/static/dist/yaml-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/calendar.js` & `smartpip2-2.1.9.5/airflow/www/static/js/calendar.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/circles.js` & `smartpip2-2.1.9.5/airflow/www/static/js/circles.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/connection_form.js` & `smartpip2-2.1.9.5/airflow/www/static/js/connection_form.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/dag.js` & `smartpip2-2.1.9.5/airflow/www/static/js/dag.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/dag_code.js` & `smartpip2-2.1.9.5/airflow/www/static/js/dag_code.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/dag_dependencies.js` & `smartpip2-2.1.9.5/airflow/www/static/js/dag_dependencies.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/dags.js` & `smartpip2-2.1.9.5/airflow/www/static/js/dags.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/datetime_utils.js` & `smartpip2-2.1.9.5/airflow/www/static/js/datetime_utils.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/duration_chart.js` & `smartpip2-2.1.9.5/airflow/www/static/js/duration_chart.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/gantt.js` & `smartpip2-2.1.9.5/airflow/www/static/js/gantt.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/graph.js` & `smartpip2-2.1.9.5/airflow/www/static/js/graph.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/ie.js` & `smartpip2-2.1.9.5/airflow/www/static/js/ie.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/main.js` & `smartpip2-2.1.9.5/airflow/www/static/js/main.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/meta_value.js` & `smartpip2-2.1.9.5/airflow/www/static/js/meta_value.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/task_instance.js` & `smartpip2-2.1.9.5/airflow/www/static/js/task_instance.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/task_instances.js` & `smartpip2-2.1.9.5/airflow/www/static/js/task_instances.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/ti_log.js` & `smartpip2-2.1.9.5/airflow/www/static/js/ti_log.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/tree.js` & `smartpip2-2.1.9.5/airflow/www/static/js/tree.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/trigger.js` & `smartpip2-2.1.9.5/airflow/www/static/js/trigger.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/js/variable_edit.js` & `smartpip2-2.1.9.5/airflow/www/static/js/variable_edit.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/loading.gif` & `smartpip2-2.1.9.5/airflow/www/static/loading.gif`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/pin.svg` & `smartpip2-2.1.9.5/airflow/www/static/pin.svg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/pin_100.png` & `smartpip2-2.1.9.5/airflow/www/static/pin_100.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/pin_25.png` & `smartpip2-2.1.9.5/airflow/www/static/pin_25.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/pin_32.png` & `smartpip2-2.1.9.5/airflow/www/static/pin_32.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/pin_35.png` & `smartpip2-2.1.9.5/airflow/www/static/pin_35.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/pin_40.png` & `smartpip2-2.1.9.5/airflow/www/static/pin_40.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/pin_large.png` & `smartpip2-2.1.9.5/airflow/www/static/pin_large.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/screenshots/gantt.png` & `smartpip2-2.1.9.5/airflow/www/static/screenshots/gantt.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/screenshots/graph.png` & `smartpip2-2.1.9.5/airflow/www/static/screenshots/graph.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/static/screenshots/tree.png` & `smartpip2-2.1.9.5/airflow/www/static/screenshots/tree.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/calendar.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/calendar.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/chart.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/chart.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/circles.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/circles.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/code.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/code.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/config.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/config.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/confirm.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/confirm.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_create.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/conn_create.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_edit.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/conn_edit.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/dag.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_code.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/dag_code.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_dependencies.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/dag_dependencies.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_details.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/dag_details.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/dags.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/dags.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/duration_chart.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/duration_chart.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/gantt.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/gantt.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/graph.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/graph.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/main.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/main.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/model_list.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/model_list.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/noaccess.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/noaccess.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/plugin.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/plugin.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/redoc.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/redoc.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/task.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/task.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/task_instance.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/task_instance.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_code.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/ti_code.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_log.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/ti_log.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/traceback.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/traceback.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/tree.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/tree.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/trigger.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/trigger.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_edit.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/variable_edit.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_list.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/variable_list.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/airflow/xcom.html` & `smartpip2-2.1.9.5/airflow/www/templates/airflow/xcom.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/analytics/google_analytics.html` & `smartpip2-2.1.9.5/airflow/www/templates/analytics/google_analytics.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/analytics/metarouter.html` & `smartpip2-2.1.9.5/airflow/www/templates/analytics/metarouter.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/analytics/segment.html` & `smartpip2-2.1.9.5/airflow/www/templates/analytics/segment.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/custom_icons.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/custom_icons.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/dag_docs.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/dag_docs.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/flash.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/flash.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/index.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/index.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/loading_dots.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/loading_dots.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_menu.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/navbar_menu.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_right.html` & `smartpip2-2.1.9.5/airflow/www/templates/appbuilder/navbar_right.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/utils.py` & `smartpip2-2.1.9.5/airflow/www/utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/validators.py` & `smartpip2-2.1.9.5/airflow/www/validators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/views.py` & `smartpip2-2.1.9.5/airflow/www/views.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/webpack.config.js` & `smartpip2-2.1.9.5/airflow/www/webpack.config.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/airflow/www/widgets.py` & `smartpip2-2.1.9.5/airflow/www/widgets.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-bootstrap.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-bootstrap.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-bootstrap3-typeahead.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-bootstrap3-typeahead.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-connexion.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-connexion.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-d3-shape.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-d3-shape.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-d3-tip.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-d3-tip.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-d3js.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-d3js.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-dagre-d3.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-dagre-d3.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-datatables.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-datatables.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-elasticmock.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-elasticmock.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-flask-kerberos.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-flask-kerberos.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-hue.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-hue.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-jqclock.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-jqclock.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-jquery.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-jquery.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-moment-strftime.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-moment-strftime.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-moment.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-moment.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/licenses/LICENSE-normalize.txt` & `smartpip2-2.1.9.5/licenses/LICENSE-normalize.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/README` & `smartpip2-2.1.9.5/scripts/systemd/README`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/airflow` & `smartpip2-2.1.9.5/scripts/systemd/airflow`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/airflow-flower.service` & `smartpip2-2.1.9.5/scripts/systemd/airflow-flower.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/airflow-kerberos.service` & `smartpip2-2.1.9.5/scripts/systemd/airflow-kerberos.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/airflow-scheduler.service` & `smartpip2-2.1.9.5/scripts/systemd/airflow-scheduler.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/airflow-webserver.service` & `smartpip2-2.1.9.5/scripts/systemd/airflow-webserver.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/airflow-worker.service` & `smartpip2-2.1.9.5/scripts/systemd/airflow-worker.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/scripts/systemd/airflow.conf` & `smartpip2-2.1.9.5/scripts/systemd/airflow.conf`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/setup.cfg` & `smartpip2-2.1.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.4/setup.py` & `smartpip2-2.1.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # And it is particularly useful when you add a new provider and there is no
 # PyPI version to install the provider package from
 INSTALL_PROVIDERS_FROM_SOURCES = 'INSTALL_PROVIDERS_FROM_SOURCES'
 PY39 = sys.version_info >= (3, 9)
 
 logger = logging.getLogger(__name__)
 
-version = '2.1.9.4'
+version = '2.1.9.5'
 
 my_dir = dirname(__file__)
 
 
 def airflow_test_suite() -> unittest.TestSuite:
     """Test suite for Airflow tests"""
     test_loader = unittest.TestLoader()
```

### Comparing `smartpip2-2.1.9.4/smartpip2.egg-info/PKG-INFO` & `smartpip2-2.1.9.5/smartpip2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: smartpip2
-Version: 2.1.9.4
+Version: 2.1.9.5
 Summary: Programmatically author, schedule and monitor data pipelines
 Home-page: https://www.smartchart.cn/
 Author: Apache Software Foundation
 Author-email: 84345999@qq.com
 License: Apache License 2.0
-Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.4
+Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.5
 Project-URL: Documentation, https://airflow.apache.org/docs/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Description: <!--
          Licensed to the Apache Software Foundation (ASF) under one
          or more contributor license agreements.  See the NOTICE file
          distributed with this work for additional information
@@ -357,116 +357,116 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: jdbc
-Provides-Extra: statsd
-Provides-Extra: s3
-Provides-Extra: async
-Provides-Extra: cgroups
-Provides-Extra: all
-Provides-Extra: rabbitmq
-Provides-Extra: docker
-Provides-Extra: microsoft.winrm
-Provides-Extra: pagerduty
-Provides-Extra: druid
+Provides-Extra: mongo
+Provides-Extra: zendesk
+Provides-Extra: apache.hive
 Provides-Extra: snowflake
-Provides-Extra: plexus
-Provides-Extra: discord
-Provides-Extra: slack
-Provides-Extra: apache.livy
-Provides-Extra: celery
-Provides-Extra: databricks
 Provides-Extra: devel
 Provides-Extra: webhdfs
-Provides-Extra: kerberos
-Provides-Extra: jira
-Provides-Extra: devel_hadoop
-Provides-Extra: cncf.kubernetes
-Provides-Extra: crypto
-Provides-Extra: microsoft.azure
-Provides-Extra: spark
-Provides-Extra: tableau
-Provides-Extra: cloudant
-Provides-Extra: google
-Provides-Extra: apache.hive
-Provides-Extra: mongo
+Provides-Extra: hive
+Provides-Extra: sendgrid
 Provides-Extra: deprecated_api
+Provides-Extra: discord
+Provides-Extra: devel_all
+Provides-Extra: grpc
+Provides-Extra: apache.spark
+Provides-Extra: kubernetes
+Provides-Extra: all
+Provides-Extra: trino
+Provides-Extra: apache.drill
+Provides-Extra: async
+Provides-Extra: microsoft.winrm
+Provides-Extra: apache.sqoop
 Provides-Extra: openfaas
-Provides-Extra: hdfs
-Provides-Extra: hive
-Provides-Extra: amazon
-Provides-Extra: ldap
-Provides-Extra: presto
-Provides-Extra: qubole
-Provides-Extra: telegram
-Provides-Extra: airbyte
-Provides-Extra: gcp_api
-Provides-Extra: ftp
-Provides-Extra: pinot
-Provides-Extra: mysql
-Provides-Extra: odbc
+Provides-Extra: crypto
+Provides-Extra: docker
+Provides-Extra: qds
 Provides-Extra: salesforce
-Provides-Extra: neo4j
+Provides-Extra: databricks
+Provides-Extra: plexus
+Provides-Extra: celery
+Provides-Extra: kerberos
+Provides-Extra: jenkins
 Provides-Extra: dingding
-Provides-Extra: devel_ci
-Provides-Extra: apache.atlas
-Provides-Extra: hashicorp
+Provides-Extra: telegram
+Provides-Extra: devel_hadoop
+Provides-Extra: all_dbs
+Provides-Extra: sentry
 Provides-Extra: apache.hdfs
-Provides-Extra: mssql
-Provides-Extra: yandex
-Provides-Extra: dask
-Provides-Extra: samba
-Provides-Extra: gcp
-Provides-Extra: imap
-Provides-Extra: jenkins
-Provides-Extra: virtualenv
-Provides-Extra: github_enterprise
-Provides-Extra: segment
-Provides-Extra: devel_all
-Provides-Extra: apache.drill
-Provides-Extra: singularity
 Provides-Extra: aws
-Provides-Extra: postgres
+Provides-Extra: vertica
+Provides-Extra: jdbc
+Provides-Extra: datadog
+Provides-Extra: apache.cassandra
+Provides-Extra: apache.pig
 Provides-Extra: papermill
-Provides-Extra: sendgrid
-Provides-Extra: apache.kylin
+Provides-Extra: exasol
+Provides-Extra: redis
+Provides-Extra: imap
+Provides-Extra: apache.pinot
+Provides-Extra: tableau
+Provides-Extra: apache.atlas
+Provides-Extra: neo4j
+Provides-Extra: presto
+Provides-Extra: password
+Provides-Extra: oracle
+Provides-Extra: azure
+Provides-Extra: jira
 Provides-Extra: opsgenie
+Provides-Extra: gcp
+Provides-Extra: sftp
+Provides-Extra: google
+Provides-Extra: statsd
+Provides-Extra: ftp
+Provides-Extra: druid
+Provides-Extra: singularity
 Provides-Extra: asana
-Provides-Extra: oracle
-Provides-Extra: apache.pinot
-Provides-Extra: exasol
-Provides-Extra: apache.cassandra
-Provides-Extra: doc
-Provides-Extra: microsoft.mssql
-Provides-Extra: atlas
-Provides-Extra: kubernetes
+Provides-Extra: rabbitmq
+Provides-Extra: apache.webhdfs
+Provides-Extra: hashicorp
 Provides-Extra: apache.beam
-Provides-Extra: elasticsearch
-Provides-Extra: redis
-Provides-Extra: vertica
+Provides-Extra: facebook
+Provides-Extra: cgroups
+Provides-Extra: pagerduty
+Provides-Extra: hdfs
+Provides-Extra: microsoft.azure
+Provides-Extra: dask
+Provides-Extra: odbc
+Provides-Extra: postgres
 Provides-Extra: google_auth
-Provides-Extra: sentry
-Provides-Extra: zendesk
-Provides-Extra: apache.sqoop
+Provides-Extra: gcp_api
 Provides-Extra: http
+Provides-Extra: cloudant
+Provides-Extra: slack
+Provides-Extra: spark
+Provides-Extra: elasticsearch
+Provides-Extra: qubole
+Provides-Extra: airbyte
+Provides-Extra: doc
+Provides-Extra: pinot
+Provides-Extra: virtualenv
+Provides-Extra: apache.livy
+Provides-Extra: ldap
+Provides-Extra: samba
+Provides-Extra: cassandra
 Provides-Extra: leveldb
-Provides-Extra: apache.pig
-Provides-Extra: facebook
-Provides-Extra: apache.webhdfs
-Provides-Extra: apache.druid
-Provides-Extra: trino
-Provides-Extra: all_dbs
-Provides-Extra: sftp
+Provides-Extra: s3
+Provides-Extra: github_enterprise
+Provides-Extra: yandex
+Provides-Extra: devel_ci
+Provides-Extra: mssql
 Provides-Extra: winrm
-Provides-Extra: azure
-Provides-Extra: grpc
+Provides-Extra: microsoft.mssql
+Provides-Extra: amazon
 Provides-Extra: sqlite
-Provides-Extra: password
-Provides-Extra: apache.spark
-Provides-Extra: cassandra
-Provides-Extra: qds
-Provides-Extra: datadog
+Provides-Extra: cncf.kubernetes
+Provides-Extra: segment
+Provides-Extra: apache.kylin
+Provides-Extra: mysql
+Provides-Extra: apache.druid
 Provides-Extra: ssh
+Provides-Extra: atlas
```

### Comparing `smartpip2-2.1.9.4/smartpip2.egg-info/SOURCES.txt` & `smartpip2-2.1.9.5/smartpip2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 setup.py
 airflow/__init__.py
 airflow/__main__.py
 airflow/alembic.ini
 airflow/configuration.py
 airflow/customized_form_field_behaviours.schema.json
 airflow/exceptions.py
-airflow/git_version
 airflow/logging_config.py
 airflow/plugins_manager.py
 airflow/provider_info.schema.json
 airflow/providers_manager.py
 airflow/sentry.py
 airflow/settings.py
 airflow/stats.py
```

### Comparing `smartpip2-2.1.9.4/smartpip2.egg-info/requires.txt` & `smartpip2-2.1.9.5/smartpip2.egg-info/requires.txt`

 * *Files identical despite different names*

