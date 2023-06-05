# Comparing `tmp/taipy-core-2.3.0.dev0.tar.gz` & `tmp/taipy-core-2.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.3.0.dev0.tar", last modified: Tue May 23 20:17:16 2023, max compression
+gzip compressed data, was "taipy-core-2.3.0.dev1.tar", last modified: Mon Jun  5 16:01:49 2023, max compression
```

## Comparing `taipy-core-2.3.0.dev0.tar` & `taipy-core-2.3.0.dev1.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.512005 taipy-core-2.3.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.512005 taipy-core-2.3.0.dev0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_backup/_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_core_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_labeled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_submittable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/_bcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/default_custom_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/_core_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.524005 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    40959 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.524005 taipy-core-2.3.0.dev0/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/cycle_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/abstract_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/data_node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/job_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/core_event_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/registration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.532005 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/pipeline_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.532005 taipy-core-2.3.0.dev0/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:17:09.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    29447 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.848070 taipy-core-2.3.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.848070 taipy-core-2.3.0.dev1/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_backup/_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_core_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_labeled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_submittable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_abstract_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_bcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/default_custom_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/warn_if_inputs_not_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/_core_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.860070 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_config_id_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40959 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.860070 taipy-core-2.3.0.dev1/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/data_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/core_event_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.868070 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.868070 taipy-core-2.3.0.dev1/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.868070 taipy-core-2.3.0.dev1/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:42.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29447 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/tests/test_taipy.py
```

### Comparing `taipy-core-2.3.0.dev0/LICENSE` & `taipy-core-2.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/PKG-INFO` & `taipy-core-2.3.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev0
+Version: 2.3.0.dev1
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev0/README.md` & `taipy-core-2.3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/setup.py` & `taipy-core-2.3.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_backup/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_backup/_backup.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_backup/_backup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 
 import os
-import pathlib
 
 __BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME = "TAIPY_BACKUP_FILE_PATH"
 
 
-def append_to_backup_file(new_file_path: str):
+def _append_to_backup_file(new_file_path: str):
     if preserve_file_path := os.getenv(__BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME):
         with open(preserve_file_path, "a") as f:
             f.write(f"{new_file_path}\n")
 
 
-def remove_from_backup_file(to_remove_file_path: str):
+def _remove_from_backup_file(to_remove_file_path: str):
     preserve_file_path = os.getenv(__BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME, None)
     if preserve_file_path:
         try:
             with open(preserve_file_path, "r+") as f:
                 old_backup = f.read()
                 to_remove_file_path = to_remove_file_path + "\n"
 
@@ -41,10 +40,10 @@
                     f.seek(0)
                     f.write(new_backup)
                     f.truncate()
         except Exception:
             pass
 
 
-def replace_in_backup_file(old_file_path: str, new_file_path: str):
-    remove_from_backup_file(old_file_path)
-    append_to_backup_file(new_file_path)
+def _replace_in_backup_file(old_file_path: str, new_file_path: str):
+    _remove_from_backup_file(old_file_path)
+    _append_to_backup_file(new_file_path)
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_core.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_core.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_core_cli.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_core_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_entity/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_dag.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_dag.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_entity.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_entity_ids.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_labeled.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_labeled.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_reload.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_reload.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_submittable.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_submittable.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_manager/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_abstract_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_repository/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/_bcolor.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_bcolor.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/_version_cli.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_utils.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/common/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/common/_listattributes.py` & `taipy-core-2.3.0.dev1/src/taipy/core/common/_listattributes.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/common/_repr_enum.py` & `taipy-core-2.3.0.dev1/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/common/_utils.py` & `taipy-core-2.3.0.dev1/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/common/_warnings.py` & `taipy-core-2.3.0.dev1/src/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/common/default_custom_document.py` & `taipy-core-2.3.0.dev1/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py` & `taipy-core-2.3.0.dev1/src/taipy/core/common/warn_if_inputs_not_ready.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from taipy.config.checker._checker import _Checker
 from taipy.config.common.frequency import Frequency  # type: ignore
 from taipy.config.common.scope import Scope  # type: ignore
 from taipy.config.config import Config  # type: ignore
 from taipy.config.global_app.global_app_config import GlobalAppConfig  # type: ignore
 
 from ._core_section import CoreSection
+from .checkers import _global_config_checker
 from .checkers._config_id_checker import _ConfigIdChecker
 from .checkers._data_node_config_checker import _DataNodeConfigChecker
 from .checkers._job_config_checker import _JobConfigChecker
 from .checkers._pipeline_config_checker import _PipelineConfigChecker
 from .checkers._scenario_config_checker import _ScenarioConfigChecker
 from .checkers._task_config_checker import _TaskConfigChecker
 from .data_node_config import DataNodeConfig
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/_core_section.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/_core_section.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_config_id_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,20 @@
         if not isinstance(data_node_config.scope, Scope):
             self._error(
                 data_node_config._SCOPE_KEY,
                 data_node_config.scope,
                 f"`{data_node_config._SCOPE_KEY}` field of DataNodeConfig `{data_node_config_id}` must be"
                 f" populated with a Scope value.",
             )
+        if data_node_config.scope == Scope.PIPELINE:
+            self._warning(
+                data_node_config._SCOPE_KEY,
+                data_node_config.scope,
+                f"`{Scope.PIPELINE}` is deprecated. Please use other `Scope` value instead.",
+            )
 
     def _check_required_properties(self, data_node_config_id: str, data_node_config: DataNodeConfig):
         if storage_type := data_node_config.storage_type:
             if storage_type in DataNodeConfig._REQUIRED_PROPERTIES:
                 required_properties = DataNodeConfig._REQUIRED_PROPERTIES[storage_type]
                 if storage_type == DataNodeConfig._STORAGE_TYPE_VALUE_SQL:
                     if data_node_config.properties:
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/config.schema.json` & `taipy-core-2.3.0.dev1/src/taipy/core/config/config.schema.json`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/data_node_config.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/data_node_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/job_config.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/job_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/pipeline_config.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/pipeline_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing import Any, Dict, List, Optional, Union
 
 from taipy.config._config import _Config
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 from taipy.config.config import Config
 from taipy.config.section import Section
 
+from ..common._warnings import _warn_deprecated
 from .task_config import TaskConfig
 
 
 class PipelineConfig(Section):
     """
     Configuration fields needed to instantiate an actual `Pipeline^`.
 
@@ -92,14 +93,15 @@
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new pipeline configuration.
         """
         section = PipelineConfig(id, task_configs, **properties)
         Config._register(section)
+        _warn_deprecated("PipelineConfig")
         return Config.sections[PipelineConfig.name][id]
 
     @staticmethod
     def _configure_default(task_configs: Union[TaskConfig, List[TaskConfig]], **properties) -> "PipelineConfig":
         """Configure the default values for pipeline configurations.
 
         This function creates the *default pipeline configuration* object,
@@ -112,8 +114,9 @@
                 a single task configuration object is this pipeline holds a single task.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The default pipeline configuration.
         """
         section = PipelineConfig(_Config.DEFAULT_KEY, task_configs, **properties)
         Config._register(section)
+        _warn_deprecated("PipelineConfig")
         return Config.sections[PipelineConfig.name][_Config.DEFAULT_KEY]
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/scenario_config.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/scenario_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from taipy.config._config import _Config
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 from taipy.config.common._validate_id import _validate_id
 from taipy.config.common.frequency import Frequency
 from taipy.config.config import Config
 from taipy.config.section import Section
 
+from ..common._warnings import _warn_deprecated
 from .pipeline_config import PipelineConfig
 from .task_config import TaskConfig
 
 
 class ScenarioConfig(Section):
     """
     Configuration fields needed to instantiate an actual `Scenario^`.
@@ -68,18 +69,20 @@
         return ScenarioConfig(self.id, copy(self._pipelines), self.frequency, copy(comp), **copy(self._properties))
 
     def __getattr__(self, item: str) -> Optional[Any]:
         return _tpl._replace_templates(self._properties.get(item))
 
     @property
     def pipeline_configs(self) -> List[PipelineConfig]:
+        _warn_deprecated("PipelineConfig")
         return self._pipelines
 
     @property
     def pipelines(self) -> List[PipelineConfig]:
+        _warn_deprecated("PipelineConfig")
         return self._pipelines
 
     @classmethod
     def default_config(cls):
         return ScenarioConfig(cls._DEFAULT_KEY, [], None, dict())
 
     def _to_dict(self):
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/config/task_config.py` & `taipy-core-2.3.0.dev1/src/taipy/core/config/task_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/cycle.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/cycle/cycle_id.py` & `taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os
 from typing import Dict, Iterable, Optional, Set, Union
 
 from taipy.config._config import _Config
 from taipy.config.common.scope import Scope
 from taipy.config.config import Config
 
-from .._backup._backup import append_to_backup_file, remove_from_backup_file
+from .._backup._backup import _append_to_backup_file, _remove_from_backup_file
 from .._manager._manager import _Manager
 from .._version._version_manager_factory import _VersionManagerFactory
 from ..config.data_node_config import DataNodeConfig
 from ..cycle.cycle_id import CycleId
 from ..exceptions.exceptions import InvalidDataNodeType
 from ..notification import EventEntityType, EventOperation, _publish_event
 from ..pipeline.pipeline_id import PipelineId
@@ -70,15 +70,15 @@
     @classmethod
     def _create_and_set(
         cls, data_node_config: DataNodeConfig, owner_id: Optional[str], parent_ids: Optional[Set[str]]
     ) -> DataNode:
         data_node = cls.__create(data_node_config, owner_id, parent_ids)
         cls._set(data_node)
         if isinstance(data_node, _AbstractFileDataNode):
-            append_to_backup_file(new_file_path=data_node._path)
+            _append_to_backup_file(new_file_path=data_node._path)
         _publish_event(cls._EVENT_ENTITY_TYPE, data_node.id, EventOperation.CREATION, None)
         return data_node
 
     @classmethod
     def __create(
         cls, data_node_config: DataNodeConfig, owner_id: Optional[str], parent_ids: Optional[Set[str]]
     ) -> DataNode:
@@ -115,47 +115,47 @@
     def _clean_pickle_files(cls, data_nodes: Iterable[DataNode]):
         for data_node in data_nodes:
             cls._clean_pickle_file(data_node)
 
     @classmethod
     def _remove_dn_file_path_in_backup_file(cls, data_node: DataNode):
         if isinstance(data_node, _AbstractFileDataNode):
-            remove_from_backup_file(to_remove_file_path=data_node.path)
+            _remove_from_backup_file(to_remove_file_path=data_node.path)
 
     @classmethod
     def _remove_dn_file_paths_in_backup_file(cls, data_nodes: Iterable[DataNode]):
         for data_node in data_nodes:
             if isinstance(data_node, _AbstractFileDataNode):
-                remove_from_backup_file(to_remove_file_path=data_node.path)
+                _remove_from_backup_file(to_remove_file_path=data_node.path)
 
     @classmethod
     def _delete(cls, data_node_id: DataNodeId):
         data_node = cls._get(data_node_id, None)
-        super()._delete(data_node_id)
         if data_node:
             cls._clean_pickle_file(data_node)
             cls._remove_dn_file_path_in_backup_file(data_node)
+        super()._delete(data_node_id)
 
     @classmethod
     def _delete_many(cls, data_node_ids: Iterable[DataNodeId]):
         data_nodes = []
         for data_node_id in data_node_ids:
             if data_node := cls._get(data_node_id):
                 data_nodes.append(data_node)
-        super()._delete_many(data_node_ids)
         cls._clean_pickle_files(data_nodes)
         cls._remove_dn_file_paths_in_backup_file(data_nodes)
+        super()._delete_many(data_node_ids)
 
     @classmethod
     def _delete_all(cls):
         data_nodes = cls._get_all()
-        super()._delete_all()
         cls._clean_pickle_files(data_nodes)
         cls._remove_dn_file_paths_in_backup_file(data_nodes)
+        super()._delete_all()
 
     @classmethod
     def _delete_by_version(cls, version_number: str):
         data_nodes = cls._get_all(version_number)
-        cls._repository._delete_by(attribute="version", value=version_number, version_number="all")
         cls._clean_pickle_files(data_nodes)
         cls._remove_dn_file_paths_in_backup_file(data_nodes)
+        cls._repository._delete_by(attribute="version", value=version_number, version_number="all")
         _publish_event(cls._EVENT_ENTITY_TYPE, None, EventOperation.DELETION, None)
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 # specific language governing permissions and limitations under the License.
 
 import pathlib
 from datetime import datetime, timedelta
 from pydoc import locate
 from typing import Any, Dict, Iterable, List, Optional, Union
 
+from taipy.config.common.scope import Scope
+
 from .._repository._repository import _AbstractRepository
 from .._repository._repository_adapter import _RepositoryAdapter
 from ..common._utils import _load_fct
+from ..common._warnings import _warn_deprecated
 from ._data_model import _DataNodeModel
 from .data_node import DataNode
 from .generic import GenericDataNode
 from .json import JSONDataNode
 from .sql import SQLDataNode
 
 
@@ -201,14 +204,18 @@
                 model.data_node_properties[self._CUSTOM_DOCUMENT_KEY] = locate(
                     model.data_node_properties[self._CUSTOM_DOCUMENT_KEY]
                 )
 
         validity_period = None
         if model.validity_seconds is not None and model.validity_days is not None:
             validity_period = timedelta(days=model.validity_days, seconds=model.validity_seconds)
+
+        if model.scope == Scope.PIPELINE:
+            _warn_deprecated(f"`{Scope.PIPELINE}`", suggest="other `Scope` value")
+
         return self.class_map[model.storage_type](
             config_id=model.config_id,
             scope=model.scope,
             id=model.id,
             name=model.name,
             owner_id=model.owner_id,
             parent_ids=set(model.parent_ids),
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/_filter.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/abstract_file.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_file.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/abstract_sql.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/csv.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from typing import Any, Dict, List, Optional, Set
 
 import modin.pandas as modin_pd
 import pandas as pd
 
 from taipy.config.common.scope import Scope
 
-from .._backup._backup import replace_in_backup_file
+from .._backup._backup import _replace_in_backup_file
 from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
 from ..exceptions.exceptions import InvalidExposedType
 from ..job.job_id import JobId
 from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
 from .data_node_id import DataNodeId, Edit
@@ -41,17 +41,19 @@
         name (str): A user-readable name of this data node.
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         path (str): The path to the CSV file.
         properties (dict[str, Any]): A dictionary of additional properties. The _properties_
             must have a _"default_path"_ or _"path"_ entry with the path of the CSV file:
 
             - _"default_path"_ `(str)`: The default path of the CSV file.\n
@@ -132,15 +134,15 @@
         return self._path
 
     @path.setter
     def path(self, value):
         tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
-        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
+        _replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     def _check_exposed_type(self, exposed_type):
         if isinstance(exposed_type, str) and exposed_type not in self.__VALID_STRING_EXPOSED_TYPES:
             raise InvalidExposedType(
                 f"Invalid string exposed type {exposed_type}. Supported values are "
                 f"{', '.join(self.__VALID_STRING_EXPOSED_TYPES)}"
             )
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/data_node.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/data_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,19 @@
             None.
         parent_ids (Optional[Set[str]]): The set of identifiers of the parent tasks.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The list of Edits (an alias for dict) containing medata about each
             edition of that node.
         version (str): The string indicates the application version of the data node to
             instantiate. If not provided, the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If *validity_period* is set to None, the data node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if the data node is locked for modification. False
             otherwise.
         kwargs: A dictionary of additional properties.
     """
 
     _ID_PREFIX = "DATANODE"
     __ID_SEPARATOR = "_"
@@ -174,14 +176,16 @@
     def last_edition_date(self, val):
         _warn_deprecated("last_edition_date", suggest="last_edit_date")
         self.last_edit_date = val
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def scope(self):
+        if self._scope == Scope.PIPELINE:
+            _warn_deprecated(f"`{Scope.PIPELINE}`", suggest="other `Scope` value")
         return self._scope
 
     @scope.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def scope(self, val):
         self._scope = val
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/data_node_id.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/data_node_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/excel.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/excel.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import modin.pandas as modin_pd
 import numpy as np
 import pandas as pd
 from openpyxl import load_workbook
 
 from taipy.config.common.scope import Scope
 
-from .._backup._backup import replace_in_backup_file
+from .._backup._backup import _replace_in_backup_file
 from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
 from ..exceptions.exceptions import ExposedTypeLengthMismatch, InvalidExposedType, NonExistingExcelSheet
 from ..job.job_id import JobId
 from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
 from .data_node_id import DataNodeId, Edit
@@ -45,17 +45,19 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
             `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         path (str): The path to the Excel file.
         properties (dict[str, Any]): A dictionary of additional properties. The _properties_
             must have a _"default_path"_ or _"path"_ entry with the path of the Excel file:
 
             - _"default_path"_ `(str)`: The path of the Excel file.\n
@@ -138,15 +140,15 @@
         return self._path
 
     @path.setter
     def path(self, value):
         tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
-        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
+        _replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     @classmethod
     def storage_type(cls) -> str:
         return cls.__STORAGE_TYPE
 
     def _check_exposed_type(self, exposed_type):
         if isinstance(exposed_type, str) and exposed_type not in self.__VALID_STRING_EXPOSED_TYPES:
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/generic.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,17 +34,19 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
             `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. Note that the
             _properties_ parameter must at least contain an entry for either _"read_fct"_ or
             _"write_fct"_ representing the read and write functions.
             Entries for _"read_fct_args"_ and _"write_fct_args"_ respectively represent
             potential parameters for the _"read_fct"_ and _"write_fct"_ functions.
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/in_memory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/in_memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,17 +38,19 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
             `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. When creating an
             _In Memory_ data node, if the _properties_ dictionary contains a _"default_data"_
             entry, the data node is automatically written with the corresponding _"default_data"_
             value.
     """
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/json.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from enum import Enum
 from os.path import isfile
 from pydoc import locate
 from typing import Any, Dict, List, Optional, Set
 
 from taipy.config.common.scope import Scope
 
-from .._backup._backup import replace_in_backup_file
+from .._backup._backup import _replace_in_backup_file
 from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
 from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
 from .data_node_id import DataNodeId, Edit
 
 
@@ -39,17 +39,19 @@
         name (str): A user-readable name of this data node.
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         path (str): The path to the JSON file.
         encoder (json.JSONEncoder): The JSON encoder that is used to write into the JSON file.
         decoder (json.JSONDecoder): The JSON decoder that is used to read from the JSON file.
         properties (dict[str, Any]): A dictionary of additional properties. The _properties_
             must have a _"default_path"_ or _"path"_ entry with the path of the JSON file.
@@ -121,15 +123,15 @@
         return self._path
 
     @path.setter
     def path(self, value):
         tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
-        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
+        _replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def encoder(self):
         return self._encoder
 
     @encoder.setter
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/mongo.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/mongo.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,19 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
             None.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. Note that the
             _properties_ parameter must at least contain an entry for _"db_name"_ and _"collection_name"_:
 
             - _"db_name"_ `(str)`: The database name.\n
             - _"collection_name"_ `(str)`: The collection in the database to read from and to write the data to.\n
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/operator.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/parquet.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Any, Dict, List, Optional, Set
 
 import modin.pandas as modin_pd
 import pandas as pd
 
 from taipy.config.common.scope import Scope
 
-from .._backup._backup import replace_in_backup_file
+from .._backup._backup import _replace_in_backup_file
 from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
 from ..exceptions.exceptions import InvalidExposedType, UnknownCompressionAlgorithm, UnknownParquetEngine
 from ..job.job_id import JobId
 from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
 from .data_node_id import DataNodeId, Edit
@@ -40,17 +40,19 @@
         name (str): A user-readable name of this data node.
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If *validity_period* is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         path (str): The path to the Parquet file.
         properties (dict[str, Any]): A dictionary of additional properties. *properties*
             must have a *"default_path"* or *"path"* entry with the path of the Parquet file:
 
             - *"default_path"* (`str`): The default path of the Parquet file.
@@ -174,15 +176,15 @@
         return self._path
 
     @path.setter
     def path(self, value):
         tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
-        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
+        _replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     def _check_exposed_type(self, exposed_type):
         if isinstance(exposed_type, str) and exposed_type not in self.__VALID_STRING_EXPOSED_TYPES:
             raise InvalidExposedType(
                 f"Invalid string exposed type {exposed_type}. Supported values are "
                 f"{', '.join(self.__VALID_STRING_EXPOSED_TYPES)}"
             )
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/pickle.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/pickle.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from datetime import datetime, timedelta
 from typing import Any, List, Optional, Set
 
 import modin.pandas as pd
 
 from taipy.config.common.scope import Scope
 
-from .._backup._backup import replace_in_backup_file
+from .._backup._backup import _replace_in_backup_file
 from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
 from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
 from .data_node_id import DataNodeId, Edit
 
 
@@ -38,17 +38,19 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
             `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties.
             When creating a pickle data node, if the _properties_ dictionary contains a
             _"default_data"_ entry, the data node is automatically written with the corresponding
             _"default_data"_ value.
             If the _properties_ dictionary contains a _"default_path"_ or _"path"_ entry, the data will be stored
@@ -117,15 +119,15 @@
 
     @path.setter  # type: ignore
     def path(self, value):
         tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
         self.properties[self.__IS_GENERATED_KEY] = False
-        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
+        _replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def is_generated(self) -> bool:
         return self._is_generated
 
     def _read(self):
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/sql.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,19 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
             None.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. Note that the
             _properties_ parameter must at least contain an entry for _"db_name"_, _"db_engine"_, _"read_query"_,
             and _"write_query_builder"_:
 
             - _"db_name"_ `(str)`: The database name, or the name of the SQLite database file.
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/data/sql_table.py` & `taipy-core-2.3.0.dev1/src/taipy/core/data/sql_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,19 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
             None.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
-        validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
-            always up-to-date.
+        validity_period (Optional[timedelta]): The duration implemented as a timedelta since the last edit date for
+            which the data node can be considered up-to-date. Once the validity period has passed, the data node is
+            considered stale and relevant tasks will run even if they are skippable (see the
+            [Task management page](../core/entities/task-mgt.md) for more details).
+            If _validity_period_ is set to `None`, the data node is always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. Note that the
             _properties_ parameter must at least contain an entry for _"db_name"_, _"db_engine"_, _"table_name"_:
 
             - _"db_name"_ `(str)`: The database name, or the name of the SQLite database file.
             - _"db_engine"_ `(str)`: The database engine. For now, the accepted values are _"sqlite"_, _"mssql"_,
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/exceptions/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/exceptions/exceptions.py` & `taipy-core-2.3.0.dev1/src/taipy/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import pathlib
 from datetime import datetime
 from typing import Any, Iterable, List, Optional, Union
 
 from taipy.logger._taipy_logger import _TaipyLogger
 
+from .._orchestrator.utils import migrate_subscriber
 from .._repository._repository import _AbstractRepository
 from .._repository._repository_adapter import _RepositoryAdapter
 from ..common._utils import _fcts_to_dict, _load_fct
 from ..exceptions.exceptions import InvalidSubscriber
 from ..task._task_repository_factory import _TaskRepositoryFactory
 from ._job_model import _JobModel
 from .job import Job
@@ -55,19 +56,20 @@
         )
 
         job._status = model.status
         job._force = model.force
         job._creation_date = datetime.fromisoformat(model.creation_date)  # type: ignore
         for it in model.subscribers:
             try:
-                job._subscribers.append(_load_fct(it.get("fct_module"), it.get("fct_name")))  # type:ignore
+                # Migrate from taipy-core 2.2 to taipy-core 2.3
+                fct_module, fct_name = migrate_subscriber(it.get("fct_module"), it.get("fct_name"))
+                job._subscribers.append(_load_fct(fct_module, fct_name))  # type:ignore
             except AttributeError:
                 raise InvalidSubscriber(f"The subscriber function {it.get('fct_name')} cannot be loaded.")
         job._stacktrace = model.stacktrace
-
         return job
 
     def load(self, model_id: str) -> Job:
         return self.repo.load(model_id)
 
     def _load_all(self, version_number: Optional[str] = None) -> List[Job]:
         return self.repo._load_all(version_number)
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/job.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/job_id.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/job_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/job/status.py` & `taipy-core-2.3.0.dev1/src/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/notification/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/notification/core_event_consumer.py` & `taipy-core-2.3.0.dev1/src/taipy/core/notification/core_event_consumer.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/notification/event.py` & `taipy-core-2.3.0.dev1/src/taipy/core/notification/event.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/notification/notifier.py` & `taipy-core-2.3.0.dev1/src/taipy/core/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/notification/registration.py` & `taipy-core-2.3.0.dev1/src/taipy/core/notification/registration.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/notification/registration_id.py` & `taipy-core-2.3.0.dev1/src/taipy/core/notification/registration_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/notification/topic.py` & `taipy-core-2.3.0.dev1/src/taipy/core/notification/topic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/pipeline.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/pipeline_id.py` & `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,14 @@
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def name(self) -> Optional[str]:
         return self._properties.get("name")
 
     @name.setter  # type: ignore
-    @_self_setter(_MANAGER_NAME)
     def name(self, val):
         self._properties["name"] = val
 
     def has_tag(self, tag: str) -> bool:
         """Indicate if the scenario has a given tag.
 
         Parameters:
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario_id.py` & `taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/taipy.py` & `taipy-core-2.3.0.dev1/src/taipy/core/taipy.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/__init__.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_model.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/task.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,16 +164,18 @@
         """Retrieve the lowest scope of the task based on its data nodes.
 
         Returns:
             The lowest scope present in input and output data nodes or GLOBAL if there are
                 either no input or no output.
         """
         data_nodes = list(self.__input.values()) + list(self.__output.values())
-        scope = min(dn.scope for dn in data_nodes) if len(data_nodes) != 0 else Scope.GLOBAL
-        return Scope(scope)
+        scope = Scope(min(dn.scope for dn in data_nodes)) if len(data_nodes) != 0 else Scope.GLOBAL
+        if scope == Scope.PIPELINE:
+            _warn_deprecated(f"`{Scope.PIPELINE}`", suggest="other `Scope` value")
+        return scope
 
     @property  # type: ignore
     def version(self):
         return self._version
 
     def submit(
         self,
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy/core/task/task_id.py` & `taipy-core-2.3.0.dev1/src/taipy/core/task/task_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-2.3.0.dev1/src/taipy_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev0
+Version: 2.3.0.dev1
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev0/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-2.3.0.dev1/src/taipy_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/taipy/core/_manager/__init__.py
 src/taipy/core/_manager/_manager.py
 src/taipy/core/_manager/_manager_factory.py
 src/taipy/core/_orchestrator/__init__.py
 src/taipy/core/_orchestrator/_abstract_orchestrator.py
 src/taipy/core/_orchestrator/_orchestrator.py
 src/taipy/core/_orchestrator/_orchestrator_factory.py
+src/taipy/core/_orchestrator/utils.py
 src/taipy/core/_orchestrator/_dispatcher/__init__.py
 src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
 src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
 src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
 src/taipy/core/_repository/__init__.py
 src/taipy/core/_repository/_filesystem_repository.py
 src/taipy/core/_repository/_repository.py
@@ -64,14 +65,15 @@
 src/taipy/core/config/job_config.py
 src/taipy/core/config/pipeline_config.py
 src/taipy/core/config/scenario_config.py
 src/taipy/core/config/task_config.py
 src/taipy/core/config/checkers/__init__.py
 src/taipy/core/config/checkers/_config_id_checker.py
 src/taipy/core/config/checkers/_data_node_config_checker.py
+src/taipy/core/config/checkers/_global_config_checker.py
 src/taipy/core/config/checkers/_job_config_checker.py
 src/taipy/core/config/checkers/_pipeline_config_checker.py
 src/taipy/core/config/checkers/_scenario_config_checker.py
 src/taipy/core/config/checkers/_task_config_checker.py
 src/taipy/core/cycle/__init__.py
 src/taipy/core/cycle/_cycle_fs_repository.py
 src/taipy/core/cycle/_cycle_manager.py
```

### Comparing `taipy-core-2.3.0.dev0/tests/test_complex_application.py` & `taipy-core-2.3.0.dev1/tests/test_complex_application.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev0/tests/test_taipy.py` & `taipy-core-2.3.0.dev1/tests/test_taipy.py`

 * *Files identical despite different names*

