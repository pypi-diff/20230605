# Comparing `tmp/quetz-server-0.8.0.tar.gz` & `tmp/quetz-server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quetz-server-0.8.0.tar", last modified: Thu Jun  1 07:34:21 2023, max compression
+gzip compressed data, was "quetz-server-0.9.0.tar", last modified: Mon Jun  5 07:56:40 2023, max compression
```

## Comparing `quetz-server-0.8.0.tar` & `quetz-server-0.9.0.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.390586 quetz-server-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 07:34:02.000000 quetz-server-0.8.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 07:34:02.000000 quetz-server-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 07:34:02.000000 quetz-server-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22389 2023-06-01 07:34:11.000000 quetz-server-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-01 07:34:02.000000 quetz-server-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 07:34:02.000000 quetz-server-0.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-01 07:34:02.000000 quetz-server-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-01 07:34:02.000000 quetz-server-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-01 07:34:21.390586 quetz-server-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-06-01 07:34:02.000000 quetz-server-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 07:34:02.000000 quetz-server-0.8.0/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-01 07:34:02.000000 quetz-server-0.8.0/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-01 07:34:02.000000 quetz-server-0.8.0/dev_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/Dockerfile.jupyterhub
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/docker_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/grafana.env
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/graphana_datasources.yml
--rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/jupyterhub_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/postgres.conf
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/postgres.env
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/prometheus.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/wait-for-postgres.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/assets/quetz_header.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/_static/quetz_favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/_static/quetz_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/source/deploying/
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/authenticators.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/frontend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/migrations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/nginx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/workers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.374586 quetz-server-0.8.0/docs/source/qeps/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/qeps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/qeps/qep-001-user-permissions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.374586 quetz-server-0.8.0/docs/source/using/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/using/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/using/mirroring.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-06-01 07:34:02.000000 quetz-server-0.8.0/download-test-package.sh
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-01 07:34:02.000000 quetz-server-0.8.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-01 07:34:02.000000 quetz-server-0.8.0/init_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-01 07:34:09.000000 quetz-server-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.374586 quetz-server-0.8.0/quetz/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-01 07:34:09.000000 quetz-server-0.8.0/quetz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/jupyterhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/basic_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/basic_frontend/avatar.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/basic_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/basic_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/channel_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/condainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    42862 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/database_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    57621 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/a80fb051a659_create_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/pkgstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/repo_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/rest_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/reindexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/templates/channeldata-index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/templates/subdir-index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/mockups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_main_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/authentification/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.366586 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/other-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/other-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/test-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_pkg_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_versionorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/versionorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz_db_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/LIBSOLV_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/conda.c
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/conda.h
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/quetz_pg.c
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/quetz_sqlite.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.390586 quetz-server-0.8.0/quetz_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-01 07:34:21.390586 quetz-server-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:34:02.000000 quetz-server-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.191593 quetz-server-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 07:56:24.000000 quetz-server-0.9.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-05 07:56:24.000000 quetz-server-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 07:56:24.000000 quetz-server-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23537 2023-06-05 07:56:31.000000 quetz-server-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 07:56:24.000000 quetz-server-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-05 07:56:24.000000 quetz-server-0.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-05 07:56:24.000000 quetz-server-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 07:56:24.000000 quetz-server-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-05 07:56:40.191593 quetz-server-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-06-05 07:56:24.000000 quetz-server-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-05 07:56:24.000000 quetz-server-0.9.0/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-05 07:56:24.000000 quetz-server-0.9.0/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-05 07:56:24.000000 quetz-server-0.9.0/dev_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/Dockerfile.jupyterhub
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/docker_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/grafana.env
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/graphana_datasources.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/jupyterhub_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/postgres.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/postgres.env
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/prometheus.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker/wait-for-postgres.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/assets/quetz_header.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/_static/quetz_favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/_static/quetz_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docs/source/deploying/
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/authenticators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/frontend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/nginx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/deploying/workers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docs/source/qeps/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/qeps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/qeps/qep-001-user-permissions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.175593 quetz-server-0.9.0/docs/source/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/using/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-05 07:56:24.000000 quetz-server-0.9.0/docs/source/using/mirroring.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-06-05 07:56:24.000000 quetz-server-0.9.0/download-test-package.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-05 07:56:24.000000 quetz-server-0.9.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-05 07:56:24.000000 quetz-server-0.9.0/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-05 07:56:29.000000 quetz-server-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.179593 quetz-server-0.9.0/quetz/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 07:56:29.000000 quetz-server-0.9.0/quetz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.179593 quetz-server-0.9.0/quetz/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/jupyterhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authentication/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.179593 quetz-server-0.9.0/quetz/basic_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/basic_frontend/avatar.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/basic_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/basic_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/channel_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/condainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    42862 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/database_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.183593 quetz-server-0.9.0/quetz/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/jobs/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/jobs/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/jobs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/jobs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/jobs/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/jobs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57633 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.183593 quetz-server-0.9.0/quetz/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/metrics/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/metrics/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/metrics/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/metrics/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/metrics/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/metrics/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.183593 quetz-server-0.9.0/quetz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.183593 quetz-server-0.9.0/quetz/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/a80fb051a659_create_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/pkgstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/repo_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/rest_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.187593 quetz-server-0.9.0/quetz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/reindexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tasks/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.187593 quetz-server-0.9.0/quetz/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/templates/channeldata-index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/templates/subdir-index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.187593 quetz-server-0.9.0/quetz/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/testing/mockups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.187593 quetz-server-0.9.0/quetz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.187593 quetz-server-0.9.0/quetz/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/test_main_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.191593 quetz-server-0.9.0/quetz/tests/authentification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/authentification/test_auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/authentification/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/authentification/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/authentification/test_pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.191593 quetz-server-0.9.0/quetz/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.171593 quetz-server-0.9.0/quetz/tests/data/dummy-plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.191593 quetz-server-0.9.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.191593 quetz-server-0.9.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/other-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/other-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/test-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/data/test-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_pkg_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_versionorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/tests/test_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz/versionorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.191593 quetz-server-0.9.0/quetz_db_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz_db_ext/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz_db_ext/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz_db_ext/LIBSOLV_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz_db_ext/conda.c
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz_db_ext/conda.h
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz_db_ext/quetz_pg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-05 07:56:24.000000 quetz-server-0.9.0/quetz_db_ext/quetz_sqlite.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:56:40.191593 quetz-server-0.9.0/quetz_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-05 07:56:40.000000 quetz-server-0.9.0/quetz_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-05 07:56:40.000000 quetz-server-0.9.0/quetz_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:56:40.000000 quetz-server-0.9.0/quetz_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 07:56:40.000000 quetz-server-0.9.0/quetz_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 07:56:40.000000 quetz-server-0.9.0/quetz_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 07:56:40.000000 quetz-server-0.9.0/quetz_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-05 07:56:40.191593 quetz-server-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:56:24.000000 quetz-server-0.9.0/setup.py
```

### Comparing `quetz-server-0.8.0/.pre-commit-config.yaml` & `quetz-server-0.9.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
           - types-orjson
           - types-pkg-resources
           - types-redis
           - types-requests
           - types-six
           - types-toml
           - types-ujson
+          - types-aiofiles
         args: [--show-error-codes]
   - repo: https://github.com/Quantco/pre-commit-mirrors-prettier
     rev: 2.7.1
     hooks:
       - id: prettier-conda
   - repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.294
```

### Comparing `quetz-server-0.8.0/CHANGELOG.md` & `quetz-server-0.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.9.0
+
+([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.8.0...935be5b02961e952396ca1fac20e073ec8907062))
+
+### Enhancements made
+
+- Add async friendly upload [#626](https://github.com/mamba-org/quetz/pull/626) ([@ivergara](https://github.com/ivergara))
+
+### Maintenance and upkeep improvements
+
+- Run CI on main branch [#637](https://github.com/mamba-org/quetz/pull/637) ([@janjagusch](https://github.com/janjagusch))
+- Add GCS env vars [#636](https://github.com/mamba-org/quetz/pull/636) ([@janjagusch](https://github.com/janjagusch))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-06-01&to=2023-06-05&type=c))
+
+[@codecov-commenter](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Acodecov-commenter+updated%3A2023-06-01..2023-06-05&type=Issues) | [@ivergara](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Aivergara+updated%3A2023-06-01..2023-06-05&type=Issues) | [@janjagusch](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Ajanjagusch+updated%3A2023-06-01..2023-06-05&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.8.0
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.7.0...b1ac607ed0900b6242519cd452e92539f83a6721))
 
 ### Enhancements made
 
 - Sanitize DB urls before printing [#633](https://github.com/mamba-org/quetz/pull/633) ([@AndreasAlbertQC](https://github.com/AndreasAlbertQC))
@@ -22,16 +43,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-04-11&to=2023-06-01&type=c))
 
 [@AndreasAlbertQC](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3AAndreasAlbertQC+updated%3A2023-04-11..2023-06-01&type=Issues) | [@codecov-commenter](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Acodecov-commenter+updated%3A2023-04-11..2023-06-01&type=Issues) | [@ivergara](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Aivergara+updated%3A2023-04-11..2023-06-01&type=Issues) | [@janjagusch](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Ajanjagusch+updated%3A2023-04-11..2023-06-01&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3AmartinRenou+updated%3A2023-04-11..2023-06-01&type=Issues) | [@pavelzw](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Apavelzw+updated%3A2023-04-11..2023-06-01&type=Issues) | [@SauravMaheshkar](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3ASauravMaheshkar+updated%3A2023-04-11..2023-06-01&type=Issues) | [@sbivol](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Asbivol+updated%3A2023-04-11..2023-06-01&type=Issues) | [@YYYasin19](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3AYYYasin19+updated%3A2023-04-11..2023-06-01&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.7.0
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.6.3...bc0ac65796d14083ae587eba103d6d60250759ff))
 
 ### Enhancements made
 
 - Add endpoints for health checks [#622](https://github.com/mamba-org/quetz/pull/622) ([@janjagusch](https://github.com/janjagusch))
```

### Comparing `quetz-server-0.8.0/CONTRIBUTING.md` & `quetz-server-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/Dockerfile` & `quetz-server-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/LICENSE` & `quetz-server-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/MANIFEST.in` & `quetz-server-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/PKG-INFO` & `quetz-server-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.8.0
+Version: 0.9.0
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.8.0 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.9.0 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
```

### Comparing `quetz-server-0.8.0/README.md` & `quetz-server-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/RELEASE.md` & `quetz-server-0.9.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/alembic.ini` & `quetz-server-0.9.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/dev_config.toml` & `quetz-server-0.9.0/dev_config.toml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docker/Dockerfile` & `quetz-server-0.9.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docker/docker_config.toml` & `quetz-server-0.9.0/docker/docker_config.toml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docker/jupyterhub_config.py` & `quetz-server-0.9.0/docker/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docker/nginx.conf` & `quetz-server-0.9.0/docker/nginx.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docker/postgres.conf` & `quetz-server-0.9.0/docker/postgres.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docker-compose.yml` & `quetz-server-0.9.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/Makefile` & `quetz-server-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/assets/quetz_header.png` & `quetz-server-0.9.0/docs/assets/quetz_header.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/make.bat` & `quetz-server-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/_static/quetz_favicon.ico` & `quetz-server-0.9.0/docs/source/_static/quetz_favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/_static/quetz_logo.png` & `quetz-server-0.9.0/docs/source/_static/quetz_logo.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/conf.py` & `quetz-server-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/deploying/authenticators.rst` & `quetz-server-0.9.0/docs/source/deploying/authenticators.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/deploying/configuration.rst` & `quetz-server-0.9.0/docs/source/deploying/configuration.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/deploying/database.rst` & `quetz-server-0.9.0/docs/source/deploying/database.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/deploying/migrations.rst` & `quetz-server-0.9.0/docs/source/deploying/migrations.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/deploying/nginx.rst` & `quetz-server-0.9.0/docs/source/deploying/nginx.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/deploying/workers.rst` & `quetz-server-0.9.0/docs/source/deploying/workers.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/index.rst` & `quetz-server-0.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/plugins.rst` & `quetz-server-0.9.0/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/qeps/qep-001-user-permissions.rst` & `quetz-server-0.9.0/docs/source/qeps/qep-001-user-permissions.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/using/basics.rst` & `quetz-server-0.9.0/docs/source/using/basics.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/docs/source/using/mirroring.rst` & `quetz-server-0.9.0/docs/source/using/mirroring.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/environment.yml` & `quetz-server-0.9.0/environment.yml`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,15 @@
   - s3fs
   - gcsfs >=2022.03
   - sphinx
   - sphinx-book-theme>=0.3
   - tenacity
   - xattr
   - aiofiles
+  - aioshutil
   - pyyaml
   - ujson
   - prometheus_client
   - pamela
   - typing_extensions
   - adlfs
   - importlib_metadata
```

### Comparing `quetz-server-0.8.0/init_db.py` & `quetz-server-0.9.0/init_db.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/pyproject.toml` & `quetz-server-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [tool.jupyter-releaser.options]
 check-imports = ["quetz"]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.tbump.version]
-current = "0.8.0"
+current = "0.9.0"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [[tool.tbump.field]]
 name = "channel"
```

### Comparing `quetz-server-0.8.0/quetz/authentication/auth_dao.py` & `quetz-server-0.9.0/quetz/authentication/auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/azuread.py` & `quetz-server-0.9.0/quetz/authentication/azuread.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/base.py` & `quetz-server-0.9.0/quetz/authentication/base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/github.py` & `quetz-server-0.9.0/quetz/authentication/github.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/gitlab.py` & `quetz-server-0.9.0/quetz/authentication/gitlab.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/google.py` & `quetz-server-0.9.0/quetz/authentication/google.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/jupyterhub.py` & `quetz-server-0.9.0/quetz/authentication/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/oauth2.py` & `quetz-server-0.9.0/quetz/authentication/oauth2.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/pam.py` & `quetz-server-0.9.0/quetz/authentication/pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authentication/registry.py` & `quetz-server-0.9.0/quetz/authentication/registry.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/authorization.py` & `quetz-server-0.9.0/quetz/authorization.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/basic_frontend/avatar.jpg` & `quetz-server-0.9.0/quetz/basic_frontend/avatar.jpg`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/basic_frontend/favicon.ico` & `quetz-server-0.9.0/quetz/basic_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/basic_frontend/index.html` & `quetz-server-0.9.0/quetz/basic_frontend/index.html`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/channel_data.py` & `quetz-server-0.9.0/quetz/channel_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/cli.py` & `quetz-server-0.9.0/quetz/cli.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/condainfo.py` & `quetz-server-0.9.0/quetz/condainfo.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/config.py` & `quetz-server-0.9.0/quetz/config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/dao.py` & `quetz-server-0.9.0/quetz/dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/database.py` & `quetz-server-0.9.0/quetz/database.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/database_extensions.py` & `quetz-server-0.9.0/quetz/database_extensions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/db_models.py` & `quetz-server-0.9.0/quetz/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/deps.py` & `quetz-server-0.9.0/quetz/deps.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/frontend.py` & `quetz-server-0.9.0/quetz/frontend.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/hooks.py` & `quetz-server-0.9.0/quetz/hooks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/jobs/api.py` & `quetz-server-0.9.0/quetz/jobs/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/jobs/dao.py` & `quetz-server-0.9.0/quetz/jobs/dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/jobs/handlers.py` & `quetz-server-0.9.0/quetz/jobs/handlers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/jobs/models.py` & `quetz-server-0.9.0/quetz/jobs/models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/jobs/rest_models.py` & `quetz-server-0.9.0/quetz/jobs/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/jobs/runner.py` & `quetz-server-0.9.0/quetz/jobs/runner.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/main.py` & `quetz-server-0.9.0/quetz/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1384,15 +1384,15 @@
 
     user_id = auth.assert_user()
     auth.assert_create_package(channel_name)
     condainfo = CondaInfo((body), filename)
     dest = os.path.join(condainfo.info["subdir"], filename)
 
     body.seek(0)
-    pkgstore.add_package(body, channel_name, dest)
+    await pkgstore.add_package_async(body, channel_name, dest)
 
     package_name = str(condainfo.info.get("name"))
     package_data = rest_models.Package(
         name=package_name,
         summary=str(condainfo.about.get("summary", "n/a")),
         description=str(condainfo.about.get("description", "n/a")),
     )
```

### Comparing `quetz-server-0.8.0/quetz/metrics/api.py` & `quetz-server-0.9.0/quetz/metrics/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/metrics/db_models.py` & `quetz-server-0.9.0/quetz/metrics/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/metrics/middleware.py` & `quetz-server-0.9.0/quetz/metrics/middleware.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/metrics/rest_models.py` & `quetz-server-0.9.0/quetz/metrics/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/metrics/tasks.py` & `quetz-server-0.9.0/quetz/metrics/tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/metrics/view.py` & `quetz-server-0.9.0/quetz/metrics/view.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/env.py` & `quetz-server-0.9.0/quetz/migrations/env.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py` & `quetz-server-0.9.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py` & `quetz-server-0.9.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py` & `quetz-server-0.9.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py` & `quetz-server-0.9.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py` & `quetz-server-0.9.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py` & `quetz-server-0.9.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py` & `quetz-server-0.9.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py` & `quetz-server-0.9.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py` & `quetz-server-0.9.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py` & `quetz-server-0.9.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py` & `quetz-server-0.9.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/a80fb051a659_create_tables.py` & `quetz-server-0.9.0/quetz/migrations/versions/a80fb051a659_create_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py` & `quetz-server-0.9.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py` & `quetz-server-0.9.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py` & `quetz-server-0.9.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py` & `quetz-server-0.9.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py` & `quetz-server-0.9.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py` & `quetz-server-0.9.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/pkgstores.py` & `quetz-server-0.9.0/quetz/pkgstores.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import tempfile
 import warnings
 from contextlib import contextmanager
 from os import PathLike
 from threading import Lock
 from typing import IO, List, Tuple, Union
 
+import aiofiles
+import aioshutil
 import fsspec
 from tenacity import retry
 from tenacity.retry import retry_if_exception_type
 from tenacity.stop import stop_after_attempt
 
 try:
     import xattr
@@ -77,14 +79,18 @@
         pass
 
     @abc.abstractmethod
     def url(self, channel: str, src: str, expires: int = 0) -> str:
         pass
 
     @abc.abstractmethod
+    def add_package_async(self, package: File, channel: str, destination: str):
+        pass
+
+    @abc.abstractmethod
     def add_package(self, package: File, channel: str, destination: str):
         pass
 
     @abc.abstractmethod
     def add_file(
         self, data: Union[str, bytes], channel: str, destination: StrPath
     ) -> None:
@@ -171,14 +177,23 @@
         channel_path = path.join(self.channels_dir, name)
         self.fs.rm(channel_path, recursive=True)
 
     def add_package(self, package: File, channel: str, destination: str) -> None:
         with self._atomic_open(channel, destination) as f:
             shutil.copyfileobj(package, f)
 
+    async def add_package_async(
+        self, package: File, channel: str, destination: str
+    ) -> None:
+        full_path = path.join(self.channels_dir, channel, destination)
+        self.fs.makedirs(path.dirname(full_path), exist_ok=True)
+
+        async with aiofiles.open(full_path, 'wb') as f:
+            await f.write(package.read())
+
     def add_file(
         self, data: Union[str, bytes], channel: str, destination: StrPath
     ) -> None:
         mode = "w" if isinstance(data, str) else "wb"
         with self._atomic_open(channel, destination, mode) as f:
             f.write(data)
 
@@ -282,15 +297,17 @@
         if region:
             client_kwargs["region_name"] = region
 
         # When using IAM, key and secret will be empty, so need to pass None
         # to the s3fs constructor
         key = config['key'] if config['key'] != '' else None
         secret = config['secret'] if config['secret'] != '' else None
-        self.fs = s3fs.S3FileSystem(key=key, secret=secret, client_kwargs=client_kwargs)
+        self.fs = s3fs.S3FileSystem(
+            key=key, secret=secret, asynchronous=True, client_kwargs=client_kwargs
+        )
 
         self.bucket_prefix = config['bucket_prefix']
         self.bucket_suffix = config['bucket_suffix']
         super().__init__()
 
     @property
     def support_redirect(self):
@@ -329,14 +346,23 @@
     def add_package(self, package: File, channel: str, destination: str) -> None:
         with self._get_fs() as fs:
             bucket = self._bucket_map(channel)
             with fs.open(path.join(bucket, destination), "wb", acl="private") as pkg:
                 # use a chunk size of 10 Megabytes
                 shutil.copyfileobj(package, pkg, 10 * 1024 * 1024)
 
+    async def add_package_async(
+        self, package: File, channel: str, destination: str
+    ) -> None:
+        with self._get_fs() as fs:
+            bucket = self._bucket_map(channel)
+            with fs.open(path.join(bucket, destination), "wb", acl="private") as pkg:
+                # use a chunk size of 10 Megabytes
+                await aioshutil.copyfileobj(package, pkg, 10 * 1024 * 1024)
+
     def add_file(
         self, data: Union[str, bytes], channel: str, destination: StrPath
     ) -> None:
         if type(data) is str:
             mode = "w"
         else:
             mode = "wb"
@@ -422,14 +448,15 @@
         self.access_key = config.get("account_access_key")
         self.conn_string = config.get("conn_str")
 
         self.fs = adlfs.AzureBlobFileSystem(
             account_name=self.storage_account_name,
             connection_string=self.conn_string,
             account_key=self.access_key,
+            asynchronous=True,
         )
 
         self.container_prefix = config['container_prefix']
         self.container_suffix = config['container_suffix']
         super().__init__()
 
     @property
@@ -468,14 +495,23 @@
     def add_package(self, package: File, channel: str, destination: str) -> None:
         with self._get_fs() as fs:
             container = self._container_map(channel)
             with fs.open(path.join(container, destination), "wb") as pkg:
                 # use a chunk size of 10 Megabytes
                 shutil.copyfileobj(package, pkg, 10 * 1024 * 1024)
 
+    async def add_package_async(
+        self, package: File, channel: str, destination: str
+    ) -> None:
+        with self._get_fs() as fs:
+            container = self._container_map(channel)
+            with fs.open(path.join(container, destination), "wb") as pkg:
+                # use a chunk size of 10 Megabytes
+                await aioshutil.copyfileobj(package, pkg, 10 * 1024 * 1024)
+
     def add_file(
         self, data: Union[str, bytes], channel: str, destination: StrPath
     ) -> None:
         if type(data) is str:
             mode = "w"
         else:
             mode = "wb"
@@ -567,14 +603,15 @@
         self.region = config.get("region")
 
         self.fs = gcsfs.GCSFileSystem(
             project=self.project,
             token=self.token if self.token else None,
             cache_timeout=self.cache_timeout,
             default_location=self.region,
+            asynchronous=True,
         )
 
         self.bucket_prefix = config['bucket_prefix']
         self.bucket_suffix = config['bucket_suffix']
         super().__init__()
 
     @property
@@ -617,14 +654,23 @@
     def add_package(self, package: File, channel: str, destination: str) -> None:
         with self._get_fs() as fs:
             container = self._bucket_map(channel)
             with fs.open(path.join(container, destination), "wb") as pkg:
                 # use a chunk size of 10 Megabytes
                 shutil.copyfileobj(package, pkg, 10 * 1024 * 1024)
 
+    async def add_package_async(
+        self, package: File, channel: str, destination: str
+    ) -> None:
+        with self._get_fs() as fs:
+            container = self._bucket_map(channel)
+            with fs.open(path.join(container, destination), "wb") as pkg:
+                # use a chunk size of 10 Megabytes
+                await aioshutil.copyfileobj(package, pkg, 10 * 1024 * 1024)
+
     def add_file(
         self, data: Union[str, bytes], channel: str, destination: StrPath
     ) -> None:
         if type(data) is str:
             mode = "w"
         else:
             mode = "wb"
```

### Comparing `quetz-server-0.8.0/quetz/repo_data.py` & `quetz-server-0.9.0/quetz/repo_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/rest_models.py` & `quetz-server-0.9.0/quetz/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tasks/common.py` & `quetz-server-0.9.0/quetz/tasks/common.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tasks/indexing.py` & `quetz-server-0.9.0/quetz/tasks/indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tasks/mirror.py` & `quetz-server-0.9.0/quetz/tasks/mirror.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tasks/reindexing.py` & `quetz-server-0.9.0/quetz/tasks/reindexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tasks/workers.py` & `quetz-server-0.9.0/quetz/tasks/workers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/templates/channeldata-index.html.j2` & `quetz-server-0.9.0/quetz/templates/channeldata-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/templates/subdir-index.html.j2` & `quetz-server-0.9.0/quetz/templates/subdir-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/testing/fixtures.py` & `quetz-server-0.9.0/quetz/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/testing/mockups.py` & `quetz-server-0.9.0/quetz/testing/mockups.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/testing/utils.py` & `quetz-server-0.9.0/quetz/testing/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/api/conftest.py` & `quetz-server-0.9.0/quetz/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/api/test_api_keys.py` & `quetz-server-0.9.0/quetz/tests/api/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/api/test_channels.py` & `quetz-server-0.9.0/quetz/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/api/test_main.py` & `quetz-server-0.9.0/quetz/tests/api/test_main.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/api/test_main_packages.py` & `quetz-server-0.9.0/quetz/tests/api/test_main_packages.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/api/test_metrics.py` & `quetz-server-0.9.0/quetz/tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/api/test_users.py` & `quetz-server-0.9.0/quetz/tests/api/test_users.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/authentification/test_auth_dao.py` & `quetz-server-0.9.0/quetz/tests/authentification/test_auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/authentification/test_base.py` & `quetz-server-0.9.0/quetz/tests/authentification/test_base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/authentification/test_oauth.py` & `quetz-server-0.9.0/quetz/tests/authentification/test_oauth.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/authentification/test_pam.py` & `quetz-server-0.9.0/quetz/tests/authentification/test_pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/conftest.py` & `quetz-server-0.9.0/quetz/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/data/other-package-0.1-0.tar.bz2` & `quetz-server-0.9.0/quetz/tests/data/other-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/data/other-package-0.2-0.tar.bz2` & `quetz-server-0.9.0/quetz/tests/data/other-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0.tar.bz2` & `quetz-server-0.9.0/quetz/tests/data/test-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2` & `quetz-server-0.9.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/data/test-package-0.2-0.tar.bz2` & `quetz-server-0.9.0/quetz/tests/data/test-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_auth.py` & `quetz-server-0.9.0/quetz/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_cli.py` & `quetz-server-0.9.0/quetz/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_config.py` & `quetz-server-0.9.0/quetz/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_dao.py` & `quetz-server-0.9.0/quetz/tests/test_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_database.py` & `quetz-server-0.9.0/quetz/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_indexing.py` & `quetz-server-0.9.0/quetz/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_jobs.py` & `quetz-server-0.9.0/quetz/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_mirror.py` & `quetz-server-0.9.0/quetz/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_pkg_stores.py` & `quetz-server-0.9.0/quetz/tests/test_pkg_stores.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import hashlib
 import os
 import shutil
 import time
 import uuid
+from collections.abc import Collection
+from io import BytesIO
+from pathlib import Path
 
 import pytest
 
 from quetz.pkgstores import (
     AzureBlobStore,
     GoogleCloudStorageStore,
     LocalStore,
+    PackageStore,
     S3Store,
     has_xattr,
 )
 
 s3_config = {
     'key': os.environ.get("S3_ACCESS_KEY"),
     'secret': os.environ.get("S3_SECRET_KEY"),
@@ -176,65 +180,81 @@
 
     yield
 
     # cleanup
     any_store.remove_channel(channel_name)
 
 
-def test_store_add_list_files(any_store, channel, channel_name):
-    def assert_files(expected_files, n_retries=3):
-        n_retries = 3
+def assert_files(
+    pkg_store: PackageStore,
+    channel_name: str,
+    expected_files: Collection[str],
+    n_retries: int = 3,
+):
+    """
+    Asserts that the files in the package store match the expected files with retry.
+    """
+    for _ in range(n_retries):
+        files = pkg_store.list_files(channel_name)
+        try:
+            assert files == expected_files
+        except AssertionError:
+            continue
+        else:
+            assert set(files) == set(expected_files)
 
-        files = []
-        for i in range(n_retries):
-            files = pkg_store.list_files(channel_name)
-            try:
-                assert files == expected_files
-            except AssertionError:
-                continue
-            break
-        assert files == expected_files
 
+def test_store_add_list_files(any_store, channel, channel_name):
     pkg_store = any_store
 
     pkg_store.add_file("content", channel_name, "test.txt")
     pkg_store.add_file("content", channel_name, "test_2.txt")
 
-    assert_files(["test.txt", "test_2.txt"])
+    assert_files(pkg_store, channel_name, ["test.txt", "test_2.txt"])
 
     pkg_store.delete_file(channel_name, "test.txt")
 
-    assert_files(["test_2.txt"])
+    assert_files(pkg_store, channel_name, ["test_2.txt"])
 
     metadata = pkg_store.get_filemetadata(channel_name, "test_2.txt")
     assert metadata[0] > 0
     assert type(metadata[1]) is float
     assert type(metadata[2]) is str
 
 
-def test_move_file(any_store, channel, channel_name):
-    def assert_files(expected_files, n_retries=3):
-        n_retries = 3
+@pytest.mark.asyncio
+async def test_add_package_async(any_store, channel, channel_name):
+    pkg_store = any_store
+
+    data = (Path(__file__).parent / "data" / "test-package-0.1-0.tar.bz2").read_bytes()
+
+    await pkg_store.add_package_async(
+        BytesIO(data), channel_name, "test-package-0.1-0.tar.gz"
+    )
+
+    assert_files(pkg_store, channel_name, ["test-package-0.1-0.tar.gz"])
 
-        files = []
-        for i in range(n_retries):
-            files = pkg_store.list_files(channel_name)
-            try:
-                assert files == expected_files
-            except AssertionError:
-                continue
-            break
-        assert files == expected_files
 
+def test_add_package(any_store, channel, channel_name):
+    pkg_store = any_store
+
+    data = (Path(__file__).parent / "data" / "test-package-0.1-0.tar.bz2").read_bytes()
+
+    pkg_store.add_package(BytesIO(data), channel_name, "test-package-0.1-0.tar.gz")
+
+    assert_files(pkg_store, channel_name, ["test-package-0.1-0.tar.gz"])
+
+
+def test_move_file(any_store, channel, channel_name):
     pkg_store = any_store
 
     pkg_store.add_file("content", channel_name, "test.txt")
     pkg_store.move_file(channel_name, "test.txt", "test_2.txt")
 
-    assert_files(['test_2.txt'])
+    assert_files(pkg_store, channel_name, ['test_2.txt'])
 
 
 @pytest.mark.parametrize("redirect_enabled", [False, True])
 @pytest.mark.parametrize("redirect_endpoint", ["/files", "/static"])
 def test_local_store_url(redirect_enabled, redirect_endpoint):
     local_store = LocalStore(
         {
```

### Comparing `quetz-server-0.8.0/quetz/tests/test_tasks.py` & `quetz-server-0.9.0/quetz/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_versionorder.py` & `quetz-server-0.9.0/quetz/tests/test_versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/tests/test_workers.py` & `quetz-server-0.9.0/quetz/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/utils.py` & `quetz-server-0.9.0/quetz/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz/versionorder.py` & `quetz-server-0.9.0/quetz/versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_db_ext/CMakeLists.txt` & `quetz-server-0.9.0/quetz_db_ext/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_db_ext/LIBSOLV_LICENSE.txt` & `quetz-server-0.9.0/quetz_db_ext/LIBSOLV_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_db_ext/conda.c` & `quetz-server-0.9.0/quetz_db_ext/conda.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_db_ext/conda.h` & `quetz-server-0.9.0/quetz_db_ext/conda.h`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_db_ext/quetz_pg.c` & `quetz-server-0.9.0/quetz_db_ext/quetz_pg.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_db_ext/quetz_sqlite.c` & `quetz-server-0.9.0/quetz_db_ext/quetz_sqlite.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_server.egg-info/PKG-INFO` & `quetz-server-0.9.0/quetz_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.8.0
+Version: 0.9.0
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.8.0 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.9.0 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
```

### Comparing `quetz-server-0.8.0/quetz_server.egg-info/SOURCES.txt` & `quetz-server-0.9.0/quetz_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.8.0/quetz_server.egg-info/requires.txt` & `quetz-server-0.9.0/quetz_server.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 tenacity
 toml
 typer
 typing_extensions
 ujson
 uvicorn
 zstandard
+aioshutil
 
 [all]
 adlfs
 gcsfs>=2022.02
 pamela
 psycopg2
 s3fs
```

### Comparing `quetz-server-0.8.0/setup.cfg` & `quetz-server-0.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 	tenacity
 	toml
 	typer
 	typing_extensions
 	ujson
 	uvicorn
 	zstandard
+	aioshutil
 
 [options.entry_points]
 console_scripts = 
 	quetz = quetz.cli:app
 
 [options.extras_require]
 azure =
```

