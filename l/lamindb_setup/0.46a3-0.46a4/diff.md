# Comparing `tmp/lamindb_setup-0.46a3.tar.gz` & `tmp/lamindb_setup-0.46a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.46a3.tar", last modified: Fri Jun  2 16:03:58 2023, max compression
+gzip compressed data, was "lamindb_setup-0.46a4.tar", last modified: Mon Jun  5 12:59:52 2023, max compression
```

## Comparing `lamindb_setup-0.46a3.tar` & `lamindb_setup-0.46a4.tar`

### file list

```diff
@@ -1,171 +1,89 @@
--rw-r--r--   0        0        0     3304 2023-06-01 11:33:10.497771 lamindb_setup-0.46a3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.46a3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.46a3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.46a3/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.46a3/.gitmodules
--rw-r--r--   0        0        0     1793 2023-06-01 11:33:10.497933 lamindb_setup-0.46a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.46a3/LICENSE
--rw-r--r--   0        0        0      182 2023-06-01 11:33:49.258270 lamindb_setup-0.46a3/README.md
--rw-r--r--   0        0        0       52 2023-05-26 12:29:21.559991 lamindb_setup-0.46a3/docs/api.md
--rw-r--r--   0        0        0    50353 2023-06-02 16:03:38.945364 lamindb_setup-0.46a3/docs/changelog.md
--rw-r--r--   0        0        0     5356 2023-06-01 11:33:10.498487 lamindb_setup-0.46a3/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3553 2023-06-01 11:33:10.498687 lamindb_setup-0.46a3/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     6339 2023-06-01 11:33:10.498876 lamindb_setup-0.46a3/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-05-26 12:29:21.560682 lamindb_setup-0.46a3/docs/faq/index.md
--rw-r--r--   0        0        0     1244 2023-06-01 11:33:10.499064 lamindb_setup-0.46a3/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.46a3/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2880 2023-06-01 11:33:10.499418 lamindb_setup-0.46a3/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2144 2023-06-01 11:33:10.499589 lamindb_setup-0.46a3/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     8821 2023-06-01 11:33:10.499805 lamindb_setup-0.46a3/docs/guide/00-index.ipynb
--rw-r--r--   0        0        0     5037 2023-06-01 11:33:10.499992 lamindb_setup-0.46a3/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0     8081 2023-06-01 11:33:10.500188 lamindb_setup-0.46a3/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     4342 2023-06-01 11:33:10.500381 lamindb_setup-0.46a3/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6104 2023-06-01 11:33:10.500592 lamindb_setup-0.46a3/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3329 2023-06-01 11:33:10.500807 lamindb_setup-0.46a3/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     3331 2023-05-26 12:29:21.561700 lamindb_setup-0.46a3/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-05-26 12:29:21.561778 lamindb_setup-0.46a3/docs/index.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.46a3/docs/test_notebooks.py
--rw-r--r--   0        0        0      118 2023-05-26 12:29:21.561849 lamindb_setup-0.46a3/lamin-project.yaml
--rw-r--r--   0        0        0     2794 2023-06-02 16:03:32.990491 lamindb_setup-0.46a3/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5268 2023-06-01 11:33:10.501041 lamindb_setup-0.46a3/lamindb_setup/__main__.py
--rw-r--r--   0        0        0      100 2023-06-01 11:33:10.501383 lamindb_setup-0.46a3/lamindb_setup/_assets/__init__.py
--rw-r--r--   0        0        0     1813 2023-06-02 16:02:42.978369 lamindb_setup-0.46a3/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-06-01 11:33:10.501769 lamindb_setup-0.46a3/lamindb_setup/_check_versions.py
--rw-r--r--   0        0        0      567 2023-06-01 11:33:10.501880 lamindb_setup-0.46a3/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2182 2023-06-01 11:33:10.502044 lamindb_setup-0.46a3/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      329 2023-06-01 11:33:10.502137 lamindb_setup-0.46a3/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7275 2023-06-02 16:02:42.978682 lamindb_setup-0.46a3/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     7291 2023-06-01 11:33:10.502702 lamindb_setup-0.46a3/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      135 2023-06-01 11:33:10.502811 lamindb_setup-0.46a3/lamindb_setup/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-06-01 11:33:10.503004 lamindb_setup-0.46a3/lamindb_setup/_migrate/alembic.ini
--rw-r--r--   0        0        0     3731 2023-06-01 11:33:10.503365 lamindb_setup-0.46a3/lamindb_setup/_migrate/core.py
--rw-r--r--   0        0        0     7656 2023-06-01 11:33:10.503596 lamindb_setup-0.46a3/lamindb_setup/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-06-01 11:33:10.503705 lamindb_setup-0.46a3/lamindb_setup/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-06-01 11:33:10.503790 lamindb_setup-0.46a3/lamindb_setup/_migrate/script.py.mako
--rw-r--r--   0        0        0     4849 2023-06-01 11:33:10.503950 lamindb_setup-0.46a3/lamindb_setup/_migrate/utils.py
--rw-r--r--   0        0        0      790 2023-06-01 11:33:10.504025 lamindb_setup-0.46a3/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      803 2023-06-01 11:33:10.504108 lamindb_setup-0.46a3/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-06-01 11:33:10.504188 lamindb_setup-0.46a3/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1848 2023-06-01 11:33:10.504348 lamindb_setup-0.46a3/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-01 11:33:10.504569 lamindb_setup-0.46a3/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.46a3/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.46a3/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3488 2023-06-01 11:33:10.504859 lamindb_setup-0.46a3/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      456 2023-06-01 11:33:10.505005 lamindb_setup-0.46a3/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     3886 2023-06-01 11:33:10.505126 lamindb_setup-0.46a3/lamindb_setup/dev/_clone.py
--rw-r--r--   0        0        0     7299 2023-06-01 11:33:10.505212 lamindb_setup-0.46a3/lamindb_setup/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.46a3/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     1693 2023-06-01 11:33:10.505393 lamindb_setup-0.46a3/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.46a3/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-06-01 11:33:10.505542 lamindb_setup-0.46a3/lamindb_setup/dev/_exclusion.py
--rw-r--r--   0        0        0     9422 2023-06-02 16:02:42.978976 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-06-01 11:33:10.506008 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2728 2023-06-01 11:33:10.506321 lamindb_setup-0.46a3/lamindb_setup/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     4115 2023-06-02 16:02:42.979223 lamindb_setup-0.46a3/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5536 2023-06-01 11:33:10.506569 lamindb_setup-0.46a3/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2536 2023-06-01 11:33:10.506639 lamindb_setup-0.46a3/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      356 2023-06-01 11:33:10.506745 lamindb_setup-0.46a3/lamindb_setup/test/__init__.py
--rw-r--r--   0        0        0       50 2023-06-01 11:33:10.506814 lamindb_setup-0.46a3/lamindb_setup/test/_env.py
--rw-r--r--   0        0        0     3949 2023-06-01 11:33:10.507074 lamindb_setup-0.46a3/lamindb_setup/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6673 2023-06-01 11:33:10.507279 lamindb_setup-0.46a3/lamindb_setup/test/_migrations_unit.py
--rw-r--r--   0        0        0      254 2023-06-01 11:33:10.507525 lamindb_setup-0.46a3/lamindb_setup/test/_nox.py
--rw-r--r--   0        0        0      188 2023-06-01 11:33:10.507620 lamindb_setup-0.46a3/lamindb_setup/test/nox.py
--rw-r--r--   0        0        0     2811 2023-06-02 12:28:18.951248 lamindb_setup-0.46a3/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.46a3/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-30 14:21:30.384364 lamindb_setup-0.46a3/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.46a3/lnschema-core/.gitignore
--rw-r--r--   0        0        0        0 2023-06-02 12:28:18.951387 lamindb_setup-0.46a3/lnschema-core/.gitmodules
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.46a3/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.46a3/lnschema-core/LICENSE
--rw-r--r--   0        0        0      364 2023-05-30 14:21:30.384850 lamindb_setup-0.46a3/lnschema-core/README.md
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.384908 lamindb_setup-0.46a3/lnschema-core/django_project/__init__.py
--rw-r--r--   0        0        0      404 2023-05-30 14:21:30.384975 lamindb_setup-0.46a3/lnschema-core/django_project/asgi.py
--rw-r--r--   0        0        0     3572 2023-05-30 14:21:30.385044 lamindb_setup-0.46a3/lnschema-core/django_project/settings.py
--rw-r--r--   0        0        0      770 2023-05-30 14:21:30.385110 lamindb_setup-0.46a3/lnschema-core/django_project/urls.py
--rw-r--r--   0        0        0      404 2023-05-30 14:21:30.385276 lamindb_setup-0.46a3/lnschema-core/django_project/wsgi.py
--rw-r--r--   0        0        0    24509 2023-06-02 12:28:18.952040 lamindb_setup-0.46a3/lnschema-core/docs/changelog.md
--rw-r--r--   0        0        0     1485 2023-05-31 12:00:39.299258 lamindb_setup-0.46a3/lnschema-core/docs/guide/0-core-schema.ipynb
--rw-r--r--   0        0        0     8386 2023-05-31 12:00:39.320747 lamindb_setup-0.46a3/lnschema-core/docs/guide/1-data-validation.ipynb
--rw-r--r--   0        0        0       68 2023-05-30 14:21:30.385923 lamindb_setup-0.46a3/lnschema-core/docs/guide/index.md
--rw-r--r--   0        0        0      112 2023-05-30 14:21:30.386018 lamindb_setup-0.46a3/lnschema-core/docs/index.md
--rw-r--r--   0        0        0      202 2023-05-30 14:21:30.386086 lamindb_setup-0.46a3/lnschema-core/lamin-project.yaml
--rw-r--r--   0        0        0     1033 2023-06-02 12:28:39.298653 lamindb_setup-0.46a3/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0    24693 2023-06-02 12:28:18.952953 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_core.py
--rw-r--r--   0        0        0     1514 2023-05-30 14:21:30.386812 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_link.py
--rw-r--r--   0        0        0     1652 2023-06-02 15:54:27.350134 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0      228 2023-05-30 14:21:30.386885 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_timestamps.py
--rw-r--r--   0        0        0      932 2023-06-02 12:28:18.953448 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_types.py
--rw-r--r--   0        0        0      349 2023-06-02 12:28:18.953894 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_users.py
--rw-r--r--   0        0        0      100 2023-05-30 14:21:30.387077 lamindb_setup-0.46a3/lnschema-core/lnschema_core/apps.py
--rw-r--r--   0        0        0      313 2023-05-30 14:21:30.387173 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/__init__.py
--rw-r--r--   0        0        0     2477 2023-05-30 14:21:30.387427 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/_id.py
--rw-r--r--   0        0        0     1075 2023-05-30 14:21:30.387523 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/_versions.py
--rw-r--r--   0        0        0      579 2023-05-30 14:21:30.387597 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/id.py
--rw-r--r--   0        0        0    13429 2023-06-02 15:54:27.350430 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/sqlmodel.py
--rw-r--r--   0        0        0      227 2023-05-30 14:21:30.387777 lamindb_setup-0.46a3/lnschema-core/lnschema_core/link.py
--rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.387839 lamindb_setup-0.46a3/lnschema-core/lnschema_core/manage.py
--rw-r--r--   0        0        0     9699 2023-05-31 19:24:00.354344 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0      409 2023-06-02 12:28:39.298909 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0002_alter_file_id.py
--rw-r--r--   0        0        0      417 2023-06-02 12:28:39.299082 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0003_alter_folder_id.py
--rw-r--r--   0        0        0      661 2023-06-02 12:28:39.299271 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0004_alter_folder_created_at_alter_folder_updated_at.py
--rw-r--r--   0        0        0     1368 2023-06-02 12:28:39.299452 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0005_alter_project_id_alter_run_id_alter_storage_id_and_more.py
--rw-r--r--   0        0        0     2831 2023-06-02 12:28:39.299634 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0006_transform_hash_alter_features_created_by_and_more.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0     3694 2023-05-30 14:21:30.388217 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py
--rw-r--r--   0        0        0     6580 2023-05-30 14:21:30.388467 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py
--rw-r--r--   0        0        0     2073 2023-05-30 14:21:30.388554 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py
--rw-r--r--   0        0        0     4358 2023-05-30 14:21:30.388622 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py
--rw-r--r--   0        0        0     3333 2023-05-30 14:21:30.388701 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py
--rw-r--r--   0        0        0      817 2023-05-30 14:21:30.388767 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py
--rw-r--r--   0        0        0      536 2023-05-30 14:21:30.388831 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py
--rw-r--r--   0        0        0      976 2023-05-30 14:21:30.388893 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py
--rw-r--r--   0        0        0     6332 2023-05-30 14:21:30.388963 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py
--rw-r--r--   0        0        0     2886 2023-05-30 14:21:30.389027 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py
--rw-r--r--   0        0        0      762 2023-05-30 14:21:30.389088 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py
--rw-r--r--   0        0        0      668 2023-05-30 14:21:30.389149 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py
--rw-r--r--   0        0        0     1082 2023-05-30 14:21:30.389209 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-30-439c4ee0a22a-v0_9_0.py
--rw-r--r--   0        0        0     1725 2023-05-30 14:21:30.389276 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-07-0c819d33ca9b-v0_10_0.py
--rw-r--r--   0        0        0      613 2023-05-30 14:21:30.389356 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-10-3d244a8d3148-v0_11_0.py
--rw-r--r--   0        0        0      646 2023-05-30 14:21:30.389424 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-11-2ddcb037e3ea-v0_12_0.py
--rw-r--r--   0        0        0     3507 2023-05-30 14:21:30.389485 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-19-cf5913791674-v0_14_0.py
--rw-r--r--   0        0        0     2344 2023-05-30 14:21:30.389548 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-31-98da12fc80a8-v0_15_0.py
--rw-r--r--   0        0        0     8560 2023-05-30 14:21:30.389626 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-10-4ee426b656bb-v0_16_0.py
--rw-r--r--   0        0        0     4792 2023-05-30 14:21:30.389844 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-11-66bfd6cf2e2d-v0_17_0.py
--rw-r--r--   0        0        0     4603 2023-05-30 14:21:30.389927 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-28-4b4005b7841c-v0_21_1.py
--rw-r--r--   0        0        0     1209 2023-05-30 14:21:30.390122 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-12-07-9d94f3b9566d-v0_21_3.py
--rw-r--r--   0        0        0     2202 2023-05-30 14:21:30.390229 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-12-07-db1df7b2aaad-v0_22_0.py
--rw-r--r--   0        0        0     1098 2023-05-30 14:21:30.390300 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-01-09-f6b6b85cdffc-v0_24_0.py
--rw-r--r--   0        0        0     1229 2023-05-30 14:21:30.390371 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-02-9d283a1685a5-v0_25_6.py
--rw-r--r--   0        0        0     3580 2023-05-30 14:21:30.390448 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-07-8bf788467d0a-v0_25_9.py
--rw-r--r--   0        0        0      593 2023-05-30 14:21:30.390525 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-10-ff3b5b3ec913-v0_26_1.py
--rw-r--r--   0        0        0      973 2023-05-30 14:21:30.390584 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-14-8280855a5064-v0_26_2.py
--rw-r--r--   0        0        0     1120 2023-05-30 14:21:30.390641 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-21-1dafcf0b22aa-v0_28_0.py
--rw-r--r--   0        0        0     1067 2023-05-30 14:21:30.390699 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-22-6952574e2d49-v0_28_1.py
--rw-r--r--   0        0        0     1712 2023-05-30 14:21:30.390788 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-23-24e55331f27c-v0_28_2.py
--rw-r--r--   0        0        0      483 2023-05-30 14:21:30.390866 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-23-3dd9f8d41861-v0_28_3.py
--rw-r--r--   0        0        0      581 2023-05-30 14:21:30.390932 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-24-873683a29806-v0_28_7.py
--rw-r--r--   0        0        0      778 2023-05-30 14:21:30.390997 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-21-9640062eefee-v0_30rc1.py
--rw-r--r--   0        0        0     5367 2023-05-30 14:21:30.391066 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-23-ebafd37fd6e1-v0_30rc2.py
--rw-r--r--   0        0        0     6957 2023-05-30 14:21:30.391136 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-24-5846a15d9241-0_30rc3.py
--rw-r--r--   0        0        0     1658 2023-05-30 14:21:30.391214 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-05-6de59093e378-v0_32_0.py
--rw-r--r--   0        0        0      780 2023-05-30 14:21:30.391283 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-13-d161a14a12e3-v0_32_1.py
--rw-r--r--   0        0        0     4440 2023-05-30 14:21:30.391353 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-16-6a73c00555b4-v0_33_0.py
--rw-r--r--   0        0        0     3782 2023-05-30 14:21:30.391419 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-05-24-c3f38ffe9e03-v0_34a1.py
--rw-r--r--   0        0        0     8841 2023-05-30 14:21:30.391507 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-05-28-1c49c9f9a982-v0_34a2.py
--rw-r--r--   0        0        0    18194 2023-06-02 15:54:27.350739 lamindb_setup-0.46a3/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      205 2023-05-30 14:21:30.391658 lamindb_setup-0.46a3/lnschema-core/lnschema_core/types.py
--rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.391734 lamindb_setup-0.46a3/lnschema-core/manage.py
--rw-r--r--   0        0        0     1281 2023-06-02 12:28:18.955047 lamindb_setup-0.46a3/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      966 2023-06-02 12:28:18.955511 lamindb_setup-0.46a3/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0     1212 2023-06-02 12:28:18.955860 lamindb_setup-0.46a3/lnschema-core/tests/test_migrations.py
--rw-r--r--   0        0        0      475 2023-05-30 14:21:30.392155 lamindb_setup-0.46a3/lnschema-core/tests/test_notebooks.py
--rw-r--r--   0        0        0     2112 2023-06-01 11:33:10.507865 lamindb_setup-0.46a3/noxfile.py
--rw-r--r--   0        0        0     1399 2023-06-01 11:33:10.508034 lamindb_setup-0.46a3/pyproject.toml
--rw-r--r--   0        0        0      658 2023-06-01 11:33:10.508216 lamindb_setup-0.46a3/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.46a3/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.46a3/tests/test_load_instance.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.46a3/tests/test_set_storage.py
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 lamindb_setup-0.46a3/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.46a4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.46a4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.46a4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.46a4/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.46a4/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.46a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.46a4/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.46a4/README.md
+-rw-r--r--   0        0        0       52 2023-05-26 12:29:21.559991 lamindb_setup-0.46a4/docs/api.md
+-rw-r--r--   0        0        0    51804 2023-06-05 12:59:32.556986 lamindb_setup-0.46a4/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.46a4/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.46a4/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.46a4/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     5058 2023-06-04 16:47:53.812781 lamindb_setup-0.46a4/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8821 2023-06-04 17:52:00.959624 lamindb_setup-0.46a4/docs/guide/00-index.ipynb
+-rw-r--r--   0        0        0     5037 2023-06-01 11:33:10.499992 lamindb_setup-0.46a4/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0     8081 2023-06-01 11:33:10.500188 lamindb_setup-0.46a4/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     4342 2023-06-01 11:33:10.500381 lamindb_setup-0.46a4/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-04 11:49:29.988148 lamindb_setup-0.46a4/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3271 2023-06-04 11:49:29.988389 lamindb_setup-0.46a4/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     3331 2023-05-26 12:29:21.561700 lamindb_setup-0.46a4/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-05-26 12:29:21.561778 lamindb_setup-0.46a4/docs/index.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.46a4/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.46a4/lamin-project.yaml
+-rw-r--r--   0        0        0     2626 2023-06-05 12:59:06.828598 lamindb_setup-0.46a4/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5344 2023-06-04 19:41:00.162639 lamindb_setup-0.46a4/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.46a4/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      567 2023-06-01 11:33:10.501880 lamindb_setup-0.46a4/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2182 2023-06-01 11:33:10.502044 lamindb_setup-0.46a4/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.46a4/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.46a4/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6969 2023-06-05 12:38:39.756205 lamindb_setup-0.46a4/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6073 2023-06-04 19:41:00.163584 lamindb_setup-0.46a4/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.46a4/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.46a4/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.46a4/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.46a4/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1857 2023-06-04 19:41:00.164149 lamindb_setup-0.46a4/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.46a4/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.46a4/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.46a4/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.46a4/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.46a4/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.46a4/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.46a4/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     2546 2023-06-04 19:41:00.164891 lamindb_setup-0.46a4/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.46a4/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-06-01 11:33:10.505542 lamindb_setup-0.46a4/lamindb_setup/dev/_exclusion.py
+-rw-r--r--   0        0        0     8983 2023-06-04 19:41:00.165203 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     3419 2023-06-04 19:41:00.165550 lamindb_setup-0.46a4/lamindb_setup/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.46a4/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.46a4/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2563 2023-06-04 19:41:00.165849 lamindb_setup-0.46a4/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0     2811 2023-06-02 12:28:18.951248 lamindb_setup-0.46a4/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.46a4/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-30 14:21:30.384364 lamindb_setup-0.46a4/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.46a4/lnschema-core/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-02 12:28:18.951387 lamindb_setup-0.46a4/lnschema-core/.gitmodules
+-rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.46a4/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.46a4/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      364 2023-05-30 14:21:30.384850 lamindb_setup-0.46a4/lnschema-core/README.md
+-rw-r--r--   0        0        0    25152 2023-06-04 14:18:28.863714 lamindb_setup-0.46a4/lnschema-core/docs/changelog.md
+-rw-r--r--   0        0        0     1485 2023-06-04 11:09:43.036808 lamindb_setup-0.46a4/lnschema-core/docs/guide/core-schema.ipynb
+-rw-r--r--   0        0        0       52 2023-06-04 11:09:43.037197 lamindb_setup-0.46a4/lnschema-core/docs/guide/index.md
+-rw-r--r--   0        0        0      112 2023-05-30 14:21:30.386018 lamindb_setup-0.46a4/lnschema-core/docs/index.md
+-rw-r--r--   0        0        0      202 2023-05-30 14:21:30.386086 lamindb_setup-0.46a4/lnschema-core/lamin-project.yaml
+-rw-r--r--   0        0        0      544 2023-06-04 14:18:28.863945 lamindb_setup-0.46a4/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-04 14:18:28.864113 lamindb_setup-0.46a4/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0      740 2023-06-04 14:37:07.398773 lamindb_setup-0.46a4/lnschema-core/lnschema_core/_types.py
+-rw-r--r--   0        0        0      349 2023-06-02 12:28:18.953894 lamindb_setup-0.46a4/lnschema-core/lnschema_core/_users.py
+-rw-r--r--   0        0        0     2810 2023-06-04 11:09:43.037807 lamindb_setup-0.46a4/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0     9848 2023-06-05 09:38:49.986505 lamindb_setup-0.46a4/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.46a4/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    21409 2023-06-04 14:37:07.399082 lamindb_setup-0.46a4/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      180 2023-06-04 14:37:07.399765 lamindb_setup-0.46a4/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0     1283 2023-06-04 14:18:28.865001 lamindb_setup-0.46a4/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-04 14:37:07.399971 lamindb_setup-0.46a4/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      475 2023-05-30 14:21:30.392155 lamindb_setup-0.46a4/lnschema-core/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1814 2023-06-04 07:52:37.336139 lamindb_setup-0.46a4/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-05 12:57:21.542553 lamindb_setup-0.46a4/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.46a4/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.46a4/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.46a4/tests/test_load_instance.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.46a4/tests/test_set_storage.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.46a4/PKG-INFO
```

### Comparing `lamindb_setup-0.46a3/.github/workflows/build.yml` & `lamindb_setup-0.46a4/.github/workflows/build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,14 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
         group:
           - "unit"
           - "docs"
-          - "unit-django"
-          - "docs-django"
     timeout-minutes: 20
 
     steps:
       - name: Checkout main
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
@@ -74,17 +72,21 @@
       # - uses: "google-github-actions/auth@v0"
       #   with:
       #     credentials_json: "${{ secrets.GCP_CREDENTIALS }}"
       # - uses: "google-github-actions/setup-gcloud@v0"
       - run: nox -s "install(group='${{ matrix.group }}')"
       - run: nox -s "build(group='${{ matrix.group }}')"
         env:
-          GITHUB_EVENT_NAME: ${{ github.event_name }}
           SUPABASE_STAGING_URL: ${{ secrets.SUPABASE_STAGING_URL }}
           SUPABASE_STAGING_ANON_KEY: ${{ secrets.SUPABASE_STAGING_ANON_KEY }}
+      - name: upload coverage
+        uses: actions/upload-artifact@v2
+        with:
+          name: coverage--${{ matrix.group }}
+          path: .coverage
       - run: nox -s docs
         if: ${{ matrix.group == 'docs' }}
       - uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
       - uses: nwtgck/actions-netlify@v1.2
         if: ${{ matrix.group == 'docs' }}
@@ -92,7 +94,30 @@
           publish-dir: "_build/html"
           production-deploy: ${{ github.event_name == 'push' }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
           enable-commit-comment: false
         env:
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
           NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
+
+  coverage:
+    needs: build
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: 3.9
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml"
+      - run: |
+          pip install coverage[toml]
+          pip install --no-deps .
+      - uses: actions/download-artifact@v2
+      - name: run coverage
+        run: |
+          coverage combine coverage--*/.coverage*
+          coverage report --fail-under=0
+          coverage xml
+      - uses: codecov/codecov-action@v2
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `lamindb_setup-0.46a3/.github/workflows/latest-changes.yml` & `lamindb_setup-0.46a4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/.gitignore` & `lamindb_setup-0.46a4/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/.pre-commit-config.yaml` & `lamindb_setup-0.46a4/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     hooks:
       - id: mypy
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.1.1
     hooks:
       - id: pydocstyle
         args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
-          - --ignore=D100,D101,D102,D103,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413
+          - --ignore=D100,D101,D102,D103,D104,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413
```

### Comparing `lamindb_setup-0.46a3/LICENSE` & `lamindb_setup-0.46a4/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/docs/changelog.md` & `lamindb_setup-0.46a4/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🏗️ Enable Django backend (lamindb) | [390](https://github.com/laminlabs/lamindb-setup/pull/390) | [falexwolf](https://github.com/falexwolf) | 2023-06-02 | 0.46a3
+🔊 Better logging | [399](https://github.com/laminlabs/lamindb-setup/pull/399) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 | 0.46a3
+💄 Prettier settings file names | [398](https://github.com/laminlabs/lamindb-setup/pull/398) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
+⚡ Bionty versions table & performance improvements | [396](https://github.com/laminlabs/lamindb-setup/pull/396) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-04 |
+🔥 Remove all occurances of sqlmodel | [397](https://github.com/laminlabs/lamindb-setup/pull/397) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
+🔥 Delete SQLAlchemy related content | [395](https://github.com/laminlabs/lamindb-setup/pull/395) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
+🔥 Remove alembic migrations infra & fix coverage | [394](https://github.com/laminlabs/lamindb-setup/pull/394) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
+✨ Add migrations management for Django (start breaking SQLAlchemy) | [393](https://github.com/laminlabs/lamindb-setup/pull/393) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
+✨ Extend django to lnschema-bionty | [392](https://github.com/laminlabs/lamindb-setup/pull/392) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-04 |
+✨ New id and version in track | [391](https://github.com/laminlabs/lamindb-setup/pull/391) | [Koncopd](https://github.com/Koncopd) | 2023-06-02 |
+🏗️ Enable Django backend (lamindb) | [390](https://github.com/laminlabs/lamindb-setup/pull/390) | [falexwolf](https://github.com/falexwolf) | 2023-06-02 |
 🚚 Rename package to `lamindb_setup` | [389](https://github.com/laminlabs/lamindb-setup/pull/389) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.46a2
 🏗️ Add Django backend | [388](https://github.com/laminlabs/lndb/pull/388) | [falexwolf](https://github.com/falexwolf) | 2023-05-31 | 0.46a1
 ♻️ Refactor CI | [387](https://github.com/laminlabs/lndb/pull/387) | [falexwolf](https://github.com/falexwolf) | 2023-05-30 | 0.45.0
 🐛 Unlock on uncaught exceptions in ipython | [386](https://github.com/laminlabs/lndb/pull/386) | [Koncopd](https://github.com/Koncopd) | 2023-05-30 |
 ⬆️ Upgrade to lnhub-rest 0.9.8 | [384](https://github.com/laminlabs/lndb/pull/384) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a4
 ⬆️ Upgrade lnhub-rest to 0.9.7 | [383](https://github.com/laminlabs/lndb/pull/383) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a3
 📝 Add setup overview from lamindb | [382](https://github.com/laminlabs/lndb/pull/382) | [falexwolf](https://github.com/falexwolf) | 2023-05-27 |
```

### Comparing `lamindb_setup-0.46a3/docs/faq/check-synchronization.ipynb` & `lamindb_setup-0.46a4/docs/faq/test-sqlite-sync.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9918733465608466%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'instance_name = "*

 * *            'f"lamindb-setup-ci-test-sqlite-sync"\\n\'), (1, \'!lamin load {instance_name}\\n\')], '*

 * *            "delete: [3, 2, 1, 0]}}, 2: {'source': {insert: [(0, 'from lamindb_setup import init, "*

 * *            "settings, delete\\n')], delete: [0]}}, 12: {'source': ['Update the local version of "*

 * *            "the sqlite file:']}, 13: {'source': "*

 * *            "['settings.instance._update_local_sqlite_file()']}, 20: {'source': "*

 * *            "['set […]*

```diff
@@ -12,45 +12,33 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6e685a68",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb_setup\n",
-                "\n",
-                "group = \"django\" if lamindb_setup._USE_DJANGO else \"sqlalchemy\"\n",
-                "instance_name = f\"lamindb-setup-ci-{group}\"\n",
+                "instance_name = f\"lamindb-setup-ci-test-sqlite-sync\"\n",
+                "!lamin load {instance_name}\n",
                 "!lamin delete {instance_name}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f906c3b7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lamindb_setup import login, init, settings, delete\n",
+                "from lamindb_setup import init, settings, delete\n",
                 "import os"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "47db6427",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "login(\"testuser1@lamin.ai\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "b651f6da",
             "metadata": {},
             "outputs": [],
             "source": [
                 "init(\n",
                 "    storage=\"s3://lndb-setup-ci\",\n",
                 "    name=instance_name,\n",
@@ -137,25 +125,25 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "27bd0aac",
             "metadata": {},
             "source": [
-                "Access to the session restores the local version of sqlite database by downloading it from the cloud."
+                "Update the local version of the sqlite file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ee390b27",
             "metadata": {},
             "outputs": [],
             "source": [
-                "settings.instance.session()"
+                "settings.instance._update_local_sqlite_file()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c7bb2d22",
             "metadata": {},
@@ -216,15 +204,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7616cb64",
             "metadata": {},
             "outputs": [],
             "source": [
-                "settings.instance.session()"
+                "settings.instance._update_local_sqlite_file()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b350c551",
             "metadata": {},
@@ -233,20 +221,22 @@
                 "assert cache_file.stat().st_mtime == sqlite_file.modified.timestamp()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "adb57f7c",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "# clean up\n",
-                "settings.instance._sqlite_file.unlink()\n",
-                "delete(\"lndb-setup-ci\")"
+                "!lamin delete {instance_name}"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `lamindb_setup-0.46a3/docs/faq/clone.ipynb` & `lamindb_setup-0.46a4/docs/faq/switch-environment.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7970413165266106%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('tags', [])])}, 'source': ['# Test switch "*

 * *            "environment'], 'id': 'b43d09d5-26d3-440d-b334-9643ec5248e6'}, 1: {'source': ['from "*

 * *            "lamindb_setup import settings, signup, init, login\\n', 'from "*

 * *            "lamindb_setup.dev._settings_load import load_instance_settings\\n', 'import os'], "*

 * *            "'id': '33c2bb76-d61f-4866-87e2-780e61600022'}, 2: {'source': "*

 * *            '[\'login("testuser1@lamin.ai")\\n\', \'init(storage=" […]*

```diff
@@ -1,160 +1,123 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Clone a shallow copy of an instance for testing"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The function `clone_test` demonstrated below clones a shallow copy (last 20 rows of each table) of the current instance and returns the connection url to the test instance clone.\n",
-                "\n",
-                "Alternatively, one can pass an `InstanceSettings` object."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import lamindb_setup\n",
-                "from lamindb_setup import init, settings\n",
-                "from lamindb_setup.dev._clone import clone_test"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
+            "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
+            "metadata": {
+                "tags": []
+            },
             "source": [
-                "## A remote SQLite instance"
+                "# Test switch environment"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "if not lamindb_setup._USE_DJANGO:\n",
-                "    init(storage=\"s3://lamin-site-assets\")"
+                "from lamindb_setup import settings, signup, init, login\n",
+                "from lamindb_setup.dev._settings_load import load_instance_settings\n",
+                "import os"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "a9cbc2b8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "if not lamindb_setup._USE_DJANGO:\n",
-                "    clone_test()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Clean up the test instance."
+                "login(\"testuser1@lamin.ai\")\n",
+                "init(storage=\"mydata_prod\")\n",
+                "\n",
+                "user_access_token_prod = settings.user.access_token\n",
+                "!lamin delete mydata_prod"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "a5e8a0a6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "!rm -r lamin-site-assets_test"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Alternative way of calling `clone_test`."
+                "# os.environ[\"LAMIN_ENV\"] = \"dev\"\n",
+                "\n",
+                "# login(\"testuser1@lamin.ai\", password=\"BCRRvPjzjnEW4z0Sg4ecB474CEdOeFNWG5OgTnsO\")\n",
+                "# init(storage=\"mydata_dev\")\n",
+                "\n",
+                "# user_access_token_dev = settings.user.access_token"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "6c948145",
             "metadata": {},
             "outputs": [],
             "source": [
-                "if not lamindb_setup._USE_DJANGO:\n",
-                "    clone_test(settings.instance)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Clean up the test instance."
+                "# os.environ[\"LAMIN_ENV\"] = \"test\"\n",
+                "\n",
+                "# login(\"testuser1@lamin.ai\", password=\"3gYFv98ctNqYzgsf9iOrxmVUWkT2LkAD2l1V75jz\")\n",
+                "# init(storage=\"mydata_test\")\n",
+                "\n",
+                "# user_access_token_test = settings.user.access_token"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "f63669d8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "!rm -r lamin-site-assets_test"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## A postgres instance"
+                "# os.environ[\"LAMIN_ENV\"] = \"prod\"\n",
+                "\n",
+                "# settings.instance.name == \"mydata_prod\"\n",
+                "# settings.user.access_token == user_access_token_prod"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "87f37005",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# init(storage=\"gs://ln-retro-pg-std\", db=\"postgresql://batman:robin@35.222.187.204:5432/retro\")"
+                "# os.environ[\"LAMIN_ENV\"] = \"dev\"\n",
+                "\n",
+                "# settings.instance.name == \"mydata_dev\"\n",
+                "# settings.user.access_token == user_access_token_dev"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "db95be8e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# clone_test()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Clean up:"
+                "# os.environ[\"LAMIN_ENV\"] = \"test\"\n",
+                "\n",
+                "# settings.instance.name == \"mydata_test\"\n",
+                "# settings.user.access_token == user_access_token_test"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "26fe982b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# !docker stop pgtest\n",
-                "# !docker rm pgtest"
+                "# os.environ[\"LAMIN_ENV\"] = \"prod\""
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "base",
             "language": "python",
@@ -166,18 +129,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "40d3a090f54c6569ab1632332b64b2c03c39dcf918b08424e98f38b5ae0af88f"
             }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `lamindb_setup-0.46a3/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.46a4/docs/faq/edge-cases-login-init.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997354497354498%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(1, '    settings_dir / "*

 * *            'f"{get_settings_file_name_prefix()}user--testuser1@lamin.ai.env"\\n\'), (3, '*

 * *            "'(settings_dir / "*

 * *            'f"{get_settings_file_name_prefix()}user--testuser1.env").unlink()\\n\')], delete: [3, '*

 * *            '1]}}}'}*

```diff
@@ -83,17 +83,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "(\n",
-                "    settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1@lamin.ai.env\"\n",
+                "    settings_dir / f\"{get_settings_file_name_prefix()}user--testuser1@lamin.ai.env\"\n",
                 ").unlink()\n",
-                "(settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1.env\").unlink()\n",
+                "(settings_dir / f\"{get_settings_file_name_prefix()}user--testuser1.env\").unlink()\n",
                 "current_user_settings_file().unlink()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `lamindb_setup-0.46a3/docs/faq/manage-migrations.ipynb` & `lamindb_setup-0.46a4/lnschema-core/docs/guide/core-schema.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8025049603174603%*

 * *Differences: {"'cells'": "{0: {'source': ['# Core schema']}, 3: {'source': ['lookup = "*

 * *            'ln.User.lookup(field="handle")\']}, 4: {\'cell_type\': \'code\', \'source\': '*

 * *            "['lookup.testuser1'], 'execution_count': None, 'outputs': [], delete: "*

 * *            "['attachments']}, 5: {'source': ['ln.schema.view()']}, insert: [(1, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict([('tags', ['hide-cell'])])), ('outputs', []), ('source', ['!l […]*

```diff
@@ -1,68 +1,87 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Manage migrations"
+                "# Core schema"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "!lamin init --storage testdb"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb_setup"
+                "import lamindb as ln"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "lookup = ln.User.lookup(field=\"handle\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Running the following on the CLI\n",
-                "```\n",
-                "lamin migrate generate\n",
-                "```\n",
-                "runs"
+                "lookup.testuser1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# lamindb_setup.migrate.generate(package_name=\"lnschema_core\")"
+                "ln.schema.view()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3.9.12 ('base1')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.13"
         },
         "vscode": {
             "interpreter": {
-                "hash": "40d3a090f54c6569ab1632332b64b2c03c39dcf918b08424e98f38b5ae0af88f"
+                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
             }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `lamindb_setup-0.46a3/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.46a4/docs/guide/03-load-instance.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9240612599206349%*

 * *Differences: {"'cells'": "{0: {'source': ['# Load & close an instance']}, 1: {'id': "*

 * *            "'5fd65a65-5c34-462e-a980-a5aed1a2713f', 'metadata': {replace: OrderedDict([('tags', "*

 * *            "['hide-cell'])])}, 'source': ['!lamin close\\n', '!lamin delete mydata\\n', '!lamin "*

 * *            "init --storage mydata\\n', '!rm -r ./mydata_new_loc\\n', '!mv mydata "*

 * *            "./mydata_new_loc\\n', '!lamin close']}, 2: {'id': "*

 * *            "'33c2bb76-d61f-4866-87e2-780e61600022', 'source': ['import lamindb_setup as "*

 * *  […]*

```diff
@@ -4,126 +4,187 @@
             "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Test switch environment"
+                "# Load & close an instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
-            "metadata": {},
+            "id": "5fd65a65-5c34-462e-a980-a5aed1a2713f",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "from lamindb_setup import settings, signup, init, login\n",
-                "from lamindb_setup.dev._settings_load import load_instance_settings\n",
-                "import os"
+                "!lamin close\n",
+                "!lamin delete mydata\n",
+                "!lamin init --storage mydata\n",
+                "!rm -r ./mydata_new_loc\n",
+                "!mv mydata ./mydata_new_loc\n",
+                "!lamin close"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a9cbc2b8",
+            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "login(\"testuser1@lamin.ai\")\n",
-                "init(storage=\"mydata_prod\")\n",
-                "\n",
-                "user_access_token_prod = settings.user.access_token\n",
-                "!lamin delete mydata_prod"
+                "import lamindb_setup as ln_setup"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a5e8a0a6",
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "1be836bb",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# os.environ[\"LAMIN_ENV\"] = \"dev\"\n",
-                "\n",
-                "# login(\"testuser1@lamin.ai\", password=\"BCRRvPjzjnEW4z0Sg4ecB474CEdOeFNWG5OgTnsO\")\n",
-                "# init(storage=\"mydata_dev\")\n",
-                "\n",
-                "# user_access_token_dev = settings.user.access_token"
+                "## Load your own instance by name"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "a5c94e19",
+            "metadata": {},
+            "source": [
+                "If the user is the instance owner, load the instance by name:\n",
+                "```\n",
+                "ln_setup.load(\"mydata\")  # CLI: lamin load mydata\n",
+                "```"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "c878d40a",
+            "metadata": {},
+            "source": [
+                "You can also load with a new default storage location:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6c948145",
+            "id": "b857dc27",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# os.environ[\"LAMIN_ENV\"] = \"test\"\n",
-                "\n",
-                "# login(\"testuser1@lamin.ai\", password=\"3gYFv98ctNqYzgsf9iOrxmVUWkT2LkAD2l1V75jz\")\n",
-                "# init(storage=\"mydata_test\")\n",
-                "\n",
-                "# user_access_token_test = settings.user.access_token"
+                "ln_setup.load(\n",
+                "    \"mydata\", storage=\"./mydata_new_loc\"\n",
+                ")  # CLI: lamin load mydata --storage ./mydata_new_loc"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f63669d8",
-            "metadata": {},
+            "id": "2276e0be",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "# os.environ[\"LAMIN_ENV\"] = \"prod\"\n",
+                "from pathlib import Path\n",
                 "\n",
-                "# settings.instance.name == \"mydata_prod\"\n",
-                "# settings.user.access_token == user_access_token_prod"
+                "assert ln_setup.settings.instance.storage.is_cloud == False\n",
+                "assert ln_setup.settings.instance.name == \"mydata\"\n",
+                "assert (\n",
+                "    ln_setup.settings.instance.storage.root.as_posix()\n",
+                "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
+                ")\n",
+                "assert ln_setup.settings.instance.storage.cache_dir is None\n",
+                "assert (\n",
+                "    ln_setup.settings.instance.db\n",
+                "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/mydata.lndb\"\n",
+                ")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "914af9a6",
+            "metadata": {},
+            "source": [
+                "## Load an instance from another account"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "65ab467e",
+            "metadata": {},
+            "source": [
+                "If you have the permission, you can load an instance from another owner:\n",
+                "```\n",
+                "ln_setup.load(\"<owner>/mydata\")  # lamin load owner/mydata\n",
+                "```\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "0986a5f3",
+            "metadata": {},
+            "source": [
+                "If there is a typo, or you get the account wrong, you'll see:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "87f37005",
+            "id": "bc3568ae",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# os.environ[\"LAMIN_ENV\"] = \"dev\"\n",
-                "\n",
-                "# settings.instance.name == \"mydata_dev\"\n",
-                "# settings.user.access_token == user_access_token_dev"
+                "assert ln_setup.load(\"testuser2/mydata\") == \"instance-not-reachable\""
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "e3701120",
+            "metadata": {},
+            "source": [
+                "## Close an instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "db95be8e",
+            "id": "8e54d8cd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# os.environ[\"LAMIN_ENV\"] = \"test\"\n",
-                "\n",
-                "# settings.instance.name == \"mydata_test\"\n",
-                "# settings.user.access_token == user_access_token_test"
+                "ln_setup.close()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "26fe982b",
+            "id": "e8f70b17",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# os.environ[\"LAMIN_ENV\"] = \"prod\""
+                "!lamin delete mydata"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "base",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -133,14 +194,14 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
-                "hash": "40d3a090f54c6569ab1632332b64b2c03c39dcf918b08424e98f38b5ae0af88f"
+                "hash": "5c7b89af1651d0b8571dde13640ecdccf7d5a6204171d6ab33e7c296e100e08a"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lamindb_setup-0.46a3/docs/faq/test-migrations-e2e.ipynb` & `lamindb_setup-0.46a4/docs/guide/05-schema-modules.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8127777777777778%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}, 'source': ['# Configure schema modules'], "*

 * *            "delete: ['id']}, 1: {'cell_type': 'code', 'metadata': {replace: OrderedDict([('tags', "*

 * *            "['hide-cell'])])}, 'source': ['!lamin close\\n', '!lamin delete mydata2'], "*

 * *            "'execution_count': None, 'outputs': [], delete: ['attachments', 'id']}, 2: {'source': "*

 * *            "['import lamindb_setup as ln_setup'], delete: ['id']}, 3: {'source': ['The `bionty` "*

 * *            'schema m […]*

```diff
@@ -1,114 +1,133 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "source": [
-                "# Test migrations e2e on clones of instances"
+                "# Configure schema modules"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "78e419b6-cfe0-452f-ac8f-49adc91621df",
-            "metadata": {},
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
+            "outputs": [],
             "source": [
-                "There are two ways of invoking this functionality: `migrate_clone` and `migrate_clones`. "
+                "!lamin close\n",
+                "!lamin delete mydata2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb_setup"
+                "import lamindb_setup as ln_setup"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "119134fc-1362-4b6f-85e9-d65e5ab091cf",
             "metadata": {},
             "source": [
-                "## SQLite"
+                "The `bionty` schema module maps fundamental biological entities: https://github.com/laminlabs/lnschema-bionty\n",
+                "\n",
+                "The `lamin1` module is an example for a configurable in-house schema that tracks lab operations: https://github.com/laminlabs/lnschema-lamin1\n",
+                "\n",
+                "You can configure an arbitrary number of schema modules."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "_USE_DJANGO = True\n",
+                "\n",
+                "if not _USE_DJANGO:\n",
+                "    ln_setup.init(\n",
+                "        storage=\"mydata2\", schema=\"bionty,lamin1\"\n",
+                "    )  # CLI: lamin init --storage mydata2 --schema bionty,lamin1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2fe506c7-9788-4f04-8d12-a5a855a81db0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "if not lamindb_setup._USE_DJANGO:\n",
-                "    lamindb_setup.test.migrate_clone(storage=\"s3://lamin-site-assets\")"
+                "if not _USE_DJANGO:\n",
+                "    ln_setup.schema.draw()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "For `bionty`, supporting public ontology versions are automatically tracked:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8f16a4b4-e165-4df3-af1b-592796b9bca5",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "if not lamindb_setup._USE_DJANGO:\n",
-                "    lamindb_setup.delete(\"lamin-site-assets_test\")"
+                "from lamindb_setup.dev._setup_knowledge import load_bionty_versions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f1f43b5a-59ca-419a-8ed1-9672f2ff2025",
             "metadata": {},
             "outputs": [],
             "source": [
-                "if not lamindb_setup._USE_DJANGO:\n",
-                "    lamindb_setup.test.migrate_clones(\n",
-                "        \"lnschema_core\", n_instances=1, dialect_name=\"sqlite\"\n",
-                "    )"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "e53c8996-73a1-4c5f-b54f-4ea9ea117702",
-            "metadata": {},
-            "source": [
-                "## Postgres"
+                "if not _USE_DJANGO:\n",
+                "    load_bionty_versions(ln_setup.settings.instance, display=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cd10731f-5667-4550-99db-90fb47e92c32",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "if not lamindb_setup._USE_DJANGO:\n",
-                "    lamindb_setup.test.migrate_clone(\n",
-                "        db=\"postgresql://batman:robin@35.222.187.204:5432/lamindata\",\n",
-                "        schema=\"bionty,lamin1\",\n",
-                "    )"
+                "if not _USE_DJANGO:\n",
+                "    # clean up\n",
+                "    ln_setup.delete(\"mydata2\")\n",
+                "    # test with postgres\n",
+                "    from laminci.db import setup_local_test_postgres\n",
+                "\n",
+                "    pgurl = setup_local_test_postgres()\n",
+                "    ln_setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\", db=pgurl)\n",
+                "    !docker stop pgtest && docker rm pgtest\n",
+                "    ln_setup.delete(\"pgtest\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "py39",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -123,9 +142,9 @@
         "vscode": {
             "interpreter": {
                 "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
             }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `lamindb_setup-0.46a3/docs/guide/00-index.ipynb` & `lamindb_setup-0.46a4/docs/guide/00-index.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/docs/guide/01-setup-user.ipynb` & `lamindb_setup-0.46a4/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/docs/guide/02-init-instance.ipynb` & `lamindb_setup-0.46a4/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/docs/guide/03-load-instance.ipynb` & `lamindb_setup-0.46a4/docs/guide/04-set-storage.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9380739795918367%*

 * *Differences: {"'cells'": "{0: {'source': ['# Set storage']}, 1: {'id': '6422b64e', 'source': {insert: [(1, "*

 * *            "'!lamin delete pgtest')], delete: [5, 4, 3, 2, 1]}}, 3: {'id': 'a7cf42fb', 'source': "*

 * *            "['## Set storage']}, 6: {'cell_type': 'code', 'id': '63392da0', 'source': "*

 * *            "['ln_setup.settings.storage.root'], 'execution_count': None, 'outputs': [], delete: "*

 * *            "['attachments']}, 7: {'id': 'e6638f44', 'source': ['Local storage:']}, 9: {'id': "*

 * *            "'47b1f038', 'source […]*

```diff
@@ -4,34 +4,30 @@
             "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Load & close an instance"
+                "# Set storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5fd65a65-5c34-462e-a980-a5aed1a2713f",
+            "id": "6422b64e",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "!lamin close\n",
-                "!lamin delete mydata\n",
-                "!lamin init --storage mydata\n",
-                "!rm -r ./mydata_new_loc\n",
-                "!mv mydata ./mydata_new_loc\n",
-                "!lamin close"
+                "!lamin delete pgtest"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
@@ -39,146 +35,221 @@
             "source": [
                 "import lamindb_setup as ln_setup"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "1be836bb",
+            "id": "a7cf42fb",
             "metadata": {},
             "source": [
-                "## Load your own instance by name"
+                "## Set storage"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "a5c94e19",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8fd59ad3-04b9-42fb-83cc-ab7beedbec72",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "import laminci\n",
+                "\n",
+                "!docker stop pgtest && docker rm pgtest\n",
+                "pgurl = laminci.db.setup_local_test_postgres()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d6b0bd5e",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "If the user is the instance owner, load the instance by name:\n",
-                "```\n",
-                "ln_setup.load(\"mydata\")  # CLI: lamin load mydata\n",
-                "```"
+                "ln_setup.init(storage=\"./storage1\", db=pgurl)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "63392da0",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln_setup.settings.storage.root"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "c878d40a",
+            "id": "e6638f44",
+            "metadata": {},
+            "source": [
+                "Local storage:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "49b9ef11",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "You can also load with a new default storage location:"
+                "ln_setup.set.storage(\"./storage_2\")  # CLI: lamin set --storage ./storage_2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b857dc27",
+            "id": "47b1f038",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.load(\n",
-                "    \"mydata\", storage=\"./mydata_new_loc\"\n",
-                ")  # CLI: lamin load mydata --storage ./mydata_new_loc"
+                "ln_setup.settings.storage.root"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2276e0be",
+            "id": "8e481aa0",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
-                "assert ln_setup.settings.instance.storage.is_cloud == False\n",
-                "assert ln_setup.settings.instance.name == \"mydata\"\n",
-                "assert (\n",
-                "    ln_setup.settings.instance.storage.root.as_posix()\n",
-                "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
-                ")\n",
-                "assert ln_setup.settings.instance.storage.cache_dir is None\n",
-                "assert (\n",
-                "    ln_setup.settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/mydata.lndb\"\n",
-                ")"
+                "assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "914af9a6",
+            "id": "de1c12b8",
             "metadata": {},
             "source": [
-                "## Load an instance from another account"
+                "Cloud storage:"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "65ab467e",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8436575d",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "If you have the permission, you can load an instance from another owner:\n",
-                "```\n",
-                "ln_setup.load(\"<owner>/mydata\")  # lamin load owner/mydata\n",
-                "```\n"
+                "ln_setup.set.storage(\"s3://lndb-setup-ci\")  # lamin set --storage s3://lndb-setup-ci"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "af069899",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln_setup.settings.storage.root"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "0986a5f3",
+            "id": "859a972e",
             "metadata": {},
             "source": [
-                "If there is a typo, or you get the account wrong, you'll see:"
+                "See an overview:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bc3568ae",
-            "metadata": {},
+            "id": "d2934990",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "assert ln_setup.load(\"testuser2/mydata\") == \"instance-not-reachable\""
+                "assert ln_setup.settings.storage.is_cloud\n",
+                "assert ln_setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
+                "# root.fs contains the underlying fsspec filesystem\n",
+                "assert (\n",
+                "    ln_setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "e3701120",
+            "id": "ae953b6a",
             "metadata": {},
             "source": [
-                "## Close an instance"
+                "You can set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8e54d8cd",
+            "id": "f9294082",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.close()"
+                "ln_setup.set.storage(\"s3://lndb-setup-ci\", cache_regions=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e8f70b17",
-            "metadata": {},
+            "id": "d6915638-db49-4d3d-bd91-819bb4719ef7",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "!lamin delete mydata"
+                "# test cache_regions\n",
+                "assert not ln_setup.settings.storage.root.fs.cache_regions\n",
+                "# test setting storage not by owner\n",
+                "ln_setup.login(\n",
+                "    \"testuser2@lamin.ai\", password=\"goeoNJKE61ygbz1vhaCVynGERaRrlviPBVQsjkhz\"\n",
+                ")\n",
+                "ln_setup.set.storage(\"./storage_3\")\n",
+                "assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\"\n",
+                "!docker stop pgtest && docker rm pgtest"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "3fb6a223",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "### Currently not possible: setting storage for SQLite instance"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "6ccb6573",
+            "metadata": {},
+            "source": [
+                "If you try to set the storage for an sqlite instance, an error message is returned:\n",
+                "```\n",
+                "assert ln_setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\"\n",
+                "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -194,14 +265,14 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
-                "hash": "5c7b89af1651d0b8571dde13640ecdccf7d5a6204171d6ab33e7c296e100e08a"
+                "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lamindb_setup-0.46a3/docs/guide/migrate.md` & `lamindb_setup-0.46a4/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/__init__.py` & `lamindb_setup-0.46a4/lamindb_setup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,26 +49,21 @@
    :toctree:
 
    dev
 """
 
 import os
 
-__version__ = "0.46a3"  # denote a release candidate for 0.1.0 with 0.1rc1
-_USE_DJANGO = os.getenv("LAMINDB_USE_DJANGO") == "1"
-# _USE_DJANGO = True
-if _USE_DJANGO:
-    print("using django backend")
+__version__ = "0.46a4"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
-from . import _check_versions  # noqa
-from . import dev, test
+from . import dev
 from ._close import close  # noqa
 from ._delete import delete  # noqa
 from ._info import info  # noqa
 from ._init_instance import init  # noqa
 from ._load_instance import load  # noqa
 from ._migrate import migrate
 from ._register_instance import register  # noqa
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/__main__.py` & `lamindb_setup-0.46a4/lamindb_setup/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import argparse
-import os
-import sys
 
-from lamin_logger import logger
-
-from . import _init_instance, _setup_user, delete, info, register, set
-from ._close import close as close_instance
-from ._init_instance import description as instance
-from ._notebook import track
+# most important dynamic to optimize import time
+from ._docstrings import instance_description as instance
 from .dev._settings_user import user_description as user
 
 signup_help = "First time sign up."
 login_help = "Log in an already-signed-up user."
 init_help = "Init & config instance with db & storage."
 load_help = "Load instance by name."
 set_storage_help = "Set storage used by an instance."
@@ -82,15 +76,15 @@
 
 # register instance
 subparsers.add_parser("register", help=register_help)
 
 # migrate
 migr = subparsers.add_parser("migrate", help=migr_help)
 aa = migr.add_argument
-aa("action", choices=["generate"], help="Generate migration.")
+aa("action", choices=["create", "deploy"], help="Manage migrations.")
 
 # track anotebook (init nbproject metadata)
 track_parser = subparsers.add_parser("track", help=track_help)
 aa = track_parser.add_argument
 filepath_help = "A path to the notebook to track."
 aa("filepath", type=str, metavar="filepath", help=filepath_help)
 pypackage_help = "One or more (delimited by ',') python packages to track."
@@ -104,52 +98,70 @@
     if result in ["migrate-unnecessary", "migrate-success", "migrate-skipped", None]:
         return None  # is interpreted as success (exit code 0) by shell
     else:
         return result
 
 
 def main():
-    if os.path.basename(sys.argv[0]) == "lndb":
-        logger.warning("CLI `lndb` is deprecated, use `lamin` instead.")
     if args.command == "signup":
-        return _setup_user.signup(email=args.email)
+        from ._setup_user import signup
+
+        return signup(email=args.email)
     if args.command == "login":
-        return _setup_user.login(
+        from ._setup_user import login
+
+        return login(
             args.user,
             password=args.password,
         )
     elif args.command == "init":
-        result = _init_instance.init(
+        from ._init_instance import init
+
+        result = init(
             storage=args.storage,
             db=args.db,
             schema=args.schema,
             name=args.name,
         )
         return process_result(result)
     elif args.command == "load":
-        result = _init_instance.load(
+        from ._load_instance import load
+
+        result = load(
             identifier=args.instance,
             storage=args.storage,
         )
         return process_result(result)
     elif args.command == "close":
-        return close_instance()
+        from ._close import close
+
+        return close()
     elif args.command == "register":
+        from ._register_instance import register
+
         return register()
     elif args.command == "delete":
+        from ._delete import delete
+
         return delete(
             instance_name=args.instance,
         )
     elif args.command == "info":
+        from ._info import info
+
         return info()
     elif args.command == "set":
+        from ._set import set
+
         return set.storage(args.storage)
     elif args.command == "migrate":
-        from . import migrate
+        from ._migrate import migrate
 
-        if args.action == "generate":
-            return migrate.generate()
+        if args.action == "create":
+            return migrate.create()
+        elif args.action == "deploy":
+            return migrate.deploy()
     elif args.command == "track":
+        from ._notebook import track
+
         track(args.filepath, args.pypackage)
-    else:
-        logger.error("Invalid command. Try `lamin -h`.")
-        return 1
+    return 1
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_close.py` & `lamindb_setup-0.46a4/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_delete.py` & `lamindb_setup-0.46a4/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_init_instance.py` & `lamindb_setup-0.46a4/lamindb_setup/_init_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 import importlib
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
-from lnhub_rest.core.instance._init_instance import init_instance as init_instance_hub
-from lnhub_rest.core.instance._init_instance import validate_db_arg, validate_schema_arg
-from lnhub_rest.core.storage._add_storage import (
-    get_storage_region,
-    validate_storage_root_arg,
-)
 from pydantic import PostgresDsn
 
 from lamindb_setup.dev.upath import UPath
 
-from . import _USE_DJANGO
+from ._docstrings import instance_description as description
 from ._load_instance import load, load_from_isettings
 from ._settings import settings
 from .dev import InstanceSettings
-from .dev._db import insert_if_not_exists, upsert
 from .dev._docs import doc_args
-from .dev._setup_knowledge import write_bionty_versions
-from .dev._setup_schema import load_schema, setup_schema
+from .dev._setup_knowledge import write_bionty_versions  # noqa
+from .dev._setup_schema import load_schema
 from .dev._storage import Storage
 
 
 def register(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
-    if _USE_DJANGO:
-        from lnschema_core.models import Storage, User
+    from django.db.utils import OperationalError
+    from lnschema_core.models import Storage, User
 
+    try:
         user, created = User.objects.update_or_create(
             id=usettings.id,
             defaults=dict(
                 handle=usettings.handle,
                 name=usettings.name,
                 email=usettings.email,
             ),
         )
         if created:
             logger.success(f"Saved: {user}")
         storage, created = Storage.objects.update_or_create(
             root=isettings.storage.root_as_str,
             defaults=dict(
                 root=isettings.storage.root_as_str,
+                type=isettings.storage.type,
                 region=isettings.storage.region,
+                created_by_id=usettings.id,
             ),
         )
         if created:
             logger.success(f"Saved: {storage}")
-    else:
-        upsert.user(usettings.email, usettings.id, usettings.handle, usettings.name)
-        insert_if_not_exists.storage(isettings.storage)
+    except OperationalError as error:
+        logger.warning(f"Instance seems not set up ({error})")
+
+
+def reload_schema_modules(isettings: InstanceSettings):
+    from lnhub_rest._assets._schemas import get_schema_module_name
+
+    schema_names = ["core"] + list(isettings.schema)
+    schema_module_names = [get_schema_module_name(n) for n in schema_names]
+
+    for schema_module_name in schema_module_names:
+        if schema_module_name in sys.modules:
+            schema_module = importlib.import_module(schema_module_name)
+            importlib.reload(schema_module)
 
 
 def reload_lamindb(isettings: InstanceSettings):
     # only touch lamindb if we're operating from lamindb
-    if "lnschema_core" in sys.modules:
-        import lnschema_core
-
-        importlib.reload(lnschema_core)
+    reload_schema_modules(isettings)
     if "lamindb" in sys.modules:
         import lamindb
 
         importlib.reload(lamindb)
     else:
         # only log if we're outside lamindb
         # lamindb itself logs upon import!
@@ -82,62 +86,63 @@
 
 ERROR_SQLITE_CACHE = """
 Your cached local SQLite file exists, while your cloud SQLite file ({}) doesn't.
 Either delete your cache ({}) or add it back to the cloud (if delete was accidental).
 """
 
 
-# This provides the doc strings for the init function on the
-# CLI and the API
-# It is located here as it *mostly* parallels the InstanceSettings docstrings.
-# Small differences are on purpose, due to the different scope!
-class description:
-    storage_root = """Storage root. Either local dir, ``s3://bucket_name`` or ``gs://bucket_name``."""  # noqa
-    db = """Database connection url, do not pass for SQLite."""
-    name = """Instance name."""
-    schema = """Comma-separated string of schema modules. None if not set."""
-
-
 @doc_args(
     description.storage_root,
     description.name,
     description.db,
     description.schema,
 )
 def init(
     *,
     storage: Union[str, Path, UPath],
     name: Optional[str] = None,
     db: Optional[PostgresDsn] = None,
     schema: Optional[str] = None,
     _migrate: bool = False,  # not user-facing
     _test: bool = False,
-) -> Optional[str]:
+) -> None:
     """Creating and loading a LaminDB instance.
 
     Args:
         storage: {}
         name: {}
         db: {}
         schema: {}
     """
+    from lnhub_rest.core.instance._init_instance import (
+        init_instance as init_instance_hub,
+    )
+    from lnhub_rest.core.instance._init_instance import (
+        validate_db_arg,
+        validate_schema_arg,
+    )
+    from lnhub_rest.core.storage._add_storage import (
+        get_storage_region,
+        validate_storage_root_arg,
+    )
+
     assert settings.user.id  # check user is logged in
     owner = settings.user.handle
 
     schema = validate_schema_arg(schema)
     validate_storage_root_arg(str(storage))
     validate_db_arg(db)
 
     name_str = infer_instance_name(storage=storage, name=name, db=db)
     # test whether instance exists by trying to load it
-    message = load(
+    response = load(
         f"{owner}/{name_str}", _log_error_message=False, migrate=_migrate, _test=_test
     )
-    if message != "instance-not-reachable":
-        return message
+    if response is None:
+        return None  # successful load!
 
     isettings = InstanceSettings(
         owner=owner,
         name=name_str,
         storage_root=storage,
         storage_region=get_storage_region(storage),
         db=db,
@@ -167,46 +172,36 @@
             pass  # everything is alright!
         elif isinstance(result, str):
             raise RuntimeError(f"Creating instance on hub failed:\n{result}")
         logger.success(
             f"Registered instance on hub: https://lamin.ai/{owner}/{name_str}"
         )
     else:
-        logger.info(
-            "Not registering instance on hub, if you want, call `lamin register`"
+        logger.hint(
+            "Not registering local instance on hub, if you want, call `lamin register`"
         )
 
     if _test:
         isettings._persist()
         return None
 
-    # this does not yet setup a setup for a new database
-    persist_settings_load_schema(isettings)
-
-    message = None
     if not isettings._is_db_setup(mute=True)[0]:
-        setup_schema(isettings, settings.user)
-        register(isettings, settings.user)
-        write_bionty_versions(isettings)
-        # now ensure that everything worked
-        check, msg = isettings._is_db_setup()
-        if not check:
-            raise RuntimeError(msg)
+        load_schema(isettings, init=True)
+        register(isettings, settings.user)  # if this doesn't emit warning, we're good
+        # write_bionty_versions(isettings)
+        isettings._update_cloud_sqlite_file()
     else:
         # we're currently using this for testing migrations
         # passing connection strings of databases that need to be tested
         # for migrations
         logger.warning("Your instance seems already set up, attempt load:")
-        message = load_from_isettings(isettings, migrate=_migrate)
+        load_from_isettings(isettings, migrate=_migrate)
 
+    isettings._persist()
     reload_lamindb(isettings)
-    logger.success(
-        f"Created & loaded instance: {settings.user.handle}/{isettings.name}"
-    )
-    return message
 
 
 def infer_instance_name(
     *,
     storage: Union[str, Path, UPath],
     name: Optional[str] = None,
     db: Optional[PostgresDsn] = None,
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_load_instance.py` & `lamindb_setup-0.46a4/lamindb_setup/_load_instance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import os
 from pathlib import Path
 from typing import Optional, Union
 
-import sqlmodel as sqm
 from lamin_logger import logger
-from lnhub_rest.core.instance._load_instance import (
-    load_instance as load_instance_from_hub,
-)
 
 from lamindb_setup.dev.upath import UPath
 
-from . import _USE_DJANGO
 from ._settings import InstanceSettings, settings
 from .dev._django import setup_django
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
 from .dev._storage import StorageSettings
 
 
@@ -31,22 +26,21 @@
 
     Args:
         identifier: `str` - The instance identifier can the instance name (owner is
             current user), handle/name, or the URL: https://lamin.ai/handle/name.
         storage: `Optional[PathLike] = None` - Load the instance with an
             updated default storage.
         migrate: `Optional[bool] = None` - Whether to auto-migrate or not.
-
-    Returns:
-        - "migrate-failed" if migration failed
-        - "migrate-success" if migration was successful
-        - "migrate-unnecessary" if migration was not required
     """
     owner, name = get_owner_name_from_identifier(identifier)
 
+    from lnhub_rest.core.instance._load_instance import (
+        load_instance as load_instance_from_hub,
+    )
+
     hub_result = load_instance_from_hub(
         owner=owner, name=name, _access_token=_access_token
     )
     # if hub_result is not a string, it means it made a request
     # that successfully returned metadata
     if not isinstance(hub_result, str):
         instance_result, storage_result = hub_result
@@ -85,33 +79,27 @@
         else:
             logger.warning(
                 "Instance metadata exists, but DB might have been corrupted or deleted."
                 " Re-initializing the DB."
             )
             return "instance-not-reachable"
 
-    if _USE_DJANGO:
-        setup_django(isettings)
-    else:
-        from ._init_instance import persist_settings_load_schema
-
-        persist_settings_load_schema(isettings)
+    setup_django(isettings)
     if storage is not None and isettings.dialect == "sqlite":
-        update_storage(isettings)
+        update_root_field_in_default_storage(isettings)
 
     if not isettings.storage.root.exists():
         raise RuntimeError(
             f"Storage root does not exist: {isettings.storage.root}\n"
             "Please amend by passing --storage <my-storage-root>"
         )
 
-    message = load_from_isettings(isettings, migrate)
-    if not message == "migrate-failed":
-        os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
-    return message
+    load_from_isettings(isettings, migrate)
+    os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
+    return None
 
 
 def get_owner_name_from_identifier(identifier: str):
     if "/" in identifier:
         if identifier.startswith("https://lamin.ai/"):
             identifier = identifier.replace("https://lamin.ai/", "")
         split = identifier.split("/")
@@ -126,31 +114,22 @@
         name = identifier
     return owner, name
 
 
 def load_from_isettings(
     isettings: InstanceSettings,
     migrate: Optional[bool] = None,
-) -> Optional[str]:
+) -> None:
     from ._init_instance import persist_settings_load_schema, register, reload_lamindb
-    from ._migrate import check_deploy_migration
-    from .dev._setup_knowledge import load_bionty_versions
+    from .dev._setup_knowledge import load_bionty_versions  # noqa
 
     persist_settings_load_schema(isettings)
-    message = None
-    if not _USE_DJANGO:
-        message = check_deploy_migration(
-            usettings=settings.user, isettings=isettings, attempt_deploy=migrate
-        )
-        if message == "migrate-failed":
-            return message
     register(isettings, settings.user)
-    load_bionty_versions(isettings)
+    # load_bionty_versions(isettings)
     reload_lamindb(isettings)
-    return message
 
 
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: Union[str, Path, UPath]
 ) -> None:
     ssettings = StorageSettings(storage, instance_settings=isettings)
     if ssettings.is_cloud:
@@ -167,36 +146,25 @@
         # assumption is you want to merely update the storage location
         isettings._storage = ssettings  # need this here already
     # update isettings in place
     isettings._storage = ssettings
 
 
 # this is different from register!
-def update_storage(isettings: InstanceSettings):
-    if _USE_DJANGO:
-        from lnschema_core.models import Storage
-
-        storages = Storage.objects.all()
-        if len(storages) != 1:
-            raise RuntimeError("Can't identify which storage location to update")
-        storage = storages[0]
-        storage.root = isettings.storage.root_as_str
-        storage.save()
-    else:
-        from lnschema_core import Storage
+# register registers a new storage location
+# update_root_field_in_default_storage updates the root
+# field in the default storage locations
+def update_root_field_in_default_storage(isettings: InstanceSettings):
+    from lnschema_core.models import Storage
 
-        isettings._engine = sqm.create_engine(isettings.db)
-        with sqm.Session(isettings.engine) as session:
-            storage = session.exec(
-                sqm.select(Storage).where(Storage.root == isettings.storage.root_as_str)
-            ).one_or_none()
-        if storage is None:
-            with sqm.Session(isettings.engine) as session:
-                storage_record = session.exec(sqm.select(Storage)).one()
-                storage_record.root = isettings.storage.root_as_str
-                session.add(storage_record)
-                session.commit()
-                session.refresh(storage_record)
-            logger.success(
-                f"Updated storage root {storage_record.id} to"
-                f" {isettings.storage.root_as_str}"
-            )
+    storages = Storage.objects.all()
+    if len(storages) != 1:
+        raise RuntimeError(
+            "You have several storage locations: Can't identify in which storage"
+            " location the root column is to be updated!"
+        )
+    storage = storages[0]
+    storage.root = isettings.storage.root_as_str
+    storage.save()
+    logger.success(
+        f"Updated storage root {storage.id} to {isettings.storage.root_as_str}"
+    )
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_register_instance.py` & `lamindb_setup-0.46a4/lamindb_setup/_register_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from lamin_logger import logger
-from lnhub_rest.core.instance._init_instance import init_instance as init_instance_hub
 
 from ._settings import settings
 
 
 def register():
     """Register an instance on the hub."""
+    from lnhub_rest.core.instance._init_instance import (
+        init_instance as init_instance_hub,
+    )
+
     isettings = settings.instance
     result = init_instance_hub(
         owner=isettings.owner,
         name=isettings.name,
         storage=isettings.storage.root_as_str,
         db=isettings.db if isettings.dialect != "sqlite" else None,
         schema=isettings._schema_str,
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_schema.py` & `lamindb_setup-0.46a4/lamindb_setup/_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import sqlalchemy as sql
-
 from ._settings import settings
 
 
 class schema:
     """Inspect the schema."""
 
     @classmethod
     def draw(cls, view=True):
         """Make a diagram of entity relationships."""
         import erdiagram
+        import sqlalchemy as sa
 
         engine = settings.instance.engine
-        metadata = sql.MetaData(bind=engine)
+        metadata = sa.MetaData(bind=engine)
         metadata.reflect()
         graph = erdiagram.create_schema_graph(
             metadata=metadata,
             show_datatypes=False,
             show_indexes=False,  # ditto for indexes
             rankdir="TB",
             concentrate=False,  # Don't try to join the relation lines together
@@ -25,12 +24,14 @@
             erdiagram.view(graph)
         else:
             return graph
 
     @classmethod
     def list_entities(cls):
         """Return all entities in the db."""
-        metadata = sql.MetaData()
+        import sqlalchemy as sa
+
+        metadata = sa.MetaData()
         engine = settings.instance.engine
         metadata.reflect(bind=engine)
         table_names = [table.name for table in metadata.sorted_tables]
         return table_names
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_set.py` & `lamindb_setup-0.46a4/lamindb_setup/_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pathlib import Path
 from typing import Union
 
 from lamin_logger import logger
-from lnhub_rest.core.storage._add_storage import add_storage as add_storage_hub
 
 from lamindb_setup.dev.upath import UPath
 
 from ._init_instance import register
 from ._settings import settings
 from .dev import deprecated
 from .dev._settings_instance import InstanceSettings
@@ -27,14 +26,16 @@
 
         >>> ln.setup.set.storage(
         >>>    "s3://some-bucket",
         >>>     profile="some_profile", # fsspec arg
         >>>     cache_regions=True # fsspec arg for s3
         >>> )
         """
+        from lnhub_rest.core.storage._add_storage import add_storage as add_storage_hub
+
         if settings.instance.dialect == "sqlite":
             logger.error("Can't set storage for sqlite instances.")
             return "set-storage-failed"
 
         new_isettings = InstanceSettings(
             owner=settings.instance.owner,
             name=settings.instance.name,
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_settings.py` & `lamindb_setup-0.46a4/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/_setup_user.py` & `lamindb_setup-0.46a4/lamindb_setup/_setup_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Union
 
 from lamin_logger import logger
-from lnhub_rest.core.account._signup_signin import sign_in_hub, sign_up_hub
 
 from ._settings import settings
 from .dev._settings_load import load_or_create_user_settings, load_user_settings
 from .dev._settings_save import save_user_settings
 from .dev._settings_store import user_settings_file_email, user_settings_file_handle
 
 
 def signup(email: str) -> Union[str, None]:
     """Sign up user."""
+    from lnhub_rest.core.account._signup_signin import sign_up_hub
+
     response = sign_up_hub(email)
     if response == "handle-exists":  # handle already exists
         logger.error("The handle already exists. Please choose a different one.")
         return "handle-exists"
     if response == "user-exists":  # user already exists
         logger.error("User already exists! Please login instead: `lamin login`.")
         return "user-exists"
@@ -75,14 +76,16 @@
 
     if user_settings.password is None:
         raise RuntimeError(
             "No stored user password, please call: lamin login <your-email>"
             " --password <your-password>"
         )
 
+    from lnhub_rest.core.account._signup_signin import sign_in_hub
+
     response = sign_in_hub(
         user_settings.email, user_settings.password, user_settings.handle
     )
     if response == "could-not-login":
         return response
     elif response == "complete-signup":
         return response
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_exclusion.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Literal, Optional, Set, Tuple, Union
 
-import sqlalchemy as sa
-import sqlmodel as sqm
 from lamin_logger import logger
-from pydantic import PostgresDsn
-from sqlalchemy.future import Engine
 
-from .. import _USE_DJANGO
 from ._exclusion import empty_locker, get_locker
 from ._settings_save import save_instance_settings
 from ._settings_store import current_instance_settings_file, instance_settings_file
 from ._storage import StorageSettings
 from .upath import UPath
 
 # leave commented out until we understand more how to deal with
@@ -27,48 +22,33 @@
 # def _set_sqlite_pragma(dbapi_connection, connection_record):
 #     if isinstance(dbapi_connection, SQLite3Connection):
 #         cursor = dbapi_connection.cursor()
 #         cursor.execute("PRAGMA foreign_keys=ON;")
 #         cursor.close()
 
 
-class DjangoSession:
-    def delete(self, record):
-        record.delete()
-
-    def commit(self):
-        pass
-
-    def close(self):
-        pass
-
-    def refresh(self, record):
-        pass
-
-
 class InstanceSettings:
     """Instance settings."""
 
     def __init__(
         self,
         owner: str,  # owner handle
         name: str,  # instance name
         storage_root: Union[str, Path, UPath],  # storage location on cloud
         storage_region: Optional[str] = None,
-        db: Optional[PostgresDsn] = None,  # DB URI
+        db: Optional[str] = None,  # DB URI
         schema: Optional[str] = None,  # comma-separated string of schema names
     ):
         self._owner: str = owner
         self._name: str = name
         self._storage: StorageSettings = StorageSettings(
             storage_root, instance_settings=self, region=storage_region
         )
         self._db: Optional[str] = db
         self._schema_str: Optional[str] = schema
-        self._engine: Engine = sqm.create_engine(self.db)
 
     def __repr__(self):
         """Rich string representation."""
         representation = f"Current instance: {self.identifier}"
         attrs = ["owner", "name", "storage", "db", "schema"]
         for attr in attrs:
             value = getattr(self, attr)
@@ -117,25 +97,27 @@
     def _sqlite_file_local(self) -> Path:
         """Local SQLite file."""
         return self.storage.cloud_to_local_no_update(self._sqlite_file)
 
     def _update_cloud_sqlite_file(self) -> None:
         """Upload the local sqlite file to the cloud file."""
         if self.is_cloud_sqlite:
+            logger.info("Updating cloud sqlite file")
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.upload_from(cache_file)  # type: ignore
             cloud_mtime = sqlite_file.modified.timestamp()  # type: ignore
             # this seems to work even if there is an open connection
             # to the cache file
             os.utime(cache_file, times=(cloud_mtime, cloud_mtime))
 
     def _update_local_sqlite_file(self) -> None:
         """Download the cloud sqlite file if it is newer than local."""
         if self.is_cloud_sqlite:
+            logger.info("Updating local sqlite file")
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.synchronize(cache_file)  # type: ignore
 
     @property
     def db(self) -> str:
         """Database URL."""
@@ -152,31 +134,26 @@
         if self._db is None or self._db.startswith("sqlite://"):
             return "sqlite"
         else:
             assert self._db.startswith("postgresql")
             return "postgresql"
 
     @property
-    def engine(self) -> Engine:
+    def engine(self):
         """Database engine.
 
         In case of remote sqlite, does not update the local sqlite.
         """
-        return self._engine
+        import sqlalchemy as sa
 
-    def session(self) -> sqm.Session:
-        """Database session.
+        return sa.create_engine(self.db, future=True)
 
-        In case of remote sqlite, updates the local sqlite file first.
-        """
-        self._update_local_sqlite_file()
-        if _USE_DJANGO:
-            return DjangoSession()
-        else:
-            return sqm.Session(self.engine, expire_on_commit=False)
+    @property
+    def session(self):
+        raise NotImplementedError
 
     @property
     def is_cloud_sqlite(self) -> bool:
         # can we make this a private property, Sergei?
         # as it's not relevant to the user
         """Is this a cloud instance with sqlite db."""
         return self.dialect == "sqlite" and self.storage.is_cloud
@@ -239,15 +216,17 @@
                     False,
                     f"SQLite file {self._sqlite_file} does not exist! It should be in"
                     f" the storage root: {self.storage.root}",
                 )
             else:
                 return False, f"Connection {self.db} not reachable"
 
-        engine = sqm.create_engine(self.db)
+        import sqlalchemy as sa
+
+        engine = sa.create_engine(self.db)
         with engine.connect() as conn:
             try:  # cannot import lnschema_core here, need to use plain SQL
                 result = conn.execute(
                     sa.text("select * from lnschema_core_user")
                 ).first()
             except Exception as e:
                 return False, f"Your DB is not initialized: {e}"
@@ -262,14 +241,16 @@
     def _is_db_reachable(self, mute: bool = False) -> bool:
         if self.dialect == "sqlite":
             if not self._sqlite_file.exists():
                 if not mute:
                     logger.warning(f"SQLite file {self._sqlite_file} does not exist")
                 return False
         else:
+            import sqlalchemy as sa
+
             engine = sa.create_engine(self.db)
             try:
                 engine.connect()
             except Exception:
                 if not mute:
                     logger.warning(f"Connection {self.db} not reachable")
                 return False
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 
 def current_user_settings_file():
     return settings_dir / f"{get_settings_file_name_prefix()}current_user.env"
 
 
 def instance_settings_file(name: str, owner: str):
     return (
-        settings_dir / f"{get_settings_file_name_prefix()}{owner}-instance-{name}.env"
+        settings_dir / f"{get_settings_file_name_prefix()}instance--{owner}--{name}.env"
     )
 
 
 def user_settings_file_email(email: str):
-    return settings_dir / f"{get_settings_file_name_prefix()}user-{email}.env"
+    return settings_dir / f"{get_settings_file_name_prefix()}user--{email}.env"
 
 
 def user_settings_file_handle(handle: str):
-    return settings_dir / f"{get_settings_file_name_prefix()}user-{handle}.env"
+    return settings_dir / f"{get_settings_file_name_prefix()}user--{handle}.env"
 
 
 class InstanceSettingsStore(BaseSettings):
     owner: str
     name: str
     storage_root: str
     storage_region: str  # should be Optional, but we use types for instantiating
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_setup_knowledge.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_setup_knowledge.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from pathlib import Path
 from typing import Dict
 
-import pandas as pd
-import sqlmodel as sqm
-from IPython.display import display as ipython_display
-
-from ._db import insert
 from ._settings_instance import InstanceSettings
 
 
 def write_bionty_versions(isettings: InstanceSettings):
     """Write bionty ._current.yaml to the CurrentBiontyVersions table."""
     if "bionty" in isettings.schema:
         import bionty as bt
-        from bionty.dev._io import load_yaml
-        from lnschema_bionty import dev
-
-        basedir = Path(bt.__file__).parent / "versions"
-        _current = load_yaml(basedir / "._current.yaml")
-        local = load_yaml(Path.home() / ".lamin/bionty/versions/local.yaml")
+        from lnschema_bionty import BiontyVersions, CurrentBiontyVersions
 
-        # here we set integer ids from 0
-        records = []
-        for i, (entity, db) in enumerate(_current.items()):
-            db_name = next(iter(db))
-            db_version = db[db_name]
-            record = dev.BiontyVersions(
-                id=i,
-                entity=entity,
-                database=db_name,
-                database_v=db_version,
-                database_url=local.get(entity)
-                .get(db_name)
-                .get("versions")
-                .get(db_version)[0],
-            )
-            records.append(record)
+        columns_mapper = {
+            "bionty class": "entity",
+            "source key": "source_key",
+            "ontology": "source_name",
+        }
+
+        all_versions = bt.display_available_versions(return_df=True).reset_index()
+        all_versions.columns = all_versions.columns.str.lower()
+        all_versions.rename(columns=columns_mapper, inplace=True)
+        all_versions_dict = all_versions.to_dict(orient="records")
+
+        current_versions = bt.display_active_versions(return_df=True).reset_index()
+        current_versions.columns = current_versions.columns.str.lower()
+        current_versions.rename(columns=columns_mapper, inplace=True)
+        current_versions = current_versions.set_index(["entity", "species"])
+
+        all_records = []
+        current_records = []
+
+        for kwargs in all_versions_dict:
+            record = BiontyVersions(**kwargs)
+            all_records.append(record)
+            current = current_versions.loc[
+                (kwargs["entity"], kwargs["species"])
+            ].to_dict()
+            if (current["source_key"] == kwargs["source_key"]) and (
+                current["version"] == kwargs["version"]
+            ):
+                current_records.append(CurrentBiontyVersions(bionty_version=record))
 
-        insert.bionty_versions(records)
+        BiontyVersions.objects.bulk_create(all_records)
+        CurrentBiontyVersions.objects.bulk_create(current_records)
 
 
 def load_bionty_versions(isettings: InstanceSettings, display: bool = False):
     """Write CurrentBiontyVersions to ._lamindb_setup.yaml in bionty."""
     if "bionty" in isettings.schema:
         import bionty as bt
         from bionty.dev._io import write_yaml
@@ -51,22 +55,28 @@
 
         # these two lines help over the incomplete migration
         # of the core schema module v0.34.0 and related in lnschema_bionty
         # v0.18.0
         dev.BiontyVersions.__table__.schema = None
         dev.CurrentBiontyVersions.__table__.schema = None
 
+        import sqlalchemy as sqm  # no module-level import, not a dependency!!!
+
         stmt = sqm.select(dev.BiontyVersions).join(dev.CurrentBiontyVersions)
         with isettings.session() as ss:
             results = ss.exec(stmt).all()
         # avoid breaking change
         # if no versions were written in the db, write versions from bionty
         if len(results) == 0:
             write_bionty_versions(isettings)
         records = [row.dict() for row in results]
+
+        import pandas as pd  # no module-level import, is slow!!!
+        from IPython.display import display as ipython_display  # is slow!
+
         df = pd.DataFrame.from_records(records)
         df_lndb = df.set_index("entity")[["database", "database_v"]]
         if display:
             ipython_display(df_lndb)
         lndb_dict: Dict = {}
         for entity, db in df_lndb.iterrows():
             lndb_dict[entity] = {}
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 from pathlib import Path
 from typing import Literal, Optional, Union
 
-import sqlmodel as sqm
 from appdirs import AppDirs
 
-from .. import _USE_DJANGO
 from .upath import UPath
 
 DIRS = AppDirs("lamindb", "laminlabs")
 
 
 class StorageSettings:
     """Manage cloud or local storage settings."""
@@ -47,31 +45,22 @@
             storage_root = Path(storage).resolve()
         return storage_root
 
     @property
     def id(self) -> str:
         """Storage id."""
         if self._id is None:
-            if not _USE_DJANGO:
-                from lnschema_core import Storage
+            from lnschema_core.models import Storage
 
-                with sqm.Session(self._instance_settings.engine) as session:
-                    # needs to have been registered before!
-                    storage = session.exec(
-                        sqm.select(Storage).where(Storage.root == self.root_as_str)
-                    ).one_or_none()
-                if storage is None:
-                    raise RuntimeError(
-                        f"{self.root_as_str} wasn't registered in the db! "
-                        "Check ln.select(ln.Storage).all()"
-                    )
-            else:
-                from lnschema_core.models import Storage
-
-                storage = Storage.objects.get(root=self.root_as_str)
+            storage = Storage.objects.get(root=self.root_as_str)
+            if storage is None:
+                raise RuntimeError(
+                    f"{self.root_as_str} wasn't registered in the db! "
+                    "Check `ln.select(ln.Storage).df()`"
+                )
             self._id = storage.id
         return self._id
 
     @property
     def root(self) -> Union[Path, UPath]:
         """Root storage location."""
         return self._root
```

### Comparing `lamindb_setup-0.46a3/lamindb_setup/dev/upath.py` & `lamindb_setup-0.46a4/lamindb_setup/dev/upath.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 """
 
 import os
 from datetime import timezone
 from pathlib import Path
 from typing import Union
 
-import fsspec
 from dateutil.parser import isoparse  # type: ignore
 from lamin_logger import logger
 from upath import UPath
 
 
 def infer_filesystem(path: Union[Path, UPath, str]):
+    import fsspec  # improve cold start
+
     path_str = str(path)
 
     if isinstance(path, UPath):
         fs = path.fs
     else:
         protocol = fsspec.utils.get_protocol(path_str)
         if protocol == "s3":
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.46a4/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.46a4/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lnschema-core/.gitignore` & `lamindb_setup-0.46a4/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.46a4/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lnschema-core/LICENSE` & `lamindb_setup-0.46a4/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/lnschema-core/docs/changelog.md` & `lamindb_setup-0.46a4/lnschema-core/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+:fire: Remove unncessary files | [180](https://github.com/laminlabs/lnschema-core/pull/180) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 | 0.35a4
+♻️ Absorb `DjangoORM.create()` in `DjangoORM.__init__()` | [178](https://github.com/laminlabs/lnschema-core/pull/178) | [falexwolf](https://github.com/falexwolf) | 2023-06-03 |
+➖ Remove nbproject from code | [179](https://github.com/laminlabs/lnschema-core/pull/179) | [Koncopd](https://github.com/Koncopd) | 2023-06-03 |
+🏗️ Enable Django backend | [177](https://github.com/laminlabs/lnschema-core/pull/177) | [falexwolf](https://github.com/falexwolf) | 2023-06-02 | 0.35a3
 🚚 Rename lndb to lamindb-setup | [176](https://github.com/laminlabs/lnschema-core/pull/176) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.35a2
 🏗️ Add Django backend | [175](https://github.com/laminlabs/lnschema-core/pull/175) | [falexwolf](https://github.com/falexwolf) | 2023-05-31 | 0.35a1
 👷 Refactor CI | [174](https://github.com/laminlabs/lnschema-core/pull/174) | [falexwolf](https://github.com/falexwolf) | 2023-05-30 |
 🏗️ Remove SQL-level schema modules | [172](https://github.com/laminlabs/lnschema-core/pull/172) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.34.0
 🏗️ Introduce Django skeleton | [171](https://github.com/laminlabs/lnschema-core/pull/171) | [falexwolf](https://github.com/falexwolf) | 2023-05-24 |
 ♻️ Refactor types | [170](https://github.com/laminlabs/lnschema-core/pull/170) | [falexwolf](https://github.com/falexwolf) | 2023-05-23 |
 ♻️ Refactor `BaseORM` | [169](https://github.com/laminlabs/lnschema-core/pull/169) | [falexwolf](https://github.com/falexwolf) | 2023-05-17 | 0.33.8
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.46a4/lnschema-core/lnschema_core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,26 @@
-"""Data lineage (`yvzi`)."""
+"""Data objects & lineage (`yvzi`)."""
 _schema_id = "yvzi"
 _name = "core"
-_migration = "1c49c9f9a982"
-__version__ = "0.35a2"
+__version__ = "0.35a4"
 
 import lamindb_setup as _lamindb_setup
 from lamindb_setup._check_instance_setup import (
     check_instance_setup as _check_instance_setup,
 )
 
-try:
-    from lamindb_setup import _USE_DJANGO
-except Exception:
-    _USE_DJANGO = False
-
 _INSTANCE_SETUP = _check_instance_setup()
 
 if _INSTANCE_SETUP:
-    from . import dev, link, types
-
-    if not _USE_DJANGO:
-        from ._core import (  # type: ignore
-            Features,
-            File,
-            Folder,
-            Project,
-            Run,
-            Storage,
-            Transform,
-            User,
-        )
-        from .dev.sqlmodel import BaseORM
-        from .link import RunInput
-    else:
-        from .models import (  # type: ignore
-            BaseORM,
-            Features,
-            File,
-            Folder,
-            Project,
-            Run,
-            RunInput,
-            Storage,
-            Transform,
-            User,
-        )
+    from . import ids, types
+    from .models import (  # type: ignore
+        BaseORM,
+        Features,
+        File,
+        Folder,
+        Project,
+        Run,
+        RunInput,
+        Storage,
+        Transform,
+        User,
+    )
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.46a4/lnschema-core/lnschema_core/_lookup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import re
 from collections import namedtuple
-from typing import Any, Iterable, Optional
+from typing import Iterable, Optional
 
-from lamindb_setup import _USE_DJANGO
+from django.db import models
 
 
-def lookup(cls: Any, field: Optional[str] = None):
+def lookup(orm: models.Model, field: Optional[str] = None):
     """Lookup rows by field."""
-    import lamindb as ln
-
     if field is None:
         # by default use the name field
-        if "name" in cls.__fields__:
+        if "name" in orm.__fields__:
             field = "name"
         else:
-            non_ids = [i for i in cls.__fields__.keys() if "id" not in i]
+            non_ids = [i for i in orm.__fields__.keys() if "id" not in i]
             if len(non_ids) > 0:
                 # the first field isn't named with id
                 field = non_ids[0]
             else:
                 # the first field
-                field = next(iter(cls.__fields__.keys()))
-    if _USE_DJANGO:
-        values = set(cls.objects.values_list(field, flat=True))
-    else:
-        df = ln.select(cls).df()
-        values = set(df[field].values)
+                field = next(iter(orm.__fields__.keys()))
+    values = set(orm.objects.values_list(field, flat=True))
     for value in [None, ""]:
         if value in values:
             values.remove(value)
-    keys = to_lookup_keys(values, padding=cls.__name__)
-    nt = namedtuple_from_dict(d=dict(zip(keys, values)), name=cls.__name__)
+    keys = to_lookup_keys(values, padding=orm.__name__)
+    nt = namedtuple_from_dict(d=dict(zip(keys, values)), name=orm.__name__)
     return nt
 
 
 def to_lookup_keys(x: Iterable[str], padding: str = "LOOKUP") -> list:
     """Convert a list of strings to tab-completion allowed formats."""
     lookup = [re.sub("[^0-9a-zA-Z]+", "_", str(i)) for i in x]
     for i, value in enumerate(lookup):
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/lnschema_core/_types.py` & `lamindb_setup-0.46a4/lnschema-core/lnschema_core/_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from enum import Enum
 from pathlib import Path
-from typing import Callable, TypeVar
+from typing import Any, TypeVar
 
-import anndata as ad
-import numpy as np
-import pandas as pd
-from lamindb_setup.dev.upath import UPath
-from sqlalchemy.orm.attributes import InstrumentedAttribute
+from upath import UPath
 
 PathLike = TypeVar("PathLike", str, Path, UPath)
-DataLike = TypeVar("DataLike", ad.AnnData, pd.DataFrame)
-ListLike = TypeVar("ListLike", pd.Series, list, np.array)
-SQLModelField = TypeVar("SQLModelField", Callable, InstrumentedAttribute)
+# statically typing the following is hard because these are all heavy dependencies, even DataFrame is heavy & slow to import
+DataLike = Any
 
 
 class Usage(str, Enum):
     """Data access types."""
 
     ingest = "ingest"
     insert = "insert"
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/_id.py` & `lamindb_setup-0.46a4/lnschema-core/lnschema_core/ids.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+"""IDs.
+
+See: https://github.com/laminlabs/lamin-notes/blob/main/docs/2022/ids.ipynb
+
+Base generators:
+
+.. autosummary::
+   :toctree: .
+
+   base26
+   base62
+   base64
+
+Entity-related generators:
+
+.. autosummary::
+   :toctree: .
+
+   schema
+   user
+   instance
+   storage
+   file
+   folder
+   run
+   transform
+   project
+   secret
+"""
 # Some IDs got updated on 2023-02-14 to be multiples of 4
 # for matching byte representation, should we ever go there.
 import secrets
 import string
 
 
 def base64(n_char: int) -> str:
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.46a4/lnschema-core/lnschema_core/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,48 @@
+import builtins
 from pathlib import Path, PurePosixPath
-from typing import Any, List, NamedTuple, Optional, Union
+from typing import Any, Iterable, List, NamedTuple, Optional, Union
 
 import pandas as pd
 from django.db import models
 from lamin_logger import logger
-from nbproject._is_run_from_ipython import is_run_from_ipython
 from upath import UPath
 
+from . import ids
 from ._lookup import lookup as _lookup
 from ._users import current_user_id
-from .dev import id as idg
-from .types import DataLike, ListLike, PathLike, TransformType
+from .types import DataLike, PathLike, TransformType
+
+is_run_from_ipython = getattr(builtins, "__IPYTHON__", False)
 
 
 class NoResultFound(Exception):
     pass
 
 
 class MultipleResultsFound(Exception):
     pass
 
 
 class LaminQuerySet(models.QuerySet):
+    """Extension of Django QuerySet.
+
+    This brings some of the SQLAlchemy/SQLModel/SQL-inspired calls.
+
+    As LaminDB was based on SQLAlchemy/SQLModel in the beginning, and might
+    support it again in the future, these calls will be supported longtime.
+    """
+
     def df(self):
-        return pd.DataFrame(self.values())
+        df = pd.DataFrame(self.values())
+        if "id" in df.columns:
+            df = df.set_index("id")
+        return df
 
-    def list(self):
+    def list(self) -> List:
         return list(self)
 
     def first(self):
         if len(self) == 0:
             return None
         return self[0]
 
@@ -71,151 +84,192 @@
     file = models.ForeignKey("File", on_delete=models.CASCADE)
 
     class Meta:
         managed = True
 
 
 class User(BaseORM):
+    """User accounts.
+
+    All data in this table is synched from the cloud user account to ensure a
+    globally unique user identity.
+    """
+
     id = models.CharField(max_length=8, primary_key=True)
     email = models.CharField(max_length=64, unique=True)
     handle = models.CharField(max_length=64, unique=True)
     name = models.CharField(max_length=64, blank=True, null=True)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         managed = True
 
 
 class Storage(BaseORM):
-    id = models.CharField(max_length=8, default=idg.storage, primary_key=True)
+    """Storage locations, often object storage buckets.
+
+    A file or run-associated file can be stored in any desired S3,
+    GCP bucket or local storage location.
+
+    This table tracks these locations along with metadata.
+    """
+
+    id = models.CharField(max_length=8, default=ids.storage, primary_key=True)
     root = models.CharField(max_length=255)
+    """Path to the root of the storage location: an s3 path, a local path, etc."""
     type = models.CharField(max_length=63, blank=True, null=True)
+    """Local vs. s3 vs. gcp etc."""
     region = models.CharField(max_length=63, blank=True, null=True)
+    """Cloud storage region, if applicable."""
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
     created_by = models.ForeignKey(User, models.DO_NOTHING, blank=True, null=True, default=current_user_id)
 
     class Meta:
         managed = True
 
 
 class Project(BaseORM):
-    id = models.CharField(max_length=8, default=idg.project, primary_key=True)
+    """Projects."""
+
+    id = models.CharField(max_length=8, default=ids.project, primary_key=True)
     name = models.CharField(max_length=64)
     folders = models.ManyToManyField("Folder")
     files = models.ManyToManyField("File")
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         managed = True
 
 
 class Transform(BaseORM):
-    name = models.CharField(max_length=127)
-    hash = models.CharField(max_length=12, default=idg.transform)
+    """Data transformations.
+
+    Jupyter notebooks, pipelines, and apps.
+
+    A pipeline is typically versioned software that can perform a data
+    transformation/processing workflow. This can be anything from typical
+    workflow tools (Nextflow, Snakemake, Prefect, Apache Airflow, etc.) to
+    simple (versioned) scripts.
+
+    Data can also be ingested & transformed through an app.
+    """
+
+    name = models.CharField(max_length=255)
+    """A name for the transform, a pipeline name, or a file name of a notebook or script.
+    """
+    hash = models.CharField(max_length=12, default=ids.transform)
     version = models.CharField(max_length=10, default="0")
+    """Version identifier, defaults to `"0"`.
+
+    Use this to label different versions of the same transform.
+
+    Consider using `semantic versioning <https://semver.org>`__
+    with `Python versioning <https://peps.python.org/pep-0440/>`__.
+    """
     type = models.CharField(max_length=63, choices=TransformType.choices(), db_index=True, default=(TransformType.notebook if is_run_from_ipython else TransformType.pipeline))
-    title = models.CharField(max_length=63, blank=True, null=True)
-    reference = models.CharField(max_length=63, blank=True, null=True)
+    """Transform type. Defaults to `notebook` if run from IPython, otherwise to `pipeline`.
+    """
+    title = models.TextField(blank=True, null=True)
+    """An additional title, like a notebook title.
+    """
+    reference = models.CharField(max_length=255, blank=True, null=True)
+    """Reference for the transform, e.g., a URL.
+    """
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         managed = True
         unique_together = (("name", "version"),)
 
 
 class Run(BaseORM):
-    id = models.CharField(max_length=12, default=idg.run, primary_key=True)
+    """Runs of data transforms.
+
+    A `run` is any transform of a `file`.
+
+    Args:
+        id: Optional[str] = None
+        name: Optional[str] = None
+        load_latest: bool = False - Load latest run for given notebook or pipeline.
+        transform: Optional[Transform] = None
+        inputs: List[File] = None
+        outputs: List[File] = None
+
+    It typically has inputs and outputs:
+
+    - References to outputs are stored in the `file` table in the
+      `run_id` column as a foreign key the `run`
+      table. This is possible as every given `file` has a unique data run:
+      the `run` that produced the `file`. However, note that a given
+      `run` may output several `files`.
+    - References to inputs are stored in the `run_in` table, a
+      many-to-many link table between the `file` and `run` tables. Any
+      `file` might serve as an input for many `runs`. Similarly, any
+      `run` might have many `files` as inputs.
+    """
+
+    id = models.CharField(max_length=12, default=ids.run, primary_key=True)
     name = models.CharField(max_length=255, blank=True, null=True)
     external_id = models.CharField(max_length=255, blank=True, null=True)
     transform = models.ForeignKey(Transform, models.DO_NOTHING)
     inputs = models.ManyToManyField("File", through=RunInput, related_name="input_of")
     # outputs on File
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now_add=True)
 
     class Meta:
         managed = True
 
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *,
-        id: Optional[str] = None,
-        name: Optional[str] = None,
-        load_latest: bool = False,
-        external_id: Optional[str] = None,
-        transform: Optional[Transform] = None,
-        inputs: List["File"] = None,
-        outputs: List["File"] = None,
-    ):
-        kwargs = {k: v for k, v in locals().items() if v and k != "self"}
 
-        import lamindb as ln
+class Features(BaseORM):
+    """Feature sets.
 
-        global_context = False
-        if transform is None:
-            if ln.context.transform is not None:
-                global_context = True
-                transform = ln.context.transform
-            else:
-                raise ValueError("Either call `ln.Run(transform=transform)` or `ln.track(transform=...)`.")
+    A feature set is represented by the hash of the set of primary keys and the feature type.
 
-        if not isinstance(transform, Transform):
-            raise TypeError("transform needs to be of type Transform")
+    The current supported feature types are lnschema_bionty.Gene,
+    lnschema_bionty.Protein & lnschema_bionty.CellMarker.
 
-        run = None
-        if load_latest:
-            run = ln.select(ln.Run, transform=transform).order_by("-created_at").first()
-            if run is not None:
-                logger.info(f"Loaded: {run}")
-        elif id is not None:
-            run = ln.select(ln.Run, id=id).one_or_none()
-            if run is None:
-                raise NotImplementedError("You can currently only pass existing ids")
-
-        if run is None:
-            kwargs["transform_id"] = transform.id
-            if "load_latest" in kwargs:
-                del kwargs["load_latest"]
-            del kwargs["cls"]
-            run = cls(**kwargs)
-            run._ln_identity_key = None
-        else:
-            run = cls(**run.dict())
-            run._ln_identity_key = run.id  # simulate query result
+    Guides:
 
-        if global_context:
-            if run is None:
-                added_self = ln.add(run)
-                run._ln_identity_key = added_self.id  # type: ignore
-                logger.success(f"Saved: {run}")
-            ln.context.run = run
+    - :doc:`/guide/scrna`
+    - :doc:`guide/flow`
 
-        return run
+    Examples:
 
+    >>> import lnschema_bionty as bt
+    >>> reference = bt.Gene(species="mouse")
+    >>> features = ln.Features(adata, reference=reference)
+    >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq", features=features)
+
+    Args:
+        data: [Path, str, pd.DataFrame, ad.AnnData] - DataFrame or AnnData to parse.
+        reference: Any = None - Reference for mapping features.
+        id: str = None - Primary key.
+        type: Any = None - Type of reference.
+        files: List[File] - Files to link against.
+    """
 
-class Features(BaseORM):
     id = models.CharField(max_length=63, primary_key=True)
     type = models.CharField(max_length=63)
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now=True)
     files = models.ManyToManyField("File")
 
     class Meta:
         managed = True
 
     def __init__(  # type: ignore
         self,
-        iterable: ListLike = None,
+        iterable: Iterable = None,
         field: models.CharField = None,
         *,
         id: str = None,
         type: Any = None,
         # continue with fields
         files: List["File"] = [],
         **map_kwargs,
@@ -229,15 +283,15 @@
             kwargs.pop("iterable")
 
         kwargs = {k: v for k, v in kwargs.items() if v and k != "self"}
         super().__init__(**kwargs)
 
     def __new__(
         cls,
-        iterable: ListLike = None,
+        iterable: Iterable = None,
         field: models.CharField = None,
         *,
         id: str = None,
         type: Any = None,
         # continue with fields
         files: List["File"] = [],
         **map_kwargs,
@@ -289,57 +343,74 @@
         return tree(
             dir_path=self.path(),
             level=level,
             limit_to_directories=limit_to_directories,
             length_limit=length_limit,
         )
 
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        path: Optional[Union[Path, UPath, str]] = None,
-        *,
-        # continue with fields
-        name: Optional[str] = None,
-        key: Optional[str] = None,
-        storage_id: Optional[str] = None,
-        files: List["File"] = [],
-    ):
-        if path is not None:
-            from lamindb._folder import get_folder_kwargs_from_data
+    def __init__(self, *args, **kwargs):  # type: ignore
+        if len(args) > 1 and isinstance(args[0], str) and len(args[0]) == 20:  # initialize with all fields from db as args
+            super().__init__(*args, **kwargs)
+            return None
+        else:  # user-facing calling signature
+            if len(args) != 1 and "files" not in kwargs:
+                raise ValueError("Either provide path as arg or provide files as kwarg!")
+            if len(args) == 1:
+                path: Optional[Union[Path, UPath, str]] = args[0]
+            else:
+                path = None
+            name: Optional[str] = kwargs.pop("name") if "name" in kwargs else None
+            key: Optional[str] = kwargs.pop("key") if "key" in kwargs else None
+            files: Optional[str] = kwargs.pop("files") if "files" in kwargs else None
+            if len(kwargs) != 0:
+                raise ValueError(f"This kwargs are not permitted: {kwargs}")
 
+        from lamindb._folder import get_folder_kwargs_from_data
+
+        if path is not None:
             kwargs, privates = get_folder_kwargs_from_data(
                 path=path,
                 name=name,
                 key=key,
             )
+            files = kwargs.pop("files")
         else:
-            kwargs = {k: v for k, v in locals().items() if v and k != "self"}
-        kwargs["id"] = idg.folder()
-
-        files = kwargs.pop("files")
-
-        folder = cls(**kwargs)
+            kwargs = dict(name=name)
+        kwargs["id"] = ids.folder()
+        super().__init__(**kwargs)
         if path is not None:
-            folder._local_filepath = privates["local_filepath"]
-            folder._cloud_filepath = privates["cloud_filepath"]
-            folder._files = files
-        return folder
+            self._local_filepath = privates["local_filepath"]
+            self._cloud_filepath = privates["cloud_filepath"]
+            self._files = files
 
 
 class File(BaseORM):
-    id = models.CharField(max_length=20, primary_key=True)
+    id: str = models.CharField(max_length=20, primary_key=True)
     name = models.CharField(max_length=255, blank=True, null=True)
     suffix = models.CharField(max_length=63, blank=True, null=True)
+    """Suffix to construct the storage key. Defaults to `None`.
+
+    This is a file extension if the `file` is stored in a file format.
+    It's `None` if the storage format doesn't have a canonical extension.
+    """
     size = models.BigIntegerField(blank=True, null=True)
+    """Size in bytes.
+
+    Examples: 1KB is 1e3 bytes, 1MB is 1e6, 1GB is 1e9, 1TB is 1e12 etc.
+    """
     hash = models.CharField(max_length=63, blank=True, null=True)
+    """Hash (md5)."""
     key = models.CharField(max_length=255, blank=True, null=True)
+    """Storage key, the relative path within the storage location."""
     run = models.ForeignKey(Run, models.DO_NOTHING, blank=True, null=True, related_name="outputs")
+    """:class:`~lamindb.Run` that created the `file`."""
     transform = models.ForeignKey(Transform, models.DO_NOTHING, blank=True, null=True)
-    storage = models.ForeignKey(Storage, models.DO_NOTHING)
+    """:class:`~lamindb.Transform` whose run created the `file`."""
+    storage: "Storage" = models.ForeignKey(Storage, models.DO_NOTHING)
+    """:class:`~lamindb.Storage` location of `file`, see `.path()` for full path."""
     # folders from Folders.files
     # features from Features.files
     # input_of from Run.inputs
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
 
@@ -405,32 +476,33 @@
         self._memory_rep = privates["memory_rep"]
         self._to_store = not privates["check_path_in_storage"]  # no need to upload if new file is already in storage
 
     @property
     def __name__(cls) -> str:
         return "File"
 
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        data: Union[PathLike, DataLike] = None,
-        *,
-        key: Optional[str] = None,
-        name: Optional[str] = None,
-        run: Optional[Run] = None,
-        format: Optional[str] = None,
-        features: List[Features] = None,
-        input_of: List[Run] = None,
+    def __init__(  # type: ignore
+        self,
+        *args,
+        **kwargs,
     ):
-        if features is None:
-            features = []
-        if input_of is None:
-            input_of = []
-        if not isinstance(features, List):
-            features = [features]
+        if len(args) > 1 and isinstance(args[0], str) and len(args[0]) == 20:  # initialize with all fields from db as args
+            super().__init__(*args, **kwargs)
+            return None
+        else:  # user facing calling signature
+            if len(args) > 1:
+                raise ValueError("Only one non-keyword arg allowed")
+            if len(args) == 0:
+                data: Union[PathLike, DataLike] = kwargs["data"]
+            else:
+                data: Union[PathLike, DataLike] = args[0]
+            key: Optional[str] = kwargs["key"] if "key" in kwargs else None
+            name: Optional[str] = kwargs["name"] if "name" in kwargs else None
+            run: Optional[Run] = kwargs["run"] if "run" in kwargs else None
+            format = kwargs["format"] if "format" in kwargs else None
 
         def log_hint(*, check_path_in_storage: bool, key: str, id: str, suffix: str) -> None:
             hint = ""
             if check_path_in_storage:
                 hint += "file in storage ✓"
             else:
                 hint += "file will be copied to storage upon `ln.add()`"
@@ -445,17 +517,15 @@
         kwargs, privates = get_file_kwargs_from_data(
             data=data,
             name=name,
             key=key,
             run=run,
             format=format,
         )
-        kwargs["id"] = idg.file()
-        if features is not None:
-            kwargs["features"] = features
+        kwargs["id"] = ids.file()
         log_hint(
             check_path_in_storage=privates["check_path_in_storage"],
             key=kwargs["key"],
             id=kwargs["id"],
             suffix=kwargs["suffix"],
         )
 
@@ -468,21 +538,20 @@
             else:
                 # accessing the relationship should always be possible if
                 # the above if clause was false as then, we should have a fresh
                 # Transform object that is not queried from the DB
                 assert kwargs["run"].transform is not None
                 kwargs["transform"] = kwargs["run"].transform
 
-        file = cls(**kwargs)
+        super().__init__(**kwargs)
         if data is not None:
-            file._local_filepath = privates["local_filepath"]
-            file._cloud_filepath = privates["cloud_filepath"]
-            file._memory_rep = privates["memory_rep"]
-            file._to_store = not privates["check_path_in_storage"]
-        return file
+            self._local_filepath = privates["local_filepath"]
+            self._cloud_filepath = privates["cloud_filepath"]
+            self._memory_rep = privates["memory_rep"]
+            self._to_store = not privates["check_path_in_storage"]
 
     def save(self, *args, **kwargs):
         if self.transform is not None:
             self.transform.save()
         if self.run is not None:
             self.run.save()
         super().save(*args, **kwargs)
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/noxfile.py` & `lamindb_setup-0.46a4/lnschema-core/noxfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     run_pre_commit(session)
 
 
 @nox.session
 def install(session: nox.Session) -> None:
     session.run(*"pip install --no-deps .[django]".split())
     session.run(*"git clone --no-single-branch --depth 1 https://github.com/laminlabs/lamindb".split())
-    response = requests.get("https://github.com/laminlabs/lamindb/tree/rename")
+    response = requests.get("https://github.com/laminlabs/lamindb/tree/cleanup")
     if response.status_code < 400:
         with session.chdir("./lamindb"):
-            session.run(*"git switch rename".split())
+            session.run(*"git switch cleanup".split())
     if sys.platform.startswith("linux"):  # remove version pin when running on CI
         session.run(*"sed -i /lnschema_core/d ./lamindb/pyproject.toml".split())
     session.run(*"pip install ./lamindb[aws,test]".split())
 
 
 @nox.session()
 def build(session: nox.Session) -> None:
```

### Comparing `lamindb_setup-0.46a3/lnschema-core/pyproject.toml` & `lamindb_setup-0.46a4/lnschema-core/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,31 +11,26 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "lamindb_setup",
-    "anndata",
-    "sqlmodel>=0.0.8",
-    "sqlalchemy>=1.4.41",
-    "pydantic<2.0.0",
-    "typeguard<3.0.0",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnschema-core"
 
 [project.optional-dependencies]
 test = [
     "pre-commit",
     "nox",
+    "laminci",
     "pytest>=6.0",
     "pytest-cov",
-    "pytest_alembic",
     "nbproject-test",
 ]
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
```

### Comparing `lamindb_setup-0.46a3/noxfile.py` & `lamindb_setup-0.46a4/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 import nox
-from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_artifact
+from laminci import upload_docs_artifact
 from laminci.nox import build_docs, login_testuser1, login_testuser2, run_pre_commit
 
 nox.options.default_venv_backend = "none"
 
 
 LAMIN_ENV = "prod"
 if "GITHUB_REF_NAME" in os.environ:
@@ -23,19 +23,17 @@
 def lint(session: nox.Session) -> None:
     run_pre_commit(session)
 
 
 @nox.session
 @nox.parametrize(
     "group",
-    ["unit", "docs", "unit-django", "docs-django"],
+    ["unit", "docs"],
 )
 def install(session: nox.Session, group: str) -> None:
-    if "django" in group:
-        session.run(*"pip install django dj_database_url".split())
     session.run(*"pip install bionty".split())
     session.run(*"pip install --no-deps lnschema_bionty".split())
     session.run(
         *"pip install --no-deps git+https://github.com/laminlabs/lnschema-lamin1"
         .split()
     )
     # install lnschema-core from sub-module
@@ -43,27 +41,24 @@
     # install lamindb-setup without deps
     session.run(*"pip install .[aws,test]".split())
 
 
 @nox.session
 @nox.parametrize(
     "group",
-    ["unit", "docs", "unit-django", "docs-django"],
+    ["unit", "docs"],
 )
 def build(session: nox.Session, group: str):
     login_testuser1(session, env=env)
     login_testuser2(session, env=env)
-    if "django" in group:
-        os.environ["LAMINDB_USE_DJANGO"] = "1"
-        env["LAMINDB_USE_DJANGO"] = "1"
     coverage_args = "--cov=lamindb_setup --cov-append --cov-report=term-missing"  # noqa
     if group.startswith("unit"):
         session.run(*f"pytest -s {coverage_args} ./tests".split(), env=env)
     elif group.startswith("docs"):
         session.run(*f"pytest -s {coverage_args} ./docs".split(), env=env)
 
 
 @nox.session
 def docs(session: nox.Session):
+    session.run(*"lamin init --storage ./docsbuild".split())
     build_docs(session)
     upload_docs_artifact()
-    move_built_docs_to_docs_slash_project_slug()
```

### Comparing `lamindb_setup-0.46a3/pyproject.toml` & `lamindb_setup-0.46a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,44 +7,42 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.8",
-    "lndb",  # this is just until lnhub_rest is decoupled from lndb
+    "lnhub_rest==0.9.10",
+    "sqlmodel",  # this here just for lnhub_rest
     # NO other Lamin packages should be pinned or even be a dependency
-    "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.35a1",
-    "lamin_logger>=0.2.3",
+    "lamin_logger>=0.3.3",
     # External dependencies
-    "pytest_alembic==0.9.1",  # let's pin this as we use internals
-    "psycopg2-binary",
+    "django",
+    "dj_database_url",
+    "pydantic[dotenv]",
+    "ipython",
+    "sqlalchemy",  # just temporarily
     "appdirs",
-    "python-dotenv",
-    "erdiagram",
-    "alembic",
-    "natsort",
-    "pandas",
+    "pandas",  # remove!!!
     "python-dateutil",
     "universal_pathlib"
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lamindb-setup"
 
 [project.optional-dependencies]
 aws = [
     "s3fs",
 ]
-django = [
-    "django",
-]
 test = [
+    "psycopg2-binary",
+    "python-dotenv",
+    "erdiagram",
     "pre-commit",
     "nox",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test>=0.4.3",
 ]
```

### Comparing `lamindb_setup-0.46a3/tests/test_bionty.py` & `lamindb_setup-0.46a4/tests/test_bionty.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sqlmodel as sqm
 
 import lamindb_setup as ln_setup
 
 
 def test_init_bionty():
-    if not ln_setup._USE_DJANGO:
+    _USE_DJANGO = True
+    if not _USE_DJANGO:
         ln_setup.login(
             "testuser1@lamin.ai", password="cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS"
         )
         ln_setup.init(storage="test-bionty", schema="bionty")
 
         import lnschema_bionty
```

### Comparing `lamindb_setup-0.46a3/tests/test_init_instance.py` & `lamindb_setup-0.46a4/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/tests/test_load_instance.py` & `lamindb_setup-0.46a4/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a3/PKG-INFO` & `lamindb_setup-0.46a4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.46a3
+Version: 0.46a4
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.9.8
-Requires-Dist: lndb
-Requires-Dist: laminci>=0.3.0
+Requires-Dist: lnhub_rest==0.9.10
+Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35a1
-Requires-Dist: lamin_logger>=0.2.3
-Requires-Dist: pytest_alembic==0.9.1
-Requires-Dist: psycopg2-binary
+Requires-Dist: lamin_logger>=0.3.3
+Requires-Dist: django
+Requires-Dist: dj_database_url
+Requires-Dist: pydantic[dotenv]
+Requires-Dist: ipython
+Requires-Dist: sqlalchemy
 Requires-Dist: appdirs
-Requires-Dist: python-dotenv
-Requires-Dist: erdiagram
-Requires-Dist: alembic
-Requires-Dist: natsort
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: universal_pathlib
 Requires-Dist: s3fs ; extra == "aws"
-Requires-Dist: django ; extra == "django"
+Requires-Dist: psycopg2-binary ; extra == "test"
+Requires-Dist: python-dotenv ; extra == "test"
+Requires-Dist: erdiagram ; extra == "test"
 Requires-Dist: pre-commit ; extra == "test"
 Requires-Dist: nox ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lamindb-setup
 Provides-Extra: aws
-Provides-Extra: django
 Provides-Extra: test
 
+[![codecov](https://codecov.io/gh/laminlabs/lamindb-setup/branch/main/graph/badge.svg)](https://codecov.io/gh/laminlabs/lamindb-setup)
+
 # lamindb-setup: Setup LaminDB
 
 - Stable user docs: [lamin.ai/docs/setup/](https://lamin.ai/docs/setup/)
 - Latest developer docs: [netlify](https://lndb-htry.netlify.app/docs/lndb/)
```

